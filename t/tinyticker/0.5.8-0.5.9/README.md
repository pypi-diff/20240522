# Comparing `tmp/tinyticker-0.5.8.tar.gz` & `tmp/tinyticker-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinyticker-0.5.8.tar", max compression
+gzip compressed data, was "tinyticker-0.5.9.tar", max compression
```

## Comparing `tinyticker-0.5.8.tar` & `tinyticker-0.5.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     1068 2024-05-21 01:55:21.895522 tinyticker-0.5.8/LICENSE
--rw-r--r--   0        0        0     3858 2024-05-21 01:55:21.895522 tinyticker-0.5.8/README.md
--rw-r--r--   0        0        0      917 2024-05-21 01:55:21.895522 tinyticker-0.5.8/pyproject.toml
--rw-r--r--   0        0        0      207 2024-05-21 01:55:21.895522 tinyticker-0.5.8/tinyticker/__init__.py
--rw-r--r--   0        0        0     6145 2024-05-21 01:55:21.895522 tinyticker-0.5.8/tinyticker/__main__.py
--rw-r--r--   0        0        0     2470 2024-05-21 01:55:21.895522 tinyticker-0.5.8/tinyticker/config.py
--rw-r--r--   0        0        0     8857 2024-05-21 01:55:21.895522 tinyticker-0.5.8/tinyticker/display.py
--rw-r--r--   0        0        0      345 2024-05-21 01:55:21.895522 tinyticker-0.5.8/tinyticker/paths.py
--rw-r--r--   0        0        0    15671 2024-05-21 01:55:21.895522 tinyticker-0.5.8/tinyticker/ticker.py
--rw-r--r--   0        0        0     2391 2024-05-21 01:55:21.895522 tinyticker-0.5.8/tinyticker/utils.py
--rw-r--r--   0        0        0      278 2024-05-21 01:55:21.895522 tinyticker-0.5.8/tinyticker/waveshare_lib/__init__.py
--rw-r--r--   0        0        0     1297 2024-05-21 01:55:21.895522 tinyticker-0.5.8/tinyticker/waveshare_lib/_base.py
--rw-r--r--   0        0        0     4104 2024-05-21 01:55:21.895522 tinyticker-0.5.8/tinyticker/waveshare_lib/device.py
--rw-r--r--   0        0        0     8593 2024-05-21 01:55:21.899522 tinyticker-0.5.8/tinyticker/waveshare_lib/epd2in13.py
--rw-r--r--   0        0        0    12127 2024-05-21 01:55:21.899522 tinyticker-0.5.8/tinyticker/waveshare_lib/epd2in13_V2.py
--rw-r--r--   0        0        0    14828 2024-05-21 01:55:21.899522 tinyticker-0.5.8/tinyticker/waveshare_lib/epd2in13_V3.py
--rw-r--r--   0        0        0    10709 2024-05-21 01:55:21.899522 tinyticker-0.5.8/tinyticker/waveshare_lib/epd2in13_V4.py
--rw-r--r--   0        0        0     6057 2024-05-21 01:55:21.899522 tinyticker-0.5.8/tinyticker/waveshare_lib/epd2in13b_V3.py
--rw-r--r--   0        0        0     6860 2024-05-21 01:55:21.899522 tinyticker-0.5.8/tinyticker/waveshare_lib/epd2in13b_V4.py
--rw-r--r--   0        0        0     5907 2024-05-21 01:55:21.899522 tinyticker-0.5.8/tinyticker/waveshare_lib/epd2in13bc.py
--rw-r--r--   0        0        0     1283 2024-05-21 01:55:21.899522 tinyticker-0.5.8/tinyticker/waveshare_lib/models.py
--rw-r--r--   0        0        0       95 2024-05-21 01:55:21.899522 tinyticker-0.5.8/tinyticker/web/__init__.py
--rw-r--r--   0        0        0     2598 2024-05-21 01:55:21.899522 tinyticker-0.5.8/tinyticker/web/__main__.py
--rw-r--r--   0        0        0     6643 2024-05-21 01:55:21.899522 tinyticker-0.5.8/tinyticker/web/app.py
--rw-r--r--   0        0        0     2909 2024-05-21 01:55:21.899522 tinyticker-0.5.8/tinyticker/web/command.py
--rw-r--r--   0        0        0   274777 2024-05-21 01:55:21.899522 tinyticker-0.5.8/tinyticker/web/templates/css/uikit.min.css
--rw-r--r--   0        0        0    12844 2024-05-21 01:55:21.899522 tinyticker-0.5.8/tinyticker/web/templates/images/apple-touch-icon.png
--rw-r--r--   0        0        0      742 2024-05-21 01:55:21.899522 tinyticker-0.5.8/tinyticker/web/templates/images/favicon-16x16.png
--rw-r--r--   0        0        0     1645 2024-05-21 01:55:21.899522 tinyticker-0.5.8/tinyticker/web/templates/images/favicon-32x32.png
--rw-r--r--   0        0        0    14553 2024-05-21 01:55:21.899522 tinyticker-0.5.8/tinyticker/web/templates/index.html
--rw-r--r--   0        0        0     1573 2024-05-21 01:55:21.899522 tinyticker-0.5.8/tinyticker/web/templates/js/index.js
--rw-r--r--   0        0        0    65291 2024-05-21 01:55:21.899522 tinyticker-0.5.8/tinyticker/web/templates/js/uikit-icons.min.js
--rw-r--r--   0        0        0   136629 2024-05-21 01:55:21.899522 tinyticker-0.5.8/tinyticker/web/templates/js/uikit.min.js
--rw-r--r--   0        0        0     2349 2024-05-21 01:55:21.899522 tinyticker-0.5.8/tinyticker/web/templates/logfiles.html
--rw-r--r--   0        0        0     5147 1970-01-01 00:00:00.000000 tinyticker-0.5.8/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-05-21 12:21:05.681176 tinyticker-0.5.9/LICENSE
+-rw-r--r--   0        0        0     3858 2024-05-21 12:21:05.681176 tinyticker-0.5.9/README.md
+-rw-r--r--   0        0        0      917 2024-05-21 12:21:05.685176 tinyticker-0.5.9/pyproject.toml
+-rw-r--r--   0        0        0      207 2024-05-21 12:21:05.685176 tinyticker-0.5.9/tinyticker/__init__.py
+-rw-r--r--   0        0        0     5908 2024-05-21 12:21:05.685176 tinyticker-0.5.9/tinyticker/__main__.py
+-rw-r--r--   0        0        0     2470 2024-05-21 12:21:05.685176 tinyticker-0.5.9/tinyticker/config.py
+-rw-r--r--   0        0        0     8857 2024-05-21 12:21:05.685176 tinyticker-0.5.9/tinyticker/display.py
+-rw-r--r--   0        0        0      345 2024-05-21 12:21:05.685176 tinyticker-0.5.9/tinyticker/paths.py
+-rw-r--r--   0        0        0    15671 2024-05-21 12:21:05.685176 tinyticker-0.5.9/tinyticker/ticker.py
+-rw-r--r--   0        0        0     2391 2024-05-21 12:21:05.685176 tinyticker-0.5.9/tinyticker/utils.py
+-rw-r--r--   0        0        0      278 2024-05-21 12:21:05.685176 tinyticker-0.5.9/tinyticker/waveshare_lib/__init__.py
+-rw-r--r--   0        0        0     1297 2024-05-21 12:21:05.685176 tinyticker-0.5.9/tinyticker/waveshare_lib/_base.py
+-rw-r--r--   0        0        0     4104 2024-05-21 12:21:05.685176 tinyticker-0.5.9/tinyticker/waveshare_lib/device.py
+-rw-r--r--   0        0        0     8593 2024-05-21 12:21:05.685176 tinyticker-0.5.9/tinyticker/waveshare_lib/epd2in13.py
+-rw-r--r--   0        0        0    12127 2024-05-21 12:21:05.685176 tinyticker-0.5.9/tinyticker/waveshare_lib/epd2in13_V2.py
+-rw-r--r--   0        0        0    14828 2024-05-21 12:21:05.685176 tinyticker-0.5.9/tinyticker/waveshare_lib/epd2in13_V3.py
+-rw-r--r--   0        0        0    10709 2024-05-21 12:21:05.685176 tinyticker-0.5.9/tinyticker/waveshare_lib/epd2in13_V4.py
+-rw-r--r--   0        0        0     6057 2024-05-21 12:21:05.685176 tinyticker-0.5.9/tinyticker/waveshare_lib/epd2in13b_V3.py
+-rw-r--r--   0        0        0     6860 2024-05-21 12:21:05.685176 tinyticker-0.5.9/tinyticker/waveshare_lib/epd2in13b_V4.py
+-rw-r--r--   0        0        0     5907 2024-05-21 12:21:05.685176 tinyticker-0.5.9/tinyticker/waveshare_lib/epd2in13bc.py
+-rw-r--r--   0        0        0     1283 2024-05-21 12:21:05.685176 tinyticker-0.5.9/tinyticker/waveshare_lib/models.py
+-rw-r--r--   0        0        0       95 2024-05-21 12:21:05.689176 tinyticker-0.5.9/tinyticker/web/__init__.py
+-rw-r--r--   0        0        0     2598 2024-05-21 12:21:05.689176 tinyticker-0.5.9/tinyticker/web/__main__.py
+-rw-r--r--   0        0        0     6643 2024-05-21 12:21:05.689176 tinyticker-0.5.9/tinyticker/web/app.py
+-rw-r--r--   0        0        0     3021 2024-05-21 12:21:05.689176 tinyticker-0.5.9/tinyticker/web/command.py
+-rw-r--r--   0        0        0   274777 2024-05-21 12:21:05.689176 tinyticker-0.5.9/tinyticker/web/templates/css/uikit.min.css
+-rw-r--r--   0        0        0    12844 2024-05-21 12:21:05.689176 tinyticker-0.5.9/tinyticker/web/templates/images/apple-touch-icon.png
+-rw-r--r--   0        0        0      742 2024-05-21 12:21:05.689176 tinyticker-0.5.9/tinyticker/web/templates/images/favicon-16x16.png
+-rw-r--r--   0        0        0     1645 2024-05-21 12:21:05.689176 tinyticker-0.5.9/tinyticker/web/templates/images/favicon-32x32.png
+-rw-r--r--   0        0        0    14649 2024-05-21 12:21:05.689176 tinyticker-0.5.9/tinyticker/web/templates/index.html
+-rw-r--r--   0        0        0     1573 2024-05-21 12:21:05.689176 tinyticker-0.5.9/tinyticker/web/templates/js/index.js
+-rw-r--r--   0        0        0    65291 2024-05-21 12:21:05.689176 tinyticker-0.5.9/tinyticker/web/templates/js/uikit-icons.min.js
+-rw-r--r--   0        0        0   136629 2024-05-21 12:21:05.689176 tinyticker-0.5.9/tinyticker/web/templates/js/uikit.min.js
+-rw-r--r--   0        0        0     2349 2024-05-21 12:21:05.689176 tinyticker-0.5.9/tinyticker/web/templates/logfiles.html
+-rw-r--r--   0        0        0     5147 1970-01-01 00:00:00.000000 tinyticker-0.5.9/PKG-INFO
```

### Comparing `tinyticker-0.5.8/LICENSE` & `tinyticker-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.8/README.md` & `tinyticker-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.8/pyproject.toml` & `tinyticker-0.5.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tinyticker"
-version = "0.5.8"
+version = "0.5.9"
 description = "A tiny Raspberry Pi powered ePaper ticker."
 authors = ["Loic Coyle <loic.coyle@hotmail.fr>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/loiccoyle/tinyticker"
 keywords = ["raspberry-pi", "ticker", "stock", "crypto", "epaper", "finance"]
```

### Comparing `tinyticker-0.5.8/tinyticker/__main__.py` & `tinyticker-0.5.9/tinyticker/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,20 +121,20 @@
             show=True,
             weight="bold",
             fontsize="small",
         )
 
 
 def main():
-    logger.info("Tinyticker version: %s", __version__)
     args = parse_args(sys.argv[1:])
     config_file: Path = args.config
 
     if args.verbose > 0:
         set_verbosity(logger, args.verbose)
+    logger.info("Tinyticker version: %s", __version__)
 
     # make sure the config file exists and can be parsed before setting up the file
     # monitor
     load_config_safe(config_file)
 
     # write the process pid to file.
     pid = os.getpid()
@@ -142,22 +142,14 @@
     logger.info("PID: %s", pid)
     if not PID_FILE.parent.is_dir():
         PID_FILE.parent.mkdir(parents=True, exist_ok=True)
     PID_FILE.write_text(str(pid))
 
     logger.debug("Args: %s", args)
 
-    #  setup signal handlers
-    def restart(*_) -> None:
-        """Restart both the ticker and the main thread."""
-        logger.info("Restarting.")
-        os.execv(sys.argv[0], sys.argv)
-
-    signal.signal(signal.SIGUSR1, restart)
-
     def refresh(*_) -> None:
         """Kill the ticker process, it gets restarted in the main thread."""
         logger.info("Refreshing ticker process.")
         if not tick_process._closed and tick_process.is_alive():  # type: ignore
             tick_process.kill()
             tick_process.join()
             tick_process.close()
```

### Comparing `tinyticker-0.5.8/tinyticker/config.py` & `tinyticker-0.5.9/tinyticker/config.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.8/tinyticker/display.py` & `tinyticker-0.5.9/tinyticker/display.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.8/tinyticker/ticker.py` & `tinyticker-0.5.9/tinyticker/ticker.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.8/tinyticker/utils.py` & `tinyticker-0.5.9/tinyticker/utils.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.8/tinyticker/waveshare_lib/_base.py` & `tinyticker-0.5.9/tinyticker/waveshare_lib/_base.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.8/tinyticker/waveshare_lib/device.py` & `tinyticker-0.5.9/tinyticker/waveshare_lib/device.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.8/tinyticker/waveshare_lib/epd2in13.py` & `tinyticker-0.5.9/tinyticker/waveshare_lib/epd2in13.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.8/tinyticker/waveshare_lib/epd2in13_V2.py` & `tinyticker-0.5.9/tinyticker/waveshare_lib/epd2in13_V2.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.8/tinyticker/waveshare_lib/epd2in13_V3.py` & `tinyticker-0.5.9/tinyticker/waveshare_lib/epd2in13_V3.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.8/tinyticker/waveshare_lib/epd2in13_V4.py` & `tinyticker-0.5.9/tinyticker/waveshare_lib/epd2in13_V4.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.8/tinyticker/waveshare_lib/epd2in13b_V3.py` & `tinyticker-0.5.9/tinyticker/waveshare_lib/epd2in13b_V3.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.8/tinyticker/waveshare_lib/epd2in13b_V4.py` & `tinyticker-0.5.9/tinyticker/waveshare_lib/epd2in13b_V4.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.8/tinyticker/waveshare_lib/epd2in13bc.py` & `tinyticker-0.5.9/tinyticker/waveshare_lib/epd2in13bc.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.8/tinyticker/waveshare_lib/models.py` & `tinyticker-0.5.9/tinyticker/waveshare_lib/models.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.8/tinyticker/web/__main__.py` & `tinyticker-0.5.9/tinyticker/web/__main__.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.8/tinyticker/web/app.py` & `tinyticker-0.5.9/tinyticker/web/app.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.8/tinyticker/web/command.py` & `tinyticker-0.5.9/tinyticker/web/command.py`

 * *Files 10% similar despite different names*

```diff
@@ -46,22 +46,18 @@
     except subprocess.CalledProcessError as exc:
         LOGGER.error("Command failed.")
         LOGGER.error(exc.output.decode("utf8"))
 
 
 @register
 def restart() -> None:
-    """Restart the tinyticker process."""
-    if PID_FILE.is_file():
-        LOGGER.info("Sending SIGUSR1 to tinyticker.")
-        with open(PID_FILE, "r") as pid_file:
-            pid = int(pid_file.readline())
-        os.kill(pid, signal.SIGUSR1)
-    else:
-        LOGGER.info("tinyticker is not runnning.")
+    """Restart the tinyticker and tinyticker-web systemd services."""
+    LOGGER.info("Restarting services.")
+    try_command("systemctl --user restart tinyticker")
+    try_command("systemctl --user restart tinyticker-web")
 
 
 @register
 def refresh() -> None:
     """Refresh tinyticker's ticker process."""
     if PID_FILE.is_file():
         LOGGER.info("Sending SIGUSR2 to tinyticker.")
@@ -86,21 +82,24 @@
     try_command("sudo comitup-cli d")
     reboot()
 
 
 @register
 def update() -> None:
     """Update tinyticker with pip."""
-    args = ["install", "--upgrade", "tinyticker"]
-    # rpi requires an added flag to update system packages
+    # the `--break-system-packages` flag is required to update system packages on rpi
     # https://www.raspberrypi.com/documentation/computers/os.html#about-python-virtual-environments
-    error = pipmain(args + ["--break-system-packages"])
-    if error:
-        # if for some reason we are not running on an rpi, try again without the flag
-        error = pipmain(args)
+    # it should be safe as we are installing in the user pkgs and this user is solely dedicated
+    # to running tinyticker
+    args = ["install", "--user", "--upgrade", "tinyticker", "--break-system-packages"]
+    LOGGER.info(f"Updating tinyticker with: pip {' '.join(args)}")
+    error = pipmain(args)
+    if not error:
+        LOGGER.info("Update successful, restarting the services.")
+        restart()
 
 
 @register
 def default() -> None:
     """Write the default config."""
     LOGGER.info("Setting config to default.")
     TinytickerConfig().to_file(CONFIG_FILE)
```

### Comparing `tinyticker-0.5.8/tinyticker/web/templates/css/uikit.min.css` & `tinyticker-0.5.9/tinyticker/web/templates/css/uikit.min.css`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.8/tinyticker/web/templates/images/apple-touch-icon.png` & `tinyticker-0.5.9/tinyticker/web/templates/images/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.8/tinyticker/web/templates/images/favicon-16x16.png` & `tinyticker-0.5.9/tinyticker/web/templates/images/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.8/tinyticker/web/templates/images/favicon-32x32.png` & `tinyticker-0.5.9/tinyticker/web/templates/images/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.8/tinyticker/web/templates/index.html` & `tinyticker-0.5.9/tinyticker/web/templates/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -51,16 +51,17 @@
           </div>
           <form class="uk-form-stacked" action="/command">
             <button
               type="submit"
               name="command"
               value="update"
               class="uk-button uk-button-primary uk-width-expand uk-margin-small-bottom"
+              uk-tooltip="Update the tinyticker package, will restart once complete."
             >
-              Update
+              Update & Restart
             </button>
           </form>
         </div>
         <div class="uk-width-large">
           <p class="uk-text-large">Config</p>
           <form action="/set_hostname">
             <label class="uk-form-label" for="hostname">Hostname: </label>
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
 🚀 TinyTicker Dashboard 🚀
 🥳 Update available 🥳
-Update
+Update & Restart
 Config
 Hostname:[{{ hostname }}      ][Set & Reboot]
 ===============================================================================
 ePaper display model
 {%- for epd_model_option in epd_model_options -%} {%- if epd_model_option.name
 == epd_model -%}
 {{ epd_model_option.desc }}
```

### Comparing `tinyticker-0.5.8/tinyticker/web/templates/js/index.js` & `tinyticker-0.5.9/tinyticker/web/templates/js/index.js`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.8/tinyticker/web/templates/js/uikit-icons.min.js` & `tinyticker-0.5.9/tinyticker/web/templates/js/uikit-icons.min.js`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.8/tinyticker/web/templates/js/uikit.min.js` & `tinyticker-0.5.9/tinyticker/web/templates/js/uikit.min.js`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.8/tinyticker/web/templates/logfiles.html` & `tinyticker-0.5.9/tinyticker/web/templates/logfiles.html`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.8/PKG-INFO` & `tinyticker-0.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinyticker
-Version: 0.5.8
+Version: 0.5.9
 Summary: A tiny Raspberry Pi powered ePaper ticker.
 Home-page: https://github.com/loiccoyle/tinyticker
 License: MIT
 Keywords: raspberry-pi,ticker,stock,crypto,epaper,finance
 Author: Loic Coyle
 Author-email: loic.coyle@hotmail.fr
 Requires-Python: >=3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tinyticker Version: 0.5.8 Summary: A tiny Raspberry
+Metadata-Version: 2.1 Name: tinyticker Version: 0.5.9 Summary: A tiny Raspberry
 Pi powered ePaper ticker. Home-page: https://github.com/loiccoyle/tinyticker
 License: MIT Keywords: raspberry-pi,ticker,stock,crypto,epaper,finance Author:
 Loic Coyle Author-email: loic.coyle@hotmail.fr Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
```

