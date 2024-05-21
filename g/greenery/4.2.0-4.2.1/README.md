# Comparing `tmp/greenery-4.2.0.tar.gz` & `tmp/greenery-4.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "greenery-4.2.0.tar", last modified: Mon Jan  8 23:00:43 2024, max compression
+gzip compressed data, was "greenery-4.2.1.tar", last modified: Tue May 21 23:19:41 2024, max compression
```

## Comparing `greenery-4.2.0.tar` & `greenery-4.2.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2024-01-08 23:00:43.331685 greenery-4.2.0/
--rw-rw-rw-   0        0        0     1082 2022-05-22 15:44:09.000000 greenery-4.2.0/LICENSE.txt
--rw-rw-rw-   0        0        0      498 2024-01-08 23:00:43.329683 greenery-4.2.0/PKG-INFO
--rw-rw-rw-   0        0        0    14246 2024-01-08 22:58:59.000000 greenery-4.2.0/README.md
-drwxrwxrwx   0        0        0        0 2024-01-08 23:00:43.313300 greenery-4.2.0/greenery/
--rw-rw-rw-   0        0        0      414 2024-01-08 22:58:59.000000 greenery-4.2.0/greenery/__init__.py
--rw-rw-rw-   0        0        0     2570 2023-08-03 20:40:33.000000 greenery-4.2.0/greenery/bound.py
--rw-rw-rw-   0        0        0     2841 2023-08-03 20:40:33.000000 greenery-4.2.0/greenery/bound_test.py
--rw-rw-rw-   0        0        0    13684 2023-09-10 17:45:40.000000 greenery-4.2.0/greenery/charclass.py
--rw-rw-rw-   0        0        0     9309 2023-09-10 17:45:40.000000 greenery-4.2.0/greenery/charclass_test.py
--rw-rw-rw-   0        0        0     2518 2023-08-06 19:09:38.000000 greenery-4.2.0/greenery/conc_test.py
--rw-rw-rw-   0        0        0    32612 2024-01-08 22:58:59.000000 greenery-4.2.0/greenery/fsm.py
--rw-rw-rw-   0        0        0    36234 2023-09-10 18:19:52.000000 greenery-4.2.0/greenery/fsm_test.py
--rw-rw-rw-   0        0        0     2413 2023-08-06 23:17:09.000000 greenery-4.2.0/greenery/mult_test.py
--rw-rw-rw-   0        0        0     6601 2023-08-03 20:40:33.000000 greenery-4.2.0/greenery/multiplier.py
--rw-rw-rw-   0        0        0     4342 2023-08-03 20:40:33.000000 greenery-4.2.0/greenery/multiplier_test.py
--rw-rw-rw-   0        0        0     9968 2023-08-06 23:17:09.000000 greenery-4.2.0/greenery/parse.py
--rw-rw-rw-   0        0        0     8003 2023-08-06 23:17:09.000000 greenery-4.2.0/greenery/parse_test.py
--rw-rw-rw-   0        0        0     4579 2023-08-06 19:11:22.000000 greenery-4.2.0/greenery/pattern_test.py
--rw-rw-rw-   0        0        0    32465 2023-09-10 18:19:52.000000 greenery-4.2.0/greenery/rxelems.py
--rw-rw-rw-   0        0        0    44492 2023-08-06 23:17:09.000000 greenery-4.2.0/greenery/rxelems_test.py
-drwxrwxrwx   0        0        0        0 2024-01-08 23:00:43.328674 greenery-4.2.0/greenery.egg-info/
--rw-rw-rw-   0        0        0      498 2024-01-08 23:00:43.000000 greenery-4.2.0/greenery.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      512 2024-01-08 23:00:43.000000 greenery-4.2.0/greenery.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-08 23:00:43.000000 greenery-4.2.0/greenery.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-01-08 23:00:43.000000 greenery-4.2.0/greenery.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-01-08 23:00:43.332686 greenery-4.2.0/setup.cfg
--rw-rw-rw-   0        0        0      979 2024-01-08 22:58:59.000000 greenery-4.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 23:19:41.782009 greenery-4.2.1/
+-rw-rw-rw-   0        0        0     1082 2022-05-22 15:44:10.000000 greenery-4.2.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      498 2024-05-21 23:19:41.782009 greenery-4.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0    14358 2024-05-21 23:18:57.000000 greenery-4.2.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 23:19:41.766209 greenery-4.2.1/greenery/
+-rw-rw-rw-   0        0        0      414 2024-01-08 22:59:00.000000 greenery-4.2.1/greenery/__init__.py
+-rw-rw-rw-   0        0        0     2570 2023-08-03 20:40:34.000000 greenery-4.2.1/greenery/bound.py
+-rw-rw-rw-   0        0        0     2841 2023-08-03 20:40:34.000000 greenery-4.2.1/greenery/bound_test.py
+-rw-rw-rw-   0        0        0    13684 2023-09-10 17:45:42.000000 greenery-4.2.1/greenery/charclass.py
+-rw-rw-rw-   0        0        0     9311 2024-05-21 23:18:57.000000 greenery-4.2.1/greenery/charclass_test.py
+-rw-rw-rw-   0        0        0     2518 2023-08-06 19:09:40.000000 greenery-4.2.1/greenery/conc_test.py
+-rw-rw-rw-   0        0        0    32654 2024-05-21 23:18:57.000000 greenery-4.2.1/greenery/fsm.py
+-rw-rw-rw-   0        0        0    36234 2024-05-21 22:14:47.000000 greenery-4.2.1/greenery/fsm_test.py
+-rw-rw-rw-   0        0        0     2413 2023-08-06 23:17:10.000000 greenery-4.2.1/greenery/mult_test.py
+-rw-rw-rw-   0        0        0     6601 2023-08-03 20:40:34.000000 greenery-4.2.1/greenery/multiplier.py
+-rw-rw-rw-   0        0        0     4342 2023-08-03 20:40:34.000000 greenery-4.2.1/greenery/multiplier_test.py
+-rw-rw-rw-   0        0        0    10433 2024-05-21 23:18:57.000000 greenery-4.2.1/greenery/parse.py
+-rw-rw-rw-   0        0        0     8681 2024-05-21 23:18:57.000000 greenery-4.2.1/greenery/parse_test.py
+-rw-rw-rw-   0        0        0     4579 2023-08-06 19:11:24.000000 greenery-4.2.1/greenery/pattern_test.py
+-rw-rw-rw-   0        0        0    32465 2023-09-10 18:19:54.000000 greenery-4.2.1/greenery/rxelems.py
+-rw-rw-rw-   0        0        0    44492 2024-05-21 22:14:45.000000 greenery-4.2.1/greenery/rxelems_test.py
+drwxrwxrwx   0        0        0        0 2024-05-21 23:19:41.782009 greenery-4.2.1/greenery.egg-info/
+-rw-rw-rw-   0        0        0      498 2024-05-21 23:19:41.000000 greenery-4.2.1/greenery.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      512 2024-05-21 23:19:41.000000 greenery-4.2.1/greenery.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 23:19:41.000000 greenery-4.2.1/greenery.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-21 23:19:41.000000 greenery-4.2.1/greenery.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-21 23:19:41.782009 greenery-4.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      979 2024-05-21 23:18:57.000000 greenery-4.2.1/setup.py
```

### Comparing `greenery-4.2.0/LICENSE.txt` & `greenery-4.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `greenery-4.2.0/README.md` & `greenery-4.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
 * This method is intentionally rigorously simple, and tolerates no ambiguity. For example, a hyphen must be escaped in a character class even if it appears first or last. `[-abc]` is a syntax error, write `[\-abc]`. Escaping something which doesn't need it is a syntax error too: `[\ab]` resolves to neither `[\\ab]` nor `[ab]`.
 
 * The `^` and `$` metacharacters are not supported. By default, `greenery` assumes that all regexes are anchored at the start and end of any input string. Carets and dollar signs will be parsed as themselves. If you want to *not* anchor at the start or end of the string, put `.*` at the start or end of your regex respectively.
 
   This is because computing the intersection between `.*a.*` and `.*b.*` (1) is largely pointless and (2) usually results in gibberish coming out of the program.
 
-* The non-greedy operators `*?`, `+?`, `??` and `{m,n}?` are not supported, since they do not alter the regular language.
+* The non-greedy operators `*?`, `+?`, `??` and `{m,n}?` are permitted but do nothing. This is because they do not alter the regular language. For example, `abc{0,5}def` and `abc{0,5}?def` represent precisely the same set of strings.
 
 * Parentheses are used to alternate between multiple possibilities e.g. `(a|bc)` only, not for capture grouping. Here's why:
 
   ```python
   print(parse("(ab)c") & parse("a(bc)"))
   # "abc"
   ```
```

### Comparing `greenery-4.2.0/greenery/bound.py` & `greenery-4.2.1/greenery/bound.py`

 * *Files identical despite different names*

### Comparing `greenery-4.2.0/greenery/bound_test.py` & `greenery-4.2.1/greenery/bound_test.py`

 * *Files identical despite different names*

### Comparing `greenery-4.2.0/greenery/charclass.py` & `greenery-4.2.1/greenery/charclass.py`

 * *Files identical despite different names*

### Comparing `greenery-4.2.0/greenery/charclass_test.py` & `greenery-4.2.1/greenery/charclass_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 
 def test_issubset() -> None:
     assert Charclass("a").issubset(Charclass("a"))
     assert not Charclass("a").issubset(Charclass("b"))
     assert Charclass("a").issubset(Charclass((("a", "b"),)))
     assert Charclass("a").issubset(~Charclass("b"))
     assert not (~Charclass("a")).issubset(Charclass("b"))
-    assert ~Charclass("a").issubset(DOT)
+    assert (~Charclass("a")).issubset(DOT)
 
 
 def test_charclass_str() -> None:
     assert str(WORDCHAR) == "\\w"
     assert str(DIGIT) == "\\d"
     assert str(SPACECHAR) == "\\s"
     assert str(Charclass("a")) == "a"
```

### Comparing `greenery-4.2.0/greenery/conc_test.py` & `greenery-4.2.1/greenery/conc_test.py`

 * *Files identical despite different names*

### Comparing `greenery-4.2.0/greenery/fsm.py` & `greenery-4.2.1/greenery/fsm.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,14 +65,15 @@
     alphabet: frozenset[AlphaType]
     states: frozenset[StateType]
     initial: StateType
     finals: frozenset[StateType]
     map: Mapping[StateType, Mapping[AlphaType, StateType]]
 
     # noinspection PyShadowingBuiltins
+    # pylint: disable=too-many-arguments
     def __init__(
         self,
         /,
         *,
         alphabet: Iterable[AlphaType],
         states: Iterable[StateType],
         initial: StateType,
```

### Comparing `greenery-4.2.0/greenery/fsm_test.py` & `greenery-4.2.1/greenery/fsm_test.py`

 * *Files identical despite different names*

### Comparing `greenery-4.2.0/greenery/mult_test.py` & `greenery-4.2.1/greenery/mult_test.py`

 * *Files identical despite different names*

### Comparing `greenery-4.2.0/greenery/multiplier.py` & `greenery-4.2.1/greenery/multiplier.py`

 * *Files identical despite different names*

### Comparing `greenery-4.2.0/greenery/multiplier_test.py` & `greenery-4.2.1/greenery/multiplier_test.py`

 * *Files identical despite different names*

### Comparing `greenery-4.2.0/greenery/parse.py` & `greenery-4.2.1/greenery/parse.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     NONWORDCHAR,
     SPACECHAR,
     WORDCHAR,
     Charclass,
     escapes,
     shorthand,
 )
-from .multiplier import Multiplier, symbolic
+from .multiplier import ONE, Multiplier, symbolic
 from .rxelems import Conc, Mult, Pattern
 
 # Currently many statements are grouped by `try/except NoMatch` in order to try
 # multiple matching functions in sequence. They can be refactored into smaller
 # functions to remove this suppression.
 # pylint: disable=too-many-try-statements
 
@@ -290,15 +290,18 @@
     except NoMatch:
         pass
 
     # "" empty string = infinite bound as in "{4,}"
     return INF, i
 
 
-def match_multiplier(string: str, i: int) -> MatchResult[Multiplier]:
+def match_nonempty_greedy_multiplier(string: str, i: int) -> MatchResult[Multiplier]:
+    """
+    Any multiplier which isn't the default empty string (equivalent to `{1,1}`)
+    """
     # {2,3} or {2,}
     try:
         j = static(string, i, "{")
         min_, j = match_bound(string, j)
         j = static(string, j, ",")
         max_, j = match_bound(string, j)
         j = static(string, j, "}")
@@ -311,26 +314,42 @@
         j = static(string, i, "{")
         min_, j = match_bound(string, j)
         j = static(string, j, "}")
         return Multiplier(min_, min_), j
     except NoMatch:
         pass
 
-    # "?"/"*"/"+"/""
-    # we do these in reverse order of symbol length, because
-    # that forces "" to be done last
-    for mult, symbol in sorted(symbolic.items(), key=lambda kv: -len(kv[1])):
+    # "?"/"*"/"+"
+    for mult, symbol in symbolic.items():
+        if not symbol:
+            continue
         try:
             return mult, static(string, i, symbol)
         except NoMatch:
             pass
 
     raise NoMatch
 
 
+def match_nonempty_multiplier(string: str, i: int) -> MatchResult[Multiplier]:
+    multiplier, j = match_nonempty_greedy_multiplier(string, i)
+    try:
+        j = static(string, j, "?")
+    except NoMatch:
+        pass
+    return multiplier, j
+
+
+def match_multiplier(string: str, i: int) -> MatchResult[Multiplier]:
+    try:
+        return match_nonempty_multiplier(string, i)
+    except NoMatch:
+        return ONE, i
+
+
 def match_mult(string: str, i: int) -> MatchResult[Mult]:
     multiplicand, j = match_multiplicand(string, i)
     multiplier, j = match_multiplier(string, j)
     return Mult(multiplicand, multiplier), j
 
 
 def match_conc(string: str, i: int) -> MatchResult[Conc]:
```

### Comparing `greenery-4.2.0/greenery/parse_test.py` & `greenery-4.2.1/greenery/parse_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,14 +93,30 @@
     )
     assert match_mult("abcde[^fg]*h{5}[a-z]+T{2,}", 21) == (
         Mult(Charclass("T"), Multiplier(Bound(2), INF)),
         26,
     )
 
 
+def test_lazy_multipliers() -> None:
+    assert match_mult("abcde[^fg]*?", 5) == (Mult(~Charclass("fg"), STAR), 12)
+    assert match_mult("abcde[^fg]*?h{5}?[a-z]+", 12) == (
+        Mult(Charclass("h"), Multiplier(Bound(5), Bound(5))),
+        17,
+    )
+    assert match_mult("abcde[^fg]*?h{5}?[a-z]+?T{1,}", 17) == (
+        Mult(Charclass("abcdefghijklmnopqrstuvwxyz"), PLUS),
+        24,
+    )
+    assert match_mult("abcde[^fg]*?h{5}?[a-z]+?T{2,}?", 24) == (
+        Mult(Charclass("T"), Multiplier(Bound(2), INF)),
+        30,
+    )
+
+
 def test_charclass_ranges() -> None:
     # Should accept arbitrary ranges of characters in charclasses. No longer
     # limited to alphanumerics. (User beware...)
     assert parse("[z{|}~]") == parse("[z-~]")
     assert parse("[\\w:;<=>?@\\[\\\\\\]\\^`]") == parse("[0-z]")
 
 
@@ -126,14 +142,18 @@
         Conc(Mult(Charclass("abcdefg012345678$%"), PLUS))
     )
     assert parse("[a-g0-8$%\\^]+") == Pattern(
         Conc(Mult(Charclass("abcdefg012345678$%^"), PLUS))
     )
 
 
+def test_lazy_mult_parsing() -> None:
+    assert parse("[a-g]+?") == Pattern(Conc(Mult(Charclass("abcdefg"), PLUS)))
+
+
 def test_conc_parsing() -> None:
     assert parse("abcde[^fg]*h{5}[a-z]+") == Pattern(
         Conc(
             Mult(Charclass("a"), ONE),
             Mult(Charclass("b"), ONE),
             Mult(Charclass("c"), ONE),
             Mult(Charclass("d"), ONE),
```

### Comparing `greenery-4.2.0/greenery/pattern_test.py` & `greenery-4.2.1/greenery/pattern_test.py`

 * *Files identical despite different names*

### Comparing `greenery-4.2.0/greenery/rxelems.py` & `greenery-4.2.1/greenery/rxelems.py`

 * *Files identical despite different names*

### Comparing `greenery-4.2.0/greenery/rxelems_test.py` & `greenery-4.2.1/greenery/rxelems_test.py`

 * *Files identical despite different names*

### Comparing `greenery-4.2.0/greenery.egg-info/SOURCES.txt` & `greenery-4.2.1/greenery.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `greenery-4.2.0/setup.py` & `greenery-4.2.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 from setuptools import setup
 
 setup(
     name="greenery",
-    version="4.2.0",
+    version="4.2.1",
     tests_require=["pytest"],
     packages=["greenery"],
     package_dir={"greenery": "greenery"},
     author="qntm",
     author_email="qntm <qntm@users.noreply.github.com>",
     description="Greenery allows manipulation of regular expressions",
     license="MIT License",
```

