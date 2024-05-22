# Comparing `tmp/screenpy_playwright-0.0.4.tar.gz` & `tmp/screenpy_playwright-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "screenpy_playwright-0.0.4.tar", max compression
+gzip compressed data, was "screenpy_playwright-0.0.5.tar", max compression
```

## Comparing `screenpy_playwright-0.0.4.tar` & `screenpy_playwright-0.0.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1071 2024-05-15 19:35:56.065664 screenpy_playwright-0.0.4/LICENSE
--rw-r--r--   0        0        0     3480 2024-05-15 19:35:56.069664 screenpy_playwright-0.0.4/README.md
--rw-r--r--   0        0        0     6199 2024-05-15 19:35:56.069664 screenpy_playwright-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      877 2024-05-15 19:35:56.069664 screenpy_playwright-0.0.4/screenpy_playwright/__init__.py
--rw-r--r--   0        0        0      938 2024-05-15 19:35:56.069664 screenpy_playwright-0.0.4/screenpy_playwright/__version__.py
--rw-r--r--   0        0        0      189 2024-05-15 19:35:56.069664 screenpy_playwright-0.0.4/screenpy_playwright/abilities/__init__.py
--rw-r--r--   0        0        0     2706 2024-05-15 19:35:56.069664 screenpy_playwright-0.0.4/screenpy_playwright/abilities/browse_the_web_synchronously.py
--rw-r--r--   0        0        0      898 2024-05-15 19:35:56.069664 screenpy_playwright-0.0.4/screenpy_playwright/actions/__init__.py
--rw-r--r--   0        0        0     2008 2024-05-15 19:35:56.069664 screenpy_playwright-0.0.4/screenpy_playwright/actions/click.py
--rw-r--r--   0        0        0     2914 2024-05-15 19:35:56.069664 screenpy_playwright-0.0.4/screenpy_playwright/actions/enter.py
--rw-r--r--   0        0        0     2123 2024-05-15 19:35:56.069664 screenpy_playwright-0.0.4/screenpy_playwright/actions/open.py
--rw-r--r--   0        0        0     1352 2024-05-15 19:35:56.069664 screenpy_playwright-0.0.4/screenpy_playwright/actions/refresh_the_page.py
--rw-r--r--   0        0        0     3205 2024-05-15 19:35:56.069664 screenpy_playwright-0.0.4/screenpy_playwright/actions/save_screenshot.py
--rw-r--r--   0        0        0     3250 2024-05-15 19:35:56.069664 screenpy_playwright-0.0.4/screenpy_playwright/actions/scroll.py
--rw-r--r--   0        0        0     3368 2024-05-15 19:35:56.069664 screenpy_playwright-0.0.4/screenpy_playwright/actions/select.py
--rw-r--r--   0        0        0      274 2024-05-15 19:35:56.069664 screenpy_playwright-0.0.4/screenpy_playwright/exceptions.py
--rw-r--r--   0        0        0      165 2024-05-15 19:35:56.069664 screenpy_playwright-0.0.4/screenpy_playwright/protocols.py
--rw-r--r--   0        0        0       39 2024-05-15 19:35:56.069664 screenpy_playwright-0.0.4/screenpy_playwright/py.typed
--rw-r--r--   0        0        0      554 2024-05-15 19:35:56.069664 screenpy_playwright-0.0.4/screenpy_playwright/questions/__init__.py
--rw-r--r--   0        0        0     1870 2024-05-15 19:35:56.069664 screenpy_playwright-0.0.4/screenpy_playwright/questions/attribute.py
--rw-r--r--   0        0        0     1369 2024-05-15 19:35:56.069664 screenpy_playwright-0.0.4/screenpy_playwright/questions/browser_url.py
--rw-r--r--   0        0        0      709 2024-05-15 19:35:56.069664 screenpy_playwright-0.0.4/screenpy_playwright/questions/element.py
--rw-r--r--   0        0        0     1259 2024-05-15 19:35:56.069664 screenpy_playwright-0.0.4/screenpy_playwright/questions/number.py
--rw-r--r--   0        0        0     1297 2024-05-15 19:35:56.069664 screenpy_playwright-0.0.4/screenpy_playwright/questions/text.py
--rw-r--r--   0        0        0      199 2024-05-15 19:35:56.069664 screenpy_playwright-0.0.4/screenpy_playwright/resolutions/__init__.py
--rw-r--r--   0        0        0      146 2024-05-15 19:35:56.069664 screenpy_playwright-0.0.4/screenpy_playwright/resolutions/custom_matchers/__init__.py
--rw-r--r--   0        0        0     1466 2024-05-15 19:35:56.069664 screenpy_playwright-0.0.4/screenpy_playwright/resolutions/custom_matchers/is_visible_element.py
--rw-r--r--   0        0        0      714 2024-05-15 19:35:56.069664 screenpy_playwright-0.0.4/screenpy_playwright/resolutions/is_visible.py
--rw-r--r--   0        0        0     6191 2024-05-15 19:35:56.073664 screenpy_playwright-0.0.4/screenpy_playwright/target.py
--rw-r--r--   0        0        0     5530 1970-01-01 00:00:00.000000 screenpy_playwright-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-05-22 21:30:10.051318 screenpy_playwright-0.0.5/LICENSE
+-rw-r--r--   0        0        0     3480 2024-05-22 21:30:10.051318 screenpy_playwright-0.0.5/README.md
+-rw-r--r--   0        0        0     6199 2024-05-22 21:30:10.051318 screenpy_playwright-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      877 2024-05-22 21:30:10.051318 screenpy_playwright-0.0.5/screenpy_playwright/__init__.py
+-rw-r--r--   0        0        0      938 2024-05-22 21:30:10.051318 screenpy_playwright-0.0.5/screenpy_playwright/__version__.py
+-rw-r--r--   0        0        0      189 2024-05-22 21:30:10.051318 screenpy_playwright-0.0.5/screenpy_playwright/abilities/__init__.py
+-rw-r--r--   0        0        0     2706 2024-05-22 21:30:10.051318 screenpy_playwright-0.0.5/screenpy_playwright/abilities/browse_the_web_synchronously.py
+-rw-r--r--   0        0        0      898 2024-05-22 21:30:10.051318 screenpy_playwright-0.0.5/screenpy_playwright/actions/__init__.py
+-rw-r--r--   0        0        0     2008 2024-05-22 21:30:10.051318 screenpy_playwright-0.0.5/screenpy_playwright/actions/click.py
+-rw-r--r--   0        0        0     3083 2024-05-22 21:30:10.051318 screenpy_playwright-0.0.5/screenpy_playwright/actions/enter.py
+-rw-r--r--   0        0        0     2123 2024-05-22 21:30:10.051318 screenpy_playwright-0.0.5/screenpy_playwright/actions/open.py
+-rw-r--r--   0        0        0     1352 2024-05-22 21:30:10.055317 screenpy_playwright-0.0.5/screenpy_playwright/actions/refresh_the_page.py
+-rw-r--r--   0        0        0     3205 2024-05-22 21:30:10.055317 screenpy_playwright-0.0.5/screenpy_playwright/actions/save_screenshot.py
+-rw-r--r--   0        0        0     3250 2024-05-22 21:30:10.055317 screenpy_playwright-0.0.5/screenpy_playwright/actions/scroll.py
+-rw-r--r--   0        0        0     3368 2024-05-22 21:30:10.055317 screenpy_playwright-0.0.5/screenpy_playwright/actions/select.py
+-rw-r--r--   0        0        0      274 2024-05-22 21:30:10.055317 screenpy_playwright-0.0.5/screenpy_playwright/exceptions.py
+-rw-r--r--   0        0        0      165 2024-05-22 21:30:10.055317 screenpy_playwright-0.0.5/screenpy_playwright/protocols.py
+-rw-r--r--   0        0        0       39 2024-05-22 21:30:10.055317 screenpy_playwright-0.0.5/screenpy_playwright/py.typed
+-rw-r--r--   0        0        0      554 2024-05-22 21:30:10.055317 screenpy_playwright-0.0.5/screenpy_playwright/questions/__init__.py
+-rw-r--r--   0        0        0     1870 2024-05-22 21:30:10.055317 screenpy_playwright-0.0.5/screenpy_playwright/questions/attribute.py
+-rw-r--r--   0        0        0     1369 2024-05-22 21:30:10.055317 screenpy_playwright-0.0.5/screenpy_playwright/questions/browser_url.py
+-rw-r--r--   0        0        0      709 2024-05-22 21:30:10.055317 screenpy_playwright-0.0.5/screenpy_playwright/questions/element.py
+-rw-r--r--   0        0        0     1259 2024-05-22 21:30:10.055317 screenpy_playwright-0.0.5/screenpy_playwright/questions/number.py
+-rw-r--r--   0        0        0     1297 2024-05-22 21:30:10.055317 screenpy_playwright-0.0.5/screenpy_playwright/questions/text.py
+-rw-r--r--   0        0        0      199 2024-05-22 21:30:10.055317 screenpy_playwright-0.0.5/screenpy_playwright/resolutions/__init__.py
+-rw-r--r--   0        0        0      146 2024-05-22 21:30:10.055317 screenpy_playwright-0.0.5/screenpy_playwright/resolutions/custom_matchers/__init__.py
+-rw-r--r--   0        0        0     1466 2024-05-22 21:30:10.055317 screenpy_playwright-0.0.5/screenpy_playwright/resolutions/custom_matchers/is_visible_element.py
+-rw-r--r--   0        0        0      714 2024-05-22 21:30:10.055317 screenpy_playwright-0.0.5/screenpy_playwright/resolutions/is_visible.py
+-rw-r--r--   0        0        0     7167 2024-05-22 21:30:10.055317 screenpy_playwright-0.0.5/screenpy_playwright/target.py
+-rw-r--r--   0        0        0     5530 1970-01-01 00:00:00.000000 screenpy_playwright-0.0.5/PKG-INFO
```

### Comparing `screenpy_playwright-0.0.4/LICENSE` & `screenpy_playwright-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `screenpy_playwright-0.0.4/README.md` & `screenpy_playwright-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `screenpy_playwright-0.0.4/pyproject.toml` & `screenpy_playwright-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -127,15 +127,15 @@
 
 ################################################################################
 #                 END OF BOILERPLATE ScreenPyHQ CONFIGURATIONS                 #
 ################################################################################
 
 [tool.poetry]
 name = "screenpy_playwright"
-version = "0.0.4"
+version = "0.0.5"
 description = "ScreenPy extension to enable interacting with Playwright."
 authors = ["Perry Goy <perry.goy@gmail.com>"]
 maintainers = ["Marcel Wilson"]
 license = "MIT"
 repository = "https://github.com/ScreenPyHQ/screenpy_playwright"
 documentation = "https://screenpy-playwright-docs.readthedocs.io"
 readme = "README.md"
```

### Comparing `screenpy_playwright-0.0.4/screenpy_playwright/__init__.py` & `screenpy_playwright-0.0.5/screenpy_playwright/__init__.py`

 * *Files identical despite different names*

### Comparing `screenpy_playwright-0.0.4/screenpy_playwright/__version__.py` & `screenpy_playwright-0.0.5/screenpy_playwright/__version__.py`

 * *Files identical despite different names*

### Comparing `screenpy_playwright-0.0.4/screenpy_playwright/abilities/browse_the_web_synchronously.py` & `screenpy_playwright-0.0.5/screenpy_playwright/abilities/browse_the_web_synchronously.py`

 * *Files identical despite different names*

### Comparing `screenpy_playwright-0.0.4/screenpy_playwright/actions/__init__.py` & `screenpy_playwright-0.0.5/screenpy_playwright/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `screenpy_playwright-0.0.4/screenpy_playwright/actions/click.py` & `screenpy_playwright-0.0.5/screenpy_playwright/actions/click.py`

 * *Files identical despite different names*

### Comparing `screenpy_playwright-0.0.4/screenpy_playwright/actions/enter.py` & `screenpy_playwright-0.0.5/screenpy_playwright/actions/enter.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,15 +52,18 @@
         The text will be masked, and appear as "[CENSORED]" in logs.
 
         Aliases:
             - ``the_password``
         """
         return cls(text, mask=True, **kwargs)
 
-    the_password = the_secret
+    @classmethod
+    def the_password(cls, text: str, **kwargs: Unpack[EnterTypes]) -> Self:
+        """Alias for ``the_secret``, recreated for mypy."""
+        return cls.the_secret(text, **kwargs)
 
     def into_the(self, target: Target, **kwargs: Unpack[EnterTypes]) -> Enter:
         """Target the element to enter text into.
 
         Aliases:
             - ``into``
         """
```

### Comparing `screenpy_playwright-0.0.4/screenpy_playwright/actions/open.py` & `screenpy_playwright-0.0.5/screenpy_playwright/actions/open.py`

 * *Files identical despite different names*

### Comparing `screenpy_playwright-0.0.4/screenpy_playwright/actions/refresh_the_page.py` & `screenpy_playwright-0.0.5/screenpy_playwright/actions/refresh_the_page.py`

 * *Files identical despite different names*

### Comparing `screenpy_playwright-0.0.4/screenpy_playwright/actions/save_screenshot.py` & `screenpy_playwright-0.0.5/screenpy_playwright/actions/save_screenshot.py`

 * *Files identical despite different names*

### Comparing `screenpy_playwright-0.0.4/screenpy_playwright/actions/scroll.py` & `screenpy_playwright-0.0.5/screenpy_playwright/actions/scroll.py`

 * *Files identical despite different names*

### Comparing `screenpy_playwright-0.0.4/screenpy_playwright/actions/select.py` & `screenpy_playwright-0.0.5/screenpy_playwright/actions/select.py`

 * *Files identical despite different names*

### Comparing `screenpy_playwright-0.0.4/screenpy_playwright/questions/__init__.py` & `screenpy_playwright-0.0.5/screenpy_playwright/questions/__init__.py`

 * *Files identical despite different names*

### Comparing `screenpy_playwright-0.0.4/screenpy_playwright/questions/attribute.py` & `screenpy_playwright-0.0.5/screenpy_playwright/questions/attribute.py`

 * *Files identical despite different names*

### Comparing `screenpy_playwright-0.0.4/screenpy_playwright/questions/browser_url.py` & `screenpy_playwright-0.0.5/screenpy_playwright/questions/browser_url.py`

 * *Files identical despite different names*

### Comparing `screenpy_playwright-0.0.4/screenpy_playwright/questions/element.py` & `screenpy_playwright-0.0.5/screenpy_playwright/questions/element.py`

 * *Files identical despite different names*

### Comparing `screenpy_playwright-0.0.4/screenpy_playwright/questions/number.py` & `screenpy_playwright-0.0.5/screenpy_playwright/questions/number.py`

 * *Files identical despite different names*

### Comparing `screenpy_playwright-0.0.4/screenpy_playwright/questions/text.py` & `screenpy_playwright-0.0.5/screenpy_playwright/questions/text.py`

 * *Files identical despite different names*

### Comparing `screenpy_playwright-0.0.4/screenpy_playwright/resolutions/custom_matchers/is_visible_element.py` & `screenpy_playwright-0.0.5/screenpy_playwright/resolutions/custom_matchers/is_visible_element.py`

 * *Files identical despite different names*

### Comparing `screenpy_playwright-0.0.4/screenpy_playwright/resolutions/is_visible.py` & `screenpy_playwright-0.0.5/screenpy_playwright/resolutions/is_visible.py`

 * *Files identical despite different names*

### Comparing `screenpy_playwright-0.0.4/screenpy_playwright/target.py` & `screenpy_playwright-0.0.5/screenpy_playwright/target.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,42 @@
 """Represent an element on the page using its locator and a description."""
 
 from __future__ import annotations
 
 from collections import UserString
 from dataclasses import dataclass
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Pattern, Tuple, TypedDict, Union
 
 from playwright.sync_api import Locator
 
 from .abilities import BrowseTheWebSynchronously
 from .exceptions import TargetingError
 
 if TYPE_CHECKING:
     from screenpy import Actor
-    from typing_extensions import Self
+    from typing_extensions import NotRequired, Self, Unpack
+
+    _ManipulationArgsType = Tuple[Union[str, int, None], ...]
+
+    class _ManipulationKwargsType(TypedDict):
+        """Types for kwargs that are passed to Playwright's locator methods."""
+
+        has_text: NotRequired[str | Pattern[str] | None]
+        has_not_text: NotRequired[str | Pattern[str] | None]
+        has: NotRequired[Locator | None]
+        has_not: NotRequired[Locator | None]
+        exact: NotRequired[bool | None]
+        checked: NotRequired[bool | None]
+        disabled: NotRequired[bool | None]
+        expanded: NotRequired[bool | None]
+        include_hidden: NotRequired[bool | None]
+        level: NotRequired[int | None]
+        name: NotRequired[str | Pattern[str] | None]
+        pressed: NotRequired[bool | None]
+        selected: NotRequired[bool | None]
 
 
 @dataclass
 class _Manipulation(UserString):
     """Represent one of the Playwright options for creating a locator.
 
     Could be a function or an attribute.
@@ -25,30 +44,34 @@
     This class allows the ScreenPy Playwright Target to behave just like a
     Playwright Locator, which has a robust, chainable API for describing
     elements.
     """
 
     target: Target
     name: str
-    args: tuple | None = None
-    kwargs: dict | None = None
+    args: _ManipulationArgsType | None = None
+    kwargs: _ManipulationKwargsType | None = None
 
     def __hash__(self) -> int:
         """Appear as the name, in case this is an attribute and not a method."""
         return hash(self.name)
 
     def __eq__(self, other: object) -> bool:
         """Appear as the name, in case this is an attribute and not a method."""
         return self.name == other
 
     def __getattr__(self, name: str) -> Target | _Manipulation:
         """Defer back to the Target for unknown attributes."""
         return getattr(self.target, name)
 
-    def __call__(self, *args: str, **kwargs: str) -> Target:
+    def __call__(
+        self,
+        *args: Unpack[_ManipulationArgsType],
+        **kwargs: Unpack[_ManipulationKwargsType],
+    ) -> Target:
         """Add args and kwargs to the manipulation."""
         self.args = args
         self.kwargs = kwargs
         return self.target
 
     def __repr__(self) -> str:
         """Reconstruct the locator function/attribute string."""
@@ -86,15 +109,15 @@
 
         # Using Target methods with Playwright strategies
         Target.the('"Pick up Milk" todo item').in_frame("#todoframe").get_by_text(
             "Pick up Milk"
         )
 
         # Using Playwright strategies directly
-        Target().frame_locator("#todoframe").get_by_label("todo")
+        Target("To-Do list").frame_locator("#todoframe").get_by_label("todo")
     """
 
     manipulations: list[_Manipulation]
     _description: str | None
 
     @classmethod
     def the(cls: type[Self], name: str) -> Self:
```

### Comparing `screenpy_playwright-0.0.4/PKG-INFO` & `screenpy_playwright-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: screenpy_playwright
-Version: 0.0.4
+Version: 0.0.5
 Summary: ScreenPy extension to enable interacting with Playwright.
 Home-page: https://github.com/ScreenPyHQ/screenpy_playwright
 License: MIT
 Author: Perry Goy
 Author-email: perry.goy@gmail.com
 Maintainer: Marcel Wilson
 Requires-Python: >=3.8,<4.0
```

