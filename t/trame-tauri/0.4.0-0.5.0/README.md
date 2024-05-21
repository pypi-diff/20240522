# Comparing `tmp/trame-tauri-0.4.0.tar.gz` & `tmp/trame-tauri-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trame-tauri-0.4.0.tar", last modified: Thu Apr  4 20:06:07 2024, max compression
+gzip compressed data, was "trame-tauri-0.5.0.tar", last modified: Tue May 21 21:59:23 2024, max compression
```

## Comparing `trame-tauri-0.4.0.tar` & `trame-tauri-0.5.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:06:07.032626 trame-tauri-0.4.0/
--rw-r--r--   0 root         (0) root         (0)      583 2024-04-04 20:05:43.000000 trame-tauri-0.4.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       31 2024-04-04 20:05:43.000000 trame-tauri-0.4.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2518 2024-04-04 20:06:07.032626 trame-tauri-0.4.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1736 2024-04-04 20:05:43.000000 trame-tauri-0.4.0/README.rst
--rw-r--r--   0 root         (0) root         (0)      925 2024-04-04 20:06:07.032626 trame-tauri-0.4.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-04 20:05:43.000000 trame-tauri-0.4.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:06:07.032626 trame-tauri-0.4.0/trame/
--rw-r--r--   0 root         (0) root         (0)       65 2024-04-04 20:05:43.000000 trame-tauri-0.4.0/trame/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:06:07.032626 trame-tauri-0.4.0/trame/modules/
--rw-r--r--   0 root         (0) root         (0)       65 2024-04-04 20:05:43.000000 trame-tauri-0.4.0/trame/modules/__init__.py
--rw-r--r--   0 root         (0) root         (0)       33 2024-04-04 20:05:43.000000 trame-tauri-0.4.0/trame/modules/tauri.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:06:07.032626 trame-tauri-0.4.0/trame/widgets/
--rw-r--r--   0 root         (0) root         (0)       65 2024-04-04 20:05:43.000000 trame-tauri-0.4.0/trame/widgets/__init__.py
--rw-r--r--   0 root         (0) root         (0)      135 2024-04-04 20:05:43.000000 trame-tauri-0.4.0/trame/widgets/tauri.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:06:07.032626 trame-tauri-0.4.0/trame_tauri/
--rw-r--r--   0 root         (0) root         (0)       93 2024-04-04 20:05:43.000000 trame-tauri-0.4.0/trame_tauri/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:06:07.032626 trame-tauri-0.4.0/trame_tauri/module/
--rw-r--r--   0 root         (0) root         (0)      199 2024-04-04 20:05:43.000000 trame-tauri-0.4.0/trame_tauri/module/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:06:07.032626 trame-tauri-0.4.0/trame_tauri/module/serve/
--rw-r--r--   0 root         (0) root         (0)    32933 2024-04-04 20:06:02.000000 trame-tauri-0.4.0/trame_tauri/module/serve/trame-tauri.umd.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:06:07.032626 trame-tauri-0.4.0/trame_tauri/widgets/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 20:05:43.000000 trame-tauri-0.4.0/trame_tauri/widgets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4411 2024-04-04 20:05:43.000000 trame-tauri-0.4.0/trame_tauri/widgets/tauri.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 20:06:07.032626 trame-tauri-0.4.0/trame_tauri.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2518 2024-04-04 20:06:07.000000 trame-tauri-0.4.0/trame_tauri.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      499 2024-04-04 20:06:07.000000 trame-tauri-0.4.0/trame_tauri.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 20:06:07.000000 trame-tauri-0.4.0/trame_tauri.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2024-04-04 20:06:07.000000 trame-tauri-0.4.0/trame_tauri.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2024-04-04 20:06:07.000000 trame-tauri-0.4.0/trame_tauri.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 21:59:23.612942 trame-tauri-0.5.0/
+-rw-r--r--   0 root         (0) root         (0)      583 2024-05-21 21:59:00.000000 trame-tauri-0.5.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       31 2024-05-21 21:59:00.000000 trame-tauri-0.5.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2518 2024-05-21 21:59:23.612942 trame-tauri-0.5.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1736 2024-05-21 21:59:00.000000 trame-tauri-0.5.0/README.rst
+-rw-r--r--   0 root         (0) root         (0)      925 2024-05-21 21:59:23.612942 trame-tauri-0.5.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-21 21:59:00.000000 trame-tauri-0.5.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 21:59:23.612942 trame-tauri-0.5.0/trame/
+-rw-r--r--   0 root         (0) root         (0)       65 2024-05-21 21:59:00.000000 trame-tauri-0.5.0/trame/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 21:59:23.612942 trame-tauri-0.5.0/trame/modules/
+-rw-r--r--   0 root         (0) root         (0)       65 2024-05-21 21:59:00.000000 trame-tauri-0.5.0/trame/modules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       33 2024-05-21 21:59:00.000000 trame-tauri-0.5.0/trame/modules/tauri.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 21:59:23.612942 trame-tauri-0.5.0/trame/widgets/
+-rw-r--r--   0 root         (0) root         (0)       65 2024-05-21 21:59:00.000000 trame-tauri-0.5.0/trame/widgets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      135 2024-05-21 21:59:00.000000 trame-tauri-0.5.0/trame/widgets/tauri.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 21:59:23.612942 trame-tauri-0.5.0/trame_tauri/
+-rw-r--r--   0 root         (0) root         (0)       93 2024-05-21 21:59:00.000000 trame-tauri-0.5.0/trame_tauri/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 21:59:23.612942 trame-tauri-0.5.0/trame_tauri/module/
+-rw-r--r--   0 root         (0) root         (0)      199 2024-05-21 21:59:00.000000 trame-tauri-0.5.0/trame_tauri/module/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 21:59:23.612942 trame-tauri-0.5.0/trame_tauri/module/serve/
+-rw-r--r--   0 root         (0) root         (0)    36142 2024-05-21 21:59:20.000000 trame-tauri-0.5.0/trame_tauri/module/serve/trame-tauri.umd.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 21:59:23.612942 trame-tauri-0.5.0/trame_tauri/widgets/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-21 21:59:00.000000 trame-tauri-0.5.0/trame_tauri/widgets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7776 2024-05-21 21:59:00.000000 trame-tauri-0.5.0/trame_tauri/widgets/tauri.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 21:59:23.612942 trame-tauri-0.5.0/trame_tauri.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2518 2024-05-21 21:59:23.000000 trame-tauri-0.5.0/trame_tauri.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      499 2024-05-21 21:59:23.000000 trame-tauri-0.5.0/trame_tauri.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-21 21:59:23.000000 trame-tauri-0.5.0/trame_tauri.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-05-21 21:59:23.000000 trame-tauri-0.5.0/trame_tauri.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2024-05-21 21:59:23.000000 trame-tauri-0.5.0/trame_tauri.egg-info/top_level.txt
```

### Comparing `trame-tauri-0.4.0/LICENSE` & `trame-tauri-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trame-tauri-0.4.0/PKG-INFO` & `trame-tauri-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trame-tauri
-Version: 0.4.0
+Version: 0.5.0
 Summary: Helper widget to provide simpler integration with Tauri
 Author: Kitware Inc.
 License: Apache Software License
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `trame-tauri-0.4.0/README.rst` & `trame-tauri-0.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `trame-tauri-0.4.0/setup.cfg` & `trame-tauri-0.5.0/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = trame-tauri
-version = 0.4.0
+version = 0.5.0
 description = Helper widget to provide simpler integration with Tauri
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 author = Kitware Inc.
 license = Apache Software License
 classifiers = 
 	Development Status :: 4 - Beta
```

### Comparing `trame-tauri-0.4.0/trame_tauri/module/serve/trame-tauri.umd.js` & `trame-tauri-0.5.0/trame_tauri/module/serve/trame-tauri.umd.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -1,119 +1,118 @@
-(function(m, _) {
-    typeof exports == "object" && typeof module < "u" ? _(exports) : typeof define == "function" && define.amd ? define(["exports"], _) : (m = typeof globalThis < "u" ? globalThis : m || self, _(m.trame_tauri = {}))
-})(this, function(m) {
+(function(g, y) {
+    typeof exports == "object" && typeof module < "u" ? y(exports, require("vue")) : typeof define == "function" && define.amd ? define(["exports", "vue"], y) : (g = typeof globalThis < "u" ? globalThis : g || self, y(g.trame_tauri = {}, g.Vue))
+})(this, function(g, y) {
     "use strict";
 
-    function _() {
+    function pe() {
         return window.crypto.getRandomValues(new Uint32Array(1))[0]
     }
 
-    function c(t, e = !1) {
-        const a = _(),
+    function b(t, e = !1) {
+        const a = pe(),
             i = `_${a}`;
         return Object.defineProperty(window, i, {
             value: r => (e && Reflect.deleteProperty(window, i), t == null ? void 0 : t(r)),
             writable: !1,
             configurable: !0
         }), a
     }
-    async function E(t, e = {}) {
+    async function U(t, e = {}) {
         return new Promise((a, i) => {
-            const r = c(l => {
-                    a(l), Reflect.deleteProperty(window, `_${s}`)
+            const r = b(u => {
+                    a(u), Reflect.deleteProperty(window, `_${s}`)
                 }, !0),
-                s = c(l => {
-                    i(l), Reflect.deleteProperty(window, `_${r}`)
+                s = b(u => {
+                    i(u), Reflect.deleteProperty(window, `_${r}`)
                 }, !0);
             window.__TAURI_IPC__({
                 cmd: t,
                 callback: r,
                 error: s,
                 ...e
             })
         })
     }
 
-    function ae(t, e = "asset") {
+    function ge(t, e = "asset") {
         return window.__TAURI__.convertFileSrc(t, e)
     }
-    const ne = Object.freeze(Object.defineProperty({
+    const be = Object.freeze(Object.defineProperty({
         __proto__: null,
-        convertFileSrc: ae,
-        invoke: E,
-        transformCallback: c
+        convertFileSrc: ge,
+        invoke: U,
+        transformCallback: b
     }, Symbol.toStringTag, {
         value: "Module"
     }));
     async function n(t) {
-        return E("tauri", t)
+        return U("tauri", t)
     }
-    async function v(t, e) {
+    async function $(t, e) {
         return n({
             __tauriModule: "Event",
             message: {
                 cmd: "unlisten",
                 event: t,
                 eventId: e
             }
         })
     }
-    async function F(t, e, a) {
+    async function k(t, e, a) {
         await n({
             __tauriModule: "Event",
             message: {
                 cmd: "emit",
                 event: t,
                 windowLabel: e,
                 payload: a
             }
         })
     }
-    async function w(t, e, a) {
+    async function L(t, e, a) {
         return n({
             __tauriModule: "Event",
             message: {
                 cmd: "listen",
                 event: t,
                 windowLabel: e,
-                handler: c(a)
+                handler: b(a)
             }
-        }).then(i => async () => v(t, i))
+        }).then(i => async () => $(t, i))
     }
-    async function j(t, e, a) {
-        return w(t, e, i => {
-            a(i), v(t, i.id).catch(() => {})
+    async function H(t, e, a) {
+        return L(t, e, i => {
+            a(i), $(t, i.id).catch(() => {})
         })
     }
-    var u;
+    var d;
     (function(t) {
         t.WINDOW_RESIZED = "tauri://resize", t.WINDOW_MOVED = "tauri://move", t.WINDOW_CLOSE_REQUESTED = "tauri://close-requested", t.WINDOW_CREATED = "tauri://window-created", t.WINDOW_DESTROYED = "tauri://destroyed", t.WINDOW_FOCUS = "tauri://focus", t.WINDOW_BLUR = "tauri://blur", t.WINDOW_SCALE_FACTOR_CHANGED = "tauri://scale-change", t.WINDOW_THEME_CHANGED = "tauri://theme-changed", t.WINDOW_FILE_DROP = "tauri://file-drop", t.WINDOW_FILE_DROP_HOVER = "tauri://file-drop-hover", t.WINDOW_FILE_DROP_CANCELLED = "tauri://file-drop-cancelled", t.MENU = "tauri://menu", t.CHECK_UPDATE = "tauri://update", t.UPDATE_AVAILABLE = "tauri://update-available", t.INSTALL_UPDATE = "tauri://update-install", t.STATUS_UPDATE = "tauri://update-status", t.DOWNLOAD_PROGRESS = "tauri://update-download-progress"
-    })(u || (u = {}));
-    async function M(t, e) {
-        return w(t, null, e)
+    })(d || (d = {}));
+    async function D(t, e) {
+        return L(t, null, e)
     }
-    async function P(t, e) {
-        return j(t, null, e)
+    async function T(t, e) {
+        return H(t, null, e)
     }
-    async function A(t, e) {
-        return F(t, void 0, e)
+    async function C(t, e) {
+        return k(t, void 0, e)
     }
-    const ie = Object.freeze(Object.defineProperty({
+    const we = Object.freeze(Object.defineProperty({
             __proto__: null,
             get TauriEvent() {
-                return u
+                return d
             },
-            emit: A,
-            listen: M,
-            once: P
+            emit: C,
+            listen: D,
+            once: T
         }, Symbol.toStringTag, {
             value: "Module"
         })),
-        re = {
-            name: "TauriEvent",
+        Me = {
             props: {
                 listen: {
                     type: Array,
                     default: () => []
                 },
                 once: {
                     type: Array,
@@ -122,50 +121,50 @@
             },
             async mounted() {
                 this.unsubscribes = [];
                 for (let t = 0; t < this.listen.length; t++) {
                     const e = this.listen[t],
                         a = `tauri://${e.replaceAll("_","-")}`,
                         i = e.replaceAll("-", "_");
-                    this.unsubscribes.push(await M(a, r => {
+                    this.unsubscribes.push(await D(a, r => {
                         this.$emit(i, r.payload)
                     }))
                 }
                 for (let t = 0; t < this.once.length; t++) {
                     const e = this.once[t],
                         a = `tauri://${e.replaceAll("_","-")}`,
                         i = e.replaceAll("-", "_");
-                    this.unsubscribes.push(await P(a, r => {
+                    this.unsubscribes.push(await T(a, r => {
                         this.$emit(i, r.payload)
                     }))
                 }
             },
             beforeUnmount() {
                 for (; this.unsubscribes.length;) this.unsubscribes.pop()()
             }
         };
-    async function z(t = {}) {
+    async function V(t = {}) {
         return typeof t == "object" && Object.freeze(t), n({
             __tauriModule: "Dialog",
             message: {
                 cmd: "openDialog",
                 options: t
             }
         })
     }
-    async function x(t = {}) {
+    async function q(t = {}) {
         return typeof t == "object" && Object.freeze(t), n({
             __tauriModule: "Dialog",
             message: {
                 cmd: "saveDialog",
                 options: t
             }
         })
     }
-    async function I(t, e) {
+    async function G(t, e) {
         var i, r;
         const a = typeof e == "string" ? {
             title: e
         } : e;
         return n({
             __tauriModule: "Dialog",
             message: {
@@ -173,15 +172,15 @@
                 message: t.toString(),
                 title: (i = a == null ? void 0 : a.title) == null ? void 0 : i.toString(),
                 type: a == null ? void 0 : a.type,
                 buttonLabel: (r = a == null ? void 0 : a.okLabel) == null ? void 0 : r.toString()
             }
         })
     }
-    async function N(t, e) {
+    async function J(t, e) {
         var i, r, s;
         const a = typeof e == "string" ? {
             title: e
         } : e;
         return n({
             __tauriModule: "Dialog",
             message: {
@@ -189,15 +188,15 @@
                 message: t.toString(),
                 title: (i = a == null ? void 0 : a.title) == null ? void 0 : i.toString(),
                 type: a == null ? void 0 : a.type,
                 buttonLabels: [((r = a == null ? void 0 : a.okLabel) == null ? void 0 : r.toString()) ?? "Yes", ((s = a == null ? void 0 : a.cancelLabel) == null ? void 0 : s.toString()) ?? "No"]
             }
         })
     }
-    async function R(t, e) {
+    async function K(t, e) {
         var i, r, s;
         const a = typeof e == "string" ? {
             title: e
         } : e;
         return n({
             __tauriModule: "Dialog",
             message: {
@@ -205,1287 +204,115 @@
                 message: t.toString(),
                 title: (i = a == null ? void 0 : a.title) == null ? void 0 : i.toString(),
                 type: a == null ? void 0 : a.type,
                 buttonLabels: [((r = a == null ? void 0 : a.okLabel) == null ? void 0 : r.toString()) ?? "Ok", ((s = a == null ? void 0 : a.cancelLabel) == null ? void 0 : s.toString()) ?? "Cancel"]
             }
         })
     }
-    const se = Object.freeze(Object.defineProperty({
+    const Pe = Object.freeze(Object.defineProperty({
             __proto__: null,
-            ask: N,
-            confirm: R,
-            message: I,
-            open: z,
-            save: x
+            ask: J,
+            confirm: K,
+            message: G,
+            open: V,
+            save: q
         }, Symbol.toStringTag, {
             value: "Module"
         })),
-        $ = {
-            TauriEvents: re,
-            TauriDialog: {
-                emits: ["open", "save", "message", "confirm", "ask"],
-                setup(t, {
-                    emit: e,
-                    expose: a
-                }) {
-                    a({
-                        open: async i => e("open", await z(i)),
-                        save: async i => e("save", await x(i)),
-                        message: async i => e("message", await I(i)),
-                        confirm: async i => e("confirm", await R(i)),
-                        ask: async i => e("ask", await N(i))
-                    })
-                }
-            }
-        };
-    async function oe() {
-        return n({
-            __tauriModule: "App",
-            message: {
-                cmd: "getAppVersion"
-            }
-        })
-    }
-    async function le() {
-        return n({
-            __tauriModule: "App",
-            message: {
-                cmd: "getAppName"
-            }
-        })
-    }
-    async function ue() {
-        return n({
-            __tauriModule: "App",
-            message: {
-                cmd: "getTauriVersion"
-            }
-        })
-    }
-    async function ce() {
-        return n({
-            __tauriModule: "App",
-            message: {
-                cmd: "show"
-            }
-        })
-    }
-    async function de() {
-        return n({
-            __tauriModule: "App",
-            message: {
-                cmd: "hide"
-            }
-        })
-    }
-    const me = {
-        ...Object.freeze(Object.defineProperty({
-            __proto__: null,
-            getName: le,
-            getTauriVersion: ue,
-            getVersion: oe,
-            hide: de,
-            show: ce
-        }, Symbol.toStringTag, {
-            value: "Module"
-        }))
-    };
-    async function he() {
-        return n({
-            __tauriModule: "Cli",
-            message: {
-                cmd: "cliMatches"
-            }
-        })
-    }
-    const _e = {
-        ...Object.freeze(Object.defineProperty({
-            __proto__: null,
-            getMatches: he
-        }, Symbol.toStringTag, {
-            value: "Module"
-        }))
-    };
-    async function ye(t) {
-        return n({
-            __tauriModule: "Clipboard",
-            message: {
-                cmd: "writeText",
-                data: t
-            }
-        })
-    }
-    async function pe() {
-        return n({
-            __tauriModule: "Clipboard",
-            message: {
-                cmd: "readText",
-                data: null
-            }
-        })
-    }
-    const ge = {
-            ...Object.freeze(Object.defineProperty({
-                __proto__: null,
-                readText: pe,
-                writeText: ye
-            }, Symbol.toStringTag, {
-                value: "Module"
-            }))
-        },
-        fe = {
-            ...se
-        },
-        be = {
-            ...ie
-        };
-    var o;
-    (function(t) {
-        t[t.Audio = 1] = "Audio", t[t.Cache = 2] = "Cache", t[t.Config = 3] = "Config", t[t.Data = 4] = "Data", t[t.LocalData = 5] = "LocalData", t[t.Desktop = 6] = "Desktop", t[t.Document = 7] = "Document", t[t.Download = 8] = "Download", t[t.Executable = 9] = "Executable", t[t.Font = 10] = "Font", t[t.Home = 11] = "Home", t[t.Picture = 12] = "Picture", t[t.Public = 13] = "Public", t[t.Runtime = 14] = "Runtime", t[t.Template = 15] = "Template", t[t.Video = 16] = "Video", t[t.Resource = 17] = "Resource", t[t.App = 18] = "App", t[t.Log = 19] = "Log", t[t.Temp = 20] = "Temp", t[t.AppConfig = 21] = "AppConfig", t[t.AppData = 22] = "AppData", t[t.AppLocalData = 23] = "AppLocalData", t[t.AppCache = 24] = "AppCache", t[t.AppLog = 25] = "AppLog"
-    })(o || (o = {}));
-    async function we(t, e = {}) {
-        return n({
-            __tauriModule: "Fs",
-            message: {
-                cmd: "readTextFile",
-                path: t,
-                options: e
-            }
-        })
-    }
-    async function Me(t, e = {}) {
-        const a = await n({
-            __tauriModule: "Fs",
-            message: {
-                cmd: "readFile",
-                path: t,
-                options: e
-            }
-        });
-        return Uint8Array.from(a)
-    }
-    async function U(t, e, a) {
-        typeof a == "object" && Object.freeze(a), typeof t == "object" && Object.freeze(t);
-        const i = {
-            path: "",
-            contents: ""
-        };
-        let r = a;
-        return typeof t == "string" ? i.path = t : (i.path = t.path, i.contents = t.contents), typeof e == "string" ? i.contents = e ?? "" : r = e, n({
-            __tauriModule: "Fs",
-            message: {
-                cmd: "writeFile",
-                path: i.path,
-                contents: Array.from(new TextEncoder().encode(i.contents)),
-                options: r
-            }
-        })
-    }
-    async function Pe(t, e, a) {
-        typeof a == "object" && Object.freeze(a), typeof t == "object" && Object.freeze(t);
-        const i = {
-            path: "",
-            contents: []
-        };
-        let r = a;
-        return typeof t == "string" ? i.path = t : (i.path = t.path, i.contents = t.contents), e && "dir" in e ? r = e : typeof t == "string" && (i.contents = e ?? []), n({
-            __tauriModule: "Fs",
-            message: {
-                cmd: "writeFile",
-                path: i.path,
-                contents: Array.from(i.contents instanceof ArrayBuffer ? new Uint8Array(i.contents) : i.contents),
-                options: r
-            }
-        })
-    }
-    async function Ae(t, e = {}) {
-        return n({
-            __tauriModule: "Fs",
-            message: {
-                cmd: "readDir",
-                path: t,
-                options: e
-            }
-        })
-    }
-    async function Oe(t, e = {}) {
-        return n({
-            __tauriModule: "Fs",
-            message: {
-                cmd: "createDir",
-                path: t,
-                options: e
-            }
-        })
-    }
-    async function We(t, e = {}) {
-        return n({
-            __tauriModule: "Fs",
-            message: {
-                cmd: "removeDir",
-                path: t,
-                options: e
-            }
-        })
-    }
-    async function Se(t, e, a = {}) {
-        return n({
-            __tauriModule: "Fs",
-            message: {
-                cmd: "copyFile",
-                source: t,
-                destination: e,
-                options: a
-            }
-        })
-    }
-    async function De(t, e = {}) {
-        return n({
-            __tauriModule: "Fs",
-            message: {
-                cmd: "removeFile",
-                path: t,
-                options: e
-            }
-        })
-    }
-    async function Le(t, e, a = {}) {
-        return n({
-            __tauriModule: "Fs",
-            message: {
-                cmd: "renameFile",
-                oldPath: t,
-                newPath: e,
-                options: a
-            }
-        })
-    }
-    async function Te(t, e = {}) {
-        return n({
-            __tauriModule: "Fs",
-            message: {
-                cmd: "exists",
-                path: t,
-                options: e
-            }
-        })
-    }
-    const Ce = {
-        ...Object.freeze(Object.defineProperty({
-            __proto__: null,
-            get BaseDirectory() {
-                return o
-            },
-            get Dir() {
-                return o
-            },
-            copyFile: Se,
-            createDir: Oe,
-            exists: Te,
-            readBinaryFile: Me,
-            readDir: Ae,
-            readTextFile: we,
-            removeDir: We,
-            removeFile: De,
-            renameFile: Le,
-            writeBinaryFile: Pe,
-            writeFile: U,
-            writeTextFile: U
-        }, Symbol.toStringTag, {
-            value: "Module"
-        }))
-    };
-    async function Ee(t, e) {
-        return n({
-            __tauriModule: "GlobalShortcut",
-            message: {
-                cmd: "register",
-                shortcut: t,
-                handler: c(e)
-            }
-        })
-    }
-    async function ve(t, e) {
-        return n({
-            __tauriModule: "GlobalShortcut",
-            message: {
-                cmd: "registerAll",
-                shortcuts: t,
-                handler: c(e)
-            }
-        })
-    }
-    async function Fe(t) {
-        return n({
-            __tauriModule: "GlobalShortcut",
-            message: {
-                cmd: "isRegistered",
-                shortcut: t
-            }
-        })
-    }
-    async function je(t) {
-        return n({
-            __tauriModule: "GlobalShortcut",
-            message: {
-                cmd: "unregister",
-                shortcut: t
-            }
-        })
-    }
-    async function ze() {
-        return n({
-            __tauriModule: "GlobalShortcut",
-            message: {
-                cmd: "unregisterAll"
-            }
-        })
-    }
-    const xe = {
-        ...Object.freeze(Object.defineProperty({
-            __proto__: null,
-            isRegistered: Fe,
-            register: Ee,
-            registerAll: ve,
-            unregister: je,
-            unregisterAll: ze
-        }, Symbol.toStringTag, {
-            value: "Module"
-        }))
-    };
-    var y;
-    (function(t) {
-        t[t.JSON = 1] = "JSON", t[t.Text = 2] = "Text", t[t.Binary = 3] = "Binary"
-    })(y || (y = {}));
-    async function Ie(t) {
-        const e = {},
-            a = async (i, r) => {
-                if (r !== null) {
-                    let s;
-                    typeof r == "string" ? s = r : r instanceof Uint8Array || Array.isArray(r) ? s = Array.from(r) : r instanceof File ? s = {
-                        file: Array.from(new Uint8Array(await r.arrayBuffer())),
-                        mime: r.type,
-                        fileName: r.name
-                    } : typeof r.file == "string" ? s = {
-                        file: r.file,
-                        mime: r.mime,
-                        fileName: r.fileName
-                    } : s = {
-                        file: Array.from(r.file),
-                        mime: r.mime,
-                        fileName: r.fileName
-                    }, e[String(i)] = s
-                }
-            };
-        if (t instanceof FormData)
-            for (const [i, r] of t) await a(i, r);
-        else
-            for (const [i, r] of Object.entries(t)) await a(i, r);
-        return e
-    }
-    class h {
-        constructor(e, a) {
-            this.type = e, this.payload = a
-        }
-        static form(e) {
-            return new h("Form", e)
-        }
-        static json(e) {
-            return new h("Json", e)
-        }
-        static text(e) {
-            return new h("Text", e)
-        }
-        static bytes(e) {
-            return new h("Bytes", Array.from(e instanceof ArrayBuffer ? new Uint8Array(e) : e))
-        }
-    }
-    class k {
-        constructor(e) {
-            this.url = e.url, this.status = e.status, this.ok = this.status >= 200 && this.status < 300, this.headers = e.headers, this.rawHeaders = e.rawHeaders, this.data = e.data
-        }
-    }
-    class H {
-        constructor(e) {
-            this.id = e
-        }
-        async drop() {
-            return n({
-                __tauriModule: "Http",
-                message: {
-                    cmd: "dropClient",
-                    client: this.id
-                }
-            })
-        }
-        async request(e) {
-            var i;
-            const a = !e.responseType || e.responseType === y.JSON;
-            return a && (e.responseType = y.Text), ((i = e.body) == null ? void 0 : i.type) === "Form" && (e.body.payload = await Ie(e.body.payload)), n({
-                __tauriModule: "Http",
-                message: {
-                    cmd: "httpRequest",
-                    client: this.id,
-                    options: e
-                }
-            }).then(r => {
-                const s = new k(r);
-                if (a) {
-                    try {
-                        s.data = JSON.parse(s.data)
-                    } catch (l) {
-                        if (s.ok && s.data === "") s.data = {};
-                        else if (s.ok) throw Error(`Failed to parse response \`${s.data}\` as JSON: ${l};
-              try setting the \`responseType\` option to \`ResponseType.Text\` or \`ResponseType.Binary\` if the API does not return a JSON response.`)
-                    }
-                    return s
-                }
-                return s
-            })
-        }
-        async get(e, a) {
-            return this.request({
-                method: "GET",
-                url: e,
-                ...a
-            })
-        }
-        async post(e, a, i) {
-            return this.request({
-                method: "POST",
-                url: e,
-                body: a,
-                ...i
-            })
-        }
-        async put(e, a, i) {
-            return this.request({
-                method: "PUT",
-                url: e,
-                body: a,
-                ...i
-            })
-        }
-        async patch(e, a) {
-            return this.request({
-                method: "PATCH",
-                url: e,
-                ...a
-            })
-        }
-        async delete(e, a) {
-            return this.request({
-                method: "DELETE",
-                url: e,
-                ...a
-            })
-        }
-    }
-    async function V(t) {
-        return n({
-            __tauriModule: "Http",
-            message: {
-                cmd: "createClient",
-                options: t
-            }
-        }).then(e => new H(e))
-    }
-    let O = null;
-    async function Ne(t, e) {
-        return O === null && (O = await V()), O.request({
-            url: t,
-            method: (e == null ? void 0 : e.method) ?? "GET",
-            ...e
-        })
-    }
-    const Re = {
-        ...Object.freeze(Object.defineProperty({
-            __proto__: null,
-            Body: h,
-            Client: H,
-            Response: k,
-            get ResponseType() {
-                return y
-            },
-            fetch: Ne,
-            getClient: V
-        }, Symbol.toStringTag, {
-            value: "Module"
-        }))
-    };
-    async function $e() {
-        return window.Notification.permission !== "default" ? Promise.resolve(window.Notification.permission === "granted") : n({
-            __tauriModule: "Notification",
-            message: {
-                cmd: "isNotificationPermissionGranted"
-            }
-        })
-    }
-    async function Ue() {
-        return window.Notification.requestPermission()
-    }
-
-    function ke(t) {
-        typeof t == "string" ? new window.Notification(t) : new window.Notification(t.title, t)
-    }
-    const He = {
-        ...Object.freeze(Object.defineProperty({
-            __proto__: null,
-            isPermissionGranted: $e,
-            requestPermission: Ue,
-            sendNotification: ke
-        }, Symbol.toStringTag, {
-            value: "Module"
-        }))
-    };
-
-    function W() {
-        return navigator.appVersion.includes("Win")
-    }
-    const Ve = W() ? `\r
-` : `
-`;
-    async function Ge() {
-        return n({
-            __tauriModule: "Os",
-            message: {
-                cmd: "platform"
-            }
-        })
-    }
-    async function qe() {
-        return n({
-            __tauriModule: "Os",
-            message: {
-                cmd: "version"
-            }
-        })
-    }
-    async function Je() {
-        return n({
-            __tauriModule: "Os",
-            message: {
-                cmd: "osType"
-            }
-        })
-    }
-    async function Ke() {
-        return n({
-            __tauriModule: "Os",
-            message: {
-                cmd: "arch"
-            }
-        })
-    }
-    async function Qe() {
-        return n({
-            __tauriModule: "Os",
-            message: {
-                cmd: "tempdir"
-            }
-        })
-    }
-    async function Ye() {
-        return n({
-            __tauriModule: "Os",
-            message: {
-                cmd: "locale"
-            }
-        })
-    }
-    const Ze = {
-        ...Object.freeze(Object.defineProperty({
-            __proto__: null,
-            EOL: Ve,
-            arch: Ke,
-            locale: Ye,
-            platform: Ge,
-            tempdir: Qe,
-            type: Je,
-            version: qe
-        }, Symbol.toStringTag, {
-            value: "Module"
-        }))
-    };
-    async function Xe() {
-        return G()
-    }
-    async function G() {
-        return n({
-            __tauriModule: "Path",
-            message: {
-                cmd: "resolvePath",
-                path: "",
-                directory: o.AppConfig
-            }
-        })
-    }
-    async function Be() {
-        return n({
-            __tauriModule: "Path",
-            message: {
-                cmd: "resolvePath",
-                path: "",
-                directory: o.AppData
-            }
-        })
-    }
-    async function et() {
-        return n({
-            __tauriModule: "Path",
-            message: {
-                cmd: "resolvePath",
-                path: "",
-                directory: o.AppLocalData
-            }
-        })
-    }
-    async function tt() {
-        return n({
-            __tauriModule: "Path",
-            message: {
-                cmd: "resolvePath",
-                path: "",
-                directory: o.AppCache
-            }
-        })
-    }
-    async function at() {
-        return n({
-            __tauriModule: "Path",
-            message: {
-                cmd: "resolvePath",
-                path: "",
-                directory: o.Audio
-            }
-        })
-    }
-    async function nt() {
-        return n({
-            __tauriModule: "Path",
-            message: {
-                cmd: "resolvePath",
-                path: "",
-                directory: o.Cache
-            }
-        })
-    }
-    async function it() {
-        return n({
-            __tauriModule: "Path",
-            message: {
-                cmd: "resolvePath",
-                path: "",
-                directory: o.Config
-            }
-        })
-    }
-    async function rt() {
-        return n({
-            __tauriModule: "Path",
-            message: {
-                cmd: "resolvePath",
-                path: "",
-                directory: o.Data
-            }
-        })
-    }
-    async function st() {
-        return n({
-            __tauriModule: "Path",
-            message: {
-                cmd: "resolvePath",
-                path: "",
-                directory: o.Desktop
-            }
-        })
-    }
-    async function ot() {
-        return n({
-            __tauriModule: "Path",
-            message: {
-                cmd: "resolvePath",
-                path: "",
-                directory: o.Document
-            }
-        })
-    }
-    async function lt() {
-        return n({
-            __tauriModule: "Path",
-            message: {
-                cmd: "resolvePath",
-                path: "",
-                directory: o.Download
-            }
-        })
-    }
-    async function ut() {
-        return n({
-            __tauriModule: "Path",
-            message: {
-                cmd: "resolvePath",
-                path: "",
-                directory: o.Executable
-            }
-        })
-    }
-    async function ct() {
-        return n({
-            __tauriModule: "Path",
-            message: {
-                cmd: "resolvePath",
-                path: "",
-                directory: o.Font
-            }
-        })
-    }
-    async function dt() {
-        return n({
-            __tauriModule: "Path",
-            message: {
-                cmd: "resolvePath",
-                path: "",
-                directory: o.Home
-            }
-        })
-    }
-    async function mt() {
-        return n({
-            __tauriModule: "Path",
-            message: {
-                cmd: "resolvePath",
-                path: "",
-                directory: o.LocalData
-            }
-        })
-    }
-    async function ht() {
-        return n({
-            __tauriModule: "Path",
-            message: {
-                cmd: "resolvePath",
-                path: "",
-                directory: o.Picture
-            }
-        })
-    }
-    async function _t() {
-        return n({
-            __tauriModule: "Path",
-            message: {
-                cmd: "resolvePath",
-                path: "",
-                directory: o.Public
-            }
-        })
-    }
-    async function yt() {
-        return n({
-            __tauriModule: "Path",
-            message: {
-                cmd: "resolvePath",
-                path: "",
-                directory: o.Resource
-            }
-        })
-    }
-    async function pt(t) {
-        return n({
-            __tauriModule: "Path",
-            message: {
-                cmd: "resolvePath",
-                path: t,
-                directory: o.Resource
-            }
-        })
-    }
-    async function gt() {
-        return n({
-            __tauriModule: "Path",
-            message: {
-                cmd: "resolvePath",
-                path: "",
-                directory: o.Runtime
-            }
-        })
-    }
-    async function ft() {
-        return n({
-            __tauriModule: "Path",
-            message: {
-                cmd: "resolvePath",
-                path: "",
-                directory: o.Template
-            }
-        })
-    }
-    async function bt() {
-        return n({
-            __tauriModule: "Path",
-            message: {
-                cmd: "resolvePath",
-                path: "",
-                directory: o.Video
-            }
-        })
-    }
-    async function wt() {
-        return q()
-    }
-    async function q() {
-        return n({
-            __tauriModule: "Path",
-            message: {
-                cmd: "resolvePath",
-                path: "",
-                directory: o.AppLog
-            }
-        })
-    }
-    const Mt = W() ? "\\" : "/",
-        Pt = W() ? ";" : ":";
-    async function At(...t) {
-        return n({
-            __tauriModule: "Path",
-            message: {
-                cmd: "resolve",
-                paths: t
-            }
-        })
-    }
-    async function Ot(t) {
-        return n({
-            __tauriModule: "Path",
-            message: {
-                cmd: "normalize",
-                path: t
-            }
-        })
-    }
-    async function Wt(...t) {
-        return n({
-            __tauriModule: "Path",
-            message: {
-                cmd: "join",
-                paths: t
-            }
-        })
-    }
-    async function St(t) {
-        return n({
-            __tauriModule: "Path",
-            message: {
-                cmd: "dirname",
-                path: t
-            }
-        })
-    }
-    async function Dt(t) {
-        return n({
-            __tauriModule: "Path",
-            message: {
-                cmd: "extname",
-                path: t
-            }
-        })
-    }
-    async function Lt(t, e) {
-        return n({
-            __tauriModule: "Path",
-            message: {
-                cmd: "basename",
-                path: t,
-                ext: e
-            }
-        })
-    }
-    async function Tt(t) {
-        return n({
-            __tauriModule: "Path",
-            message: {
-                cmd: "isAbsolute",
-                path: t
-            }
-        })
-    }
-    const Ct = {
-        ...Object.freeze(Object.defineProperty({
-            __proto__: null,
-            get BaseDirectory() {
-                return o
-            },
-            appCacheDir: tt,
-            appConfigDir: G,
-            appDataDir: Be,
-            appDir: Xe,
-            appLocalDataDir: et,
-            appLogDir: q,
-            audioDir: at,
-            basename: Lt,
-            cacheDir: nt,
-            configDir: it,
-            dataDir: rt,
-            delimiter: Pt,
-            desktopDir: st,
-            dirname: St,
-            documentDir: ot,
-            downloadDir: lt,
-            executableDir: ut,
-            extname: Dt,
-            fontDir: ct,
-            homeDir: dt,
-            isAbsolute: Tt,
-            join: Wt,
-            localDataDir: mt,
-            logDir: wt,
-            normalize: Ot,
-            pictureDir: ht,
-            publicDir: _t,
-            resolve: At,
-            resolveResource: pt,
-            resourceDir: yt,
-            runtimeDir: gt,
-            sep: Mt,
-            templateDir: ft,
-            videoDir: bt
-        }, Symbol.toStringTag, {
-            value: "Module"
-        }))
-    };
-    async function Et(t = 0) {
-        return n({
-            __tauriModule: "Process",
-            message: {
-                cmd: "exit",
-                exitCode: t
-            }
-        })
-    }
-    async function vt() {
-        return n({
-            __tauriModule: "Process",
-            message: {
-                cmd: "relaunch"
-            }
-        })
-    }
-    const Ft = {
-        ...Object.freeze(Object.defineProperty({
-            __proto__: null,
-            exit: Et,
-            relaunch: vt
-        }, Symbol.toStringTag, {
-            value: "Module"
-        }))
-    };
-    async function jt(t, e, a = [], i) {
-        return typeof a == "object" && Object.freeze(a), n({
-            __tauriModule: "Shell",
-            message: {
-                cmd: "execute",
-                program: e,
-                args: a,
-                options: i,
-                onEventFn: c(t)
-            }
-        })
-    }
-    class p {
-        constructor() {
-            this.eventListeners = Object.create(null)
-        }
-        addListener(e, a) {
-            return this.on(e, a)
-        }
-        removeListener(e, a) {
-            return this.off(e, a)
-        }
-        on(e, a) {
-            return e in this.eventListeners ? this.eventListeners[e].push(a) : this.eventListeners[e] = [a], this
-        }
-        once(e, a) {
-            const i = (...r) => {
-                this.removeListener(e, i), a(...r)
-            };
-            return this.addListener(e, i)
-        }
-        off(e, a) {
-            return e in this.eventListeners && (this.eventListeners[e] = this.eventListeners[e].filter(i => i !== a)), this
-        }
-        removeAllListeners(e) {
-            return e ? delete this.eventListeners[e] : this.eventListeners = Object.create(null), this
-        }
-        emit(e, ...a) {
-            if (e in this.eventListeners) {
-                const i = this.eventListeners[e];
-                for (const r of i) r(...a);
-                return !0
-            }
-            return !1
-        }
-        listenerCount(e) {
-            return e in this.eventListeners ? this.eventListeners[e].length : 0
-        }
-        prependListener(e, a) {
-            return e in this.eventListeners ? this.eventListeners[e].unshift(a) : this.eventListeners[e] = [a], this
-        }
-        prependOnceListener(e, a) {
-            const i = (...r) => {
-                this.removeListener(e, i), a(...r)
-            };
-            return this.prependListener(e, i)
-        }
-    }
-    class J {
-        constructor(e) {
-            this.pid = e
-        }
-        async write(e) {
-            return n({
-                __tauriModule: "Shell",
-                message: {
-                    cmd: "stdinWrite",
-                    pid: this.pid,
-                    buffer: typeof e == "string" ? e : Array.from(e)
-                }
-            })
-        }
-        async kill() {
-            return n({
-                __tauriModule: "Shell",
-                message: {
-                    cmd: "killChild",
-                    pid: this.pid
-                }
-            })
-        }
-    }
-    class S extends p {
-        constructor(e, a = [], i) {
-            super(), this.stdout = new p, this.stderr = new p, this.program = e, this.args = typeof a == "string" ? [a] : a, this.options = i ?? {}
-        }
-        static sidecar(e, a = [], i) {
-            const r = new S(e, a, i);
-            return r.options.sidecar = !0, r
-        }
-        async spawn() {
-            return jt(e => {
-                switch (e.event) {
-                    case "Error":
-                        this.emit("error", e.payload);
-                        break;
-                    case "Terminated":
-                        this.emit("close", e.payload);
-                        break;
-                    case "Stdout":
-                        this.stdout.emit("data", e.payload);
-                        break;
-                    case "Stderr":
-                        this.stderr.emit("data", e.payload);
-                        break
-                }
-            }, this.program, this.args, this.options).then(e => new J(e))
-        }
-        async execute() {
-            return new Promise((e, a) => {
-                this.on("error", a);
-                const i = [],
-                    r = [];
-                this.stdout.on("data", s => {
-                    i.push(s)
-                }), this.stderr.on("data", s => {
-                    r.push(s)
-                }), this.on("close", s => {
-                    e({
-                        code: s.code,
-                        signal: s.signal,
-                        stdout: i.join(`
-`),
-                        stderr: r.join(`
-`)
-                    })
-                }), this.spawn().catch(a)
-            })
-        }
-    }
-    async function zt(t, e) {
-        return n({
-            __tauriModule: "Shell",
-            message: {
-                cmd: "open",
-                path: t,
-                with: e
-            }
-        })
-    }
-    const xt = {
-            ...Object.freeze(Object.defineProperty({
-                __proto__: null,
-                Child: J,
-                Command: S,
-                EventEmitter: p,
-                open: zt
-            }, Symbol.toStringTag, {
-                value: "Module"
-            }))
-        },
-        It = {
-            ...ne
-        };
-    async function D(t) {
-        return M(u.STATUS_UPDATE, e => {
-            t(e == null ? void 0 : e.payload)
-        })
-    }
-    async function Nt() {
-        let t;
-
-        function e() {
-            t && t(), t = void 0
-        }
-        return new Promise((a, i) => {
-            function r(s) {
-                if (s.error) {
-                    e(), i(s.error);
-                    return
-                }
-                s.status === "DONE" && (e(), a())
-            }
-            D(r).then(s => {
-                t = s
-            }).catch(s => {
-                throw e(), s
-            }), A(u.INSTALL_UPDATE).catch(s => {
-                throw e(), s
-            })
-        })
-    }
-    async function Rt() {
-        let t;
-
-        function e() {
-            t && t(), t = void 0
-        }
-        return new Promise((a, i) => {
-            function r(l) {
-                e(), a({
-                    manifest: l,
-                    shouldUpdate: !0
+        Ae = {
+            emits: ["open", "save", "message", "confirm", "ask"],
+            setup(t, {
+                emit: e,
+                expose: a
+            }) {
+                a({
+                    open: async i => e("open", await V(i)),
+                    save: async i => e("save", await q(i)),
+                    message: async i => e("message", await G(i)),
+                    confirm: async i => e("confirm", await K(i)),
+                    ask: async i => e("ask", await J(i))
                 })
             }
-
-            function s(l) {
-                if (l.error) {
-                    e(), i(l.error);
-                    return
-                }
-                l.status === "UPTODATE" && (e(), a({
-                    shouldUpdate: !1
-                }))
-            }
-            P(u.UPDATE_AVAILABLE, l => {
-                r(l == null ? void 0 : l.payload)
-            }).catch(l => {
-                throw e(), l
-            }), D(s).then(l => {
-                t = l
-            }).catch(l => {
-                throw e(), l
-            }), A(u.CHECK_UPDATE).catch(l => {
-                throw e(), l
-            })
-        })
-    }
-    const $t = {
-        ...Object.freeze(Object.defineProperty({
-            __proto__: null,
-            checkUpdate: Rt,
-            installUpdate: Nt,
-            onUpdaterEvent: D
-        }, Symbol.toStringTag, {
-            value: "Module"
-        }))
-    };
-    class K {
+        };
+    class v {
         constructor(e, a) {
             this.type = "Logical", this.width = e, this.height = a
         }
     }
-    class g {
+    class P {
         constructor(e, a) {
             this.type = "Physical", this.width = e, this.height = a
         }
         toLogical(e) {
-            return new K(this.width / e, this.height / e)
+            return new v(this.width / e, this.height / e)
         }
     }
-    class Q {
+    class E {
         constructor(e, a) {
             this.type = "Logical", this.x = e, this.y = a
         }
     }
-    class f {
+    class A {
         constructor(e, a) {
             this.type = "Physical", this.x = e, this.y = a
         }
         toLogical(e) {
-            return new Q(this.x / e, this.y / e)
+            return new E(this.x / e, this.y / e)
         }
     }
-    var b;
+    var S;
     (function(t) {
         t[t.Critical = 1] = "Critical", t[t.Informational = 2] = "Informational"
-    })(b || (b = {}));
+    })(S || (S = {}));
 
-    function Ut() {
-        return new d(window.__TAURI_METADATA__.__currentWindow.label, {
+    function Se() {
+        return new f(window.__TAURI_METADATA__.__currentWindow.label, {
             skip: !0
         })
     }
 
-    function L() {
-        return window.__TAURI_METADATA__.__windows.map(t => new d(t.label, {
+    function F() {
+        return window.__TAURI_METADATA__.__windows.map(t => new f(t.label, {
             skip: !0
         }))
     }
-    const Y = ["tauri://created", "tauri://error"];
-    class Z {
+    const Q = ["tauri://created", "tauri://error"];
+    class Y {
         constructor(e) {
             this.label = e, this.listeners = Object.create(null)
         }
         async listen(e, a) {
             return this._handleTauriEvent(e, a) ? Promise.resolve(() => {
                 const i = this.listeners[e];
                 i.splice(i.indexOf(a), 1)
-            }) : w(e, this.label, a)
+            }) : L(e, this.label, a)
         }
         async once(e, a) {
             return this._handleTauriEvent(e, a) ? Promise.resolve(() => {
                 const i = this.listeners[e];
                 i.splice(i.indexOf(a), 1)
-            }) : j(e, this.label, a)
+            }) : H(e, this.label, a)
         }
         async emit(e, a) {
-            if (Y.includes(e)) {
+            if (Q.includes(e)) {
                 for (const i of this.listeners[e] || []) i({
                     event: e,
                     id: -1,
                     windowLabel: this.label,
                     payload: a
                 });
                 return Promise.resolve()
             }
-            return F(e, this.label, a)
+            return k(e, this.label, a)
         }
         _handleTauriEvent(e, a) {
-            return Y.includes(e) ? (e in this.listeners ? this.listeners[e].push(a) : this.listeners[e] = [a], !0) : !1
+            return Q.includes(e) ? (e in this.listeners ? this.listeners[e].push(a) : this.listeners[e] = [a], !0) : !1
         }
     }
-    class X extends Z {
+    class Z extends Y {
         async scaleFactor() {
             return n({
                 __tauriModule: "Window",
                 message: {
                     cmd: "manage",
                     data: {
                         label: this.label,
@@ -1507,15 +334,15 @@
                             type: "innerPosition"
                         }
                     }
                 }
             }).then(({
                 x: e,
                 y: a
-            }) => new f(e, a))
+            }) => new A(e, a))
         }
         async outerPosition() {
             return n({
                 __tauriModule: "Window",
                 message: {
                     cmd: "manage",
                     data: {
@@ -1524,15 +351,15 @@
                             type: "outerPosition"
                         }
                     }
                 }
             }).then(({
                 x: e,
                 y: a
-            }) => new f(e, a))
+            }) => new A(e, a))
         }
         async innerSize() {
             return n({
                 __tauriModule: "Window",
                 message: {
                     cmd: "manage",
                     data: {
@@ -1541,15 +368,15 @@
                             type: "innerSize"
                         }
                     }
                 }
             }).then(({
                 width: e,
                 height: a
-            }) => new g(e, a))
+            }) => new P(e, a))
         }
         async outerSize() {
             return n({
                 __tauriModule: "Window",
                 message: {
                     cmd: "manage",
                     data: {
@@ -1558,15 +385,15 @@
                             type: "outerSize"
                         }
                     }
                 }
             }).then(({
                 width: e,
                 height: a
-            }) => new g(e, a))
+            }) => new P(e, a))
         }
         async isFullscreen() {
             return n({
                 __tauriModule: "Window",
                 message: {
                     cmd: "manage",
                     data: {
@@ -1744,15 +571,15 @@
                         }
                     }
                 }
             })
         }
         async requestUserAttention(e) {
             let a = null;
-            return e && (e === b.Critical ? a = {
+            return e && (e === S.Critical ? a = {
                 type: "Critical"
             } : a = {
                 type: "Informational"
             }), n({
                 __tauriModule: "Window",
                 message: {
                     cmd: "manage",
@@ -2240,101 +1067,101 @@
                             type: "startDragging"
                         }
                     }
                 }
             })
         }
         async onResized(e) {
-            return this.listen(u.WINDOW_RESIZED, a => {
-                a.payload = te(a.payload), e(a)
+            return this.listen(d.WINDOW_RESIZED, a => {
+                a.payload = ee(a.payload), e(a)
             })
         }
         async onMoved(e) {
-            return this.listen(u.WINDOW_MOVED, a => {
-                a.payload = ee(a.payload), e(a)
+            return this.listen(d.WINDOW_MOVED, a => {
+                a.payload = B(a.payload), e(a)
             })
         }
         async onCloseRequested(e) {
-            return this.listen(u.WINDOW_CLOSE_REQUESTED, a => {
-                const i = new B(a);
+            return this.listen(d.WINDOW_CLOSE_REQUESTED, a => {
+                const i = new X(a);
                 Promise.resolve(e(i)).then(() => {
                     if (!i.isPreventDefault()) return this.close()
                 })
             })
         }
         async onFocusChanged(e) {
-            const a = await this.listen(u.WINDOW_FOCUS, r => {
+            const a = await this.listen(d.WINDOW_FOCUS, r => {
                     e({
                         ...r,
                         payload: !0
                     })
                 }),
-                i = await this.listen(u.WINDOW_BLUR, r => {
+                i = await this.listen(d.WINDOW_BLUR, r => {
                     e({
                         ...r,
                         payload: !1
                     })
                 });
             return () => {
                 a(), i()
             }
         }
         async onScaleChanged(e) {
-            return this.listen(u.WINDOW_SCALE_FACTOR_CHANGED, e)
+            return this.listen(d.WINDOW_SCALE_FACTOR_CHANGED, e)
         }
         async onMenuClicked(e) {
-            return this.listen(u.MENU, e)
+            return this.listen(d.MENU, e)
         }
         async onFileDropEvent(e) {
-            const a = await this.listen(u.WINDOW_FILE_DROP, s => {
+            const a = await this.listen(d.WINDOW_FILE_DROP, s => {
                     e({
                         ...s,
                         payload: {
                             type: "drop",
                             paths: s.payload
                         }
                     })
                 }),
-                i = await this.listen(u.WINDOW_FILE_DROP_HOVER, s => {
+                i = await this.listen(d.WINDOW_FILE_DROP_HOVER, s => {
                     e({
                         ...s,
                         payload: {
                             type: "hover",
                             paths: s.payload
                         }
                     })
                 }),
-                r = await this.listen(u.WINDOW_FILE_DROP_CANCELLED, s => {
+                r = await this.listen(d.WINDOW_FILE_DROP_CANCELLED, s => {
                     e({
                         ...s,
                         payload: {
                             type: "cancel"
                         }
                     })
                 });
             return () => {
                 a(), i(), r()
             }
         }
         async onThemeChanged(e) {
-            return this.listen(u.WINDOW_THEME_CHANGED, e)
+            return this.listen(d.WINDOW_THEME_CHANGED, e)
         }
     }
-    class B {
+    class X {
         constructor(e) {
             this._preventDefault = !1, this.event = e.event, this.windowLabel = e.windowLabel, this.id = e.id
         }
         preventDefault() {
             this._preventDefault = !0
         }
         isPreventDefault() {
             return this._preventDefault
         }
     }
-    class d extends X {
+    class f extends Z {
         constructor(e, a = {}) {
             super(e), a != null && a.skip || n({
                 __tauriModule: "Window",
                 message: {
                     cmd: "createWebview",
                     data: {
                         options: {
@@ -2342,136 +1169,1523 @@
                             ...a
                         }
                     }
                 }
             }).then(async () => this.emit("tauri://created")).catch(async i => this.emit("tauri://error", i))
         }
         static getByLabel(e) {
-            return L().some(a => a.label === e) ? new d(e, {
+            return F().some(a => a.label === e) ? new f(e, {
                 skip: !0
             }) : null
         }
         static async getFocusedWindow() {
-            for (const e of L())
+            for (const e of F())
                 if (await e.isFocused()) return e;
             return null
         }
     }
-    let T;
-    "__TAURI_METADATA__" in window ? T = new d(window.__TAURI_METADATA__.__currentWindow.label, {
+    let O;
+    "__TAURI_METADATA__" in window ? O = new f(window.__TAURI_METADATA__.__currentWindow.label, {
         skip: !0
     }) : (console.warn(`Could not find "window.__TAURI_METADATA__". The "appWindow" value will reference the "main" window label.
-Note that this is not an issue if running this frontend on a browser instead of a Tauri window.`), T = new d("main", {
+Note that this is not an issue if running this frontend on a browser instead of a Tauri window.`), O = new f("main", {
         skip: !0
     }));
 
-    function C(t) {
+    function z(t) {
         return t === null ? null : {
             name: t.name,
             scaleFactor: t.scaleFactor,
-            position: ee(t.position),
-            size: te(t.size)
+            position: B(t.position),
+            size: ee(t.size)
         }
     }
 
-    function ee(t) {
-        return new f(t.x, t.y)
+    function B(t) {
+        return new A(t.x, t.y)
     }
 
-    function te(t) {
-        return new g(t.width, t.height)
+    function ee(t) {
+        return new P(t.width, t.height)
     }
-    async function kt() {
+    async function Oe() {
         return n({
             __tauriModule: "Window",
             message: {
                 cmd: "manage",
                 data: {
                     cmd: {
                         type: "currentMonitor"
                     }
                 }
             }
-        }).then(C)
+        }).then(z)
     }
-    async function Ht() {
+    async function We() {
         return n({
             __tauriModule: "Window",
             message: {
                 cmd: "manage",
                 data: {
                     cmd: {
                         type: "primaryMonitor"
                     }
                 }
             }
-        }).then(C)
+        }).then(z)
     }
-    async function Vt() {
+    async function Le() {
         return n({
             __tauriModule: "Window",
             message: {
                 cmd: "manage",
                 data: {
                     cmd: {
                         type: "availableMonitors"
                     }
                 }
             }
-        }).then(t => t.map(C))
+        }).then(t => t.map(z))
     }
-    const Gt = {
-            ...Object.freeze(Object.defineProperty({
-                __proto__: null,
-                CloseRequestedEvent: B,
-                LogicalPosition: Q,
-                LogicalSize: K,
-                PhysicalPosition: f,
-                PhysicalSize: g,
-                get UserAttentionType() {
-                    return b
+    const De = Object.freeze(Object.defineProperty({
+            __proto__: null,
+            CloseRequestedEvent: X,
+            LogicalPosition: E,
+            LogicalSize: v,
+            PhysicalPosition: A,
+            PhysicalSize: P,
+            get UserAttentionType() {
+                return S
+            },
+            WebviewWindow: f,
+            WebviewWindowHandle: Y,
+            WindowManager: Z,
+            get appWindow() {
+                return O
+            },
+            availableMonitors: Le,
+            currentMonitor: Oe,
+            getAll: F,
+            getCurrent: Se,
+            primaryMonitor: We
+        }, Symbol.toStringTag, {
+            value: "Module"
+        })),
+        te = ["x", "y", "width", "height"];
+    let Te = 1;
+    const ae = {
+        TauriEvents: Me,
+        TauriDialog: Ae,
+        TauriWindow: {
+            props: {
+                main: {
+                    type: Boolean,
+                    default: !1
+                },
+                title: {
+                    type: String,
+                    default: ""
+                },
+                url: {
+                    type: String
+                },
+                visible: {
+                    type: Boolean,
+                    default: !1
+                },
+                width: {
+                    type: Number,
+                    default: -1
+                },
+                height: {
+                    type: Number,
+                    default: -1
+                },
+                x: {
+                    type: Number,
+                    default: -1
                 },
-                WebviewWindow: d,
-                WebviewWindowHandle: Z,
-                WindowManager: X,
-                get appWindow() {
-                    return T
+                y: {
+                    type: Number,
+                    default: -1
                 },
-                availableMonitors: Vt,
-                currentMonitor: kt,
-                getAll: L,
-                getCurrent: Ut,
-                primaryMonitor: Ht
+                options: {
+                    type: Object,
+                    default: () => ({})
+                },
+                preventClose: {
+                    type: Boolean,
+                    default: !1
+                }
+            },
+            emits: ["created", "closed", "fileDrop", "focusChanged", "menuClicked", "moved", "resized", "scaleChanged", "themeChanged"],
+            setup(t, {
+                emit: e,
+                expose: a
+            }) {
+                const i = y.ref([0, 0]),
+                    r = y.ref([0, 0]),
+                    s = y.ref(1),
+                    u = `tauri_window_label_${Te++}`,
+                    ce = {
+                        ...t.options,
+                        url: t.url,
+                        title: t.title,
+                        visible: t.visible
+                    };
+                for (let o = 0; o < te.length; o++) {
+                    const c = te[o];
+                    t[c] > 0 && (ce[c] = Number(t[c]))
+                }
+                const m = t.main ? O : new f(u, ce),
+                    _ = [];
+                y.onBeforeUnmount(() => {
+                    for (; _.length;) _.pop()();
+                    R(), de()
+                }), t.main ? m.scaleFactor().then(o => {
+                    s.value = o, m.outerPosition().then(c => {
+                        const p = c.toLogical(o);
+                        i.value = [p.x, p.y]
+                    }), m.outerSize().then(c => {
+                        const p = c.toLogical(o);
+                        r.value = [p.width, p.height]
+                    })
+                }) : m.once("tauri://created", async () => {
+                    s.value = await m.scaleFactor();
+                    const o = (await m.outerPosition()).toLogical(s.value),
+                        c = (await m.outerSize()).toLogical(s.value);
+                    i.value = [o.x, o.y], r.value = [c.width, c.height], e("created", {
+                        scaleFactor: s.value,
+                        position: i.value,
+                        size: r.value
+                    })
+                }), m.once("tauri://error", function(o) {
+                    console.error("Tauri window error"), console.error(o)
+                }), _.push(m.onCloseRequested(o => {
+                    e("closed"), t.preventClose && o.preventDefault()
+                })), _.push(m.onFileDropEvent(o => {
+                    e("fileDrop", o)
+                })), _.push(m.onFocusChanged(({
+                    payload: o
+                }) => {
+                    e("focusChanged", o)
+                })), _.push(m.onMenuClicked(({
+                    payload: o
+                }) => {
+                    e("menuClicked", o)
+                })), _.push(m.onMoved(async ({
+                    payload: o
+                }) => {
+                    const c = o.toLogical(s.value),
+                        p = [c.x, c.y];
+                    i.value = p, e("moved", p)
+                })), _.push(m.onResized(({
+                    payload: o
+                }) => {
+                    const c = o.toLogical(s.value);
+                    r.value = [c.width, c.height], e("resized", r.value)
+                })), _.push(m.onScaleChanged(({
+                    payload: o
+                }) => {
+                    s.value = o.scaleFactor, e("scaleChanged", o.scaleFactor)
+                })), _.push(m.onThemeChanged(({
+                    payload: o
+                }) => {
+                    e("themeChanged", o)
+                })), y.watch(() => t.title, _e), y.watch(() => [t.x, t.y], o => he(o[0], o[1])), y.watch(() => [t.width, t.height], o => ye(o[0], o[1])), y.watch(() => t.visible, o => (o ? me : R)());
+
+                function h() {
+                    return m
+                }
+
+                function ha() {
+                    return h().center()
+                }
+
+                function de() {
+                    return h().close()
+                }
+
+                function me() {
+                    return h().show()
+                }
+
+                function R() {
+                    return h().hide()
+                }
+
+                function ya() {
+                    return h().maximize()
+                }
+
+                function _a() {
+                    return h().unmaximize()
+                }
+
+                function fa() {
+                    return h().minimize()
+                }
+
+                function pa() {
+                    return h().unminimize()
+                }
+
+                function ga() {
+                    return h().setFocus()
+                }
+
+                function ba(o = !0) {
+                    return h().setFullscreen(o)
+                }
+
+                function wa(o = null) {
+                    return h().requestUserAttention(o)
+                }
+
+                function he(o, c) {
+                    return h().setPosition(new E(o, c))
+                }
+
+                function ye(o, c) {
+                    return h().setSize(new v(o, c))
+                }
+
+                function _e(o) {
+                    return h().setTitle(o)
+                }
+                const fe = {
+                    getWebWindow: h,
+                    center: ha,
+                    close: de,
+                    show: me,
+                    hide: R,
+                    maximize: ya,
+                    unmaximize: _a,
+                    minimize: fa,
+                    unminimize: pa,
+                    requestUserAttention: wa,
+                    grabFocus: ga,
+                    setFullscreen: ba,
+                    setPosition: he,
+                    setSize: ye,
+                    setTitle: _e
+                };
+                return a(fe), {
+                    getWebWindow: h,
+                    api: fe,
+                    position: i,
+                    size: r,
+                    scaleFactor: s
+                }
+            },
+            template: `
+    <slot
+      :webWindow="getWebWindow()"
+      :api="api"
+      :position="position"
+      :size="size"
+      :scaleFactor="scaleFactor"
+    />`
+        }
+    };
+    async function Ce() {
+        return n({
+            __tauriModule: "App",
+            message: {
+                cmd: "getAppVersion"
+            }
+        })
+    }
+    async function ve() {
+        return n({
+            __tauriModule: "App",
+            message: {
+                cmd: "getAppName"
+            }
+        })
+    }
+    async function Ee() {
+        return n({
+            __tauriModule: "App",
+            message: {
+                cmd: "getTauriVersion"
+            }
+        })
+    }
+    async function Fe() {
+        return n({
+            __tauriModule: "App",
+            message: {
+                cmd: "show"
+            }
+        })
+    }
+    async function ze() {
+        return n({
+            __tauriModule: "App",
+            message: {
+                cmd: "hide"
+            }
+        })
+    }
+    const xe = {
+        ...Object.freeze(Object.defineProperty({
+            __proto__: null,
+            getName: ve,
+            getTauriVersion: Ee,
+            getVersion: Ce,
+            hide: ze,
+            show: Fe
+        }, Symbol.toStringTag, {
+            value: "Module"
+        }))
+    };
+    async function je() {
+        return n({
+            __tauriModule: "Cli",
+            message: {
+                cmd: "cliMatches"
+            }
+        })
+    }
+    const Ne = {
+        ...Object.freeze(Object.defineProperty({
+            __proto__: null,
+            getMatches: je
+        }, Symbol.toStringTag, {
+            value: "Module"
+        }))
+    };
+    async function Ie(t) {
+        return n({
+            __tauriModule: "Clipboard",
+            message: {
+                cmd: "writeText",
+                data: t
+            }
+        })
+    }
+    async function Re() {
+        return n({
+            __tauriModule: "Clipboard",
+            message: {
+                cmd: "readText",
+                data: null
+            }
+        })
+    }
+    const Ue = {
+            ...Object.freeze(Object.defineProperty({
+                __proto__: null,
+                readText: Re,
+                writeText: Ie
+            }, Symbol.toStringTag, {
+                value: "Module"
+            }))
+        },
+        $e = {
+            ...Pe
+        },
+        ke = {
+            ...we
+        };
+    var l;
+    (function(t) {
+        t[t.Audio = 1] = "Audio", t[t.Cache = 2] = "Cache", t[t.Config = 3] = "Config", t[t.Data = 4] = "Data", t[t.LocalData = 5] = "LocalData", t[t.Desktop = 6] = "Desktop", t[t.Document = 7] = "Document", t[t.Download = 8] = "Download", t[t.Executable = 9] = "Executable", t[t.Font = 10] = "Font", t[t.Home = 11] = "Home", t[t.Picture = 12] = "Picture", t[t.Public = 13] = "Public", t[t.Runtime = 14] = "Runtime", t[t.Template = 15] = "Template", t[t.Video = 16] = "Video", t[t.Resource = 17] = "Resource", t[t.App = 18] = "App", t[t.Log = 19] = "Log", t[t.Temp = 20] = "Temp", t[t.AppConfig = 21] = "AppConfig", t[t.AppData = 22] = "AppData", t[t.AppLocalData = 23] = "AppLocalData", t[t.AppCache = 24] = "AppCache", t[t.AppLog = 25] = "AppLog"
+    })(l || (l = {}));
+    async function He(t, e = {}) {
+        return n({
+            __tauriModule: "Fs",
+            message: {
+                cmd: "readTextFile",
+                path: t,
+                options: e
+            }
+        })
+    }
+    async function Ve(t, e = {}) {
+        const a = await n({
+            __tauriModule: "Fs",
+            message: {
+                cmd: "readFile",
+                path: t,
+                options: e
+            }
+        });
+        return Uint8Array.from(a)
+    }
+    async function ne(t, e, a) {
+        typeof a == "object" && Object.freeze(a), typeof t == "object" && Object.freeze(t);
+        const i = {
+            path: "",
+            contents: ""
+        };
+        let r = a;
+        return typeof t == "string" ? i.path = t : (i.path = t.path, i.contents = t.contents), typeof e == "string" ? i.contents = e ?? "" : r = e, n({
+            __tauriModule: "Fs",
+            message: {
+                cmd: "writeFile",
+                path: i.path,
+                contents: Array.from(new TextEncoder().encode(i.contents)),
+                options: r
+            }
+        })
+    }
+    async function qe(t, e, a) {
+        typeof a == "object" && Object.freeze(a), typeof t == "object" && Object.freeze(t);
+        const i = {
+            path: "",
+            contents: []
+        };
+        let r = a;
+        return typeof t == "string" ? i.path = t : (i.path = t.path, i.contents = t.contents), e && "dir" in e ? r = e : typeof t == "string" && (i.contents = e ?? []), n({
+            __tauriModule: "Fs",
+            message: {
+                cmd: "writeFile",
+                path: i.path,
+                contents: Array.from(i.contents instanceof ArrayBuffer ? new Uint8Array(i.contents) : i.contents),
+                options: r
+            }
+        })
+    }
+    async function Ge(t, e = {}) {
+        return n({
+            __tauriModule: "Fs",
+            message: {
+                cmd: "readDir",
+                path: t,
+                options: e
+            }
+        })
+    }
+    async function Je(t, e = {}) {
+        return n({
+            __tauriModule: "Fs",
+            message: {
+                cmd: "createDir",
+                path: t,
+                options: e
+            }
+        })
+    }
+    async function Ke(t, e = {}) {
+        return n({
+            __tauriModule: "Fs",
+            message: {
+                cmd: "removeDir",
+                path: t,
+                options: e
+            }
+        })
+    }
+    async function Qe(t, e, a = {}) {
+        return n({
+            __tauriModule: "Fs",
+            message: {
+                cmd: "copyFile",
+                source: t,
+                destination: e,
+                options: a
+            }
+        })
+    }
+    async function Ye(t, e = {}) {
+        return n({
+            __tauriModule: "Fs",
+            message: {
+                cmd: "removeFile",
+                path: t,
+                options: e
+            }
+        })
+    }
+    async function Ze(t, e, a = {}) {
+        return n({
+            __tauriModule: "Fs",
+            message: {
+                cmd: "renameFile",
+                oldPath: t,
+                newPath: e,
+                options: a
+            }
+        })
+    }
+    async function Xe(t, e = {}) {
+        return n({
+            __tauriModule: "Fs",
+            message: {
+                cmd: "exists",
+                path: t,
+                options: e
+            }
+        })
+    }
+    const Be = {
+        ...Object.freeze(Object.defineProperty({
+            __proto__: null,
+            get BaseDirectory() {
+                return l
+            },
+            get Dir() {
+                return l
+            },
+            copyFile: Qe,
+            createDir: Je,
+            exists: Xe,
+            readBinaryFile: Ve,
+            readDir: Ge,
+            readTextFile: He,
+            removeDir: Ke,
+            removeFile: Ye,
+            renameFile: Ze,
+            writeBinaryFile: qe,
+            writeFile: ne,
+            writeTextFile: ne
+        }, Symbol.toStringTag, {
+            value: "Module"
+        }))
+    };
+    async function et(t, e) {
+        return n({
+            __tauriModule: "GlobalShortcut",
+            message: {
+                cmd: "register",
+                shortcut: t,
+                handler: b(e)
+            }
+        })
+    }
+    async function tt(t, e) {
+        return n({
+            __tauriModule: "GlobalShortcut",
+            message: {
+                cmd: "registerAll",
+                shortcuts: t,
+                handler: b(e)
+            }
+        })
+    }
+    async function at(t) {
+        return n({
+            __tauriModule: "GlobalShortcut",
+            message: {
+                cmd: "isRegistered",
+                shortcut: t
+            }
+        })
+    }
+    async function nt(t) {
+        return n({
+            __tauriModule: "GlobalShortcut",
+            message: {
+                cmd: "unregister",
+                shortcut: t
+            }
+        })
+    }
+    async function it() {
+        return n({
+            __tauriModule: "GlobalShortcut",
+            message: {
+                cmd: "unregisterAll"
+            }
+        })
+    }
+    const rt = {
+        ...Object.freeze(Object.defineProperty({
+            __proto__: null,
+            isRegistered: at,
+            register: et,
+            registerAll: tt,
+            unregister: nt,
+            unregisterAll: it
+        }, Symbol.toStringTag, {
+            value: "Module"
+        }))
+    };
+    var M;
+    (function(t) {
+        t[t.JSON = 1] = "JSON", t[t.Text = 2] = "Text", t[t.Binary = 3] = "Binary"
+    })(M || (M = {}));
+    async function st(t) {
+        const e = {},
+            a = async (i, r) => {
+                if (r !== null) {
+                    let s;
+                    typeof r == "string" ? s = r : r instanceof Uint8Array || Array.isArray(r) ? s = Array.from(r) : r instanceof File ? s = {
+                        file: Array.from(new Uint8Array(await r.arrayBuffer())),
+                        mime: r.type,
+                        fileName: r.name
+                    } : typeof r.file == "string" ? s = {
+                        file: r.file,
+                        mime: r.mime,
+                        fileName: r.fileName
+                    } : s = {
+                        file: Array.from(r.file),
+                        mime: r.mime,
+                        fileName: r.fileName
+                    }, e[String(i)] = s
+                }
+            };
+        if (t instanceof FormData)
+            for (const [i, r] of t) await a(i, r);
+        else
+            for (const [i, r] of Object.entries(t)) await a(i, r);
+        return e
+    }
+    class w {
+        constructor(e, a) {
+            this.type = e, this.payload = a
+        }
+        static form(e) {
+            return new w("Form", e)
+        }
+        static json(e) {
+            return new w("Json", e)
+        }
+        static text(e) {
+            return new w("Text", e)
+        }
+        static bytes(e) {
+            return new w("Bytes", Array.from(e instanceof ArrayBuffer ? new Uint8Array(e) : e))
+        }
+    }
+    class ie {
+        constructor(e) {
+            this.url = e.url, this.status = e.status, this.ok = this.status >= 200 && this.status < 300, this.headers = e.headers, this.rawHeaders = e.rawHeaders, this.data = e.data
+        }
+    }
+    class re {
+        constructor(e) {
+            this.id = e
+        }
+        async drop() {
+            return n({
+                __tauriModule: "Http",
+                message: {
+                    cmd: "dropClient",
+                    client: this.id
+                }
+            })
+        }
+        async request(e) {
+            var i;
+            const a = !e.responseType || e.responseType === M.JSON;
+            return a && (e.responseType = M.Text), ((i = e.body) == null ? void 0 : i.type) === "Form" && (e.body.payload = await st(e.body.payload)), n({
+                __tauriModule: "Http",
+                message: {
+                    cmd: "httpRequest",
+                    client: this.id,
+                    options: e
+                }
+            }).then(r => {
+                const s = new ie(r);
+                if (a) {
+                    try {
+                        s.data = JSON.parse(s.data)
+                    } catch (u) {
+                        if (s.ok && s.data === "") s.data = {};
+                        else if (s.ok) throw Error(`Failed to parse response \`${s.data}\` as JSON: ${u};
+              try setting the \`responseType\` option to \`ResponseType.Text\` or \`ResponseType.Binary\` if the API does not return a JSON response.`)
+                    }
+                    return s
+                }
+                return s
+            })
+        }
+        async get(e, a) {
+            return this.request({
+                method: "GET",
+                url: e,
+                ...a
+            })
+        }
+        async post(e, a, i) {
+            return this.request({
+                method: "POST",
+                url: e,
+                body: a,
+                ...i
+            })
+        }
+        async put(e, a, i) {
+            return this.request({
+                method: "PUT",
+                url: e,
+                body: a,
+                ...i
+            })
+        }
+        async patch(e, a) {
+            return this.request({
+                method: "PATCH",
+                url: e,
+                ...a
+            })
+        }
+        async delete(e, a) {
+            return this.request({
+                method: "DELETE",
+                url: e,
+                ...a
+            })
+        }
+    }
+    async function se(t) {
+        return n({
+            __tauriModule: "Http",
+            message: {
+                cmd: "createClient",
+                options: t
+            }
+        }).then(e => new re(e))
+    }
+    let x = null;
+    async function ot(t, e) {
+        return x === null && (x = await se()), x.request({
+            url: t,
+            method: (e == null ? void 0 : e.method) ?? "GET",
+            ...e
+        })
+    }
+    const lt = {
+        ...Object.freeze(Object.defineProperty({
+            __proto__: null,
+            Body: w,
+            Client: re,
+            Response: ie,
+            get ResponseType() {
+                return M
+            },
+            fetch: ot,
+            getClient: se
+        }, Symbol.toStringTag, {
+            value: "Module"
+        }))
+    };
+    async function ut() {
+        return window.Notification.permission !== "default" ? Promise.resolve(window.Notification.permission === "granted") : n({
+            __tauriModule: "Notification",
+            message: {
+                cmd: "isNotificationPermissionGranted"
+            }
+        })
+    }
+    async function ct() {
+        return window.Notification.requestPermission()
+    }
+
+    function dt(t) {
+        typeof t == "string" ? new window.Notification(t) : new window.Notification(t.title, t)
+    }
+    const mt = {
+        ...Object.freeze(Object.defineProperty({
+            __proto__: null,
+            isPermissionGranted: ut,
+            requestPermission: ct,
+            sendNotification: dt
+        }, Symbol.toStringTag, {
+            value: "Module"
+        }))
+    };
+
+    function j() {
+        return navigator.appVersion.includes("Win")
+    }
+    const ht = j() ? `\r
+` : `
+`;
+    async function yt() {
+        return n({
+            __tauriModule: "Os",
+            message: {
+                cmd: "platform"
+            }
+        })
+    }
+    async function _t() {
+        return n({
+            __tauriModule: "Os",
+            message: {
+                cmd: "version"
+            }
+        })
+    }
+    async function ft() {
+        return n({
+            __tauriModule: "Os",
+            message: {
+                cmd: "osType"
+            }
+        })
+    }
+    async function pt() {
+        return n({
+            __tauriModule: "Os",
+            message: {
+                cmd: "arch"
+            }
+        })
+    }
+    async function gt() {
+        return n({
+            __tauriModule: "Os",
+            message: {
+                cmd: "tempdir"
+            }
+        })
+    }
+    async function bt() {
+        return n({
+            __tauriModule: "Os",
+            message: {
+                cmd: "locale"
+            }
+        })
+    }
+    const wt = {
+        ...Object.freeze(Object.defineProperty({
+            __proto__: null,
+            EOL: ht,
+            arch: pt,
+            locale: bt,
+            platform: yt,
+            tempdir: gt,
+            type: ft,
+            version: _t
+        }, Symbol.toStringTag, {
+            value: "Module"
+        }))
+    };
+    async function Mt() {
+        return oe()
+    }
+    async function oe() {
+        return n({
+            __tauriModule: "Path",
+            message: {
+                cmd: "resolvePath",
+                path: "",
+                directory: l.AppConfig
+            }
+        })
+    }
+    async function Pt() {
+        return n({
+            __tauriModule: "Path",
+            message: {
+                cmd: "resolvePath",
+                path: "",
+                directory: l.AppData
+            }
+        })
+    }
+    async function At() {
+        return n({
+            __tauriModule: "Path",
+            message: {
+                cmd: "resolvePath",
+                path: "",
+                directory: l.AppLocalData
+            }
+        })
+    }
+    async function St() {
+        return n({
+            __tauriModule: "Path",
+            message: {
+                cmd: "resolvePath",
+                path: "",
+                directory: l.AppCache
+            }
+        })
+    }
+    async function Ot() {
+        return n({
+            __tauriModule: "Path",
+            message: {
+                cmd: "resolvePath",
+                path: "",
+                directory: l.Audio
+            }
+        })
+    }
+    async function Wt() {
+        return n({
+            __tauriModule: "Path",
+            message: {
+                cmd: "resolvePath",
+                path: "",
+                directory: l.Cache
+            }
+        })
+    }
+    async function Lt() {
+        return n({
+            __tauriModule: "Path",
+            message: {
+                cmd: "resolvePath",
+                path: "",
+                directory: l.Config
+            }
+        })
+    }
+    async function Dt() {
+        return n({
+            __tauriModule: "Path",
+            message: {
+                cmd: "resolvePath",
+                path: "",
+                directory: l.Data
+            }
+        })
+    }
+    async function Tt() {
+        return n({
+            __tauriModule: "Path",
+            message: {
+                cmd: "resolvePath",
+                path: "",
+                directory: l.Desktop
+            }
+        })
+    }
+    async function Ct() {
+        return n({
+            __tauriModule: "Path",
+            message: {
+                cmd: "resolvePath",
+                path: "",
+                directory: l.Document
+            }
+        })
+    }
+    async function vt() {
+        return n({
+            __tauriModule: "Path",
+            message: {
+                cmd: "resolvePath",
+                path: "",
+                directory: l.Download
+            }
+        })
+    }
+    async function Et() {
+        return n({
+            __tauriModule: "Path",
+            message: {
+                cmd: "resolvePath",
+                path: "",
+                directory: l.Executable
+            }
+        })
+    }
+    async function Ft() {
+        return n({
+            __tauriModule: "Path",
+            message: {
+                cmd: "resolvePath",
+                path: "",
+                directory: l.Font
+            }
+        })
+    }
+    async function zt() {
+        return n({
+            __tauriModule: "Path",
+            message: {
+                cmd: "resolvePath",
+                path: "",
+                directory: l.Home
+            }
+        })
+    }
+    async function xt() {
+        return n({
+            __tauriModule: "Path",
+            message: {
+                cmd: "resolvePath",
+                path: "",
+                directory: l.LocalData
+            }
+        })
+    }
+    async function jt() {
+        return n({
+            __tauriModule: "Path",
+            message: {
+                cmd: "resolvePath",
+                path: "",
+                directory: l.Picture
+            }
+        })
+    }
+    async function Nt() {
+        return n({
+            __tauriModule: "Path",
+            message: {
+                cmd: "resolvePath",
+                path: "",
+                directory: l.Public
+            }
+        })
+    }
+    async function It() {
+        return n({
+            __tauriModule: "Path",
+            message: {
+                cmd: "resolvePath",
+                path: "",
+                directory: l.Resource
+            }
+        })
+    }
+    async function Rt(t) {
+        return n({
+            __tauriModule: "Path",
+            message: {
+                cmd: "resolvePath",
+                path: t,
+                directory: l.Resource
+            }
+        })
+    }
+    async function Ut() {
+        return n({
+            __tauriModule: "Path",
+            message: {
+                cmd: "resolvePath",
+                path: "",
+                directory: l.Runtime
+            }
+        })
+    }
+    async function $t() {
+        return n({
+            __tauriModule: "Path",
+            message: {
+                cmd: "resolvePath",
+                path: "",
+                directory: l.Template
+            }
+        })
+    }
+    async function kt() {
+        return n({
+            __tauriModule: "Path",
+            message: {
+                cmd: "resolvePath",
+                path: "",
+                directory: l.Video
+            }
+        })
+    }
+    async function Ht() {
+        return le()
+    }
+    async function le() {
+        return n({
+            __tauriModule: "Path",
+            message: {
+                cmd: "resolvePath",
+                path: "",
+                directory: l.AppLog
+            }
+        })
+    }
+    const Vt = j() ? "\\" : "/",
+        qt = j() ? ";" : ":";
+    async function Gt(...t) {
+        return n({
+            __tauriModule: "Path",
+            message: {
+                cmd: "resolve",
+                paths: t
+            }
+        })
+    }
+    async function Jt(t) {
+        return n({
+            __tauriModule: "Path",
+            message: {
+                cmd: "normalize",
+                path: t
+            }
+        })
+    }
+    async function Kt(...t) {
+        return n({
+            __tauriModule: "Path",
+            message: {
+                cmd: "join",
+                paths: t
+            }
+        })
+    }
+    async function Qt(t) {
+        return n({
+            __tauriModule: "Path",
+            message: {
+                cmd: "dirname",
+                path: t
+            }
+        })
+    }
+    async function Yt(t) {
+        return n({
+            __tauriModule: "Path",
+            message: {
+                cmd: "extname",
+                path: t
+            }
+        })
+    }
+    async function Zt(t, e) {
+        return n({
+            __tauriModule: "Path",
+            message: {
+                cmd: "basename",
+                path: t,
+                ext: e
+            }
+        })
+    }
+    async function Xt(t) {
+        return n({
+            __tauriModule: "Path",
+            message: {
+                cmd: "isAbsolute",
+                path: t
+            }
+        })
+    }
+    const Bt = {
+        ...Object.freeze(Object.defineProperty({
+            __proto__: null,
+            get BaseDirectory() {
+                return l
+            },
+            appCacheDir: St,
+            appConfigDir: oe,
+            appDataDir: Pt,
+            appDir: Mt,
+            appLocalDataDir: At,
+            appLogDir: le,
+            audioDir: Ot,
+            basename: Zt,
+            cacheDir: Wt,
+            configDir: Lt,
+            dataDir: Dt,
+            delimiter: qt,
+            desktopDir: Tt,
+            dirname: Qt,
+            documentDir: Ct,
+            downloadDir: vt,
+            executableDir: Et,
+            extname: Yt,
+            fontDir: Ft,
+            homeDir: zt,
+            isAbsolute: Xt,
+            join: Kt,
+            localDataDir: xt,
+            logDir: Ht,
+            normalize: Jt,
+            pictureDir: jt,
+            publicDir: Nt,
+            resolve: Gt,
+            resolveResource: Rt,
+            resourceDir: It,
+            runtimeDir: Ut,
+            sep: Vt,
+            templateDir: $t,
+            videoDir: kt
+        }, Symbol.toStringTag, {
+            value: "Module"
+        }))
+    };
+    async function ea(t = 0) {
+        return n({
+            __tauriModule: "Process",
+            message: {
+                cmd: "exit",
+                exitCode: t
+            }
+        })
+    }
+    async function ta() {
+        return n({
+            __tauriModule: "Process",
+            message: {
+                cmd: "relaunch"
+            }
+        })
+    }
+    const aa = {
+        ...Object.freeze(Object.defineProperty({
+            __proto__: null,
+            exit: ea,
+            relaunch: ta
+        }, Symbol.toStringTag, {
+            value: "Module"
+        }))
+    };
+    async function na(t, e, a = [], i) {
+        return typeof a == "object" && Object.freeze(a), n({
+            __tauriModule: "Shell",
+            message: {
+                cmd: "execute",
+                program: e,
+                args: a,
+                options: i,
+                onEventFn: b(t)
+            }
+        })
+    }
+    class W {
+        constructor() {
+            this.eventListeners = Object.create(null)
+        }
+        addListener(e, a) {
+            return this.on(e, a)
+        }
+        removeListener(e, a) {
+            return this.off(e, a)
+        }
+        on(e, a) {
+            return e in this.eventListeners ? this.eventListeners[e].push(a) : this.eventListeners[e] = [a], this
+        }
+        once(e, a) {
+            const i = (...r) => {
+                this.removeListener(e, i), a(...r)
+            };
+            return this.addListener(e, i)
+        }
+        off(e, a) {
+            return e in this.eventListeners && (this.eventListeners[e] = this.eventListeners[e].filter(i => i !== a)), this
+        }
+        removeAllListeners(e) {
+            return e ? delete this.eventListeners[e] : this.eventListeners = Object.create(null), this
+        }
+        emit(e, ...a) {
+            if (e in this.eventListeners) {
+                const i = this.eventListeners[e];
+                for (const r of i) r(...a);
+                return !0
+            }
+            return !1
+        }
+        listenerCount(e) {
+            return e in this.eventListeners ? this.eventListeners[e].length : 0
+        }
+        prependListener(e, a) {
+            return e in this.eventListeners ? this.eventListeners[e].unshift(a) : this.eventListeners[e] = [a], this
+        }
+        prependOnceListener(e, a) {
+            const i = (...r) => {
+                this.removeListener(e, i), a(...r)
+            };
+            return this.prependListener(e, i)
+        }
+    }
+    class ue {
+        constructor(e) {
+            this.pid = e
+        }
+        async write(e) {
+            return n({
+                __tauriModule: "Shell",
+                message: {
+                    cmd: "stdinWrite",
+                    pid: this.pid,
+                    buffer: typeof e == "string" ? e : Array.from(e)
+                }
+            })
+        }
+        async kill() {
+            return n({
+                __tauriModule: "Shell",
+                message: {
+                    cmd: "killChild",
+                    pid: this.pid
+                }
+            })
+        }
+    }
+    class N extends W {
+        constructor(e, a = [], i) {
+            super(), this.stdout = new W, this.stderr = new W, this.program = e, this.args = typeof a == "string" ? [a] : a, this.options = i ?? {}
+        }
+        static sidecar(e, a = [], i) {
+            const r = new N(e, a, i);
+            return r.options.sidecar = !0, r
+        }
+        async spawn() {
+            return na(e => {
+                switch (e.event) {
+                    case "Error":
+                        this.emit("error", e.payload);
+                        break;
+                    case "Terminated":
+                        this.emit("close", e.payload);
+                        break;
+                    case "Stdout":
+                        this.stdout.emit("data", e.payload);
+                        break;
+                    case "Stderr":
+                        this.stderr.emit("data", e.payload);
+                        break
+                }
+            }, this.program, this.args, this.options).then(e => new ue(e))
+        }
+        async execute() {
+            return new Promise((e, a) => {
+                this.on("error", a);
+                const i = [],
+                    r = [];
+                this.stdout.on("data", s => {
+                    i.push(s)
+                }), this.stderr.on("data", s => {
+                    r.push(s)
+                }), this.on("close", s => {
+                    e({
+                        code: s.code,
+                        signal: s.signal,
+                        stdout: i.join(`
+`),
+                        stderr: r.join(`
+`)
+                    })
+                }), this.spawn().catch(a)
+            })
+        }
+    }
+    async function ia(t, e) {
+        return n({
+            __tauriModule: "Shell",
+            message: {
+                cmd: "open",
+                path: t,
+                with: e
+            }
+        })
+    }
+    const ra = {
+            ...Object.freeze(Object.defineProperty({
+                __proto__: null,
+                Child: ue,
+                Command: N,
+                EventEmitter: W,
+                open: ia
             }, Symbol.toStringTag, {
                 value: "Module"
             }))
         },
-        qt = {
+        sa = {
+            ...be
+        };
+    async function I(t) {
+        return D(d.STATUS_UPDATE, e => {
+            t(e == null ? void 0 : e.payload)
+        })
+    }
+    async function oa() {
+        let t;
+
+        function e() {
+            t && t(), t = void 0
+        }
+        return new Promise((a, i) => {
+            function r(s) {
+                if (s.error) {
+                    e(), i(s.error);
+                    return
+                }
+                s.status === "DONE" && (e(), a())
+            }
+            I(r).then(s => {
+                t = s
+            }).catch(s => {
+                throw e(), s
+            }), C(d.INSTALL_UPDATE).catch(s => {
+                throw e(), s
+            })
+        })
+    }
+    async function la() {
+        let t;
+
+        function e() {
+            t && t(), t = void 0
+        }
+        return new Promise((a, i) => {
+            function r(u) {
+                e(), a({
+                    manifest: u,
+                    shouldUpdate: !0
+                })
+            }
+
+            function s(u) {
+                if (u.error) {
+                    e(), i(u.error);
+                    return
+                }
+                u.status === "UPTODATE" && (e(), a({
+                    shouldUpdate: !1
+                }))
+            }
+            T(d.UPDATE_AVAILABLE, u => {
+                r(u == null ? void 0 : u.payload)
+            }).catch(u => {
+                throw e(), u
+            }), I(s).then(u => {
+                t = u
+            }).catch(u => {
+                throw e(), u
+            }), C(d.CHECK_UPDATE).catch(u => {
+                throw e(), u
+            })
+        })
+    }
+    const ua = {
+            ...Object.freeze(Object.defineProperty({
+                __proto__: null,
+                checkUpdate: la,
+                installUpdate: oa,
+                onUpdaterEvent: I
+            }, Symbol.toStringTag, {
+                value: "Module"
+            }))
+        },
+        ca = {
+            ...De
+        },
+        da = {
             tauri: {
-                app: me,
-                cli: _e,
-                clipboard: ge,
-                dialog: fe,
-                event: be,
-                fs: Ce,
-                globalShortcut: xe,
-                http: Re,
-                notification: He,
-                os: Ze,
-                path: Ct,
-                process: Ft,
-                shell: xt,
-                tauri: It,
-                updater: $t,
-                window: Gt
+                app: xe,
+                cli: Ne,
+                clipboard: Ue,
+                dialog: $e,
+                event: ke,
+                fs: Be,
+                globalShortcut: rt,
+                http: lt,
+                notification: mt,
+                os: wt,
+                path: Bt,
+                process: aa,
+                shell: ra,
+                tauri: sa,
+                updater: ua,
+                window: ca
             }
         };
 
-    function Jt(t) {
-        Object.keys($).forEach(e => {
-            t.component(e, $[e])
-        }), Object.assign(window.trame.utils, qt)
+    function ma(t) {
+        Object.keys(ae).forEach(e => {
+            t.component(e, ae[e])
+        }), Object.assign(window.trame.utils, da)
     }
-    m.install = Jt, Object.defineProperty(m, Symbol.toStringTag, {
+    g.install = ma, Object.defineProperty(g, Symbol.toStringTag, {
         value: "Module"
     })
 });
```

### Comparing `trame-tauri-0.4.0/trame_tauri.egg-info/PKG-INFO` & `trame-tauri-0.5.0/trame_tauri.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trame-tauri
-Version: 0.4.0
+Version: 0.5.0
 Summary: Helper widget to provide simpler integration with Tauri
 Author: Kitware Inc.
 License: Apache Software License
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
```

