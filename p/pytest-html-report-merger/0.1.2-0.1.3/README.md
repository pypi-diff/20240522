# Comparing `tmp/pytest_html_report_merger-0.1.2.tar.gz` & `tmp/pytest_html_report_merger-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_html_report_merger-0.1.2.tar", max compression
+gzip compressed data, was "pytest_html_report_merger-0.1.3.tar", max compression
```

## Comparing `pytest_html_report_merger-0.1.2.tar` & `pytest_html_report_merger-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1072 2023-10-23 02:30:07.756496 pytest_html_report_merger-0.1.2/LICENSE
--rw-r--r--   0        0        0       83 2023-10-23 02:30:07.756496 pytest_html_report_merger-0.1.2/README.md
--rw-r--r--   0        0        0      853 2023-10-23 02:30:08.784508 pytest_html_report_merger-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       22 2023-10-23 02:30:07.756496 pytest_html_report_merger-0.1.2/src/pytest_html_report_merger/__init__.py
--rw-r--r--   0        0        0     7962 2023-10-23 02:30:07.756496 pytest_html_report_merger-0.1.2/src/pytest_html_report_merger/__main__.py
--rw-r--r--   0        0        0      559 1970-01-01 00:00:00.000000 pytest_html_report_merger-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-22 12:19:16.942581 pytest_html_report_merger-0.1.3/LICENSE
+-rw-r--r--   0        0        0      366 2024-05-22 12:19:16.942581 pytest_html_report_merger-0.1.3/README.md
+-rw-r--r--   0        0        0      875 2024-05-22 12:19:18.058588 pytest_html_report_merger-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-05-22 12:19:16.942581 pytest_html_report_merger-0.1.3/src/pytest_html_report_merger/__init__.py
+-rw-r--r--   0        0        0     8993 2024-05-22 12:19:16.942581 pytest_html_report_merger-0.1.3/src/pytest_html_report_merger/__main__.py
+-rw-r--r--   0        0        0      893 1970-01-01 00:00:00.000000 pytest_html_report_merger-0.1.3/PKG-INFO
```

### Comparing `pytest_html_report_merger-0.1.2/LICENSE` & `pytest_html_report_merger-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_html_report_merger-0.1.2/pyproject.toml` & `pytest_html_report_merger-0.1.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytest_html_report_merger"
-version = "0.1.2"
+version = "0.1.3"
 description = ""
 authors = ["dskard"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
@@ -12,14 +12,15 @@
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.6.0"
 pytest = "^7.1.2"
 pdbpp = "^0.10.3"
 python-semantic-release = "^7.31.4"
 pre-commit = "^3.5.0"
+pytest-html = "4.0.2"
 
 [tool.poetry.scripts]
 pytest-html-report-merger = "pytest_html_report_merger.__main__:cli"
 
 [tool.semantic_release]
 version_variable = [
     "src/pytest_html_report_merger/__init__.py:__version__"
```

### Comparing `pytest_html_report_merger-0.1.2/src/pytest_html_report_merger/__main__.py` & `pytest_html_report_merger-0.1.3/src/pytest_html_report_merger/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -55,14 +55,49 @@
         based on https://stackoverflow.com/a/28503916
         """
 
         minutes, seconds = divmod(td.total_seconds(), 60)
         hours, minutes = divmod(minutes, 60)
         return "{:02d}:{:02d}:{:02d}".format(int(hours), int(minutes), int(seconds))
 
+    def _parse_summary(self, report):
+        # use a regular expression to find a string like:
+        # 402 tests took 09:40:47.
+        # this string shows up if test cases were run
+        element = report.select(".run-count")[0]
+        pattern = r"(\d+) tests{0,1} took (\d{2}):(\d{2}):(\d{2})"
+        matches = re.search(pattern, element.string)
+        if matches is not None:
+            total_tests = int(matches.groups()[0])
+            (t_hour, t_minute, t_second) = matches.groups()[1:4]
+            total_time_delta = datetime.timedelta(
+                hours=int(t_hour), minutes=int(t_minute), seconds=int(t_second)
+            )
+        else:
+            # use a regular expression to look for a string like:
+            # 0 test took 0 ms.
+            # this string shows up if there were no tests run.
+            # i think the units will always be ms
+            pattern = r"(\d+) tests{0,1} took (\d+)"
+            matches = re.search(pattern, element.string)
+            if matches is not None:
+                total_tests = int(matches.groups()[0])
+                t_ms = int(matches.groups()[1])
+                total_time_delta = datetime.timedelta(seconds=t_ms * 1000)
+            else:
+                # TODO:
+                # there is a bigger problem with our regular expressions we have
+                # to investigate. for now, we don't fail because it is more
+                # important that we get the merged results than get the number of
+                # tests correct.
+                total_tests = 0
+                total_time_delta = datetime.timedelta(seconds=0)
+
+        return (total_tests, total_time_delta)
+
     def process_report(self, report_path):
         # open the first html file
         html_doc = ""
         with open(report_path, "r") as f:
             html_doc = f.read()
         soup = bs4.BeautifulSoup(html_doc, features="html.parser")
 
@@ -98,41 +133,26 @@
         # that allows the seconds to be 60, which datetime.datetime.strptime()
         # cannot parse. when that gets fixed, we can use lines like these
         # matches = re.search(r"(\d+) tests took (\d{2}):(\d{2}):(\d{2})", base_element.string)
         # base_total_time_str = matches.groups()[1]
         # t = datetime.datetime.strptime(base_total_time_str,"%H:%M:%S")
 
         # parse the number of tests and timings from the base report
-        base_element = self.base.select(".run-count")[0]
-        matches = re.search(
-            r"(\d+) tests took (\d{2}):(\d{2}):(\d{2})", base_element.string
-        )
-        base_total_tests = int(matches.groups()[0])
-        (t_hour, t_minute, t_second) = matches.groups()[1:4]
-        base_total_time_delta = datetime.timedelta(
-            hours=int(t_hour), minutes=int(t_minute), seconds=int(t_second)
-        )
+        (base_total_tests, base_total_time_delta) = self._parse_summary(self.base)
 
         # parse the number of tests and timings from the provided report
-        soup_element = soup.select(".run-count")[0]
-        matches = re.search(
-            r"(\d+) tests took (\d{2}):(\d{2}):(\d{2})", soup_element.string
-        )
-        soup_total_tests = int(matches.groups()[0])
-        (t_hour, t_minute, t_second) = matches.groups()[1:4]
-        soup_total_time_delta = datetime.timedelta(
-            hours=int(t_hour), minutes=int(t_minute), seconds=int(t_second)
-        )
+        (soup_total_tests, soup_total_time_delta) = self._parse_summary(soup)
 
         # sum up the test count and time deltas
         total_tests = base_total_tests + soup_total_tests
         total_time_delta = base_total_time_delta + soup_total_time_delta
         total_time_str = self._format_time(total_time_delta)
 
         # save the updated total tests and total time.
+        base_element = self.base.select(".run-count")[0]
         base_element.string = f"{total_tests} tests took {total_time_str}."
 
         # parse the filter counts
 
         for key in [
             "passed",
             "skipped",
```

