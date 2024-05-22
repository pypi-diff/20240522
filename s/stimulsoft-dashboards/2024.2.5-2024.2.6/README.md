# Comparing `tmp/stimulsoft_dashboards-2024.2.5.tar.gz` & `tmp/stimulsoft_dashboards-2024.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stimulsoft_dashboards-2024.2.5.tar", last modified: Wed May  8 10:58:04 2024, max compression
+gzip compressed data, was "stimulsoft_dashboards-2024.2.6.tar", last modified: Mon May 20 14:21:14 2024, max compression
```

## Comparing `stimulsoft_dashboards-2024.2.5.tar` & `stimulsoft_dashboards-2024.2.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 10:58:04.521111 stimulsoft_dashboards-2024.2.5/
--rw-rw-rw-   0        0        0    25131 2024-02-19 11:37:32.000000 stimulsoft_dashboards-2024.2.5/LICENSE.md
--rw-rw-rw-   0        0        0     8477 2024-05-08 10:58:04.521111 stimulsoft_dashboards-2024.2.5/PKG-INFO
--rw-rw-rw-   0        0        0     7676 2024-03-05 12:00:02.000000 stimulsoft_dashboards-2024.2.5/README.md
--rw-rw-rw-   0        0        0       42 2024-05-08 10:58:04.521111 stimulsoft_dashboards-2024.2.5/setup.cfg
--rw-rw-rw-   0        0        0     1217 2024-05-08 10:57:58.000000 stimulsoft_dashboards-2024.2.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-08 10:58:04.514111 stimulsoft_dashboards-2024.2.5/stimulsoft_dashboards/
--rw-rw-rw-   0        0        0        2 2024-01-26 12:17:37.000000 stimulsoft_dashboards-2024.2.5/stimulsoft_dashboards/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 10:58:04.517111 stimulsoft_dashboards-2024.2.5/stimulsoft_dashboards/report/
--rw-rw-rw-   0        0        0      167 2024-02-16 16:29:50.000000 stimulsoft_dashboards-2024.2.5/stimulsoft_dashboards/report/StiDashboard.py
--rw-rw-rw-   0        0        0       40 2024-02-19 15:40:28.000000 stimulsoft_dashboards-2024.2.5/stimulsoft_dashboards/report/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 10:58:04.518111 stimulsoft_dashboards-2024.2.5/stimulsoft_dashboards/resources/
--rw-rw-rw-   0        0        0      660 2024-02-16 16:35:24.000000 stimulsoft_dashboards-2024.2.5/stimulsoft_dashboards/resources/StiResourcesHelper.py
--rw-rw-rw-   0        0        0        2 2024-01-26 12:17:37.000000 stimulsoft_dashboards-2024.2.5/stimulsoft_dashboards/resources/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 10:58:04.520111 stimulsoft_dashboards-2024.2.5/stimulsoft_dashboards/resources/scripts/
--rw-rw-rw-   0        0        0      502 2024-02-16 16:24:27.000000 stimulsoft_dashboards-2024.2.5/stimulsoft_dashboards/resources/scripts/StiScriptResource.py
--rw-rw-rw-   0        0        0        2 2024-01-26 12:17:37.000000 stimulsoft_dashboards-2024.2.5/stimulsoft_dashboards/resources/scripts/__init__.py
--rw-rw-rw-   0        0        0   703489 2024-05-06 08:25:08.000000 stimulsoft_dashboards-2024.2.5/stimulsoft_dashboards/resources/scripts/stimulsoft.dashboards.js
--rw-rw-rw-   0        0        0   195363 2024-05-06 08:27:54.000000 stimulsoft_dashboards-2024.2.5/stimulsoft_dashboards/resources/scripts/stimulsoft.dashboards.pack.js
-drwxrwxrwx   0        0        0        0 2024-05-08 10:58:04.516111 stimulsoft_dashboards-2024.2.5/stimulsoft_dashboards.egg-info/
--rw-rw-rw-   0        0        0     8477 2024-05-08 10:58:04.000000 stimulsoft_dashboards-2024.2.5/stimulsoft_dashboards.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      719 2024-05-08 10:58:04.000000 stimulsoft_dashboards-2024.2.5/stimulsoft_dashboards.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 10:58:04.000000 stimulsoft_dashboards-2024.2.5/stimulsoft_dashboards.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2024-05-08 10:58:04.000000 stimulsoft_dashboards-2024.2.5/stimulsoft_dashboards.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2024-05-08 10:58:04.000000 stimulsoft_dashboards-2024.2.5/stimulsoft_dashboards.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-20 14:21:14.745390 stimulsoft_dashboards-2024.2.6/
+-rw-rw-rw-   0        0        0    25131 2024-02-19 11:37:32.000000 stimulsoft_dashboards-2024.2.6/LICENSE.md
+-rw-rw-rw-   0        0        0     8477 2024-05-20 14:21:14.745390 stimulsoft_dashboards-2024.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0     7676 2024-03-05 12:00:02.000000 stimulsoft_dashboards-2024.2.6/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-20 14:21:14.745390 stimulsoft_dashboards-2024.2.6/setup.cfg
+-rw-rw-rw-   0        0        0     1217 2024-05-20 14:06:36.000000 stimulsoft_dashboards-2024.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 14:21:14.738870 stimulsoft_dashboards-2024.2.6/stimulsoft_dashboards/
+-rw-rw-rw-   0        0        0        2 2024-01-26 12:17:37.000000 stimulsoft_dashboards-2024.2.6/stimulsoft_dashboards/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 14:21:14.741384 stimulsoft_dashboards-2024.2.6/stimulsoft_dashboards/report/
+-rw-rw-rw-   0        0        0      167 2024-02-16 16:29:50.000000 stimulsoft_dashboards-2024.2.6/stimulsoft_dashboards/report/StiDashboard.py
+-rw-rw-rw-   0        0        0       40 2024-02-19 15:40:28.000000 stimulsoft_dashboards-2024.2.6/stimulsoft_dashboards/report/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 14:21:14.741384 stimulsoft_dashboards-2024.2.6/stimulsoft_dashboards/resources/
+-rw-rw-rw-   0        0        0      660 2024-02-16 16:35:24.000000 stimulsoft_dashboards-2024.2.6/stimulsoft_dashboards/resources/StiResourcesHelper.py
+-rw-rw-rw-   0        0        0        2 2024-01-26 12:17:37.000000 stimulsoft_dashboards-2024.2.6/stimulsoft_dashboards/resources/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 14:21:14.744384 stimulsoft_dashboards-2024.2.6/stimulsoft_dashboards/resources/scripts/
+-rw-rw-rw-   0        0        0      502 2024-02-16 16:24:27.000000 stimulsoft_dashboards-2024.2.6/stimulsoft_dashboards/resources/scripts/StiScriptResource.py
+-rw-rw-rw-   0        0        0        2 2024-01-26 12:17:37.000000 stimulsoft_dashboards-2024.2.6/stimulsoft_dashboards/resources/scripts/__init__.py
+-rw-rw-rw-   0        0        0   704284 2024-05-20 13:28:50.000000 stimulsoft_dashboards-2024.2.6/stimulsoft_dashboards/resources/scripts/stimulsoft.dashboards.js
+-rw-rw-rw-   0        0        0   195640 2024-05-20 13:31:42.000000 stimulsoft_dashboards-2024.2.6/stimulsoft_dashboards/resources/scripts/stimulsoft.dashboards.pack.js
+drwxrwxrwx   0        0        0        0 2024-05-20 14:21:14.740384 stimulsoft_dashboards-2024.2.6/stimulsoft_dashboards.egg-info/
+-rw-rw-rw-   0        0        0     8477 2024-05-20 14:21:14.000000 stimulsoft_dashboards-2024.2.6/stimulsoft_dashboards.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      719 2024-05-20 14:21:14.000000 stimulsoft_dashboards-2024.2.6/stimulsoft_dashboards.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 14:21:14.000000 stimulsoft_dashboards-2024.2.6/stimulsoft_dashboards.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2024-05-20 14:21:14.000000 stimulsoft_dashboards-2024.2.6/stimulsoft_dashboards.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2024-05-20 14:21:14.000000 stimulsoft_dashboards-2024.2.6/stimulsoft_dashboards.egg-info/top_level.txt
```

### Comparing `stimulsoft_dashboards-2024.2.5/LICENSE.md` & `stimulsoft_dashboards-2024.2.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `stimulsoft_dashboards-2024.2.5/PKG-INFO` & `stimulsoft_dashboards-2024.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stimulsoft_dashboards
-Version: 2024.2.5
+Version: 2024.2.6
 Summary: Data visualization in Python applications.
 Home-page: https://www.stimulsoft.com/en/products/dashboards-python
 Author: Stimulsoft
 Author-email: info@stimulsoft.com
 License: https://www.stimulsoft.com/en/licensing/developers
 Classifier: License :: Other/Proprietary License
 Classifier: Framework :: Django
```

### Comparing `stimulsoft_dashboards-2024.2.5/README.md` & `stimulsoft_dashboards-2024.2.6/README.md`

 * *Files identical despite different names*

### Comparing `stimulsoft_dashboards-2024.2.5/setup.py` & `stimulsoft_dashboards-2024.2.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md') as file:
     readmeFile = file.read()
 
 setup(
     name = 'stimulsoft_dashboards',
-    version = '2024.2.5',
+    version = '2024.2.6',
     author = 'Stimulsoft',
     author_email = 'info@stimulsoft.com',
     description = 'Data visualization in Python applications.',
     long_description = readmeFile,
     long_description_content_type = 'text/markdown',
     url = 'https://www.stimulsoft.com/en/products/dashboards-python',
     license = 'https://www.stimulsoft.com/en/licensing/developers',
@@ -20,12 +20,12 @@
         'Programming Language :: Python',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: 3.12',
         'Topic :: Office/Business',
         'Topic :: Software Development'
     ],
-    install_requires = ['stimulsoft-reports==2024.2.5'],
+    install_requires = ['stimulsoft-reports==2024.2.6'],
     packages = find_packages(include=['stimulsoft_dashboards', 'stimulsoft_dashboards.*']),
     package_data = {'stimulsoft_dashboards': ['**/scripts/*.js']},
     python_requires = '>=3.10'
 )
```

### Comparing `stimulsoft_dashboards-2024.2.5/stimulsoft_dashboards/resources/StiResourcesHelper.py` & `stimulsoft_dashboards-2024.2.6/stimulsoft_dashboards/resources/StiResourcesHelper.py`

 * *Files identical despite different names*

### Comparing `stimulsoft_dashboards-2024.2.5/stimulsoft_dashboards/resources/scripts/stimulsoft.dashboards.js` & `stimulsoft_dashboards-2024.2.6/stimulsoft_dashboards/resources/scripts/stimulsoft.dashboards.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,26 +1,26 @@
 /*
 Stimulsoft.Dashboards.JS
-Version: 2024.2.5
-Build date: 2024.05.06
+Version: 2024.2.6
+Build date: 2024.05.20
 License: https://www.stimulsoft.com/en/licensing/reports
 */
 ! function(t) {
     var e;
     "undefined" != typeof process && process.__nwjs || "object" != typeof exports || "undefined" == typeof module ? "function" == typeof define && define.amd ? define(["./stimulsoft.reports"], e => Object.assign(e, t(e.Stimulsoft))) : window.Stimulsoft ? window.Stimulsoft.Report && window.Stimulsoft.Report.StiReport ? Object.assign(window, t(window.Stimulsoft)) : window.Stimulsoft.dashboardsFactory = t : window.Stimulsoft = {
         dashboardsFactory: t
     } : module.exports = (e = require("./stimulsoft.reports"), Object.assign(e, t(e.Stimulsoft)))
 }(function(L) {
     var Z = L.StiOptions;
 
     function y(e, t) {
         for (var r in t) r in e ? y(e[r], t[r]) : e[r] = t[r];
         return e
     }
-    L && (L.__engineVersion && "2024.2.5" !== L.__engineVersion ? console.warn("Scripts versions mismatch: engine ver. = %s; dashboards ver. = 2024.2.5", L.__engineVersion) : "2024.2.5" !== L.__reportsVersion && console.warn("Scripts versions mismatch: reports ver. = %s; dashboards ver. = 2024.2.5", L.__reportsVersion));
+    L && (L.__engineVersion && "2024.2.6" !== L.__engineVersion ? console.warn("Scripts versions mismatch: engine ver. = %s; dashboards ver. = 2024.2.6", L.__engineVersion) : "2024.2.6" !== L.__reportsVersion && console.warn("Scripts versions mismatch: reports ver. = %s; dashboards ver. = 2024.2.6", L.__reportsVersion));
     var L = y(L || {}, {
             Dashboard: {
                 Components: {
                     Panel: {},
                     Button: {},
                     Cards: {},
                     Helpers: {},
@@ -1277,17 +1277,17 @@
         }
         F.F.StiMeasureCardsColumn = Fr
     }
     let Fr = F.F.StiMeasureCardsColumn,
         vr = L.Base.Drawing.StiColor,
         Ar = L.Base.Meters.IStiBubbleColumn;
     {
-        class Li extends Fr {
+        class Bi extends Fr {
             implements() {
-                return Li.ImplementsStiBubbleCardsColumn || (Li.ImplementsStiBubbleCardsColumn = super.implements().concat([Ar, l])), Li.ImplementsStiBubbleCardsColumn
+                return Bi.ImplementsStiBubbleCardsColumn || (Bi.ImplementsStiBubbleCardsColumn = super.implements().concat([Ar, l])), Bi.ImplementsStiBubbleCardsColumn
             }
             meta() {
                 return [...super.meta(), new i("HorAlignment", "", z, z.Center), new h("AllowCustomColors"), new r("PositiveColor", "", vr.get("537eb6")), new r("NegativeColor", "", vr.get("ff0000"))]
             }
             getUniqueCode() {
                 let e = super.getUniqueCode();
                 return e = 397 * e ^ this.horAlignment[L.System.StiObject.stimulsoft]().getHashCode(), Math.abs(e)
@@ -1295,39 +1295,39 @@
             get localizedName() {
                 return b.get("Chart", "Bubble")
             }
             constructor(e, t, r, i, s, n, l, a, o, u, h, m, c, d) {
                 super(e, t, r, i, s, n, l, a, o, u, d), this.ident = F.e.StiMeterIdent.BubbleCardsColumn, this.allowCustomColors = !1, this.positiveColor = vr.get("537eb6"), this.negativeColor = vr.get("ff0000"), this.horAlignment = z.Center, null != h && (this.allowCustomColors = h), null != m && (this.positiveColor = m), null != c && (this.negativeColor = c)
             }
         }
-        F.F.StiBubbleCardsColumn = Li
+        F.F.StiBubbleCardsColumn = Bi
     }
     F.F.StiCardsColumnVisibilityHelper = class {
         static getVisible(e, t) {
             if (e.visibility == pr.True) return !0;
             if (e.visibility == pr.False) return !1;
             if (B.isNullOrWhiteSpace(e.visibilityExpression)) return !1;
             let r = O.parse2(e.visibilityExpression, t);
             return V.tryToBool(r)
         }
     };
     let Ir = L.Base.Meters.IStiDimensionCardsColumn;
     {
-        class Hi extends Mr {
+        class zi extends Mr {
             implements() {
-                return Hi.ImplementsStiDimensionCardsColumn || (Hi.ImplementsStiDimensionCardsColumn = super.implements().concat([ze, Ir])), Hi.ImplementsStiDimensionCardsColumn
+                return zi.ImplementsStiDimensionCardsColumn || (zi.ImplementsStiDimensionCardsColumn = super.implements().concat([ze, Ir])), zi.ImplementsStiDimensionCardsColumn
             }
             get localizedName() {
                 return b.get("Dashboard", "Dimension")
             }
             constructor(e, t, r, i, s, n, l, a, o, u, h) {
                 super(e, t, r, i, s, n, l, a, o, u, h), this.ident = F.e.StiMeterIdent.DimensionCardsColumn
             }
         }
-        F.F.StiDimensionCardsColumn = Hi
+        F.F.StiDimensionCardsColumn = zi
     }
     let Dr = L.Base.StiActivator,
         Rr = (F.G.StiMeterLoader = class {
             static loadFromJson2(e) {
                 let t = new P;
                 return e.forEach(e => t.add(this.loadFromJson(e))), t.where(e => null != e)
             }
@@ -1356,54 +1356,54 @@
                 return b.get("PropertyMain", "IndicatorValue")
             }
             constructor(e, t, r) {
                 super(e, t, r), this.ident = F.e.StiMeterIdent.IndicatorValueChartMeter
             }
         }, L.Base.Meters.IStiArgumentMeter);
     {
-        class Ls extends F.e.StiDimensionMeter {
+        class Bs extends F.e.StiDimensionMeter {
             implements() {
-                return Ls.ImplementsStiArgumentChartMeter || (Ls.ImplementsStiArgumentChartMeter = super.implements().concat([Rr])), Ls.ImplementsStiArgumentChartMeter
+                return Bs.ImplementsStiArgumentChartMeter || (Bs.ImplementsStiArgumentChartMeter = super.implements().concat([Rr])), Bs.ImplementsStiArgumentChartMeter
             }
             get localizedName() {
                 return b.get("PropertyMain", "Argument")
             }
             constructor(e, t, r) {
                 super(e, t, r), this.ident = F.e.StiMeterIdent.ArgumentChartMeter
             }
         }
-        F.H.StiArgumentChartMeter = Ls
+        F.H.StiArgumentChartMeter = Bs
     }
     let Er = L.Base.Meters.IStiValueMeter;
     {
-        class Yi extends F.e.StiDimensionMeter {
+        class Ki extends F.e.StiDimensionMeter {
             implements() {
-                return Yi.ImplementsStiKeyTreeViewBoxMeter || (Yi.ImplementsStiKeyTreeViewBoxMeter = super.implements().concat([Er])), Yi.ImplementsStiKeyTreeViewBoxMeter
+                return Ki.ImplementsStiKeyTreeViewBoxMeter || (Ki.ImplementsStiKeyTreeViewBoxMeter = super.implements().concat([Er])), Ki.ImplementsStiKeyTreeViewBoxMeter
             }
             get localizedName() {
                 return b.get("PropertyMain", "Key")
             }
             constructor(e, t, r) {
                 super(e, t, r), this.ident = F.e.StiMeterIdent.KeyTreeViewBoxMeter
             }
         }
-        F.I.StiKeyTreeViewBoxMeter = Yi
+        F.I.StiKeyTreeViewBoxMeter = Ki
     } {
-        class Ki extends F.e.StiDimensionMeter {
+        class Qi extends F.e.StiDimensionMeter {
             implements() {
-                return Ki.ImplementsStiKeyTreeViewMeter || (Ki.ImplementsStiKeyTreeViewMeter = super.implements().concat([Er])), Ki.ImplementsStiKeyTreeViewMeter
+                return Qi.ImplementsStiKeyTreeViewMeter || (Qi.ImplementsStiKeyTreeViewMeter = super.implements().concat([Er])), Qi.ImplementsStiKeyTreeViewMeter
             }
             get localizedName() {
                 return b.get("PropertyMain", "Key")
             }
             constructor(e, t, r) {
                 super(e, t, r), this.ident = F.e.StiMeterIdent.KeyTreeViewMeter
             }
         }
-        F.J.StiKeyTreeViewMeter = Ki
+        F.J.StiKeyTreeViewMeter = Qi
     }
     F.x.StiDashboardInteractionLoader = class {
         static loadInteractionFromJsonObject(e) {
             let t = e.properties().firstOrDefault(e => "Ident" == e.name).value.toString(),
                 r = F.x.StiDashboardInteractionCreator.new2(t);
             return r.loadFromJsonObject(e), r
         }
@@ -1498,17 +1498,17 @@
         Kr = L.Base.StiSummaryColumnType,
         Qr = L.Report.Dashboard.IStiElementInteraction,
         qr = F.x.StiDashboardInteractionLoader,
         _r = F.g.StiTableColumnDashboardInteraction,
         $r = L.Report.Components.ImplementsIStiTextFormat,
         ei = L.Base.Meters.IStiTableColumn;
     {
-        class Cs extends F.e.StiMeter {
+        class xs extends F.e.StiMeter {
             implements() {
-                return Cs.ImplementsStiTableColumn || (Cs.ImplementsStiTableColumn = super.implements().concat([Cr, yr, ei, zr, fr, ...wr, ...$r, ...Sr, l, Qr])), Cs.ImplementsStiTableColumn
+                return xs.ImplementsStiTableColumn || (xs.ImplementsStiTableColumn = super.implements().concat([Cr, yr, ei, zr, fr, ...wr, ...$r, ...Sr, l, Qr])), xs.ImplementsStiTableColumn
             }
             meta() {
                 return [...super.meta(), new i("HorAlignment", "", z, z.Left), new i("SummaryAlignment", "", z, z.Right), new i("HeaderAlignment", "", z, z.Center), new s("TextFormat").check(() => !(this.textFormat.is(Jt) || null == this.textFormat)).set(e => this.textFormat = br.createFromJsonObject(e.value)).setXml(e => {
                     let t = br.loadFormatFromXml(e);
                     null != t && (this.textFormat = t)
                 }), new r("ForeColor", "", N.transparent), new h("ShowTotalSummary"), new i("SummaryType", "", Kr, Kr.Sum), new h("Visible", "", !0).check(() => !1), new i("Visibility", "", Hr, Hr.True), new n("VisibilityExpression").check(() => null != this.visibilityExpression), new s("DashboardInteraction").check(() => null != this.dashboardInteraction.as(_r)).set(e => {
                     var t;
@@ -1543,49 +1543,49 @@
             set visible(e) {
                 this.visibility = e ? Hr.True : Hr.False
             }
             constructor(e, t, r, i, s, n, l, a, o, u, h, m, c) {
                 super(e, t, r), this.horAlignment = z.Left, this.textFormat = new Jt, this.foreColor = N.transparent, this.dashboardInteraction = new _r, this.visibility = Hr.True, this.visibilityExpression = null, this.showTotalSummary = !1, this.summaryType = Kr.Sum, this.summaryAlignment = z.Right, this.headerAlignment = z.Center, null != i && (this.horAlignment = i), null != s && (this.textFormat = s), null != n && (this.visibility = n), null != l && (this.visibilityExpression = l), null != o && (this.showTotalSummary = o), null != h && (this.summaryAlignment = h), null != m && (this.headerAlignment = m), null != u && (this.summaryType = u), null != a && (this.foreColor = a), null != c && (this.dashboardInteraction = c)
             }
         }
-        F.K.StiTableColumn = Cs
+        F.K.StiTableColumn = xs
     } {
-        class is extends F.K.StiTableColumn {
+        class ss extends F.K.StiTableColumn {
             implements() {
-                return is.ImplementsStiMeasureColumn || (is.ImplementsStiMeasureColumn = super.implements().concat([vt, Tr])), is.ImplementsStiMeasureColumn
+                return ss.ImplementsStiMeasureColumn || (ss.ImplementsStiMeasureColumn = super.implements().concat([vt, Tr])), ss.ImplementsStiMeasureColumn
             }
             get localizedName() {
                 return b.get("Dashboard", "Indicator")
             }
             constructor(e, t, r, i, s, n, l, a, o, u, h, m, c) {
                 super(e, t, r, i, s, n, l, a, o, u, h, m, c), this.ident = F.e.StiMeterIdent.MeasureColumn
             }
         }
-        F.K.StiMeasureColumn = is
+        F.K.StiMeasureColumn = ss
     }
     let ti = L.Base.Meters.IStiIndicatorColumn;
     {
-        class Qi extends F.K.StiMeasureColumn {
+        class qi extends F.K.StiMeasureColumn {
             implements() {
-                return Qi.ImplementsStiIndicatorColumn || (Qi.ImplementsStiIndicatorColumn = super.implements().concat([ti])), Qi.ImplementsStiIndicatorColumn
+                return qi.ImplementsStiIndicatorColumn || (qi.ImplementsStiIndicatorColumn = super.implements().concat([ti])), qi.ImplementsStiIndicatorColumn
             }
             get localizedName() {
                 return b.get("Dashboard", "Dimension")
             }
             constructor(e, t, r, i, s, n, l, a, o, u, h) {
                 super(e, t, r, i, s, n, l, a, o, u, h), this.ident = F.e.StiMeterIdent.IndicatorColumn
             }
         }
-        F.K.StiIndicatorColumn = Qi
+        F.K.StiIndicatorColumn = qi
     }
     let ri = L.Base.Meters.IStiColorScaleColumn;
     {
-        class qi extends F.K.StiMeasureColumn {
+        class _i extends F.K.StiMeasureColumn {
             implements() {
-                return qi.ImplementsStiColorScaleColumn || (qi.ImplementsStiColorScaleColumn = super.implements().concat([ri, l])), qi.ImplementsStiColorScaleColumn
+                return _i.ImplementsStiColorScaleColumn || (_i.ImplementsStiColorScaleColumn = super.implements().concat([ri, l])), _i.ImplementsStiColorScaleColumn
             }
             meta() {
                 return [...super.meta(), new r("MinimumColor", "", N.red), new r("MaximumColor", "", N.green)]
             }
             getUniqueCode() {
                 let e = super.getUniqueCode();
                 return e = 397 * (e = 397 * e ^ this.minimumColor[L.System.StiObject.stimulsoft]().getHashCode()) ^ this.maximumColor[L.System.StiObject.stimulsoft]().getHashCode(), Math.abs(e)
@@ -1593,21 +1593,21 @@
             get localizedName() {
                 return b.get("Dashboard", "ColorScale")
             }
             constructor(e, t, r, i, s, n, l, a, o, u, h, m, c) {
                 super(e, t, r, i, s, n, l, a, o, u, h), this.ident = F.e.StiMeterIdent.ColorScaleColumn, this.minimumColor = N.red, this.maximumColor = N.green, null != m && (this.minimumColor = m), null != c && (this.maximumColor = c)
             }
         }
-        F.K.StiColorScaleColumn = qi
+        F.K.StiColorScaleColumn = _i
     }
     let ii = L.Base.Meters.IStiDataBarsColumn;
     {
-        class _i extends F.K.StiMeasureColumn {
+        class $i extends F.K.StiMeasureColumn {
             implements() {
-                return _i.ImplementsStiDataBarsColumn || (_i.ImplementsStiDataBarsColumn = super.implements().concat([ii, l])), _i.ImplementsStiDataBarsColumn
+                return $i.ImplementsStiDataBarsColumn || ($i.ImplementsStiDataBarsColumn = super.implements().concat([ii, l])), $i.ImplementsStiDataBarsColumn
             }
             meta() {
                 return [...super.meta(), new i("HorAlignment", "", z, z.Center), new se("Width", "", 0), new ne("Minimum"), new ne("Maximum"), new r("PositiveColor", "", N.transparent), new r("NegativeColor", "", N.transparent), new r("OverlappedColor", "", N.transparent), new r("FillColor", "", N.transparent)]
             }
             getUniqueCode() {
                 let e = super.getUniqueCode();
                 return e = 397 * (e = 397 * (e = 397 * (e = 397 * (e = 397 * (e = 397 * (e = 397 * (e = 397 * e ^ this.width[L.System.StiObject.stimulsoft]().getHashCode()) ^ this.horAlignment) ^ this.positiveColor.getHashCode()) ^ this.negativeColor.getHashCode()) ^ this.overlappedColor.getHashCode()) ^ this.fillColor.getHashCode()) ^ (null != this.minimum ? this.minimum[L.System.StiObject.stimulsoft]().getHashCode() : 0)) ^ (null != this.maximum ? this.maximum[L.System.StiObject.stimulsoft]().getHashCode() : 0)
@@ -1615,21 +1615,21 @@
             get localizedName() {
                 return b.get("Dashboard", "DataBars")
             }
             constructor(e, t, r, i, s, n, l, a, o, u, h, m, c, d, g, p, S, w, b) {
                 super(e, t, r, i, s, n, l, a, c, d, g), this.ident = F.e.StiMeterIdent.DataBarsColumn, this.width = 0, this.positiveColor = N.transparent, this.negativeColor = N.transparent, this.overlappedColor = N.transparent, this.fillColor = N.transparent, this.minimum = "", this.maximum = "", null != p && (this.headerAlignment = p), null != o && (this.positiveColor = o), null != u && (this.negativeColor = u), null != h && (this.overlappedColor = h), null != m && (this.fillColor = m), null != S && (this.width = S), null != w && (this.minimum = w), null != b && (this.maximum = b)
             }
         }
-        F.K.StiDataBarsColumn = _i
+        F.K.StiDataBarsColumn = $i
     }
     let si = L.Base.Meters.IStiSparklinesColumn;
     {
-        class $i extends F.K.StiMeasureColumn {
+        class es extends F.K.StiMeasureColumn {
             implements() {
-                return $i.ImplementsStiSparklinesColumn || ($i.ImplementsStiSparklinesColumn = super.implements().concat([si, l])), $i.ImplementsStiSparklinesColumn
+                return es.ImplementsStiSparklinesColumn || (es.ImplementsStiSparklinesColumn = super.implements().concat([si, l])), es.ImplementsStiSparklinesColumn
             }
             meta() {
                 return [...super.meta(), new i("Type", "", F.K.StiSparklinesType, F.K.StiSparklinesType.Area), new h("ShowHighLowPoints"), new h("ShowFirstLastPoints", "", !0), new h("AllowCustomColors"), new r("PositiveColor", "", vr.get("537eb6")), new r("NegativeColor", "", vr.get("ff0000"))]
             }
             getUniqueCode() {
                 let e = super.getUniqueCode();
                 return e = 397 * (e = 397 * (e = 397 * (e = 397 * (e = 397 * (e = 397 * e ^ this.type[L.System.StiObject.stimulsoft]().getHashCode()) ^ this.showHighLowPoints[L.System.StiObject.stimulsoft]().getHashCode()) ^ this.showFirstLastPoints[L.System.StiObject.stimulsoft]().getHashCode()) ^ this.allowCustomColors[L.System.StiObject.stimulsoft]().getHashCode()) ^ this.positiveColor[L.System.StiObject.stimulsoft]().getHashCode()) ^ this.negativeColor[L.System.StiObject.stimulsoft]().getHashCode(), Math.abs(e)
@@ -1637,19 +1637,19 @@
             get localizedName() {
                 return b.get("Dashboard", "Sparklines")
             }
             constructor(e, t, r, i, s, n, l, a, o, u, h, m, c, d, g, p, S) {
                 super(e, t, r, i, s, o, u, h, m, c, d), this.type = F.K.StiSparklinesType.Area, this.showHighLowPoints = !1, this.showFirstLastPoints = !0, this.allowCustomColors = !1, this.positiveColor = vr.get("537eb6"), this.negativeColor = vr.get("ff0000"), this.ident = F.e.StiMeterIdent.SparklinesColumn, null != n && (this.type = n), null != l && (this.showHighLowPoints = l), null != a && (this.showFirstLastPoints = a), null != g && (this.allowCustomColors = g), null != p && (this.positiveColor = p), null != S && (this.negativeColor = S)
             }
         }
-        F.K.StiSparklinesColumn = $i
+        F.K.StiSparklinesColumn = es
     } {
-        class Gi extends F.K.StiMeasureColumn {
+        class Xi extends F.K.StiMeasureColumn {
             implements() {
-                return Gi.ImplementsStiBubbleColumn || (Gi.ImplementsStiBubbleColumn = super.implements().concat([Ar, l])), Gi.ImplementsStiBubbleColumn
+                return Xi.ImplementsStiBubbleColumn || (Xi.ImplementsStiBubbleColumn = super.implements().concat([Ar, l])), Xi.ImplementsStiBubbleColumn
             }
             meta() {
                 return [...super.meta(), new i("HorAlignment", "", z, z.Center), new h("AllowCustomColors"), new r("PositiveColor", "", vr.get("537eb6")), new r("NegativeColor", "", vr.get("ff0000"))]
             }
             getUniqueCode() {
                 let e = super.getUniqueCode();
                 return e = 397 * (e = 397 * (e = 397 * e ^ this.allowCustomColors[L.System.StiObject.stimulsoft]().getHashCode()) ^ this.positiveColor[L.System.StiObject.stimulsoft]().getHashCode()) ^ this.negativeColor[L.System.StiObject.stimulsoft]().getHashCode(), Math.abs(e)
@@ -1657,15 +1657,15 @@
             get localizedName() {
                 return b.get("Chart", "Bubble")
             }
             constructor(e, t, r, i, s, n, l, a, o, u, h, m, c, d) {
                 super(e, t, r, i, s, n, l, a, o, u, h), this.ident = F.e.StiMeterIdent.BubbleColumn, this.allowCustomColors = !1, this.positiveColor = vr.get("537eb6"), this.negativeColor = vr.get("ff0000"), this.horAlignment = z.Center, null != m && (this.allowCustomColors = m), null != c && (this.positiveColor = c), null != d && (this.negativeColor = d)
             }
         }
-        F.K.StiBubbleColumn = Gi
+        F.K.StiBubbleColumn = Xi
     }
     let ni = L.System.Globalization.CultureInfo,
         li = (F.h.StiCultureHelper = class {
             static set(e) {
                 let t = null == e ? void 0 : e.getParsedCulture();
                 if (B.isNullOrWhiteSpace(t)) return null;
                 let r = ni.currentCulture;
@@ -1674,56 +1674,57 @@
                 } catch (e) {}
                 return r
             }
             static restore(e) {
                 if (null == e) return;
                 ni.currentCulture = e
             }
-        }, L.Data.Functions.StiExtValueConverter),
-        ai = F.h.StiCultureHelper,
-        oi = L.Report.Dictionary.StiDataColumn,
-        ui = L.Data.Helpers.StiMoneyNameHelper;
+        }, F.a.StiTextFormatState),
+        ai = L.Data.Functions.StiExtValueConverter,
+        oi = F.h.StiCultureHelper,
+        ui = L.Report.Dictionary.StiDataColumn,
+        hi = L.Data.Helpers.StiMoneyNameHelper;
     {
-        class ts {
+        class rs {
             static get defaultGeneralFormat() {
                 return null == this._defaultGeneralFormat && (this._defaultGeneralFormat = new Jt), this._defaultGeneralFormat
             }
             static get defaultCurrencyFormat() {
                 return null == this._defaultCurrencyFormat && (this._defaultCurrencyFormat = new Jr), this._defaultCurrencyFormat
             }
             static get defaultPercentageFormat() {
-                return null == this._defaultPercentageFormat && (this._defaultPercentageFormat = new Ur(1, 1, null, null, 0, null, 100, null, null, null, null, L.Report.Components.StiTextFormatState.DecimalDigits | L.Report.Components.StiTextFormatState.GroupSize | L.Report.Components.StiTextFormatState.PositivePattern | L.Report.Components.StiTextFormatState.NegativePattern)), this._defaultPercentageFormat
+                return null == this._defaultPercentageFormat && (this._defaultPercentageFormat = new Ur, this._defaultPercentageFormat.positivePattern = 1, this._defaultPercentageFormat.negativePattern = 1, this._defaultPercentageFormat.decimalDigits = 0, this._defaultPercentageFormat.groupSize = 100, this._defaultPercentageFormat.state = li.DecimalDigits | li.GroupSize | li.PositivePattern | li.NegativePattern), this._defaultPercentageFormat
             }
             static get defaultNumberFormat() {
                 return null == this._defaultNumberFormat && (this._defaultNumberFormat = new Wr), this._defaultNumberFormat
             }
             static get defaultIntegerFormat() {
-                return null == this._defaultIntegerFormat && (this._defaultIntegerFormat = new Wr(null, null, null, 0, null, null, !1, !1)), this._defaultIntegerFormat
+                return null == this._defaultIntegerFormat && (this._defaultIntegerFormat = new Wr, this._defaultIntegerFormat.decimalDigits = 0, this._defaultIntegerFormat.useGroupSeparator = !1, this._defaultIntegerFormat.useLocalSetting = !1), this._defaultIntegerFormat
             }
             static get defaultDateFormat() {
                 return null == this._defaultDateFormat && (this._defaultDateFormat = new Xr), this._defaultDateFormat
             }
             static get defaultBooleanFormat() {
                 return null == this._defaultBooleanFormat && (this._defaultBooleanFormat = new Zr), this._defaultBooleanFormat
             }
             static formatBasedOnColumnType(e, t, r) {
                 let i = t.cache[r];
-                return null == i && (i = ts.formatBasedOnColumnType2(e, t.textFormat, t, r), t.cache[r] = i), i
+                return null == i && (i = rs.formatBasedOnColumnType2(e, t.textFormat, t, r), t.cache[r] = i), i
             }
             static formatBasedOnColumnType2(t, r, i, s) {
                 var n;
-                this.storedCulture = ai.set(t.report);
+                this.storedCulture = oi.set(t.report);
                 try {
                     if (null == s) return "";
                     if (null == i) return s.toString();
                     let e = null == (n = null == t ? void 0 : t.report) ? void 0 : n.getParsedCulture();
-                    if (li.isEligable(s, e)) return li.convert(s, e);
+                    if (ai.isEligable(s, e)) return ai.convert(s, e);
                     if (null != s && (null == r || r instanceof Jt)) {
                         let e = typeof s;
-                        if ("number" == e && ui.isMoneyName(i.label)) return this.defaultCurrencyFormat.format(s);
+                        if ("number" == e && hi.isMoneyName(i.label)) return this.defaultCurrencyFormat.format(s);
                         if ("number" == e) return this.defaultNumberFormat.format(s);
                         if ("boolean" == e) return this.defaultBooleanFormat.format(s);
                         if ("object" == e) {
                             let e = Le.getType(s);
                             if (Le.isDateType(e)) return this.defaultDateFormat.format(s)
                         }
                     }
@@ -1731,72 +1732,72 @@
                 } catch (e) {
                     return s.toString()
                 } finally {
                     F.h.StiCultureHelper.restore(this.storedCulture)
                 }
             }
             static format(e, t, r) {
-                this.storedCulture = ai.set(e);
+                this.storedCulture = oi.set(e);
                 try {
                     if (null == r) return "";
                     return null != t ? t.format(r) : r.toString()
                 } catch (e) {
                     return r.toString()
                 } finally {
                     F.h.StiCultureHelper.restore(this.storedCulture)
                 }
             }
             static formatAsPercentage(e, t) {
-                this.storedCulture = ai.set(e);
+                this.storedCulture = oi.set(e);
                 try {
                     if (null == t) return "";
                     return this.defaultPercentageFormat.format(t)
                 } catch (e) {
                     return t.toString()
                 } finally {
                     F.h.StiCultureHelper.restore(this.storedCulture)
                 }
             }
             static formatAsPercentage2(e, t, r) {
-                this.storedCulture = ai.set(e);
+                this.storedCulture = oi.set(e);
                 try {
                     if (null == r) return "";
                     if (null == t || t.is(Jt)) return this.defaultPercentageFormat.format(r);
                     return t.format(r)
                 } catch (e) {
                     return r.toString()
                 } finally {
                     F.h.StiCultureHelper.restore(this.storedCulture)
                 }
             }
             static getDefaultFormatForColumn(e) {
                 let t = F.h.StiMeterHelper.toDataType(e);
                 if (null == t) return this.defaultGeneralFormat;
                 if (Le.isNumericType(t)) {
-                    if (ui.isMoneyName(e.as(oi).nameInSource)) return this.defaultCurrencyFormat;
+                    if (hi.isMoneyName(e.as(ui).nameInSource)) return this.defaultCurrencyFormat;
                     if (Le.isIntegerType(t)) return this.defaultIntegerFormat;
                     return this.defaultNumberFormat
                 }
                 if (Le.isDateType(t)) return this.defaultDateFormat;
                 if (t == Boolean) return this.defaultBooleanFormat;
                 return this.defaultGeneralFormat
             }
         }
-        F.h.StiTextFormatHelper = ts
+        F.h.StiTextFormatHelper = rs
     }
-    let hi = L.Report.Dashboard.StiTableColumnSize,
-        mi = L.Report.Dashboard.IStiTableColumnSize,
-        ci = L.Base.Meters.IStiDimensionColumn;
+    let mi = L.Report.Dashboard.StiTableColumnSize,
+        ci = L.Report.Dashboard.IStiTableColumnSize,
+        di = L.Base.Meters.IStiDimensionColumn;
     {
-        class rs extends F.K.StiTableColumn {
+        class is extends F.K.StiTableColumn {
             implements() {
-                return rs.ImplementsStiDimensionColumn || (rs.ImplementsStiDimensionColumn = super.implements().concat([ze, ci, mi])), rs.ImplementsStiDimensionColumn
+                return is.ImplementsStiDimensionColumn || (is.ImplementsStiDimensionColumn = super.implements().concat([ze, di, ci])), is.ImplementsStiDimensionColumn
             }
             meta() {
-                return [...super.meta(), new h("ShowHyperlink"), new n("HyperlinkPattern"), new s("Size").check(() => null != this.size).set(e => this.size = hi.createFromJsonObject(e.value)).setXml(e => this.size = hi.createFromXml(e))]
+                return [...super.meta(), new h("ShowHyperlink"), new n("HyperlinkPattern"), new s("Size").check(() => null != this.size).set(e => this.size = mi.createFromJsonObject(e.value)).setXml(e => this.size = mi.createFromXml(e))]
             }
             clone() {
                 var e;
                 let t = super.clone();
                 return t.size = null == (e = this.size) ? void 0 : e.clone(), t
             }
             get localizedName() {
@@ -1807,244 +1808,244 @@
                 null != (e = this.size) && e.checkRules()
             }
             getUniqueCode() {
                 let e = super.getUniqueCode();
                 return e = 397 * (e = 397 * (e = 397 * e ^ this.showHyperlink[L.System.StiObject.stimulsoft]().getHashCode()) ^ this.hyperlinkPattern[L.System.StiObject.stimulsoft]().getHashCode()) ^ this.size[L.System.StiObject.stimulsoft]().getHashCode(), Math.abs(e)
             }
             constructor(e, t, r, i, s, n, l, a, o, u, h, m, c, d, g) {
-                super(e, t, r, i, s, n, l, o, m, c, d), this.ident = F.e.StiMeterIdent.DimensionColumn, this.showHyperlink = !1, this.hyperlinkPattern = "", this.size = new hi, null != u && (this.showHyperlink = u), null != h && (this.hyperlinkPattern = h), null != g && (this.size = g)
+                super(e, t, r, i, s, n, l, o, m, c, d), this.ident = F.e.StiMeterIdent.DimensionColumn, this.showHyperlink = !1, this.hyperlinkPattern = "", this.size = new mi, null != u && (this.showHyperlink = u), null != h && (this.hyperlinkPattern = h), null != g && (this.size = g)
             }
         }
-        F.K.StiDimensionColumn = rs
+        F.K.StiDimensionColumn = is
     }
-    let di = L.Base.Meters.IStiColorMapMeter;
+    let gi = L.Base.Meters.IStiColorMapMeter;
     {
-        class ss extends F.e.StiDimensionMeter {
+        class ns extends F.e.StiDimensionMeter {
             implements() {
-                return ss.ImplementsStiColorMapMeter || (ss.ImplementsStiColorMapMeter = super.implements().concat([di])), ss.ImplementsStiColorMapMeter
+                return ns.ImplementsStiColorMapMeter || (ns.ImplementsStiColorMapMeter = super.implements().concat([gi])), ns.ImplementsStiColorMapMeter
             }
             get localizedName() {
                 return b.get("PropertyMain", "Color")
             }
             constructor(e, t, r) {
                 super(e, t, r), this.ident = F.e.StiMeterIdent.ColorMapMeter
             }
         }
-        F.L.StiColorMapMeter = ss
+        F.L.StiColorMapMeter = ns
     }
-    let gi = L.Base.Meters.IStiValueMapMeter;
+    let pi = L.Base.Meters.IStiValueMapMeter;
     {
-        class ns extends F.e.StiMeasureMeter {
+        class ls extends F.e.StiMeasureMeter {
             implements() {
-                return ns.ImplementsStiValueMapMeter || (ns.ImplementsStiValueMapMeter = super.implements().concat([gi])), ns.ImplementsStiValueMapMeter
+                return ls.ImplementsStiValueMapMeter || (ls.ImplementsStiValueMapMeter = super.implements().concat([pi])), ls.ImplementsStiValueMapMeter
             }
             get localizedName() {
                 return b.get("PropertyMain", "Value")
             }
             constructor(e, t, r) {
                 super(e, t, r), this.ident = F.e.StiMeterIdent.ValueMapMeter
             }
         }
-        F.L.StiValueMapMeter = ns
+        F.L.StiValueMapMeter = ls
     }
-    let pi = L.Base.Meters.IStiGroupMapMeter;
+    let Si = L.Base.Meters.IStiGroupMapMeter;
     {
-        class ls extends F.e.StiDimensionMeter {
+        class as extends F.e.StiDimensionMeter {
             implements() {
-                return ls.ImplementsStiGroupMapMeter || (ls.ImplementsStiGroupMapMeter = super.implements().concat([pi])), ls.ImplementsStiGroupMapMeter
+                return as.ImplementsStiGroupMapMeter || (as.ImplementsStiGroupMapMeter = super.implements().concat([Si])), as.ImplementsStiGroupMapMeter
             }
             get localizedName() {
                 return b.get("PropertyMain", "Group")
             }
             constructor(e, t, r) {
                 super(e, t, r), this.ident = F.e.StiMeterIdent.GroupMapMeter
             }
         }
-        F.L.StiGroupMapMeter = ls
+        F.L.StiGroupMapMeter = as
     }
-    let Si = L.Base.Meters.IStiNameMapMeter;
+    let wi = L.Base.Meters.IStiNameMapMeter;
     {
-        class as extends F.e.StiDimensionMeter {
+        class os extends F.e.StiDimensionMeter {
             implements() {
-                return as.ImplementsStiNameMapMeter || (as.ImplementsStiNameMapMeter = super.implements().concat([Si])), as.ImplementsStiNameMapMeter
+                return os.ImplementsStiNameMapMeter || (os.ImplementsStiNameMapMeter = super.implements().concat([wi])), os.ImplementsStiNameMapMeter
             }
             get localizedName() {
                 return b.get("PropertyMain", "Name")
             }
             constructor(e, t, r) {
                 super(e, t, r), this.ident = F.e.StiMeterIdent.NameMapMeter
             }
         }
-        F.L.StiNameMapMeter = as
+        F.L.StiNameMapMeter = os
     }
-    let wi = L.Base.Meters.IStiKeyMapMeter;
+    let bi = L.Base.Meters.IStiKeyMapMeter;
     {
-        class os extends F.e.StiDimensionMeter {
+        class us extends F.e.StiDimensionMeter {
             implements() {
-                return os.ImplementsStiKeyMapMeter || (os.ImplementsStiKeyMapMeter = super.implements().concat([wi])), os.ImplementsStiKeyMapMeter
+                return us.ImplementsStiKeyMapMeter || (us.ImplementsStiKeyMapMeter = super.implements().concat([bi])), us.ImplementsStiKeyMapMeter
             }
             get localizedName() {
                 return b.get("PropertyMain", "Key")
             }
             constructor(e, t, r) {
                 super(e, t, r), this.ident = F.e.StiMeterIdent.KeyMapMeter
             }
         }
-        F.L.StiKeyMapMeter = os
+        F.L.StiKeyMapMeter = us
     } {
-        class us extends F.e.StiMeasureMeter {
+        class hs extends F.e.StiMeasureMeter {
             implements() {
-                return us.ImplementsStiValueProgressMeter || (us.ImplementsStiValueProgressMeter = super.implements().concat([Er])), us.ImplementsStiValueProgressMeter
+                return hs.ImplementsStiValueProgressMeter || (hs.ImplementsStiValueProgressMeter = super.implements().concat([Er])), hs.ImplementsStiValueProgressMeter
             }
             get localizedName() {
                 return b.get("PropertyMain", "Value")
             }
             constructor(e, t, r) {
                 super(e, t, r), this.ident = F.e.StiMeterIdent.ValueProgressMeter
             }
         }
-        F.M.StiValueProgressMeter = us
+        F.M.StiValueProgressMeter = hs
     } {
-        class hs extends F.e.StiMeasureMeter {
+        class ms extends F.e.StiMeasureMeter {
             implements() {
-                return hs.ImplementsStiValueProgressMeter || (hs.ImplementsStiValueProgressMeter = super.implements().concat([Er])), hs.ImplementsStiValueProgressMeter
+                return ms.ImplementsStiValueProgressMeter || (ms.ImplementsStiValueProgressMeter = super.implements().concat([Er])), ms.ImplementsStiValueProgressMeter
             }
             get localizedName() {
                 return b.get("PropertyMain", "Target")
             }
             constructor(e, t, r) {
                 super(e, t, r), this.ident = F.e.StiMeterIdent.TargetProgressMeter
             }
         }
-        F.M.StiTargetProgressMeter = hs
+        F.M.StiTargetProgressMeter = ms
     } {
-        class ms extends F.e.StiDimensionMeter {
+        class cs extends F.e.StiDimensionMeter {
             implements() {
-                return ms.ImplementsStiSeriesProgressMeter || (ms.ImplementsStiSeriesProgressMeter = super.implements().concat([Er])), ms.ImplementsStiSeriesProgressMeter
+                return cs.ImplementsStiSeriesProgressMeter || (cs.ImplementsStiSeriesProgressMeter = super.implements().concat([Er])), cs.ImplementsStiSeriesProgressMeter
             }
             get localizedName() {
                 return b.get("PropertyMain", "Series")
             }
             constructor(e, t, r) {
                 super(e, t, r), this.ident = F.e.StiMeterIdent.SeriesProgressMeter
             }
         }
-        F.M.StiSeriesProgressMeter = ms
+        F.M.StiSeriesProgressMeter = cs
     }
-    let bi = L.Report.Dashboard.ImplementsIStiPivotItem,
-        fi = L.Report.Dashboard.IStiPivotItem,
-        yi = L.Report.CrossTab.Core.StiSortDirection,
-        Ci = L.Report.Dashboard.IStiMeterRules,
-        xi = L.Report.Dashboard.ImplementsIStiTableColumnSize,
-        Mi = L.Base.Meters.IStiPivotColumn,
-        Ti = L.Data.Engine.IStiDataTopN,
-        Fi = L.Data.Engine.StiDataTopN;
+    let fi = L.Report.Dashboard.ImplementsIStiPivotItem,
+        yi = L.Report.Dashboard.IStiPivotItem,
+        Ci = L.Report.CrossTab.Core.StiSortDirection,
+        xi = L.Report.Dashboard.IStiMeterRules,
+        Mi = L.Report.Dashboard.ImplementsIStiTableColumnSize,
+        Ti = L.Base.Meters.IStiPivotColumn,
+        Fi = L.Data.Engine.IStiDataTopN,
+        vi = L.Data.Engine.StiDataTopN;
     {
-        class cs extends F.e.StiMeter {
+        class ds extends F.e.StiMeter {
             implements() {
-                return cs.ImplementsStiPivotColumn || (cs.ImplementsStiPivotColumn = super.implements().concat([ze, Cr, yr, mi, Mi, fi, Ti, Ci, ...wr, ...$r, ...xi, ...bi, l])), cs.ImplementsStiPivotColumn
+                return ds.ImplementsStiPivotColumn || (ds.ImplementsStiPivotColumn = super.implements().concat([ze, Cr, yr, ci, Ti, yi, Fi, xi, ...wr, ...$r, ...Mi, ...fi, l])), ds.ImplementsStiPivotColumn
             }
             clone() {
                 var e;
                 let t = super.clone();
                 return t.textFormat = this.textFormat.clone(), t.topN = this.topN.clone(), t.size = null == (e = this.size) ? void 0 : e.clone(), t.horAlignment = this.horAlignment, t.showTotal = this.showTotal, t.totalLabel = this.totalLabel, t.sortDirection = this.sortDirection, t.expandExpression = this.expandExpression, t.visibility = this.visibility, t.visibilityExpression = this.visibilityExpression, t
             }
             meta() {
-                return [...super.meta(), new i("HorAlignment", "", z, z.Center), new h("ShowTotal", "", !0), new n("TotalLabel"), new s("TextFormat").check(() => !(this.textFormat.is(Jt) || null == this.textFormat)).set(e => this.textFormat = br.createFromJsonObject(e.value)).setXml(e => this.textFormat = br.loadFormatFromXml(e)), new s("TopN").check(() => null != this.topN).set(e => this.topN = Fi.createFromJsonObject(e.value)).setXml(e => this.topN = Fi.createFromXml(e)), new s("Size").check(() => null != this.size).set(e => this.size = hi.createFromJsonObject(e.value)).setXml(e => this.size = hi.createFromXml(e)), new i("SortDirection", "", yi, yi.Asc), new n("ExpandExpression"), new i("Visibility", "", Hr, Hr.True), new n("VisibilityExpression").check(() => null != this.visibilityExpression)]
+                return [...super.meta(), new i("HorAlignment", "", z, z.Center), new h("ShowTotal", "", !0), new n("TotalLabel"), new s("TextFormat").check(() => !(this.textFormat.is(Jt) || null == this.textFormat)).set(e => this.textFormat = br.createFromJsonObject(e.value)).setXml(e => this.textFormat = br.loadFormatFromXml(e)), new s("TopN").check(() => null != this.topN).set(e => this.topN = vi.createFromJsonObject(e.value)).setXml(e => this.topN = vi.createFromXml(e)), new s("Size").check(() => null != this.size).set(e => this.size = mi.createFromJsonObject(e.value)).setXml(e => this.size = mi.createFromXml(e)), new i("SortDirection", "", Ci, Ci.Asc), new n("ExpandExpression"), new i("Visibility", "", Hr, Hr.True), new n("VisibilityExpression").check(() => null != this.visibilityExpression)]
             }
             checkRules() {
                 var e;
                 null != (e = this.size) && e.checkRules()
             }
             get strSortDirection() {
-                return `` + ve.getName(yi, this.sortDirection) + (this.sortDirection != yi.None ? "ending" : "")
+                return `` + ve.getName(Ci, this.sortDirection) + (this.sortDirection != Ci.None ? "ending" : "")
             }
             set strSortDirection(e) {
-                this.sortDirection = ve.parse(yi, e.replace("ending", ""))
+                this.sortDirection = ve.parse(Ci, e.replace("ending", ""))
             }
             getUniqueCode() {
                 let e = super.getUniqueCode();
                 return e = 397 * (e = 397 * (e = 397 * (e = 397 * (e = 397 * (e = 397 * (e = 397 * (e = 397 * (e = 397 * (e = 397 * e ^ this.horAlignment) ^ this.sortDirection) ^ (null != this.textFormat ? this.textFormat[L.System.StiObject.stimulsoft]().getHashCode() : 0)) ^ (null != this.topN ? this.topN[L.System.StiObject.stimulsoft]().getHashCode() : 0)) ^ (null != this.size ? this.size[L.System.StiObject.stimulsoft]().getHashCode() : 0)) ^ (null != this.showTotal ? this.showTotal[L.System.StiObject.stimulsoft]().getHashCode() : 0)) ^ (null != this.totalLabel ? this.totalLabel[L.System.StiObject.stimulsoft]().getHashCode() : 0)) ^ (null != this.expandExpression ? this.expandExpression[L.System.StiObject.stimulsoft]().getHashCode() : 0)) ^ (null != this.visibility ? this.visibility[L.System.StiObject.stimulsoft]().getHashCode() : 0)) ^ (null != this.visibilityExpression ? this.visibilityExpression[L.System.StiObject.stimulsoft]().getHashCode() : 0), Math.abs(e)
             }
             get localizedName() {
                 return b.get("Components", "StiPivotColumn")
             }
             constructor(e, t, r, i, s, n, l, a, o, u, h, m, c) {
-                super(e, t, r), this.horAlignment = z.Center, this.showTotal = !0, this.totalLabel = "", this.textFormat = new Jt, this.size = new hi, this.visibility = Hr.True, this.visibilityExpression = "", this.expandExpression = "", this.topN = new Fi, this.sortDirection = yi.Asc, this.ident = F.e.StiMeterIdent.PivotColumn, null != i && (this.horAlignment = i), null != s && (this.textFormat = s), null != n && (this.topN = n), null != o && (this.size = o), null != l && (this.showTotal = l), null != a && (this.totalLabel = a), null != u && (this.sortDirection = u), null != h && (this.expandExpression = h), null != m && (this.visibility = m), null != c && (this.visibilityExpression = c)
+                super(e, t, r), this.horAlignment = z.Center, this.showTotal = !0, this.totalLabel = "", this.textFormat = new Jt, this.size = new mi, this.visibility = Hr.True, this.visibilityExpression = "", this.expandExpression = "", this.topN = new vi, this.sortDirection = Ci.Asc, this.ident = F.e.StiMeterIdent.PivotColumn, null != i && (this.horAlignment = i), null != s && (this.textFormat = s), null != n && (this.topN = n), null != o && (this.size = o), null != l && (this.showTotal = l), null != a && (this.totalLabel = a), null != u && (this.sortDirection = u), null != h && (this.expandExpression = h), null != m && (this.visibility = m), null != c && (this.visibilityExpression = c)
             }
         }
-        F.N.StiPivotColumn = cs
+        F.N.StiPivotColumn = ds
     }
-    let vi = L.Base.Meters.IStiPivotRow;
+    let Ai = L.Base.Meters.IStiPivotRow;
     {
-        class ds extends F.e.StiMeter {
+        class gs extends F.e.StiMeter {
             implements() {
-                return ds.ImplementsStiPivotRow || (ds.ImplementsStiPivotRow = super.implements().concat([ze, Cr, yr, mi, vi, fi, Ti, Ci, ...wr, ...$r, ...xi, ...bi, l])), ds.ImplementsStiPivotRow
+                return gs.ImplementsStiPivotRow || (gs.ImplementsStiPivotRow = super.implements().concat([ze, Cr, yr, ci, Ai, yi, Fi, xi, ...wr, ...$r, ...Mi, ...fi, l])), gs.ImplementsStiPivotRow
             }
             clone() {
                 var e;
                 let t = super.clone();
                 return t.textFormat = this.textFormat.clone(), t.topN = this.topN.clone(), t.size = null == (e = this.size) ? void 0 : e.clone(), t.horAlignment = this.horAlignment, t.showTotal = this.showTotal, t.totalLabel = this.totalLabel, t.sortDirection = this.sortDirection, t.expandExpression = this.expandExpression, t.visibility = this.visibility, t.visibilityExpression = this.visibilityExpression, t
             }
             meta() {
-                return [...super.meta(), new i("HorAlignment", "", z, z.Center), new h("ShowTotal", "", !0), new n("TotalLabel"), new s("TextFormat").check(() => !(this.textFormat.is(Jt) || null == this.textFormat)).set(e => this.textFormat = br.createFromJsonObject(e.value)).setXml(e => this.textFormat = br.loadFormatFromXml(e)), new s("TopN").check(() => null != this.topN).set(e => this.topN = Fi.createFromJsonObject(e.value)).setXml(e => this.topN = Fi.createFromXml(e)), new s("Size").check(() => null != this.size).set(e => this.size = hi.createFromJsonObject(e.value)).setXml(e => this.size = hi.createFromXml(e)), new i("SortDirection", "", yi, yi.Asc), new n("ExpandExpression"), new i("Visibility", "", Hr, Hr.True), new n("VisibilityExpression").check(() => null != this.visibilityExpression)]
+                return [...super.meta(), new i("HorAlignment", "", z, z.Center), new h("ShowTotal", "", !0), new n("TotalLabel"), new s("TextFormat").check(() => !(this.textFormat.is(Jt) || null == this.textFormat)).set(e => this.textFormat = br.createFromJsonObject(e.value)).setXml(e => this.textFormat = br.loadFormatFromXml(e)), new s("TopN").check(() => null != this.topN).set(e => this.topN = vi.createFromJsonObject(e.value)).setXml(e => this.topN = vi.createFromXml(e)), new s("Size").check(() => null != this.size).set(e => this.size = mi.createFromJsonObject(e.value)).setXml(e => this.size = mi.createFromXml(e)), new i("SortDirection", "", Ci, Ci.Asc), new n("ExpandExpression"), new i("Visibility", "", Hr, Hr.True), new n("VisibilityExpression").check(() => null != this.visibilityExpression)]
             }
             checkRules() {
                 var e;
                 null != (e = this.size) && e.checkRules()
             }
             get strSortDirection() {
-                return `` + ve.getName(yi, this.sortDirection) + (this.sortDirection != yi.None ? "ending" : "")
+                return `` + ve.getName(Ci, this.sortDirection) + (this.sortDirection != Ci.None ? "ending" : "")
             }
             set strSortDirection(e) {
-                this.sortDirection = ve.parse(yi, e.replace("ending", ""))
+                this.sortDirection = ve.parse(Ci, e.replace("ending", ""))
             }
             getUniqueCode() {
                 let e = super.getUniqueCode();
                 return e = 397 * (e = 397 * (e = 397 * (e = 397 * (e = 397 * (e = 397 * (e = 397 * (e = 397 * (e = 397 * (e = 397 * e ^ this.horAlignment) ^ this.sortDirection) ^ (null != this.textFormat ? this.textFormat[L.System.StiObject.stimulsoft]().getHashCode() : 0)) ^ (null != this.topN ? this.topN[L.System.StiObject.stimulsoft]().getHashCode() : 0)) ^ (null != this.size ? this.size[L.System.StiObject.stimulsoft]().getHashCode() : 0)) ^ (null != this.showTotal ? this.showTotal[L.System.StiObject.stimulsoft]().getHashCode() : 0)) ^ (null != this.totalLabel ? this.totalLabel[L.System.StiObject.stimulsoft]().getHashCode() : 0)) ^ (null != this.expandExpression ? this.expandExpression[L.System.StiObject.stimulsoft]().getHashCode() : 0)) ^ (null != this.visibility ? this.visibility[L.System.StiObject.stimulsoft]().getHashCode() : 0)) ^ (null != this.visibilityExpression ? this.visibilityExpression[L.System.StiObject.stimulsoft]().getHashCode() : 0), Math.abs(e)
             }
             get localizedName() {
                 return b.get("Components", "StiPivotRow")
             }
             constructor(e, t, r, i, s, n, l, a, o, u, h, m, c) {
-                super(e, t, r), this.horAlignment = z.Center, this.showTotal = !0, this.totalLabel = "", this.textFormat = new Jt, this.size = new hi, this.visibility = Hr.True, this.visibilityExpression = "", this.expandExpression = "", this.topN = new Fi, this.sortDirection = yi.Asc, this.ident = F.e.StiMeterIdent.PivotRow, null != i && (this.horAlignment = i), null != s && (this.textFormat = s), null != n && (this.topN = n), null != o && (this.size = o), null != l && (this.showTotal = l), null != a && (this.totalLabel = a), null != u && (this.sortDirection = u), null != h && (this.expandExpression = h), null != m && (this.visibility = m), null != c && (this.visibilityExpression = c)
+                super(e, t, r), this.horAlignment = z.Center, this.showTotal = !0, this.totalLabel = "", this.textFormat = new Jt, this.size = new mi, this.visibility = Hr.True, this.visibilityExpression = "", this.expandExpression = "", this.topN = new vi, this.sortDirection = Ci.Asc, this.ident = F.e.StiMeterIdent.PivotRow, null != i && (this.horAlignment = i), null != s && (this.textFormat = s), null != n && (this.topN = n), null != o && (this.size = o), null != l && (this.showTotal = l), null != a && (this.totalLabel = a), null != u && (this.sortDirection = u), null != h && (this.expandExpression = h), null != m && (this.visibility = m), null != c && (this.visibilityExpression = c)
             }
         }
-        F.N.StiPivotRow = ds
+        F.N.StiPivotRow = gs
     }
-    let Ai = L.Base.Meters.IStiPivotSummary;
+    let Ii = L.Base.Meters.IStiPivotSummary;
     {
-        class gs extends F.e.StiMeasureMeter {
+        class ps extends F.e.StiMeasureMeter {
             implements() {
-                return gs.ImplementsStiPivotSummary || (gs.ImplementsStiPivotSummary = super.implements().concat([Cr, yr, mi, Ai, fi, Ci, ...wr, ...$r, ...xi, ...bi, l])), gs.ImplementsStiPivotSummary
+                return ps.ImplementsStiPivotSummary || (ps.ImplementsStiPivotSummary = super.implements().concat([Cr, yr, ci, Ii, yi, xi, ...wr, ...$r, ...Mi, ...fi, l])), ps.ImplementsStiPivotSummary
             }
             clone() {
                 var e;
                 let t = super.clone();
                 return t.textFormat = this.textFormat.clone(), t.size = null == (e = this.size) ? void 0 : e.clone(), t.hideZeros = this.hideZeros, t.horAlignment = this.horAlignment, t.visibility = this.visibility, t.visibilityExpression = this.visibilityExpression, t
             }
             meta() {
-                return [...super.meta(), new i("HorAlignment", "", z, z.Center), new s("TextFormat").check(() => !(this.textFormat.is(Jt) || null == this.textFormat)).set(e => this.textFormat = br.createFromJsonObject(e.value)).setXml(e => this.textFormat = br.loadFormatFromXml(e)), new s("Size").check(() => null != this.size).set(e => this.size = hi.createFromJsonObject(e.value)).setXml(e => this.size = hi.createFromXml(e)), new h("HideZeros", "", !0), new i("Visibility", "", Hr, Hr.True), new n("VisibilityExpression").check(() => null != this.visibilityExpression)]
+                return [...super.meta(), new i("HorAlignment", "", z, z.Center), new s("TextFormat").check(() => !(this.textFormat.is(Jt) || null == this.textFormat)).set(e => this.textFormat = br.createFromJsonObject(e.value)).setXml(e => this.textFormat = br.loadFormatFromXml(e)), new s("Size").check(() => null != this.size).set(e => this.size = mi.createFromJsonObject(e.value)).setXml(e => this.size = mi.createFromXml(e)), new h("HideZeros", "", !0), new i("Visibility", "", Hr, Hr.True), new n("VisibilityExpression").check(() => null != this.visibilityExpression)]
             }
             checkRules() {
                 var e;
                 null != (e = this.size) && e.checkRules()
             }
             getUniqueCode() {
                 let e = super.getUniqueCode();
                 return e = 397 * (e = 397 * (e = 397 * (e = 397 * (e = 397 * (e = 397 * e ^ this.horAlignment) ^ (null != this.textFormat ? this.textFormat[L.System.StiObject.stimulsoft]().getHashCode() : 0)) ^ (null != this.size ? this.size[L.System.StiObject.stimulsoft]().getHashCode() : 0)) ^ (null != this.hideZeros ? this.hideZeros[L.System.StiObject.stimulsoft]().getHashCode() : 0)) ^ (null != this.visibility ? this.visibility[L.System.StiObject.stimulsoft]().getHashCode() : 0)) ^ (null != this.visibilityExpression ? this.visibilityExpression[L.System.StiObject.stimulsoft]().getHashCode() : 0), Math.abs(e)
             }
             get localizedName() {
                 return b.get("Components", "StiPivotSummary")
             }
             constructor(e, t, r, i, s, n, l, a, o) {
-                super(e, t, r), this.horAlignment = z.Center, this.textFormat = new Jt, this.size = new hi, this.visibility = Hr.True, this.visibilityExpression = "", this.hideZeros = !0, this.ident = F.e.StiMeterIdent.PivotSummary, null != i && (this.horAlignment = i), null != s && (this.textFormat = s), null != n && (this.size = n), null != l && (this.hideZeros = l), null != a && (this.visibility = a), null != o && (this.visibilityExpression = o)
+                super(e, t, r), this.horAlignment = z.Center, this.textFormat = new Jt, this.size = new mi, this.visibility = Hr.True, this.visibilityExpression = "", this.hideZeros = !0, this.ident = F.e.StiMeterIdent.PivotSummary, null != i && (this.horAlignment = i), null != s && (this.textFormat = s), null != n && (this.size = n), null != l && (this.hideZeros = l), null != a && (this.visibility = a), null != o && (this.visibilityExpression = o)
             }
         }
-        F.N.StiPivotSummary = gs
+        F.N.StiPivotSummary = ps
     }
     F.O.StiLatitudeMapMeter = class extends F.e.StiDimensionMeter {
         get localizedName() {
             return b.get("PropertyMain", "Latitude")
         }
         constructor(e, t, r) {
             super(e, t, r), this.ident = F.e.StiMeterIdent.LatitudeMapMeter
@@ -2054,214 +2055,214 @@
             return b.get("PropertyMain", "Longitude")
         }
         constructor(e, t, r) {
             super(e, t, r), this.ident = F.e.StiMeterIdent.LongitudeMapMeter
         }
     };
     {
-        class ws extends F.e.StiDimensionMeter {
+        class bs extends F.e.StiDimensionMeter {
             implements() {
-                return ws.ImplementsStiKeyListBoxMeter || (ws.ImplementsStiKeyListBoxMeter = super.implements().concat([Er])), ws.ImplementsStiKeyListBoxMeter
+                return bs.ImplementsStiKeyListBoxMeter || (bs.ImplementsStiKeyListBoxMeter = super.implements().concat([Er])), bs.ImplementsStiKeyListBoxMeter
             }
             get localizedName() {
                 return b.get("PropertyMain", "Key")
             }
             constructor(e, t, r) {
                 super(e, t, r), this.ident = F.e.StiMeterIdent.KeyListBoxMeter
             }
         }
-        F.P.StiKeyListBoxMeter = ws
+        F.P.StiKeyListBoxMeter = bs
     } {
-        class bs extends F.e.StiDimensionMeter {
+        class fs extends F.e.StiDimensionMeter {
             implements() {
-                return bs.ImplementsStiNameListBoxMeter || (bs.ImplementsStiNameListBoxMeter = super.implements().concat([Rr])), bs.ImplementsStiNameListBoxMeter
+                return fs.ImplementsStiNameListBoxMeter || (fs.ImplementsStiNameListBoxMeter = super.implements().concat([Rr])), fs.ImplementsStiNameListBoxMeter
             }
             get localizedName() {
                 return b.get("PropertyMain", "Name")
             }
             constructor(e, t, r) {
                 super(e, t, r), this.ident = F.e.StiMeterIdent.NameListBoxMeter
             }
         }
-        F.P.StiNameListBoxMeter = bs
+        F.P.StiNameListBoxMeter = fs
     } {
-        class fs extends F.e.StiDimensionMeter {
+        class ys extends F.e.StiDimensionMeter {
             implements() {
-                return fs.ImplementsStiValueDatePickerMeter || (fs.ImplementsStiValueDatePickerMeter = super.implements().concat([Er])), fs.ImplementsStiValueDatePickerMeter
+                return ys.ImplementsStiValueDatePickerMeter || (ys.ImplementsStiValueDatePickerMeter = super.implements().concat([Er])), ys.ImplementsStiValueDatePickerMeter
             }
             get localizedName() {
                 return b.get("PropertyMain", "Value")
             }
             constructor(e, t, r) {
                 super(e, t, r), this.ident = F.e.StiMeterIdent.ValueDatePickerMeter
             }
         }
-        F.Q.StiValueDatePickerMeter = fs
+        F.Q.StiValueDatePickerMeter = ys
     } {
-        class Oi extends F.e.StiDimensionMeter {
+        class Vi extends F.e.StiDimensionMeter {
             implements() {
-                return Oi.ImplementsStiValueNumberBoxMeter || (Oi.ImplementsStiValueNumberBoxMeter = super.implements().concat([Er])), Oi.ImplementsStiValueNumberBoxMeter
+                return Vi.ImplementsStiValueNumberBoxMeter || (Vi.ImplementsStiValueNumberBoxMeter = super.implements().concat([Er])), Vi.ImplementsStiValueNumberBoxMeter
             }
             get localizedName() {
                 return b.get("PropertyMain", "Value")
             }
             constructor(e, t, r) {
                 super(e, t, r), this.ident = F.e.StiMeterIdent.ValueNumberBoxMeter
             }
         }
-        F.R.StiValueNumberBoxMeter = Oi
+        F.R.StiValueNumberBoxMeter = Vi
     }
     F.H.StiEndValueChartMeter = class extends F.e.StiMeasureMeter {
         get localizedName() {
             return b.get("PropertyMain", "ValueEnd")
         }
         constructor(e, t, r) {
             super(e, t, r), this.ident = F.e.StiMeterIdent.EndValueChartMeter
         }
     };
     {
-        class xs extends F.e.StiDimensionMeter {
+        class Ms extends F.e.StiDimensionMeter {
             implements() {
-                return xs.ImplementsStiNameComboBoxMeter || (xs.ImplementsStiNameComboBoxMeter = super.implements().concat([Rr])), xs.ImplementsStiNameComboBoxMeter
+                return Ms.ImplementsStiNameComboBoxMeter || (Ms.ImplementsStiNameComboBoxMeter = super.implements().concat([Rr])), Ms.ImplementsStiNameComboBoxMeter
             }
             get localizedName() {
                 return b.get("PropertyMain", "Name")
             }
             constructor(e, t, r) {
                 super(e, t, r), this.ident = F.e.StiMeterIdent.NameComboBoxMeter
             }
         }
-        F.S.StiNameComboBoxMeter = xs
+        F.S.StiNameComboBoxMeter = Ms
     } {
-        class Ms extends F.e.StiDimensionMeter {
+        class Ts extends F.e.StiDimensionMeter {
             implements() {
-                return Ms.ImplementsStiKeyComboBoxMeter || (Ms.ImplementsStiKeyComboBoxMeter = super.implements().concat([Er])), Ms.ImplementsStiKeyComboBoxMeter
+                return Ts.ImplementsStiKeyComboBoxMeter || (Ts.ImplementsStiKeyComboBoxMeter = super.implements().concat([Er])), Ts.ImplementsStiKeyComboBoxMeter
             }
             get localizedName() {
                 return b.get("PropertyMain", "Key")
             }
             constructor(e, t, r) {
                 super(e, t, r), this.ident = F.e.StiMeterIdent.KeyComboBoxMeter
             }
         }
-        F.S.StiKeyComboBoxMeter = Ms
+        F.S.StiKeyComboBoxMeter = Ts
     }
-    let Ii = L.Base.Meters.IStiSeriesMeter;
+    let Di = L.Base.Meters.IStiSeriesMeter;
     {
-        class Ts extends F.e.StiDimensionMeter {
+        class Fs extends F.e.StiDimensionMeter {
             implements() {
-                return Ts.ImplementsStiSeriesGaugeMeter || (Ts.ImplementsStiSeriesGaugeMeter = super.implements().concat([Ii])), Ts.ImplementsStiSeriesGaugeMeter
+                return Fs.ImplementsStiSeriesGaugeMeter || (Fs.ImplementsStiSeriesGaugeMeter = super.implements().concat([Di])), Fs.ImplementsStiSeriesGaugeMeter
             }
             get localizedName() {
                 return b.get("PropertyMain", "Series")
             }
             constructor(e, t, r) {
                 super(e, t, r), this.ident = F.e.StiMeterIdent.SeriesGaugeMeter
             }
         }
-        F.T.StiSeriesGaugeMeter = Ts
+        F.T.StiSeriesGaugeMeter = Fs
     } {
-        class Fs extends F.e.StiMeasureMeter {
+        class vs extends F.e.StiMeasureMeter {
             implements() {
-                return Fs.ImplementsStiValueGaugeMeter || (Fs.ImplementsStiValueGaugeMeter = super.implements().concat([Er])), Fs.ImplementsStiValueGaugeMeter
+                return vs.ImplementsStiValueGaugeMeter || (vs.ImplementsStiValueGaugeMeter = super.implements().concat([Er])), vs.ImplementsStiValueGaugeMeter
             }
             get localizedName() {
                 return b.get("PropertyMain", "Value")
             }
             constructor(e, t, r) {
                 super(e, t, r), this.ident = F.e.StiMeterIdent.ValueGaugeMeter
             }
         }
-        F.T.StiValueGaugeMeter = Fs
+        F.T.StiValueGaugeMeter = vs
     }
-    let Di = L.Base.Meters.IStiTargetMeter;
+    let Ri = L.Base.Meters.IStiTargetMeter;
     {
-        class vs extends F.e.StiMeasureMeter {
+        class As extends F.e.StiMeasureMeter {
             implements() {
-                return vs.ImplementsStiTargetGaugeMeter || (vs.ImplementsStiTargetGaugeMeter = super.implements().concat([Di])), vs.ImplementsStiTargetGaugeMeter
+                return As.ImplementsStiTargetGaugeMeter || (As.ImplementsStiTargetGaugeMeter = super.implements().concat([Ri])), As.ImplementsStiTargetGaugeMeter
             }
             get localizedName() {
                 return b.get("PropertyMain", "Target")
             }
             constructor(e, t, r) {
                 super(e, t, r), this.ident = F.e.StiMeterIdent.TargetGaugeMeter
             }
         }
-        F.T.StiTargetGaugeMeter = vs
+        F.T.StiTargetGaugeMeter = As
     } {
-        class As extends F.e.StiDimensionMeter {
+        class Is extends F.e.StiDimensionMeter {
             implements() {
-                return As.ImplementsStiSeriesIndicatorMeter || (As.ImplementsStiSeriesIndicatorMeter = super.implements().concat([Ii])), As.ImplementsStiSeriesIndicatorMeter
+                return Is.ImplementsStiSeriesIndicatorMeter || (Is.ImplementsStiSeriesIndicatorMeter = super.implements().concat([Di])), Is.ImplementsStiSeriesIndicatorMeter
             }
             get localizedName() {
                 return b.get("PropertyMain", "Series")
             }
             constructor(e, t, r) {
                 super(e, t, r), this.ident = F.e.StiMeterIdent.SeriesIndicatorMeter
             }
         }
-        F.U.StiSeriesIndicatorMeter = As
+        F.U.StiSeriesIndicatorMeter = Is
     } {
-        class Is extends F.e.StiMeasureMeter {
+        class Ds extends F.e.StiMeasureMeter {
             implements() {
-                return Is.ImplementsStiValueIndicatorMeter || (Is.ImplementsStiValueIndicatorMeter = super.implements().concat([Er])), Is.ImplementsStiValueIndicatorMeter
+                return Ds.ImplementsStiValueIndicatorMeter || (Ds.ImplementsStiValueIndicatorMeter = super.implements().concat([Er])), Ds.ImplementsStiValueIndicatorMeter
             }
             get localizedName() {
                 return b.get("PropertyMain", "Value")
             }
             constructor(e, t, r) {
                 super(e, t, r), this.ident = F.e.StiMeterIdent.ValueIndicatorMeter
             }
         }
-        F.U.StiValueIndicatorMeter = Is
+        F.U.StiValueIndicatorMeter = Ds
     } {
-        class Ds extends F.e.StiMeasureMeter {
+        class Rs extends F.e.StiMeasureMeter {
             implements() {
-                return Ds.ImplementsStiTargetIndicatorMeter || (Ds.ImplementsStiTargetIndicatorMeter = super.implements().concat([Di])), Ds.ImplementsStiTargetIndicatorMeter
+                return Rs.ImplementsStiTargetIndicatorMeter || (Rs.ImplementsStiTargetIndicatorMeter = super.implements().concat([Ri])), Rs.ImplementsStiTargetIndicatorMeter
             }
             get localizedName() {
                 return b.get("PropertyMain", "Target")
             }
             constructor(e, t, r) {
                 super(e, t, r), this.ident = F.e.StiMeterIdent.TargetIndicatorMeter
             }
         }
-        F.U.StiTargetIndicatorMeter = Ds
+        F.U.StiTargetIndicatorMeter = Rs
     }
     F.H.StiWeightChartMeter = class extends F.e.StiMeasureMeter {
         get localizedName() {
             return b.get("PropertyMain", "Weight")
         }
         constructor(e, t, r) {
             super(e, t, r), this.ident = F.e.StiMeterIdent.WeightChartMeter
         }
     };
     let c = L.Report.Dashboard.StiChartSeriesType,
-        Ri = L.Base.Drawing.StiPenStyle,
-        Ei = L.Report.Chart.StiSeriesYAxis;
+        Ei = L.Base.Drawing.StiPenStyle,
+        Oi = L.Report.Chart.StiSeriesYAxis;
     {
-        class Bs extends F.e.StiMeasureMeter {
+        class Ps extends F.e.StiMeasureMeter {
             implements() {
-                return Bs.ImplementsStiValueChartMeter || (Bs.ImplementsStiValueChartMeter = super.implements().concat([Er, l])), Bs.ImplementsStiValueChartMeter
+                return Ps.ImplementsStiValueChartMeter || (Ps.ImplementsStiValueChartMeter = super.implements().concat([Er, l])), Ps.ImplementsStiValueChartMeter
             }
             meta() {
-                return [...super.meta(), new i("SeriesType", "", c, c.ClusteredColumn), new i("YAxis", "", Ei, Ei.LeftYAxis), new i("LineStyle", "", Ri, Ri.Solid), new se("LineWidth", "", 2), new i("ShowZeros", "", Ct, Ct.Zero), new i("ShowNulls", "", Ct, Ct.Zero)]
+                return [...super.meta(), new i("SeriesType", "", c, c.ClusteredColumn), new i("YAxis", "", Oi, Oi.LeftYAxis), new i("LineStyle", "", Ei, Ei.Solid), new se("LineWidth", "", 2), new i("ShowZeros", "", Ct, Ct.Zero), new i("ShowNulls", "", Ct, Ct.Zero)]
             }
             getUniqueCode() {
                 let e = super.getUniqueCode();
                 return e = 397 * (e = 397 * (e = 397 * (e = 397 * (e = 397 * (e = 397 * e ^ this.seriesType) ^ this.yAxis) ^ this.lineStyle) ^ this.lineWidth) ^ this.showNulls) ^ this.showZeros, Math.abs(e)
             }
             get localizedName() {
                 return b.get("PropertyMain", "Value")
             }
             constructor(e, t, r, i, s, n, l, a, o) {
-                super(e, t, r), this.seriesType = c.ClusteredColumn, this.yAxis = Ei.LeftYAxis, this.lineStyle = Ri.Solid, this.lineWidth = 2, this.showZeros = Ct.Zero, this.showNulls = Ct.Zero, this.ident = F.e.StiMeterIdent.ValueChartMeter, null != i && (this.seriesType = i), null != s && (this.yAxis = s), null != n && (this.lineStyle = n), null != l && (this.lineWidth = l), null != o && (this.showNulls = o), null != a && (this.showZeros = a)
+                super(e, t, r), this.seriesType = c.ClusteredColumn, this.yAxis = Oi.LeftYAxis, this.lineStyle = Ei.Solid, this.lineWidth = 2, this.showZeros = Ct.Zero, this.showNulls = Ct.Zero, this.ident = F.e.StiMeterIdent.ValueChartMeter, null != i && (this.seriesType = i), null != s && (this.yAxis = s), null != n && (this.lineStyle = n), null != l && (this.lineWidth = l), null != o && (this.showNulls = o), null != a && (this.showZeros = a)
             }
         }
-        F.H.StiValueChartMeter = Bs
+        F.H.StiValueChartMeter = Ps
     }
     F.H.StiOpenValueChartMeter = class extends F.H.StiValueChartMeter {
         get localizedName() {
             return b.get("PropertyMain", "ValueOpen")
         }
         constructor(e, t, r, i) {
             super(e, t, r, i), this.ident = F.e.StiMeterIdent.OpenValueChartMeter, this.seriesType = c.Candlestick, null != i && (this.seriesType = i)
@@ -2285,39 +2286,39 @@
             return b.get("PropertyMain", "ValueHigh")
         }
         constructor(e, t, r) {
             super(e, t, r), this.ident = F.e.StiMeterIdent.HighValueChartMeter
         }
     };
     {
-        class Ps extends F.e.StiDimensionMeter {
+        class js extends F.e.StiDimensionMeter {
             implements() {
-                return Ps.ImplementsStiSeriesChartMeter || (Ps.ImplementsStiSeriesChartMeter = super.implements().concat([Ii])), Ps.ImplementsStiSeriesChartMeter
+                return js.ImplementsStiSeriesChartMeter || (js.ImplementsStiSeriesChartMeter = super.implements().concat([Di])), js.ImplementsStiSeriesChartMeter
             }
             get localizedName() {
                 return b.get("PropertyMain", "Series")
             }
             constructor(e, t, r) {
                 super(e, t, r), this.ident = F.e.StiMeterIdent.SeriesChartMeter
             }
         }
-        F.H.StiSeriesChartMeter = Ps
+        F.H.StiSeriesChartMeter = js
     } {
-        class ki extends F.e.StiDimensionMeter {
+        class Ni extends F.e.StiDimensionMeter {
             implements() {
-                return ki.ImplementsSortByChartMeter || (ki.ImplementsSortByChartMeter = super.implements().concat([Ii])), ki.ImplementsSortByChartMeter
+                return Ni.ImplementsSortByChartMeter || (Ni.ImplementsSortByChartMeter = super.implements().concat([Di])), Ni.ImplementsSortByChartMeter
             }
             get localizedName() {
                 return b.get("PropertyMain", "SortBy")
             }
             constructor(e, t, r) {
                 super(e, t, r), this.ident = F.e.StiMeterIdent.SortByChartMeter
             }
         }
-        F.H.StiSortByChartMeter = ki
+        F.H.StiSortByChartMeter = Ni
     }
     F.O.StiLocationMapMeter = class extends F.e.StiDimensionMeter {
         get localizedName() {
             return b.get("PropertyMain", "Location")
         }
         constructor(e, t, r) {
             super(e, t, r), this.ident = F.e.StiMeterIdent.LocationMapMeter
@@ -2341,30 +2342,30 @@
             return b.get("PropertyMain", "Argument")
         }
         constructor(e, t, r) {
             super(e, t, r), this.ident = F.e.StiMeterIdent.LocationArgumentMapMeter
         }
     };
     {
-        class Ni extends F.F.StiMeasureCardsColumn {
+        class Li extends F.F.StiMeasureCardsColumn {
             implements() {
-                return Ni.ImplementsStiIndicatorCardsColumn || (Ni.ImplementsStiIndicatorCardsColumn = super.implements().concat([ti])), Ni.ImplementsStiIndicatorCardsColumn
+                return Li.ImplementsStiIndicatorCardsColumn || (Li.ImplementsStiIndicatorCardsColumn = super.implements().concat([ti])), Li.ImplementsStiIndicatorCardsColumn
             }
             get localizedName() {
                 return b.get("Dashboard", "Dimension")
             }
             constructor(e, t, r, i, s, n, l, a, o, u, h) {
                 super(e, t, r, i, s, n, l, a, o, u, h), this.ident = F.e.StiMeterIdent.IndicatorCardsColumn
             }
         }
-        F.F.StiIndicatorCardsColumn = Ni
+        F.F.StiIndicatorCardsColumn = Li
     } {
-        class Bi extends F.F.StiMeasureCardsColumn {
+        class Pi extends F.F.StiMeasureCardsColumn {
             implements() {
-                return Bi.ImplementsStiColorScaleCardsColumn || (Bi.ImplementsStiColorScaleCardsColumn = super.implements().concat([ri, l])), Bi.ImplementsStiColorScaleCardsColumn
+                return Pi.ImplementsStiColorScaleCardsColumn || (Pi.ImplementsStiColorScaleCardsColumn = super.implements().concat([ri, l])), Pi.ImplementsStiColorScaleCardsColumn
             }
             meta() {
                 return [...super.meta(), new r("MinimumColor", "", N.red), new r("MaximumColor", "", N.green)]
             }
             getUniqueCode() {
                 let e = super.getUniqueCode();
                 return e = 397 * (e = 397 * e ^ this.minimumColor[L.System.StiObject.stimulsoft]().getHashCode()) ^ this.maximumColor[L.System.StiObject.stimulsoft]().getHashCode(), Math.abs(e)
@@ -2372,35 +2373,35 @@
             get localizedName() {
                 return b.get("Dashboard", "ColorScale")
             }
             constructor(e, t, r, i, s, n, l, a, o, u, h, m, c) {
                 super(e, t, r, i, s, n, l, a, o, u, c), this.ident = F.e.StiMeterIdent.ColorScaleCardsColumn, this.minimumColor = N.red, this.maximumColor = N.green, null != h && (this.minimumColor = h), null != m && (this.maximumColor = m)
             }
         }
-        F.F.StiColorScaleCardsColumn = Bi
+        F.F.StiColorScaleCardsColumn = Pi
     } {
-        class Pi extends F.F.StiMeasureCardsColumn {
+        class ji extends F.F.StiMeasureCardsColumn {
             implements() {
-                return Pi.ImplementsStiDataBarsCardsColumnn || (Pi.ImplementsStiDataBarsCardsColumnn = super.implements().concat([ii, l])), Pi.ImplementsStiDataBarsCardsColumnn
+                return ji.ImplementsStiDataBarsCardsColumnn || (ji.ImplementsStiDataBarsCardsColumnn = super.implements().concat([ii, l])), ji.ImplementsStiDataBarsCardsColumnn
             }
             meta() {
                 return [...super.meta(), new se("Width"), new ne("Minimum"), new ne("Maximum"), new r("PositiveColor", "", N.transparent), new r("NegativeColor", "", N.transparent), new r("OverlappedColor", "", N.transparent), new r("FillColor", "", N.transparent)]
             }
             get localizedName() {
                 return b.get("Dashboard", "DataBars")
             }
             constructor(e, t, r, i, s, n, l, a, o, u, h) {
                 super(e, t, r, i, s, n, l, a, o, u, h), this.ident = F.e.StiMeterIdent.DataBarsCardsColumn, this.width = 0, this.positiveColor = N.transparent, this.negativeColor = N.transparent, this.overlappedColor = N.transparent, this.fillColor = N.transparent, this.minimum = "", this.maximum = ""
             }
         }
-        F.F.StiDataBarsCardsColumn = Pi
+        F.F.StiDataBarsCardsColumn = ji
     } {
-        class ji extends F.F.StiMeasureCardsColumn {
+        class Hi extends F.F.StiMeasureCardsColumn {
             implements() {
-                return ji.ImplementsStiSparklinesCardsColumn || (ji.ImplementsStiSparklinesCardsColumn = super.implements().concat([si, l])), ji.ImplementsStiSparklinesCardsColumn
+                return Hi.ImplementsStiSparklinesCardsColumn || (Hi.ImplementsStiSparklinesCardsColumn = super.implements().concat([si, l])), Hi.ImplementsStiSparklinesCardsColumn
             }
             meta() {
                 return [...super.meta(), new i("Type", "", F.K.StiSparklinesType, F.K.StiSparklinesType.Area), new h("ShowHighLowPoints"), new h("ShowFirstLastPoints", "", !0), new h("AllowCustomColors"), new se("Height"), new r("PositiveColor", "", vr.get("537eb6")), new r("NegativeColor", "", vr.get("ff0000"))]
             }
             getUniqueCode() {
                 let e = super.getUniqueCode();
                 return e = 397 * (e = 397 * (e = 397 * (e = 397 * (e = 397 * (e = 397 * e ^ this.type[L.System.StiObject.stimulsoft]().getHashCode()) ^ this.showHighLowPoints[L.System.StiObject.stimulsoft]().getHashCode()) ^ this.showFirstLastPoints[L.System.StiObject.stimulsoft]().getHashCode()) ^ this.allowCustomColors[L.System.StiObject.stimulsoft]().getHashCode()) ^ this.positiveColor[L.System.StiObject.stimulsoft]().getHashCode()) ^ this.negativeColor[L.System.StiObject.stimulsoft]().getHashCode(), Math.abs(e)
@@ -2408,722 +2409,722 @@
             get localizedName() {
                 return b.get("Dashboard", "Sparklines")
             }
             constructor(e, t, r, i, s, n, l, a, o, u, h, m, c, d, g, p, S) {
                 super(e, t, r, i, s, n, l, h, m, c, S), this.type = F.K.StiSparklinesType.Area, this.showHighLowPoints = !1, this.showFirstLastPoints = !0, this.allowCustomColors = !1, this.positiveColor = vr.get("537eb6"), this.negativeColor = vr.get("ff0000"), this.height = 0, this.ident = F.e.StiMeterIdent.SparklinesCardsColumn, null != a && (this.type = a), null != o && (this.showHighLowPoints = o), null != u && (this.showFirstLastPoints = u), null != d && (this.allowCustomColors = d), null != g && (this.positiveColor = g), null != p && (this.negativeColor = p)
             }
         }
-        F.F.StiSparklinesCardsColumn = ji
+        F.F.StiSparklinesCardsColumn = Hi
     }
-    let Oi = F.R.StiValueNumberBoxMeter,
-        Vi = F.H.StiIndicatorValueChartMeter,
-        ki = F.H.StiSortByChartMeter,
-        Ni = F.F.StiIndicatorCardsColumn,
-        Li = F.F.StiBubbleCardsColumn,
-        Bi = F.F.StiColorScaleCardsColumn,
-        Pi = F.F.StiDataBarsCardsColumn,
-        ji = F.F.StiSparklinesCardsColumn,
-        Hi = F.F.StiDimensionCardsColumn,
-        zi = L.Report.Dictionary.StiDataColumnExt,
-        Gi = F.K.StiBubbleColumn,
-        Xi = F.O.StiLocationArgumentMapMeter,
-        Wi = F.O.StiLocationMapMeter,
-        Ji = F.O.StiLocationColorMapMeter,
-        Ui = F.O.StiLocationValueMapMeter,
-        Zi = L.Data.Engine.StiDataFilterCondition,
-        Yi = F.I.StiKeyTreeViewBoxMeter,
-        Ki = F.J.StiKeyTreeViewMeter,
-        Qi = F.K.StiIndicatorColumn,
-        qi = F.K.StiColorScaleColumn,
-        _i = F.K.StiDataBarsColumn,
-        $i = F.K.StiSparklinesColumn,
-        es = L.Data.Functions.Funcs,
-        ts = F.h.StiTextFormatHelper,
-        rs = F.K.StiDimensionColumn,
-        is = F.K.StiMeasureColumn,
-        ss = F.L.StiColorMapMeter,
-        ns = F.L.StiValueMapMeter,
-        ls = F.L.StiGroupMapMeter,
-        as = F.L.StiNameMapMeter,
-        os = F.L.StiKeyMapMeter,
-        us = F.M.StiValueProgressMeter,
-        hs = F.M.StiTargetProgressMeter,
-        ms = F.M.StiSeriesProgressMeter,
-        cs = F.N.StiPivotColumn,
-        ds = F.N.StiPivotRow,
-        gs = F.N.StiPivotSummary,
-        ps = F.O.StiLatitudeMapMeter,
-        Ss = F.O.StiLongitudeMapMeter,
-        ws = F.P.StiKeyListBoxMeter,
-        bs = F.P.StiNameListBoxMeter,
-        fs = F.Q.StiValueDatePickerMeter,
-        ys = L.Data.Engine.StiDataExpressionHelper,
-        Cs = F.K.StiTableColumn,
+    let Vi = F.R.StiValueNumberBoxMeter,
+        ki = F.H.StiIndicatorValueChartMeter,
+        Ni = F.H.StiSortByChartMeter,
+        Li = F.F.StiIndicatorCardsColumn,
+        Bi = F.F.StiBubbleCardsColumn,
+        Pi = F.F.StiColorScaleCardsColumn,
+        ji = F.F.StiDataBarsCardsColumn,
+        Hi = F.F.StiSparklinesCardsColumn,
+        zi = F.F.StiDimensionCardsColumn,
+        Gi = L.Report.Dictionary.StiDataColumnExt,
+        Xi = F.K.StiBubbleColumn,
+        Wi = F.O.StiLocationArgumentMapMeter,
+        Ji = F.O.StiLocationMapMeter,
+        Ui = F.O.StiLocationColorMapMeter,
+        Zi = F.O.StiLocationValueMapMeter,
+        Yi = L.Data.Engine.StiDataFilterCondition,
+        Ki = F.I.StiKeyTreeViewBoxMeter,
+        Qi = F.J.StiKeyTreeViewMeter,
+        qi = F.K.StiIndicatorColumn,
+        _i = F.K.StiColorScaleColumn,
+        $i = F.K.StiDataBarsColumn,
+        es = F.K.StiSparklinesColumn,
+        ts = L.Data.Functions.Funcs,
+        rs = F.h.StiTextFormatHelper,
+        is = F.K.StiDimensionColumn,
+        ss = F.K.StiMeasureColumn,
+        ns = F.L.StiColorMapMeter,
+        ls = F.L.StiValueMapMeter,
+        as = F.L.StiGroupMapMeter,
+        os = F.L.StiNameMapMeter,
+        us = F.L.StiKeyMapMeter,
+        hs = F.M.StiValueProgressMeter,
+        ms = F.M.StiTargetProgressMeter,
+        cs = F.M.StiSeriesProgressMeter,
+        ds = F.N.StiPivotColumn,
+        gs = F.N.StiPivotRow,
+        ps = F.N.StiPivotSummary,
+        Ss = F.O.StiLatitudeMapMeter,
+        ws = F.O.StiLongitudeMapMeter,
+        bs = F.P.StiKeyListBoxMeter,
+        fs = F.P.StiNameListBoxMeter,
+        ys = F.Q.StiValueDatePickerMeter,
+        Cs = L.Data.Engine.StiDataExpressionHelper,
+        xs = F.K.StiTableColumn,
         w = L.System.DateTime,
-        xs = F.S.StiNameComboBoxMeter,
-        Ms = F.S.StiKeyComboBoxMeter,
-        Ts = F.T.StiSeriesGaugeMeter,
-        Fs = F.T.StiValueGaugeMeter,
-        vs = F.T.StiTargetGaugeMeter,
-        As = F.U.StiSeriesIndicatorMeter,
-        Is = F.U.StiValueIndicatorMeter,
-        Ds = F.U.StiTargetIndicatorMeter,
-        Rs = L.Data.Helpers.StiExpressionHelper,
-        Es = F.H.StiWeightChartMeter,
-        Os = F.H.StiOpenValueChartMeter,
-        Vs = F.H.StiCloseValueChartMeter,
-        ks = F.H.StiLowValueChartMeter,
-        Ns = F.H.StiHighValueChartMeter,
-        Ls = F.H.StiArgumentChartMeter,
-        Bs = F.H.StiValueChartMeter,
-        Ps = F.H.StiSeriesChartMeter,
-        js = F.H.StiEndValueChartMeter,
-        Hs = L.Base.IStiAppAlias,
-        zs = L.Report.Dictionary.StiVariable;
+        Ms = F.S.StiNameComboBoxMeter,
+        Ts = F.S.StiKeyComboBoxMeter,
+        Fs = F.T.StiSeriesGaugeMeter,
+        vs = F.T.StiValueGaugeMeter,
+        As = F.T.StiTargetGaugeMeter,
+        Is = F.U.StiSeriesIndicatorMeter,
+        Ds = F.U.StiValueIndicatorMeter,
+        Rs = F.U.StiTargetIndicatorMeter,
+        Es = L.Data.Helpers.StiExpressionHelper,
+        Os = F.H.StiWeightChartMeter,
+        Vs = F.H.StiOpenValueChartMeter,
+        ks = F.H.StiCloseValueChartMeter,
+        Ns = F.H.StiLowValueChartMeter,
+        Ls = F.H.StiHighValueChartMeter,
+        Bs = F.H.StiArgumentChartMeter,
+        Ps = F.H.StiValueChartMeter,
+        js = F.H.StiSeriesChartMeter,
+        Hs = F.H.StiEndValueChartMeter,
+        zs = L.Base.IStiAppAlias,
+        Gs = L.Report.Dictionary.StiVariable;
     {
         class yg {
             static getValue(e) {
-                if (e.is(Bs)) return e;
-                let t = new Bs;
+                if (e.is(Ps)) return e;
+                let t = new Ps;
                 return t.expression = d.toTotalExpression(e), t.label = e.label, t
             }
             static getGanttStartValue(e) {
-                let t = new Bs;
+                let t = new Ps;
                 return t.expression = d.toExpression(e), t.label = d.toAlias(e), t.seriesType = c.Gantt, t
             }
             static getGanttEndValue(e) {
-                let t = new js;
+                let t = new Hs;
                 return t.expression = d.toExpression(e), t.label = d.toAlias(e), t
             }
             static getEndValue(e) {
-                if (e.is2(js)) return e;
-                let t = new js;
+                if (e.is2(Hs)) return e;
+                let t = new Hs;
                 return t.expression = d.toTotalExpression(e), t.label = e.label, t
             }
             static getOpenValue(e) {
-                if (e.is(Os)) return e;
-                let t = new Os;
-                return t.expression = d.toTotalExpression(e), t.label = e.label, t
-            }
-            static getCloseValue(e) {
-                if (e.is2(Vs)) return e;
+                if (e.is(Vs)) return e;
                 let t = new Vs;
                 return t.expression = d.toTotalExpression(e), t.label = e.label, t
             }
-            static getLowValue(e) {
+            static getCloseValue(e) {
                 if (e.is2(ks)) return e;
                 let t = new ks;
                 return t.expression = d.toTotalExpression(e), t.label = e.label, t
             }
-            static getHighValue(e) {
+            static getLowValue(e) {
                 if (e.is2(Ns)) return e;
                 let t = new Ns;
                 return t.expression = d.toTotalExpression(e), t.label = e.label, t
             }
+            static getHighValue(e) {
+                if (e.is2(Ls)) return e;
+                let t = new Ls;
+                return t.expression = d.toTotalExpression(e), t.label = e.label, t
+            }
             static getValue2(e, t) {
-                let r = new Bs;
+                let r = new Ps;
                 return r.expression = d.toTotalExpression2(e), r.seriesType = null != t.values && 0 < t.values.length ? t.values.firstOrDefault().seriesType : c.ClusteredColumn, r.label = d.toAlias(e), r
             }
             static getEndValue2(e) {
-                let t = new js;
+                let t = new Hs;
                 return t.expression = d.toTotalExpression2(e), t.label = d.toAlias(e), t
             }
             static getCloseValue2(e) {
-                let t = new Vs;
+                let t = new ks;
                 return t.expression = d.toTotalExpression2(e), t.label = d.toAlias(e), t
             }
             static getLowValue2(e) {
-                let t = new ks;
+                let t = new Ns;
                 return t.expression = d.toTotalExpression2(e), t.label = d.toAlias(e), t
             }
             static getHighValue2(e) {
-                let t = new Ns;
+                let t = new Ls;
                 return t.expression = d.toTotalExpression2(e), t.label = d.toAlias(e), t
             }
             static getWeight(e) {
-                if (e.is2(Es)) return e;
-                let t = new Es;
+                if (e.is2(Os)) return e;
+                let t = new Os;
                 return t.expression = d.toTotalExpression(e), t.label = e.label, t
             }
             static getWeight2(e) {
-                let t = new Es;
+                let t = new Os;
                 return t.expression = d.toTotalExpression2(e), t.label = d.toAlias(e), t
             }
             static getArgument(e) {
-                if (e.is2(Ls)) return e;
-                let t = new Ls;
-                return t.expression = Rs.removeFunction(e.expression), t.label = e.label, t
+                if (e.is2(Bs)) return e;
+                let t = new Bs;
+                return t.expression = Es.removeFunction(e.expression), t.label = e.label, t
             }
             static getArgument2(e) {
-                let t = new Ls;
+                let t = new Bs;
                 return t.expression = d.toExpression(e), t.label = d.toAlias(e), t
             }
             static getX2(e) {
-                let t = new Ls;
+                let t = new Bs;
                 return t.expression = d.toExpression(e), t.label = d.toAlias(e), t
             }
             static getX(e) {
-                if (e.is2(Ls)) return e;
-                let t = new Ls;
-                return t.expression = Rs.removeFunction(e.expression), t.label = e.label, t
+                if (e.is2(Bs)) return e;
+                let t = new Bs;
+                return t.expression = Es.removeFunction(e.expression), t.label = e.label, t
             }
             static getY2(e) {
-                let t = new Bs;
+                let t = new Ps;
                 return t.expression = d.toExpression(e), t.label = d.toAlias(e), t
             }
             static getY(e) {
-                if (e.is(Bs)) return e;
-                let t = new Bs;
-                return t.expression = Rs.removeFunction(e.expression), t.label = e.label, t
+                if (e.is(Ps)) return e;
+                let t = new Ps;
+                return t.expression = Es.removeFunction(e.expression), t.label = e.label, t
             }
             static getSeries(e) {
-                if (e.is2(Ps)) return e;
-                let t = new Ps;
-                return t.expression = Rs.removeFunction(e.expression), t.label = e.label, t
+                if (e.is2(js)) return e;
+                let t = new js;
+                return t.expression = Es.removeFunction(e.expression), t.label = e.label, t
             }
             static getSortBy(e) {
-                if (e.is2(ki)) return e;
-                let t = new ki;
-                return t.expression = Rs.removeFunction(e.expression), t.label = e.label, t
+                if (e.is2(Ni)) return e;
+                let t = new Ni;
+                return t.expression = Es.removeFunction(e.expression), t.label = e.label, t
             }
             static getSeries2(e) {
-                let t = new Ps;
+                let t = new js;
                 return t.expression = d.toExpression(e), t.label = d.toAlias(e), t
             }
             static getSortBy2(e) {
-                let t = new ki;
+                let t = new Ni;
                 return t.expression = d.toExpression(e), t.label = d.toAlias(e), t
             }
             static getIndicatorValue(e) {
-                if (e.is2(Vi)) return e;
-                let t = new Vi;
-                return t.expression = Rs.removeFunction(e.expression), t.label = e.label, t
+                if (e.is2(ki)) return e;
+                let t = new ki;
+                return t.expression = Es.removeFunction(e.expression), t.label = e.label, t
             }
             static getIndicatorValue2(e) {
-                let t = new Vi;
+                let t = new ki;
                 return t.expression = d.toExpression(e), t.label = d.toAlias(e), t
             }
         }
         F.h.Chart = yg;
         class Cg {
             static getName(e) {
-                if (e.is2(xs)) return e;
-                let t = new xs;
+                if (e.is2(Ms)) return e;
+                let t = new Ms;
                 return t.expression = e.expression, t.label = e.label, t
             }
             static getName2(e) {
-                let t = new xs;
+                let t = new Ms;
                 return t.expression = d.toExpression(e), t.label = d.toAlias(e), t
             }
             static getKey(e) {
-                if (e.is2(Ms)) return e;
-                let t = new Ms;
+                if (e.is2(Ts)) return e;
+                let t = new Ts;
                 return t.expression = e.expression, t.label = e.label, t
             }
             static getKey2(e) {
-                let t = new Ms;
+                let t = new Ts;
                 return t.expression = d.toExpression(e), t.label = d.toAlias(e), t
             }
         }
         F.h.ComboBox = Cg;
         class xg {
             static getFilter2(e) {
                 let t = "",
                     r = (null != e && null != e.type && (Le.isDateType(e.type) ? t = w.now.toString("MM/dd/yyyy") : Le.isNumericType(e.type) && (t = "0")), new f);
-                return r.key = pe.generateKey(), r.condition = Zi.EqualTo, r.path = d.toExpression(e), r.value = t, r.value2 = t, r
+                return r.key = pe.generateKey(), r.condition = Yi.EqualTo, r.path = d.toExpression(e), r.value = t, r.value2 = t, r
             }
             static getFilter(e, t) {
-                let r = ys.getDataColumnFromExpression(t.page.as(F.e.StiDashboard), e.expression),
+                let r = Cs.getDataColumnFromExpression(t.page.as(F.e.StiDashboard), e.expression),
                     i = "",
                     s = (null != r && null != r.getDataType() && (Le.isDateType(r.getDataType()) ? i = w.now.toString("MM/dd/yyyy") : Le.isNumericType(r.getDataType()) && (i = "0")), new f);
-                return s.key = pe.generateKey(), s.condition = Zi.EqualTo, s.path = Rs.removeFunction(e.expression), s.value = i, s.value2 = i, s
+                return s.key = pe.generateKey(), s.condition = Yi.EqualTo, s.path = Es.removeFunction(e.expression), s.value = i, s.value2 = i, s
             }
         }
         F.h.DataFilter = xg;
         class Mg {
             static getValue(e) {
-                if (e.is2(fs)) return e;
-                let t = new fs;
+                if (e.is2(ys)) return e;
+                let t = new ys;
                 return t.expression = e.expression, t.label = e.label, t
             }
             static getValue2(e) {
-                let t = new fs;
+                let t = new ys;
                 return t.expression = d.toExpression(e), t.label = d.toAlias(e), t
             }
         }
         F.h.DatePicker = Mg;
         class Tg {
             static getValue(e) {
-                if (e.is2(Oi)) return e;
-                let t = new Oi;
+                if (e.is2(Vi)) return e;
+                let t = new Vi;
                 return t.expression = e.expression, t.label = e.label, t
             }
             static getValue2(e) {
-                let t = new Oi;
+                let t = new Vi;
                 return t.expression = d.toExpression(e), t.label = d.toAlias(e), t
             }
         }
         F.h.NumberBox = Tg;
         class Fg {
             static getSeries(e) {
-                if (e.is2(Ts)) return e;
-                let t = new Ts;
-                return t.expression = Rs.removeFunction(e.expression), t.label = e.label, t
+                if (e.is2(Fs)) return e;
+                let t = new Fs;
+                return t.expression = Es.removeFunction(e.expression), t.label = e.label, t
             }
             static getSeries2(e) {
-                let t = new Ts;
+                let t = new Fs;
                 return t.expression = d.toExpression(e), t.label = d.toAlias(e), t
             }
             static getValue(e) {
-                if (e.is2(Fs)) return e;
-                let t = new Fs;
+                if (e.is2(vs)) return e;
+                let t = new vs;
                 return t.expression = d.toTotalExpression(e), t.label = e.label, t
             }
             static getValue2(e) {
-                let t = new Fs;
+                let t = new vs;
                 return t.expression = d.toTotalExpression2(e), t.label = d.toAlias(e), t
             }
             static getTarget(e) {
-                if (e.is2(vs)) return e;
-                let t = new vs;
+                if (e.is2(As)) return e;
+                let t = new As;
                 return t.expression = d.toTotalExpression(e), t.label = e.label, t
             }
             static getTarget2(e) {
-                let t = new vs;
+                let t = new As;
                 return t.expression = d.toTotalExpression2(e), t.label = d.toAlias(e), t
             }
         }
         F.h.Gauge = Fg;
         class vg {
             static getSeries(e) {
-                if (e.is2(As)) return e;
-                let t = new As;
-                return t.expression = Rs.removeFunction(e.expression), t.label = e.label, t
+                if (e.is2(Is)) return e;
+                let t = new Is;
+                return t.expression = Es.removeFunction(e.expression), t.label = e.label, t
             }
             static getSeries2(e) {
-                let t = new As;
+                let t = new Is;
                 return t.expression = d.toExpression(e), t.label = d.toAlias(e), t
             }
             static getValue(e) {
-                if (e.is2(Is)) return e;
-                let t = new Is;
+                if (e.is2(Ds)) return e;
+                let t = new Ds;
                 return t.expression = d.toTotalExpression(e), t.label = e.label, t
             }
             static getValue2(e) {
-                let t = new Is;
+                let t = new Ds;
                 return t.expression = d.toTotalExpression2(e), t.label = d.toAlias(e), t
             }
             static getTarget(e) {
-                if (e.is2(Ds)) return e;
-                let t = new Ds;
+                if (e.is2(Rs)) return e;
+                let t = new Rs;
                 return t.expression = d.toTotalExpression(e), t.label = e.label, t
             }
             static getTarget2(e) {
-                let t = new Ds;
+                let t = new Rs;
                 return t.expression = d.toTotalExpression2(e), t.label = d.toAlias(e), t
             }
         }
         F.h.Indicator = vg;
         class Ag {
             static getName(e) {
-                if (e.is2(bs)) return e;
-                let t = new bs;
+                if (e.is2(fs)) return e;
+                let t = new fs;
                 return t.expression = e.expression, t.label = e.label, t
             }
             static getName2(e) {
-                let t = new bs;
+                let t = new fs;
                 return t.expression = d.toExpression(e), t.label = d.toAlias(e), t
             }
             static getKey(e) {
-                if (e.is2(ws)) return e;
-                let t = new ws;
+                if (e.is2(bs)) return e;
+                let t = new bs;
                 return t.expression = e.expression, t.label = e.label, t
             }
             static getKey2(e) {
-                let t = new ws;
+                let t = new bs;
                 return t.expression = d.toExpression(e), t.label = d.toAlias(e), t
             }
         }
         F.h.ListBox = Ag;
         class Ig {
             static getLatitude(e) {
-                if (e.is2(ps)) return e;
-                let t = new ps;
+                if (e.is2(Ss)) return e;
+                let t = new Ss;
                 return t.expression = e.expression, t.label = e.label, t
             }
             static getLongitude(e) {
-                if (e.is2(Ss)) return e;
-                let t = new Ss;
+                if (e.is2(ws)) return e;
+                let t = new ws;
                 return t.expression = e.expression, t.label = e.label, t
             }
             static getLocation(e) {
-                if (e.is2(Wi)) return e;
-                return new Wi(null, e.expression, e.label)
-            }
-            static getLocationColor(e) {
                 if (e.is2(Ji)) return e;
                 return new Ji(null, e.expression, e.label)
             }
-            static getLocationValue(e) {
+            static getLocationColor(e) {
                 if (e.is2(Ui)) return e;
                 return new Ui(null, e.expression, e.label)
             }
+            static getLocationValue(e) {
+                if (e.is2(Zi)) return e;
+                return new Zi(null, e.expression, e.label)
+            }
             static getLocationArgument(e) {
-                if (e.is2(Xi)) return e;
-                return new Xi(null, e.expression, e.label)
+                if (e.is2(Wi)) return e;
+                return new Wi(null, e.expression, e.label)
             }
             static getLatitude2(e) {
-                let t = new ps;
+                let t = new Ss;
                 return t.expression = d.toExpression(e), t.label = d.toAlias(e), t
             }
             static getLongitude2(e) {
-                let t = new Ss;
+                let t = new ws;
                 return t.expression = d.toExpression(e), t.label = d.toAlias(e), t
             }
             static getLocation2(e) {
-                return new Wi(null, d.toExpression(e), d.toAlias(e))
+                return new Ji(null, d.toExpression(e), d.toAlias(e))
             }
             static getLocationColor2(e) {
-                return new Ji(null, d.toExpression(e), d.toAlias(e))
+                return new Ui(null, d.toExpression(e), d.toAlias(e))
             }
             static getLocationValue2(e) {
-                return new Ui(null, d.toExpression(e), d.toAlias(e))
+                return new Zi(null, d.toExpression(e), d.toAlias(e))
             }
             static getLocationArgument2(e) {
-                return new Xi(null, d.toExpression(e), d.toAlias(e))
+                return new Wi(null, d.toExpression(e), d.toAlias(e))
             }
         }
         F.h.OnlineMap = Ig;
         class Dg {
             static getColumn(e) {
-                if (e.is(cs)) return e;
-                let t = new cs;
-                return t.expression = e.expression, t.label = e.label, t.textFormat = this.getFormat(e), t.topN = this.getTopN(e), t.horAlignment = e.is(Cr) ? e.as(Cr).horAlignment : z.Center, t.size = e.is(mi) ? e.size : new hi, t.totalLabel = this.getTotalLabel(e), t.showTotal = this.getShowTotal(e), t.sortDirection = this.getSortDirection(e), t.expandExpression = this.getExpandExpression(e), t
-            }
-            static getRow(e) {
                 if (e.is(ds)) return e;
                 let t = new ds;
-                return t.expression = e.expression, t.label = e.label, t.textFormat = this.getFormat(e), t.topN = this.getTopN(e), t.horAlignment = e.is(Cr) ? e.as(Cr).horAlignment : z.Center, t.size = e.is(mi) ? e.size : new hi, t.totalLabel = this.getTotalLabel(e), t.showTotal = this.getShowTotal(e), t.sortDirection = this.getSortDirection(e), t.expandExpression = this.getExpandExpression(e), t
+                return t.expression = e.expression, t.label = e.label, t.textFormat = this.getFormat(e), t.topN = this.getTopN(e), t.horAlignment = e.is(Cr) ? e.as(Cr).horAlignment : z.Center, t.size = e.is(ci) ? e.size : new mi, t.totalLabel = this.getTotalLabel(e), t.showTotal = this.getShowTotal(e), t.sortDirection = this.getSortDirection(e), t.expandExpression = this.getExpandExpression(e), t
+            }
+            static getRow(e) {
+                if (e.is(gs)) return e;
+                let t = new gs;
+                return t.expression = e.expression, t.label = e.label, t.textFormat = this.getFormat(e), t.topN = this.getTopN(e), t.horAlignment = e.is(Cr) ? e.as(Cr).horAlignment : z.Center, t.size = e.is(ci) ? e.size : new mi, t.totalLabel = this.getTotalLabel(e), t.showTotal = this.getShowTotal(e), t.sortDirection = this.getSortDirection(e), t.expandExpression = this.getExpandExpression(e), t
             }
             static getShowTotal(e) {
-                return e.is(vi) ? e.as(vi).showTotal : !e.is(Mi) || e.as(Mi).showTotal
+                return e.is(Ai) ? e.as(Ai).showTotal : !e.is(Ti) || e.as(Ti).showTotal
             }
             static getTotalLabel(e) {
-                return e.is(vi) ? e.as(vi).totalLabel : e.is(Mi) ? e.as(Mi).totalLabel : ""
+                return e.is(Ai) ? e.as(Ai).totalLabel : e.is(Ti) ? e.as(Ti).totalLabel : ""
             }
             static getSortDirection(e) {
-                return e.is(vi) ? e.as(vi).strSortDirection : e.is(Mi) ? e.as(Mi).strSortDirection : "None"
+                return e.is(Ai) ? e.as(Ai).strSortDirection : e.is(Ti) ? e.as(Ti).strSortDirection : "None"
             }
             static getExpandExpression(e) {
-                return e.is(vi) ? e.as(vi).expandExpression : e.is(Mi) ? e.as(Mi).expandExpression : ""
+                return e.is(Ai) ? e.as(Ai).expandExpression : e.is(Ti) ? e.as(Ti).expandExpression : ""
             }
             static getSummary(e) {
-                if (e.is(gs)) return e;
-                let t = new gs;
+                if (e.is(ps)) return e;
+                let t = new ps;
                 return t.expression = d.toTotalExpression(e), t.label = e.label, t.textFormat = this.getFormat(e), t
             }
             static getSummary3(e, t) {
-                if (e.is(gs)) return e;
-                let r = new gs;
+                if (e.is(ps)) return e;
+                let r = new ps;
                 return r.expression = d.toTotalExpression3(e, t), r.label = e.label, r.textFormat = this.getFormat(e), r
             }
             static getColumn2(e) {
-                let t = new cs;
+                let t = new ds;
                 return t.expression = d.toExpression(e), t.label = d.toAlias(e), t
             }
             static getRow2(e) {
-                let t = new ds;
+                let t = new gs;
                 return t.expression = d.toExpression(e), t.label = d.toAlias(e), t
             }
             static getSummary2(e) {
-                let t = new gs;
+                let t = new ps;
                 return t.expression = d.toTotalExpression2(e), t.label = d.toAlias(e), t
             }
             static getFormat(e) {
-                if (e.is(cs)) return e.textFormat;
                 if (e.is(ds)) return e.textFormat;
                 if (e.is(gs)) return e.textFormat;
+                if (e.is(ps)) return e.textFormat;
                 return new Jt
             }
             static getTopN(e) {
-                if (e.is(cs)) return e.topN;
                 if (e.is(ds)) return e.topN;
-                return new Fi
+                if (e.is(gs)) return e.topN;
+                return new vi
             }
         }
         F.h.Pivot = Dg;
         class Rg {
             static getSeries(e) {
-                if (e.is2(ms)) return e;
-                let t = new ms;
-                return t.expression = Rs.removeFunction(e.expression), t.label = e.label, t
+                if (e.is2(cs)) return e;
+                let t = new cs;
+                return t.expression = Es.removeFunction(e.expression), t.label = e.label, t
             }
             static getSeries2(e) {
-                let t = new ms;
+                let t = new cs;
                 return t.expression = d.toExpression(e), t.label = d.toAlias(e), t
             }
             static getValue(e) {
-                if (e.is2(us)) return e;
-                let t = new us;
+                if (e.is2(hs)) return e;
+                let t = new hs;
                 return t.expression = d.toTotalExpression(e), t.label = e.label, t
             }
             static getValue2(e) {
-                let t = new us;
+                let t = new hs;
                 return t.expression = d.toTotalExpression2(e), t.label = d.toAlias(e), t
             }
             static getTarget(e) {
-                if (e.is2(hs)) return e;
-                let t = new hs;
+                if (e.is2(ms)) return e;
+                let t = new ms;
                 return t.expression = d.toTotalExpression(e), t.label = e.label, t
             }
             static getTarget2(e) {
-                let t = new hs;
+                let t = new ms;
                 return t.expression = d.toTotalExpression2(e), t.label = d.toAlias(e), t
             }
         }
         F.h.Progress = Rg;
         class Eg {
             static getKey(e) {
-                if (e.is2(os)) return e;
-                let t = new os;
+                if (e.is2(us)) return e;
+                let t = new us;
                 return t.expression = e.expression, t.label = e.label, t
             }
             static getName(e) {
-                if (e.is2(as)) return e;
-                let t = new as;
+                if (e.is2(os)) return e;
+                let t = new os;
                 return t.expression = e.expression, t.label = e.label, t
             }
             static getGroup(e) {
-                if (e.is2(ls)) return e;
-                let t = new ls;
+                if (e.is2(as)) return e;
+                let t = new as;
                 return t.expression = e.expression, t.label = e.label, t
             }
             static getValue(e, t) {
-                let r = new ns,
-                    i = (r.loadFromString(e.saveToString()), ys.isNumericDataColumnInExpression(t, r.expression) ? "Sum" : "Count");
-                return r.expression = Rs.replaceFunction(r.expression, i), r
+                let r = new ls,
+                    i = (r.loadFromString(e.saveToString()), Cs.isNumericDataColumnInExpression(t, r.expression) ? "Sum" : "Count");
+                return r.expression = Es.replaceFunction(r.expression, i), r
             }
             static getColor(e) {
-                if (e.is2(ss)) return e;
-                let t = new ss;
+                if (e.is2(ns)) return e;
+                let t = new ns;
                 return t.expression = e.expression, t.label = e.label, t
             }
             static getKey2(e) {
-                let t = new os;
+                let t = new us;
                 return t.expression = d.toExpression(e), t.label = d.toAlias(e), t
             }
             static getName2(e) {
-                let t = new as;
+                let t = new os;
                 return t.expression = d.toExpression(e), t.label = d.toAlias(e), t
             }
             static getValue2(e) {
-                let t = new ns;
+                let t = new ls;
                 return t.expression = d.toTotalExpression2(e), t.label = d.toAlias(e), t
             }
             static getGroup2(e) {
-                let t = new ls;
+                let t = new as;
                 return t.expression = d.toExpression(e), t.label = d.toAlias(e), t
             }
             static getColor2(e) {
-                let t = new ss;
+                let t = new ns;
                 return t.expression = d.toExpression(e), t.label = d.toAlias(e), t
             }
         }
         F.h.RegionMap = Eg;
         class Og {
             static getColumn(e) {
-                let t = e.as(Cs);
-                return (t = null == t ? new(e.is(vt) ? is : rs) : t).loadFromString(e.saveToString()), t
+                let t = e.as(xs);
+                return (t = null == t ? new(e.is(vt) ? ss : is) : t).loadFromString(e.saveToString()), t
             }
             static getDimension(e) {
-                let t = new rs;
-                return t.loadFromString(e.saveToString()), es.isMeasureFunction(t.expression) && (t.expression = Rs.removeFunction(t.expression)), t
+                let t = new is;
+                return t.loadFromString(e.saveToString()), ts.isMeasureFunction(t.expression) && (t.expression = Es.removeFunction(t.expression)), t
             }
             static getDimension2(e) {
-                let t = new rs;
-                return t.textFormat = ts.getDefaultFormatForColumn(e), t.expression = d.toExpression(e), t.horAlignment = F.h.StiTableAlignmentHelper.getHorAlign(e), t.label = d.toAlias(e), t
+                let t = new is;
+                return t.textFormat = rs.getDefaultFormatForColumn(e), t.expression = d.toExpression(e), t.horAlignment = F.h.StiTableAlignmentHelper.getHorAlign(e), t.label = d.toAlias(e), t
             }
             static getMeasure(e, t) {
-                let r = new is;
-                if (r.loadFromString(e.saveToString()), e.is(rs) || e.is($i)) {
-                    let e = ys.isNumericDataColumnInExpression(t, r.expression) ? "Sum" : "Count";
-                    r.expression = Rs.replaceFunction(r.expression, e)
+                let r = new ss;
+                if (r.loadFromString(e.saveToString()), e.is(is) || e.is(es)) {
+                    let e = Cs.isNumericDataColumnInExpression(t, r.expression) ? "Sum" : "Count";
+                    r.expression = Es.replaceFunction(r.expression, e)
                 }
                 return r
             }
             static getMeasure2(e) {
-                let t = new is;
-                return t.textFormat = ts.getDefaultFormatForColumn(e), t.expression = d.toTotalExpression2(e), t.horAlignment = F.h.StiTableAlignmentHelper.getHorAlign(e), t.label = d.toAlias(e), t
+                let t = new ss;
+                return t.textFormat = rs.getDefaultFormatForColumn(e), t.expression = d.toTotalExpression2(e), t.horAlignment = F.h.StiTableAlignmentHelper.getHorAlign(e), t.label = d.toAlias(e), t
             }
             static getDataBars(e, t) {
-                let r = new _i;
-                if (r.loadFromString(e.saveToString()), e.is(rs) || e.is($i)) {
-                    let e = ys.isNumericDataColumnInExpression(t, r.expression) ? "Sum" : "First";
-                    r.expression = Rs.replaceFunction(r.expression, e)
+                let r = new $i;
+                if (r.loadFromString(e.saveToString()), e.is(is) || e.is(es)) {
+                    let e = Cs.isNumericDataColumnInExpression(t, r.expression) ? "Sum" : "First";
+                    r.expression = Es.replaceFunction(r.expression, e)
                 }
                 return r
             }
             static getColorScale(e, t) {
-                let r = new qi;
-                if (r.loadFromString(e.saveToString()), e.is(rs) || e.is($i)) {
-                    let e = ys.isNumericDataColumnInExpression(t, r.expression) ? "Sum" : "Count";
-                    r.expression = Rs.replaceFunction(r.expression, e)
+                let r = new _i;
+                if (r.loadFromString(e.saveToString()), e.is(is) || e.is(es)) {
+                    let e = Cs.isNumericDataColumnInExpression(t, r.expression) ? "Sum" : "Count";
+                    r.expression = Es.replaceFunction(r.expression, e)
                 }
                 return r
             }
             static getSparklines(e) {
-                let t = new $i;
-                return t.loadFromString(e.saveToString()), es.isMeasureFunction(t.expression) && (t.expression = Rs.removeFunction(t.expression)), t
+                let t = new es;
+                return t.loadFromString(e.saveToString()), ts.isMeasureFunction(t.expression) && (t.expression = Es.removeFunction(t.expression)), t
             }
             static getBubble(e, t) {
-                let r = new Gi;
-                if (r.loadFromString(e.saveToString()), e.is(rs) || e.is($i)) {
-                    let e = ys.isNumericDataColumnInExpression(t, r.expression) ? "Sum" : "Count";
-                    r.expression = Rs.replaceFunction(r.expression, e)
+                let r = new Xi;
+                if (r.loadFromString(e.saveToString()), e.is(is) || e.is(es)) {
+                    let e = Cs.isNumericDataColumnInExpression(t, r.expression) ? "Sum" : "Count";
+                    r.expression = Es.replaceFunction(r.expression, e)
                 }
                 return r
             }
             static getIndicator(e, t) {
-                let r = new Qi;
-                if (r.loadFromString(e.saveToString()), e.is(rs) || e.is($i)) {
-                    let e = ys.isNumericDataColumnInExpression(t, r.expression) ? "Sum" : "Count";
-                    r.expression = Rs.replaceFunction(r.expression, e)
+                let r = new qi;
+                if (r.loadFromString(e.saveToString()), e.is(is) || e.is(es)) {
+                    let e = Cs.isNumericDataColumnInExpression(t, r.expression) ? "Sum" : "Count";
+                    r.expression = Es.replaceFunction(r.expression, e)
                 }
                 return r.horAlignment = z.Right, r
             }
         }
         F.h.Table = Og;
         class Vg {
             static getColumn(e) {
                 let t = e.as(Mr);
-                return (t = null == t ? new(e.is(vt) ? Fr : Hi) : t).loadFromString(e.saveToString()), t
+                return (t = null == t ? new(e.is(vt) ? Fr : zi) : t).loadFromString(e.saveToString()), t
             }
             static getDimension(e) {
-                let t = new Hi;
-                return t.loadFromString(e.saveToString()), es.isMeasureFunction(t.expression) && (t.expression = Rs.removeFunction(t.expression)), t
+                let t = new zi;
+                return t.loadFromString(e.saveToString()), ts.isMeasureFunction(t.expression) && (t.expression = Es.removeFunction(t.expression)), t
             }
             static getDimension2(e) {
-                let t = new Hi;
-                return t.textFormat = ts.getDefaultFormatForColumn(e), t.expression = d.toExpression(e), t.horAlignment = F.h.StiTableAlignmentHelper.getHorAlign(e), t.label = d.toAlias(e), t
+                let t = new zi;
+                return t.textFormat = rs.getDefaultFormatForColumn(e), t.expression = d.toExpression(e), t.horAlignment = F.h.StiTableAlignmentHelper.getHorAlign(e), t.label = d.toAlias(e), t
             }
             static getMeasure(e, t) {
                 let r = new Fr;
-                if (r.loadFromString(e.saveToString()), e.is2(Hi) || e.is2(ji)) {
-                    let e = ys.isNumericDataColumnInExpression(t, r.expression) ? "Sum" : "Count";
-                    r.expression = Rs.replaceFunction(r.expression, e)
+                if (r.loadFromString(e.saveToString()), e.is2(zi) || e.is2(Hi)) {
+                    let e = Cs.isNumericDataColumnInExpression(t, r.expression) ? "Sum" : "Count";
+                    r.expression = Es.replaceFunction(r.expression, e)
                 }
                 return r
             }
             static getMeasure2(e) {
                 let t = new Fr;
-                return t.textFormat = ts.getDefaultFormatForColumn(e), t.expression = d.toTotalExpression2(e), t.horAlignment = F.h.StiTableAlignmentHelper.getHorAlign(e), t.label = d.toAlias(e), t
+                return t.textFormat = rs.getDefaultFormatForColumn(e), t.expression = d.toTotalExpression2(e), t.horAlignment = F.h.StiTableAlignmentHelper.getHorAlign(e), t.label = d.toAlias(e), t
             }
             static getDataBars(e, t) {
-                let r = new Pi;
-                if (r.loadFromString(e.saveToString()), e.is2(Hi) || e.is2(ji)) {
-                    let e = ys.isNumericDataColumnInExpression(t, r.expression) ? "Sum" : "First";
-                    r.expression = Rs.replaceFunction(r.expression, e)
+                let r = new ji;
+                if (r.loadFromString(e.saveToString()), e.is2(zi) || e.is2(Hi)) {
+                    let e = Cs.isNumericDataColumnInExpression(t, r.expression) ? "Sum" : "First";
+                    r.expression = Es.replaceFunction(r.expression, e)
                 }
                 return r
             }
             static getColorScale(e, t) {
-                let r = new Bi;
-                if (r.loadFromString(e.saveToString()), e.is2(Hi) || e.is2(ji)) {
-                    let e = ys.isNumericDataColumnInExpression(t, r.expression) ? "Sum" : "Count";
-                    r.expression = Rs.replaceFunction(r.expression, e)
+                let r = new Pi;
+                if (r.loadFromString(e.saveToString()), e.is2(zi) || e.is2(Hi)) {
+                    let e = Cs.isNumericDataColumnInExpression(t, r.expression) ? "Sum" : "Count";
+                    r.expression = Es.replaceFunction(r.expression, e)
                 }
                 return r
             }
             static getSparklines(e) {
-                let t = new ji;
-                return t.loadFromString(e.saveToString()), es.isMeasureFunction(t.expression) && (t.expression = Rs.removeFunction(t.expression)), t
+                let t = new Hi;
+                return t.loadFromString(e.saveToString()), ts.isMeasureFunction(t.expression) && (t.expression = Es.removeFunction(t.expression)), t
             }
             static getBubble(e, t) {
-                let r = new Li;
-                if (r.loadFromString(e.saveToString()), e.is2(Hi) || e.is2(ji)) {
-                    let e = ys.isNumericDataColumnInExpression(t, r.expression) ? "Sum" : "Count";
-                    r.expression = Rs.replaceFunction(r.expression, e)
+                let r = new Bi;
+                if (r.loadFromString(e.saveToString()), e.is2(zi) || e.is2(Hi)) {
+                    let e = Cs.isNumericDataColumnInExpression(t, r.expression) ? "Sum" : "Count";
+                    r.expression = Es.replaceFunction(r.expression, e)
                 }
                 return r
             }
             static getIndicator(e, t) {
-                let r = new Ni;
-                if (r.loadFromString(e.saveToString()), e.is2(Hi) || e.is2(ji)) {
-                    let e = ys.isNumericDataColumnInExpression(t, r.expression) ? "Sum" : "Count";
-                    r.expression = Rs.replaceFunction(r.expression, e)
+                let r = new Li;
+                if (r.loadFromString(e.saveToString()), e.is2(zi) || e.is2(Hi)) {
+                    let e = Cs.isNumericDataColumnInExpression(t, r.expression) ? "Sum" : "Count";
+                    r.expression = Es.replaceFunction(r.expression, e)
                 }
                 return r.horAlignment = z.Right, r
             }
         }
         F.h.Cards = Vg;
         class kg {
             static getKey(e) {
-                if (e.is2(Ki)) return e;
-                let t = new Ki;
+                if (e.is2(Qi)) return e;
+                let t = new Qi;
                 return t.expression = e.expression, t.label = e.label, t
             }
             static getKey2(e) {
-                let t = new Ki;
+                let t = new Qi;
                 return t.expression = d.toExpression(e), t.label = d.toAlias(e), t
             }
         }
         F.h.TreeView = kg;
         class Ng {
             static getKey(e) {
-                if (e.is2(Yi)) return e;
-                let t = new Yi;
+                if (e.is2(Ki)) return e;
+                let t = new Ki;
                 return t.expression = e.expression, t.label = e.label, t
             }
             static getKey2(e) {
-                let t = new Yi;
+                let t = new Ki;
                 return t.expression = d.toExpression(e), t.label = d.toAlias(e), t
             }
         }
         F.h.TreeViewBox = Ng;
         class d {
             static toTotalExpression2(e) {
-                let t = null == e ? void 0 : e.as(oi);
-                if (null != t) return zi.isNumericType(t) ? this.toSumExpression2(t) : this.toCountExpression2(t);
+                let t = null == e ? void 0 : e.as(ui);
+                if (null != t) return Gi.isNumericType(t) ? this.toSumExpression2(t) : this.toCountExpression2(t);
                 return null == e ? void 0 : e.getName()
             }
             static toTotalExpression(e) {
-                if (Rs.isFunctionPresent(e.expression)) return e.expression;
+                if (Es.isFunctionPresent(e.expression)) return e.expression;
                 return this.toCountExpression(e.expression)
             }
             static toTotalExpression3(e, t) {
-                if (Rs.isFunctionPresent(e.expression)) return e.expression;
-                return ys.isNumericDataColumnInExpression(t, e.expression) ? this.toSumExpression(e.expression) : this.toCountExpression(e.expression)
+                if (Es.isFunctionPresent(e.expression)) return e.expression;
+                return Cs.isNumericDataColumnInExpression(t, e.expression) ? this.toSumExpression(e.expression) : this.toCountExpression(e.expression)
             }
             static toSumExpression2(e) {
                 return `Sum(${this.toExpression(e)})`
             }
             static toSumExpression(e) {
                 return `Sum(${e})`
             }
             static toCountExpression2(e) {
                 return `Count(${this.toExpression(e)})`
             }
             static toCountExpression(e) {
                 return `Count(${e})`
             }
             static toExpression(e) {
-                let t = null == e ? void 0 : e.as(oi);
-                if (null != t) return es.toExpression2(t.dataSource.name, t.name);
-                return es.toExpression(null == e ? void 0 : e.getName())
+                let t = null == e ? void 0 : e.as(ui);
+                if (null != t) return ts.toExpression2(t.dataSource.name, t.name);
+                return ts.toExpression(null == e ? void 0 : e.getName())
             }
             static toAlias(e) {
-                let t = e.as(Hs);
+                let t = e.as(zs);
                 if (null != t) return t.getAlias();
                 return null == e ? void 0 : e.getName()
             }
             static toDataType(e) {
                 var t, r;
-                let i = null == (t = null == e ? void 0 : e.as(oi)) ? void 0 : t.type;
+                let i = null == (t = null == e ? void 0 : e.as(ui)) ? void 0 : t.type;
                 if (null != i) return i;
-                return null == (r = null == e ? void 0 : e.as(zs)) ? void 0 : r.type
+                return null == (r = null == e ? void 0 : e.as(Gs)) ? void 0 : r.type
             }
         }
         d.Chart = yg, d.ComboBox = Cg, d.DataFilter = xg, d.DatePicker = Mg, d.NumberBox = Tg, d.Gauge = Fg, d.Indicator = vg, d.ListBox = Ag, d.OnlineMap = Ig, d.Pivot = Dg, d.Progress = Rg, d.RegionMap = Eg, d.Table = Og, d.Cards = Vg, d.TreeView = kg, d.TreeViewBox = Ng, F.h.StiMeterHelper = d
     }
     F.F.StiCardsItem = class {
         constructor() {
             this.cornerRadius = new m(0), this.margin = new lt(12, 12, 12, 12), this.padding = new nt(12, 12, 12, 12), this.colorEach = !1
@@ -3146,99 +3147,99 @@
         isDefaultMargin() {
             return 12 == this.margin.left && 12 == this.margin.top && 12 == this.margin.right && 12 == this.margin.bottom
         }
         isDefaultPadding() {
             return 12 == this.padding.left && 12 == this.padding.top && 12 == this.padding.right && 12 == this.padding.bottom
         }
     };
-    let Gs = L.Report.Dashboard.IStiInteractionLayout;
+    let Xs = L.Report.Dashboard.IStiInteractionLayout;
     {
-        class Ws extends F.g.StiDashboardInteraction {
+        class Js extends F.g.StiDashboardInteraction {
             implements() {
-                return Ws.ImplementsIStiCardsDashboardInteraction || (Ws.ImplementsIStiCardsDashboardInteraction = super.implements().concat([l, Gs])), Ws.ImplementsIStiCardsDashboardInteraction
+                return Js.ImplementsIStiCardsDashboardInteraction || (Js.ImplementsIStiCardsDashboardInteraction = super.implements().concat([l, Xs])), Js.ImplementsIStiCardsDashboardInteraction
             }
             meta() {
                 return [...super.meta(), new h("ShowFullScreenButton", "", !0), new h("ShowSaveButton", "", !0), new h("ShowViewDataButton", "", !0)]
             }
             get isDefaultLayout() {
                 return this.showFullScreenButton && this.showSaveButton && this.showViewDataButton && null == this.fileName && null == this.headerText && null == this.footerText
             }
             isDefault() {
                 return this.isDefaultLayout
             }
             constructor(e, t, r) {
                 super(), this.ident = Lr.Cards, this.availableOnClick = Br.None, this.availableOnHover = Pr.None, this.showFullScreenButton = !0, this.showSaveButton = !0, this.showViewDataButton = !0, this.fileName = null, this.headerText = null, this.footerText = null, null != e && (this.showFullScreenButton = e), null != t && (this.showSaveButton = t), null != r && (this.showViewDataButton = r)
             }
         }
-        F.g.StiCardsDashboardInteraction = Ws
+        F.g.StiCardsDashboardInteraction = Js
     }
-    let Xs = L.Report.Components.IStiShowBlanks,
-        Ws = F.g.StiCardsDashboardInteraction,
+    let Ws = L.Report.Components.IStiShowBlanks,
+        Js = F.g.StiCardsDashboardInteraction,
         d = F.h.StiMeterHelper,
-        Js = L.System.Text.StiReportObjectStringConverter,
-        Us = L.Report.Dashboard.IStiSeriesColors,
-        Zs = F.F.StiCardsItem,
+        Us = L.System.Text.StiReportObjectStringConverter,
+        Zs = L.Report.Dashboard.IStiSeriesColors,
+        Ys = F.F.StiCardsItem,
         g = F.G.StiMeterLoader,
-        Ys = L.Report.Dashboard.StiItemOrientation,
-        Ks = L.Report.Dashboard.ImplementsIStiCardsElement,
-        Qs = L.Report.Dashboard.ImplementsIStiElementLayout,
-        qs = L.Report.Dashboard.IStiElementLayout,
-        _s = L.Report.Dashboard.StiElementLayout,
-        $s = L.Report.Dashboard.ImplementsIStiTitleElement,
-        en = L.Data.Helpers.StiUsedDataHelper,
-        tn = L.Report.Dashboard.IStiCardsElement,
-        rn = L.Data.Engine.StiDataSortRule,
-        sn = L.Data.Engine.StiDataActionRule;
+        Ks = L.Report.Dashboard.StiItemOrientation,
+        Qs = L.Report.Dashboard.ImplementsIStiCardsElement,
+        qs = L.Report.Dashboard.ImplementsIStiElementLayout,
+        _s = L.Report.Dashboard.IStiElementLayout,
+        $s = L.Report.Dashboard.StiElementLayout,
+        en = L.Report.Dashboard.ImplementsIStiTitleElement,
+        tn = L.Data.Helpers.StiUsedDataHelper,
+        rn = L.Report.Dashboard.IStiCardsElement,
+        sn = L.Data.Engine.StiDataSortRule,
+        nn = L.Data.Engine.StiDataActionRule;
     {
         class Cm extends F.e.StiElement {
             implements() {
-                return Cm.ImplementsStiCardsElement || (Cm.ImplementsStiCardsElement = super.implements().concat([tn, Ke, Oe, qs, Qr, Ze, Us, Ne, Xs, ...Ks, ...$s, ...Qs, ...Ue, l])), Cm.ImplementsStiCardsElement
+                return Cm.ImplementsStiCardsElement || (Cm.ImplementsStiCardsElement = super.implements().concat([rn, Ke, Oe, _s, Qr, Ze, Zs, Ne, Ws, ...Qs, ...en, ...qs, ...Ue, l])), Cm.ImplementsStiCardsElement
             }
             clone(e) {
                 var t, r, i;
                 let s = super.clone(e);
                 return s.transformActions = this.transformActions.select(e => e.clone()).toList(), s.transformFilters = this.transformFilters.select(e => e.clone()).toList(), s.transformSorts = this.transformSorts.select(e => e.clone()).toList(), s.columns = this.columns.select(e => e.clone()).toList(), s.dashboardInteraction = null == (t = this.dashboardInteraction) ? void 0 : t.clone(), s.dataFilters = this.dataFilters.select(e => e.clone()).toList(), s.title = null != this.title ? this.title.clone() : null, s.seriesColors = null != this.seriesColors ? this.seriesColors[L.System.StiObject.stimulsoft]().clone() : null, s.cornerRadius = null == (r = this.cornerRadius) ? void 0 : r.clone(), s.shadow = null == (i = this.shadow) ? void 0 : i.clone(), s
             }
             meta() {
-                return [...super.meta(), new s("Columns").get(e => a.Serialize.objectArray(this.columns, e)).set(e => this.columns.addRange(e.value.properties().select(e => g.loadFromJson(e.value).as(Mr)).where(e => null != e))).setXml(e => this.columns.addRange(e.childNodes.select(e => g.loadFromXml(e)).where(e => null != e))), new i("Orientation", "", Ys, Ys.Horizontal), new s("Title").check(() => null != this.title).set(e => this.title = F.e.StiTitle.createFromJsonObject(e.value)).setXml(e => this.title = F.e.StiTitle.createFromXml(e)), new s("Layout").check(() => null != this.layout).set(e => this.layout = _s.createFromJsonObject(e.value)).setXml(e => this.layout = _s.createFromXml(e)), new i("Style", "", o, o.Auto), new n("CustomStyleName"), new se("ColumnCount", "", 0), new n("Group"), new h("CrossFiltering", "", !0), new s("TransformActions").get(e => a.Serialize.objectArray(this.transformActions, e)).set(e => this.transformActions.addRange(e.value.properties().select(e => sn.loadFromJson(e.value)))).setXml(e => this.transformActions.addRange(e.childNodes.select(e => sn.loadFromXml(e)))), new s("TransformFilters").get(e => a.Serialize.objectArray(this.transformFilters, e)).set(e => this.transformFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.transformFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new s("TransformSorts").get(e => a.Serialize.objectArray(this.transformSorts, e)).set(e => this.transformSorts.addRange(e.value.properties().select(e => rn.loadFromJson(e.value)))).setXml(e => this.transformSorts.addRange(e.childNodes.select(e => rn.loadFromXml(e)))), new s("DataFilters").get(e => a.Serialize.objectArray(this.dataFilters, e)).set(e => this.dataFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.dataFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new s("Cards").get(e => this.cards.saveToJsonObject(e)), new n("CornerRadius").get(() => this.cornerRadius.toString()).set(e => this.cornerRadius = m.tryParse(e.value.toString())).setXml(e => this.cornerRadius = m.tryParse(e.textContent)), new n("Shadow").get(() => a.Serialize.jShadow(this.shadow)).set(e => this.shadow = a.Deserialize.simpleSahdow(e.value)).setXml(e => this.shadow = Ye.loadFromXml(e.textContent)), new s("SeriesColors").get(() => a.Serialize.colorArray(this.seriesColors)).set(e => this.seriesColors = a.Deserialize.colorArray(e.value)).setXml(e => this.seriesColors = Js.convertStringToColorArray(e.textContent)), new h("ShowBlanks"), new s("DashboardInteraction").check(() => null != this.dashboardInteraction.as(Ws)).set(e => {
+                return [...super.meta(), new s("Columns").get(e => a.Serialize.objectArray(this.columns, e)).set(e => this.columns.addRange(e.value.properties().select(e => g.loadFromJson(e.value).as(Mr)).where(e => null != e))).setXml(e => this.columns.addRange(e.childNodes.select(e => g.loadFromXml(e)).where(e => null != e))), new i("Orientation", "", Ks, Ks.Horizontal), new s("Title").check(() => null != this.title).set(e => this.title = F.e.StiTitle.createFromJsonObject(e.value)).setXml(e => this.title = F.e.StiTitle.createFromXml(e)), new s("Layout").check(() => null != this.layout).set(e => this.layout = $s.createFromJsonObject(e.value)).setXml(e => this.layout = $s.createFromXml(e)), new i("Style", "", o, o.Auto), new n("CustomStyleName"), new se("ColumnCount", "", 0), new n("Group"), new h("CrossFiltering", "", !0), new s("TransformActions").get(e => a.Serialize.objectArray(this.transformActions, e)).set(e => this.transformActions.addRange(e.value.properties().select(e => nn.loadFromJson(e.value)))).setXml(e => this.transformActions.addRange(e.childNodes.select(e => nn.loadFromXml(e)))), new s("TransformFilters").get(e => a.Serialize.objectArray(this.transformFilters, e)).set(e => this.transformFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.transformFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new s("TransformSorts").get(e => a.Serialize.objectArray(this.transformSorts, e)).set(e => this.transformSorts.addRange(e.value.properties().select(e => sn.loadFromJson(e.value)))).setXml(e => this.transformSorts.addRange(e.childNodes.select(e => sn.loadFromXml(e)))), new s("DataFilters").get(e => a.Serialize.objectArray(this.dataFilters, e)).set(e => this.dataFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.dataFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new s("Cards").get(e => this.cards.saveToJsonObject(e)), new n("CornerRadius").get(() => this.cornerRadius.toString()).set(e => this.cornerRadius = m.tryParse(e.value.toString())).setXml(e => this.cornerRadius = m.tryParse(e.textContent)), new n("Shadow").get(() => a.Serialize.jShadow(this.shadow)).set(e => this.shadow = a.Deserialize.simpleSahdow(e.value)).setXml(e => this.shadow = Ye.loadFromXml(e.textContent)), new s("SeriesColors").get(() => a.Serialize.colorArray(this.seriesColors)).set(e => this.seriesColors = a.Deserialize.colorArray(e.value)).setXml(e => this.seriesColors = Us.convertStringToColorArray(e.textContent)), new h("ShowBlanks"), new s("DashboardInteraction").check(() => null != this.dashboardInteraction.as(Js)).set(e => {
                     var t;
-                    let r = null == (t = qr.loadInteractionFromJsonObject(e.value)) ? void 0 : t.as(Ws);
+                    let r = null == (t = qr.loadInteractionFromJsonObject(e.value)) ? void 0 : t.as(Js);
                     null != r && (this.dashboardInteraction = r)
                 }).setXml(e => {
                     var t;
-                    let r = null == (t = qr.loadInteractionFromXml(e)) ? void 0 : t.as(Ws);
+                    let r = null == (t = qr.loadInteractionFromXml(e)) ? void 0 : t.as(Js);
                     null != r && (this.dashboardInteraction = r)
                 })]
             }
             get toolboxPosition() {
                 return tt.CardsElement
             }
             get localizedName() {
                 return A.get("Components", "StiCards")
             }
             convertFrom(e) {
                 let t = e.fetchAllMeters();
                 if (this.columns.clear(), null == t) return;
                 t.cast().forEach(e => {
                     let t = null;
-                    e.is2(ze) ? t = new Hi : e.is2(si) ? t = new F.F.StiSparklinesCardsColumn : e.is2(ii) ? t = new F.F.StiDataBarsCardsColumn : e.is2(ti) ? t = new F.F.StiIndicatorCardsColumn : e.is2(ri) ? t = new F.F.StiColorScaleCardsColumn : e.is2(Ar) ? t = new F.F.StiBubbleCardsColumn : e.is2(vt) && ((t = new Fr).horAlignment = z.Right), null != t && (t.loadFromJsonObject(e.saveToJsonObject(je.Report)), this.columns.add(t))
-                }, this), null == this.dashboardInteraction && (this.dashboardInteraction = new Ws)
+                    e.is2(ze) ? t = new zi : e.is2(si) ? t = new F.F.StiSparklinesCardsColumn : e.is2(ii) ? t = new F.F.StiDataBarsCardsColumn : e.is2(ti) ? t = new F.F.StiIndicatorCardsColumn : e.is2(ri) ? t = new F.F.StiColorScaleCardsColumn : e.is2(Ar) ? t = new F.F.StiBubbleCardsColumn : e.is2(vt) && ((t = new Fr).horAlignment = z.Right), null != t && (t.loadFromJsonObject(e.saveToJsonObject(je.Report)), this.columns.add(t))
+                }, this), null == this.dashboardInteraction && (this.dashboardInteraction = new Js)
             }
             createMeters(e) {
                 let t = e.as(Cm);
                 this.columns.clear();
                 for (let e of t.columns) this.columns.add(e)
             }
             createMeters2(t) {
                 this.columns.clear();
                 for (let e of t.columns.list) null != e && null != e.type && Le.isNumericType(e.type) ? this.columns.add(d.Cards.getMeasure2(e)) : this.columns.add(d.Cards.getDimension2(e))
             }
             createMeter(e) {
-                let t = e.as(oi),
-                    r = e.as(zs),
+                let t = e.as(ui),
+                    r = e.as(Gs),
                     i = null != t ? t.type : null == r ? void 0 : r.type;
                 if (null != i && Le.isNumericType(i)) {
                     let e = d.Cards.getMeasure2(t);
                     this.columns.add(e)
                 } else this.columns.add(d.Cards.getDimension2(e))
             }
             removeMeter(e) {
@@ -3249,15 +3250,15 @@
             }
             insertMeter(e, t) {
                 let r = t.as(Mr);
                 if (null == r) return;
                 0 <= e && e < this.columns.length ? this.columns.insert(e, r) : this.columns.add(r)
             }
             insertNewDimension(e) {
-                let t = new Hi;
+                let t = new zi;
                 t.horAlignment = z.Left, this.insertMeter(e, t)
             }
             insertNewMeasure(e) {
                 let t = new Fr;
                 t.expression = "Sum()", t.horAlignment = z.Right, this.insertMeter(e, t)
             }
             getMeasure(e) {
@@ -3272,15 +3273,15 @@
             fetchAllMeters() {
                 return this.columns.cast()
             }
             getMeters() {
                 return this.columns.cast()
             }
             retrieveUsedDataNames() {
-                return en.getMany2(this.columns)
+                return tn.getMany2(this.columns)
             }
             get isDefined() {
                 return null != this.columns && 0 < this.columns.length
             }
             setString(e, t) {
                 switch (e) {
                     case "Title.Text":
@@ -3302,27 +3303,27 @@
             get style() {
                 return this._style
             }
             set style(e) {
                 (this._style = e) != o.Custom && (this.customStyleName = "")
             }
             constructor(e = j.empty) {
-                super(e), this.helpUrl = "user-manual/dashboards_cards.htm", this.dataFilters = new P, this.transformActions = new P, this.transformFilters = new P, this.transformSorts = new P, this.dataTransformation = {}, this.group = "", this.title = new F.e.StiTitle, this.crossFiltering = !0, this.shadow = new Ye, this.layout = new _s, this.cornerRadius = new m(0), this.showBlanks = !1, this._style = o.Auto, this.customStyleName = "", this.seriesColors = [], this.orientation = Ys.Horizontal, this.columns = new P, this.cards = new Zs, this.columnCount = 0, this.title.text = this.localizedName, this.dashboardInteraction = new Ws
+                super(e), this.helpUrl = "user-manual/dashboards_cards.htm", this.dataFilters = new P, this.transformActions = new P, this.transformFilters = new P, this.transformSorts = new P, this.dataTransformation = {}, this.group = "", this.title = new F.e.StiTitle, this.crossFiltering = !0, this.shadow = new Ye, this.layout = new $s, this.cornerRadius = new m(0), this.showBlanks = !1, this._style = o.Auto, this.customStyleName = "", this.seriesColors = [], this.orientation = Ks.Horizontal, this.columns = new P, this.cards = new Ys, this.columnCount = 0, this.title.text = this.localizedName, this.dashboardInteraction = new Js
             }
         }
         F.F.StiCardsElement = Cm
     } {
         let e;
         (D = e = F.H.StiChartLabelsStyle || (F.H.StiChartLabelsStyle = {}))[D["Value"] = 0] = "Value", D[D["PercentOfTotal"] = 1] = "PercentOfTotal", D[D["Category"] = 2] = "Category", D[D["CategoryValue"] = 3] = "CategoryValue", D[D["CategoryPercentOfTotal"] = 4] = "CategoryPercentOfTotal";
         let t;
         (I = t = F.H.StiLegendVisibility || (F.H.StiLegendVisibility = {}))[I["False"] = 0] = "False", I[I["Auto"] = 1] = "Auto", I[I["Always"] = 2] = "Always"
     } {
-        class nn {
+        class ln {
             implements() {
-                return nn.implementsStiChartAreaIndicator || (nn.implementsStiChartAreaIndicator = [l, Vt]), nn.implementsStiChartAreaIndicator
+                return ln.implementsStiChartAreaIndicator || (ln.implementsStiChartAreaIndicator = [l, Vt]), ln.implementsStiChartAreaIndicator
             }
             meta() {
                 return [new s("Value"), new s("Title")]
             }
             saveToJsonObject(e) {
                 return u.saveToJsonObject(e, this)
             }
@@ -3336,22 +3337,22 @@
                 let e = this[L.System.StiObject.stimulsoft]().memberwiseClone();
                 return e.value = this.value.clone(), e.title = this.title.clone(), e
             }
             constructor() {
                 this.value = new F.H.StiChartAreaIndicatorValue, this.title = new F.H.StiChartAreaIndicatorTitle
             }
         }
-        F.H.StiChartAreaIndicator = nn
+        F.H.StiChartAreaIndicator = ln
     }
-    let nn = F.H.StiChartAreaIndicator,
-        ln = L.Report.Dashboard.IStiChartArea;
+    let ln = F.H.StiChartAreaIndicator,
+        an = L.Report.Dashboard.IStiChartArea;
     {
         class Lg {
             implements() {
-                return Lg.ImplementsStiChartArea || (Lg.ImplementsStiChartArea = [ln, l]), Lg.ImplementsStiChartArea
+                return Lg.ImplementsStiChartArea || (Lg.ImplementsStiChartArea = [an, l]), Lg.ImplementsStiChartArea
             }
             meta() {
                 return [new h("ColorEach"), new h("SideBySide", "", !1, !0), new s("GridLinesHor"), new s("GridLinesVert"), new s("InterlacingHor"), new s("InterlacingVert"), new h("ReverseHor"), new h("ReverseVert"), new s("XAxis").check(() => !1), new s("XTopAxis").check(() => !1), new s("YAxis").check(() => !1), new s("YRightAxis").check(() => !1), new s("Indicator"), new se("HorSpacing", "", 6), new se("VertSpacing", "", 6)]
             }
             saveToJsonObject(e) {
                 return u.saveToJsonObject(e, this)
             }
@@ -3374,15 +3375,15 @@
             get vertSpacing() {
                 return this._vertSpacing
             }
             set vertSpacing(e) {
                 0 <= e && (this._vertSpacing = e)
             }
             constructor(e, t, r, i, s, n, l, a, o, u, h, m) {
-                this.sideBySide = !0, this.colorEach = !1, this.reverseHor = !1, this.reverseVert = !1, this.interlacingHor = new F.H.StiHorChartInterlacing, this.interlacingVert = new F.H.StiVertChartInterlacing, this.gridLinesHor = new F.H.StiHorChartGridLines, this.gridLinesVert = new F.H.StiVertChartGridLines, this.xAxis = new F.H.StiXChartAxis, this.xTopAxis = new F.H.StiXTopChartAxis, this.yAxis = new F.H.StiYChartAxis, this.yRightAxis = new F.H.StiYRightChartAxis, this.indicator = new nn, this._horSpacing = 6, this._vertSpacing = 6, null != e && (this.colorEach = e), null != t && (this.reverseHor = t), null != r && (this.reverseVert = r), null != i && (this.gridLinesHor = i), null != s && (this.gridLinesVert = s), null != s && (this.interlacingHor = n), null != l && (this.interlacingVert = l), null != a && (this.xAxis = a), null != o && (this.yAxis = o), null != u && (this.xTopAxis = u), null != h && (this.yRightAxis = h), null != m && (this.indicator = m)
+                this.sideBySide = !0, this.colorEach = !1, this.reverseHor = !1, this.reverseVert = !1, this.interlacingHor = new F.H.StiHorChartInterlacing, this.interlacingVert = new F.H.StiVertChartInterlacing, this.gridLinesHor = new F.H.StiHorChartGridLines, this.gridLinesVert = new F.H.StiVertChartGridLines, this.xAxis = new F.H.StiXChartAxis, this.xTopAxis = new F.H.StiXTopChartAxis, this.yAxis = new F.H.StiYChartAxis, this.yRightAxis = new F.H.StiYRightChartAxis, this.indicator = new ln, this._horSpacing = 6, this._vertSpacing = 6, null != e && (this.colorEach = e), null != t && (this.reverseHor = t), null != r && (this.reverseVert = r), null != i && (this.gridLinesHor = i), null != s && (this.gridLinesVert = s), null != s && (this.interlacingHor = n), null != l && (this.interlacingVert = l), null != a && (this.xAxis = a), null != o && (this.yAxis = o), null != u && (this.xTopAxis = u), null != h && (this.yRightAxis = h), null != m && (this.indicator = m)
             }
         }
         F.H.StiChartArea = Lg
     } {
         class Bg {
             constructor() {
                 this.text = "", this.color = N.transparent
@@ -3431,22 +3432,22 @@
             clone() {
                 let e = this[L.System.StiObject.stimulsoft]().memberwiseClone();
                 return e
             }
         }
         F.H.StiChartAreaIndicatorValue = Pg
     }
-    let an = L.Report.Chart.StiLabelsPlacement;
+    let on = L.Report.Chart.StiLabelsPlacement;
     {
-        class on {
+        class un {
             implements() {
-                return on.ImplementsStiChartAxisLabels || (on.ImplementsStiChartAxisLabels = [Vt, ar, ...rr, l]), on.ImplementsStiChartAxisLabels
+                return un.ImplementsStiChartAxisLabels || (un.ImplementsStiChartAxisLabels = [Vt, ar, ...rr, l]), un.ImplementsStiChartAxisLabels
             }
             meta() {
-                return [new se("Angle", "", 0), new n("TextBefore"), new n("TextAfter"), new Rt("Font", "", "Arial", 8), new i("Placement", "", an, an.AutoRotation), new r("Color", "", N.transparent), new i("TextAlignment", "", z, z.Right), new se("Step", "", 0), new h("WordWrap"), new se("Width")]
+                return [new se("Angle", "", 0), new n("TextBefore"), new n("TextAfter"), new Rt("Font", "", "Arial", 8), new i("Placement", "", on, on.AutoRotation), new r("Color", "", N.transparent), new i("TextAlignment", "", z, z.Right), new se("Step", "", 0), new h("WordWrap"), new se("Width")]
             }
             saveToJsonObject(e) {
                 return u.saveToJsonObject(e, this)
             }
             loadFromJsonObject(e) {
                 u.loadFromJsonObject(e, this)
             }
@@ -3454,20 +3455,20 @@
                 u.loadFromXml(e, this)
             }
             clone() {
                 let e = this[L.System.StiObject.stimulsoft]().memberwiseClone();
                 return e.font = this.font.clone(), e
             }
             constructor(e, t, r, i, s, n, l, a, o) {
-                this.angle = 0, this.color = N.transparent, this.font = new H("Arial", 8), this.placement = an.AutoRotation, this.textAlignment = z.Right, this.textAfter = "", this.textBefore = "", this.step = 0, this.wordWrap = !1, this.width = 0, null != e && (this.textBefore = e), null != t && (this.textAfter = t), null != r && (this.angle = r), null != i && (this.font = i), null != s && (this.placement = s), null != n && (this.color = n), null != l && (this.textAlignment = l), null != a && (this.width = a), null != o && (this.wordWrap = o)
+                this.angle = 0, this.color = N.transparent, this.font = new H("Arial", 8), this.placement = on.AutoRotation, this.textAlignment = z.Right, this.textAfter = "", this.textBefore = "", this.step = 0, this.wordWrap = !1, this.width = 0, null != e && (this.textBefore = e), null != t && (this.textAfter = t), null != r && (this.angle = r), null != i && (this.font = i), null != s && (this.placement = s), null != n && (this.color = n), null != l && (this.textAlignment = l), null != a && (this.width = a), null != o && (this.wordWrap = o)
             }
         }
-        F.H.StiChartAxisLabels = on
+        F.H.StiChartAxisLabels = un
     }
-    let on = F.H.StiChartAxisLabels;
+    let un = F.H.StiChartAxisLabels;
     {
         class jg {
             implements() {
                 return jg.ImplementsStiChartAxis || (jg.ImplementsStiChartAxis = [l, Vt]), jg.ImplementsStiChartAxis
             }
             is(e) {
                 if (e instanceof L.System.Interface) return -1 != this.implements().indexOf(e);
@@ -3495,15 +3496,15 @@
             loadFromJsonObject(e) {
                 u.loadFromJsonObject(e, this)
             }
             loadFromXml(e) {
                 u.loadFromXml(e, this)
             }
             constructor(e, t, r) {
-                this.labels = new on, this.range = new F.H.StiChartAxisRange, this.visible = !0, null != e && (this.labels = e), null != t && (this.range = t), null != r && (this.visible = r)
+                this.labels = new un, this.range = new F.H.StiChartAxisRange, this.visible = !0, null != e && (this.labels = e), null != t && (this.range = t), null != r && (this.visible = r)
             }
         }
         F.H.StiChartAxis = jg
     } {
         class Hg {
             implements() {
                 return Hg.ImplementsStiChartAxisRange || (Hg.ImplementsStiChartAxisRange = [l, Vt]), Hg.ImplementsStiChartAxisRange
@@ -3531,17 +3532,17 @@
             }
             constructor(e, t, r) {
                 this._minimum = 0, this.maximum = 0, this.auto = !0, null != e && (this.auto = e), null != t && (this.minimum = t), null != r && (this.maximum = r)
             }
         }
         F.H.StiChartAxisRange = Hg
     }
-    let un = L.Report.Chart.StiTitlePosition,
-        hn = L.System.Drawing.FontStyle,
-        mn = L.System.Drawing.StringAlignment;
+    let hn = L.Report.Chart.StiTitlePosition,
+        mn = L.System.Drawing.FontStyle,
+        cn = L.System.Drawing.StringAlignment;
     {
         let e;
         (R = e = F.H.Order || (F.H.Order = {}))[R["Alignment"] = 1] = "Alignment", R[R["Color"] = 2] = "Color", R[R["Direction"] = 3] = "Direction", R[R["Font"] = 4] = "Font", R[R["Placement"] = 5] = "Placement", R[R["Position"] = 6] = "Position", R[R["Text"] = 7] = "Text", R[R["Visible"] = 8] = "Visible";
         class zg {
             implements() {
                 return zg.ImplementsStiChartAxisTitle || (zg.ImplementsStiChartAxisTitle = [l]), zg.ImplementsStiChartAxisTitle
             }
@@ -3555,15 +3556,15 @@
                 return this.is(e)
             }
             as(e) {
                 if (this.is(e)) return this;
                 return null
             }
             meta() {
-                return [new Rt("Font", "", "Arial", 12, hn.Bold), new n("Text"), new r("Color", "", N.transparent), new i("Alignment", "", mn, mn.Center), new i("Position", "", un, un.Outside), new h("Visible", "", !0)]
+                return [new Rt("Font", "", "Arial", 12, mn.Bold), new n("Text"), new r("Color", "", N.transparent), new i("Alignment", "", cn, cn.Center), new i("Position", "", hn, hn.Outside), new h("Visible", "", !0)]
             }
             saveToJsonObject(e) {
                 return u.saveToJsonObject(e, this)
             }
             loadFromJsonObject(e) {
                 u.loadFromJsonObject(e, this)
             }
@@ -3571,28 +3572,28 @@
                 u.loadFromXml(e, this)
             }
             clone() {
                 let e = this[L.System.StiObject.stimulsoft]().memberwiseClone();
                 return e.font = this.font.clone(), e
             }
             constructor(e, t, r, i, s, n) {
-                this.visible = !0, this.alignment = mn.Center, this.color = N.transparent, this.font = new H("Arial", 12, hn.Bold), this.position = un.Outside, this.text = "", null != e && (this.font = e), null != t && (this.text = t), null != r && (this.color = r), null != i && (this.alignment = i), null != s && (this.position = s), null != n && (this.visible = n)
+                this.visible = !0, this.alignment = cn.Center, this.color = N.transparent, this.font = new H("Arial", 12, mn.Bold), this.position = hn.Outside, this.text = "", null != e && (this.font = e), null != t && (this.text = t), null != r && (this.color = r), null != i && (this.alignment = i), null != s && (this.position = s), null != n && (this.visible = n)
             }
         }
         F.H.StiChartAxisTitle = zg
     }
-    let cn = L.Report.Chart.StiConstantLines_StiTextPosition,
-        dn = L.Report.Dashboard.IStiChartConstantLines;
+    let dn = L.Report.Chart.StiConstantLines_StiTextPosition,
+        gn = L.Report.Dashboard.IStiChartConstantLines;
     {
         class Gg {
             implements() {
-                return Gg.ImplementsStiChartConstantLines || (Gg.ImplementsStiChartConstantLines = [Vt, dn, l]), Gg.ImplementsStiChartConstantLines
+                return Gg.ImplementsStiChartConstantLines || (Gg.ImplementsStiChartConstantLines = [Vt, gn, l]), Gg.ImplementsStiChartConstantLines
             }
             meta() {
-                return [new n("Text"), new r("LineColor"), new i("LineStyle", "", Ri, Ri.Solid), new se("LineWidth", "", 1), new ne("AxisValue", "", "1"), new i("Position", "", cn, cn.LeftTop)]
+                return [new n("Text"), new r("LineColor"), new i("LineStyle", "", Ei, Ei.Solid), new se("LineWidth", "", 1), new ne("AxisValue", "", "1"), new i("Position", "", dn, dn.LeftTop)]
             }
             saveToJsonObject(e) {
                 return u.saveToJsonObject(e, this)
             }
             loadFromJsonObject(e) {
                 u.loadFromJsonObject(e, this)
             }
@@ -3607,28 +3608,28 @@
                 return t.loadFromJsonObject(e), t
             }
             static createFromXml(e) {
                 let t = new Gg;
                 return t.loadFromXml(e), t
             }
             constructor(e, t, r, i, s, n) {
-                this.text = "", this.lineStyle = Ri.Solid, this.lineColor = N.black, this.axisValue = "1", this.lineWidth = 1, this.position = cn.LeftTop, null != e && (this.text = e), null != t && (this.axisValue = t), null != r && (this.lineColor = r), null != i && (this.lineStyle = i), null != s && (this.lineWidth = s), null != n && (this.position = n)
+                this.text = "", this.lineStyle = Ei.Solid, this.lineColor = N.black, this.axisValue = "1", this.lineWidth = 1, this.position = dn.LeftTop, null != e && (this.text = e), null != t && (this.axisValue = t), null != r && (this.lineColor = r), null != i && (this.lineStyle = i), null != s && (this.lineWidth = s), null != n && (this.position = n)
             }
         }
         F.H.StiChartConstantLines = Gg
     }
-    let gn = L.Report.Chart.StiMarkerType,
-        pn = L.Report.Chart.StiExtendedStyleBool;
+    let pn = L.Report.Chart.StiMarkerType,
+        Sn = L.Report.Chart.StiExtendedStyleBool;
     {
         class jn {
             implements() {
                 return jn.ImplementsStiChartMarker || (jn.ImplementsStiChartMarker = [Vt, l]), jn.ImplementsStiChartMarker
             }
             meta() {
-                return [new se("Size", "", 7), new se("Angle", "", 0), new i("Type", "", gn, gn.Circle), new i("Visible", "", pn, pn.FromStyle)]
+                return [new se("Size", "", 7), new se("Angle", "", 0), new i("Type", "", pn, pn.Circle), new i("Visible", "", Sn, Sn.FromStyle)]
             }
             saveToJsonObject(e) {
                 return u.saveToJsonObject(e, this)
             }
             loadFromJsonObject(e) {
                 u.loadFromJsonObject(e, this)
             }
@@ -3643,22 +3644,22 @@
                 return t.loadFromJsonObject(e), t
             }
             static createFromXml(e) {
                 let t = new F.H.StiChartConstantLines;
                 return t.loadFromXml(e), t
             }
             constructor(e) {
-                this.size = 7, this.angle = 0, this.type = gn.Circle, this.visible = pn.FromStyle, null != e && (this.size = e)
+                this.size = 7, this.angle = 0, this.type = pn.Circle, this.visible = Sn.FromStyle, null != e && (this.size = e)
             }
         }
         F.H.StiChartMarker = jn
     }
     F.H.StiChartLegendTitle = class {
         meta() {
-            return [new Rt("Font", "", "Arial", 12, hn.Bold), new n("Text"), new r("Color", "", N.transparent)]
+            return [new Rt("Font", "", "Arial", 12, mn.Bold), new n("Text"), new r("Color", "", N.transparent)]
         }
         saveToJsonObject(e) {
             return u.saveToJsonObject(e, this)
         }
         loadFromJsonObject(e) {
             u.loadFromJsonObject(e, this)
         }
@@ -3666,25 +3667,25 @@
             u.loadFromXml(e, this)
         }
         clone() {
             let e = this[L.System.StiObject.stimulsoft]().memberwiseClone();
             return e.font = this.font.clone(), e
         }
         constructor(e, t, r) {
-            this.color = N.transparent, this.font = new H("Arial", 12, hn.Bold), this.text = "", null != e && (this.font = e), null != t && (this.text = t), null != r && (this.color = r)
+            this.color = N.transparent, this.font = new H("Arial", 12, mn.Bold), this.text = "", null != e && (this.font = e), null != t && (this.text = t), null != r && (this.color = r)
         }
     };
-    let Sn = L.Report.Chart.StiSeriesLabelsValueType;
+    let wn = L.Report.Chart.StiSeriesLabelsValueType;
     {
-        class fn {
+        class yn {
             implements() {
-                return fn.ImplementsStiChartLegendLabels || (fn.ImplementsStiChartLegendLabels = [Vt, ar, ...rr, l]), fn.ImplementsStiChartLegendLabels
+                return yn.ImplementsStiChartLegendLabels || (yn.ImplementsStiChartLegendLabels = [Vt, ar, ...rr, l]), yn.ImplementsStiChartLegendLabels
             }
             meta() {
-                return [new Rt("Font", "", "Arial", 8), new r("Color", "", N.transparent), new i("ValueType", "", Sn)]
+                return [new Rt("Font", "", "Arial", 8), new r("Color", "", N.transparent), new i("ValueType", "", wn)]
             }
             saveToJsonObject(e) {
                 return u.saveToJsonObject(e, this)
             }
             loadFromJsonObject(e) {
                 u.loadFromJsonObject(e, this)
             }
@@ -3695,30 +3696,30 @@
                 let e = this[L.System.StiObject.stimulsoft]().memberwiseClone();
                 return e.font = this.font.clone(), e
             }
             constructor(e, t, r) {
                 this.color = N.transparent, this.font = new H("Arial", 8), this.valueType = null, null != e && (this.font = e), null != t && (this.color = t), null != r && (this.valueType = r)
             }
         }
-        F.H.StiChartLegendLabels = fn
+        F.H.StiChartLegendLabels = yn
     }
-    let wn = L.Report.Chart.StiLegendDirection,
-        bn = F.H.StiChartLegendTitle,
-        fn = F.H.StiChartLegendLabels,
-        yn = L.Report.Chart.StiLegendVertAlignment,
-        Cn = L.Report.Chart.StiLegendHorAlignment;
+    let bn = L.Report.Chart.StiLegendDirection,
+        fn = F.H.StiChartLegendTitle,
+        yn = F.H.StiChartLegendLabels,
+        Cn = L.Report.Chart.StiLegendVertAlignment,
+        xn = L.Report.Chart.StiLegendHorAlignment;
     {
         let e;
         (E = e = F.H.Order || (F.H.Order = {}))[E["HorAlignment"] = 1] = "HorAlignment", E[E["Labels"] = 2] = "Labels", E[E["Title"] = 3] = "Title", E[E["VertAlignment"] = 4] = "VertAlignment";
         class Qn {
             implements() {
                 return Qn.ImplementsStiChartLegend || (Qn.ImplementsStiChartLegend = [l]), Qn.ImplementsStiChartLegend
             }
             meta() {
-                return [new s("Title"), new s("Labels"), new i("HorAlignment", "", Cn, Cn.Left), new i("VertAlignment", "", yn, yn.TopOutside), new h("Visible", "", !0), new i("Visibility", "", F.H.StiLegendVisibility, F.H.StiLegendVisibility.Auto), new i("Direction", "", wn, wn.TopToBottom), new se("Columns")]
+                return [new s("Title"), new s("Labels"), new i("HorAlignment", "", xn, xn.Left), new i("VertAlignment", "", Cn, Cn.TopOutside), new h("Visible", "", !0), new i("Visibility", "", F.H.StiLegendVisibility, F.H.StiLegendVisibility.Auto), new i("Direction", "", bn, bn.TopToBottom), new se("Columns")]
             }
             saveToJsonObject(e) {
                 return u.saveToJsonObject(e, this)
             }
             loadFromJsonObject(e) {
                 u.loadFromJsonObject(e, this)
             }
@@ -3732,117 +3733,117 @@
             get visible() {
                 return this.visibility == F.H.StiLegendVisibility.Auto
             }
             set visible(e) {
                 this.visibility = e ? F.H.StiLegendVisibility.Auto : F.H.StiLegendVisibility.False
             }
             constructor(e, t, r, i, s, n, l) {
-                this.horAlignment = Cn.Left, this.vertAlignment = yn.TopOutside, this.visibility = F.H.StiLegendVisibility.Auto, this.direction = wn.TopToBottom, this.columns = 0, this.labels = new fn, this.title = new bn, null != e && (this.title = e), null != t && (this.labels = t), null != r && (this.horAlignment = r), null != i && (this.vertAlignment = i), null != s && (this.visibility = s), null != n && (this.direction = n), null != l && (this.columns = l)
+                this.horAlignment = xn.Left, this.vertAlignment = Cn.TopOutside, this.visibility = F.H.StiLegendVisibility.Auto, this.direction = bn.TopToBottom, this.columns = 0, this.labels = new yn, this.title = new fn, null != e && (this.title = e), null != t && (this.labels = t), null != r && (this.horAlignment = r), null != i && (this.vertAlignment = i), null != s && (this.visibility = s), null != n && (this.direction = n), null != l && (this.columns = l)
             }
         }
         F.H.StiChartLegend = Qn
     }
-    let xn = L.Report.Chart.StiDirection,
-        Mn = (F.H.StiYChartAxisTitle = class extends F.H.StiChartAxisTitle {
+    let Mn = L.Report.Chart.StiDirection,
+        Tn = (F.H.StiYChartAxisTitle = class extends F.H.StiChartAxisTitle {
             meta() {
-                return [...super.meta(), new i("Direction", "", xn, xn.BottomToTop)]
+                return [...super.meta(), new i("Direction", "", Mn, Mn.BottomToTop)]
             }
             constructor(e, t, r, i, s, n, l) {
-                super(e, t, r, i, n, l), this.direction = xn.BottomToTop, null != s && (this.direction = s)
+                super(e, t, r, i, n, l), this.direction = Mn.BottomToTop, null != s && (this.direction = s)
             }
         }, F.H.StiYChartAxisTitle),
-        Tn = (F.H.StiYChartAxis = class extends F.H.StiChartAxis {
+        Fn = (F.H.StiYChartAxis = class extends F.H.StiChartAxis {
             clone() {
                 var e;
                 let t = super.clone();
                 return t.title = this.title.clone(), t.range = null == (e = this.range) ? void 0 : e.clone(), t
             }
             meta() {
                 return [...super.meta(), new s("Title"), new h("StartFromZero", "", !0)]
             }
             constructor(e, t, r, i) {
-                super(e), this.title = new Mn, this.startFromZero = !0, null != e && (this.labels = e), null != t && (this.title = t), null != r && (this.visible = r), null != i && (this.startFromZero = i)
+                super(e), this.title = new Tn, this.startFromZero = !0, null != e && (this.labels = e), null != t && (this.title = t), null != r && (this.visible = r), null != i && (this.startFromZero = i)
             }
         }, L.Base.StiAutoBool),
-        Fn = (F.H.StiXChartAxis = class extends F.H.StiChartAxis {
+        vn = (F.H.StiXChartAxis = class extends F.H.StiChartAxis {
             clone() {
                 let e = super.clone();
                 return e.title = this.title.clone(), e
             }
             meta() {
-                return [...super.meta(), new s("Title").check(() => null != this.title), new i("ShowEdgeValues", "", Tn, Tn.Auto), new i("StartFromZero", "", Tn, Tn.Auto)]
+                return [...super.meta(), new s("Title").check(() => null != this.title), new i("ShowEdgeValues", "", Fn, Fn.Auto), new i("StartFromZero", "", Fn, Fn.Auto)]
             }
             constructor(e, t, r, i, s) {
-                super(e), this.title = new F.H.StiXChartAxisTitle, this.showEdgeValues = Tn.Auto, this.startFromZero = Tn.Auto, null != e && (this.labels = e), null != t && (this.title = t), null != r && (this.visible = r), null != i && (this.startFromZero = i), null != s && (this.showEdgeValues = s)
+                super(e), this.title = new F.H.StiXChartAxisTitle, this.showEdgeValues = Fn.Auto, this.startFromZero = Fn.Auto, null != e && (this.labels = e), null != t && (this.title = t), null != r && (this.visible = r), null != i && (this.startFromZero = i), null != s && (this.showEdgeValues = s)
             }
         }, F.H.StiYChartMeter = class extends F.e.StiDimensionMeter {
             get localizedName() {
                 return `Y` + b.get("PropertyMain", "Value")
             }
             constructor(e, t, r) {
                 super(e, t, r), this.ident = F.e.StiMeterIdent.YChartMeter
             }
         }, L.Report.Dashboard.IStiChartDashboardInteraction),
-        vn = L.Report.Dashboard.StiInteractionViewsState,
-        An = L.Report.Dashboard.IStiAllowUserSortingDashboardInteraction,
-        In = L.Report.Dashboard.IStiAllowUserDrillDownDashboardInteraction;
+        An = L.Report.Dashboard.StiInteractionViewsState,
+        In = L.Report.Dashboard.IStiAllowUserSortingDashboardInteraction,
+        Dn = L.Report.Dashboard.IStiAllowUserDrillDownDashboardInteraction;
     {
         class zn extends F.g.StiDashboardInteraction {
             implements() {
-                return zn.ImplementsIStiChartDashboardInteraction || (zn.ImplementsIStiChartDashboardInteraction = super.implements().concat([Fn, In, An, l, Gs])), zn.ImplementsIStiChartDashboardInteraction
+                return zn.ImplementsIStiChartDashboardInteraction || (zn.ImplementsIStiChartDashboardInteraction = super.implements().concat([vn, Dn, In, l, Xs])), zn.ImplementsIStiChartDashboardInteraction
             }
             meta() {
-                return [...super.meta(), new h("AllowUserDrillDown"), new h("AllowUserSorting", "", !0), new h("ShowFullScreenButton", "", !0), new h("ShowSaveButton", "", !0), new h("ShowViewDataButton", "", !0), new n("FileName"), new n("HeaderText"), new n("FooterText"), new i("ViewsState", "", vn, vn.OnHover)]
+                return [...super.meta(), new h("AllowUserDrillDown"), new h("AllowUserSorting", "", !0), new h("ShowFullScreenButton", "", !0), new h("ShowSaveButton", "", !0), new h("ShowViewDataButton", "", !0), new n("FileName"), new n("HeaderText"), new n("FooterText"), new i("ViewsState", "", An, An.OnHover)]
             }
             get isDefaultLayout() {
                 return this.showFullScreenButton && this.showSaveButton && this.showViewDataButton && null == this.fileName && null == this.headerText && null == this.footerText
             }
             isDefault() {
                 return this.onHover == Vr.ShowToolTip && this.onClick == kr.ApplyFilter && this.hyperlinkDestination == Nr.NewTab && B.isNullOrEmpty(this.hyperlink) && B.isNullOrEmpty(this.drillDownPageKey) && null != this.drillDownParameters && 0 == this.drillDownParameters.length && B.isNullOrEmpty(this.toolTip) && !this.allowUserDrillDown && this.allowUserSorting && this.isDefaultLayout
             }
             constructor(e, t, r, i, s, n, l, a, o, u, h, m, c, d, g) {
-                super(e, t, r, i, s, n, l), this.ident = Lr.Chart, this.allowUserDrillDown = !1, this.allowUserSorting = !0, this.availableOnClick = Br.ApplyFilter | Br.OpenHyperlink | Br.ShowDashboard | Br.DrillDown, this.availableOnDataManipulation = jr.AllowDrillDown | jr.AllowSorting, this.viewsState = vn.OnHover, this.showFullScreenButton = !0, this.showSaveButton = !0, this.showViewDataButton = !0, this.fileName = null, this.headerText = null, this.footerText = null, null != a && (this.allowUserDrillDown = a), null != o && (this.fileName = o), null != u && (this.headerText = u), null != h && (this.footerText = h), null != m && (this.showFullScreenButton = m), null != c && (this.showSaveButton = c), null != d && (this.showViewDataButton = d), null != g && (this.viewsState = g)
+                super(e, t, r, i, s, n, l), this.ident = Lr.Chart, this.allowUserDrillDown = !1, this.allowUserSorting = !0, this.availableOnClick = Br.ApplyFilter | Br.OpenHyperlink | Br.ShowDashboard | Br.DrillDown, this.availableOnDataManipulation = jr.AllowDrillDown | jr.AllowSorting, this.viewsState = An.OnHover, this.showFullScreenButton = !0, this.showSaveButton = !0, this.showViewDataButton = !0, this.fileName = null, this.headerText = null, this.footerText = null, null != a && (this.allowUserDrillDown = a), null != o && (this.fileName = o), null != u && (this.headerText = u), null != h && (this.footerText = h), null != m && (this.showFullScreenButton = m), null != c && (this.showSaveButton = c), null != d && (this.showViewDataButton = d), null != g && (this.viewsState = g)
             }
         }
         F.g.StiChartDashboardInteraction = zn
     }
-    let Dn = L.Data.Engine.IStiDrillDownElement,
-        Rn = (F.g.StiDrillDownHelper = class {
+    let Rn = L.Data.Engine.IStiDrillDownElement,
+        En = (F.g.StiDrillDownHelper = class {
             static isDrillAvailable(e) {
-                let t = e.is(Qr) ? e.dashboardInteraction.as(In) : null;
+                let t = e.is(Qr) ? e.dashboardInteraction.as(Dn) : null;
                 if (null == t || !t.allowUserDrillDown) return !1;
-                let r = e.as(Dn);
+                let r = e.as(Rn);
                 return null != r
             }
             static isDrillUpAvailable(e) {
                 if (!this.isDrillAvailable(e)) return !1;
-                let t = e.as(Dn);
+                let t = e.as(Rn);
                 return 0 < t.drillDownCurrentLevel
             }
             static isDrillDownAvailable(e) {
                 if (!this.isDrillAvailable(e)) return !1;
-                let t = e.as(Dn);
+                let t = e.as(Rn);
                 return t.drillDownCurrentLevel < t.drillDownLevelCount - 1
             }
             static drillUp(e) {
-                let t = e.as(Dn);
+                let t = e.as(Rn);
                 t.drillDownCurrentLevel--, t.drillDownFilters = t.drillDownFiltersList[t.drillDownCurrentLevel], t.drillDownFiltersList.removeAt(t.drillDownFiltersList.length - 1)
             }
             static drillDown(e, t = null) {
-                let r = e.as(Dn);
+                let r = e.as(Rn);
                 r.drillDownFiltersList.add(r.drillDownFilters), r.drillDownFilters = t, r.drillDownCurrentLevel++
             }
         }, L.Report.Dashboard.StiChartTrendLineType);
     {
         class rl {
             implements() {
-                return rl.ImplementsStiChartTrendLine || (rl.ImplementsStiChartTrendLine = [Vt, dn, l]), rl.ImplementsStiChartTrendLine
+                return rl.ImplementsStiChartTrendLine || (rl.ImplementsStiChartTrendLine = [Vt, gn, l]), rl.ImplementsStiChartTrendLine
             }
             meta() {
-                return [new n("KeyValueMeter"), new i("Type", "", Rn, Rn.None), new i("LineStyle", "", Ri, Ri.Solid), new r("LineColor", "", N.black), new se("LineWidth", "", 1)]
+                return [new n("KeyValueMeter"), new i("Type", "", En, En.None), new i("LineStyle", "", Ei, Ei.Solid), new r("LineColor", "", N.black), new se("LineWidth", "", 1)]
             }
             saveToJsonObject(e) {
                 return u.saveToJsonObject(e, this)
             }
             loadFromJsonObject(e) {
                 u.loadFromJsonObject(e, this)
             }
@@ -3857,26 +3858,25 @@
                 return t.loadFromJsonObject(e), t
             }
             static createFromXml(e) {
                 let t = new rl;
                 return t.loadFromXml(e), t
             }
             constructor(e, t, r, i, s) {
-                this.type = Rn.None, this.lineStyle = Ri.Solid, this.lineColor = N.black, this.lineWidth = 1, null != e && (this.keyValueMeter = e), null != t && (this.type = t), null != r && (this.lineColor = r), null != i && (this.lineStyle = i), null != s && (this.lineWidth = s)
+                this.type = En.None, this.lineStyle = Ei.Solid, this.lineColor = N.black, this.lineWidth = 1, null != e && (this.keyValueMeter = e), null != t && (this.type = t), null != r && (this.lineColor = r), null != i && (this.lineStyle = i), null != s && (this.lineWidth = s)
             }
         }
         F.H.StiChartTrendLine = rl
     }
-    let En = L.Report.Chart.StiColumnShape3D,
-        On = L.Report.Chart.StiPie3dOptions,
-        Vn = L.Report.StiDataMode,
-        kn = L.Report.Dashboard.StiUserViewState,
-        Nn = L.Report.Dashboard.IStiUserViewStates,
-        Ln = L.System.StiArray,
-        Bn = L.Report.Components.StiTextFormatState,
+    let On = L.Report.Chart.StiColumnShape3D,
+        Vn = L.Report.Chart.StiPie3dOptions,
+        kn = L.Report.StiDataMode,
+        Nn = L.Report.Dashboard.StiUserViewState,
+        Ln = L.Report.Dashboard.IStiUserViewStates,
+        Bn = L.System.StiArray,
         Pn = L.Report.Dashboard.StiChartSeriesCreator,
         jn = F.H.StiChartMarker,
         Hn = F.g.StiDrillDownHelper,
         zn = F.g.StiChartDashboardInteraction,
         Gn = L.Report.Dashboard.IStiNegativeSeriesColors,
         Xn = L.Report.Dashboard.IStiParetoSeriesColors,
         Wn = L.Report.Dashboard.ImplementsIStiSeriesColors,
@@ -3890,73 +3890,74 @@
         _n = F.H.StiYChartMeter,
         $n = L.Report.Dashboard.StiChartGroups,
         el = L.Report.Dashboard.IStiChartElement,
         tl = L.Data.Engine.ImplementsIStiDrillDownElement,
         rl = F.H.StiChartTrendLine,
         il = L.Report.Chart.IStiShowNullsSeries;
     {
+        let t = L.Report.Components.StiTextFormatState;
         dt.add("StiChartElement", "Stimulsoft.Dashboard.Export.Tools.StiChartElementExportTool");
         class Am extends F.e.StiElement {
             implements() {
-                return Am.ImplementsStiChartElement || (Am.ImplementsStiChartElement = super.implements().concat([el, Ke, Ze, Nn, ye, Oe, qs, Ne, Us, Gn, Xn, Xs, ...Kn, ...Qe, ...Ue, ...Zn, ...Yn, ...$s, ...Qs, ...Wn, ...Jn, ...Un, ...tl, l, Qr, Dn])), Am.ImplementsStiChartElement
+                return Am.ImplementsStiChartElement || (Am.ImplementsStiChartElement = super.implements().concat([el, Ke, Ze, Ln, ye, Oe, _s, Ne, Zs, Gn, Xn, Ws, ...Kn, ...Qe, ...Ue, ...Zn, ...Yn, ...en, ...qs, ...Wn, ...Jn, ...Un, ...tl, l, Qr, Rn])), Am.ImplementsStiChartElement
             }
             clone(e) {
                 var t, r, i, s, n;
                 let l = super.clone(e);
                 return l.values = this.values.select(e => e.clone()).toList(), l.endValues = this.endValues.select(e => e.clone()).toList(), l.closeValues = this.closeValues.select(e => e.clone()).toList(), l.lowValues = this.lowValues.select(e => e.clone()).toList(), l.highValues = this.highValues.select(e => e.clone()).toList(), l.arguments = this.arguments.select(e => e.clone()).toList(), l.weights = this.weights.select(e => e.clone()).toList(), l.series = null != this.series ? this.series.clone() : null, l.sortBy = null != this.sortBy ? this.sortBy.clone() : null, l.indicatorValue = null == (t = this.indicatorValue) ? void 0 : t.clone(), l.userFilters = this.userFilters.select(e => e.clone()).toList(), l.userSorts = this.userSorts.select(e => e.clone()).toList(), l.userViewStates = this.userViewStates.select(e => e.clone()).toList(), l.transformActions = this.transformActions.select(e => e.clone()).toList(), l.transformFilters = this.transformFilters.select(e => e.clone()).toList(), l.transformSorts = this.transformSorts.select(e => e.clone()).toList(), l.dataFilters = this.dataFilters.select(e => e.clone()).toList(), l.topN = this.topN.clone(), l.argumentFormat = null != this.argumentFormat ? this.argumentFormat.clone() : null, l.valueFormat = null != this.valueFormat ? this.valueFormat.clone() : null, l.title = null != this.title ? this.title.clone() : null, l.layout = null != this.layout ? this.layout.clone() : null, l.dashboardInteraction = this.dashboardInteraction.clone(), l.xAxis = null != this.xAxis ? this.xAxis.clone() : null, l.xTopAxis = null == (r = this.xTopAxis) ? void 0 : r.clone(), l.yAxis = null != this.yAxis ? this.yAxis.clone() : null, l.yRightAxis = null == (i = this.yRightAxis) ? void 0 : i.clone(), l.legend = null != this.legend ? this.legend.clone() : null, l.area = null != this.area ? this.area.clone() : null, l.seriesColors = null != this.seriesColors ? this.seriesColors[L.System.StiObject.stimulsoft]().clone() : null, l.negativeSeriesColors = null != this.negativeSeriesColors ? this.negativeSeriesColors[L.System.StiObject.stimulsoft]().clone() : null, l.paretoSeriesColors = null != this.paretoSeriesColors ? this.paretoSeriesColors[L.System.StiObject.stimulsoft]().clone() : null, l.marker = null != this.marker ? this.marker.clone() : null, l.constantLines = this.constantLines.select(e => e.clone()).toList(), l.trendLines = this.trendLines.select(e => e.clone()).toList(), l.chartConditions = this.chartConditions.select(e => e.clone()).toList(), l.shadow = null == (s = this.shadow) ? void 0 : s.clone(), l.cornerRadius = null == (n = this.cornerRadius) ? void 0 : n.clone(), l
             }
             meta() {
-                return [...super.meta(), new s("UserFilters").get(e => a.Serialize.objectArray(this.userFilters, e)).set(e => this.userFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.userFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new s("UserSorts").get(e => a.Serialize.objectArray(this.userSorts, e)).set(e => this.userSorts.addRange(e.value.properties().select(e => rn.loadFromJson(e.value)))).setXml(e => this.userSorts.addRange(e.childNodes.select(e => rn.loadFromXml(e)))), new s("TransformActions").get(e => a.Serialize.objectArray(this.transformActions, e)).set(e => this.transformActions.addRange(e.value.properties().select(e => sn.loadFromJson(e.value)))).setXml(e => this.transformActions.addRange(e.childNodes.select(e => sn.loadFromXml(e)))), new s("TransformFilters").get(e => a.Serialize.objectArray(this.transformFilters, e)).set(e => this.transformFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.transformFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new s("TransformSorts").get(e => a.Serialize.objectArray(this.transformSorts, e)).set(e => this.transformSorts.addRange(e.value.properties().select(e => rn.loadFromJson(e.value)))).setXml(e => this.transformSorts.addRange(e.childNodes.select(e => rn.loadFromXml(e)))), new s("DataFilters").get(e => a.Serialize.objectArray(this.dataFilters, e)).set(e => this.dataFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.dataFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new s("Values").get(e => a.Serialize.objectArray(this.values, e)).set(e => this.values.addRange(e.value.properties().select(e => g.loadFromJson(e.value)))).setXml(e => this.values.addRange(e.childNodes.select(e => g.loadFromXml(e)))), new s("EndValues").get(e => a.Serialize.objectArray(this.endValues, e)).set(e => this.endValues.addRange(e.value.properties().select(e => g.loadFromJson(e.value)))).setXml(e => this.endValues.addRange(e.childNodes.select(e => g.loadFromXml(e)))), new s("CloseValues").get(e => a.Serialize.objectArray(this.closeValues, e)).set(e => this.closeValues.addRange(e.value.properties().select(e => g.loadFromJson(e.value)))).setXml(e => this.closeValues.addRange(e.childNodes.select(e => g.loadFromXml(e)))), new s("LowValues").get(e => a.Serialize.objectArray(this.lowValues, e)).set(e => this.lowValues.addRange(e.value.properties().select(e => g.loadFromJson(e.value)))).setXml(e => this.lowValues.addRange(e.childNodes.select(e => g.loadFromXml(e)))), new s("HighValues").get(e => a.Serialize.objectArray(this.highValues, e)).set(e => this.highValues.addRange(e.value.properties().select(e => g.loadFromJson(e.value)))).setXml(e => this.highValues.addRange(e.childNodes.select(e => g.loadFromXml(e)))), new s("Arguments").get(e => a.Serialize.objectArray(this.arguments, e)).set(e => this.arguments.addRange(e.value.properties().select(e => g.loadFromJson(e.value)))).setXml(e => this.arguments.addRange(e.childNodes.select(e => g.loadFromXml(e)))), new s("Weights").get(e => a.Serialize.objectArray(this.weights, e)).set(e => this.weights.addRange(e.value.properties().select(e => g.loadFromJson(e.value)))).setXml(e => this.weights.addRange(e.childNodes.select(e => g.loadFromXml(e)))), new s("UserViewStates").get(e => a.Serialize.objectArray(this.userViewStates, e)).set(e => this.userViewStates.addRange(e.value.properties().select(e => kn.loadFromJson(e.value)))).setXml(e => this.userViewStates.addRange(e.childNodes.select(e => kn.loadFromXml(e)))), new h("ColorEach"), new h("CrossFiltering", "", !0), new s("TopN").check(() => null != this.topN).set(e => this.topN = Fi.createFromJsonObject(e.value)).setXml(e => this.topN = Fi.createFromXml(e)), new s("DashboardInteraction").check(() => null != this.dashboardInteraction.as(zn)).set(e => {
+                return [...super.meta(), new s("UserFilters").get(e => a.Serialize.objectArray(this.userFilters, e)).set(e => this.userFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.userFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new s("UserSorts").get(e => a.Serialize.objectArray(this.userSorts, e)).set(e => this.userSorts.addRange(e.value.properties().select(e => sn.loadFromJson(e.value)))).setXml(e => this.userSorts.addRange(e.childNodes.select(e => sn.loadFromXml(e)))), new s("TransformActions").get(e => a.Serialize.objectArray(this.transformActions, e)).set(e => this.transformActions.addRange(e.value.properties().select(e => nn.loadFromJson(e.value)))).setXml(e => this.transformActions.addRange(e.childNodes.select(e => nn.loadFromXml(e)))), new s("TransformFilters").get(e => a.Serialize.objectArray(this.transformFilters, e)).set(e => this.transformFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.transformFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new s("TransformSorts").get(e => a.Serialize.objectArray(this.transformSorts, e)).set(e => this.transformSorts.addRange(e.value.properties().select(e => sn.loadFromJson(e.value)))).setXml(e => this.transformSorts.addRange(e.childNodes.select(e => sn.loadFromXml(e)))), new s("DataFilters").get(e => a.Serialize.objectArray(this.dataFilters, e)).set(e => this.dataFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.dataFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new s("Values").get(e => a.Serialize.objectArray(this.values, e)).set(e => this.values.addRange(e.value.properties().select(e => g.loadFromJson(e.value)))).setXml(e => this.values.addRange(e.childNodes.select(e => g.loadFromXml(e)))), new s("EndValues").get(e => a.Serialize.objectArray(this.endValues, e)).set(e => this.endValues.addRange(e.value.properties().select(e => g.loadFromJson(e.value)))).setXml(e => this.endValues.addRange(e.childNodes.select(e => g.loadFromXml(e)))), new s("CloseValues").get(e => a.Serialize.objectArray(this.closeValues, e)).set(e => this.closeValues.addRange(e.value.properties().select(e => g.loadFromJson(e.value)))).setXml(e => this.closeValues.addRange(e.childNodes.select(e => g.loadFromXml(e)))), new s("LowValues").get(e => a.Serialize.objectArray(this.lowValues, e)).set(e => this.lowValues.addRange(e.value.properties().select(e => g.loadFromJson(e.value)))).setXml(e => this.lowValues.addRange(e.childNodes.select(e => g.loadFromXml(e)))), new s("HighValues").get(e => a.Serialize.objectArray(this.highValues, e)).set(e => this.highValues.addRange(e.value.properties().select(e => g.loadFromJson(e.value)))).setXml(e => this.highValues.addRange(e.childNodes.select(e => g.loadFromXml(e)))), new s("Arguments").get(e => a.Serialize.objectArray(this.arguments, e)).set(e => this.arguments.addRange(e.value.properties().select(e => g.loadFromJson(e.value)))).setXml(e => this.arguments.addRange(e.childNodes.select(e => g.loadFromXml(e)))), new s("Weights").get(e => a.Serialize.objectArray(this.weights, e)).set(e => this.weights.addRange(e.value.properties().select(e => g.loadFromJson(e.value)))).setXml(e => this.weights.addRange(e.childNodes.select(e => g.loadFromXml(e)))), new s("UserViewStates").get(e => a.Serialize.objectArray(this.userViewStates, e)).set(e => this.userViewStates.addRange(e.value.properties().select(e => Nn.loadFromJson(e.value)))).setXml(e => this.userViewStates.addRange(e.childNodes.select(e => Nn.loadFromXml(e)))), new h("ColorEach"), new h("CrossFiltering", "", !0), new s("TopN").check(() => null != this.topN).set(e => this.topN = vi.createFromJsonObject(e.value)).setXml(e => this.topN = vi.createFromXml(e)), new s("DashboardInteraction").check(() => null != this.dashboardInteraction.as(zn)).set(e => {
                     var t;
                     let r = null == (t = qr.loadInteractionFromJsonObject(e.value)) ? void 0 : t.as(zn);
                     null != r && (this.dashboardInteraction = r)
                 }).setXml(e => {
                     var t;
                     let r = null == (t = qr.loadInteractionFromXml(e)) ? void 0 : t.as(zn);
                     null != r && (this.dashboardInteraction = r)
-                }), new s("Title").check(() => null != this.title).set(e => this.title = qn.createFromJsonObject(e.value)).setXml(e => this.title = qn.createFromXml(e)), new s("Layout").check(() => null != this.layout).set(e => this.layout = _s.createFromJsonObject(e.value)).setXml(e => this.layout = _s.createFromXml(e)), new s("ManuallyEnteredChartMeter").check(() => null != this.manuallyEnteredChartMeter).set(e => {
+                }), new s("Title").check(() => null != this.title).set(e => this.title = qn.createFromJsonObject(e.value)).setXml(e => this.title = qn.createFromXml(e)), new s("Layout").check(() => null != this.layout).set(e => this.layout = $s.createFromJsonObject(e.value)).setXml(e => this.layout = $s.createFromXml(e)), new s("ManuallyEnteredChartMeter").check(() => null != this.manuallyEnteredChartMeter).set(e => {
                     let t = g.loadFromJson(e.value).as(F.H.StiValueChartMeter);
                     null != t && (this.manuallyEnteredChartMeter = t)
                 }).setXml(e => {
                     let t = g.loadFromXml(e).as(F.H.StiValueChartMeter);
                     null != t && (this.manuallyEnteredChartMeter = t)
                 }), new s("Series").check(() => null != this.series).set(e => {
-                    let t = g.loadFromJson(e.value).as(Ps);
+                    let t = g.loadFromJson(e.value).as(js);
                     null != t && (this.series = t)
                 }).setXml(e => {
-                    let t = g.loadFromXml(e).as(Ps);
+                    let t = g.loadFromXml(e).as(js);
                     null != t && (this.series = t)
                 }), new s("SortBy").check(() => null != this.sortBy).set(e => {
                     let t = g.loadFromJson(e.value).as(F.H.StiSortByChartMeter);
                     null != t && (this.sortBy = t)
                 }).setXml(e => {
                     let t = g.loadFromXml(e).as(F.H.StiSortByChartMeter);
                     null != t && (this.sortBy = t)
                 }), new s("IndicatorValue").check(() => null != this.indicatorValue).set(e => {
                     let t = g.loadFromJson(e.value).as(F.H.StiIndicatorValueChartMeter);
                     null != t && (this.indicatorValue = t)
                 }).setXml(e => {
                     let t = g.loadFromXml(e).as(F.H.StiIndicatorValueChartMeter);
                     null != t && (this.indicatorValue = t)
-                }), new s("ArgumentFormat").check(() => null != this.argumentFormat).set(e => this.argumentFormat = br.createFromJsonObject(e.value)).setXml(e => this.argumentFormat = br.loadFormatFromXml(e, this.report)), new s("ValueFormat").check(() => null != this.valueFormat).set(e => this.valueFormat = br.createFromJsonObject(e.value)).setXml(e => this.valueFormat = br.loadFormatFromXml(e, this.report)), new s("XAxis").check(() => null != this.xAxis), new s("XTopAxis").check(() => null != this.xTopAxis), new s("YAxis").check(() => null != this.yAxis), new s("YRightAxis").check(() => null != this.yRightAxis), new s("Legend").check(() => null != this.legend), new s("Area").check(() => null != this.area), new s("Marker").check(() => null != this.marker), new s("Labels").check(() => null != this.labels), new s("Options3D").check(() => null != this.options3D), new s("SeriesColors").get(() => a.Serialize.colorArray(this.seriesColors)).set(e => this.seriesColors = a.Deserialize.colorArray(e.value)).setXml(e => this.seriesColors = Js.convertStringToColorArray(e.textContent)), new s("NegativeSeriesColors").get(() => a.Serialize.colorArray(this.negativeSeriesColors)).set(e => this.negativeSeriesColors = a.Deserialize.colorArray(e.value)).setXml(e => this.negativeSeriesColors = Js.convertStringToColorArray(e.textContent)), new s("ParetoSeriesColors").get(() => a.Serialize.colorArray(this.paretoSeriesColors)).set(e => this.paretoSeriesColors = a.Deserialize.colorArray(e.value)).setXml(e => this.paretoSeriesColors = Js.convertStringToColorArray(e.textContent)), new i("Style", "", o, o.Auto), new n("Group"), new n("CustomStyleName"), new s("ConstantLines").get(e => a.Serialize.objectArray(this.constantLines, e)).set(e => this.constantLines.addRange(e.value.properties().select(e => F.H.StiChartConstantLines.createFromJson(e.value)))).setXml(e => this.constantLines.addRange(e.childNodes.select(e => F.H.StiChartConstantLines.createFromXml(e)))), new s("TrendLines").get(e => a.Serialize.objectArray(this.trendLines, e)).set(e => this.trendLines.addRange(e.value.properties().select(e => rl.createFromJson(e.value)))).setXml(e => this.trendLines.addRange(e.childNodes.select(e => rl.createFromXml(e)))), new s("ChartConditions").get(e => a.Serialize.objectArray(this.chartConditions, e)).set(e => this.chartConditions.addRange(e.value.properties().select(e => F.H.StiChartElementCondition.createFromJson(e.value)))).setXml(e => this.chartConditions.addRange(e.childNodes.select(e => F.H.StiChartElementCondition.createFromXml(e)))), new n("CornerRadius").get(() => this.cornerRadius.toString()).set(e => this.cornerRadius = m.tryParse(e.value.toString())).setXml(e => this.cornerRadius = m.tryParse(e.textContent)), new n("Shadow").get(() => a.Serialize.jShadow(this.shadow)).set(e => this.shadow = a.Deserialize.simpleSahdow(e.value)).setXml(e => this.shadow = Ye.loadFromXml(e.textContent)), new i("DataMode", "", Vn, Vn.UsingDataFields), new n("ManuallyEnteredData"), new i("Icon", "", kt).check(() => null != this.icon), new h("RoundValues", "", !0), new n("SelectedViewStateKey").check(() => null != this.selectedViewStateKey), new i("ColumnShape", "", En, En.Box), new h("ShowBlanks")]
+                }), new s("ArgumentFormat").check(() => null != this.argumentFormat).set(e => this.argumentFormat = br.createFromJsonObject(e.value)).setXml(e => this.argumentFormat = br.loadFormatFromXml(e, this.report)), new s("ValueFormat").check(() => null != this.valueFormat).set(e => this.valueFormat = br.createFromJsonObject(e.value)).setXml(e => this.valueFormat = br.loadFormatFromXml(e, this.report)), new s("XAxis").check(() => null != this.xAxis), new s("XTopAxis").check(() => null != this.xTopAxis), new s("YAxis").check(() => null != this.yAxis), new s("YRightAxis").check(() => null != this.yRightAxis), new s("Legend").check(() => null != this.legend), new s("Area").check(() => null != this.area), new s("Marker").check(() => null != this.marker), new s("Labels").check(() => null != this.labels), new s("Options3D").check(() => null != this.options3D), new s("SeriesColors").get(() => a.Serialize.colorArray(this.seriesColors)).set(e => this.seriesColors = a.Deserialize.colorArray(e.value)).setXml(e => this.seriesColors = Us.convertStringToColorArray(e.textContent)), new s("NegativeSeriesColors").get(() => a.Serialize.colorArray(this.negativeSeriesColors)).set(e => this.negativeSeriesColors = a.Deserialize.colorArray(e.value)).setXml(e => this.negativeSeriesColors = Us.convertStringToColorArray(e.textContent)), new s("ParetoSeriesColors").get(() => a.Serialize.colorArray(this.paretoSeriesColors)).set(e => this.paretoSeriesColors = a.Deserialize.colorArray(e.value)).setXml(e => this.paretoSeriesColors = Us.convertStringToColorArray(e.textContent)), new i("Style", "", o, o.Auto), new n("Group"), new n("CustomStyleName"), new s("ConstantLines").get(e => a.Serialize.objectArray(this.constantLines, e)).set(e => this.constantLines.addRange(e.value.properties().select(e => F.H.StiChartConstantLines.createFromJson(e.value)))).setXml(e => this.constantLines.addRange(e.childNodes.select(e => F.H.StiChartConstantLines.createFromXml(e)))), new s("TrendLines").get(e => a.Serialize.objectArray(this.trendLines, e)).set(e => this.trendLines.addRange(e.value.properties().select(e => rl.createFromJson(e.value)))).setXml(e => this.trendLines.addRange(e.childNodes.select(e => rl.createFromXml(e)))), new s("ChartConditions").get(e => a.Serialize.objectArray(this.chartConditions, e)).set(e => this.chartConditions.addRange(e.value.properties().select(e => F.H.StiChartElementCondition.createFromJson(e.value)))).setXml(e => this.chartConditions.addRange(e.childNodes.select(e => F.H.StiChartElementCondition.createFromXml(e)))), new n("CornerRadius").get(() => this.cornerRadius.toString()).set(e => this.cornerRadius = m.tryParse(e.value.toString())).setXml(e => this.cornerRadius = m.tryParse(e.textContent)), new n("Shadow").get(() => a.Serialize.jShadow(this.shadow)).set(e => this.shadow = a.Deserialize.simpleSahdow(e.value)).setXml(e => this.shadow = Ye.loadFromXml(e.textContent)), new i("DataMode", "", kn, kn.UsingDataFields), new n("ManuallyEnteredData"), new i("Icon", "", kt).check(() => null != this.icon), new h("RoundValues", "", !0), new n("SelectedViewStateKey").check(() => null != this.selectedViewStateKey), new i("ColumnShape", "", On, On.Box), new h("ShowBlanks")]
             }
             convertToBubble() {
                 null != this.arguments && this.arguments.where(e => null != e).toList().forEach(e => {
-                    e.expression = Rs.replaceFunction(e.expression, "Sum")
+                    e.expression = Es.replaceFunction(e.expression, "Sum")
                 })
             }
             convertFromBubble() {
                 null != this.arguments && this.arguments.where(e => null != e).toList().forEach(e => {
-                    e.expression = Rs.removeFunction(e.expression)
+                    e.expression = Es.removeFunction(e.expression)
                 }), null != this.weights && this.weights.clear()
             }
             convertToGantt() {
                 var e;
                 null != this.values && null != (e = this.values) && e.where(e => null != e).toList().forEach(e => {
-                    e.expression = Rs.removeFunction(e.expression)
+                    e.expression = Es.removeFunction(e.expression)
                 })
             }
             getChartSeriesTypes(r) {
                 let i = new P;
                 if (1 < this.values.length) {
                     let e = ve.parse(c, r),
                         t = $n.getGroup(e);
@@ -4018,25 +4019,25 @@
             getEndValue(e) {
                 return null != e ? d.Chart.getEndValue(e.as(F.e.StiMeter)) : null
             }
             getEndValueByIndex(e) {
                 return e < this.endValues.length ? this.endValues[e] : null
             }
             insertEndValue(e, t) {
-                let r = t.as(js);
+                let r = t.as(Hs);
                 null != r && (0 <= e && e < this.endValues.length ? this.endValues.insert(e, r) : this.endValues.add(r))
             }
             removeEndValue(e) {
                 e < this.endValues.length && this.endValues.removeAt(e)
             }
             removeAllEndValues() {
                 this.endValues.clear()
             }
             createNewEndValue() {
-                let e = new js;
+                let e = new Hs;
                 return e.expression = "Sum()", this.endValues.add(e), e
             }
             addCloseValue(e) {
                 null != e && this.closeValues.add(d.Chart.getCloseValue2(e))
             }
             getCloseValue2(e) {
                 return null != e ? d.Chart.getCloseValue2(e) : null
@@ -4044,25 +4045,25 @@
             getCloseValue(e) {
                 return null != e ? d.Chart.getCloseValue(e.as(F.e.StiMeter)) : null
             }
             getCloseValueByIndex(e) {
                 return e < this.closeValues.length ? this.closeValues[e] : null
             }
             insertCloseValue(e, t) {
-                let r = t.as(Vs);
+                let r = t.as(ks);
                 null != r && (0 <= e && e < this.closeValues.length ? this.closeValues.insert(e, r) : this.closeValues.add(r))
             }
             removeCloseValue(e) {
                 e < this.closeValues.length && this.closeValues.removeAt(e)
             }
             removeAllCloseValues() {
                 this.closeValues.clear()
             }
             createNewCloseValue() {
-                let e = new Vs;
+                let e = new ks;
                 return e.expression = "Sum()", this.closeValues.add(e), e
             }
             addLowValue(e) {
                 null != e && this.lowValues.add(d.Chart.getLowValue2(e))
             }
             getLowValue2(e) {
                 return null != e ? d.Chart.getLowValue2(e) : null
@@ -4070,25 +4071,25 @@
             getLowValue(e) {
                 return null != e ? d.Chart.getLowValue(e.as(F.e.StiMeter)) : null
             }
             getLowValueByIndex(e) {
                 return e < this.lowValues.length ? this.lowValues[e] : null
             }
             insertLowValue(e, t) {
-                let r = t.as(ks);
+                let r = t.as(Ns);
                 null != r && (0 <= e && e < this.lowValues.length ? this.lowValues.insert(e, r) : this.lowValues.add(r))
             }
             removeLowValue(e) {
                 e < this.lowValues.length && this.lowValues.removeAt(e)
             }
             removeAllLowValues() {
                 this.lowValues.clear()
             }
             createNewLowValue() {
-                let e = new ks;
+                let e = new Ns;
                 return e.expression = "Sum()", this.lowValues.add(e), e
             }
             addHighalue(e) {
                 null != e && this.highValues.add(d.Chart.getHighValue2(e))
             }
             getHighValue2(e) {
                 return null != e ? d.Chart.getHighValue2(e) : null
@@ -4096,25 +4097,25 @@
             getHighValue(e) {
                 return null != e ? d.Chart.getHighValue(e.as(F.e.StiMeter)) : null
             }
             getHighValueByIndex(e) {
                 return e < this.highValues.length ? this.highValues[e] : null
             }
             insertHighValue(e, t) {
-                let r = t.as(Ns);
+                let r = t.as(Ls);
                 null != r && (0 <= e && e < this.highValues.length ? this.highValues.insert(e, r) : this.highValues.add(r))
             }
             removeHighValue(e) {
                 e < this.highValues.length && this.highValues.removeAt(e)
             }
             removeAllHighValues() {
                 this.highValues.clear()
             }
             createNewHighValue() {
-                let e = new Ns;
+                let e = new Ls;
                 return e.expression = "Sum()", this.highValues.add(e), e
             }
             addArgument(e) {
                 null != e && this.arguments.add(d.Chart.getArgument2(e))
             }
             getArgument2(e) {
                 return null != e ? d.Chart.getArgument2(e) : null
@@ -4125,50 +4126,50 @@
             fetchAllArguments() {
                 return this.arguments.cast().toList()
             }
             getArgumentByIndex(e) {
                 return e < this.arguments.length ? this.arguments[e] : null
             }
             insertArgument(e, t) {
-                let r = t.as(Ls);
+                let r = t.as(Bs);
                 null != r && (0 <= e && e < this.arguments.length ? this.arguments.insert(e, r) : this.arguments.add(r))
             }
             removeArgument(e) {
                 e < this.arguments.length && this.arguments.removeAt(e)
             }
             removeAllArguments() {
                 this.arguments.clear()
             }
             createNewArgument() {
-                this.arguments.add(new Ls)
+                this.arguments.add(new Bs)
             }
             addWeight(e) {
                 null != e && this.weights.add(d.Chart.getWeight2(e))
             }
             getWeight2(e) {
                 return null != e ? d.Chart.getWeight2(e) : null
             }
             getWeight(e) {
                 return null != e ? d.Chart.getWeight(e.as(F.e.StiMeter)) : null
             }
             getWeightByIndex(e) {
                 return e < this.weights.length ? this.weights[e] : null
             }
             insertWeight(e, t) {
-                let r = t.as(Es);
+                let r = t.as(Os);
                 null != r && (0 <= e && e < this.weights.length ? this.weights.insert(e, r) : this.weights.add(r))
             }
             removeWeight(e) {
                 e < this.weights.length && this.weights.removeAt(e)
             }
             removeAllWeights() {
                 this.weights.clear()
             }
             createNewWeight() {
-                let e = new Es;
+                let e = new Os;
                 e.expression = "Sum()", this.weights.add(e)
             }
             addSeries(e) {
                 this.series = null != e ? d.Chart.getSeries2(e) : null
             }
             getSeries2(e) {
                 return null != e ? d.Chart.getSeries2(e) : null
@@ -4176,21 +4177,21 @@
             getSeries(e) {
                 return null != e ? d.Chart.getSeries(e.as(F.e.StiMeter)) : null
             }
             getSeries3() {
                 return this.series
             }
             insertSeries(e) {
-                this.series = e.as(Ps)
+                this.series = e.as(js)
             }
             removeSeries() {
                 this.series = null
             }
             createNewSeries() {
-                this.series = new Ps
+                this.series = new js
             }
             addSortBy(e) {
                 this.sortBy = null != e ? d.Chart.getSortBy2(e) : null
             }
             getSortBy2(e) {
                 return null != e ? d.Chart.getSortBy2(e) : null
             }
@@ -4265,46 +4266,46 @@
             }
             clearChartConditions() {
                 this.chartConditions.clear()
             }
             convertFrom(e) {
                 let t = e.fetchAllMeters();
                 if (this.values.clear(), this.arguments.clear(), null == t) return;
-                t.where(e => (e.is2(Er) || e.is2(vt)) && !e.is2(Ii)).cast().forEach(e => {
+                t.where(e => (e.is2(Er) || e.is2(vt)) && !e.is2(Di)).cast().forEach(e => {
                     let t = new F.H.StiValueChartMeter;
                     t.loadFromJsonObject(e.saveToJsonObject(je.Report)), this.values.add(t)
-                }, this), t.where(e => e.is(Ii)).cast().forEach(e => {
-                    let t = new Ls;
+                }, this), t.where(e => e.is(Di)).cast().forEach(e => {
+                    let t = new Bs;
                     t.loadFromJsonObject(e.saveToJsonObject(je.Report)), this.arguments.add(t)
                 }, this), null == this.dashboardInteraction && (this.dashboardInteraction = new zn)
             }
             fetchAllMeters() {
                 let e = new P;
-                return this.dataMode == Vn.UsingDataFields && (null != this.values && e.addRange(this.values), null != this.endValues && e.addRange(this.endValues), null != this.closeValues && e.addRange(this.closeValues), null != this.lowValues && e.addRange(this.lowValues), null != this.highValues && e.addRange(this.highValues), null != this.arguments && e.addRange(this.arguments), null != this.weights && e.addRange(this.weights), null != this.series && e.add(this.series), null != this.sortBy && e.add(this.sortBy), null != this.indicatorValue) && e.add(this.indicatorValue), e
+                return this.dataMode == kn.UsingDataFields && (null != this.values && e.addRange(this.values), null != this.endValues && e.addRange(this.endValues), null != this.closeValues && e.addRange(this.closeValues), null != this.lowValues && e.addRange(this.lowValues), null != this.highValues && e.addRange(this.highValues), null != this.arguments && e.addRange(this.arguments), null != this.weights && e.addRange(this.weights), null != this.series && e.add(this.series), null != this.sortBy && e.add(this.sortBy), null != this.indicatorValue) && e.add(this.indicatorValue), e
             }
             getMeters() {
                 let i = new P;
-                if (this.dataMode == Vn.UsingDataFields) {
+                if (this.dataMode == kn.UsingDataFields) {
                     for (let r of this.values)
                         if (this.isBubbleChart) {
                             let e = new _n;
                             e.key = r.key, e.expression = r.expression, e.label = r.label, i.add(e)
                         } else if (this.isFinancial) {
                         let e = new F.H.StiOpenValueChartMeter;
                         e.seriesType = r.seriesType, e.key = r.key, e.expression = r.expression, e.label = r.label, i.add(e)
                     } else if (this.isRange) {
                         let e = new F.H.StiStartValueChartMeter;
                         e.seriesType = r.seriesType, e.key = r.key, e.expression = r.expression, e.label = r.label, e.lineStyle = r.lineStyle, e.showNulls = r.showNulls, i.add(e)
                     } else if (r.showZeros == Ct.Zero && r.showNulls == Ct.Zero || !Pn.neww2(r.seriesType).is(il)) i.add(r);
                     else {
-                        let e = Rs.getFunction(r.expression),
+                        let e = Es.getFunction(r.expression),
                             t = null;
                         if ("sum" == (e = null != e ? e.toLowerCase() : e) ? t = "sumnulls" : "avg" == e && (t = "avgnulls"), null != t) {
                             let e = r.clone();
-                            e.expression = Rs.replaceFunction(r.expression, t), i.add(e)
+                            e.expression = Es.replaceFunction(r.expression, t), i.add(e)
                         } else i.add(r)
                     }
                     if (this.isRange)
                         for (let e of this.endValues) i.add(e);
                     if (this.isFinancial)
                         for (let e of this.closeValues) i.add(e);
                     if (this.isFinancial)
@@ -4321,18 +4322,18 @@
                         for (let e of this.weights) i.add(e);
                     null != this.series && i.add(this.series), null != this.sortBy && i.add(this.sortBy), null != this.indicatorValue && i.add(this.indicatorValue)
                 }
                 return i
             }
             retrieveUsedDataNames() {
                 let e = new P;
-                return this.dataMode == Vn.UsingDataFields && (e.addRange(en.getMany2(this.values)), e.addRange(en.getMany2(this.arguments)), e.addRange(en.getMany2(this.weights)), e.addRange(en.getMany(this.series)), e.addRange(en.getMany(this.sortBy)), e.addRange(en.getMany(this.indicatorValue))), e.distinct()
+                return this.dataMode == kn.UsingDataFields && (e.addRange(tn.getMany2(this.values)), e.addRange(tn.getMany2(this.arguments)), e.addRange(tn.getMany2(this.weights)), e.addRange(tn.getMany(this.series)), e.addRange(tn.getMany(this.sortBy)), e.addRange(tn.getMany(this.indicatorValue))), e.distinct()
             }
             get isDefined() {
-                return null != this.values && 0 < this.values.length || null != this.weights && 0 < this.weights.length && this.isBubbleChart || null != this.arguments && 0 < this.arguments.length || null != this.series || this.dataMode == Vn.ManuallyEnteringData
+                return null != this.values && 0 < this.values.length || null != this.weights && 0 < this.weights.length && this.isBubbleChart || null != this.arguments && 0 < this.arguments.length || null != this.series || this.dataMode == kn.ManuallyEnteringData
             }
             get allowSkipOwnFilter() {
                 return !0
             }
             get style() {
                 return this._style
             }
@@ -4456,15 +4457,15 @@
             getAllStrings() {
                 let t = ["Title.Text", "Legend.Title.Text"],
                     r = (this.isAxisAreaChart && (t.push("XAxis.Labels.TextAfter"), t.push("XAxis.Labels.TextBefore"), t.push("XAxis.Title.Text"), t.push("XTopAxis.Labels.TextAfter"), t.push("XTopAxis.Labels.TextBefore"), t.push("XTopAxis.Title.Text"), t.push("YAxis.Labels.TextAfter"), t.push("YAxis.Labels.TextBefore"), t.push("YAxis.Title.Text"), t.push("YRightAxis.Labels.TextAfter"), t.push("YRightAxis.Labels.TextBefore"), t.push("YRightAxis.Title.Text")), 0);
                 return this.values.forEach(e => t.push(`Value${r++}.Label`)), r = 0, this.arguments.forEach(e => t.push(`Argument${r++}.Label`)), t
             }
             getFonts() {
                 let e = super.getFonts();
-                return e.push(this.title.font), e.push(this.labels.font), e.push(this.legend.labels.font), e.push(this.legend.title.font), e.push(this.xAxis.labels.font), e.push(this.xAxis.title.font), e.push(this.xTopAxis.labels.font), e.push(this.xTopAxis.title.font), e.push(this.yAxis.labels.font), e.push(this.yAxis.title.font), e.push(this.yRightAxis.labels.font), e.push(this.yRightAxis.title.font), Ln.distinct(e)
+                return e.push(this.title.font), e.push(this.labels.font), e.push(this.legend.labels.font), e.push(this.legend.title.font), e.push(this.xAxis.labels.font), e.push(this.xAxis.title.font), e.push(this.xTopAxis.labels.font), e.push(this.xTopAxis.title.font), e.push(this.yAxis.labels.font), e.push(this.yAxis.title.font), e.push(this.yRightAxis.labels.font), e.push(this.yRightAxis.title.font), Bn.distinct(e)
             }
             get toolboxPosition() {
                 return tt.ChartElement
             }
             get localizedName() {
                 return A.get("Components", "StiChart")
             }
@@ -4505,18 +4506,19 @@
             get labels() {
                 return this._labels
             }
             set labels(e) {
                 null != e && (e.element = this), this._labels = e
             }
             static getValueFormatDefault() {
-                return new Wr(null, null, null, 0, null, null, null, null, null, Bn.DecimalDigits | Bn.Abbreviation)
+                let e = new Wr;
+                return e.decimalDigits = 0, e.state = t.DecimalDigits | t.Abbreviation, e
             }
             getManuallyEnteredDataTable() {
-                if (this.dataMode != Vn.ManuallyEnteringData) return null;
+                if (this.dataMode != kn.ManuallyEnteringData) return null;
                 return F.e.StiManuallyEnteredDataParser.getChartDataTable(this.manuallyEnteredData, this)
             }
             get isAxisAreaChart() {
                 return this.chartValuesList().any(e => null != e && (e.seriesType == c.ClusteredBar || e.seriesType == c.ClusteredColumn || e.seriesType == c.Ribbon || e.seriesType == c.Pareto || e.seriesType == c.Histogram || e.seriesType == c.FullStackedArea || e.seriesType == c.FullStackedBar || e.seriesType == c.FullStackedColumn || e.seriesType == c.FullStackedLine || e.seriesType == c.FullStackedSpline || e.seriesType == c.FullStackedSplineArea || e.seriesType == c.StackedBar || e.seriesType == c.StackedColumn || e.seriesType == c.StackedLine || e.seriesType == c.StackedSpline || e.seriesType == c.StackedArea || e.seriesType == c.StackedSplineArea || e.seriesType == c.Scatter || e.seriesType == c.ScatterLine || e.seriesType == c.ScatterSpline || e.seriesType == c.Candlestick || e.seriesType == c.Stock || e.seriesType == c.Gantt || e.seriesType == c.Bubble || e.seriesType == c.Area || e.seriesType == c.Line || e.seriesType == c.Spline || e.seriesType == c.SplineArea || e.seriesType == c.SplineRange || e.seriesType == c.Range || e.seriesType == c.RangeBar || e.seriesType == c.SteppedArea || e.seriesType == c.SteppedLine || e.seriesType == c.SteppedRange || e.seriesType == c.BoxAndWhisker))
             }
             get isStackedChart() {
                 return this.chartValuesList().any(e => null != e && (e.seriesType == c.StackedBar || e.seriesType == c.StackedColumn || e.seriesType == c.StackedLine || e.seriesType == c.StackedSpline || e.seriesType == c.StackedArea || e.seriesType == c.StackedSplineArea))
@@ -4609,37 +4611,37 @@
             }
             setBrowsableProperty(e, t) {}
             getChartSeries() {
                 let e = c.ClusteredColumn;
                 return this.chartValuesList().any() && (e = this.chartValuesList().first().seriesType), Pn.neww2(e)
             }
             chartValuesList() {
-                if (this.dataMode == Vn.UsingDataFields) return null == this.values ? new P : this.values.where(e => null != e).toList();
+                if (this.dataMode == kn.UsingDataFields) return null == this.values ? new P : this.values.where(e => null != e).toList();
                 {
                     let e = new P;
                     return null != this.manuallyEnteredChartMeter && e.add(this.manuallyEnteredChartMeter), e
                 }
             }
             constructor(e = j.empty) {
-                super(e), this.title = new qn, this.layout = new _s, this.group = "", this.crossFiltering = !0, this._style = o.Auto, this._customStyleName = "", this.userFilters = new P, this.userSorts = new P, this.userViewStates = new P, this.transformActions = new P, this.transformFilters = new P, this.transformSorts = new P, this.topN = new Fi, this.dataTransformation = {}, this.dataFilters = new P, this.seriesColors = [], this.negativeSeriesColors = [], this.paretoSeriesColors = [], this.cornerRadius = new m(0), this.showBlanks = !1, this.shadow = new Ye, this.helpUrl = "user-manual/dashboards_chart.htm", this.manuallyEnteredChartMeter = new F.H.StiValueChartMeter, this.values = new P, this.endValues = new P, this.closeValues = new P, this.lowValues = new P, this.highValues = new P, this.arguments = new P, this.weights = new P, this.legend = new Qn, this.area = new F.H.StiChartArea, this._labels = new F.H.StiChartLabels, this.argumentFormat = new Jt, this.valueFormat = new Wr(null, null, null, 0, null, null, null, null, null, Bn.DecimalDigits | Bn.Abbreviation), this.trendLines = new P, this.constantLines = new P, this.chartConditions = new P, this.marker = new jn, this.icon = null, this.roundValues = !0, this.columnShape = En.Box, this.dataMode = Vn.UsingDataFields, this.drillDownFiltersList = new P, this.drillDownFilters = new P, this.drillDownCurrentLevel = 0, this.title.text = this.localizedName, this.dashboardInteraction = new zn, this.labels = new F.H.StiChartLabels, this.previousAnimations = new P, this.options3D = new On
+                super(e), this.title = new qn, this.layout = new $s, this.group = "", this.crossFiltering = !0, this._style = o.Auto, this._customStyleName = "", this.userFilters = new P, this.userSorts = new P, this.userViewStates = new P, this.transformActions = new P, this.transformFilters = new P, this.transformSorts = new P, this.topN = new vi, this.dataTransformation = {}, this.dataFilters = new P, this.seriesColors = [], this.negativeSeriesColors = [], this.paretoSeriesColors = [], this.cornerRadius = new m(0), this.showBlanks = !1, this.shadow = new Ye, this.helpUrl = "user-manual/dashboards_chart.htm", this.manuallyEnteredChartMeter = new F.H.StiValueChartMeter, this.values = new P, this.endValues = new P, this.closeValues = new P, this.lowValues = new P, this.highValues = new P, this.arguments = new P, this.weights = new P, this.legend = new Qn, this.area = new F.H.StiChartArea, this._labels = new F.H.StiChartLabels, this.argumentFormat = new Jt, this.valueFormat = Am.getValueFormatDefault(), this.trendLines = new P, this.constantLines = new P, this.chartConditions = new P, this.marker = new jn, this.icon = null, this.roundValues = !0, this.columnShape = On.Box, this.dataMode = kn.UsingDataFields, this.drillDownFiltersList = new P, this.drillDownFilters = new P, this.drillDownCurrentLevel = 0, this.title.text = this.localizedName, this.dashboardInteraction = new zn, this.labels = new F.H.StiChartLabels, this.previousAnimations = new P, this.options3D = new Vn
             }
         }
         F.H.StiChartElement = Am
     }
     let sl = L.Report.Dashboard.IStiChartElementCondition,
         nl = L.Report.Components.StiFilterCondition,
         ll = L.Report.Components.StiFilterDataType,
         al = L.Report.Chart.StiChartConditionalField;
     {
         class Xg {
             implements() {
                 return Xg.ImplementsStiChartElementCondition || (Xg.ImplementsStiChartElementCondition = [Vt, sl, l]), Xg.ImplementsStiChartElementCondition
             }
             meta() {
-                return [new ne("Ident").get(() => this[L.System.StiObject.stimulsoft]().getType()[L.System.StiObject.stimulsoft]().getTypeName()), new n("KeyValueMeter"), new i("Condition", "", nl, nl.EqualTo), new i("DataType", "", ll, ll.Numeric), new i("Field", "", al, al.Value), new n("Value"), new r("Color", "", N.white), new i("MarkerType", "", gn, gn.Circle), new se("MarkerAngle", "", 0), new h("IsExpression")]
+                return [new ne("Ident").get(() => this[L.System.StiObject.stimulsoft]().getType()[L.System.StiObject.stimulsoft]().getTypeName()), new n("KeyValueMeter"), new i("Condition", "", nl, nl.EqualTo), new i("DataType", "", ll, ll.Numeric), new i("Field", "", al, al.Value), new n("Value"), new r("Color", "", N.white), new i("MarkerType", "", pn, pn.Circle), new se("MarkerAngle", "", 0), new h("IsExpression")]
             }
             saveToJsonObject(e) {
                 return u.saveToJsonObject(e, this)
             }
             loadFromJsonObject(e) {
                 u.loadFromJsonObject(e, this)
             }
@@ -4654,15 +4656,15 @@
                 return t.loadFromJsonObject(e), t
             }
             static createFromXml(e) {
                 let t = new Xg;
                 return t.loadFromXml(e), t
             }
             constructor(e, t, r, i, s, n, l, a, o) {
-                this.color = N.white, this.markerAngle = 0, this.markerType = gn.Circle, this.condition = nl.EqualTo, this.dataType = ll.Numeric, this.value = "", this.keyValueMeter = "", this.field = al.Value, this.isExpression = !1, null != e && (this.keyValueMeter = e), null != t && (this.color = t), null != r && (this.dataType = r), null != i && (this.condition = i), null != s && (this.value = s), null != n && (this.markerType = n), null != l && (this.markerAngle = l), null != a && (this.field = a), null != o && (this.isExpression = o)
+                this.color = N.white, this.markerAngle = 0, this.markerType = pn.Circle, this.condition = nl.EqualTo, this.dataType = ll.Numeric, this.value = "", this.keyValueMeter = "", this.field = al.Value, this.isExpression = !1, null != e && (this.keyValueMeter = e), null != t && (this.color = t), null != r && (this.dataType = r), null != i && (this.condition = i), null != s && (this.value = s), null != n && (this.markerType = n), null != l && (this.markerAngle = l), null != a && (this.field = a), null != o && (this.isExpression = o)
             }
         }
         F.H.StiChartElementCondition = Xg
     } {
         class Wg {
             constructor() {
                 this.color = N.transparent
@@ -4745,23 +4747,23 @@
     }
     let ul = L.System.Text.Encoding,
         hl = L.Base.StiPacker,
         ml = (F.H.StiChartUserViewStatesHelper = class {
             static saveToJsonObject(e) {
                 let t = new He,
                     r = je.Report;
-                return t.addPropertyJObject("UserFilters", a.Serialize.objectArray(e.userFilters, r)), t.addPropertyJObject("UserSorts", a.Serialize.objectArray(e.userSorts, r)), t.addPropertyJObject("Values", a.Serialize.objectArray(e.values, r)), t.addPropertyJObject("EndValues", a.Serialize.objectArray(e.endValues, r)), t.addPropertyJObject("CloseValues", a.Serialize.objectArray(e.closeValues, r)), t.addPropertyJObject("LowValues", a.Serialize.objectArray(e.lowValues, r)), t.addPropertyJObject("HighValues", a.Serialize.objectArray(e.highValues, r)), t.addPropertyJObject("Arguments", a.Serialize.objectArray(e.arguments, r)), t.addPropertyJObject("Weights", a.Serialize.objectArray(e.weights, r)), null != e.series && t.addPropertyJObject("Series", e.series.saveToJsonObject(r)), null != e.sortBy && t.addPropertyJObject("SortBy", e.sortBy.saveToJsonObject(r)), null != e.indicatorValue && t.addPropertyJObject("IndicatorValue", e.indicatorValue.saveToJsonObject(r)), null != e.icon && t.addPropertyEnum("Icon", kt, e.icon), t.addPropertyBool("RoundValues", e.roundValues, !0), t.addPropertyEnum("ColumnShape", En, e.columnShape, En.Box), t
+                return t.addPropertyJObject("UserFilters", a.Serialize.objectArray(e.userFilters, r)), t.addPropertyJObject("UserSorts", a.Serialize.objectArray(e.userSorts, r)), t.addPropertyJObject("Values", a.Serialize.objectArray(e.values, r)), t.addPropertyJObject("EndValues", a.Serialize.objectArray(e.endValues, r)), t.addPropertyJObject("CloseValues", a.Serialize.objectArray(e.closeValues, r)), t.addPropertyJObject("LowValues", a.Serialize.objectArray(e.lowValues, r)), t.addPropertyJObject("HighValues", a.Serialize.objectArray(e.highValues, r)), t.addPropertyJObject("Arguments", a.Serialize.objectArray(e.arguments, r)), t.addPropertyJObject("Weights", a.Serialize.objectArray(e.weights, r)), null != e.series && t.addPropertyJObject("Series", e.series.saveToJsonObject(r)), null != e.sortBy && t.addPropertyJObject("SortBy", e.sortBy.saveToJsonObject(r)), null != e.indicatorValue && t.addPropertyJObject("IndicatorValue", e.indicatorValue.saveToJsonObject(r)), null != e.icon && t.addPropertyEnum("Icon", kt, e.icon), t.addPropertyBool("RoundValues", e.roundValues, !0), t.addPropertyEnum("ColumnShape", On, e.columnShape, On.Box), t
             }
             static loadFromJsonObject(r, e) {
                 for (let t of e.properties()) switch (t.name) {
                     case "UserFilters":
                         r.userFilters.clear(), r.userFilters.addRange(t.value.properties().select(e => f.loadFromJson(e.value)));
                         break;
                     case "UserSorts":
-                        r.userSorts.clear(), r.userSorts.addRange(t.value.properties().select(e => rn.loadFromJson(e.value)));
+                        r.userSorts.clear(), r.userSorts.addRange(t.value.properties().select(e => sn.loadFromJson(e.value)));
                         break;
                     case "Values":
                         r.values.clear(), r.values.addRange(t.value.properties().select(e => g.loadFromJson(e.value)));
                         break;
                     case "EndValues":
                         r.endValues.clear(), r.endValues.addRange(t.value.properties().select(e => g.loadFromJson(e.value)));
                         break;
@@ -4787,26 +4789,26 @@
                     }
                     case "SortBy": {
                         let e = g.loadFromJson(t.value).as(F.H.StiSortByChartMeter);
                         null != e && (r.sortBy = e);
                         break
                     }
                     case "IndicatorValue": {
-                        let e = g.loadFromJson(t.value).as(Vi);
+                        let e = g.loadFromJson(t.value).as(ki);
                         null != e && (r.indicatorValue = e);
                         break
                     }
                     case "Icon":
                         r.icon = ve.parse(kt, t.value.toString());
                         break;
                     case "RoundValues":
                         r.roundValues = t.value[L.System.StiObject.stimulsoft]().toBoolean();
                         break;
                     case "ColumnShape":
-                        r.columnShape = ve.parse(En, t.value.toString());
+                        r.columnShape = ve.parse(On, t.value.toString());
                         break
                 }
             }
             static clearVisualState(e) {
                 e.values.clear(), e.endValues.clear(), e.closeValues.clear(), e.lowValues.clear(), e.highValues.clear(), e.arguments.clear(), e.weights.clear(), e.series = null, e.sortBy = null, e.icon = null
             }
             static switchSelectedViewState(e, t) {
@@ -4863,18 +4865,18 @@
             }
         }, F.H.StiVertChartInterlacing = class extends F.H.StiChartInterlacing {
             constructor(e, t) {
                 super(e, t)
             }
         }, F.H.StiXChartAxisTitle = class extends F.H.StiChartAxisTitle {
             meta() {
-                return [...super.meta(), new i("Direction", "", xn, xn.LeftToRight)]
+                return [...super.meta(), new i("Direction", "", Mn, Mn.LeftToRight)]
             }
             constructor(e, t, r, i, s, n, l) {
-                super(e, t, r, i, n, l), this.direction = xn.LeftToRight, null != s && (this.direction = s)
+                super(e, t, r, i, n, l), this.direction = Mn.LeftToRight, null != s && (this.direction = s)
             }
         }, F.H.StiXChartMeter = class extends F.e.StiDimensionMeter {
             get localizedName() {
                 return `X` + b.get("PropertyMain", "Value")
             }
             constructor(e, t, r) {
                 super(e, t, r), this.ident = F.e.StiMeterIdent.XChartMeter
@@ -4906,15 +4908,15 @@
     {
         dt.add("StiComboBoxElement", "Stimulsoft.Dashboard.Export.Tools.StiComboBoxElementExportTool");
         class gm extends F.e.StiElement {
             implements() {
                 return gm.ImplementsStiComboBoxElement || (gm.ImplementsStiComboBoxElement = super.implements().concat([pl, Ke, Ze, lr, Qr, ...dl, ...Qe, ...Ue, ...tr, l])), gm.ImplementsStiComboBoxElement
             }
             meta() {
-                return [...super.meta(), new n("ParentKey"), new n("InitialValue"), new s("UserFilters").get(e => a.Serialize.objectArray(this.userFilters, e)).set(e => this.userFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.userFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new s("TransformActions").get(e => a.Serialize.objectArray(this.transformActions, e)).set(e => this.transformActions.addRange(e.value.properties().select(e => sn.loadFromJson(e.value)))).setXml(e => this.transformActions.addRange(e.childNodes.select(e => sn.loadFromXml(e)))), new s("TransformFilters").get(e => a.Serialize.objectArray(this.transformFilters, e)).set(e => this.transformFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.transformFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new s("TransformSorts").get(e => a.Serialize.objectArray(this.transformSorts, e)).set(e => this.transformSorts.addRange(e.value.properties().select(e => rn.loadFromJson(e.value)))).setXml(e => this.transformSorts.addRange(e.childNodes.select(e => rn.loadFromXml(e)))), new s("DataFilters").get(e => a.Serialize.objectArray(this.dataFilters, e)).set(e => this.dataFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.dataFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new r("ForeColor", "", N.transparent), new n("Font").get(() => a.Serialize.fontArial8(this.font)).set(e => this.font = a.Deserialize.font(e.value, this.font)).setXml(e => this.font = L.System.Convert.toFont(e.textContent)), new h("ShowAllValue"), new h("ShowBlanks"), new i("SelectionMode", "", gl, gl.One).set(e => {
+                return [...super.meta(), new n("ParentKey"), new n("InitialValue"), new s("UserFilters").get(e => a.Serialize.objectArray(this.userFilters, e)).set(e => this.userFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.userFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new s("TransformActions").get(e => a.Serialize.objectArray(this.transformActions, e)).set(e => this.transformActions.addRange(e.value.properties().select(e => nn.loadFromJson(e.value)))).setXml(e => this.transformActions.addRange(e.childNodes.select(e => nn.loadFromXml(e)))), new s("TransformFilters").get(e => a.Serialize.objectArray(this.transformFilters, e)).set(e => this.transformFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.transformFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new s("TransformSorts").get(e => a.Serialize.objectArray(this.transformSorts, e)).set(e => this.transformSorts.addRange(e.value.properties().select(e => sn.loadFromJson(e.value)))).setXml(e => this.transformSorts.addRange(e.childNodes.select(e => sn.loadFromXml(e)))), new s("DataFilters").get(e => a.Serialize.objectArray(this.dataFilters, e)).set(e => this.dataFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.dataFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new r("ForeColor", "", N.transparent), new n("Font").get(() => a.Serialize.fontArial8(this.font)).set(e => this.font = a.Deserialize.font(e.value, this.font)).setXml(e => this.font = L.System.Convert.toFont(e.textContent)), new h("ShowAllValue"), new h("ShowBlanks"), new i("SelectionMode", "", gl, gl.One).set(e => {
                     let t = ve.parse(gl, e.value);
                     null != t && (this.selectionMode = t)
                 }).setXml(e => {
                     let t = ve.parse(gl, e.textContent);
                     null != t && (this.selectionMode = t)
                 }), new s("NameMeter").check(() => null != this.nameMeter).set(e => {
                     let t = g.loadFromJson(e.value).as(F.S.StiNameComboBoxMeter);
@@ -4964,15 +4966,15 @@
                 return null != this.nameMeter && e.add(this.nameMeter), null != this.keyMeter && e.add(this.keyMeter), e
             }
             getMeters() {
                 let e = new P;
                 return null != this.nameMeter && e.add(this.nameMeter), null != this.keyMeter && e.add(this.keyMeter), e
             }
             retrieveUsedDataNames() {
-                return en.getMany(this.nameMeter, this.keyMeter)
+                return tn.getMany(this.nameMeter, this.keyMeter)
             }
             get isDefined() {
                 return null != this.nameMeter || null != this.keyMeter
             }
             addKeyMeter2(e) {
                 this.keyMeter = null != e ? d.ComboBox.getKey2(e) : null
             }
@@ -5108,15 +5110,15 @@
                 return null
             }
             static format(e, t) {
                 var r;
                 let i = e.as(yr);
                 if (t instanceof w && !i.textFormat.is(Xr)) return t.toShortDateString();
                 let s = null == (r = null == e ? void 0 : e.report) ? void 0 : r.culture;
-                if (li.isEligable(t, s)) return li.convert(t, s);
+                if (ai.isEligable(t, s)) return ai.convert(t, s);
                 return i.textFormat.format(t)
             }
         }, F.S.StiComboBoxItem = class {
             toString() {
                 return null != this.label ? this.label : this.value.toString()
             }
             constructor(e, t = e) {
@@ -5142,33 +5144,33 @@
                 return [...super.meta(), new s("UserFilters").get(e => a.Serialize.objectArray(this.userFilters, e)).set(e => this.userFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.userFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new s("DataFilters").get(e => a.Serialize.objectArray(this.dataFilters, e)).set(e => this.dataFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.dataFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new r("ForeColor", "", N.transparent), new n("Font").get(() => a.Serialize.fontArial8(this.font)).set(e => this.font = a.Deserialize.font(e.value, this.font)).setXml(e => this.font = L.System.Convert.toFont(e.textContent)), new i("Condition", "", Tl, Tl.GreaterThanOrEqualTo), new i("SelectionMode", "", Ml, Ml.Single).set(e => {
                     let t = ve.parse(Ml, e.value);
                     null != t && (this.selectionMode = t)
                 }).setXml(e => {
                     let t = ve.parse(Ml, e.textContent);
                     null != t && (this.selectionMode = t)
                 }), new i("InitialRangeSelection", "", Cl, Cl.MonthPrevious), new i("InitialRangeSelectionSource", "", xl, xl.Variable), new s("ValueMeter").check(() => null != this.valueMeter).set(e => {
-                    let t = g.loadFromJson(e.value).as(fs);
+                    let t = g.loadFromJson(e.value).as(ys);
                     null != t && (this.valueMeter = t)
                 }).setXml(e => {
-                    let t = g.loadFromXml(e).as(fs);
+                    let t = g.loadFromXml(e).as(ys);
                     null != t && (this.valueMeter = t)
                 }), new i("Style", "", o, o.Auto), new n("Group"), new n("CustomStyleName"), new n("CornerRadius").get(() => this.cornerRadius.toString()).set(e => this.cornerRadius = m.tryParse(e.value.toString())).setXml(e => this.cornerRadius = m.tryParse(e.textContent)), new n("Shadow").get(() => a.Serialize.jShadow(this.shadow)).set(e => this.shadow = a.Deserialize.simpleSahdow(e.value)).setXml(e => this.shadow = Ye.loadFromXml(e.textContent)), new s("TextFormat").check(() => !(this.textFormat.is(Jt) || null == this.textFormat)).set(e => this.textFormat = br.createFromJsonObject(e.value)).setXml(e => this.textFormat = br.loadFormatFromXml(e, this.report)), new le("MinSize"), new le("MaxSize")]
             }
             clone(e) {
                 var t, r;
                 let i = super.clone(e);
                 return i.valueMeter = null != this.valueMeter ? this.valueMeter.clone() : null, i.userFilters = this.userFilters.select(e => e.clone()).toList(), i.dataFilters = this.dataFilters.select(e => e.clone()).toList(), i.textFormat = this.textFormat.clone(), i.shadow = null == (t = this.shadow) ? void 0 : t.clone(), i.cornerRadius = null == (r = this.cornerRadius) ? void 0 : r.clone(), i
             }
             getParentKey() {
                 return null
             }
             setParentKey(e) {}
             async applyDefaultFilters() {
                 var e;
-                let i = null == (e = F.Q.StiDatePickerHelper.getVariableSpecifiedAsValue(this.as(Fl))) ? void 0 : e.as(zs);
+                let i = null == (e = F.Q.StiDatePickerHelper.getVariableSpecifiedAsValue(this.as(Fl))) ? void 0 : e.as(Gs);
                 if (null == i) {
                     let e = await F.Q.StiDatePickerHelper.fetchDefaultUserFilters(this);
                     null != e && (this.userFilters = e)
                 } else if (Al.isRangeType(i.type) && this.initialRangeSelectionSource == xl.Selection) {
                     let e = {
                             ref: null
                         },
@@ -5190,15 +5192,15 @@
                 return null != this.valueMeter && e.add(this.valueMeter), e
             }
             getMeters() {
                 let e = new P;
                 return (F.Q.StiDatePickerHelper.isVariableSpecifiedAsValue(this) || null != this.valueMeter && this.selectionMode == Ml.AutoRange) && e.add(this.valueMeter), e
             }
             retrieveUsedDataNames() {
-                return null != this.valueMeter && this.selectionMode == Ml.AutoRange ? en.getMany(this.valueMeter) : super.retrieveUsedDataNames()
+                return null != this.valueMeter && this.selectionMode == Ml.AutoRange ? tn.getMany(this.valueMeter) : super.retrieveUsedDataNames()
             }
             get isDefined() {
                 return null != this.valueMeter
             }
             addValueMeter2(e) {
                 this.valueMeter = null != e ? d.DatePicker.getValue2(e) : null
             }
@@ -5208,21 +5210,21 @@
             getValueMeter() {
                 return this.valueMeter
             }
             removeValueMeter() {
                 this.valueMeter = null
             }
             createNewValueMeter() {
-                this.valueMeter = new fs
+                this.valueMeter = new ys
             }
             convertFrom(e) {
                 let t = e.fetchAllMeters();
                 if (null == t) return;
                 let r = t.firstOrDefault(e => e.is(Er));
-                null != (r = null == r ? t.firstOrDefault(e => e.is(vt)) : r) && (this.valueMeter = null == this.valueMeter ? new fs : this.valueMeter, this.valueMeter.loadFromJsonObject(r.saveToJsonObject(je.Report)))
+                null != (r = null == r ? t.firstOrDefault(e => e.is(vt)) : r) && (this.valueMeter = null == this.valueMeter ? new ys : this.valueMeter, this.valueMeter.loadFromJsonObject(r.saveToJsonObject(je.Report)))
             }
             get toolboxPosition() {
                 return tt.DatePickerElement
             }
             get localizedName() {
                 return A.get("Components", "StiDatePicker")
             }
@@ -5353,46 +5355,46 @@
                         ref: null
                     },
                     i = {
                         ref: null
                     },
                     s = (this.calculateRangeFromInitial(e, r, i), this.getFormatedDate(r.ref)),
                     n = this.getFormatedDate(i.ref);
-                return new f("", t, Zi.Between, s, n, !0, !1).toList()
+                return new f("", t, Yi.Between, s, n, !0, !1).toList()
             }
             static async getAutoRangeDefaultUserFilters(e, t) {
                 let r = await bl.getOrCreate(e);
                 if (null == r) return null;
                 let i = r.rows.select(e => e[0]).where(e => e instanceof w);
                 if (null == i || !i.any()) return null;
                 let s = i.where(e => e instanceof w).cast().min(),
                     n = i.where(e => e instanceof w).cast().max(),
                     l = this.getFormatedDate(s),
                     a = this.getFormatedDate(n);
-                return new f("", t, Zi.Between, l, a, !0, !1).toList()
+                return new f("", t, Yi.Between, l, a, !0, !1).toList()
             }
             static getValueMeterExpression(e) {
                 return null != e.valueMeter ? e.valueMeter.expression : null
             }
             static getCondition(e) {
                 switch (e.condition) {
                     case Tl.EqualTo:
-                        return Zi.EqualTo;
+                        return Yi.EqualTo;
                     case Tl.NotEqualTo:
-                        return Zi.NotEqualTo;
+                        return Yi.NotEqualTo;
                     case Tl.GreaterThan:
-                        return Zi.GreaterThan;
+                        return Yi.GreaterThan;
                     case Tl.GreaterThanOrEqualTo:
-                        return Zi.GreaterThanOrEqualTo;
+                        return Yi.GreaterThanOrEqualTo;
                     case Tl.LessThan:
-                        return Zi.LessThan;
+                        return Yi.LessThan;
                     case Tl.LessThanOrEqualTo:
-                        return Zi.LessThanOrEqualTo;
+                        return Yi.LessThanOrEqualTo;
                     default:
-                        return Zi.EqualTo
+                        return Yi.EqualTo
                 }
             }
             static getFormatedDate(e) {
                 return e.toString("MM/dd/yyyy")
             }
             static getVariableSpecifiedAsValue(e) {
                 var t;
@@ -5400,15 +5402,15 @@
             }
             static isVariableSpecifiedAsValue(e) {
                 var t;
                 return El.isVariableSpecifiedAsExpression(e, null == (t = e.getValueMeter()) ? void 0 : t.expression)
             }
             static getDefaultValue(t) {
                 var e;
-                let r = null == (e = this.getVariableSpecifiedAsValue(t)) ? void 0 : e.as(zs);
+                let r = null == (e = this.getVariableSpecifiedAsValue(t)) ? void 0 : e.as(Gs);
                 if (null != r) {
                     let e = t.report.dictionary.getVariableValueByName(r.name);
                     if (r.initBy != Rl.Expression || B.isNullOrEmpty(e) || (e = Dl.parseTextValue(`{${e}}`, t)), r.type == w || r.type == Vl) return V.tryToDateTime(e);
                     if (r.type == vl || r.type == Ol) return e[L.System.StiObject.stimulsoft]().is(vl) ? e : new vl
                 }
                 return w.now
             }
@@ -5473,15 +5475,15 @@
                 return e
             }
             toString(e) {
                 return null == e ? "" : e.toString()
             }
             toReadableString(e, t) {
                 let r = null == t ? void 0 : t.getParsedCulture();
-                if (li.isEligable(e, r)) return li.convert(e, r);
+                if (ai.isEligable(e, r)) return ai.convert(e, r);
                 return this.toString(e)
             }
         }, L.Base.Meters.IStiMinGaugeMeter);
     {
         class aa extends F.e.StiMeasureMeter {
             implements() {
                 return aa.ImplementsStiMinGaugeMeter || (aa.ImplementsStiMinGaugeMeter = super.implements().concat([Nl])), aa.ImplementsStiMinGaugeMeter
@@ -5604,15 +5606,15 @@
                 }
                 e.ref = b, n.ref = f, e.ref < 0 && t.calculationMode == la.Auto && !y && (e.ref = 0)
             }
             async render(e, t, r) {
                 return this.render2(e, t, r)()
             }
             render2(y, C, x) {
-                this.storedCulture = ai.set(y.report);
+                this.storedCulture = oi.set(y.report);
                 try {
                     let d = this.getValueMeterIndex(x),
                         g = this.getSeriesMeterIndex(x),
                         p = this.getTargetMeterIndex(x),
                         e = this.getMinMeterIndex(x),
                         t = this.getMaxMeterIndex(x),
                         r = this.getSeriesKeyValues(x, g, this.getSeriesKeysLimitCount(y)),
@@ -5901,35 +5903,35 @@
             getMaxValue(e, t, r) {
                 if (-1 == r) return e.maximum;
                 let i = e.calculationMode == la.Auto ? t.rows.getArrayItem(r).firstOrDefaultAsNullableNumber() : e.maximum;
                 return null != i ? i : e.maximum
             }
             getValueMeterIndex(e) {
                 if (null == e) return -1;
-                let t = e.meters.firstOrDefault(e => e.is(Fs));
+                let t = e.meters.firstOrDefault(e => e.is(vs));
                 return null != t ? e.meters.indexOf(t) : -1
             }
             getMinMeterIndex(e) {
                 if (null == e) return -1;
                 let t = e.meters.firstOrDefault(e => e.is(aa));
                 return null != t ? e.meters.indexOf(t) : -1
             }
             getMaxMeterIndex(e) {
                 if (null == e) return -1;
                 let t = e.meters.firstOrDefault(e => e.is(oa));
                 return null != t ? e.meters.indexOf(t) : -1
             }
             getSeriesMeterIndex(e) {
                 if (null == e) return -1;
-                let t = e.meters.firstOrDefault(e => e.is(Ts));
+                let t = e.meters.firstOrDefault(e => e.is(Fs));
                 return null != t ? e.meters.indexOf(t) : -1
             }
             getTargetMeterIndex(e) {
                 if (null == e) return -1;
-                let t = e.meters.firstOrDefault(e => e.is(vs));
+                let t = e.meters.firstOrDefault(e => e.is(As));
                 return null != t ? e.meters.indexOf(t) : -1
             }
         }
         F.i.StiGaugeElementBuilder = Aa
     }
     let fa = L.Report.Dashboard.ImplementsIStiGaugeRange,
         ya = L.Report.Dashboard.IStiGaugeRange;
@@ -5993,15 +5995,15 @@
                 this.color = N.red, this.startExpression = "0", this.endExpression = "100", null != e && (this.color = e), null != t && (this.startExpression = t), null != r && (this.endExpression = r)
             }
         }
         F.T.StiGaugeRange = Fa
     } {
         class Ta extends F.g.StiDashboardInteraction {
             implements() {
-                return Ta.ImplementsIStiGaugeDashboardInteraction || (Ta.ImplementsIStiGaugeDashboardInteraction = super.implements().concat([An, l, Gs])), Ta.ImplementsIStiGaugeDashboardInteraction
+                return Ta.ImplementsIStiGaugeDashboardInteraction || (Ta.ImplementsIStiGaugeDashboardInteraction = super.implements().concat([In, l, Xs])), Ta.ImplementsIStiGaugeDashboardInteraction
             }
             meta() {
                 return [...super.meta(), new h("AllowUserSorting", "", !0), new h("ShowFullScreenButton", "", !0), new h("ShowSaveButton", "", !0), new h("ShowViewDataButton", "", !0), new n("FileName"), new n("HeaderText"), new n("FooterText")]
             }
             get isDefaultLayout() {
                 return this.showFullScreenButton && this.showSaveButton && this.showViewDataButton && null == this.fileName && null == this.headerText && null == this.footerText
             }
@@ -6076,41 +6078,41 @@
         Ia = L.Report.Dashboard.IStiGaugeElement,
         Da = F.T.StiGaugeLabels,
         Ra = L.Report.Components.IStiNumberFormat;
     {
         dt.add("StiGaugeElement", "Stimulsoft.Dashboard.Export.Tools.StiGaugeElementExportTool");
         class vm extends F.e.StiElement {
             implements() {
-                return vm.ImplementsStiGaugeElement || (vm.ImplementsStiGaugeElement = super.implements().concat([Ia, Ke, Ze, Oe, ar, fr, qs, Qr, Ne, ...va, ...Qe, ...Ue, ...$s, ...rr, ...Sr, ...Qs, l, Xs, Ra])), vm.ImplementsStiGaugeElement
+                return vm.ImplementsStiGaugeElement || (vm.ImplementsStiGaugeElement = super.implements().concat([Ia, Ke, Ze, Oe, ar, fr, _s, Qr, Ne, ...va, ...Qe, ...Ue, ...en, ...rr, ...Sr, ...qs, l, Ws, Ra])), vm.ImplementsStiGaugeElement
             }
             clone(e) {
                 var t, r, i, s;
                 let n = super.clone(e);
                 return n.value = null != this.value ? this.value.clone() : null, n.series = null != this.series ? this.series.clone() : null, n.target = null != this.target ? this.target.clone() : null, n.valueFormat = null != this.valueFormat ? this.valueFormat.clone() : null, n.userSorts = this.userSorts.select(e => e.clone()).toList(), n.transformActions = this.transformActions.select(e => e.clone()).toList(), n.transformFilters = this.transformFilters.select(e => e.clone()).toList(), n.transformSorts = this.transformSorts.select(e => e.clone()).toList(), n.dataFilters = this.dataFilters.select(e => e.clone()).toList(), n.title = null != this.title ? this.title.clone() : null, n.layout = null != this.layout ? this.layout.clone() : null, n.dashboardInteraction = this.dashboardInteraction.clone(), n.labels = null == (t = this.labels) ? void 0 : t.clone(), n.targetSettings = null == (r = this.targetSettings) ? void 0 : r.clone(), n.shadow = null == (i = this.shadow) ? void 0 : i.clone(), n.cornerRadius = null == (s = this.cornerRadius) ? void 0 : s.clone(), n
             }
             meta() {
-                return [...super.meta(), new s("UserSorts").get(e => a.Serialize.objectArray(this.userSorts, e)).set(e => this.userSorts.addRange(e.value.properties().select(e => rn.loadFromJson(e.value)))).setXml(e => this.userSorts.addRange(e.childNodes.select(e => rn.loadFromXml(e)))), new s("TransformActions").get(e => a.Serialize.objectArray(this.transformActions, e)).set(e => this.transformActions.addRange(e.value.properties().select(e => sn.loadFromJson(e.value)))).setXml(e => this.transformActions.addRange(e.childNodes.select(e => sn.loadFromXml(e)))), new s("TransformFilters").get(e => a.Serialize.objectArray(this.transformFilters, e)).set(e => this.transformFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.transformFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new s("TransformSorts").get(e => a.Serialize.objectArray(this.transformSorts, e)).set(e => this.transformSorts.addRange(e.value.properties().select(e => rn.loadFromJson(e.value)))).setXml(e => this.transformSorts.addRange(e.childNodes.select(e => rn.loadFromXml(e)))), new s("DataFilters").get(e => a.Serialize.objectArray(this.dataFilters, e)).set(e => this.dataFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.dataFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new s("Ranges").get(e => a.Serialize.objectArray(this.ranges, e)).set(e => this.ranges.addRange(e.value.properties().select(e => Fa.loadFromJson(e.value)))).setXml(e => this.ranges.addRange(e.childNodes.select(e => Fa.loadFromXml(e)))), new se("Minimum", "", 0), new se("Maximum", "", 100), new i("CalculationMode", "", L.Report["Gauge"].StiGaugeCalculationMode, L.Report["Gauge"].StiGaugeCalculationMode.Auto), new i("RangeMode", "", L.Report["Gauge"].StiGaugeRangeMode, L.Report["Gauge"].StiGaugeRangeMode.Percentage), new i("Type", "", L.Report["Gauge"].StiGaugeType, L.Report["Gauge"].StiGaugeType.FullCircular), new i("RangeType", "", L.Report["Gauge"].StiGaugeRangeType, L.Report["Gauge"].StiGaugeRangeType.None), new h("ShortValue", "", !0), new h("CrossFiltering", "", !0), new h("ShowBlanks"), new n("CornerRadius").get(() => this.cornerRadius.toString()).set(e => this.cornerRadius = m.tryParse(e.value.toString())).setXml(e => this.cornerRadius = m.tryParse(e.textContent)), new s("Labels").check(() => null != this.labels), new s("TargetSettings").check(() => null != this.targetSettings), new s("Value").check(() => null != this.value).set(e => {
+                return [...super.meta(), new s("UserSorts").get(e => a.Serialize.objectArray(this.userSorts, e)).set(e => this.userSorts.addRange(e.value.properties().select(e => sn.loadFromJson(e.value)))).setXml(e => this.userSorts.addRange(e.childNodes.select(e => sn.loadFromXml(e)))), new s("TransformActions").get(e => a.Serialize.objectArray(this.transformActions, e)).set(e => this.transformActions.addRange(e.value.properties().select(e => nn.loadFromJson(e.value)))).setXml(e => this.transformActions.addRange(e.childNodes.select(e => nn.loadFromXml(e)))), new s("TransformFilters").get(e => a.Serialize.objectArray(this.transformFilters, e)).set(e => this.transformFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.transformFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new s("TransformSorts").get(e => a.Serialize.objectArray(this.transformSorts, e)).set(e => this.transformSorts.addRange(e.value.properties().select(e => sn.loadFromJson(e.value)))).setXml(e => this.transformSorts.addRange(e.childNodes.select(e => sn.loadFromXml(e)))), new s("DataFilters").get(e => a.Serialize.objectArray(this.dataFilters, e)).set(e => this.dataFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.dataFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new s("Ranges").get(e => a.Serialize.objectArray(this.ranges, e)).set(e => this.ranges.addRange(e.value.properties().select(e => Fa.loadFromJson(e.value)))).setXml(e => this.ranges.addRange(e.childNodes.select(e => Fa.loadFromXml(e)))), new se("Minimum", "", 0), new se("Maximum", "", 100), new i("CalculationMode", "", L.Report["Gauge"].StiGaugeCalculationMode, L.Report["Gauge"].StiGaugeCalculationMode.Auto), new i("RangeMode", "", L.Report["Gauge"].StiGaugeRangeMode, L.Report["Gauge"].StiGaugeRangeMode.Percentage), new i("Type", "", L.Report["Gauge"].StiGaugeType, L.Report["Gauge"].StiGaugeType.FullCircular), new i("RangeType", "", L.Report["Gauge"].StiGaugeRangeType, L.Report["Gauge"].StiGaugeRangeType.None), new h("ShortValue", "", !0), new h("CrossFiltering", "", !0), new h("ShowBlanks"), new n("CornerRadius").get(() => this.cornerRadius.toString()).set(e => this.cornerRadius = m.tryParse(e.value.toString())).setXml(e => this.cornerRadius = m.tryParse(e.textContent)), new s("Labels").check(() => null != this.labels), new s("TargetSettings").check(() => null != this.targetSettings), new s("Value").check(() => null != this.value).set(e => {
                     let t = g.loadFromJson(e.value).as(F.T.StiValueGaugeMeter);
                     null != t && (this.value = t)
                 }).setXml(e => {
                     let t = g.loadFromXml(e).as(F.T.StiValueGaugeMeter);
                     null != t && (this.value = t)
                 }), new s("Series").check(() => null != this.series).set(e => {
-                    let t = g.loadFromJson(e.value).as(Ts);
+                    let t = g.loadFromJson(e.value).as(Fs);
                     null != t && (this.series = t)
                 }).setXml(e => {
-                    let t = g.loadFromXml(e).as(Ts);
+                    let t = g.loadFromXml(e).as(Fs);
                     null != t && (this.series = t)
                 }), new s("Target").check(() => null != this.target).set(e => {
                     let t = g.loadFromJson(e.value).as(F.T.StiTargetGaugeMeter);
                     null != t && (this.target = t)
                 }).setXml(e => {
                     let t = g.loadFromXml(e).as(F.T.StiTargetGaugeMeter);
                     null != t && (this.target = t)
-                }), new s("Title").check(() => null != this.title).set(e => this.title = qn.createFromJsonObject(e.value)).setXml(e => this.title = qn.createFromXml(e)), new s("Layout").check(() => null != this.layout).set(e => this.layout = _s.createFromJsonObject(e.value)).setXml(e => this.layout = _s.createFromXml(e)), new r("ForeColor", "", N.transparent), new n("Font").get(() => a.Serialize.fontArial8(this.font)).set(e => this.font = a.Deserialize.font(e.value, this.font)).setXml(e => this.font = L.System.Convert.toFont(e.textContent)), new i("DataMode", "", Vn, Vn.UsingDataFields), new n("ManuallyEnteredData"), new i("Style", "", o, o.Auto), new n("Group"), new n("CustomStyleName"), new n("Shadow").get(() => a.Serialize.jShadow(this.shadow)).set(e => this.shadow = a.Deserialize.simpleSahdow(e.value)).setXml(e => this.shadow = Ye.loadFromXml(e.textContent)), new s("ValueFormat").check(() => null != this.valueFormat).set(e => this.valueFormat = br.createFromJsonObject(e.value)).setXml(e => this.valueFormat = br.loadFormatFromXml(e, this.report)), new s("DashboardInteraction").check(() => null != this.dashboardInteraction.as(Ta)).set(e => {
+                }), new s("Title").check(() => null != this.title).set(e => this.title = qn.createFromJsonObject(e.value)).setXml(e => this.title = qn.createFromXml(e)), new s("Layout").check(() => null != this.layout).set(e => this.layout = $s.createFromJsonObject(e.value)).setXml(e => this.layout = $s.createFromXml(e)), new r("ForeColor", "", N.transparent), new n("Font").get(() => a.Serialize.fontArial8(this.font)).set(e => this.font = a.Deserialize.font(e.value, this.font)).setXml(e => this.font = L.System.Convert.toFont(e.textContent)), new i("DataMode", "", kn, kn.UsingDataFields), new n("ManuallyEnteredData"), new i("Style", "", o, o.Auto), new n("Group"), new n("CustomStyleName"), new n("Shadow").get(() => a.Serialize.jShadow(this.shadow)).set(e => this.shadow = a.Deserialize.simpleSahdow(e.value)).setXml(e => this.shadow = Ye.loadFromXml(e.textContent)), new s("ValueFormat").check(() => null != this.valueFormat).set(e => this.valueFormat = br.createFromJsonObject(e.value)).setXml(e => this.valueFormat = br.loadFormatFromXml(e, this.report)), new s("DashboardInteraction").check(() => null != this.dashboardInteraction.as(Ta)).set(e => {
                     var t;
                     let r = null == (t = qr.loadInteractionFromJsonObject(e.value)) ? void 0 : t.as(Ta);
                     null != r && (this.dashboardInteraction = r)
                 }).setXml(e => {
                     var t;
                     let r = null == (t = qr.loadInteractionFromXml(e)) ? void 0 : t.as(Ta);
                     null != r && (this.dashboardInteraction = r)
@@ -6146,15 +6148,15 @@
             getSeries() {
                 return this.series
             }
             getSeries2(e) {
                 return null != e ? d.Gauge.getSeries(e.as(F.e.StiMeter)) : null
             }
             createNewSeries() {
-                this.series = new Ts
+                this.series = new Fs
             }
             addTarget2(e) {
                 this.target = null != e ? d.Gauge.getTarget2(e) : null
             }
             addTarget(e) {
                 this.target = d.Gauge.getTarget(e.as(F.e.StiMeter))
             }
@@ -6187,52 +6189,52 @@
             removeRange(e) {
                 e < this.ranges.length && this.ranges.removeAt(e)
             }
             createdDefaultRanges() {
                 this.ranges.clear(), this.ranges.add(new Fa(N.red, "0", "33")), this.ranges.add(new Fa(N.yellow, "33", "66")), this.ranges.add(new Fa(N.green, "66", "100"))
             }
             getManuallyEnteredDataTable() {
-                if (this.dataMode != Vn.ManuallyEnteringData) return null;
+                if (this.dataMode != kn.ManuallyEnteringData) return null;
                 return F.e.StiManuallyEnteredDataParser.getGaugeDataTable(this.manuallyEnteredData, this)
             }
             async getGaugeComponent(e = null) {
                 let t = await bl.getOrCreate(this),
                     r = (new Aa).render2(this, null != e ? e : this.clientRectangle.size, t),
                     i = new L.Report.Components.StiGauge;
                 return 1 == (await r()).count2() && ((i = (await r()).firstOrDefault().gauge).report = this.report, i.page = this.page, i.name = this.name + `_Content`, i.clientRectangle = null != e ? new j(0, 0, e.width, e.height) : this.clientRectangle.clone(), i.brush = new v(this.backColor)), i
             }
             convertFrom(e) {
                 let t = e.fetchAllMeters();
                 if (null == t) return;
                 let r = t.firstOrDefault(e => e.is(Er)),
-                    i = (null != (r = null == r ? r = t.firstOrDefault(e => e.is(vt)) : r) && (this.value = null == this.value ? new F.T.StiValueGaugeMeter : this.value, this.value.loadFromJsonObject(r.saveToJsonObject(je.Report))), t.firstOrDefault(e => e.is(Ii))),
-                    s = (null != (i = null == i ? t.firstOrDefault(e => e.is(ze)) : i) && (this.series = null == this.series ? new Ts : this.series, this.series.loadFromJsonObject(i.saveToJsonObject(je.Report))), t.firstOrDefault(e => e.is(Di)));
+                    i = (null != (r = null == r ? r = t.firstOrDefault(e => e.is(vt)) : r) && (this.value = null == this.value ? new F.T.StiValueGaugeMeter : this.value, this.value.loadFromJsonObject(r.saveToJsonObject(je.Report))), t.firstOrDefault(e => e.is(Di))),
+                    s = (null != (i = null == i ? t.firstOrDefault(e => e.is(ze)) : i) && (this.series = null == this.series ? new Fs : this.series, this.series.loadFromJsonObject(i.saveToJsonObject(je.Report))), t.firstOrDefault(e => e.is(Ri)));
                 null != s && (this.target = null == this.target ? new F.T.StiTargetGaugeMeter : this.target, this.target.loadFromJsonObject(s.saveToJsonObject(je.Report))), null == this.dashboardInteraction && (this.dashboardInteraction = new Ta)
             }
             fetchAllMeters() {
                 let e = new P;
-                return this.dataMode == Vn.UsingDataFields && (null != this.value && e.add(this.value), null != this.series && e.add(this.series), null != this.target) && e.add(this.target), e
+                return this.dataMode == kn.UsingDataFields && (null != this.value && e.add(this.value), null != this.series && e.add(this.series), null != this.target) && e.add(this.target), e
             }
             getMeters() {
                 let r = new P;
-                if (this.dataMode == Vn.UsingDataFields) {
+                if (this.dataMode == kn.UsingDataFields) {
                     if (null != this.value && (this.value.key = pe.getOrGeneratedKey(this.value.key), r.add(this.value), this.calculationMode == L.Report["Gauge"].StiGaugeCalculationMode.Auto)) {
                         let e = new F.T.StiMinGaugeMeter,
-                            t = (e.key = this.value.key, e.expression = Rs.replaceFunction(this.value.expression, "Min"), r.add(e), new F.T.StiMaxGaugeMeter);
-                        t.key = this.value.key, t.expression = Rs.replaceFunction(this.value.expression, "Max"), r.add(t)
+                            t = (e.key = this.value.key, e.expression = Es.replaceFunction(this.value.expression, "Min"), r.add(e), new F.T.StiMaxGaugeMeter);
+                        t.key = this.value.key, t.expression = Es.replaceFunction(this.value.expression, "Max"), r.add(t)
                     }
                     null != this.series && r.add(this.series), null != this.target && r.add(this.target)
                 }
                 return r
             }
             retrieveUsedDataNames() {
-                return this.dataMode == Vn.UsingDataFields ? en.getMany(this.value, this.series, this.target) : null
+                return this.dataMode == kn.UsingDataFields ? tn.getMany(this.value, this.series, this.target) : null
             }
             get isDefined() {
-                return null != this.value || null != this.series || null != this.target || this.dataMode == Vn.ManuallyEnteringData
+                return null != this.value || null != this.series || null != this.target || this.dataMode == kn.ManuallyEnteringData
             }
             get style() {
                 return this._style
             }
             set style(e) {
                 (this._style = e) != o.Custom && (this.customStyleName = "")
             }
@@ -6255,16 +6257,20 @@
             }
             get toolboxPosition() {
                 return tt.GaugeElement
             }
             get localizedName() {
                 return A.get("Components", "StiGauge")
             }
+            static getValueFormatDefault() {
+                let e = new Wr;
+                return e.decimalDigits = 0, e.state = F.a.StiTextFormatState.DecimalDigits | F.a.StiTextFormatState.Abbreviation, e
+            }
             constructor(e = j.empty) {
-                super(e), this.dataMode = Vn.UsingDataFields, this.group = "", this.title = new qn, this.layout = new _s, this.crossFiltering = !0, this.shadow = new Ye, this.cornerRadius = new m(0), this.showBlanks = !1, this.font = new H("Arial", 13), this.foreColor = N.transparent, this.transformActions = new P, this.transformFilters = new P, this.transformSorts = new P, this.dataTransformation = {}, this.dataFilters = new P, this.userSorts = new P, this._style = o.Auto, this.customStyleName = "", this.helpUrl = "user-manual/dashboards_gauge.htm", this.valueFormat = new Wr(null, null, null, 0, null, null, null, null, null, F.a.StiTextFormatState.DecimalDigits | F.a.StiTextFormatState.Abbreviation), this.shortValue = !0, this.labels = new Da, this.targetSettings = new Ma, this.minimum = 0, this.maximum = 100, this.calculationMode = L.Report["Gauge"].StiGaugeCalculationMode.Auto, this.rangeMode = L.Report["Gauge"].StiGaugeRangeMode.Percentage, this.rangeType = L.Report["Gauge"].StiGaugeRangeType.None, this.type = L.Report["Gauge"].StiGaugeType.FullCircular, this.ranges = new P, this.isSampleForStyles = !1, this.title.text = this.localizedName, this.dashboardInteraction = new Ta, this.previousAnimations = new P
+                super(e), this.dataMode = kn.UsingDataFields, this.group = "", this.title = new qn, this.layout = new $s, this.crossFiltering = !0, this.shadow = new Ye, this.cornerRadius = new m(0), this.showBlanks = !1, this.font = new H("Arial", 13), this.foreColor = N.transparent, this.transformActions = new P, this.transformFilters = new P, this.transformSorts = new P, this.dataTransformation = {}, this.dataFilters = new P, this.userSorts = new P, this._style = o.Auto, this.customStyleName = "", this.helpUrl = "user-manual/dashboards_gauge.htm", this.valueFormat = vm.getValueFormatDefault(), this.shortValue = !0, this.labels = new Da, this.targetSettings = new Ma, this.minimum = 0, this.maximum = 100, this.calculationMode = L.Report["Gauge"].StiGaugeCalculationMode.Auto, this.rangeMode = L.Report["Gauge"].StiGaugeRangeMode.Percentage, this.rangeType = L.Report["Gauge"].StiGaugeRangeType.None, this.type = L.Report["Gauge"].StiGaugeType.FullCircular, this.ranges = new P, this.isSampleForStyles = !1, this.title.text = this.localizedName, this.dashboardInteraction = new Ta, this.previousAnimations = new P
             }
         }
         F.T.StiGaugeElement = vm
     }
     F.ab.StiGaugeRangeConverter = class {};
     let Ea = F.H.StiXChartMeter,
         Oa = F.H.StiStartValueChartMeter;
@@ -6273,135 +6279,135 @@
             if (B.isNullOrEmpty(e)) return null;
             let t, r = Zt.tryParse(e);
             return null != (t = r.successfully ? ve.parse(F.e.StiMeterIdent, r.result) : ve.parse(F.e.StiMeterIdent, e)) ? this.neww2(t) : null
         }
         static neww2(e) {
             switch (e) {
                 case F.e.StiMeterIdent.ArgumentChartMeter:
-                    return new Ls;
+                    return new Bs;
                 case F.e.StiMeterIdent.SeriesChartMeter:
-                    return new Ps;
+                    return new js;
                 case F.e.StiMeterIdent.SortByChartMeter:
-                    return new ki;
+                    return new Ni;
                 case F.e.StiMeterIdent.IndicatorValueChartMeter:
-                    return new Vi;
+                    return new ki;
                 case F.e.StiMeterIdent.ValueChartMeter:
-                    return new Bs;
+                    return new Ps;
                 case F.e.StiMeterIdent.StartValueChartMeter:
                     return new Oa;
                 case F.e.StiMeterIdent.EndValueChartMeter:
-                    return new js;
+                    return new Hs;
                 case F.e.StiMeterIdent.OpenValueChartMeter:
-                    return new Os;
-                case F.e.StiMeterIdent.CloseValueChartMeter:
                     return new Vs;
-                case F.e.StiMeterIdent.LowValueChartMeter:
+                case F.e.StiMeterIdent.CloseValueChartMeter:
                     return new ks;
-                case F.e.StiMeterIdent.HighValueChartMeter:
+                case F.e.StiMeterIdent.LowValueChartMeter:
                     return new Ns;
+                case F.e.StiMeterIdent.HighValueChartMeter:
+                    return new Ls;
                 case F.e.StiMeterIdent.WeightChartMeter:
-                    return new Es;
+                    return new Os;
                 case F.e.StiMeterIdent.XChartMeter:
                     return new Ea;
                 case F.e.StiMeterIdent.YChartMeter:
                     return new _n;
                 case F.e.StiMeterIdent.KeyComboBoxMeter:
-                    return new Ms;
+                    return new Ts;
                 case F.e.StiMeterIdent.NameComboBoxMeter:
-                    return new xs;
+                    return new Ms;
                 case F.e.StiMeterIdent.MaxGaugeMeter:
                     return new oa;
                 case F.e.StiMeterIdent.MinGaugeMeter:
                     return new aa;
                 case F.e.StiMeterIdent.SeriesGaugeMeter:
-                    return new Ts;
-                case F.e.StiMeterIdent.ValueGaugeMeter:
                     return new Fs;
-                case F.e.StiMeterIdent.TargetGaugeMeter:
+                case F.e.StiMeterIdent.ValueGaugeMeter:
                     return new vs;
-                case F.e.StiMeterIdent.SeriesIndicatorMeter:
+                case F.e.StiMeterIdent.TargetGaugeMeter:
                     return new As;
+                case F.e.StiMeterIdent.SeriesIndicatorMeter:
+                    return new Is;
                 case F.e.StiMeterIdent.TargetIndicatorMeter:
-                    return new Ds;
+                    return new Rs;
                 case F.e.StiMeterIdent.ValueIndicatorMeter:
-                    return new Is;
+                    return new Ds;
                 case F.e.StiMeterIdent.KeyListBoxMeter:
-                    return new ws;
-                case F.e.StiMeterIdent.NameListBoxMeter:
                     return new bs;
+                case F.e.StiMeterIdent.NameListBoxMeter:
+                    return new fs;
                 case F.e.StiMeterIdent.LatitudeMapMeter:
-                    return new ps;
-                case F.e.StiMeterIdent.LongitudeMapMeter:
                     return new Ss;
+                case F.e.StiMeterIdent.LongitudeMapMeter:
+                    return new ws;
                 case F.e.StiMeterIdent.LocationMapMeter:
-                    return new Wi;
+                    return new Ji;
                 case F.e.StiMeterIdent.LocationValueMapMeter:
-                    return new Ui;
+                    return new Zi;
                 case F.e.StiMeterIdent.LocationArgumentMapMeter:
-                    return new Xi;
+                    return new Wi;
                 case F.e.StiMeterIdent.LocationColorMapMeter:
-                    return new Ji;
+                    return new Ui;
                 case F.e.StiMeterIdent.KeyMapMeter:
-                    return new os;
+                    return new us;
                 case F.e.StiMeterIdent.NameMapMeter:
-                    return new as;
+                    return new os;
                 case F.e.StiMeterIdent.GroupMapMeter:
-                    return new ls;
+                    return new as;
                 case F.e.StiMeterIdent.ColorMapMeter:
-                    return new ss;
-                case F.e.StiMeterIdent.ValueMapMeter:
                     return new ns;
+                case F.e.StiMeterIdent.ValueMapMeter:
+                    return new ls;
                 case F.e.StiMeterIdent.PivotColumn:
-                    return new cs;
-                case F.e.StiMeterIdent.PivotRow:
                     return new ds;
-                case F.e.StiMeterIdent.PivotSummary:
+                case F.e.StiMeterIdent.PivotRow:
                     return new gs;
+                case F.e.StiMeterIdent.PivotSummary:
+                    return new ps;
                 case F.e.StiMeterIdent.SeriesProgressMeter:
-                    return new ms;
+                    return new cs;
                 case F.e.StiMeterIdent.TargetProgressMeter:
-                    return new hs;
+                    return new ms;
                 case F.e.StiMeterIdent.ValueProgressMeter:
-                    return new us;
+                    return new hs;
                 case F.e.StiMeterIdent.ColorScaleColumn:
-                    return new qi;
-                case F.e.StiMeterIdent.DataBarsColumn:
                     return new _i;
+                case F.e.StiMeterIdent.DataBarsColumn:
+                    return new $i;
                 case F.e.StiMeterIdent.DimensionColumn:
-                    return new rs;
+                    return new is;
                 case F.e.StiMeterIdent.IndicatorColumn:
-                    return new Qi;
+                    return new qi;
                 case F.e.StiMeterIdent.MeasureColumn:
-                    return new is;
+                    return new ss;
                 case F.e.StiMeterIdent.SparklinesColumn:
-                    return new $i;
+                    return new es;
                 case F.e.StiMeterIdent.BubbleColumn:
-                    return new Gi;
+                    return new Xi;
                 case F.e.StiMeterIdent.ColorScaleCardsColumn:
-                    return new Bi;
-                case F.e.StiMeterIdent.DataBarsCardsColumn:
                     return new Pi;
+                case F.e.StiMeterIdent.DataBarsCardsColumn:
+                    return new ji;
                 case F.e.StiMeterIdent.DimensionCardsColumn:
-                    return new Hi;
+                    return new zi;
                 case F.e.StiMeterIdent.IndicatorCardsColumn:
-                    return new Ni;
+                    return new Li;
                 case F.e.StiMeterIdent.MeasureCardsColumn:
                     return new Fr;
                 case F.e.StiMeterIdent.SparklinesCardsColumn:
-                    return new ji;
+                    return new Hi;
                 case F.e.StiMeterIdent.BubbleCardsColumn:
-                    return new Li;
+                    return new Bi;
                 case F.e.StiMeterIdent.KeyTreeViewMeter:
-                    return new Ki;
+                    return new Qi;
                 case F.e.StiMeterIdent.KeyTreeViewBoxMeter:
-                    return new Yi;
+                    return new Ki;
                 case F.e.StiMeterIdent.ValueDatePickerMeter:
-                    return new fs;
+                    return new ys;
                 case F.e.StiMeterIdent.ValueNumberBoxMeter:
-                    return new Oi;
+                    return new Vi;
                 default:
                     throw new ca(e)
             }
         }
     }, F.G.StiMeterJsonConverter = class {}, F.g.StiImageDashboardInteraction = class extends F.g.StiDashboardInteraction {
         isDefault() {
             return this.onHover == Vr.ShowToolTip && this.onClick == kr.OpenHyperlink && this.hyperlinkDestination == Nr.NewTab && B.isNullOrEmpty(this.hyperlink) && B.isNullOrEmpty(this.drillDownPageKey) && null != this.drillDownParameters && 0 == this.drillDownParameters.length && B.isNullOrEmpty(this.toolTip)
@@ -6433,15 +6439,15 @@
         ja = L.Report.Dashboard.Helpers.StiDashboardImageHyperlinkCache,
         Ha = L.Report.Dashboard.IStiImageElement,
         za = L.Report.StiFontIconsHelper;
     {
         dt.add("StiImageElement", "Stimulsoft.Dashboard.Export.Tools.StiImageElementExportTool");
         class Fm extends F.e.StiElement {
             implements() {
-                return Fm.ImplementsStiImageElement || (Fm.ImplementsStiImageElement = super.implements().concat([Cr, or, Ha, Ze, Ke, Oe, Ne, ...wr, ...ir, ...Ba, ...Ue, ...Qe, ...$s, l, Qr])), Fm.ImplementsStiImageElement
+                return Fm.ImplementsStiImageElement || (Fm.ImplementsStiImageElement = super.implements().concat([Cr, or, Ha, Ze, Ke, Oe, Ne, ...wr, ...ir, ...Ba, ...Ue, ...Qe, ...en, l, Qr])), Fm.ImplementsStiImageElement
             }
             clone(e) {
                 var t, r;
                 let i = super.clone(e);
                 return i.title = null != this.title ? this.title.clone() : null, i.shadow = null == (t = this.shadow) ? void 0 : t.clone(), i.cornerRadius = null == (r = this.cornerRadius) ? void 0 : r.clone(), i
             }
             meta() {
@@ -6467,15 +6473,15 @@
             getMeters() {
                 if (!this.isImageHyperlinkDataColumnDefined()) return new P;
                 let e = ka.getRealDataColumnFromHyperlink(this.report, this.imageHyperlink),
                     t = new P;
                 return t.add(new Va(e, e, e)), t
             }
             retrieveUsedDataNames() {
-                return en.getMany2(this.getMeters()).distinct().toList()
+                return tn.getMany2(this.getMeters()).distinct().toList()
             }
             get imageToDraw() {
                 if (this.isImageDefined) return new Promise(e => {
                     e(this.image)
                 });
                 if (this.isImageIconDefined) {
                     let e = this.getPaintRectangle(!0, !1);
@@ -6484,15 +6490,15 @@
                 if (this.isImageHyperlinkDefined) return new Promise(i => {
                     setTimeout(async () => {
                         if (this.isImageHyperlinkDataColumnDefined()) {
                             let r = await bl.getOrCreate(this);
                             if (null != r) {
                                 let e = r.rows.firstOrDefault(),
                                     t = null != e ? e[L.System.StiObject.stimulsoft]().toList().firstOrDefault() : null;
-                                if (Ln.isArray(t)) {
+                                if (Bn.isArray(t)) {
                                     let e = new L.System.Drawing.Image;
                                     e.bytes = t, i(e)
                                 } else if ("string" == typeof t && !B.isNullOrEmpty(t)) {
                                     if (t[L.System.StiObject.stimulsoft]().isBase64String()) {
                                         let e = new L.System.Drawing.Image;
                                         e.base64 = t, i(e)
                                     }
@@ -6570,15 +6576,15 @@
         }
         F.X.StiImageElement = Fm
     }
     F._.StiImageBytesConverter = class {};
     {
         class Ua extends F.g.StiDashboardInteraction {
             implements() {
-                return Ua.ImplementsIStiIndicatorDashboardInteraction || (Ua.ImplementsIStiIndicatorDashboardInteraction = super.implements().concat([An, l, Gs])), Ua.ImplementsIStiIndicatorDashboardInteraction
+                return Ua.ImplementsIStiIndicatorDashboardInteraction || (Ua.ImplementsIStiIndicatorDashboardInteraction = super.implements().concat([In, l, Xs])), Ua.ImplementsIStiIndicatorDashboardInteraction
             }
             meta() {
                 return [...super.meta(), new h("AllowUserDrillDown"), new h("AllowUserSorting", "", !0), new h("ShowFullScreenButton", "", !0), new h("ShowSaveButton", "", !0), new h("ShowViewDataButton", "", !0), new n("FileName"), new n("HeaderText"), new n("FooterText")]
             }
             get isDefaultLayout() {
                 return this.showFullScreenButton && this.showSaveButton && this.showViewDataButton && null == this.fileName && null == this.headerText && !this.allowUserDrillDown && null == this.footerText
             }
@@ -6601,41 +6607,41 @@
         Ka = L.Report.Helpers.StiFontIconSet,
         Qa = L.Report.Dashboard.IStiIndicatorElement,
         qa = L.System.Convert,
         _a = L.Report.Dashboard.StiFontSizeMode;
     {
         class fh extends F.e.StiElement {
             implements() {
-                return fh.ImplementsStiIndicatorElement || (fh.ImplementsStiIndicatorElement = super.implements().concat([yr, Qa, Ke, Ze, Oe, ar, fr, qs, Qr, Ne, Wa, Xs, ...$r, ...Za, ...Qe, ...Ue, ...$s, ...rr, ...Sr, ...Qs, ...Ya, l])), fh.ImplementsStiIndicatorElement
+                return fh.ImplementsStiIndicatorElement || (fh.ImplementsStiIndicatorElement = super.implements().concat([yr, Qa, Ke, Ze, Oe, ar, fr, _s, Qr, Ne, Wa, Ws, ...$r, ...Za, ...Qe, ...Ue, ...en, ...rr, ...Sr, ...qs, ...Ya, l])), fh.ImplementsStiIndicatorElement
             }
             clone(e) {
                 var t, r;
                 let i = super.clone(e);
                 return i.value = null != this.value ? this.value.clone() : null, i.target = null != this.target ? this.target.clone() : null, i.series = null != this.series ? this.series.clone() : null, i.userSorts = this.userSorts.select(e => e.clone()).toList(), i.transformActions = this.transformActions.select(e => e.clone()).toList(), i.transformFilters = this.transformFilters.select(e => e.clone()).toList(), i.transformSorts = this.transformSorts.select(e => e.clone()).toList(), i.dataFilters = this.dataFilters.select(e => e.clone()).toList(), i.topN = this.topN.clone(), i.textFormat = this.textFormat.clone(), i.targetFormat = this.targetFormat.clone(), i.title = null != this.title ? this.title.clone() : null, i.layout = null != this.layout ? this.layout.clone() : null, i.indicatorConditions = this.indicatorConditions.select(e => e.clone()).toList(), i.dashboardInteraction = this.dashboardInteraction.clone(), i.shadow = null == (t = this.shadow) ? void 0 : t.clone(), i.cornerRadius = null == (r = this.cornerRadius) ? void 0 : r.clone(), i
             }
             meta() {
-                return [...super.meta(), new s("UserSorts").get(e => a.Serialize.objectArray(this.userSorts, e)).set(e => this.userSorts.addRange(e.value.properties().select(e => rn.loadFromJson(e.value)))).setXml(e => this.userSorts.addRange(e.childNodes.select(e => rn.loadFromXml(e)))), new s("TransformActions").get(e => a.Serialize.objectArray(this.transformActions, e)).set(e => this.transformActions.addRange(e.value.properties().select(e => sn.loadFromJson(e.value)))).setXml(e => this.transformActions.addRange(e.childNodes.select(e => sn.loadFromXml(e)))), new s("TransformFilters").get(e => a.Serialize.objectArray(this.transformFilters, e)).set(e => this.transformFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.transformFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new s("TransformSorts").get(e => a.Serialize.objectArray(this.transformSorts, e)).set(e => this.transformSorts.addRange(e.value.properties().select(e => rn.loadFromJson(e.value)))).setXml(e => this.transformSorts.addRange(e.childNodes.select(e => rn.loadFromXml(e)))), new s("DataFilters").get(e => a.Serialize.objectArray(this.dataFilters, e)).set(e => this.dataFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.dataFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new s("IconRanges").get(e => a.Serialize.objectArray(this.iconRanges, e)).set(e => this.iconRanges.addRange(e.value.properties().select(e => F.U.StiIndicatorIconRange.loadFromJson(e.value)))).setXml(e => this.iconRanges.addRange(e.childNodes.select(e => F.U.StiIndicatorIconRange.loadFromXml(e)))), new h("CrossFiltering", "", !0), new s("TopN").check(() => null != this.topN).set(e => this.topN = Fi.createFromJsonObject(e.value)).setXml(e => this.topN = Fi.createFromXml(e)), new s("TextFormat").check(() => null != this.textFormat).set(e => this.textFormat = br.createFromJsonObject(e.value)).setXml(e => this.textFormat = br.loadFormatFromXml(e, this.report)), new s("TargetFormat").check(() => null != this.targetFormat).set(e => this.targetFormat = br.createFromJsonObject(e.value)).setXml(e => this.targetFormat = br.loadFormatFromXml(e, this.report)), new s("Value").check(() => null != this.value).set(e => {
-                    let t = g.loadFromJson(e.value).as(Is);
+                return [...super.meta(), new s("UserSorts").get(e => a.Serialize.objectArray(this.userSorts, e)).set(e => this.userSorts.addRange(e.value.properties().select(e => sn.loadFromJson(e.value)))).setXml(e => this.userSorts.addRange(e.childNodes.select(e => sn.loadFromXml(e)))), new s("TransformActions").get(e => a.Serialize.objectArray(this.transformActions, e)).set(e => this.transformActions.addRange(e.value.properties().select(e => nn.loadFromJson(e.value)))).setXml(e => this.transformActions.addRange(e.childNodes.select(e => nn.loadFromXml(e)))), new s("TransformFilters").get(e => a.Serialize.objectArray(this.transformFilters, e)).set(e => this.transformFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.transformFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new s("TransformSorts").get(e => a.Serialize.objectArray(this.transformSorts, e)).set(e => this.transformSorts.addRange(e.value.properties().select(e => sn.loadFromJson(e.value)))).setXml(e => this.transformSorts.addRange(e.childNodes.select(e => sn.loadFromXml(e)))), new s("DataFilters").get(e => a.Serialize.objectArray(this.dataFilters, e)).set(e => this.dataFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.dataFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new s("IconRanges").get(e => a.Serialize.objectArray(this.iconRanges, e)).set(e => this.iconRanges.addRange(e.value.properties().select(e => F.U.StiIndicatorIconRange.loadFromJson(e.value)))).setXml(e => this.iconRanges.addRange(e.childNodes.select(e => F.U.StiIndicatorIconRange.loadFromXml(e)))), new h("CrossFiltering", "", !0), new s("TopN").check(() => null != this.topN).set(e => this.topN = vi.createFromJsonObject(e.value)).setXml(e => this.topN = vi.createFromXml(e)), new s("TextFormat").check(() => null != this.textFormat).set(e => this.textFormat = br.createFromJsonObject(e.value)).setXml(e => this.textFormat = br.loadFormatFromXml(e, this.report)), new s("TargetFormat").check(() => null != this.targetFormat).set(e => this.targetFormat = br.createFromJsonObject(e.value)).setXml(e => this.targetFormat = br.loadFormatFromXml(e, this.report)), new s("Value").check(() => null != this.value).set(e => {
+                    let t = g.loadFromJson(e.value).as(Ds);
                     null != t && (this.value = t)
                 }).setXml(e => {
-                    let t = g.loadFromXml(e).as(Is);
+                    let t = g.loadFromXml(e).as(Ds);
                     null != t && (this.value = t)
                 }), new s("Target").check(() => null != this.target).set(e => {
                     let t = g.loadFromJson(e.value).as(F.U.StiTargetIndicatorMeter);
                     null != t && (this.target = t)
                 }).setXml(e => {
                     let t = g.loadFromXml(e).as(F.U.StiTargetIndicatorMeter);
                     null != t && (this.target = t)
                 }), new s("Series").check(() => null != this.series).set(e => {
                     let t = g.loadFromJson(e.value).as(F.U.StiSeriesIndicatorMeter);
                     null != t && (this.series = t)
                 }).setXml(e => {
                     let t = g.loadFromXml(e).as(F.U.StiSeriesIndicatorMeter);
                     null != t && (this.series = t)
-                }), new s("Title").check(() => null != this.title).set(e => this.title = F.e.StiTitle.createFromJsonObject(e.value)).setXml(e => this.title = F.e.StiTitle.createFromXml(e)), new s("Layout").check(() => null != this.layout).set(e => this.layout = _s.createFromJsonObject(e.value)).setXml(e => this.layout = _s.createFromXml(e)), new r("ForeColor", "", N.transparent), new r("GlyphColor", "", N.transparent), new n("Font").get(() => a.Serialize.fontArial8(this.font)).set(e => this.font = a.Deserialize.font(e.value, this.font)).setXml(e => this.font = L.System.Convert.toFont(e.textContent)), new i("DataMode", "", Vn, Vn.UsingDataFields), new n("ManuallyEnteredData"), new i("Style", "", o, o.Auto), new n("Group"), new n("CustomStyleName"), new i("Icon", "", kt, kt.Rating4), new i("IconSet", "", Ka, Ka.Rating), new i("IconMode", "", Xa, Xa.Auto), new i("IconRangeMode", "", Ga, Ga.Percentage), new ne("CustomIcon").check(() => null != this.customIcon).get(() => qa.toBase64String(this.customIcon)).set(e => this.customIcon = qa.fromBase64String(e.value.toString())).setXml(e => this.customIcon = qa.fromBase64String(e.textContent)), new i("IconAlignment", "", Ht, Ht.Right), new i("TargetMode", "", Ja, Ja.Variation), new i("FontSizeMode", "", _a, _a.Auto), new s("IndicatorConditions").get(e => a.Serialize.objectArray(this.indicatorConditions, e)).set(e => this.indicatorConditions.addRange(e.value.properties().select(e => F.U.StiIndicatorElementCondition.createFromJson(e.value)))).setXml(e => this.indicatorConditions.addRange(e.childNodes.select(e => F.U.StiIndicatorElementCondition.createFromXml(e)))), new n("CornerRadius").get(() => this.cornerRadius.toString()).set(e => this.cornerRadius = m.tryParse(e.value.toString())).setXml(e => this.cornerRadius = m.tryParse(e.textContent)), new n("Shadow").get(() => a.Serialize.jShadow(this.shadow)).set(e => this.shadow = a.Deserialize.simpleSahdow(e.value)).setXml(e => this.shadow = Ye.loadFromXml(e.textContent)), new s("DashboardInteraction").check(() => null != this.dashboardInteraction.as(Ua)).set(e => {
+                }), new s("Title").check(() => null != this.title).set(e => this.title = F.e.StiTitle.createFromJsonObject(e.value)).setXml(e => this.title = F.e.StiTitle.createFromXml(e)), new s("Layout").check(() => null != this.layout).set(e => this.layout = $s.createFromJsonObject(e.value)).setXml(e => this.layout = $s.createFromXml(e)), new r("ForeColor", "", N.transparent), new r("GlyphColor", "", N.transparent), new n("Font").get(() => a.Serialize.fontArial8(this.font)).set(e => this.font = a.Deserialize.font(e.value, this.font)).setXml(e => this.font = L.System.Convert.toFont(e.textContent)), new i("DataMode", "", kn, kn.UsingDataFields), new n("ManuallyEnteredData"), new i("Style", "", o, o.Auto), new n("Group"), new n("CustomStyleName"), new i("Icon", "", kt, kt.Rating4), new i("IconSet", "", Ka, Ka.Rating), new i("IconMode", "", Xa, Xa.Auto), new i("IconRangeMode", "", Ga, Ga.Percentage), new ne("CustomIcon").check(() => null != this.customIcon).get(() => qa.toBase64String(this.customIcon)).set(e => this.customIcon = qa.fromBase64String(e.value.toString())).setXml(e => this.customIcon = qa.fromBase64String(e.textContent)), new i("IconAlignment", "", Ht, Ht.Right), new i("TargetMode", "", Ja, Ja.Variation), new i("FontSizeMode", "", _a, _a.Auto), new s("IndicatorConditions").get(e => a.Serialize.objectArray(this.indicatorConditions, e)).set(e => this.indicatorConditions.addRange(e.value.properties().select(e => F.U.StiIndicatorElementCondition.createFromJson(e.value)))).setXml(e => this.indicatorConditions.addRange(e.childNodes.select(e => F.U.StiIndicatorElementCondition.createFromXml(e)))), new n("CornerRadius").get(() => this.cornerRadius.toString()).set(e => this.cornerRadius = m.tryParse(e.value.toString())).setXml(e => this.cornerRadius = m.tryParse(e.textContent)), new n("Shadow").get(() => a.Serialize.jShadow(this.shadow)).set(e => this.shadow = a.Deserialize.simpleSahdow(e.value)).setXml(e => this.shadow = Ye.loadFromXml(e.textContent)), new s("DashboardInteraction").check(() => null != this.dashboardInteraction.as(Ua)).set(e => {
                     var t;
                     let r = null == (t = qr.loadInteractionFromJsonObject(e.value)) ? void 0 : t.as(Ua);
                     null != r && (this.dashboardInteraction = r)
                 }).setXml(e => {
                     var t;
                     let r = null == (t = qr.loadInteractionFromXml(e)) ? void 0 : t.as(Ua);
                     null != r && (this.dashboardInteraction = r)
@@ -6653,15 +6659,15 @@
             getValue() {
                 return this.value
             }
             getValue2(e) {
                 return null != e ? d.Indicator.getValue(e.as(F.e.StiMeter)) : null
             }
             createNewValue() {
-                this.value = new Is, this.value.expression = "Sum()"
+                this.value = new Ds, this.value.expression = "Sum()"
             }
             addTarget2(e) {
                 this.target = null != e ? d.Indicator.getTarget2(e) : null
             }
             addTarget(e) {
                 this.target = d.Indicator.getTarget(e.as(F.e.StiMeter))
             }
@@ -6706,15 +6712,15 @@
             removeRange(e) {
                 e < this.iconRanges.length && this.iconRanges.removeAt(e)
             }
             createdDefaultRanges() {
                 this.iconRanges.clear(), this.iconRanges.add(new F.U.StiIndicatorIconRange(kt.Rating1, "0", "25")), this.iconRanges.add(new F.U.StiIndicatorIconRange(kt.Rating2, "25", "50")), this.iconRanges.add(new F.U.StiIndicatorIconRange(kt.Rating3, "50", "75")), this.iconRanges.add(new F.U.StiIndicatorIconRange(kt.Rating4, "75", "100"))
             }
             getManuallyEnteredDataTable() {
-                if (this.dataMode != Vn.ManuallyEnteringData) return null;
+                if (this.dataMode != kn.ManuallyEnteringData) return null;
                 return F.e.StiManuallyEnteredDataParser.getIndicatorDataTable(this.manuallyEnteredData, this)
             }
             addIndicatorCondition(e, t, r, i, s, n, l, a, o, u, h, m, c, d) {
                 this.indicatorConditions.add(new F.U.StiIndicatorElementCondition(e, t, r, i, s, n, l, a, o, u, h, m, c, d))
             }
             fetchIndicatorConditions() {
                 let e = new P;
@@ -6723,31 +6729,31 @@
             clearIndicatorConditions() {
                 this.indicatorConditions.clear()
             }
             convertFrom(e) {
                 let t = e.fetchAllMeters();
                 if (null == t) return;
                 let r = t.firstOrDefault(e => e.is(Er)),
-                    i = (null != (r = null == r ? t.firstOrDefault(e => e.is(vt)) : r) && (this.value = null == this.value ? new Is : this.value, this.value.loadFromJsonObject(r.saveToJsonObject(je.Report))), t.firstOrDefault(e => e.is(Di))),
-                    s = (null != i && (this.target = null == this.target ? new F.U.StiTargetIndicatorMeter : this.target, this.target.loadFromJsonObject(i.saveToJsonObject(je.Report))), t.firstOrDefault(e => e.is(Ii)));
+                    i = (null != (r = null == r ? t.firstOrDefault(e => e.is(vt)) : r) && (this.value = null == this.value ? new Ds : this.value, this.value.loadFromJsonObject(r.saveToJsonObject(je.Report))), t.firstOrDefault(e => e.is(Ri))),
+                    s = (null != i && (this.target = null == this.target ? new F.U.StiTargetIndicatorMeter : this.target, this.target.loadFromJsonObject(i.saveToJsonObject(je.Report))), t.firstOrDefault(e => e.is(Di)));
                 null != (s = null == s ? t.firstOrDefault(e => e.is(ze)) : s) && (this.series = null == this.series ? new F.U.StiSeriesIndicatorMeter : this.series, this.series.loadFromJsonObject(s.saveToJsonObject(je.Report))), null == this.dashboardInteraction && (this.dashboardInteraction = new Ua)
             }
             fetchAllMeters() {
                 let e = new P;
-                return this.dataMode == Vn.UsingDataFields && (null != this.value && e.add(this.value), null != this.target && e.add(this.target), null != this.series) && e.add(this.series), e
+                return this.dataMode == kn.UsingDataFields && (null != this.value && e.add(this.value), null != this.target && e.add(this.target), null != this.series) && e.add(this.series), e
             }
             getMeters() {
                 let e = new P;
-                return this.dataMode == Vn.UsingDataFields && (null != this.value && e.add(this.value), null != this.target && e.add(this.target), null != this.series) && e.add(this.series), e
+                return this.dataMode == kn.UsingDataFields && (null != this.value && e.add(this.value), null != this.target && e.add(this.target), null != this.series) && e.add(this.series), e
             }
             retrieveUsedDataNames() {
-                return this.dataMode == Vn.UsingDataFields ? en.getMany(this.value, this.target, this.series) : null
+                return this.dataMode == kn.UsingDataFields ? tn.getMany(this.value, this.target, this.series) : null
             }
             get isDefined() {
-                return null != this.value || null != this.target || null != this.series || this.dataMode == Vn.ManuallyEnteringData
+                return null != this.value || null != this.target || null != this.series || this.dataMode == kn.ManuallyEnteringData
             }
             get style() {
                 return this._style
             }
             set style(e) {
                 (this._style = e) != o.Custom && (this.customStyleName = "")
             }
@@ -6779,15 +6785,15 @@
                 let t = this.dashboardInteraction.drillDownPageKey;
                 if (pe.isEmptyKey(t)) return null;
                 let e = this.report.pages.toList().firstOrDefault(e => e.guid == t);
                 if (null == e) return null;
                 return new P([e])
             }
             constructor(e = j.empty) {
-                super(e), this.group = "", this.shadow = new Ye, this.cornerRadius = new m(0), this.dataMode = Vn.UsingDataFields, this.textFormat = new Jt, this.font = new H("Arial", 13), this.foreColor = N.transparent, this.showBlanks = !1, this.title = new F.e.StiTitle, this.layout = new _s, this.transformActions = new P, this.transformFilters = new P, this.transformSorts = new P, this.topN = new Fi, this.dataTransformation = {}, this.dataFilters = new P, this.userSorts = new P, this._style = o.Auto, this.customStyleName = "", this.defaultClientRectangle = new j(0, 0, 160, 160), this.helpUrl = "user-manual/dashboards_indicator.htm", this.glyphColor = N.transparent, this.targetFormat = new Ur, this.icon = kt.Rating4, this.iconSet = Ka.Rating, this.iconAlignment = Ht.Right, this.targetMode = Ja.Variation, this.fontSizeMode = _a.Auto, this.iconMode = Xa.Auto, this.iconRangeMode = Ga.Percentage, this.iconRanges = new P, this.indicatorConditions = new P, this.crossFiltering = !0, this.isSampleForStyles = !1, this.title.text = this.localizedName, this.dashboardInteraction = new Ua
+                super(e), this.group = "", this.shadow = new Ye, this.cornerRadius = new m(0), this.dataMode = kn.UsingDataFields, this.textFormat = new Jt, this.font = new H("Arial", 13), this.foreColor = N.transparent, this.showBlanks = !1, this.title = new F.e.StiTitle, this.layout = new $s, this.transformActions = new P, this.transformFilters = new P, this.transformSorts = new P, this.topN = new vi, this.dataTransformation = {}, this.dataFilters = new P, this.userSorts = new P, this._style = o.Auto, this.customStyleName = "", this.defaultClientRectangle = new j(0, 0, 160, 160), this.helpUrl = "user-manual/dashboards_indicator.htm", this.glyphColor = N.transparent, this.targetFormat = new Ur, this.icon = kt.Rating4, this.iconSet = Ka.Rating, this.iconAlignment = Ht.Right, this.targetMode = Ja.Variation, this.fontSizeMode = _a.Auto, this.iconMode = Xa.Auto, this.iconRangeMode = Ga.Percentage, this.iconRanges = new P, this.indicatorConditions = new P, this.crossFiltering = !0, this.isSampleForStyles = !1, this.title.text = this.localizedName, this.dashboardInteraction = new Ua
             }
         }
         F.U.StiIndicatorElement = fh
     }
     let $a = L.Report.Dashboard.IStiIndicatorElementCondition,
         eo = L.Report.Dashboard.StiIndicatorFieldCondition,
         to = L.Report.Dashboard.StiIndicatorConditionPermissions;
@@ -6870,33 +6876,33 @@
     let so = L.Report.Dashboard.StiListBoxSelectionType,
         no = L.Report.Dashboard.ImplementsIStiListBoxElement,
         lo = L.Report.Dashboard.IStiListBoxElement;
     {
         dt.add("StiListBoxElement", "Stimulsoft.Dashboard.Export.Tools.StiListBoxElementExportTool");
         class pm extends F.e.StiElement {
             implements() {
-                return pm.ImplementsStiListBoxElement || (pm.ImplementsStiListBoxElement = super.implements().concat([lo, Ke, Ze, Oe, Ne, ...no, ...Qe, ...Ue, ...$s, l, Qr])), pm.ImplementsStiListBoxElement
+                return pm.ImplementsStiListBoxElement || (pm.ImplementsStiListBoxElement = super.implements().concat([lo, Ke, Ze, Oe, Ne, ...no, ...Qe, ...Ue, ...en, l, Qr])), pm.ImplementsStiListBoxElement
             }
             clone(e) {
                 var t, r, i;
                 let s = super.clone(e);
                 return s.keyMeter = null != this.keyMeter ? this.keyMeter.clone() : null, s.nameMeter = null != this.nameMeter ? this.nameMeter.clone() : null, s.userFilters = this.userFilters.select(e => e.clone()).toList(), s.transformActions = this.transformActions.select(e => e.clone()).toList(), s.transformFilters = this.transformFilters.select(e => e.clone()).toList(), s.transformSorts = this.transformSorts.select(e => e.clone()).toList(), s.dataFilters = this.dataFilters.select(e => e.clone()).toList(), s.textFormat = this.textFormat.clone(), s.title = null != this.title ? this.title.clone() : null, s.shadow = null == (t = this.shadow) ? void 0 : t.clone(), s.cornerRadius = null == (r = this.cornerRadius) ? void 0 : r.clone(), s.dashboardInteraction = null == (i = this.dashboardInteraction) ? void 0 : i.clone(), s
             }
             meta() {
-                return [...super.meta(), new n("ParentKey"), new n("InitialValue"), new s("UserFilters").get(e => a.Serialize.objectArray(this.userFilters, e)).set(e => this.userFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.userFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new s("TransformActions").get(e => a.Serialize.objectArray(this.transformActions, e)).set(e => this.transformActions.addRange(e.value.properties().select(e => sn.loadFromJson(e.value)))).setXml(e => this.transformActions.addRange(e.childNodes.select(e => sn.loadFromXml(e)))), new s("TransformFilters").get(e => a.Serialize.objectArray(this.transformFilters, e)).set(e => this.transformFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.transformFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new s("TransformSorts").get(e => a.Serialize.objectArray(this.transformSorts, e)).set(e => this.transformSorts.addRange(e.value.properties().select(e => rn.loadFromJson(e.value)))).setXml(e => this.transformSorts.addRange(e.childNodes.select(e => rn.loadFromXml(e)))), new s("DataFilters").get(e => a.Serialize.objectArray(this.dataFilters, e)).set(e => this.dataFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.dataFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new r("ForeColor", "", N.transparent), new n("Font").get(() => a.Serialize.fontArial8(this.font)).set(e => this.font = a.Deserialize.font(e.value, this.font)).setXml(e => this.font = L.System.Convert.toFont(e.textContent)), new h("ShowAllValue"), new h("ShowBlanks"), new i("SelectionMode", "", gl, gl.One).set(e => {
+                return [...super.meta(), new n("ParentKey"), new n("InitialValue"), new s("UserFilters").get(e => a.Serialize.objectArray(this.userFilters, e)).set(e => this.userFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.userFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new s("TransformActions").get(e => a.Serialize.objectArray(this.transformActions, e)).set(e => this.transformActions.addRange(e.value.properties().select(e => nn.loadFromJson(e.value)))).setXml(e => this.transformActions.addRange(e.childNodes.select(e => nn.loadFromXml(e)))), new s("TransformFilters").get(e => a.Serialize.objectArray(this.transformFilters, e)).set(e => this.transformFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.transformFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new s("TransformSorts").get(e => a.Serialize.objectArray(this.transformSorts, e)).set(e => this.transformSorts.addRange(e.value.properties().select(e => sn.loadFromJson(e.value)))).setXml(e => this.transformSorts.addRange(e.childNodes.select(e => sn.loadFromXml(e)))), new s("DataFilters").get(e => a.Serialize.objectArray(this.dataFilters, e)).set(e => this.dataFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.dataFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new r("ForeColor", "", N.transparent), new n("Font").get(() => a.Serialize.fontArial8(this.font)).set(e => this.font = a.Deserialize.font(e.value, this.font)).setXml(e => this.font = L.System.Convert.toFont(e.textContent)), new h("ShowAllValue"), new h("ShowBlanks"), new i("SelectionMode", "", gl, gl.One).set(e => {
                     let t = ve.parse(gl, e.value);
                     null != t && (this.selectionMode = t)
                 }).setXml(e => {
                     let t = ve.parse(gl, e.textContent);
                     null != t && (this.selectionMode = t)
-                }), new i("Orientation", "", Ys, Ys.Vertical), new i("SelectionType", "", so, so.ListBox), new s("NameMeter").check(() => null != this.nameMeter).set(e => {
-                    let t = g.loadFromJson(e.value).as(bs);
+                }), new i("Orientation", "", Ks, Ks.Vertical), new i("SelectionType", "", so, so.ListBox), new s("NameMeter").check(() => null != this.nameMeter).set(e => {
+                    let t = g.loadFromJson(e.value).as(fs);
                     null != t && (this.nameMeter = t)
                 }).setXml(e => {
-                    let t = g.loadFromXml(e).as(bs);
+                    let t = g.loadFromXml(e).as(fs);
                     null != t && (this.nameMeter = t)
                 }), new s("KeyMeter").check(() => null != this.keyMeter).set(e => {
                     let t = g.loadFromJson(e.value).as(F.P.StiKeyListBoxMeter);
                     null != t && (this.keyMeter = t)
                 }).setXml(e => {
                     let t = g.loadFromXml(e).as(F.P.StiKeyListBoxMeter);
                     null != t && (this.keyMeter = t)
@@ -6921,15 +6927,15 @@
                 return null != this.nameMeter && e.add(this.nameMeter), null != this.keyMeter && e.add(this.keyMeter), e
             }
             getMeters() {
                 let e = new P;
                 return null != this.nameMeter && e.add(this.nameMeter), null != this.keyMeter && e.add(this.keyMeter), e
             }
             retrieveUsedDataNames() {
-                return en.getMany(this.nameMeter, this.keyMeter)
+                return tn.getMany(this.nameMeter, this.keyMeter)
             }
             get isDefined() {
                 return null != this.nameMeter || null != this.keyMeter
             }
             getParentKey() {
                 return this.parentKey
             }
@@ -6964,25 +6970,25 @@
             getNameMeter() {
                 return this.nameMeter
             }
             removeNameMeter() {
                 this.nameMeter = null
             }
             createNewNameMeter() {
-                this.nameMeter = new bs
+                this.nameMeter = new fs
             }
             createNextMeter(e) {
                 null != this.keyMeter && null == this.nameMeter ? this.nameMeter = d.ListBox.getName2(e) : this.keyMeter = d.ListBox.getKey2(e)
             }
             convertFrom(e) {
                 let t = e.fetchAllMeters();
                 if (null == t) return;
                 let r = t.firstOrDefault(e => e.is(Er)),
                     i = (null != (r = null == r ? t.firstOrDefault(e => e.is(vt)) : r) && (this.keyMeter = null == this.keyMeter ? new F.P.StiKeyListBoxMeter : this.keyMeter, this.keyMeter.loadFromJsonObject(r.saveToJsonObject(je.Report))), t.firstOrDefault(e => e.is(Er)));
-                null != (i = null == i ? t.firstOrDefault(e => e.is(ze)) : i) && (this.nameMeter = null == this.nameMeter ? new bs : this.nameMeter, this.nameMeter.loadFromJsonObject(i.saveToJsonObject(je.Report)))
+                null != (i = null == i ? t.firstOrDefault(e => e.is(ze)) : i) && (this.nameMeter = null == this.nameMeter ? new fs : this.nameMeter, this.nameMeter.loadFromJsonObject(i.saveToJsonObject(je.Report)))
             }
             setString(e, t) {
                 switch (e) {
                     case "Title.Text":
                         this.title.text = t;
                         break
                 }
@@ -7000,15 +7006,15 @@
             get toolboxPosition() {
                 return tt.ListBoxElement
             }
             get localizedName() {
                 return A.get("Components", "StiListBox")
             }
             constructor(e = j.empty) {
-                super(e), this.group = "", this._style = o.Auto, this.customStyleName = "", this.showAllValue = !1, this.showBlanks = !1, this.selectionMode = gl.One, this.orientation = Ys.Vertical, this.selectionType = so.ListBox, this.title = new F.e.StiTitle, this.shadow = new Ye, this.cornerRadius = new m(0), this.userFilters = new P, this.transformActions = new P, this.transformFilters = new P, this.transformSorts = new P, this.dataTransformation = {}, this.dataFilters = new P, this.font = new H("Arial", 8), this.foreColor = N.transparent, this.textFormat = new Jt, this.defaultClientRectangle = new j(0, 0, 200, 300), this.helpUrl = "user-manual/dashboards_data_filtering_list_box.htm", this.title.text = this.localizedName, this.title.visible = !1, this.dashboardInteraction = new cl
+                super(e), this.group = "", this._style = o.Auto, this.customStyleName = "", this.showAllValue = !1, this.showBlanks = !1, this.selectionMode = gl.One, this.orientation = Ks.Vertical, this.selectionType = so.ListBox, this.title = new F.e.StiTitle, this.shadow = new Ye, this.cornerRadius = new m(0), this.userFilters = new P, this.transformActions = new P, this.transformFilters = new P, this.transformSorts = new P, this.dataTransformation = {}, this.dataFilters = new P, this.font = new H("Arial", 8), this.foreColor = N.transparent, this.textFormat = new Jt, this.defaultClientRectangle = new j(0, 0, 200, 300), this.helpUrl = "user-manual/dashboards_data_filtering_list_box.htm", this.title.text = this.localizedName, this.title.visible = !1, this.dashboardInteraction = new cl
             }
         }
         F.P.StiListBoxElement = pm
     }
     F.P.StiListBoxHelper = class {
         static fetchItems(i, e, s) {
             if (null == e || e == Tt.nullTable || 0 == e.rows.length) return null;
@@ -7074,15 +7080,15 @@
             if (null != e.nameMeter) return e.nameMeter.expression;
             return null
         }
         static format(e, t) {
             var r;
             if (t instanceof w && !e.textFormat.is(Xr)) return t.toShortDateString();
             let i = null == (r = null == e ? void 0 : e.report) ? void 0 : r.culture;
-            if (li.isEligable(t, i)) return li.convert(t, i);
+            if (ai.isEligable(t, i)) return ai.convert(t, i);
             return e.textFormat.format(t)
         }
     }, F.P.StiListBoxItem = class {
         toString() {
             return null != this.label ? this.label : this.value.toString()
         }
         constructor(e, t = e) {
@@ -7102,15 +7108,15 @@
                     r = V.tryToNumber(O.parse2(e.initialToValue, e.report)),
                     i = await this.getMinMaxRange(e);
                 return t = Math.max(t, i.from), t = Math.min(t, i.to), r = Math.max(r, i.from), r = Math.min(r, i.to), new ao(t, r)
             }
             static async getSingleInitialValue(t) {
                 var e;
                 let r = null,
-                    i = null == (e = this.getVariableSpecifiedAsValue(t)) ? void 0 : e.as(zs);
+                    i = null == (e = this.getVariableSpecifiedAsValue(t)) ? void 0 : e.as(Gs);
                 if (null != i) {
                     let e = t.report.dictionary.getVariableValueByName(i.name);
                     i.initBy != Rl.Expression || B.isNullOrEmpty(e) || (e = Dl.parseTextValue(`{${e}}`, t)), L.System.Type.isNumericType(i.type) && (r = V.tryToNullableNumber(e))
                 } else B.isNullOrEmpty(t.initialValue) || (r = V.tryToNullableNumber(O.parse2(t.initialValue, t.report, !0)));
                 let s = await this.getMinMaxRange(t);
                 return r = null != r ? (r = Math.max(Zt.getValueOrDefault(r), s.from), Math.min(Zt.getValueOrDefault(r), s.to)) : s.from, Zt.getValueOrDefault(r)
             }
@@ -7120,15 +7126,15 @@
             }
             static async getSingleDefaultUserFilters(e, t) {
                 let r = await this.getSingleInitialValue(e);
                 return new f("", t, this.getCondition(e), e.textFormat.format(r)).toList()
             }
             static async getRangeDefaultUserFilters(e, t) {
                 let r = await this.getRangeInitialValue(e);
-                return new f("", t, Zi.Between, e.textFormat.format(r.from), e.textFormat.format(r.to), !0, !1).toList()
+                return new f("", t, Yi.Between, e.textFormat.format(r.from), e.textFormat.format(r.to), !0, !1).toList()
             }
             static async getAutoRange(e) {
                 let t = this.getValueMeterExpression(e);
                 if (!B.isNullOrEmpty(t)) {
                     let t = await bl.getOrCreate(e);
                     if (null != t) {
                         let e = t.rows.select(e => e[0]).where(e => null != e && L.System.Type.isNumericType(L.System.Type.getType(e))).select(e => V.tryToNumber(e));
@@ -7140,36 +7146,36 @@
             static getValueMeterExpression(e) {
                 var t;
                 return null == (t = e.valueMeter) ? void 0 : t.expression
             }
             static getCondition(e) {
                 switch (e.condition) {
                     case uo.EqualTo:
-                        return Zi.EqualTo;
+                        return Yi.EqualTo;
                     case uo.NotEqualTo:
-                        return Zi.NotEqualTo;
+                        return Yi.NotEqualTo;
                     case uo.GreaterThan:
-                        return Zi.GreaterThan;
+                        return Yi.GreaterThan;
                     case uo.GreaterThanOrEqualTo:
-                        return Zi.GreaterThanOrEqualTo;
+                        return Yi.GreaterThanOrEqualTo;
                     case uo.LessThan:
-                        return Zi.LessThan;
+                        return Yi.LessThan;
                     case uo.LessThanOrEqualTo:
-                        return Zi.LessThanOrEqualTo;
+                        return Yi.LessThanOrEqualTo;
                     default:
-                        return Zi.EqualTo
+                        return Yi.EqualTo
                 }
             }
             static getVariableSpecifiedAsValue(e) {
                 var t;
                 return El.getVariableSpecifiedAsExpression(e, null == (t = e.getValueMeter()) ? void 0 : t.expression)
             }
             static isRange(t) {
                 if (this.isVariableSpecifiedAsValue(t)) {
-                    let e = this.getVariableSpecifiedAsValue(t).as(zs);
+                    let e = this.getVariableSpecifiedAsValue(t).as(Gs);
                     return null != e && Al.isNumericRangeType(e.type)
                 }
                 return t.selectionMode == oo.Range
             }
             static isVariableSpecifiedAsValue(e) {
                 var t;
                 return El.isVariableSpecifiedAsExpression(e, null == (t = e.getValueMeter()) ? void 0 : t.expression)
@@ -7195,33 +7201,33 @@
                 return [...super.meta(), new s("DataFilters").get(e => a.Serialize.objectArray(this.dataFilters, e)).set(e => this.dataFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.dataFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new r("ForeColor", "", N.transparent), new n("Font").get(() => a.Serialize.fontArial8(this.font)).set(e => this.font = a.Deserialize.font(e.value, this.font)).setXml(e => this.font = L.System.Convert.toFont(e.textContent)), new i("Condition", "", uo, uo.GreaterThanOrEqualTo), new i("MinMaxMode​", "", ho, ho.Auto), new i("SelectionMode", "", oo, oo.Single).set(e => {
                     let t = ve.parse(oo, e.value);
                     null != t && (this.selectionMode = t)
                 }).setXml(e => {
                     let t = ve.parse(oo, e.textContent);
                     null != t && (this.selectionMode = t)
                 }), new n("InitialValue"), new n("InitialToValue"), new n("Min"), new n("Max"), new se("DecimalDigits", "", 0), new i("HorAlignment", "", z, z.Center), new s("ValueMeter").check(() => null != this.valueMeter).set(e => {
-                    let t = g.loadFromJson(e.value).as(Oi);
+                    let t = g.loadFromJson(e.value).as(Vi);
                     null != t && (this.valueMeter = t)
                 }).setXml(e => {
-                    let t = g.loadFromXml(e).as(Oi);
+                    let t = g.loadFromXml(e).as(Vi);
                     null != t && (this.valueMeter = t)
                 }), new i("Style", "", o, o.Auto), new n("Group"), new n("CustomStyleName"), new n("CornerRadius").get(() => this.cornerRadius.toString()).set(e => this.cornerRadius = m.tryParse(e.value.toString())).setXml(e => this.cornerRadius = m.tryParse(e.textContent)), new n("Shadow").get(() => a.Serialize.jShadow(this.shadow)).set(e => this.shadow = a.Deserialize.simpleSahdow(e.value)).setXml(e => this.shadow = Ye.loadFromXml(e.textContent)), new le("MinSize"), new le("MaxSize")]
             }
             clone(e) {
                 var t, r;
                 let i = super.clone(e);
                 return i.valueMeter = null != this.valueMeter ? this.valueMeter.clone() : null, i.userFilters = this.userFilters.select(e => e.clone()).toList(), i.dataFilters = this.dataFilters.select(e => e.clone()).toList(), i.shadow = null == (t = this.shadow) ? void 0 : t.clone(), i.cornerRadius = null == (r = this.cornerRadius) ? void 0 : r.clone(), i
             }
             getParentKey() {
                 return null
             }
             setParentKey(e) {}
             async applyDefaultFilters() {
                 var e;
-                let i = null == (e = mo.getVariableSpecifiedAsValue(this)) ? void 0 : e.as(zs);
+                let i = null == (e = mo.getVariableSpecifiedAsValue(this)) ? void 0 : e.as(Gs);
                 if (null == i) {
                     let e = await mo.fetchDefaultUserFilters(this);
                     null != e && (this.userFilters = e)
                 } else if (Al.isRangeType(i.type)) {
                     let e = 0,
                         t = 0,
                         r = new L.Report.DecimalRange(e, t);
@@ -7239,15 +7245,15 @@
                 return null != this.valueMeter && e.add(this.valueMeter), e
             }
             getMeters() {
                 let e = new P;
                 return e.add(this.valueMeter), e
             }
             retrieveUsedDataNames() {
-                return en.getMany(this.valueMeter)
+                return tn.getMany(this.valueMeter)
             }
             get isDefined() {
                 return null != this.valueMeter
             }
             addValueMeter2(e) {
                 this.valueMeter = null != e ? d.NumberBox.getValue2(e) : null
             }
@@ -7257,21 +7263,21 @@
             getValueMeter() {
                 return this.valueMeter
             }
             removeValueMeter() {
                 this.valueMeter = null
             }
             createNewValueMeter() {
-                this.valueMeter = new Oi
+                this.valueMeter = new Vi
             }
             convertFrom(e) {
                 let t = e.fetchAllMeters();
                 if (null == t) return;
                 let r = t.firstOrDefault(e => e.is(Er));
-                null != (r = null == r ? t.firstOrDefault(e => e.is(vt)) : r) && (this.valueMeter = null == this.valueMeter ? new Oi : this.valueMeter, this.valueMeter.loadFromJsonObject(r.saveToJsonObject(je.Report)))
+                null != (r = null == r ? t.firstOrDefault(e => e.is(vt)) : r) && (this.valueMeter = null == this.valueMeter ? new Vi : this.valueMeter, this.valueMeter.loadFromJsonObject(r.saveToJsonObject(je.Report)))
             }
             get textFormat() {
                 let e = new Wr;
                 return e.decimalDigits = this.decimalDigits, e.state = L.Report.Components.StiTextFormatState.DecimalDigits, e
             }
             getFonts() {
                 let e = super.getFonts();
@@ -7301,15 +7307,15 @@
                 super(e), this.group = "", this.userFilters = new P, this.dataFilters = new P, this._style = o.Auto, this.customStyleName = "", this.font = new H("Arial", 8), this.foreColor = N.transparent, this.shadow = new Ye, this.cornerRadius = new m(0), this.horAlignment = z.Center, this.defaultClientRectangle = new j(0, 0, 200, 40), this.helpUrl = "user-manual/dashboards_data_filtering_number_box.htm", this.decimalDigits = 0, this.condition = uo.GreaterThanOrEqualTo, this.selectionMode = oo.Single, this.minMaxMode = ho.Auto, this.initialValue = "", this.initialToValue = "", this.min = "", this.max = ""
             }
         }
         F.R.StiNumberBoxElement = Im
     } {
         class po extends F.g.StiDashboardInteraction {
             implements() {
-                return po.ImplementsIStiOnlineMapDashboardInteraction || (po.ImplementsIStiOnlineMapDashboardInteraction = super.implements().concat([l, Gs])), po.ImplementsIStiOnlineMapDashboardInteraction
+                return po.ImplementsIStiOnlineMapDashboardInteraction || (po.ImplementsIStiOnlineMapDashboardInteraction = super.implements().concat([l, Xs])), po.ImplementsIStiOnlineMapDashboardInteraction
             }
             meta() {
                 return [...super.meta(), new h("ShowFullScreenButton", "", !0), new h("ShowSaveButton", "", !0), new h("ShowViewDataButton", "", !0), new n("FileName"), new n("HeaderText"), new n("FooterText")]
             }
             get isDefaultLayout() {
                 return this.showFullScreenButton && this.showSaveButton && this.showViewDataButton && null == this.fileName && null == this.headerText && null == this.footerText
             }
@@ -7329,23 +7335,23 @@
         fo = L.Report.Dashboard.StiOnlineMapCulture,
         yo = L.Report.Dashboard.StiOnlineMapLocationColorType,
         Co = L.Report.Dashboard.StiOnlineMapValueViewMode;
     {
         dt.add("StiOnlineMapElement", "Stimulsoft.Dashboard.Export.Tools.StiOnlineMapElementExportTool");
         class Mm extends F.e.StiElement {
             implements() {
-                return Mm.ImplementsStiOnlineMapElement || (Mm.ImplementsStiOnlineMapElement = super.implements().concat([wo, Ke, Ze, Oe, qs, Qr, Ne, ...So, ...Qe, ...Ue, ...$s, ...Qs, l])), Mm.ImplementsStiOnlineMapElement
+                return Mm.ImplementsStiOnlineMapElement || (Mm.ImplementsStiOnlineMapElement = super.implements().concat([wo, Ke, Ze, Oe, _s, Qr, Ne, ...So, ...Qe, ...Ue, ...en, ...qs, l])), Mm.ImplementsStiOnlineMapElement
             }
             clone(e) {
                 var t, r;
                 let i = super.clone(e);
                 return i.latitude = null != this.latitude ? this.latitude.clone() : null, i.longitude = null != this.longitude ? this.longitude.clone() : null, i.location = null != this.location ? this.location.clone() : null, i.locationColorMeter = null != this.locationColorMeter ? this.locationColorMeter.clone() : null, i.locationValue = null != this.locationValue ? this.locationValue.clone() : null, i.locationArgument = null != this.locationArgument ? this.locationArgument.clone() : null, i.transformActions = this.transformActions.select(e => e.clone()).toList(), i.transformFilters = this.transformFilters.select(e => e.clone()).toList(), i.transformSorts = this.transformSorts.select(e => e.clone()).toList(), i.dataFilters = this.dataFilters.select(e => e.clone()).toList(), i.title = null != this.title ? this.title.clone() : null, i.layout = null != this.layout ? this.layout.clone() : null, i.locationType = this.locationType, i.culture = this.culture, i.locationColorType = this.locationColorType, i.locationColor = this.locationColor, i.iconColor = this.iconColor, i.icon = this.icon, i.customIcon = null != this.customIcon ? qa.fromBase64String(qa.toBase64String(this.customIcon)) : null, i.dashboardInteraction = this.dashboardInteraction.clone(), i.shadow = null == (t = this.shadow) ? void 0 : t.clone(), i.cornerRadius = null == (r = this.cornerRadius) ? void 0 : r.clone(), i.onePointZoom = this.onePointZoom, i.userBingKey = this.userBingKey, i
             }
             meta() {
-                return [...super.meta(), new s("TransformActions").get(e => a.Serialize.objectArray(this.transformActions, e)).set(e => this.transformActions.addRange(e.value.properties().select(e => sn.loadFromJson(e.value)))).setXml(e => this.transformActions.addRange(e.childNodes.select(e => sn.loadFromXml(e)))), new s("TransformFilters").get(e => a.Serialize.objectArray(this.transformFilters, e)).set(e => this.transformFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.transformFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new s("TransformSorts").get(e => a.Serialize.objectArray(this.transformSorts, e)).set(e => this.transformSorts.addRange(e.value.properties().select(e => rn.loadFromJson(e.value)))).setXml(e => this.transformSorts.addRange(e.childNodes.select(e => rn.loadFromXml(e)))), new s("DataFilters").get(e => a.Serialize.objectArray(this.dataFilters, e)).set(e => this.dataFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.dataFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new s("Title").check(() => null != this.title).set(e => this.title = F.e.StiTitle.createFromJsonObject(e.value)).setXml(e => this.title = F.e.StiTitle.createFromXml(e)), new s("Layout").check(() => null != this.layout).set(e => this.layout = _s.createFromJsonObject(e.value)).setXml(e => this.layout = _s.createFromXml(e)), new s("Latitude").check(() => null != this.latitude).set(e => this.latitude = g.loadFromJson(e.value).as(F.O.StiLatitudeMapMeter)).setXml(e => this.latitude = g.loadFromXml(e).as(F.O.StiLatitudeMapMeter)), new s("Longitude").check(() => null != this.longitude).set(e => this.longitude = g.loadFromJson(e.value).as(F.O.StiLongitudeMapMeter)).setXml(e => this.longitude = g.loadFromXml(e).as(F.O.StiLongitudeMapMeter)), new s("Location").check(() => null != this.location).set(e => this.location = g.loadFromJson(e.value).as(F.O.StiLocationMapMeter)).setXml(e => this.location = g.loadFromXml(e).as(F.O.StiLocationMapMeter)), new s("LocationColorMeter").check(() => null != this.locationColorMeter).set(e => this.locationColorMeter = g.loadFromJson(e.value).as(F.O.StiLocationColorMapMeter)).setXml(e => this.locationColorMeter = g.loadFromXml(e).as(F.O.StiLocationColorMapMeter)), new s("LocationArgument").check(() => null != this.locationArgument).set(e => this.locationArgument = g.loadFromJson(e.value).as(F.O.StiLocationArgumentMapMeter)).setXml(e => this.locationArgument = g.loadFromXml(e).as(F.O.StiLocationArgumentMapMeter)), new s("LocationValue").check(() => null != this.locationValue).set(e => this.locationValue = g.loadFromJson(e.value).as(F.O.StiLocationValueMapMeter)).setXml(e => this.locationValue = g.loadFromXml(e).as(F.O.StiLocationValueMapMeter)), new n("Group"), new i("Culture", "", fo).set(e => this.culture = ve.parse(fo, e.value, !1)).setXml(e => this.culture = ve.parse(fo, e.textContent, !1)), new i("LocationType", "", bo), new r("LocationColor", "", N.limeGreen), new i("LocationColorType", "", yo), new i("ValueViewMode", "", Co), new i("Icon", "", kt), new r("IconColor", "", N.limeGreen), new h("CrossFiltering", "", !0), new n("CornerRadius").get(() => this.cornerRadius.toString()).set(e => this.cornerRadius = m.tryParse(e.value.toString())).setXml(e => this.cornerRadius = m.tryParse(e.textContent)), new n("Shadow").get(() => a.Serialize.jShadow(this.shadow)).set(e => this.shadow = a.Deserialize.simpleSahdow(e.value)).setXml(e => this.shadow = Ye.loadFromXml(e.textContent)), new ne("CustomIcon").check(() => null != this.customIcon).get(() => qa.toBase64String(this.customIcon)).set(e => this.customIcon = qa.fromBase64String(e.value.toString())).setXml(e => this.customIcon = qa.fromBase64String(e.textContent)), new s("DashboardInteraction").check(() => null != this.dashboardInteraction.as(po)).set(e => {
+                return [...super.meta(), new s("TransformActions").get(e => a.Serialize.objectArray(this.transformActions, e)).set(e => this.transformActions.addRange(e.value.properties().select(e => nn.loadFromJson(e.value)))).setXml(e => this.transformActions.addRange(e.childNodes.select(e => nn.loadFromXml(e)))), new s("TransformFilters").get(e => a.Serialize.objectArray(this.transformFilters, e)).set(e => this.transformFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.transformFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new s("TransformSorts").get(e => a.Serialize.objectArray(this.transformSorts, e)).set(e => this.transformSorts.addRange(e.value.properties().select(e => sn.loadFromJson(e.value)))).setXml(e => this.transformSorts.addRange(e.childNodes.select(e => sn.loadFromXml(e)))), new s("DataFilters").get(e => a.Serialize.objectArray(this.dataFilters, e)).set(e => this.dataFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.dataFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new s("Title").check(() => null != this.title).set(e => this.title = F.e.StiTitle.createFromJsonObject(e.value)).setXml(e => this.title = F.e.StiTitle.createFromXml(e)), new s("Layout").check(() => null != this.layout).set(e => this.layout = $s.createFromJsonObject(e.value)).setXml(e => this.layout = $s.createFromXml(e)), new s("Latitude").check(() => null != this.latitude).set(e => this.latitude = g.loadFromJson(e.value).as(F.O.StiLatitudeMapMeter)).setXml(e => this.latitude = g.loadFromXml(e).as(F.O.StiLatitudeMapMeter)), new s("Longitude").check(() => null != this.longitude).set(e => this.longitude = g.loadFromJson(e.value).as(F.O.StiLongitudeMapMeter)).setXml(e => this.longitude = g.loadFromXml(e).as(F.O.StiLongitudeMapMeter)), new s("Location").check(() => null != this.location).set(e => this.location = g.loadFromJson(e.value).as(F.O.StiLocationMapMeter)).setXml(e => this.location = g.loadFromXml(e).as(F.O.StiLocationMapMeter)), new s("LocationColorMeter").check(() => null != this.locationColorMeter).set(e => this.locationColorMeter = g.loadFromJson(e.value).as(F.O.StiLocationColorMapMeter)).setXml(e => this.locationColorMeter = g.loadFromXml(e).as(F.O.StiLocationColorMapMeter)), new s("LocationArgument").check(() => null != this.locationArgument).set(e => this.locationArgument = g.loadFromJson(e.value).as(F.O.StiLocationArgumentMapMeter)).setXml(e => this.locationArgument = g.loadFromXml(e).as(F.O.StiLocationArgumentMapMeter)), new s("LocationValue").check(() => null != this.locationValue).set(e => this.locationValue = g.loadFromJson(e.value).as(F.O.StiLocationValueMapMeter)).setXml(e => this.locationValue = g.loadFromXml(e).as(F.O.StiLocationValueMapMeter)), new n("Group"), new i("Culture", "", fo).set(e => this.culture = ve.parse(fo, e.value, !1)).setXml(e => this.culture = ve.parse(fo, e.textContent, !1)), new i("LocationType", "", bo), new r("LocationColor", "", N.limeGreen), new i("LocationColorType", "", yo), new i("ValueViewMode", "", Co), new i("Icon", "", kt), new r("IconColor", "", N.limeGreen), new h("CrossFiltering", "", !0), new n("CornerRadius").get(() => this.cornerRadius.toString()).set(e => this.cornerRadius = m.tryParse(e.value.toString())).setXml(e => this.cornerRadius = m.tryParse(e.textContent)), new n("Shadow").get(() => a.Serialize.jShadow(this.shadow)).set(e => this.shadow = a.Deserialize.simpleSahdow(e.value)).setXml(e => this.shadow = Ye.loadFromXml(e.textContent)), new ne("CustomIcon").check(() => null != this.customIcon).get(() => qa.toBase64String(this.customIcon)).set(e => this.customIcon = qa.fromBase64String(e.value.toString())).setXml(e => this.customIcon = qa.fromBase64String(e.textContent)), new s("DashboardInteraction").check(() => null != this.dashboardInteraction.as(po)).set(e => {
                     var t;
                     let r = null == (t = qr.loadInteractionFromJsonObject(e.value)) ? void 0 : t.as(po);
                     null != r && (this.dashboardInteraction = r)
                 }).setXml(e => {
                     var t;
                     let r = null == (t = qr.loadInteractionFromXml(e)) ? void 0 : t.as(po);
                     null != r && (this.dashboardInteraction = r)
@@ -7357,15 +7363,15 @@
             }
             getMeters() {
                 let e = new P;
                 return this.isDefined && (null != this.latitude && e.add(this.latitude), null != this.longitude && e.add(this.longitude), null != this.location && e.add(this.location), null != this.locationColorMeter && e.add(this.locationColorMeter), null != this.locationValue && e.add(this.locationValue), null != this.locationArgument) && e.add(this.locationArgument), e
             }
             retrieveUsedDataNames() {
                 let e = new P;
-                return e.addRange(en.getMany(this.latitude)), e.addRange(en.getMany(this.longitude)), e.addRange(en.getMany(this.location)), e.addRange(en.getMany(this.locationColorMeter)), e.addRange(en.getMany(this.locationValue)), e.addRange(en.getMany(this.locationArgument)), e.distinct().toList()
+                return e.addRange(tn.getMany(this.latitude)), e.addRange(tn.getMany(this.longitude)), e.addRange(tn.getMany(this.location)), e.addRange(tn.getMany(this.locationColorMeter)), e.addRange(tn.getMany(this.locationValue)), e.addRange(tn.getMany(this.locationArgument)), e.distinct().toList()
             }
             get isDefined() {
                 return null != this.latitude || null != this.longitude || null != Location || null != this.locationValue || null != this.locationColorMeter || null != this.locationArgument
             }
             createNextMeter(e) {
                 this.location = d.OnlineMap.getLocation2(e)
             }
@@ -7489,15 +7495,15 @@
             get onePointZoom() {
                 return this._onePointZoom
             }
             set onePointZoom(e) {
                 this._onePointZoom = Math.max(Math.min(e, 20), 1)
             }
             constructor(e = j.empty) {
-                super(e), this.group = "", this.title = new F.e.StiTitle, this.layout = new _s, this.transformActions = new P, this.transformFilters = new P, this.transformSorts = new P, this.dataTransformation = {}, this.dataFilters = new P, this.shadow = new Ye, this.cornerRadius = new m(0), this.helpUrl = "user-manual/dashboards_maps_online_map.htm", this._onePointZoom = 1, this.userBingKey = "", this.locationType = bo.Auto, this.culture = fo.en_US, this.locationColorType = yo.Single, this.valueViewMode = Co.Bubble, this.locationColor = N.limeGreen, this.icon = kt.MapMarker, this.iconColor = N.maroon, this.crossFiltering = !0, this.title.text = this.localizedName, this.dashboardInteraction = new po
+                super(e), this.group = "", this.title = new F.e.StiTitle, this.layout = new $s, this.transformActions = new P, this.transformFilters = new P, this.transformSorts = new P, this.dataTransformation = {}, this.dataFilters = new P, this.shadow = new Ye, this.cornerRadius = new m(0), this.helpUrl = "user-manual/dashboards_maps_online_map.htm", this._onePointZoom = 1, this.userBingKey = "", this.locationType = bo.Auto, this.culture = fo.en_US, this.locationColorType = yo.Single, this.valueViewMode = Co.Bubble, this.locationColor = N.limeGreen, this.icon = kt.MapMarker, this.iconColor = N.maroon, this.crossFiltering = !0, this.title.text = this.localizedName, this.dashboardInteraction = new po
             }
         }
         F.O.StiOnlineMapElement = Mm
     }
     F.N.StiPivotTableColumnVisibilityHelper = class {
         static getVisible(e, t) {
             if (e.visibility == Hr.True) return !0;
@@ -7531,15 +7537,15 @@
                 this.hash.containsKey(e.key) && this.hash.remove(e.key)
             }
         }
         vo.hash = new xo, F.h.StiPivotTableElementSelection = vo
     } {
         class To extends F.g.StiDashboardInteraction {
             implements() {
-                return To.ImplementsIStiPivotTableDashboardInteraction || (To.ImplementsIStiPivotTableDashboardInteraction = super.implements().concat([l, Gs])), To.ImplementsIStiPivotTableDashboardInteraction
+                return To.ImplementsIStiPivotTableDashboardInteraction || (To.ImplementsIStiPivotTableDashboardInteraction = super.implements().concat([l, Xs])), To.ImplementsIStiPivotTableDashboardInteraction
             }
             meta() {
                 return [...super.meta(), new h("ShowFullScreenButton", "", !0), new h("ShowSaveButton", "", !0), new h("ShowViewDataButton", "", !0), new n("FileName"), new n("HeaderText"), new n("FooterText")]
             }
             get isDefaultLayout() {
                 return this.showFullScreenButton && this.showSaveButton && this.showViewDataButton && null == this.fileName && null == this.headerText && null == this.footerText
             }
@@ -7557,35 +7563,35 @@
         Fo = L.Report.Dashboard.ImplementsIStiPivotTableElement,
         vo = F.h.StiPivotTableElementSelection,
         Ao = L.Report.Dashboard.IStiPivotTableElement;
     {
         dt.add("StiPivotTableElement", "Stimulsoft.Dashboard.Export.Tools.StiPivotTableElementExportTool");
         class Yh extends F.e.StiElement {
             implements() {
-                return Yh.ImplementsStiPivotTableElement || (Yh.ImplementsStiPivotTableElement = super.implements().concat([Ao, Ke, Ze, Oe, qs, Qr, Ne, ...Fo, ...Qe, ...Ue, ...$s, ...Qs, l])), Yh.ImplementsStiPivotTableElement
+                return Yh.ImplementsStiPivotTableElement || (Yh.ImplementsStiPivotTableElement = super.implements().concat([Ao, Ke, Ze, Oe, _s, Qr, Ne, ...Fo, ...Qe, ...Ue, ...en, ...qs, l])), Yh.ImplementsStiPivotTableElement
             }
             clone(e) {
                 var t, r;
                 let i = super.clone(e);
                 return i.columns = this.columns.select(e => e.clone()).toList(), i.rows = this.rows.select(e => e.clone()).toList(), i.summaries = this.summaries.select(e => e.clone()).toList(), i.transformActions = this.transformActions.select(e => e.clone()).toList(), i.transformFilters = this.transformFilters.select(e => e.clone()).toList(), i.transformSorts = this.transformSorts.select(e => e.clone()).toList(), i.dataFilters = this.dataFilters.select(e => e.clone()).toList(), i.title = null != this.title ? this.title.clone() : null, i.layout = null != this.layout ? this.layout.clone() : null, i.dashboardInteraction = this.dashboardInteraction.clone(), i.pivotTableConditions = this.pivotTableConditions.select(e => e.clone()).toList(), i.totalLabel = this.totalLabel, i.shadow = null == (t = this.shadow) ? void 0 : t.clone(), i.cornerRadius = null == (r = this.cornerRadius) ? void 0 : r.clone(), i
             }
             meta() {
-                return [...super.meta(), new s("TransformActions").get(e => a.Serialize.objectArray(this.transformActions, e)).set(e => this.transformActions.addRange(e.value.properties().select(e => sn.loadFromJson(e.value)))).setXml(e => this.transformActions.addRange(e.childNodes.select(e => sn.loadFromXml(e)))), new s("TransformFilters").get(e => a.Serialize.objectArray(this.transformFilters, e)).set(e => this.transformFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.transformFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new s("TransformSorts").get(e => a.Serialize.objectArray(this.transformSorts, e)).set(e => this.transformSorts.addRange(e.value.properties().select(e => rn.loadFromJson(e.value)))).setXml(e => this.transformSorts.addRange(e.childNodes.select(e => rn.loadFromXml(e)))), new s("DataFilters").get(e => a.Serialize.objectArray(this.dataFilters, e)).set(e => this.dataFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.dataFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new s("Columns").get(e => a.Serialize.objectArray(this.columns, e)).set(e => this.columns.addRange(e.value.properties().select(e => g.loadFromJson(e.value).as(cs)).where(e => null != e))).setXml(e => this.columns.addRange(e.childNodes.select(e => g.loadFromXml(e)))), new s("Rows").get(e => a.Serialize.objectArray(this.rows, e)).set(e => this.rows.addRange(e.value.properties().select(e => g.loadFromJson(e.value).as(F.N.StiPivotRow)).where(e => null != e))).setXml(e => this.rows.addRange(e.childNodes.select(e => g.loadFromXml(e)))), new s("Summaries").get(e => a.Serialize.objectArray(this.summaries, e)).set(e => this.summaries.addRange(e.value.properties().select(e => g.loadFromJson(e.value).as(gs)).where(e => null != e))).setXml(e => this.summaries.addRange(e.childNodes.select(e => g.loadFromXml(e)))), new h("CrossFiltering", "", !0), new s("Title").check(() => null != this.title).set(e => this.title = F.e.StiTitle.createFromJsonObject(e.value)).setXml(e => this.title = F.e.StiTitle.createFromXml(e)), new s("Layout").check(() => null != this.layout).set(e => this.layout = _s.createFromJsonObject(e.value)).setXml(e => this.layout = _s.createFromXml(e)), new i("Style", "", o, o.Auto), new n("Group"), new n("CustomStyleName"), new n("TotalLabel"), new s("PivotTableConditions").get(e => a.Serialize.objectArray(this.pivotTableConditions, e)).set(e => this.pivotTableConditions.addRange(e.value.properties().select(e => F.N.StiPivotTableElementCondition.loadFromJson(e.value).as(F.N.StiPivotTableElementCondition)).where(e => null != e))).setXml(e => this.pivotTableConditions.addRange(e.childNodes.select(e => F.N.StiPivotTableElementCondition.loadFromXml(e)))), new i("SummaryDirection", "", Mo, Mo.UpToDown), new n("CornerRadius").get(() => this.cornerRadius.toString()).set(e => this.cornerRadius = m.tryParse(e.value.toString())).setXml(e => this.cornerRadius = m.tryParse(e.textContent)), new n("Shadow").get(() => a.Serialize.jShadow(this.shadow)).set(e => this.shadow = a.Deserialize.simpleSahdow(e.value)).setXml(e => this.shadow = Ye.loadFromXml(e.textContent)), new s("DashboardInteraction").check(() => null != this.dashboardInteraction.as(To)).set(e => {
+                return [...super.meta(), new s("TransformActions").get(e => a.Serialize.objectArray(this.transformActions, e)).set(e => this.transformActions.addRange(e.value.properties().select(e => nn.loadFromJson(e.value)))).setXml(e => this.transformActions.addRange(e.childNodes.select(e => nn.loadFromXml(e)))), new s("TransformFilters").get(e => a.Serialize.objectArray(this.transformFilters, e)).set(e => this.transformFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.transformFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new s("TransformSorts").get(e => a.Serialize.objectArray(this.transformSorts, e)).set(e => this.transformSorts.addRange(e.value.properties().select(e => sn.loadFromJson(e.value)))).setXml(e => this.transformSorts.addRange(e.childNodes.select(e => sn.loadFromXml(e)))), new s("DataFilters").get(e => a.Serialize.objectArray(this.dataFilters, e)).set(e => this.dataFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.dataFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new s("Columns").get(e => a.Serialize.objectArray(this.columns, e)).set(e => this.columns.addRange(e.value.properties().select(e => g.loadFromJson(e.value).as(ds)).where(e => null != e))).setXml(e => this.columns.addRange(e.childNodes.select(e => g.loadFromXml(e)))), new s("Rows").get(e => a.Serialize.objectArray(this.rows, e)).set(e => this.rows.addRange(e.value.properties().select(e => g.loadFromJson(e.value).as(F.N.StiPivotRow)).where(e => null != e))).setXml(e => this.rows.addRange(e.childNodes.select(e => g.loadFromXml(e)))), new s("Summaries").get(e => a.Serialize.objectArray(this.summaries, e)).set(e => this.summaries.addRange(e.value.properties().select(e => g.loadFromJson(e.value).as(ps)).where(e => null != e))).setXml(e => this.summaries.addRange(e.childNodes.select(e => g.loadFromXml(e)))), new h("CrossFiltering", "", !0), new s("Title").check(() => null != this.title).set(e => this.title = F.e.StiTitle.createFromJsonObject(e.value)).setXml(e => this.title = F.e.StiTitle.createFromXml(e)), new s("Layout").check(() => null != this.layout).set(e => this.layout = $s.createFromJsonObject(e.value)).setXml(e => this.layout = $s.createFromXml(e)), new i("Style", "", o, o.Auto), new n("Group"), new n("CustomStyleName"), new n("TotalLabel"), new s("PivotTableConditions").get(e => a.Serialize.objectArray(this.pivotTableConditions, e)).set(e => this.pivotTableConditions.addRange(e.value.properties().select(e => F.N.StiPivotTableElementCondition.loadFromJson(e.value).as(F.N.StiPivotTableElementCondition)).where(e => null != e))).setXml(e => this.pivotTableConditions.addRange(e.childNodes.select(e => F.N.StiPivotTableElementCondition.loadFromXml(e)))), new i("SummaryDirection", "", Mo, Mo.UpToDown), new n("CornerRadius").get(() => this.cornerRadius.toString()).set(e => this.cornerRadius = m.tryParse(e.value.toString())).setXml(e => this.cornerRadius = m.tryParse(e.textContent)), new n("Shadow").get(() => a.Serialize.jShadow(this.shadow)).set(e => this.shadow = a.Deserialize.simpleSahdow(e.value)).setXml(e => this.shadow = Ye.loadFromXml(e.textContent)), new s("DashboardInteraction").check(() => null != this.dashboardInteraction.as(To)).set(e => {
                     var t;
                     let r = null == (t = qr.loadInteractionFromJsonObject(e.value)) ? void 0 : t.as(To);
                     null != r && (this.dashboardInteraction = r)
                 }).setXml(e => {
                     var t;
                     let r = null == (t = qr.loadInteractionFromXml(e)) ? void 0 : t.as(To);
                     null != r && (this.dashboardInteraction = r)
                 })]
             }
             retrieveUsedDataNames() {
-                let e = en.getMany2(this.columns);
-                return e.addRange(en.getMany2(this.rows)), e.addRange(en.getMany2(this.summaries)), e
+                let e = tn.getMany2(this.columns);
+                return e.addRange(tn.getMany2(this.rows)), e.addRange(tn.getMany2(this.summaries)), e
             }
             fetchAllMeters() {
                 let e = this.columns.cast();
                 return e.addRange(this.rows.cast()), e.addRange(this.summaries.cast()), e
             }
             getMeters() {
                 let e = this.columns.cast();
@@ -7600,27 +7606,27 @@
             set style(e) {
                 (this._style = e) != o.Custom && (this.customStyleName = "")
             }
             createNextMeter(e) {
                 0 == this.columns.length ? this.columns.add(d.Pivot.getColumn2(e)) : 0 == this.rows.length ? this.rows.add(d.Pivot.getRow2(e)) : 0 == this.summaries.length ? this.summaries.add(d.Pivot.getSummary2(e)) : this.columns.add(d.Pivot.getColumn2(e))
             }
             createNewColumn() {
-                this.columns.add(new cs)
+                this.columns.add(new ds)
             }
             getColumn2(e) {
                 return null != e ? d.Pivot.getColumn2(e) : null
             }
             getColumn(e) {
                 return null != e ? d.Pivot.getColumn(e.as(F.e.StiMeter)) : null
             }
             getColumnByIndex(e) {
                 return e < this.columns.length ? this.columns[e] : null
             }
             insertColumn(e, t) {
-                let r = t.as(cs);
+                let r = t.as(ds);
                 null != r && (0 <= e && e < this.columns.length ? this.columns.insert(e, r) : this.columns.add(r))
             }
             removeColumn(e) {
                 e < this.columns.length && this.columns.removeAt(e)
             }
             removeAllColumns() {
                 this.columns.clear()
@@ -7644,28 +7650,28 @@
             removeRow(e) {
                 e < this.rows.length && this.rows.removeAt(e)
             }
             removeAllRows() {
                 this.rows.clear()
             }
             createNewSummary() {
-                let e = new gs;
+                let e = new ps;
                 e.expression = "Sum()", this.summaries.add(e)
             }
             getSummary2(e) {
                 return null != e ? d.Pivot.getSummary2(e) : null
             }
             getSummary(e) {
                 return null != e ? d.Pivot.getSummary(e.as(F.e.StiMeter)) : null
             }
             getSummaryByIndex(e) {
                 return e < this.summaries.length ? this.summaries[e] : null
             }
             insertSummary(e, t) {
-                let r = t.as(gs);
+                let r = t.as(ps);
                 null != r && (0 <= e && e < this.summaries.length ? this.summaries.insert(e, r) : this.summaries.add(r))
             }
             removeSummary(e) {
                 e < this.summaries.length && this.summaries.removeAt(e)
             }
             removeAllSummaries() {
                 this.summaries.clear()
@@ -7687,22 +7693,22 @@
             convertFrom(e) {
                 let t = e.fetchAllMeters();
                 if (this.columns.clear(), this.rows.clear(), this.summaries.clear(), null == t) return;
                 let r = 0;
                 t.cast().forEach(t => {
                     if (t.is2(ze))
                         if (0 == (1 & r)) {
-                            let e = new cs;
+                            let e = new ds;
                             e.loadFromJsonObject(t.saveToJsonObject(je.Report)), this.columns.add(e)
                         } else {
                             let e = new F.N.StiPivotRow;
                             e.loadFromJsonObject(t.saveToJsonObject(je.Report)), this.rows.add(e)
                         }
                     else if (t.is2(vt)) {
-                        let e = new gs;
+                        let e = new ps;
                         e.loadFromJsonObject(t.saveToJsonObject(je.Report)), this.summaries.add(e)
                     }
                 }, this), null == this.dashboardInteraction && (this.dashboardInteraction = new To)
             }
             setString(r, i) {
                 switch (r) {
                     case "Title.Text":
@@ -7753,15 +7759,15 @@
             get localizedName() {
                 return b.get("Components", "StiPivotTable")
             }
             getFormatObjects() {
                 return vo.getSelectedObjects(this)
             }
             constructor(e = j.empty) {
-                super(e), this.maxIconSize = 50, this.shadow = new Ye, this.cornerRadius = new m(0), this.group = "", this.title = new F.e.StiTitle, this.layout = new _s, this.transformActions = new P, this.transformFilters = new P, this.transformSorts = new P, this.dataTransformation = {}, this.dataFilters = new P, this.crossFiltering = !0, this._style = o.Auto, this.customStyleName = "", this.summaryDirection = Mo.UpToDown, this.helpUrl = "user-manual/dashboards_pivot_table.htm", this.columns = new P, this.rows = new P, this.summaries = new P, this.totalLabel = "", this.pivotTableConditions = new P, this.title.text = this.localizedName, this.dashboardInteraction = new To
+                super(e), this.maxIconSize = 50, this.shadow = new Ye, this.cornerRadius = new m(0), this.group = "", this.title = new F.e.StiTitle, this.layout = new $s, this.transformActions = new P, this.transformFilters = new P, this.transformSorts = new P, this.dataTransformation = {}, this.dataFilters = new P, this.crossFiltering = !0, this._style = o.Auto, this.customStyleName = "", this.summaryDirection = Mo.UpToDown, this.helpUrl = "user-manual/dashboards_pivot_table.htm", this.columns = new P, this.rows = new P, this.summaries = new P, this.totalLabel = "", this.pivotTableConditions = new P, this.title.text = this.localizedName, this.dashboardInteraction = new To
             }
         }
         F.N.StiPivotTableElement = Yh
     }
     let Io = L.Report.Components.StiConditionPermissions,
         Do = L.Base.StiScale,
         Ro = L.Report.Dashboard.IStiPivotTableElementCondition;
@@ -7850,15 +7856,15 @@
         }
         F.N.StiPivotTableElementCondition = Yg
     }
     F.ac.StiPivotColumnConverter = class extends ml {}, F.ac.StiPivotRowConverter = class extends ml {}, F.ac.StiPivotSummaryConverter = class extends ml {};
     {
         class Eo extends F.g.StiDashboardInteraction {
             implements() {
-                return Eo.ImplementsIStiProgressDashboardInteraction || (Eo.ImplementsIStiProgressDashboardInteraction = super.implements().concat([An, l, Gs])), Eo.ImplementsIStiProgressDashboardInteraction
+                return Eo.ImplementsIStiProgressDashboardInteraction || (Eo.ImplementsIStiProgressDashboardInteraction = super.implements().concat([In, l, Xs])), Eo.ImplementsIStiProgressDashboardInteraction
             }
             meta() {
                 return [...super.meta(), new h("AllowUserSorting", "", !0), new h("ShowFullScreenButton", "", !0), new h("ShowSaveButton", "", !0), new h("ShowViewDataButton", "", !0), new n("FileName"), new n("HeaderText"), new n("FooterText")]
             }
             get isDefaultLayout() {
                 return this.showFullScreenButton && this.showSaveButton && this.showViewDataButton && null == this.fileName && null == this.headerText && null == this.footerText
             }
@@ -7874,41 +7880,41 @@
     let Eo = F.g.StiProgressDashboardInteraction,
         Oo = L.Report.Dashboard.ImplementsIStiProgressElement,
         Vo = L.Report.Dashboard.StiProgressElementMode,
         ko = L.Report.Dashboard.IStiProgressElement;
     {
         class xm extends F.e.StiElement {
             implements() {
-                return xm.ImplementsStiProgressElement || (xm.ImplementsStiProgressElement = super.implements().concat([yr, Ke, Ze, ko, Oe, ar, fr, qs, Qr, Ne, Us, Wa, Xs, ...$r, ...Qe, ...Ue, ...Oo, ...$s, ...rr, ...Sr, ...Qs, ...Wn, ...Ya, l])), xm.ImplementsStiProgressElement
+                return xm.ImplementsStiProgressElement || (xm.ImplementsStiProgressElement = super.implements().concat([yr, Ke, Ze, ko, Oe, ar, fr, _s, Qr, Ne, Zs, Wa, Ws, ...$r, ...Qe, ...Ue, ...Oo, ...en, ...rr, ...Sr, ...qs, ...Wn, ...Ya, l])), xm.ImplementsStiProgressElement
             }
             clone(e) {
                 var t, r;
                 let i = super.clone(e);
                 return i.value = null != this.value ? this.value.clone() : null, i.target = null != this.target ? this.target.clone() : null, i.series = null != this.series ? this.series.clone() : null, i.userSorts = this.userSorts.select(e => e.clone()).toList(), i.transformActions = this.transformActions.select(e => e.clone()), i.transformFilters = this.transformFilters.select(e => e.clone()), i.transformSorts = this.transformSorts.select(e => e.clone()), i.dataFilters = this.dataFilters.select(e => e.clone()), i.topN = this.topN.clone(), i.textFormat = this.textFormat.clone(), i.title = null != this.title ? this.title.clone() : null, i.layout = null != this.layout ? this.layout.clone() : null, i.seriesColors = null != this.seriesColors ? this.seriesColors[L.System.StiObject.stimulsoft]().clone() : null, i.progressConditions = this.progressConditions.select(e => e.clone()).toList(), i.dashboardInteraction = this.dashboardInteraction.clone(), i.shadow = null == (t = this.shadow) ? void 0 : t.clone(), i.cornerRadius = null == (r = this.cornerRadius) ? void 0 : r.clone(), i
             }
             meta() {
-                return [...super.meta(), new s("UserSorts").get(e => a.Serialize.objectArray(this.userSorts, e)).set(e => this.userSorts.addRange(e.value.properties().select(e => rn.loadFromJson(e.value)))).setXml(e => this.userSorts.addRange(e.childNodes.select(e => rn.loadFromXml(e)))), new s("TransformActions").get(e => a.Serialize.objectArray(this.transformActions, e)).set(e => this.transformActions.addRange(e.value.properties().select(e => sn.loadFromJson(e.value)))).setXml(e => this.transformActions.addRange(e.childNodes.select(e => sn.loadFromXml(e)))), new s("TransformFilters").get(e => a.Serialize.objectArray(this.transformFilters, e)).set(e => this.transformFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.transformFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new s("TransformSorts").get(e => a.Serialize.objectArray(this.transformSorts, e)).set(e => this.transformSorts.addRange(e.value.properties().select(e => rn.loadFromJson(e.value)))).setXml(e => this.transformSorts.addRange(e.childNodes.select(e => rn.loadFromXml(e)))), new s("DataFilters").get(e => a.Serialize.objectArray(this.dataFilters, e)).set(e => this.dataFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.dataFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new s("TopN").check(() => null != this.topN).set(e => this.topN = Fi.createFromJsonObject(e.value)).setXml(e => this.topN = Fi.createFromXml(e)), new s("TextFormat").check(() => null != this.textFormat).set(e => this.textFormat = br.createFromJsonObject(e.value)).setXml(e => this.textFormat = br.loadFormatFromXml(e, this.report)), new s("Value").check(() => null != this.value).set(e => {
+                return [...super.meta(), new s("UserSorts").get(e => a.Serialize.objectArray(this.userSorts, e)).set(e => this.userSorts.addRange(e.value.properties().select(e => sn.loadFromJson(e.value)))).setXml(e => this.userSorts.addRange(e.childNodes.select(e => sn.loadFromXml(e)))), new s("TransformActions").get(e => a.Serialize.objectArray(this.transformActions, e)).set(e => this.transformActions.addRange(e.value.properties().select(e => nn.loadFromJson(e.value)))).setXml(e => this.transformActions.addRange(e.childNodes.select(e => nn.loadFromXml(e)))), new s("TransformFilters").get(e => a.Serialize.objectArray(this.transformFilters, e)).set(e => this.transformFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.transformFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new s("TransformSorts").get(e => a.Serialize.objectArray(this.transformSorts, e)).set(e => this.transformSorts.addRange(e.value.properties().select(e => sn.loadFromJson(e.value)))).setXml(e => this.transformSorts.addRange(e.childNodes.select(e => sn.loadFromXml(e)))), new s("DataFilters").get(e => a.Serialize.objectArray(this.dataFilters, e)).set(e => this.dataFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.dataFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new s("TopN").check(() => null != this.topN).set(e => this.topN = vi.createFromJsonObject(e.value)).setXml(e => this.topN = vi.createFromXml(e)), new s("TextFormat").check(() => null != this.textFormat).set(e => this.textFormat = br.createFromJsonObject(e.value)).setXml(e => this.textFormat = br.loadFormatFromXml(e, this.report)), new s("Value").check(() => null != this.value).set(e => {
                     let t = g.loadFromJson(e.value).as(F.M.StiValueProgressMeter);
                     null != t && (this.value = t)
                 }).setXml(e => {
                     let t = g.loadFromXml(e).as(F.M.StiValueProgressMeter);
                     null != t && (this.value = t)
                 }), new s("Target").check(() => null != this.target).set(e => {
-                    let t = g.loadFromJson(e.value).as(hs);
+                    let t = g.loadFromJson(e.value).as(ms);
                     null != t && (this.target = t)
                 }).setXml(e => {
-                    let t = g.loadFromXml(e).as(hs);
+                    let t = g.loadFromXml(e).as(ms);
                     null != t && (this.target = t)
                 }), new s("Series").check(() => null != this.series).set(e => {
                     let t = g.loadFromJson(e.value).as(F.M.StiSeriesProgressMeter);
                     null != t && (this.series = t)
                 }).setXml(e => {
                     let t = g.loadFromXml(e).as(F.M.StiSeriesProgressMeter);
                     null != t && (this.series = t)
-                }), new s("Title").check(() => null != this.title).set(e => this.title = F.e.StiTitle.createFromJsonObject(e.value)).setXml(e => this.title = F.e.StiTitle.createFromXml(e)), new s("Layout").check(() => null != this.layout).set(e => this.layout = _s.createFromJsonObject(e.value)).setXml(e => this.layout = _s.createFromXml(e)), new r("ForeColor", "", N.transparent), new n("Font").get(() => a.Serialize.fontArial8(this.font)).set(e => this.font = a.Deserialize.font(e.value, this.font)).setXml(e => this.font = L.System.Convert.toFont(e.textContent)), new i("DataMode", "", Vn, Vn.UsingDataFields), new n("ManuallyEnteredData"), new s("SeriesColors").get(e => a.Serialize.colorArray(this.seriesColors)).set(e => this.seriesColors = a.Deserialize.colorArray(e)).setXml(e => this.seriesColors = Js.convertStringToColorArray(e.textContent)), new i("Mode", "", Vo, Vo.Circle), new i("Style", "", o, o.Auto), new n("CustomStyleName"), new n("Group"), new h("ColorEach", "", !0), new s("ProgressConditions").get(e => a.Serialize.objectArray(this.progressConditions, e)).set(e => this.progressConditions.addRange(e.value.properties().select(e => F.M.StiProgressElementCondition.createFromJson(e.value)))).setXml(e => this.progressConditions.addRange(e.childNodes.select(e => F.M.StiProgressElementCondition.createFromXml(e)))), new h("CrossFiltering", "", !0), new n("CornerRadius").get(() => this.cornerRadius.toString()).set(e => this.cornerRadius = m.tryParse(e.value.toString())).setXml(e => this.cornerRadius = m.tryParse(e.textContent)), new n("Shadow").get(() => a.Serialize.jShadow(this.shadow)).set(e => this.shadow = a.Deserialize.simpleSahdow(e.value)).setXml(e => this.shadow = Ye.loadFromXml(e.textContent)), new s("DashboardInteraction").check(() => null != this.dashboardInteraction.as(Eo)).set(e => {
+                }), new s("Title").check(() => null != this.title).set(e => this.title = F.e.StiTitle.createFromJsonObject(e.value)).setXml(e => this.title = F.e.StiTitle.createFromXml(e)), new s("Layout").check(() => null != this.layout).set(e => this.layout = $s.createFromJsonObject(e.value)).setXml(e => this.layout = $s.createFromXml(e)), new r("ForeColor", "", N.transparent), new n("Font").get(() => a.Serialize.fontArial8(this.font)).set(e => this.font = a.Deserialize.font(e.value, this.font)).setXml(e => this.font = L.System.Convert.toFont(e.textContent)), new i("DataMode", "", kn, kn.UsingDataFields), new n("ManuallyEnteredData"), new s("SeriesColors").get(e => a.Serialize.colorArray(this.seriesColors)).set(e => this.seriesColors = a.Deserialize.colorArray(e)).setXml(e => this.seriesColors = Us.convertStringToColorArray(e.textContent)), new i("Mode", "", Vo, Vo.Circle), new i("Style", "", o, o.Auto), new n("CustomStyleName"), new n("Group"), new h("ColorEach", "", !0), new s("ProgressConditions").get(e => a.Serialize.objectArray(this.progressConditions, e)).set(e => this.progressConditions.addRange(e.value.properties().select(e => F.M.StiProgressElementCondition.createFromJson(e.value)))).setXml(e => this.progressConditions.addRange(e.childNodes.select(e => F.M.StiProgressElementCondition.createFromXml(e)))), new h("CrossFiltering", "", !0), new n("CornerRadius").get(() => this.cornerRadius.toString()).set(e => this.cornerRadius = m.tryParse(e.value.toString())).setXml(e => this.cornerRadius = m.tryParse(e.textContent)), new n("Shadow").get(() => a.Serialize.jShadow(this.shadow)).set(e => this.shadow = a.Deserialize.simpleSahdow(e.value)).setXml(e => this.shadow = Ye.loadFromXml(e.textContent)), new s("DashboardInteraction").check(() => null != this.dashboardInteraction.as(Eo)).set(e => {
                     var t;
                     let r = null == (t = qr.loadInteractionFromJsonObject(e.value)) ? void 0 : t.as(Eo);
                     null != r && (this.dashboardInteraction = r)
                 }).setXml(e => {
                     var t;
                     let r = null == (t = qr.loadInteractionFromXml(e)) ? void 0 : t.as(Eo);
                     null != r && (this.dashboardInteraction = r)
@@ -7944,15 +7950,15 @@
             getTarget() {
                 return this.target
             }
             getTarget2(e) {
                 return null != e ? d.Progress.getTarget(e.as(F.e.StiMeter)) : null
             }
             createNewTarget() {
-                this.target = new hs, this.target.expression = "Sum()"
+                this.target = new ms, this.target.expression = "Sum()"
             }
             addSeries2(e) {
                 this.series = null != e ? d.Progress.getSeries2(e) : null
             }
             addSeries(e) {
                 this.series = d.Progress.getSeries(e.as(F.e.StiMeter))
             }
@@ -7965,38 +7971,38 @@
             getSeries2(e) {
                 return null != e ? d.Progress.getSeries(e.as(F.e.StiMeter)) : null
             }
             createNewSeries() {
                 this.series = new F.M.StiSeriesProgressMeter
             }
             getManuallyEnteredDataTable() {
-                if (this.dataMode != Vn.ManuallyEnteringData) return null;
+                if (this.dataMode != kn.ManuallyEnteringData) return null;
                 return F.e.StiManuallyEnteredDataParser.getProgressDataTable(this.manuallyEnteredData, this)
             }
             convertFrom(e) {
                 let t = e.fetchAllMeters();
                 if (null == t) return;
                 let r = t.firstOrDefault(e => e.is(Er)),
-                    i = (null != (r = null == r ? t.firstOrDefault(e => e.is(vt)) : r) && (this.value = null == this.value ? new F.M.StiValueProgressMeter : this.value, this.value.loadFromJsonObject(r.saveToJsonObject(je.Report))), t.firstOrDefault(e => e.is(Di))),
-                    s = (null != i && (this.target = null == this.target ? new hs : this.target, this.target.loadFromJsonObject(i.saveToJsonObject(je.Report))), t.firstOrDefault(e => e.is(Ii)));
+                    i = (null != (r = null == r ? t.firstOrDefault(e => e.is(vt)) : r) && (this.value = null == this.value ? new F.M.StiValueProgressMeter : this.value, this.value.loadFromJsonObject(r.saveToJsonObject(je.Report))), t.firstOrDefault(e => e.is(Ri))),
+                    s = (null != i && (this.target = null == this.target ? new ms : this.target, this.target.loadFromJsonObject(i.saveToJsonObject(je.Report))), t.firstOrDefault(e => e.is(Di)));
                 null != (s = null == s ? t.firstOrDefault(e => e.is(ze)) : s) && (this.series = null == this.series ? new F.M.StiSeriesProgressMeter : this.series, this.series.loadFromJsonObject(s.saveToJsonObject(je.Report))), null == this.dashboardInteraction && (this.dashboardInteraction = new Eo)
             }
             fetchAllMeters() {
                 let e = new P;
-                return this.dataMode == Vn.UsingDataFields && (null != this.value && e.add(this.value), null != this.target && e.add(this.target), null != this.series) && e.add(this.series), e
+                return this.dataMode == kn.UsingDataFields && (null != this.value && e.add(this.value), null != this.target && e.add(this.target), null != this.series) && e.add(this.series), e
             }
             getMeters() {
                 let e = new P;
-                return this.dataMode == Vn.UsingDataFields && (null != this.value && e.add(this.value), null != this.target && e.add(this.target), null != this.series) && e.add(this.series), e
+                return this.dataMode == kn.UsingDataFields && (null != this.value && e.add(this.value), null != this.target && e.add(this.target), null != this.series) && e.add(this.series), e
             }
             retrieveUsedDataNames() {
-                return this.dataMode == Vn.UsingDataFields ? en.getMany(this.value, this.target, this.series) : null
+                return this.dataMode == kn.UsingDataFields ? tn.getMany(this.value, this.target, this.series) : null
             }
             get isDefined() {
-                return null != this.value || null != this.target || null != this.series || this.dataMode == Vn.ManuallyEnteringData
+                return null != this.value || null != this.target || null != this.series || this.dataMode == kn.ManuallyEnteringData
             }
             get style() {
                 return this._style
             }
             set style(e) {
                 (this._style = e) != o.Custom && (this.customStyleName = "")
             }
@@ -8030,15 +8036,15 @@
                 let e = new P;
                 return null != this.progressConditions && e.addRange(this.progressConditions), e
             }
             clearProgressConditions() {
                 this.progressConditions.clear()
             }
             constructor(e = j.empty) {
-                super(e), this.group = "", this.dataMode = Vn.UsingDataFields, this.textFormat = new Jt, this.font = new H("Arial", 13), this.foreColor = N.transparent, this.title = new F.e.StiTitle, this.layout = new _s, this.shadow = new Ye, this.cornerRadius = new m(0), this.showBlanks = !1, this.transformActions = new P, this.transformFilters = new P, this.transformSorts = new P, this.topN = new Fi, this.dataTransformation = {}, this.crossFiltering = !0, this.dataFilters = new P, this.userSorts = new P, this._style = o.Auto, this.customStyleName = "", this.seriesColors = [], this.defaultClientRectangle = new j(0, 0, 160, 160), this.helpUrl = "user-manual/dashboards_progress.htm", this.colorEach = !0, this.mode = Vo.Circle, this.progressConditions = new P, this.isSampleForStyles = !1, this.title.text = this.localizedName, this.dashboardInteraction = new Eo
+                super(e), this.group = "", this.dataMode = kn.UsingDataFields, this.textFormat = new Jt, this.font = new H("Arial", 13), this.foreColor = N.transparent, this.title = new F.e.StiTitle, this.layout = new $s, this.shadow = new Ye, this.cornerRadius = new m(0), this.showBlanks = !1, this.transformActions = new P, this.transformFilters = new P, this.transformSorts = new P, this.topN = new vi, this.dataTransformation = {}, this.crossFiltering = !0, this.dataFilters = new P, this.userSorts = new P, this._style = o.Auto, this.customStyleName = "", this.seriesColors = [], this.defaultClientRectangle = new j(0, 0, 160, 160), this.helpUrl = "user-manual/dashboards_progress.htm", this.colorEach = !0, this.mode = Vo.Circle, this.progressConditions = new P, this.isSampleForStyles = !1, this.title.text = this.localizedName, this.dashboardInteraction = new Eo
             }
         }
         F.M.StiProgressElement = xm
     }
     let No = L.Report.Dashboard.IStiProgressElementCondition,
         Lo = L.Report.Dashboard.StiProgressFieldCondition,
         Bo = L.Report.Dashboard.StiProgressConditionPermissions;
@@ -8074,15 +8080,15 @@
                 this.condition = nl.EqualTo, this.field = Lo.Value, this.permissions = Bo.All, this.textColor = N.black, this.color = N.transparent, this.trackColor = N.transparent, this.font = new H("Arial", 8), null != e && (this.field = e), null != t && (this.condition = t), null != r && (this.value = r), null != i && (this.permissions = i), null != s && (this.font = s), null != n && (this.textColor = n), null != l && (this.color = l), null != a && (this.trackColor = a)
             }
         }
         F.M.StiProgressElementCondition = Kg
     } {
         class jo extends F.g.StiDashboardInteraction {
             implements() {
-                return jo.ImplementsIStiRegionMapDashboardInteraction || (jo.ImplementsIStiRegionMapDashboardInteraction = super.implements().concat([l, Gs])), jo.ImplementsIStiRegionMapDashboardInteraction
+                return jo.ImplementsIStiRegionMapDashboardInteraction || (jo.ImplementsIStiRegionMapDashboardInteraction = super.implements().concat([l, Xs])), jo.ImplementsIStiRegionMapDashboardInteraction
             }
             meta() {
                 return [...super.meta(), new h("ShowFullScreenButton", "", !0), new h("ShowSaveButton", "", !0), new h("ShowViewDataButton", "", !0), new n("FileName"), new n("HeaderText"), new n("FooterText")]
             }
             get isDefaultLayout() {
                 return this.showFullScreenButton && this.showSaveButton && this.showViewDataButton && null == this.fileName && null == this.headerText && null == this.footerText
             }
@@ -8103,35 +8109,35 @@
         Xo = L.Report.Maps.StiMapType,
         Wo = L.Report.Maps.StiMapSource,
         Jo = L.Report.Dashboard.IStiRegionMapElement;
     {
         dt.add("StiRegionMapElement", "Stimulsoft.Dashboard.Export.Tools.StiRegionMapElementExportTool");
         class Tm extends F.e.StiElement {
             implements() {
-                return Tm.ImplementsStiRegionMapElement || (Tm.ImplementsStiRegionMapElement = super.implements().concat([Jo, Ke, Ze, ye, Oe, qs, ar, Ne, ...Ho, ...Qe, ...Ue, ...Yn, ...$s, ...Qs, ...rr, l, Qr, Ra])), Tm.ImplementsStiRegionMapElement
+                return Tm.ImplementsStiRegionMapElement || (Tm.ImplementsStiRegionMapElement = super.implements().concat([Jo, Ke, Ze, ye, Oe, _s, ar, Ne, ...Ho, ...Qe, ...Ue, ...Yn, ...en, ...qs, ...rr, l, Qr, Ra])), Tm.ImplementsStiRegionMapElement
             }
             clone(e) {
                 var t, r, i, s;
                 let n = super.clone(e);
                 return n.keyMeter = null != this.keyMeter ? this.keyMeter.clone() : null, n.nameMeter = null != this.nameMeter ? this.nameMeter.clone() : null, n.valueMeter = null != this.valueMeter ? this.valueMeter.clone() : null, n.groupMeter = null != this.groupMeter ? this.groupMeter.clone() : null, n.colorMeter = null != this.colorMeter ? this.colorMeter.clone() : null, n.userFilters = this.userFilters.select(e => e.clone()).toList(), n.transformActions = this.transformActions.select(e => e.clone()).toList(), n.transformFilters = this.transformFilters.select(e => e.clone()).toList(), n.transformSorts = this.transformSorts.select(e => e.clone()).toList(), n.dataFilters = this.dataFilters.select(e => e.clone()).toList(), n.valueFormat = null == (t = this.valueFormat) ? void 0 : t.clone(), n.labels = null == (r = this.labels) ? void 0 : r.clone(), n.title = null != this.title ? this.title.clone() : null, n.layout = null != this.layout ? this.layout.clone() : null, n.dashboardInteraction = this.dashboardInteraction.clone(), n.shadow = null == (i = this.shadow) ? void 0 : i.clone(), n.cornerRadius = null == (s = this.cornerRadius) ? void 0 : s.clone(), n
             }
             meta() {
-                return [...super.meta(), new s("UserFilters").get(e => a.Serialize.objectArray(this.userFilters, e)).set(e => this.userFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.userFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new s("TransformActions").get(e => a.Serialize.objectArray(this.transformActions, e)).set(e => this.transformActions.addRange(e.value.properties().select(e => sn.loadFromJson(e.value)))).setXml(e => this.transformActions.addRange(e.childNodes.select(e => sn.loadFromXml(e)))), new s("TransformFilters").get(e => a.Serialize.objectArray(this.transformFilters, e)).set(e => this.transformFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.transformFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new s("TransformSorts").get(e => a.Serialize.objectArray(this.transformSorts, e)).set(e => this.transformSorts.addRange(e.value.properties().select(e => rn.loadFromJson(e.value)))).setXml(e => this.transformSorts.addRange(e.childNodes.select(e => rn.loadFromXml(e)))), new s("DataFilters").get(e => a.Serialize.objectArray(this.dataFilters, e)).set(e => this.dataFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.dataFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new s("DashboardInteraction").check(() => null != this.dashboardInteraction.as(jo)).set(e => {
+                return [...super.meta(), new s("UserFilters").get(e => a.Serialize.objectArray(this.userFilters, e)).set(e => this.userFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.userFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new s("TransformActions").get(e => a.Serialize.objectArray(this.transformActions, e)).set(e => this.transformActions.addRange(e.value.properties().select(e => nn.loadFromJson(e.value)))).setXml(e => this.transformActions.addRange(e.childNodes.select(e => nn.loadFromXml(e)))), new s("TransformFilters").get(e => a.Serialize.objectArray(this.transformFilters, e)).set(e => this.transformFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.transformFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new s("TransformSorts").get(e => a.Serialize.objectArray(this.transformSorts, e)).set(e => this.transformSorts.addRange(e.value.properties().select(e => sn.loadFromJson(e.value)))).setXml(e => this.transformSorts.addRange(e.childNodes.select(e => sn.loadFromXml(e)))), new s("DataFilters").get(e => a.Serialize.objectArray(this.dataFilters, e)).set(e => this.dataFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.dataFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new s("DashboardInteraction").check(() => null != this.dashboardInteraction.as(jo)).set(e => {
                     var t;
                     let r = null == (t = qr.loadInteractionFromJsonObject(e.value)) ? void 0 : t.as(jo);
                     null != r && (this.dashboardInteraction = r)
                 }).setXml(e => {
                     var t;
                     let r = null == (t = qr.loadInteractionFromXml(e)) ? void 0 : t.as(jo);
                     null != r && (this.dashboardInteraction = r)
-                }), new s("Labels").check(() => null != this.labels).set(e => this.labels = Po.createFromJsonObject(e.value)).setXml(e => this.labels = Po.createFromXml(e)), new s("Title").check(() => null != this.title).set(e => this.title = F.e.StiTitle.createFromJsonObject(e.value)).setXml(e => this.title = F.e.StiTitle.createFromXml(e)), new s("Layout").check(() => null != this.layout).set(e => this.layout = _s.createFromJsonObject(e.value)).setXml(e => this.layout = _s.createFromXml(e)), new s("KeyMeter").check(() => null != this.keyMeter).set(e => {
-                    let t = g.loadFromJson(e.value).as(os);
+                }), new s("Labels").check(() => null != this.labels).set(e => this.labels = Po.createFromJsonObject(e.value)).setXml(e => this.labels = Po.createFromXml(e)), new s("Title").check(() => null != this.title).set(e => this.title = F.e.StiTitle.createFromJsonObject(e.value)).setXml(e => this.title = F.e.StiTitle.createFromXml(e)), new s("Layout").check(() => null != this.layout).set(e => this.layout = $s.createFromJsonObject(e.value)).setXml(e => this.layout = $s.createFromXml(e)), new s("KeyMeter").check(() => null != this.keyMeter).set(e => {
+                    let t = g.loadFromJson(e.value).as(us);
                     null != t && (this.keyMeter = t)
                 }).setXml(e => {
-                    let t = g.loadFromXml(e).as(os);
+                    let t = g.loadFromXml(e).as(us);
                     null != t && (this.keyMeter = t)
                 }), new s("NameMeter").check(() => null != this.nameMeter).set(e => {
                     let t = g.loadFromJson(e.value).as(F.L.StiNameMapMeter);
                     null != t && (this.nameMeter = t)
                 }).setXml(e => {
                     let t = g.loadFromXml(e).as(F.L.StiNameMapMeter);
                     null != t && (this.nameMeter = t)
@@ -8160,32 +8166,36 @@
             }
             fetchAllMeters() {
                 let e = new P;
                 return null != this.keyMeter && e.add(this.keyMeter), null != this.nameMeter && e.add(this.nameMeter), null != this.valueMeter && e.add(this.valueMeter), null != this.groupMeter && e.add(this.groupMeter), null != this.colorMeter && e.add(this.colorMeter), e
             }
             getMeters() {
                 let e = new P;
-                return this.isDefined && this.dataFrom == Wo.DataColumns && (null != this.keyMeter && (Rs.isFunctionPresent(this.keyMeter.expression) ? e.add(this.keyMeter) : e.add(new os(this.keyMeter.key, `Iso2(${this.keyMeter.expression}, "${this.mapIdent}")`))), null != this.nameMeter && e.add(this.nameMeter), null != this.valueMeter && (Rs.isAggregationFunctionPresent(this.valueMeter.expression) ? e.add(this.valueMeter) : e.add(new F.L.StiValueMapMeter(this.valueMeter.key, `First(${this.valueMeter.expression})`))), null != this.groupMeter && e.add(this.groupMeter), null != this.colorMeter) && e.add(this.colorMeter), e
+                return this.isDefined && this.dataFrom == Wo.DataColumns && (null != this.keyMeter && (Es.isFunctionPresent(this.keyMeter.expression) ? e.add(this.keyMeter) : e.add(new us(this.keyMeter.key, `Iso2(${this.keyMeter.expression}, "${this.mapIdent}")`))), null != this.nameMeter && e.add(this.nameMeter), null != this.valueMeter && (Es.isAggregationFunctionPresent(this.valueMeter.expression) ? e.add(this.valueMeter) : e.add(new F.L.StiValueMapMeter(this.valueMeter.key, `First(${this.valueMeter.expression})`))), null != this.groupMeter && e.add(this.groupMeter), null != this.colorMeter) && e.add(this.colorMeter), e
             }
             retrieveUsedDataNames() {
                 let e = new P;
-                return this.dataFrom == Wo.DataColumns && (e.addRange(en.getMany(this.keyMeter)), e.addRange(en.getMany(this.nameMeter)), e.addRange(en.getMany(this.valueMeter)), e.addRange(en.getMany(this.groupMeter)), e.addRange(en.getMany(this.colorMeter))), e.distinct()
+                return this.dataFrom == Wo.DataColumns && (e.addRange(tn.getMany(this.keyMeter)), e.addRange(tn.getMany(this.nameMeter)), e.addRange(tn.getMany(this.valueMeter)), e.addRange(tn.getMany(this.groupMeter)), e.addRange(tn.getMany(this.colorMeter))), e.distinct()
             }
             get isDefined() {
                 return this.dataFrom != Wo.DataColumns || null != this.keyMeter || null != this.nameMeter || null != this.valueMeter || null != this.groupMeter || null != this.colorMeter
             }
             get isQuerable() {
                 return this.dataFrom == Wo.DataColumns
             }
             get font() {
                 return this.labels.font
             }
             set font(e) {
                 this.labels.font = e
             }
+            static getValueFormatDefault() {
+                let e = new Wr;
+                return e.decimalDigits = 1, e.state = F.a.StiTextFormatState.DecimalDigits | F.a.StiTextFormatState.Abbreviation, e
+            }
             get style() {
                 return this._style
             }
             set style(e) {
                 (this._style = e) != o.Custom && (this.customStyleName = "")
             }
             createNextMeter(e) {
@@ -8200,15 +8210,15 @@
             getKeyMeter() {
                 return this.keyMeter
             }
             removeKeyMeter() {
                 this.keyMeter = null
             }
             createNewKeyMeter() {
-                this.keyMeter = new os
+                this.keyMeter = new us
             }
             addNameMeter2(e) {
                 this.nameMeter = null != e ? d.RegionMap.getName2(e) : null
             }
             addNameMeter(e) {
                 this.nameMeter = null != e ? d.RegionMap.getName(e.as(F.e.StiMeter)) : null
             }
@@ -8264,15 +8274,15 @@
                 this.colorMeter = null
             }
             createNewColorMeter() {
                 this.colorMeter = new F.L.StiColorMapMeter
             }
             convertFrom(e) {
                 let t = e.as(F.O.StiOnlineMapElement);
-                null == t || null == t.location || t.location.isDefault() || (this.keyMeter = new os, this.keyMeter.label = t.location.label, this.keyMeter.expression = t.location.expression), null == this.dashboardInteraction && (this.dashboardInteraction = new jo)
+                null == t || null == t.location || t.location.isDefault() || (this.keyMeter = new us, this.keyMeter.label = t.location.label, this.keyMeter.expression = t.location.expression), null == this.dashboardInteraction && (this.dashboardInteraction = new jo)
             }
             setString(e, t) {
                 switch (e) {
                     case "Title.Text":
                         this.title.text = t;
                         break
                 }
@@ -8299,15 +8309,15 @@
             set dashboardInteraction(e) {
                 this._dashboardInteraction = e
             }
             getManuallyEnteredDataTable() {
                 if (this.dataFrom == Wo.Manual) {
                     let e = this.getMapData().orderBy(e => e.key).toList(),
                         r = new Tt;
-                    r.meters.add(new os("Key", "Key")), r.meters.add(new F.L.StiNameMapMeter("Name", "Name")), r.meters.add(new F.L.StiValueMapMeter("Value", "Value"));
+                    r.meters.add(new us("Key", "Key")), r.meters.add(new F.L.StiNameMapMeter("Name", "Name")), r.meters.add(new F.L.StiValueMapMeter("Value", "Value"));
                     for (let t of e) {
                         let e = [];
                         e[0] = t.key, e[1] = t.name, e[2] = t.value, r.rows.add(e)
                     }
                     return r
                 }
                 return null
@@ -8321,15 +8331,15 @@
                 return new P([e])
             }
             getMapData() {
                 let e = new zo;
                 return e.mapData = this.mapData, e.mapIdent = this.mapIdent, e.page = this.page, e.getMapData()
             }
             constructor(e = j.empty) {
-                super(e), this.group = "", this.shadow = new Ye, this.cornerRadius = new m(0), this.title = new F.e.StiTitle, this.valueFormat = new Wr(null, null, null, 1, null, null, null, null, null, L.Report.Components.StiTextFormatState.DecimalDigits | L.Report.Components.StiTextFormatState.Abbreviation), this.layout = new _s, this._style = o.Auto, this.customStyleName = "", this.userFilters = new P, this.transformActions = new P, this.transformFilters = new P, this.transformSorts = new P, this.dataTransformation = {}, this.dataFilters = new P, this.helpUrl = "user-manual/dashboards_maps_region_map.htm", this.dataMode = Vn.UsingDataFields, this.labels = new Po, this.mapIdent = "USA", this.dataFrom = Wo.Manual, this.mapType = Xo.Individual, this.showValue = !0, this.showZeros = !0, this.shortValue = !0, this.colorEach = !1, this.showBubble = !1, this.showName = Go.Full, this.crossFiltering = !0, this.title.text = this.localizedName, this.dashboardInteraction = new jo
+                super(e), this.group = "", this.shadow = new Ye, this.cornerRadius = new m(0), this.title = new F.e.StiTitle, this.valueFormat = Tm.getValueFormatDefault(), this.layout = new $s, this._style = o.Auto, this.customStyleName = "", this.userFilters = new P, this.transformActions = new P, this.transformFilters = new P, this.transformSorts = new P, this.dataTransformation = {}, this.dataFilters = new P, this.helpUrl = "user-manual/dashboards_maps_region_map.htm", this.dataMode = kn.UsingDataFields, this.labels = new Po, this.mapIdent = "USA", this.dataFrom = Wo.Manual, this.mapType = Xo.Individual, this.showValue = !0, this.showZeros = !0, this.shortValue = !0, this.colorEach = !1, this.showBubble = !1, this.showName = Go.Full, this.crossFiltering = !0, this.title.text = this.localizedName, this.dashboardInteraction = new jo
             }
         }
         F.L.StiRegionMapElement = Tm
     } {
         class Qo extends F.g.StiDashboardInteraction {
             StiShapeDashboardInteraction() {}
             constructor(e, t, r, i, s, n, l) {
@@ -8343,15 +8353,15 @@
         Yo = L.Report.Components.StiRectangleShapeType,
         Ko = L.Report.Dashboard.IStiShapeElement,
         Qo = F.g.StiShapeDashboardInteraction;
     {
         dt.add("StiShapeElement", "Stimulsoft.Dashboard.Export.Tools.StiShapeElementExportTool");
         class dm extends F.e.StiElement {
             implements() {
-                return dm.ImplementsStiShapeElement || (dm.ImplementsStiShapeElement = super.implements().concat([Ko, Oe, Qr, Ne, ...Zo, ...$s, l])), dm.ImplementsStiShapeElement
+                return dm.ImplementsStiShapeElement || (dm.ImplementsStiShapeElement = super.implements().concat([Ko, Oe, Qr, Ne, ...Zo, ...en, l])), dm.ImplementsStiShapeElement
             }
             clone(e) {
                 var t, r;
                 let i = super.clone(e);
                 return i.title = null != this.title ? this.title.clone() : null, i.shapeType = null == (t = this.shapeType) ? void 0 : t.clone(), i.dashboardInteraction = null == (r = this.dashboardInteraction) ? void 0 : r.clone(), i
             }
             meta() {
@@ -8455,15 +8465,15 @@
     }
     let qo = L.Report.Dashboard.IStiAllowUserColumnSelectionDashboardInteraction,
         _o = L.Report.Dashboard.IStiTableDashboardInteraction,
         $o = L.Report.Dashboard.IStiAllowUserFilteringDashboardInteraction;
     {
         class tu extends F.g.StiDashboardInteraction {
             implements() {
-                return tu.ImplementsIStiTableDashboardInteraction || (tu.ImplementsIStiTableDashboardInteraction = super.implements().concat([_o, An, qo, $o, l, Gs])), tu.ImplementsIStiTableDashboardInteraction
+                return tu.ImplementsIStiTableDashboardInteraction || (tu.ImplementsIStiTableDashboardInteraction = super.implements().concat([_o, In, qo, $o, l, Xs])), tu.ImplementsIStiTableDashboardInteraction
             }
             meta() {
                 return [...super.meta(), new h("AllowUserColumnSelection", "", !0), new h("AllowUserSorting", "", !0), new h("AllowUserFiltering", "", !0), new h("DrillDownFiltered", "", !0), new h("FullRowSelect"), new h("ShowFullScreenButton", "", !0), new h("ShowSaveButton", "", !0), new h("ShowViewDataButton", "", !0), new n("FileName"), new n("HeaderText"), new n("FooterText")]
             }
             get isDefaultLayout() {
                 return this.showFullScreenButton && this.showSaveButton && this.showViewDataButton && null == this.fileName && null == this.headerText && null == this.footerText
             }
@@ -8531,23 +8541,23 @@
         su = F.h.StiTableElementSelection,
         nu = L.Report.Dashboard.IStiTableElement,
         lu = F.K.StiTableElementCondition;
     {
         dt.add("StiTableElement", "Stimulsoft.Dashboard.Export.Tools.StiTableElementExportTool");
         class ym extends F.e.StiElement {
             implements() {
-                return ym.ImplementsStiTableElement || (ym.ImplementsStiTableElement = super.implements().concat([nu, Ke, Ze, Oe, qs, Ne, ...iu, ...Qe, ...Ue, ...$s, ...Qs, l, Qr, ye])), ym.ImplementsStiTableElement
+                return ym.ImplementsStiTableElement || (ym.ImplementsStiTableElement = super.implements().concat([nu, Ke, Ze, Oe, _s, Ne, ...iu, ...Qe, ...Ue, ...en, ...qs, l, Qr, ye])), ym.ImplementsStiTableElement
             }
             clone(e) {
                 var t, r;
                 let i = super.clone(e);
                 return i.columns = this.columns.select(e => e.clone()).toList(), i.userFilters = this.userFilters.select(e => e.clone()).toList(), i.userSorts = this.userSorts.select(e => e.clone()).toList(), i.transformActions = this.transformActions.select(e => e.clone()).toList(), i.transformFilters = this.transformFilters.select(e => e.clone()).toList(), i.transformSorts = this.transformSorts.select(e => e.clone()).toList(), i.dataFilters = this.dataFilters.select(e => e.clone()).toList(), i.title = null != this.title ? this.title.clone() : null, i.layout = null != this.layout ? this.layout.clone() : null, i.tableConditions = this.tableConditions.select(e => e.clone()).toList(), i.dashboardInteraction = this.dashboardInteraction.clone(), i.shadow = null == (t = this.shadow) ? void 0 : t.clone(), i.cornerRadius = null == (r = this.cornerRadius) ? void 0 : r.clone(), i
             }
             meta() {
-                return [...super.meta(), new s("Columns").get(e => a.Serialize.objectArray(this.columns, e)).set(e => this.columns.addRange(e.value.properties().select(e => g.loadFromJson(e.value).as(Cs)).where(e => null != e))).setXml(e => this.columns.addRange(e.childNodes.select(e => g.loadFromXml(e)).where(e => null != e))), new s("UserFilters").get(e => a.Serialize.objectArray(this.userFilters, e)).set(e => this.userFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.userFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new s("UserSorts").get(e => a.Serialize.objectArray(this.userSorts, e)).set(e => this.userSorts.addRange(e.value.properties().select(e => rn.loadFromJson(e.value)))).setXml(e => this.userSorts.addRange(e.childNodes.select(e => rn.loadFromXml(e)))), new s("TransformActions").get(e => a.Serialize.objectArray(this.transformActions, e)).set(e => this.transformActions.addRange(e.value.properties().select(e => sn.loadFromJson(e.value)))).setXml(e => this.transformActions.addRange(e.childNodes.select(e => sn.loadFromXml(e)))), new s("TransformFilters").get(e => a.Serialize.objectArray(this.transformFilters, e)).set(e => this.transformFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.transformFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new s("TransformSorts").get(e => a.Serialize.objectArray(this.transformSorts, e)).set(e => this.transformSorts.addRange(e.value.properties().select(e => rn.loadFromJson(e.value)))).setXml(e => this.transformSorts.addRange(e.childNodes.select(e => rn.loadFromXml(e)))), new s("DataFilters").get(e => a.Serialize.objectArray(this.dataFilters, e)).set(e => this.dataFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.dataFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new r("HeaderForeColor", "", N.transparent), new r("FooterForeColor", "", N.transparent), new r("ForeColor", "", N.transparent), new n("HeaderFont").get(() => a.Serialize.fontArial8(this.headerFont)).set(e => this.headerFont = a.Deserialize.font(e.value, this.headerFont)).setXml(e => this.headerFont = L.System.Convert.toFont(e.textContent)), new n("FooterFont").get(() => a.Serialize.fontArial8(this.footerFont)).set(e => this.footerFont = a.Deserialize.font(e.value, this.footerFont)).setXml(e => this.footerFont = L.System.Convert.toFont(e.textContent)), new Rt("Font", "", "Arial", 10), new h("CrossFiltering", "", !0), new s("TableConditions").get(e => a.Serialize.objectArray(this.tableConditions.select(e => e[L.System.StiObject.stimulsoft]().as(lu)), e)).set(e => this.tableConditions.addRange(e.value.properties().select(e => lu.createFromJson(e.value)))).setXml(e => this.tableConditions.addRange(e.childNodes.select(e => lu.createFromXml(e)))), new s("Title").check(() => null != this.title), new s("Layout").check(() => null != this.layout), new s("DashboardInteraction").check(() => null != this.dashboardInteraction.as(tu)).set(e => {
+                return [...super.meta(), new s("Columns").get(e => a.Serialize.objectArray(this.columns, e)).set(e => this.columns.addRange(e.value.properties().select(e => g.loadFromJson(e.value).as(xs)).where(e => null != e))).setXml(e => this.columns.addRange(e.childNodes.select(e => g.loadFromXml(e)).where(e => null != e))), new s("UserFilters").get(e => a.Serialize.objectArray(this.userFilters, e)).set(e => this.userFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.userFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new s("UserSorts").get(e => a.Serialize.objectArray(this.userSorts, e)).set(e => this.userSorts.addRange(e.value.properties().select(e => sn.loadFromJson(e.value)))).setXml(e => this.userSorts.addRange(e.childNodes.select(e => sn.loadFromXml(e)))), new s("TransformActions").get(e => a.Serialize.objectArray(this.transformActions, e)).set(e => this.transformActions.addRange(e.value.properties().select(e => nn.loadFromJson(e.value)))).setXml(e => this.transformActions.addRange(e.childNodes.select(e => nn.loadFromXml(e)))), new s("TransformFilters").get(e => a.Serialize.objectArray(this.transformFilters, e)).set(e => this.transformFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.transformFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new s("TransformSorts").get(e => a.Serialize.objectArray(this.transformSorts, e)).set(e => this.transformSorts.addRange(e.value.properties().select(e => sn.loadFromJson(e.value)))).setXml(e => this.transformSorts.addRange(e.childNodes.select(e => sn.loadFromXml(e)))), new s("DataFilters").get(e => a.Serialize.objectArray(this.dataFilters, e)).set(e => this.dataFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.dataFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new r("HeaderForeColor", "", N.transparent), new r("FooterForeColor", "", N.transparent), new r("ForeColor", "", N.transparent), new n("HeaderFont").get(() => a.Serialize.fontArial8(this.headerFont)).set(e => this.headerFont = a.Deserialize.font(e.value, this.headerFont)).setXml(e => this.headerFont = L.System.Convert.toFont(e.textContent)), new n("FooterFont").get(() => a.Serialize.fontArial8(this.footerFont)).set(e => this.footerFont = a.Deserialize.font(e.value, this.footerFont)).setXml(e => this.footerFont = L.System.Convert.toFont(e.textContent)), new Rt("Font", "", "Arial", 10), new h("CrossFiltering", "", !0), new s("TableConditions").get(e => a.Serialize.objectArray(this.tableConditions.select(e => e[L.System.StiObject.stimulsoft]().as(lu)), e)).set(e => this.tableConditions.addRange(e.value.properties().select(e => lu.createFromJson(e.value)))).setXml(e => this.tableConditions.addRange(e.childNodes.select(e => lu.createFromXml(e)))), new s("Title").check(() => null != this.title), new s("Layout").check(() => null != this.layout), new s("DashboardInteraction").check(() => null != this.dashboardInteraction.as(tu)).set(e => {
                     var t;
                     let r = null == (t = qr.loadInteractionFromJsonObject(e.value)) ? void 0 : t.as(tu);
                     null != r && (this.dashboardInteraction = r)
                 }).setXml(e => {
                     var t;
                     let r = null == (t = qr.loadInteractionFromXml(e)) ? void 0 : t.as(tu);
                     null != r && (this.dashboardInteraction = r)
@@ -8559,30 +8569,30 @@
                 for (let e of t.columns) this.columns.add(e)
             }
             createMeters2(t) {
                 this.columns.clear();
                 for (let e of t.columns.list) null != e && null != e.type && Le.isNumericType(e.type) ? this.columns.add(d.Table.getMeasure2(e)) : this.columns.add(d.Table.getDimension2(e))
             }
             createMeter3(e) {
-                let t = e.as(oi),
-                    r = e.as(zs),
+                let t = e.as(ui),
+                    r = e.as(Gs),
                     i = null != t ? t.type : null == r ? void 0 : r.type;
                 if (null != i && Le.isNumericType(i)) {
                     let e = d.Table.getMeasure2(t);
                     e.showTotalSummary = !0, e.summaryType = Kr.Sum, this.columns.add(e)
                 } else this.columns.add(d.Table.getDimension2(e))
             }
             removeMeter(e) {
                 e < this.columns.length && this.columns.removeAt(e)
             }
             removeAllMeters() {
                 this.columns.clear()
             }
             insertMeter(e, t) {
-                let r = t.as(Cs);
+                let r = t.as(xs);
                 if (null == r) return;
                 0 <= e && e < this.columns.length ? this.columns.insert(e, r) : this.columns.add(r)
             }
             insertNewDimension(e) {
                 let t = new F.K.StiDimensionColumn;
                 t.horAlignment = z.Left, this.insertMeter(e, t)
             }
@@ -8607,15 +8617,15 @@
             fetchAllMeters() {
                 return this.columns.cast()
             }
             getMeters() {
                 return this.columns.cast()
             }
             retrieveUsedDataNames() {
-                return en.getMany2(this.columns)
+                return tn.getMany2(this.columns)
             }
             get isDefined() {
                 return null != this.columns && 0 < this.columns.length
             }
             get allowSkipOwnFilter() {
                 return !this.dashboardInteraction.drillDownFiltered
             }
@@ -8677,15 +8687,15 @@
                         null != e && r.add(e)
                     } return 0 == r.length ? null : r.distinct()
             }
             getFormatObjects() {
                 return su.getSelectedObjects(this)
             }
             constructor(e = j.empty) {
-                super(e), this.shadow = new Ye, this.cornerRadius = new m(0), this.title = new F.e.StiTitle, this.layout = new _s, this.group = "", this.foreColor = N.transparent, this.font = new H("Arial", 10), this._style = o.Auto, this.customStyleName = "", this.userFilters = new P, this.userSorts = new P, this.transformActions = new P, this.transformFilters = new P, this.transformSorts = new P, this.dataTransformation = {}, this.dataFilters = new P, this.tableConditions = new P, this.crossFiltering = !0, this.helpUrl = "user-manual/dashboards_table.htm", this.columns = new P, this.sizeMode = ru.AutoSize, this.rowsPerPage = 0, this.pageTurnTime = 0, this.currentPageIndex = -1, this.headerForeColor = N.transparent, this.headerFont = new H("Arial", 10), this.footerForeColor = N.transparent, this.footerFont = new H("Arial", 10), this.title.text = this.localizedName, this.dashboardInteraction = new tu
+                super(e), this.shadow = new Ye, this.cornerRadius = new m(0), this.title = new F.e.StiTitle, this.layout = new $s, this.group = "", this.foreColor = N.transparent, this.font = new H("Arial", 10), this._style = o.Auto, this.customStyleName = "", this.userFilters = new P, this.userSorts = new P, this.transformActions = new P, this.transformFilters = new P, this.transformSorts = new P, this.dataTransformation = {}, this.dataFilters = new P, this.tableConditions = new P, this.crossFiltering = !0, this.helpUrl = "user-manual/dashboards_table.htm", this.columns = new P, this.sizeMode = ru.AutoSize, this.rowsPerPage = 0, this.pageTurnTime = 0, this.currentPageIndex = -1, this.headerForeColor = N.transparent, this.headerFont = new H("Arial", 10), this.footerForeColor = N.transparent, this.footerFont = new H("Arial", 10), this.title.text = this.localizedName, this.dashboardInteraction = new tu
             }
         }
         F.K.StiTableElement = ym
     }
     F.K.StiTableElementConditionHelper = class {
         static async getConditionResult(i, t, s) {
             let e = !1;
@@ -8796,21 +8806,21 @@
                     let e = l[r],
                         t = n[r];
                     if ((null == a.foreColor || null == a.backColor) && 0 <= i.keyDataFieldMeters.indexOf(e) && await this.getConditionResult(t, i, s) && (0 < (i.permissions & eu.ForeColor) && (a.foreColor = i.foreColor), 0 < (i.permissions & eu.BackColor)) && (a.backColor = i.backColor), null != a.backColor && null != a.foreColor) return a
                 }
             return null == a.foreColor && (a.foreColor = e), null == a.backColor && (a.backColor = t), a
         }
         static async processFontStyle(e, t, i, s, n) {
-            let l = hn.Regular;
+            let l = mn.Regular;
             for (let r of i.tableConditions.where(e => 0 <= e.keyDestinationMeters.indexOf(t)))
                 for (let t = 0; t < n.length; t++) {
                     let e = n[t];
                     if (0 <= r.keyDataFieldMeters.indexOf(e)) {
                         let e = s[t];
-                        await this.getConditionResult(e, r, i) && (0 < (r.permissions & eu.FontStyleBold) && r.font.bold && !(l & hn.Bold) && (l ^= hn.Bold), 0 < (r.permissions & eu.FontStyleItalic) && r.font.italic && !(l & hn.Italic) && (l ^= hn.Italic), 0 < (r.permissions & eu.FontStyleUnderline) && r.font.underline && !(l & hn.Underline) && (l ^= hn.Underline), 0 < (r.permissions & eu.FontStyleStrikeout)) && r.font.strikeout && !(l & hn.Strikeout) && (l ^= hn.Strikeout)
+                        await this.getConditionResult(e, r, i) && (0 < (r.permissions & eu.FontStyleBold) && r.font.bold && !(l & mn.Bold) && (l ^= mn.Bold), 0 < (r.permissions & eu.FontStyleItalic) && r.font.italic && !(l & mn.Italic) && (l ^= mn.Italic), 0 < (r.permissions & eu.FontStyleUnderline) && r.font.underline && !(l & mn.Underline) && (l ^= mn.Underline), 0 < (r.permissions & eu.FontStyleStrikeout)) && r.font.strikeout && !(l & mn.Strikeout) && (l ^= mn.Strikeout)
                     }
                 }
             return l
         }
         static async processFontStrikeout(e, t, s, n, l) {
             for (let i of s.tableConditions.where(e => 0 <= e.keyDestinationMeters.indexOf(t)))
                 for (let r = 0; r < l.length; r++) {
@@ -8861,15 +8871,15 @@
         hu = L.Report.Dashboard.ImplementsIStiTextElement,
         mu = L.Report.Dashboard.IStiTextElement,
         cu = L.Report.Components.IStiTextFont;
     {
         dt.add("StiTextElement", "Stimulsoft.Dashboard.Export.Tools.StiTextElementExportTool");
         class fm extends F.e.StiElement {
             implements() {
-                return fm.ImplementsStiTextElement || (fm.ImplementsStiTextElement = super.implements().concat([cu, Ke, Ze, fr, ur, or, mu, Oe, Ne, ...$r, ...Qe, ...Ue, ...Sr, ...sr, ...ir, ...hu, ...$s, l, Qr])), fm.ImplementsStiTextElement
+                return fm.ImplementsStiTextElement || (fm.ImplementsStiTextElement = super.implements().concat([cu, Ke, Ze, fr, ur, or, mu, Oe, Ne, ...$r, ...Qe, ...Ue, ...Sr, ...sr, ...ir, ...hu, ...en, l, Qr])), fm.ImplementsStiTextElement
             }
             clone(e) {
                 var t, r, i;
                 let s = super.clone(e);
                 return s.title = null != this.title ? this.title.clone() : null, s.shadow = null == (t = this.shadow) ? void 0 : t.clone(), s.cornerRadius = null == (r = this.cornerRadius) ? void 0 : r.clone(), s.dashboardInteraction = null == (i = this.dashboardInteraction) ? void 0 : i.clone(), s
             }
             meta() {
@@ -8892,19 +8902,19 @@
             fetchAllMeters() {
                 return this.getMeters()
             }
             getMeters() {
                 var e;
                 if (Z.Engine.dashboardTextElementExpressionParser == au.ReportParser) return new P;
                 if (B.isNullOrEmpty(this.text)) return null;
-                return null == (e = Rs.fetchBlocksFromExpression(this.text)) ? void 0 : e.select(e => new F.W.StiTextMeter(e, e, e)).cast().toList();
+                return null == (e = Es.fetchBlocksFromExpression(this.text)) ? void 0 : e.select(e => new F.W.StiTextMeter(e, e, e)).cast().toList();
                 return null
             }
             retrieveUsedDataNames() {
-                return Z.Engine.dashboardTextElementExpressionParser == au.ReportParser ? super.retrieveUsedDataNames() : en.getMany2(this.getMeters()).distinct().toList()
+                return Z.Engine.dashboardTextElementExpressionParser == au.ReportParser ? super.retrieveUsedDataNames() : tn.getMany2(this.getMeters()).distinct().toList()
             }
             getSimpleText() {
                 return this.getHtmlTextHelper().getSimpleText(this.text, J.getForeColor(this))
             }
             getFont() {
                 let e = this.getHtmlTextHelper();
                 if (null == e) return null;
@@ -9019,23 +9029,23 @@
     };
     let du = L.Report.Dashboard.ImplementsIStiTreeViewElement,
         gu = L.Report.Dashboard.IStiTreeViewElement;
     {
         dt.add("StiTreeViewElement", "Stimulsoft.Dashboard.Export.Tools.StiTreeViewElementExportTool");
         class wm extends F.e.StiElement {
             implements() {
-                return wm.ImplementsStiTreeViewElement || (wm.ImplementsStiTreeViewElement = super.implements().concat([gu, Ke, Ze, Oe, Ne, ...du, ...Qe, ...Ue, ...$s, l])), wm.ImplementsStiTreeViewElement
+                return wm.ImplementsStiTreeViewElement || (wm.ImplementsStiTreeViewElement = super.implements().concat([gu, Ke, Ze, Oe, Ne, ...du, ...Qe, ...Ue, ...en, l])), wm.ImplementsStiTreeViewElement
             }
             clone(e) {
                 var t, r;
                 let i = super.clone(e);
                 return i.keyMeters = this.keyMeters.select(e => e.clone()).toList(), i.userFilters = this.userFilters.select(e => e.clone()).toList(), i.transformActions = this.transformActions.select(e => e.clone()).toList(), i.transformFilters = this.transformFilters.select(e => e.clone()).toList(), i.transformSorts = this.transformSorts.select(e => e.clone()).toList(), i.dataFilters = this.dataFilters.select(e => e.clone()).toList(), i.textFormat = this.textFormat.clone(), i.title = null != this.title ? this.title.clone() : null, i.shadow = null == (t = this.shadow) ? void 0 : t.clone(), i.cornerRadius = null == (r = this.cornerRadius) ? void 0 : r.clone(), i
             }
             meta() {
-                return [...super.meta(), new n("ParentKey"), new s("UserFilters").get(e => a.Serialize.objectArray(this.userFilters, e)).set(e => this.userFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.userFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new s("TransformActions").get(e => a.Serialize.objectArray(this.transformActions, e)).set(e => this.transformActions.addRange(e.value.properties().select(e => sn.loadFromJson(e.value)))).setXml(e => this.transformActions.addRange(e.childNodes.select(e => sn.loadFromXml(e)))), new s("TransformFilters").get(e => a.Serialize.objectArray(this.transformFilters, e)).set(e => this.transformFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.transformFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new s("TransformSorts").get(e => a.Serialize.objectArray(this.transformSorts, e)).set(e => this.transformSorts.addRange(e.value.properties().select(e => rn.loadFromJson(e.value)))).setXml(e => this.transformSorts.addRange(e.childNodes.select(e => rn.loadFromXml(e)))), new s("DataFilters").get(e => a.Serialize.objectArray(this.dataFilters, e)).set(e => this.dataFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.dataFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new r("ForeColor", "", N.transparent), new n("Font").get(() => a.Serialize.fontArial8(this.font)).set(e => this.font = a.Deserialize.font(e.value, this.font)).setXml(e => this.font = L.System.Convert.toFont(e.textContent)), new h("ShowAllValue"), new h("ShowBlanks"), new s("KeyMeters").get(e => a.Serialize.objectArray(this.keyMeters, e)).set(e => this.keyMeters.addRange(e.value.properties().select(e => g.loadFromJson(e.value)))).setXml(e => this.keyMeters.addRange(e.childNodes.select(e => g.loadFromXml(e)))), new s("Title").check(() => null != this.title).set(e => this.title = F.e.StiTitle.createFromJsonObject(e.value)).setXml(e => this.title = F.e.StiTitle.createFromXml(e)), new i("SelectionMode", "", gl, gl.Multi), new i("Style", "", o, o.Auto), new n("Group"), new n("CustomStyleName"), new n("CornerRadius").get(() => this.cornerRadius.toString()).set(e => this.cornerRadius = m.tryParse(e.value.toString())).setXml(e => this.cornerRadius = m.tryParse(e.textContent)), new n("Shadow").get(() => a.Serialize.jShadow(this.shadow)).set(e => this.shadow = a.Deserialize.simpleSahdow(e.value)).setXml(e => this.shadow = Ye.loadFromXml(e.textContent)), new s("TextFormat").check(() => null != this.textFormat).set(e => this.textFormat = br.createFromJsonObject(e.value)).setXml(e => this.textFormat = br.loadFormatFromXml(e, this.report))]
+                return [...super.meta(), new n("ParentKey"), new s("UserFilters").get(e => a.Serialize.objectArray(this.userFilters, e)).set(e => this.userFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.userFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new s("TransformActions").get(e => a.Serialize.objectArray(this.transformActions, e)).set(e => this.transformActions.addRange(e.value.properties().select(e => nn.loadFromJson(e.value)))).setXml(e => this.transformActions.addRange(e.childNodes.select(e => nn.loadFromXml(e)))), new s("TransformFilters").get(e => a.Serialize.objectArray(this.transformFilters, e)).set(e => this.transformFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.transformFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new s("TransformSorts").get(e => a.Serialize.objectArray(this.transformSorts, e)).set(e => this.transformSorts.addRange(e.value.properties().select(e => sn.loadFromJson(e.value)))).setXml(e => this.transformSorts.addRange(e.childNodes.select(e => sn.loadFromXml(e)))), new s("DataFilters").get(e => a.Serialize.objectArray(this.dataFilters, e)).set(e => this.dataFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.dataFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new r("ForeColor", "", N.transparent), new n("Font").get(() => a.Serialize.fontArial8(this.font)).set(e => this.font = a.Deserialize.font(e.value, this.font)).setXml(e => this.font = L.System.Convert.toFont(e.textContent)), new h("ShowAllValue"), new h("ShowBlanks"), new s("KeyMeters").get(e => a.Serialize.objectArray(this.keyMeters, e)).set(e => this.keyMeters.addRange(e.value.properties().select(e => g.loadFromJson(e.value)))).setXml(e => this.keyMeters.addRange(e.childNodes.select(e => g.loadFromXml(e)))), new s("Title").check(() => null != this.title).set(e => this.title = F.e.StiTitle.createFromJsonObject(e.value)).setXml(e => this.title = F.e.StiTitle.createFromXml(e)), new i("SelectionMode", "", gl, gl.Multi), new i("Style", "", o, o.Auto), new n("Group"), new n("CustomStyleName"), new n("CornerRadius").get(() => this.cornerRadius.toString()).set(e => this.cornerRadius = m.tryParse(e.value.toString())).setXml(e => this.cornerRadius = m.tryParse(e.textContent)), new n("Shadow").get(() => a.Serialize.jShadow(this.shadow)).set(e => this.shadow = a.Deserialize.simpleSahdow(e.value)).setXml(e => this.shadow = Ye.loadFromXml(e.textContent)), new s("TextFormat").check(() => null != this.textFormat).set(e => this.textFormat = br.createFromJsonObject(e.value)).setXml(e => this.textFormat = br.loadFormatFromXml(e, this.report))]
             }
             getParentKey() {
                 return this.parentKey
             }
             setParentKey(e) {
                 this.parentKey = e
             }
@@ -9054,15 +9064,15 @@
                 return e.addRange(this.keyMeters), e
             }
             getMeters() {
                 let e = new P;
                 return e.addRange(this.keyMeters), e
             }
             retrieveUsedDataNames() {
-                return en.getMany2(this.keyMeters)
+                return tn.getMany2(this.keyMeters)
             }
             get isDefined() {
                 return null != this.keyMeters && 0 < this.keyMeters.length
             }
             getKeyMeter(e) {
                 return null != e ? d.TreeView.getKey2(e) : null
             }
@@ -9166,34 +9176,34 @@
                 if (null == i) return null;
                 let s = i.meter,
                     n = s.expression;
                 return Sl.createEqualBasedOnValue(i.key, n, e).toList()
             }
             static format(e, t) {
                 var r, i;
-                return t instanceof w && !e.textFormat.is(Xr) ? t.toShortDateString() : li.isEligable(t, null == (r = null == e ? void 0 : e.report) ? void 0 : r.culture) ? li.convert(t, null == (i = null == e ? void 0 : e.report) ? void 0 : i.culture) : e.textFormat.format(t)
+                return t instanceof w && !e.textFormat.is(Xr) ? t.toShortDateString() : ai.isEligable(t, null == (r = null == e ? void 0 : e.report) ? void 0 : r.culture) ? ai.convert(t, null == (i = null == e ? void 0 : e.report) ? void 0 : i.culture) : e.textFormat.format(t)
             }
             static format2(e, t) {
                 var r;
                 if (t instanceof w && !e.textFormat.is(Xr)) return t.toShortDateString();
                 let i = null == (r = null == e ? void 0 : e.report) ? void 0 : r.getParsedCulture();
-                if (li.isEligable(t, i)) return li.convert(t, i);
+                if (ai.isEligable(t, i)) return ai.convert(t, i);
                 return e.textFormat.format(t)
             }
         }, L.Report.Dashboard.ImplementsIStiTreeViewBoxElement),
         wu = F.J.StiTreeViewHelper,
         bu = L.Report.Dashboard.IStiTreeViewBoxElement;
     {
         dt.add("StiTreeViewBoxElement", "Stimulsoft.Dashboard.Export.Tools.StiTreeViewBoxElementExportTool");
         class Sm extends F.e.StiElement {
             implements() {
                 return Sm.ImplementsStiTreeViewBoxElement || (Sm.ImplementsStiTreeViewBoxElement = super.implements().concat([bu, Ke, Ze, lr, ...Su, ...Qe, ...Ue, ...tr, l])), Sm.ImplementsStiTreeViewBoxElement
             }
             meta() {
-                return [...super.meta(), new n("ParentKey"), new s("UserFilters").get(e => a.Serialize.objectArray(this.userFilters, e)).set(e => this.userFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.userFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new s("TransformActions").get(e => a.Serialize.objectArray(this.transformActions, e)).set(e => this.transformActions.addRange(e.value.properties().select(e => sn.loadFromJson(e.value)))).setXml(e => this.transformActions.addRange(e.childNodes.select(e => sn.loadFromXml(e)))), new s("TransformFilters").get(e => a.Serialize.objectArray(this.transformFilters, e)).set(e => this.transformFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.transformFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new s("TransformSorts").get(e => a.Serialize.objectArray(this.transformSorts, e)).set(e => this.transformSorts.addRange(e.value.properties().select(e => rn.loadFromJson(e.value)))).setXml(e => this.transformSorts.addRange(e.childNodes.select(e => rn.loadFromXml(e)))), new s("DataFilters").get(e => a.Serialize.objectArray(this.dataFilters, e)).set(e => this.dataFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.dataFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new r("ForeColor", "", N.transparent), new n("Font").get(() => a.Serialize.fontArial8(this.font)).set(e => this.font = a.Deserialize.font(e.value, this.font)).setXml(e => this.font = L.System.Convert.toFont(e.textContent)), new h("ShowAllValue"), new h("ShowBlanks"), new i("SelectionMode", "", gl, gl.One).set(e => {
+                return [...super.meta(), new n("ParentKey"), new s("UserFilters").get(e => a.Serialize.objectArray(this.userFilters, e)).set(e => this.userFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.userFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new s("TransformActions").get(e => a.Serialize.objectArray(this.transformActions, e)).set(e => this.transformActions.addRange(e.value.properties().select(e => nn.loadFromJson(e.value)))).setXml(e => this.transformActions.addRange(e.childNodes.select(e => nn.loadFromXml(e)))), new s("TransformFilters").get(e => a.Serialize.objectArray(this.transformFilters, e)).set(e => this.transformFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.transformFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new s("TransformSorts").get(e => a.Serialize.objectArray(this.transformSorts, e)).set(e => this.transformSorts.addRange(e.value.properties().select(e => sn.loadFromJson(e.value)))).setXml(e => this.transformSorts.addRange(e.childNodes.select(e => sn.loadFromXml(e)))), new s("DataFilters").get(e => a.Serialize.objectArray(this.dataFilters, e)).set(e => this.dataFilters.addRange(e.value.properties().select(e => f.loadFromJson(e.value)))).setXml(e => this.dataFilters.addRange(e.childNodes.select(e => f.loadFromXml(e)))), new r("ForeColor", "", N.transparent), new n("Font").get(() => a.Serialize.fontArial8(this.font)).set(e => this.font = a.Deserialize.font(e.value, this.font)).setXml(e => this.font = L.System.Convert.toFont(e.textContent)), new h("ShowAllValue"), new h("ShowBlanks"), new i("SelectionMode", "", gl, gl.One).set(e => {
                     let t = ve.parse(gl, e.value);
                     null != t && (this.selectionMode = t)
                 }).setXml(e => {
                     let t = ve.parse(gl, e.textContent);
                     null != t && (this.selectionMode = t)
                 }), new s("KeyMeters").get(e => a.Serialize.objectArray(this.keyMeters, e)).set(e => this.keyMeters.addRange(e.value.properties().select(e => g.loadFromJson(e.value)))).setXml(e => this.keyMeters.addRange(e.childNodes.select(e => g.loadFromXml(e)))), new i("Style", "", o, o.Auto), new n("Group"), new n("CustomStyleName"), new n("CornerRadius").get(() => this.cornerRadius.toString()).set(e => this.cornerRadius = m.tryParse(e.value.toString())).setXml(e => this.cornerRadius = m.tryParse(e.textContent)), new n("Shadow").get(() => a.Serialize.jShadow(this.shadow)).set(e => this.shadow = a.Deserialize.simpleSahdow(e.value)).setXml(e => this.shadow = Ye.loadFromXml(e.textContent)), new s("TextFormat").check(() => null != this.textFormat).set(e => this.textFormat = br.createFromJsonObject(e.value)).setXml(e => this.textFormat = br.loadFormatFromXml(e, this.report)), new le("MinSize"), new le("MaxSize")]
             }
@@ -9223,15 +9233,15 @@
                 return e.addRange(this.keyMeters), e
             }
             getMeters() {
                 let e = new P;
                 return e.addRange(this.keyMeters), e
             }
             retrieveUsedDataNames() {
-                return en.getMany2(this.keyMeters)
+                return tn.getMany2(this.keyMeters)
             }
             get isDefined() {
                 return null != this.keyMeters && 0 < this.keyMeters.length
             }
             getKeyMeter(e) {
                 return null != e ? d.TreeViewBox.getKey2(e) : null
             }
@@ -9292,15 +9302,15 @@
     }
     let fu = L.Report.Dashboard.ImplementsIStiWebContentElement,
         yu = L.Report.Dashboard.IStiWebContentElement;
     {
         dt.add("StiWebContentElement", "Stimulsoft.Dashboard.Export.Tools.StiWebContentElementExportTool");
         class mm extends F.e.StiElement {
             implements() {
-                return mm.ImplementsStiWebContentElement || (mm.ImplementsStiWebContentElement = super.implements().concat([yu, Ze, Ke, Oe, ...fu, ...Ue, ...Qe, ...$s, l])), mm.ImplementsStiWebContentElement
+                return mm.ImplementsStiWebContentElement || (mm.ImplementsStiWebContentElement = super.implements().concat([yu, Ze, Ke, Oe, ...fu, ...Ue, ...Qe, ...en, l])), mm.ImplementsStiWebContentElement
             }
             clone(e) {
                 var t, r;
                 let i = super.clone(e);
                 return i.title = null != this.title ? this.title.clone() : null, i.shadow = null == (t = this.shadow) ? void 0 : t.clone(), i.cornerRadius = null == (r = this.cornerRadius) ? void 0 : r.clone(), i
             }
             meta() {
@@ -9421,16 +9431,16 @@
                     n = (l.selectAll(), l.setSelectionFont(i), l.setSelectionSize(s), new vu(!1, !1, !1, !1, s, i, r, N.white, !1, !1, 0, 0, 0, X.Center)),
                     a = null,
                     o = new Fu(n, 0),
                     u = xu.parseHtmlToStates(e, o, !1);
                 for (let n of u) {
                     let e = l.text.length,
                         t = (l.select(e, 0), null),
-                        r = (t = B.isNullOrEmpty(n.ts.href) ? n.text.toString() : `<a href="${n.ts.href}">${n.text.toString()}</a>`, l.text += t, l.select(e, n.text.length), hn.Regular),
-                        i = (n.ts.bold && (r |= hn.Bold), n.ts.italic && (r |= hn.Italic), n.ts.underline && (r |= hn.Underline), n.ts.fontName),
+                        r = (t = B.isNullOrEmpty(n.ts.href) ? n.text.toString() : `<a href="${n.ts.href}">${n.text.toString()}</a>`, l.text += t, l.select(e, n.text.length), mn.Regular),
+                        i = (n.ts.bold && (r |= mn.Bold), n.ts.italic && (r |= mn.Italic), n.ts.underline && (r |= mn.Underline), n.ts.fontName),
                         s = n.ts.fontSize;
                     null == a && (a = l.font = new H(i, s)), l.selectionFont = Cu.changeFontStyle2(i, s, r), l.selectionColor = n.ts.fontColor, l.selectionAlignment = this.getAlignment(n.ts.textAlign)
                 }
                 l.select(0, 0)
             }
             getHtmlText(a, o) {
                 let u = !1,
@@ -9441,17 +9451,17 @@
                     e = (a.selectAll(), null != a.selectionFont ? a.selectionFont.name : "Arial"),
                     t = null != a.selectionFont ? a.selectionFont.sizeInPoints : 12,
                     r = ve.getName(Mu, a.selectionAlignment);
                 d = d + `<font face="${e}" size="${t}">` + `<text-align="${r}">`;
                 for (let l = 0; l < a.text.length; l++) {
                     a.select(l, 1);
                     let e = a.selectionFont,
-                        t = null != e && e.style & hn.Bold,
-                        r = null != e && e.style & hn.Italic,
-                        i = null != e && e.style & hn.Underline,
+                        t = null != e && e.style & mn.Bold,
+                        r = null != e && e.style & mn.Italic,
+                        i = null != e && e.style & mn.Underline,
                         s = a.selectionColor,
                         n = "\n" == a.text[l];
                     n && (d += "<br />"), t && !u && (u = !0, d += "<b>"), !t && u && (u = !1, d += "</b>"), r && !h && (h = !0, d += "<i>"), !r && h && (h = !1, d += "</i>"), i && !m && (m = !0, d += "<u>"), !i && m && (m = !1, d += "</u>"), c.equals(s) || (c = (c.equals(o) ? d += `<font-color="${Tu.toHtml(s)}">` : s.equals(o) ? d += "</font-color>" : d = (d += "</font-color>") + `<font-color="${Tu.toHtml(s)}">`, s)), d += a.text[l]
                 }
                 return c.equals(o) || (d += "</font-color>"), m && (d += "</u>"), h && (d += "</i>"), u && (d += "</b>"), (d = d + "</text-align>" + "</font>").toString()
             }
             getAlignment(e) {
@@ -9535,19 +9545,19 @@
                     n = s.width > r.width ? r.width / s.width : 1,
                     l = s.height > r.height ? r.height / s.height : 1,
                     a = Math.min(Math.abs(n), Math.abs(l));
                 return i.size * a
             }
         }, F.h.StiCardsElementHelper = class {
             static minDataColumnValue(e, t, r) {
-                if (!(e.is2(Pi) || e.is2(Bi) || e.is2(Li))) return 0;
+                if (!(e.is2(ji) || e.is2(Pi) || e.is2(Bi))) return 0;
                 return t.rows.any() ? t.rows.min(e => V.tryToNumber(e[r])) : 0
             }
             static maxDataColumnValue(e, t, r) {
-                if (!(e.is2(Pi) || e.is2(Bi) || e.is2(Li))) return 0;
+                if (!(e.is2(ji) || e.is2(Pi) || e.is2(Bi))) return 0;
                 return t.rows.any() ? t.rows.max(e => V.tryToNumber(e[r])) : 0
             }
         }, L.Base.Context.StiLinesSegmentGeom),
         Nu = (F.j.StiVisual = class {
             async draw(e, t) {}
             drawArrowMore(e, t, r) {
                 let i = [],
@@ -9555,15 +9565,15 @@
                 e.fillPath(N.fromArgb2(140, 140, 140), s, t.clone(), null)
             }
         }, L.Base.Context.StiFontGeom),
         Lu = L.Base.Drawing.StiRotationMode,
         Bu = (F.h.StiStringFormatHelper = class {
             static getStringFormatGeom(e) {
                 let t = e.getGenericStringFormat();
-                return t.trimming = Ru.None, t.alignment = mn.Center, t.lineAlignment = mn.Center, t
+                return t.trimming = Ru.None, t.alignment = cn.Center, t.lineAlignment = cn.Center, t
             }
             static measureAlignmentParameters(e, t, r, i) {
                 switch (e) {
                     case z.Left:
                         r.ref = Lu.LeftCenter, i.ref.x = t.x, i.ref.y = t.y + t.height / 2;
                         break;
                     case z.Center:
@@ -9589,15 +9599,15 @@
         Hu = L.Report.Painters.StiLineSparklinesCellPainter,
         zu = L.Report.Painters.StiColumnSparklinesCellPainter,
         Gu = F.K.StiSparklinesType,
         Xu = F.h.StiStringFormatHelper;
     {
         class Ku {
             static DataBarsDraw(t, e, r, i, s, n, l, a, o, u) {
-                let h = ts.formatBasedOnColumnType2(r, n.textFormat, n, a);
+                let h = rs.formatBasedOnColumnType2(r, n.textFormat, n, a);
                 if (null == a || 0 == a) return;
                 0 < o && (o = 0), u < 0 && (u = 0);
                 let m = e.clone(),
                     c = (m.inflate(-1 * l, -1 * l), t.fillRectangle(N.fromArgb3(40, i.cellDataBarsPositive), m.clone(), null), u + Math.abs(o)),
                     d = m.width * Math.abs(o) / c,
                     g = m.width * u / c,
                     p = m.width * Math.abs(a) / c,
@@ -9609,15 +9619,15 @@
                         t.fillRectangle(i.cellDataBarsOverlapped, e, null)
                     }
                 }
                 let w = t.measureString(h, new Nu(n.font.fontFamily.name, n.font.size, n.font.style, L.System.Drawing.GraphicsUnit.Point));
                 Ku.drawText(t, h, n.font, s, n.horAlignment, n.vertAlignment, e, w, l)
             }
             static colorScaleDraw(e, t, r, i, s, n, l, a, o, u) {
-                let h = ts.formatBasedOnColumnType2(r, n.textFormat, n, a),
+                let h = rs.formatBasedOnColumnType2(r, n.textFormat, n, a),
                     m = this.getScaleColor(V.tryToNumber(a), o, u, i.cellBackColor, n.minimumColor, n.maximumColor),
                     c = t.clone(),
                     d = (c.inflate(-1 * l, -1 * l), e.fillRectangle(m, c, null), e.measureString(h, new Nu(n.font.fontFamily.name, n.font.size, n.font.style, L.System.Drawing.GraphicsUnit.Point)));
                 this.drawText(e, h, n.font, s, n.horAlignment, n.vertAlignment, t, d, l)
             }
             static getScaleColor(t, r, i, s, n, l) {
                 let a = (i - r) / 2,
@@ -9655,19 +9665,19 @@
                             break;
                         default:
                             throw new ca(i.type)
                     }
                 }
             }
             static castToArray(e) {
-                return Ln.isArray(e) ? e : null
+                return Bn.isArray(e) ? e : null
             }
             static bubbleDraw(i, r, e, s, n, l, a, o, t, u, h = !0) {
                 if (0 == o) return;
-                let m = ts.formatBasedOnColumnType2(e, l.textFormat, l, o),
+                let m = rs.formatBasedOnColumnType2(e, l.textFormat, l, o),
                     c = (0 < t && (t = 0), u < 0 && (u = 0), l.horAlignment),
                     d = r.clone();
                 if (d.inflate(-1, -1), d = this.calculateBubbleRect(d, l, Math.abs(o), t, u, a), h && c != z.Center) {
                     let e = l.horAlignment == z.Left ? z.Right : z.Left,
                         t = i.measureString(m, new Nu(l.font.fontFamily.name, l.font.size, l.font.style, L.System.Drawing.GraphicsUnit.Point));
                     this.drawText(i, m, l.font, n, e, l.vertAlignment, r, t, a)
                 }
@@ -9742,15 +9752,15 @@
             }
             static getHorAlignment(e) {
                 let t = e.as(Cr);
                 return null != t ? t.horAlignment : z.Right
             }
             static getCellText(e, t, r) {
                 if (null == r) return "";
-                return ts.formatAsPercentage2(null == e ? void 0 : e.report, t.textFormat, r)
+                return rs.formatAsPercentage2(null == e ? void 0 : e.report, t.textFormat, r)
             }
             static drawIndicator(h, m, c, d, e) {
                 let g = Math.min(m.width, m.height);
                 if (null == c || 0 == c) h.fillRectangle(d.cellIndicatorNeutral, new j(m.x + (m.width - g) / 2, m.y + (m.height - 4) / 2, g, 5), null);
                 else {
                     let e = .75 * g,
                         t = (m = new j(m.x + (m.width - g) / 2, m.y + (m.height - e) / 2, g, e)).width / 2,
@@ -9764,23 +9774,23 @@
             }
             static imageDraw(e, t, r) {
                 let i = Bu.getImageBytesFromObject(r);
                 e.drawImage(i, t)
             }
             static drawWordWrapText(e, t, r, i, s, n, l, a, o) {
                 let u = e.getGenericStringFormat();
-                switch (u.trimming = Ru.None, u.lineAlignment = mn.Center, s) {
+                switch (u.trimming = Ru.None, u.lineAlignment = cn.Center, s) {
                     case z.Left:
-                        u.alignment = mn.Near;
+                        u.alignment = cn.Near;
                         break;
                     case z.Center:
-                        u.alignment = mn.Center;
+                        u.alignment = cn.Center;
                         break;
                     case z.Right:
-                        u.alignment = mn.Far;
+                        u.alignment = cn.Far;
                         break
                 }
                 let h = 0,
                     m = (l.width < a.width ? l : a).width,
                     c = Lu.CenterCenter;
                 switch (s) {
                     case z.Left:
@@ -9807,15 +9817,15 @@
                 }
                 let g = new j(h, d, m, a.height),
                     p = F.t.StiCardsVisual.getFontGeom(r, o);
                 e.drawRotatedString6(t, p, i, g, u, c, 0, !0, l.width)
             }
             static drawText(e, t, r, i, s, n, l, a, o) {
                 let u = Xu.getStringFormatGeom(e),
-                    h = (u.alignment = mn.Far, 0),
+                    h = (u.alignment = cn.Far, 0),
                     m = (l.width < a.width ? l : a).width;
                 switch (s) {
                     case z.Left:
                         h = l.x;
                         break;
                     case z.Center:
                         h = l.x + l.width / 2 - m / 2;
@@ -9994,28 +10004,28 @@
                         o = n.font,
                         i = M[d],
                         s = p.x + S.cards.margin.left * x + S.cards.padding.left * x + i.x,
                         u = p.y + S.cards.margin.top * x + S.cards.padding.top * x + i.y,
                         h = i.width,
                         m = i.height - S.cards.padding.top * x - S.cards.padding.bottom * x,
                         c = new j(s, u, h, m);
-                    if (n.is2(Pi)) {
-                        let e = n.as(Pi);
+                    if (n.is2(ji)) {
+                        let e = n.as(ji);
                         Ku.DataBarsDraw(g, c, S, C, a, e, x, V.tryToNumber(l), t, r)
-                    } else if (n.is2(Bi)) {
-                        let e = n.as(Bi);
+                    } else if (n.is2(Pi)) {
+                        let e = n.as(Pi);
                         Ku.colorScaleDraw(g, c, S, C, a, e, x, V.tryToNumber(l), t, r)
-                    } else if (n.is2(ji)) {
-                        let e = n.as(ji);
+                    } else if (n.is2(Hi)) {
+                        let e = n.as(Hi);
                         Ku.sparklinesDraw(g, c, e, l, C)
+                    } else if (n.is2(Bi)) {
+                        let e = n.as(Bi);
+                        Ku.bubbleDraw(g, c, S, C, a, e, x, V.tryToNumber(l), t, r)
                     } else if (n.is2(Li)) {
                         let e = n.as(Li);
-                        Ku.bubbleDraw(g, c, S, C, a, e, x, V.tryToNumber(l), t, r)
-                    } else if (n.is2(Ni)) {
-                        let e = n.as(Ni);
                         Ku.indicatorDraw(g, c, S, C, e, x, V.tryToNullableNumber(l))
                     } else {
                         let s = Bu.getImageFromObject(l);
                         if (null != s && null != s.height) {
                             let e = c.height / s.height,
                                 t = s.width * e,
                                 r = 0;
@@ -10030,20 +10040,20 @@
                                     r = c.x + c.width - t;
                                     break
                             }
                             let i = new j(r, c.y, t, c.height);
                             Ku.imageDraw(g, i, l)
                         } else {
                             let e = this.processRowValue(l, n),
-                                r = ts.formatBasedOnColumnType2(S, n.textFormat, n, e),
+                                r = rs.formatBasedOnColumnType2(S, n.textFormat, n, e),
                                 t = n.as(_t),
                                 i = new Nu(o.fontFamily.name, o.size, o.style, L.System.Drawing.GraphicsUnit.Point);
                             if (null != t && t.wordWrap) {
                                 let e = g.getGenericStringFormat(),
-                                    t = (e.trimming = Ru.None, e.alignment = mn.Center, e.lineAlignment = mn.Center, g.measureString2(r, i, c.width, e));
+                                    t = (e.trimming = Ru.None, e.alignment = cn.Center, e.lineAlignment = cn.Center, g.measureString2(r, i, c.width, e));
                                 Ku.drawWordWrapText(g, r, o, a, n.horAlignment, n.vertAlignment, c, t, x)
                             } else {
                                 let e = g.measureString(r, i);
                                 Ku.drawText(g, r, o, a, n.horAlignment, n.vertAlignment, c, e, x)
                             }
                         }
                     }
@@ -10059,32 +10069,32 @@
             processRowValue(e, t) {
                 var r;
                 let i = t.ident == Ju.SparklinesColumn;
                 return e = Wu.isList(e) ? i ? Wu.toList(e) : null == (r = Wu.toList(e)) ? void 0 : r.firstOrDefault() : e
             }
             static measureItem(i, s, n, l, a, o) {
                 let u;
-                if (n.is2(Pi) || n.is2(Bi)) u = this.measureDataBarsCell(i, s, n, l, a);
-                else if (n.is2(ji)) {
-                    let e = n.as(ji);
+                if (n.is2(ji) || n.is2(Pi)) u = this.measureDataBarsCell(i, s, n, l, a);
+                else if (n.is2(Hi)) {
+                    let e = n.as(Hi);
                     u = this.measureSparklinesCell(e, a)
-                } else if (n.is2(Ni)) {
-                    let e = n.as(Ni);
-                    u = this.measureIndicatorCell(i, s, e, l, a)
                 } else if (n.is2(Li)) {
                     let e = n.as(Li);
+                    u = this.measureIndicatorCell(i, s, e, l, a)
+                } else if (n.is2(Bi)) {
+                    let e = n.as(Bi);
                     u = this.measureBubbleCell(i, s, e, l, a)
                 } else if (Bu.isImage(l)) {
                     let e = Bu.getImageFromObject(l),
                         t = 50 * a,
                         r = t / e.height,
                         i = e.width * r;
                     u = new W(i, t)
                 } else {
-                    let t = ts.formatBasedOnColumnType2(s, n.textFormat, n, l),
+                    let t = rs.formatBasedOnColumnType2(s, n.textFormat, n, l),
                         r = this.getFontGeom(n.font, a),
                         e = n.as(_t);
                     if (null != e && e.wordWrap) {
                         let e = i.getGenericStringFormat();
                         u = i.measureString2(t, r, o, e), u = new W(o, u.height)
                     } else u = i.measureString(t, r)
                 }
@@ -10139,22 +10149,22 @@
                 return new W(a.width, 1.5 * a.height)
             }
             static measureSparklinesCell(e, t) {
                 let r = 0 == e.height ? 20 : e.height;
                 return new W(0, r * t)
             }
             static measureIndicatorCell(e, t, r, i, s) {
-                let n = r.as(Ni),
+                let n = r.as(Li),
                     l = Ku.getCellText(t, n, V.tryToNullableNumber(i)),
                     a = this.getFontGeom(r.font, s),
                     o = e.measureString(l, a);
                 return new W(o.width, 1.5 * o.height)
             }
             static measureBubbleCell(e, t, r, i, s) {
-                let n = ts.formatBasedOnColumnType2(t, r.textFormat, r, i),
+                let n = rs.formatBasedOnColumnType2(t, r.textFormat, r, i),
                     l = this.getFontGeom(r.font, s),
                     a = e.measureString(n, l);
                 return a.width += 4, a = new W(a.width + a.height, 1.5 * a.height)
             }
             static getForeColor(e, t, r) {
                 if (!t.foreColor.equals(N.transparent)) return t.foreColor;
                 let i = J.getForeColor(e);
@@ -10455,15 +10465,15 @@
     let mh = L.Data.Engine.StiDataSortDirection,
         ch = L.Data.Engine.StiDataSortVariation,
         dh = L.Data.Engine.StiDataTopNMode,
         gh = F.u.StiIndicatorIteration;
     {
         class Ch extends F.i.StiElementBuilder {
             async render(l, a) {
-                this.storedCulture = ai.set(l.report);
+                this.storedCulture = oi.set(l.report);
                 try {
                     let t = this.getValueMeterIndex(a),
                         r = this.getTargetMeterIndex(a),
                         i = this.getSeriesMeterIndex(a),
                         e = this.getSeriesKeys(a, i, this.getSeriesKeysLimitCount(l)),
                         s = e.count2(),
                         n = e.select(e => new gh(this.getSeries(a, i, e, l.report), this.getValue(a, t, i, s, e), this.getNullableValue(a, r, i, s, e)));
@@ -10486,25 +10496,25 @@
                         i = B.isNullOrEmpty(s.topN.othersText) ? b.get("FormDesigner", "Others") : await O.parseAsync(s.topN.othersText, s);
                     l.add(new gh(i, e, r))
                 }
                 return l
             }
             getValueMeterIndex(e) {
                 if (null == e) return -1;
-                let t = e.meters.firstOrDefault(e => e.is(Is));
+                let t = e.meters.firstOrDefault(e => e.is(Ds));
                 return null != t ? e.meters.indexOf(t) : -1
             }
             getTargetMeterIndex(e) {
                 if (null == e) return -1;
-                let t = e.meters.firstOrDefault(e => e.is(Ds));
+                let t = e.meters.firstOrDefault(e => e.is(Rs));
                 return null != t ? e.meters.indexOf(t) : -1
             }
             getSeriesMeterIndex(e) {
                 if (null == e) return -1;
-                let t = e.meters.firstOrDefault(e => e.is(As));
+                let t = e.meters.firstOrDefault(e => e.is(Is));
                 return null != t ? e.meters.indexOf(t) : -1
             }
         }
         F.i.StiIndicatorElementBuilder = Ch
     }
     let ph = L.Report.Components.TextFormats.StiNegativeColorChecker,
         Sh = L.System.Drawing.GraphicsUnit,
@@ -10536,15 +10546,15 @@
                     },
                     l = {
                         ref: o
                     },
                     u = {
                         ref: s
                     },
-                    h = ts.format(this.element.report, this.element.textFormat, this.iterations[0].value),
+                    h = rs.format(this.element.report, this.element.textFormat, this.iterations[0].value),
                     m = (this.getRectanglesSingleMode(a, h, e, n, l, u), i = n.ref, o = l.ref, s = u.ref, this.processFontName(this.element.font.fontFamily.name, this.iterations[0])),
                     c = this.processFontStyle(this.element.font, this.iterations[0]),
                     d = new H(m, 8, c),
                     g = this.processBackColor(this.iterations[0]),
                     p = this.processForeColor(this.iterations[0]),
                     S = this.processGlyphColor(this.iterations[0]),
                     w = this.processIcon(this.element.icon, this.iterations[0]),
@@ -10556,15 +10566,15 @@
                 }
                 let y = p;
                 if (this.iterations[0].value < 0 && ph.isNegativeInRed(this.element.textFormat) && (y = Z.Engine.negativeColor), this.drawTextIcon(a, h, d, za.getContent(w), y, S, i, b, f), r) {
                     let e = this.getVariation(this.iterations[0]),
                         t = J.getIndicatorStyle(this.element),
                         r = 0 <= e ? t.positiveColor : t.negativeColor,
                         i = (r = this.processTargetIconColor(r, this.iterations[0]), 0 <= e ? kt.ArrowUp : kt.ArrowDown),
-                        s = (i = this.processTargetIcon(i, this.iterations[0]), ts.formatAsPercentage2(this.element.report, this.element.targetFormat, e)),
+                        s = (i = this.processTargetIcon(i, this.iterations[0]), rs.formatAsPercentage2(this.element.report, this.element.targetFormat, e)),
                         n = 0 == e ? Ht.None : Ht.Right,
                         l = this.processTargetIconAlignment(n, this.iterations[0]);
                     this.drawTextIcon(a, s, d, za.getContent(i), r, r, o, l, null)
                 }
                 let C = null,
                     x = {
                         ref: C
@@ -10612,16 +10622,16 @@
                 !o && a ? (this.element.fontSizeMode == _a.Value ? (u = this.getFactorByFontSize(e, t, this.element, r), h = 1 - u) : this.element.fontSizeMode == _a.Target && (h = this.getFactorByFontSize(e, t, this.element, r), u = 1 - h), m = 0) : o && !a ? (h = 0, m = 1 - u) : o || a || (this.element.fontSizeMode != _a.Value ? u = 1 : (u = this.getFactorByFontSize(e, t, this.element, r), c = r.y + (r.height - r.height * u) / 2), h = 0, m = 0), i.ref = new j(r.x, c, r.width, r.height * u), s.ref = new j(i.ref.x, i.ref.bottom, r.width, r.height * h), n.ref = new j(i.ref.x, s.ref.bottom, r.width, r.height * m)
             }
             processFontStyle(e, t) {
                 let r = this.processFontBold(e.bold, t),
                     i = this.processFontItalic(e.italic, t),
                     s = this.processFontUnderline(e.underline, t),
                     n = this.processFontStrikeout(e.strikeout, t),
-                    l = hn.Regular;
-                return r && (l ^= hn.Bold), i && (l ^= hn.Italic), s && (l ^= hn.Underline), n && (l ^= hn.Strikeout), l
+                    l = mn.Regular;
+                return r && (l ^= mn.Bold), i && (l ^= mn.Italic), s && (l ^= mn.Underline), n && (l ^= mn.Strikeout), l
             }
             processFontStrikeout(e, t) {
                 for (let e of this.element.indicatorConditions)
                     if (0 < (e.permissions & to.FontStyleStrikeout) && this.getConditionResult(t, e)) return e.font.strikeout;
                 return e
             }
             processFontUnderline(e, t) {
@@ -10700,15 +10710,15 @@
                         break;
                     case eo.Target:
                         s = i.target;
                         break;
                     case eo.Variation: {
                         let e = this.getVariation(i),
                             t = new Ur,
-                            r = (t.decimalDigits = 3, ts.formatAsPercentage2(this.element.report, t, e));
+                            r = (t.decimalDigits = 3, rs.formatAsPercentage2(this.element.report, t, e));
                         s = r.replace("%", "")[L.System.StiObject.stimulsoft]().toNumber();
                         break
                     }
                 }
                 let e = !1,
                     r = this.getConditionValue(t);
                 if (null != s) {
@@ -10792,15 +10802,15 @@
                 } else
                     for (let r of this.element.iconRanges) {
                         let e = V.tryToNumber(await O.parseAsync(r.startExpression, this.element)),
                             t = V.tryToNumber(await O.parseAsync(r.endExpression, this.element));
                         this.element.iconRangeMode == Ga.Percentage && (e = s + e / 100 * n, t = s + t / 100 * n), a.add(new F.u.StiIndicatorIconRangeValue(e, t, r.icon))
                     }
                 for (let t of this.iterations) {
-                    p.add(t.series), S.add(ts.format(this.element.report, this.element.textFormat, t.value));
+                    p.add(t.series), S.add(rs.format(this.element.report, this.element.textFormat, t.value));
                     let e = a.where(e => e.isBetween(t.value)).firstOrDefault();
                     null != e ? w.add(e.icon) : w.add(null)
                 }
                 let b = this.element.font,
                     o = null,
                     u = new H(b.fontFamily.name, 1, b.style, b.unit);
                 for (let i = 0; i < this.iterations.length; i++) {
@@ -10859,16 +10869,16 @@
                     x = (C < this.minSide && (C = this.minSide), new P),
                     M = new P,
                     T = new P,
                     F = new P,
                     v = new P;
                 for (let s = 0; s < this.iterations.length; s++) {
                     let e = this.iterations[s],
-                        t = (x.add(e.series), M.add(ts.format(this.element.report, this.element.textFormat, e.value)), this.getVariation(this.iterations[s])),
-                        r = ts.formatAsPercentage2(this.element.report, this.element.targetFormat, t),
+                        t = (x.add(e.series), M.add(rs.format(this.element.report, this.element.textFormat, e.value)), this.getVariation(this.iterations[s])),
+                        r = rs.formatAsPercentage2(this.element.report, this.element.targetFormat, t),
                         i = 0 <= t ? kt.ArrowUp : kt.ArrowDown;
                     T.add(r), F.add(i), v.add(0 == t ? Ht.None : Ht.Right)
                 }
                 let s = null,
                     A = this.element.font,
                     n = new H(A.fontFamily.name, 1, A.style, A.unit);
                 for (let i = 0; i < this.iterations.length; i++) {
@@ -10994,15 +11004,15 @@
                 if (null != y && 0 < y && w != Ht.None)
                     if (null == e || 0 == e.length) {
                         let e = new Nu("Stimulsoft", .6 * y, L.System.Drawing.FontStyle.Regular, L.System.Drawing.GraphicsUnit.Point);
                         c.drawRotatedString5(p, e, r, b, Xu.getStringFormatGeom(c), Lu.CenterCenter, 0, !0)
                     } else c.drawImage(e, b)
             }
             getFontGeom(e) {
-                return new Nu("Arial", e, hn.Bold, Sh.Point)
+                return new Nu("Arial", e, mn.Bold, Sh.Point)
             }
             measureFontSize(e, t, r, i) {
                 let s = e.measureString(r, this.getFontGeom(1e3));
                 if (0 == s.width || 0 == s.height) return void(i.ref = 0);
                 let n = t.width / s.width * 1e3,
                     l = t.height / s.height * 1e3,
                     a = l < n ? l : n;
@@ -11155,15 +11165,15 @@
                         let t = this.getColors(r.length);
                         i = new xo;
                         for (let e = 0; e < r.length; e++) i.set(r[e], t[e])
                     }
                     let t = new P;
                     if (0 <= p)
                         for (let e = 0; e < Math.min(d.rows.length, this.MAX_LOCATIONS); e++) t.add(V.tryToNumber(d.rows[e][p]));
-                    Ln.sort(t);
+                    Bn.sort(t);
                     let h = t,
                         m = new Object,
                         c = 0;
                     while (c < d.rows.length && c < this.MAX_LOCATIONS) {
                         let a = d.rows[c][s];
                         if (null == a) {
                             c++;
@@ -11280,40 +11290,40 @@
                     }
                     i = !i
                 }
                 return t
             }
             static getLongitudeMeterIndex(e) {
                 if (null == e) return -1;
-                let t = e.meters.firstOrDefault(e => e.is(Ss));
+                let t = e.meters.firstOrDefault(e => e.is(ws));
                 return null != t ? e.meters.indexOf(t) : -1
             }
             static getLatitudeMeterIndex(e) {
                 if (null == e) return -1;
-                let t = e.meters.firstOrDefault(e => e.is(ps));
+                let t = e.meters.firstOrDefault(e => e.is(Ss));
                 return null != t ? e.meters.indexOf(t) : -1
             }
             static getLocationMeterIndex(e) {
                 if (null == e) return -1;
-                let t = e.meters.firstOrDefault(e => e.is(Wi));
+                let t = e.meters.firstOrDefault(e => e.is(Ji));
                 return null != t ? e.meters.indexOf(t) : -1
             }
             static getLocationColorMeterIndex(e) {
                 if (null == e) return -1;
-                let t = e.meters.firstOrDefault(e => e.is(Ji));
+                let t = e.meters.firstOrDefault(e => e.is(Ui));
                 return null != t ? e.meters.indexOf(t) : -1
             }
             static getLocationArgumentMeterIndex(e) {
                 if (null == e) return -1;
-                let t = e.meters.firstOrDefault(e => e.is(Xi));
+                let t = e.meters.firstOrDefault(e => e.is(Wi));
                 return null != t ? e.meters.indexOf(t) : -1
             }
             static getLocationValueMeterIndex(e) {
                 if (null == e) return -1;
-                let t = e.meters.firstOrDefault(e => e.is(Ui));
+                let t = e.meters.firstOrDefault(e => e.is(Zi));
                 return null != t ? e.meters.indexOf(t) : -1
             }
             static parseColor(t) {
                 let s = N.black;
                 try {
                     if (1 < t.length) {
                         if ("#" == t[0]) {
@@ -11615,17 +11625,17 @@
                     b["color"] = `rgba(${e.r}, ${e.g}, ${e.b}, ${e.a})`
                 }
                 if (w != Io.None) {
                     if (0 < (w & Io.BackColor)) {
                         let e = s.field.conditionBrush.color;
                         b["backgroundColor"] = `rgba(${e.r}, ${e.g}, ${e.b}, ${e.a})`
                     }
-                    0 < (w & Io.Font) && (b["fontFamily"] = s.field.font.name), 0 < (w & Io.FontSize) && (b["fontSize"] = s.field.font.sizeInPoints + `pt`), 0 < (w & Io.FontStyleBold) && (b["fontWeight"] = 0 < (s.field.font.style & hn.Bold) ? "bold" : "normal"), 0 < (w & Io.FontStyleItalic) && (b["fontStyle"] = 0 < (s.field.font.style & hn.Italic) ? "italic " : "normal");
+                    0 < (w & Io.Font) && (b["fontFamily"] = s.field.font.name), 0 < (w & Io.FontSize) && (b["fontSize"] = s.field.font.sizeInPoints + `pt`), 0 < (w & Io.FontStyleBold) && (b["fontWeight"] = 0 < (s.field.font.style & mn.Bold) ? "bold" : "normal"), 0 < (w & Io.FontStyleItalic) && (b["fontStyle"] = 0 < (s.field.font.style & mn.Italic) ? "italic " : "normal");
                     let e = "";
-                    if (0 < (w & Io.FontStyleStrikeout) && 0 < (s.field.font.style & hn.Strikeout) && (e += "line-through "), 0 < (w & Io.FontStyleUnderline) && 0 < (s.field.font.style & hn.Underline) && (e += "underline"), B.isNullOrEmpty(e) || (b["textDecoration"] = e), 0 < (w & Io.TextColor)) {
+                    if (0 < (w & Io.FontStyleStrikeout) && 0 < (s.field.font.style & mn.Strikeout) && (e += "line-through "), 0 < (w & Io.FontStyleUnderline) && 0 < (s.field.font.style & mn.Underline) && (e += "underline"), B.isNullOrEmpty(e) || (b["textDecoration"] = e), 0 < (w & Io.TextColor)) {
                         let e = s.field.conditionTextBrush.color;
                         b["color"] = `rgba(${e.r}, ${e.g}, ${e.b}, ${e.a})`
                     }
                 }
                 if (null != s.field) switch (s.field.horAlignment) {
                     case X.Left:
                         b["text-align"] = "left";
@@ -11648,15 +11658,15 @@
                     a = e.columns.length + (0 < e.rows.length ? 1 : 0) + (1 < e.summaries.length && e.summaryDirection == Mo.LeftToRight ? 1 : 0),
                     o = (0 == e.rows.length ? 1 : e.rows.length) + (1 < e.summaries.length && e.summaryDirection == Mo.UpToDown ? 1 : 0);
                 for (let i = 0; i < l.length; i++)
                     for (let r = 0; r < l[i].length; r++)
                         if (null != l[i][r].field) {
                             let e = l[i][r],
                                 t = !(e.isCrossSummary || e.field.is2(Zh) || (e.field.is2(Gh) || e.field.is2(Uh)) && null == e.guid);
-                            s ? (e.field.font = new H("Arial", 10, t ? hn.Bold : hn.Regular), e.field.brush = new v(N.transparent), e.field.textBrush = new v(N.black)) : t ? (i < o && r >= a ? e.field.brush = null != e.field.conditionBrush ? e.field.conditionBrush : new v(n.rowHeaderBackColor) : e.field.brush = null != e.field.conditionBrush ? e.field.conditionBrush : new v(n.columnHeaderBackColor), e.field.textBrush = null != e.field.conditionTextBrush ? e.field.conditionTextBrush : new v(n.columnHeaderForeColor)) : (e.field.brush = null != e.field.conditionBrush ? e.field.conditionBrush : new v(r % 2 != 0 ? n.alternatingCellBackColor : n.cellBackColor), e.field.textBrush = null != e.field.conditionTextBrush ? e.field.conditionTextBrush : new v(r % 2 != 0 ? n.alternatingCellForeColor : n.cellForeColor)), e.field.border.color = n.lineColor
+                            s ? (e.field.font = new H("Arial", 10, t ? mn.Bold : mn.Regular), e.field.brush = new v(N.transparent), e.field.textBrush = new v(N.black)) : t ? (i < o && r >= a ? e.field.brush = null != e.field.conditionBrush ? e.field.conditionBrush : new v(n.rowHeaderBackColor) : e.field.brush = null != e.field.conditionBrush ? e.field.conditionBrush : new v(n.columnHeaderBackColor), e.field.textBrush = null != e.field.conditionTextBrush ? e.field.conditionTextBrush : new v(n.columnHeaderForeColor)) : (e.field.brush = null != e.field.conditionBrush ? e.field.conditionBrush : new v(r % 2 != 0 ? n.alternatingCellBackColor : n.cellBackColor), e.field.textBrush = null != e.field.conditionTextBrush ? e.field.conditionTextBrush : new v(r % 2 != 0 ? n.alternatingCellForeColor : n.cellForeColor)), e.field.border.color = n.lineColor
                         }
             }
             static buildCross(l, n, t) {
                 let a = new xo;
                 for (let e = 0; e < n.meters.length; e++) a.set(n.meters[e].expression, e);
                 l.crossTabInfo.startRow = 0, l.crossTabInfo.startCol = 0;
                 let u = new Jh(null),
@@ -11733,48 +11743,48 @@
                     } for (let s of n.rows) {
                     let i = b.newRow();
                     for (let r of l.components.list) {
                         if (r.is(em)) continue;
                         let t = r.as(sm);
                         if (null != t) {
                             let e = a.contains(r.alias) ? s[a.get(r.alias)] : null;
-                            if ("number" == typeof(e = Ln.isArray(e) ? new P(e).firstOrDefault() : e) && (e = e[L.System.StiObject.stimulsoft]().toNumber()), i.sett(t.name, e), t.is(rm) && i.sett("Display__" + r.name, s[a.get(r.alias)]), t.is(Zh))
+                            if ("number" == typeof(e = Bn.isArray(e) ? new P(e).firstOrDefault() : e) && (e = e[L.System.StiObject.stimulsoft]().toNumber()), i.sett(t.name, e), t.is(rm) && i.sett("Display__" + r.name, s[a.get(r.alias)]), t.is(Zh))
                                 for (let e of t.arguments) i.sett(e.key, a.contains(e.value) ? s[a.get(e.value)] : null)
                         } else if (r.is(Wh) && !B.isNullOrEmpty(r.alias)) {
                             let e = s[a.get(r.alias)];
                             r.setTextInternal(e.toString())
                         }
                     }
                     b.rows.add(i), l.next()
                 }
                 let f = new nm,
                     r = (l.crossTabInfo.cross = f, l.crossTabInfo.cross.designTime = !1, l.crossTabInfo.cross.colFields = u, l.crossTabInfo.cross.rowFields = h, l.crossTabInfo.cross.sumFields = m, l.crossTabInfo.cross.sumHeaderFields = c, l.crossTabInfo.cross.colTitleFields = g, l.crossTabInfo.cross.rowTitleFields = d, l.crossTabInfo.cross.leftCrossTitle = p, l.crossTabInfo.cross.rightCrossTitle = S, l.crossTabInfo.cross.summaryCrossTitle = w, (l.crossTabInfo.cross.crossTab = l).dataSourceName = "pivot", new Ah("pivot", "pivot"));
                 r.dictionary = l.report.dictionary;
-                for (let e of b.columns.list) r.columns.add(new oi(e.columnName, e.columnName, e.columnName));
+                for (let e of b.columns.list) r.columns.add(new ui(e.columnName, e.columnName, e.columnName));
                 r.dataTable = b, l.report.dictionary.dataSources.add(r), l.summaryDirection = 1 < (null == o ? void 0 : o.length) ? t.summaryDirection : Mo.UpToDown, l.crossTabInfo.cross.create(b, l.report, l.summaryDirection, l.emptyValue), l.crossTabInfo.cross.crossTab = null;
                 let y = J.getPivotTableStyle(t),
                     e = 0 == s.length && 0 == i.length && 0 < o.length;
                 if (e) {
                     f.init(2, o.length);
                     for (let i = 0; i < o.length; i++) {
                         let e = o[i],
                             t = new Qh,
-                            r = (t.alias = e.expression, t.name = "CrossTab_Sum" + i.toString(), t.page = l.page, t.horAlignment = X.Center, t.textFormat = e.textFormat.clone(), t.guid = tm.newGuidString(), t.font = U.Table.Font.getCachedGdiFont(), t.brush = new v(y.cellBackColor), t.hideZeros = e.hideZeros, t.border = new ie(i == o.length - 1 ? G.Right | G.Top : 0 == i ? G.Right | G.Bottom : G.Right | G.Bottom | G.Top, y.lineColor, 1, Ri.Solid), t.height = U.Table.getHeight(t.font), f.cells[0][i] = new Kh, f.cells[0][i].text = this.getLabel(e), f.cells[0][i].field = t, f.cells[0][i].parentCell = f.cells[0][i], new Zh);
-                        r.name = "CrossTab_Sum" + i.toString(), r.value = 0 < n.rows.length ? n.rows[0][i].toString() : "", r.page = l.page, r.horAlignment = X.Right, r.textFormat = e.textFormat.clone(), r.guid = tm.newGuidString(), r.font = U.Table.Font.getCachedGdiFont(), r.border = new ie(G.None, y.lineColor, 1, Ri.Solid), r.height = U.Table.getHeight(r.font), f.cells[1][i] = new Kh, f.cells[1][i].field = r, f.cells[1][i].text = 0 < n.rows.length ? n.rows[0][i].toString() : "", f.cells[1][i].parentCell = f.cells[1][i]
+                            r = (t.alias = e.expression, t.name = "CrossTab_Sum" + i.toString(), t.page = l.page, t.horAlignment = X.Center, t.textFormat = e.textFormat.clone(), t.guid = tm.newGuidString(), t.font = U.Table.Font.getCachedGdiFont(), t.brush = new v(y.cellBackColor), t.hideZeros = e.hideZeros, t.border = new ie(i == o.length - 1 ? G.Right | G.Top : 0 == i ? G.Right | G.Bottom : G.Right | G.Bottom | G.Top, y.lineColor, 1, Ei.Solid), t.height = U.Table.getHeight(t.font), f.cells[0][i] = new Kh, f.cells[0][i].text = this.getLabel(e), f.cells[0][i].field = t, f.cells[0][i].parentCell = f.cells[0][i], new Zh);
+                        r.name = "CrossTab_Sum" + i.toString(), r.value = 0 < n.rows.length ? n.rows[0][i].toString() : "", r.page = l.page, r.horAlignment = X.Right, r.textFormat = e.textFormat.clone(), r.guid = tm.newGuidString(), r.font = U.Table.Font.getCachedGdiFont(), r.border = new ie(G.None, y.lineColor, 1, Ei.Solid), r.height = U.Table.getHeight(r.font), f.cells[1][i] = new Kh, f.cells[1][i].field = r, f.cells[1][i].text = 0 < n.rows.length ? n.rows[0][i].toString() : "", f.cells[1][i].parentCell = f.cells[1][i]
                     }
                 }
                 if (l.rightToLeft && lm.makeRightToLeft(l), l.crossTabInfo.cross.doAutoSize(), !e) {
                     for (let t = 0; t < f.cells.length; t++)
                         for (let e = 0; e < f.cells[t].length; e++) null != f.cells[t][e].field && (f.cells[t][e].field.margins = f.cells[t][e].field.margins.clone(), 0 == t && (f.cells[t][e].field.border.side = f.cells[t][e].field.border.side & ~G.Left), 0 == e && (f.cells[t][e].field.border.side = f.cells[t][e].field.border.side & ~G.Top), t == f.cells.length - 1 && (f.cells[t][e].field.border.side = f.cells[t][e].field.border.side & ~G.Right), e == f.cells[t].length - 1) && (f.cells[t][e].field.border.side = f.cells[t][e].field.border.side & ~G.Bottom);
                     let e = i.length + (0 < s.length ? 1 : 0),
                         r = (0 == s.length ? 1 : s.length) + (1 < o.length ? 1 : 0);
                     for (let t = e; t < f.cells[0].length; t++)
                         for (let e = r; e < f.cells.length; e++) null != f.cells[e][t].field && (f.cells[e][t].field.border.side = G.Left | G.Right);
                     if (1 < f.sumFields.count)
-                        for (let e = 0; e < f.cells[0].length; e++) null != f.cells[r - 1][e].field && (f.cells[r - 1][e].field.border = new ie(G.All, y.lineColor, 1, Ri.Solid));
+                        for (let e = 0; e < f.cells[0].length; e++) null != f.cells[r - 1][e].field && (f.cells[r - 1][e].field.border = new ie(G.All, y.lineColor, 1, Ei.Solid));
                     null != f.cells[0][0].field && (f.cells[0][0].field.border.side = G.Right | G.Bottom)
                 }
                 l.report.dictionary.dataSources.remove(r)
             }
             static async convertToCrossTab(e, t) {
                 let r = new _h,
                     i = (r.info.zoom = 1, r.reportUnit = null != e && null != e.report ? e.report.reportUnit : qh.HundredthsOfInch, new Lh(r)),
@@ -11810,15 +11820,15 @@
                     let e = new Qh,
                         t = (e.showTotal = r.showTotal, e.alias = r.expression, e.displayValue = "{" + r.expression + "}", e.value = e.displayValue, e.page = null, e.name = c.name + "_Column" + (f + 1).toString(), e.page = c.page, e.horAlignment = ve.parse(X, ve.getName(z, r.horAlignment)), e.guid = tm.newGuidString(), e.wordWrap = r.size.wordWrap, e.margins = new be(this.FieldMargin), e.sortDirection = r.sortDirection, e.expandExpression = r.expandExpression, 0 < r.size.minWidth && (e.minSize = new W(c.report.unit.convertFromHInches(r.size.minWidth), 0)), 0 < r.size.maxWidth && (e.maxSize = new W(c.report.unit.convertFromHInches(r.size.maxWidth), 0)), 0 < r.size.width && (e.maxSize = new W(c.report.unit.convertFromHInches(r.size.width), 0), e.minSize = new W(c.report.unit.convertFromHInches(r.size.width), 0)), await this.getCondition(i, r, e), await this.setTopN(e, r.topN, i), B.isNullOrEmpty(a) && 0 < r.expression.length && 0 <= r.expression.indexOf(".") && (a = r.expression.substring(0, r.expression.indexOf("."))), e.textFormat = r.textFormat.clone(), this.setupTitle(e, g), u.add(r, e), c.components.contains(e) && c.components.remove(e), c.components.add(e), d.set(e, e), m.add(e), e.total);
                     null == t && (t = this.createColTotal(i, e, s, l, g), B.isNullOrWhiteSpace(r.totalLabel) || (t.text = r.totalLabel), e.totalGuid = t.guid, c.components.add(t)), d.set(t, t), l.add(t), f++
                 }
                 let y = 1;
                 for (let t of w) {
                     let e = new Zh;
-                    e.alias = t.expression, this.setSummaryType(e, t.expression), e.page = null, e.name = c.name + "_Sum" + y.toString(), e.page = c.page, e.horAlignment = ve.parse(X, ve.getName(z, t.horAlignment)), e.textFormat = t.textFormat.clone(), e.guid = tm.newGuidString(), await this.getCondition(i, t, e), e.font = U.Table.Font.getCachedGdiFont(), e.border = new ie(G.All, g.lineColor, 1, Ri.Solid), e.height = U.Table.getHeight(e.font), e.hideZeros = t.hideZeros, 0 < t.size.minWidth && (e.minSize = new W(c.report.unit.convertFromHInches(t.size.minWidth), 0)), 0 < t.size.maxWidth && (e.maxSize = new W(c.report.unit.convertFromHInches(t.size.maxWidth), 0)), 0 < t.size.width && (e.maxSize = new W(c.report.unit.convertFromHInches(t.size.width), 0), e.minSize = new W(c.report.unit.convertFromHInches(t.size.width), 0)), d.set(e, e), c.components.contains(e) && c.components.remove(e), c.components.add(e), y++
+                    e.alias = t.expression, this.setSummaryType(e, t.expression), e.page = null, e.name = c.name + "_Sum" + y.toString(), e.page = c.page, e.horAlignment = ve.parse(X, ve.getName(z, t.horAlignment)), e.textFormat = t.textFormat.clone(), e.guid = tm.newGuidString(), await this.getCondition(i, t, e), e.font = U.Table.Font.getCachedGdiFont(), e.border = new ie(G.All, g.lineColor, 1, Ei.Solid), e.height = U.Table.getHeight(e.font), e.hideZeros = t.hideZeros, 0 < t.size.minWidth && (e.minSize = new W(c.report.unit.convertFromHInches(t.size.minWidth), 0)), 0 < t.size.maxWidth && (e.maxSize = new W(c.report.unit.convertFromHInches(t.size.maxWidth), 0)), 0 < t.size.width && (e.maxSize = new W(c.report.unit.convertFromHInches(t.size.width), 0), e.minSize = new W(c.report.unit.convertFromHInches(t.size.width), 0)), d.set(e, e), c.components.contains(e) && c.components.remove(e), c.components.add(e), y++
                 }
                 if (w.length < 2) {
                     for (let e of r) c.components.contains(e) && c.components.remove(e);
                     r.clear()
                 } else if (r.length > w.length)
                     while (r.length > w.length) {
                         let e = r[r.length - 1];
@@ -11938,15 +11948,15 @@
                             let e = [];
                             u.report.engine.parserConversionStore.set("*StiConditionExpression*" + u.name, e)
                         }
                         u.report.engine.parserConversionStore.get("*StiConditionExpression*" + u.name).push(n), u.conditions.add(e)
                     }
             }
             static setupTitle(e, t) {
-                e.border = new ie(G.All, t.lineColor, 1, Ri.Solid), e.font = U.Table.Font.getCachedGdiFont(), e.height = U.Table.getHeight(e.font)
+                e.border = new ie(G.All, t.lineColor, 1, Ei.Solid), e.font = U.Table.Font.getCachedGdiFont(), e.height = U.Table.getHeight(e.font)
             }
             static setupField(e) {
                 e.margins.left = 0, e.margins.right = 0, e.guid = tm.newGuidString()
             }
             static createRowTotal(e, t, r, i) {
                 let s = t.guid,
                     n = r.get(s);
@@ -11999,15 +12009,15 @@
             this.series = e, this.value = t, this.target = r
         }
     };
     let am = F.v.StiProgressIteration;
     {
         class om extends F.i.StiElementBuilder {
             async render(l, a) {
-                this.storedCulture = ai.set(l.report);
+                this.storedCulture = oi.set(l.report);
                 try {
                     let t = this.getValueMeterIndex(a),
                         r = this.getTargetMeterIndex(a),
                         i = this.getSeriesMeterIndex(a),
                         e = this.getSeriesKeys(a, i),
                         s = e.count2(),
                         n = e.select(e => new am(this.getSeries(a, i, e, l.report), this.getValue(a, t, i, s, e), this.getNullableValue(a, r, i, s, e)));
@@ -12030,25 +12040,25 @@
                         i = B.isNullOrEmpty(s.topN.othersText) ? b.get("FormDesigner", "Others") : await O.parseAsync(s.topN.othersText, s);
                     l.add(new am(i, e, r))
                 }
                 return l
             }
             getValueMeterIndex(e) {
                 if (null == e) return -1;
-                let t = e.meters.firstOrDefault(e => e.is(us));
+                let t = e.meters.firstOrDefault(e => e.is(hs));
                 return null != t ? e.meters.indexOf(t) : -1
             }
             getTargetMeterIndex(e) {
                 if (null == e) return -1;
-                let t = e.meters.firstOrDefault(e => e.is(hs));
+                let t = e.meters.firstOrDefault(e => e.is(ms));
                 return null != t ? e.meters.indexOf(t) : -1
             }
             getSeriesMeterIndex(e) {
                 if (null == e) return -1;
-                let t = e.meters.firstOrDefault(e => e.is(ms));
+                let t = e.meters.firstOrDefault(e => e.is(cs));
                 return null != t ? e.meters.indexOf(t) : -1
             }
         }
         F.i.StiProgressElementBuilder = om
     }
     F.w.StiProgressVisualCreator = class {
         static createProgressVisual(e, t) {
@@ -12121,25 +12131,25 @@
             let t = F.h.StiMeterHelper.toDataType(e);
             if (Le.isNumericType(t)) return z.Right;
             if (Le.isDateType(t)) return z.Center;
             return z.Left
         }
     }, F.h.StiTableElementHelper = class {
         static minDataColumnValue(e, t, r) {
-            if (!(e.is2(_i) || e.is2(qi) || e.is2(Gi))) return 0;
+            if (!(e.is2($i) || e.is2(_i) || e.is2(Xi))) return 0;
             return t.rows.any() ? t.rows.min(e => V.tryToNumber(e[r])) : 0
         }
         static maxDataColumnValue(e, t, r) {
-            if (!(e.is2(_i) || e.is2(qi) || e.is2(Gi))) return 0;
+            if (!(e.is2($i) || e.is2(_i) || e.is2(Xi))) return 0;
             return t.rows.any() ? t.rows.max(e => V.tryToNumber(e[r])) : 0
         }
         static calculateTotal(e, r, i) {
             switch (e.summaryType) {
                 case Kr.Sum:
-                    if (Rs.isPercentOfGrandTotal(e.expression)) return 1;
+                    if (Es.isPercentOfGrandTotal(e.expression)) return 1;
                     return i.rows.any() ? i.rows.sum(e => r < e.length ? V.tryToNumber(e[r]) : 0) : 0;
                 case Kr.Count:
                     return i.rows.any() ? i.rows.count2(e => r < e.length && null != e[r]) : 0;
                 case Kr.Min:
                     return i.rows.any() ? i.rows.min(e => r < e.length ? V.tryToNumber(e[r]) : 0) : 0;
                 case Kr.Max:
                     return i.rows.any() ? i.rows.max(e => r < e.length ? V.tryToNumber(e[r]) : 0) : 0;
@@ -12361,15 +12371,15 @@
         fc = L.Report.Chart.IStiScatterArea,
         yc = L.Base.Helpers.StiValueComparer,
         Cc = L.Report.Chart.IStiShowNullsSeriesAs,
         xc = L.Report.Chart.IStiShowZerosSeriesAs;
     {
         class S extends F.i.StiElementBuilder {
             async render(r, i) {
-                this.storedCulture = ai.set(r.report);
+                this.storedCulture = oi.set(r.report);
                 try {
                     let e = new L.Report.Components["StiChart"];
                     if (e.horSpacing = r.area.horSpacing, e.vertSpacing = r.area.vertSpacing, e.isDashboard = !0, e.page = r.page, e.previousAnimations = r.previousAnimations, e.sortAnimation = r.sortAnimation, r.sortAnimation = !1, S.setStyle(r, e), e.series.clear(), null == i) return e;
                     await this.renderElements(r, e, i), await this.renderArea(r, e), await this.renderLegend(r, e), await this.renderSeriesLabels(r, e), await S.renderConstantLines(r, e), this.simplifyValues(e), e.applyStyle(), e.allowApplyStyle = !1;
                     let t = jl.getBackColor(r, r.backColor);
                     return N.transparent.equals(t) || (e.brush = new v(t)), e
                 } finally {
@@ -12405,26 +12415,26 @@
                             null != t && t[L.System.StiObject.stimulsoft]().is(w) && (s.core.isDateTimeValues = !0), s.values[n] = e.getArrayItem(i).firstOrDefaultAsNullableNumber(), n++
                         }
                         s.originalArguments = c[L.System.StiObject.stimulsoft]().toArray(), s.arguments = this.proccessSelectArguments(c, o, s, m);
                         let r = s.as(hc);
                         if (null != r) {
                             let e = s.values,
                                 t = s.arguments;
-                            Ln.sort3(e, t), Ln.reverse(e), Ln.reverse(t), r.values = e, r.arguments = t
+                            Bn.sort3(e, t), Bn.reverse(e), Bn.reverse(t), r.values = e, r.arguments = t
                         } else if (s.is(rc)) {
                             let r = new P,
                                 i = new P;
                             for (let t = 0; t < s.values.length; t++) {
                                 let e = s.values[t];
                                 if (!(0 < e)) continue;
                                 r.add(e), null != s.arguments && t < s.arguments.length ? i.add(s.arguments[t]) : i.add(t + 1)
                             }
                             let e = r[L.System.StiObject.stimulsoft]().toArray(),
                                 t = i[L.System.StiObject.stimulsoft]().toArray();
-                            Ln.sort3(e, t), Ln.reverse(e), Ln.reverse(t), s.valuesStart = null, s.values = e, s.arguments = t
+                            Bn.sort3(e, t), Bn.reverse(e), Bn.reverse(t), s.valuesStart = null, s.values = e, s.arguments = t
                         }
                         t++, await S.processTopNElements(o, s), L.Report.Chart["StiHistogramHelper"].checkValuesAndArguments(s, o.argumentFormat), await this.renderSeriesInteraction(s, o, c.length, this.toString(a))
                     }
                 }
                 mc.checkArgument(u), pc.checkWaterfallTotals(u)
             }
             proccessSelectArguments(e, t, s, r) {
@@ -12482,18 +12492,18 @@
             renderSeries(e, t, r, i) {
                 let s = t,
                     n = Pn.neww2(t.seriesType);
                 return S.renderSeriesYAxis(e, s, n), S.renderSeriesLine(s, n), S.renderSeriesShowZeros(s, n), S.renderSeriesShowNulls(s, n), n.coreTitle = this.getSeriesTitle(e, r, t), n.core.seriesColors = null != e.seriesColors && 0 < e.seriesColors.length ? e.seriesColors : null, n.isDashboard = !0, this.renderSeriesNegativeColor(e, n, i.series.count), this.renderSeriesParetoColor(e, n, i.series.count), this.renderMarker(e, n), S.renderSeriesLighting(n), S.renderSeriesIcon(e, n), S.renderSeriesPie3d(e, n), n.is(Vm) && (n.columnShape = e.columnShape), i.series.add(n), n
             }
             static renderSeriesPie3d(e, t) {
                 var r;
-                t.is(Lm) && null != (r = e.options3D) && r[L.System.StiObject.stimulsoft]().is(On) && (t.options3D = e.options3D[L.System.StiObject.stimulsoft]().as(On))
+                t.is(Lm) && null != (r = e.options3D) && r[L.System.StiObject.stimulsoft]().is(Vn) && (t.options3D = e.options3D[L.System.StiObject.stimulsoft]().as(Vn))
             }
             static renderSeriesYAxis(e, t, r) {
-                t.is(Bs) && 1 < e.values.length && (r.yAxis = t.yAxis)
+                t.is(Ps) && 1 < e.values.length && (r.yAxis = t.yAxis)
             }
             static renderSeriesLine(r, i) {
                 if (null != r) {
                     let e = i.as(uc);
                     if (null != e) return e.lineStyle = r.lineStyle, void(e.lineWidth = r.lineWidth);
                     let t = i.as(oc);
                     null != t && (t.lineStyle = r.lineStyle, t.lineWidth = r.lineWidth)
@@ -12562,25 +12572,25 @@
             static renderInterlacingHor(e, t) {
                 e.area.interlacingHor.visible && !N.transparent.equals(e.area.interlacingHor.color) && (t.interlacingHor.interlacedBrush = new v(e.area.interlacingHor.color)), t.interlacingHor.visible = e.area.interlacingHor.visible
             }
             static renderInterlacingVert(e, t) {
                 e.area.interlacingVert.visible && !N.transparent.equals(e.area.interlacingVert.color) && (t.interlacingVert.interlacedBrush = new v(e.area.interlacingVert.color)), t.interlacingVert.visible = e.area.interlacingVert.visible
             }
             static renderGridLinesHor(e, t) {
-                e.area.gridLinesHor.visible && !N.transparent.equals(e.area.gridLinesHor.color) && (t.gridLinesHor.color = e.area.gridLinesHor.color), t.gridLinesHor.visible = e.area.gridLinesHor.visible, t.gridLinesHor.style = Ri.Solid
+                e.area.gridLinesHor.visible && !N.transparent.equals(e.area.gridLinesHor.color) && (t.gridLinesHor.color = e.area.gridLinesHor.color), t.gridLinesHor.visible = e.area.gridLinesHor.visible, t.gridLinesHor.style = Ei.Solid
             }
             static renderGridLinesVert(e, t) {
-                e.area.gridLinesVert.visible && !N.transparent.equals(e.area.gridLinesVert.color) && (t.gridLinesVert.color = e.area.gridLinesVert.color), t.gridLinesVert.visible = e.area.gridLinesVert.visible, t.gridLinesVert.style = Ri.Solid
+                e.area.gridLinesVert.visible && !N.transparent.equals(e.area.gridLinesVert.color) && (t.gridLinesVert.color = e.area.gridLinesVert.color), t.gridLinesVert.visible = e.area.gridLinesVert.visible, t.gridLinesVert.style = Ei.Solid
             }
             async renderXAxis3D(e, t) {
                 let r = t.area.as(Nm);
                 if (null == r) return;
                 let i = r.xAxis,
                     s = e.xAxis;
-                await S.renderAxis3D(e, i, s), i.visible = s.visible, s.showEdgeValues == Tn.Auto && (i.showEdgeValues = !1)
+                await S.renderAxis3D(e, i, s), i.visible = s.visible, s.showEdgeValues == Fn.Auto && (i.showEdgeValues = !1)
             }
             async renderYAxis3D(e, t) {
                 let r = t.area.as(Nm);
                 if (null == r) return;
                 let i = r.yAxis,
                     s = e.yAxis;
                 await S.renderAxis3D(e, i, s), i.visible = s.visible, null != e.valueFormat && (i.labels.formatService = S.checkValueFormat(e.valueFormat, t))
@@ -12590,24 +12600,24 @@
                 if (null == i) return;
                 let s = r ? i.xTopAxis : i.xAxis,
                     n = r ? e.xTopAxis : e.xAxis,
                     l = t.area.is(Qm),
                     a = Hn.isDrillAvailable(e) && e.drillDownCurrentLevel < e.drillDownLevelCount ? e.arguments.getRange(e.drillDownCurrentLevel, 1) : e.arguments,
                     o = (l ? e.values : a).select(this.getTitle).distinct(),
                     u = (await S.renderAxis(e, s, n), s.ticks.visible = o.any(), s.visible = n.visible, await S.renderXAxisTitleText(e, s, n, o), t.series.toList().cast().all(e => e.is(uc) || e.is(oc))),
-                    h = (n.startFromZero == Tn.Auto && (s.startFromZero = !u), t.series.toList().cast().all(e => e.core.isDateTimeValues));
-                h && i.is(Bm) && (s.startFromZero = !1), n.showEdgeValues == Tn.Auto && (s.showEdgeValues = u), s.labels.placement == an.AutoRotation && (s.labels.textAlignment = z.Left), null != e.valueFormat && i.is(Qm) && (s.labels.formatService = S.checkValueFormat(e.valueFormat, t)), null != e.argumentFormat && i.is(fc) && (s.labels.formatService = e.argumentFormat), S.renderAxisLineColor(e, s)
+                    h = (n.startFromZero == Fn.Auto && (s.startFromZero = !u), t.series.toList().cast().all(e => e.core.isDateTimeValues));
+                h && i.is(Bm) && (s.startFromZero = !1), n.showEdgeValues == Fn.Auto && (s.showEdgeValues = u), s.labels.placement == on.AutoRotation && (s.labels.textAlignment = z.Left), null != e.valueFormat && i.is(Qm) && (s.labels.formatService = S.checkValueFormat(e.valueFormat, t)), null != e.argumentFormat && i.is(fc) && (s.labels.formatService = e.argumentFormat), S.renderAxisLineColor(e, s)
             }
             async renderYAxis(e, t, r) {
                 let i = t.area.as(ac);
                 if (null == i) return;
                 let s = r ? i.yRightAxis : i.yAxis,
                     n = r ? e.yRightAxis : e.yAxis,
                     l = t.area.is(Xm) || t.area.is(Qm),
-                    a = (l && e.dataMode != Vn.ManuallyEnteringData ? e.arguments : e.chartValuesList()).select(this.getTitle).distinct(),
+                    a = (l && e.dataMode != kn.ManuallyEnteringData ? e.arguments : e.chartValuesList()).select(this.getTitle).distinct(),
                     o = (await S.renderAxis(e, s, n), s.visible = a.any() && n.visible, await S.renderYAxisTitleText(e, s, n, a), null == e.valueFormat || i.is(Qm) || (s.labels.formatService = S.checkValueFormat(e.valueFormat, t)), t.series.toList().cast().all(e => e.core.isDateTimeValues));
                 o && (i.yAxis.startFromZero = !1), S.renderAxisLineColor(e, s)
             }
             static renderXRadarAxis(e, t) {
                 let r = t.area.as(zm);
                 if (null == r) return;
                 this.renderXRadarAxisLabels(e.area.xAxis.labels, r.xAxis.labels), this.renderAxisRange(r.xAxis.range, e.xAxis), null != e.valueFormat && (r.yAxis.labels.formatService = S.checkValueFormat(e.valueFormat, t));
@@ -12694,36 +12704,36 @@
             static async renderAxis(e, t, r) {
                 let i = J.getForeColor(e);
                 this.renderAxisTitle(e, t, r, i), await this.renderAxisLabels(e, t, r), this.renderAxisStartFromZero(t, r), this.renderAxisShowEdgeValues(t, r), this.renderAxisRange(t.range, r), this.renderAxisLabelsColor(e, t, r, i)
             }
             static renderAxisTitle(e, t, r, i) {
                 let s = this.getTitleAxisChart(r),
                     n = t.title;
-                n.alignment = s.alignment, n.position = s.position, n.font = s.font, this.renderAxisLabelsTitleColor(e, n, s, i), s.is(Km) && (n.direction = s.direction), s.is(Mn) && (n.direction = s.direction)
+                n.alignment = s.alignment, n.position = s.position, n.font = s.font, this.renderAxisLabelsTitleColor(e, n, s, i), s.is(Km) && (n.direction = s.direction), s.is(Tn) && (n.direction = s.direction)
             }
             static async renderAxisLabels3D(e, t, r) {
                 t.labels.textAfter = await O.parseAsync(r.labels.textAfter, e), t.labels.textBefore = await O.parseAsync(r.labels.textBefore, e), t.labels.font = r.labels.font
             }
             static async renderAxisLabels(e, t, r) {
                 t.labels.angle = r.labels.angle, t.is(Ym) && e.isParetoChart || (t.labels.textAfter = await O.parseAsync(r.labels.textAfter, e)), t.labels.textAlignment = r.labels.textAlignment, t.labels.textBefore = await O.parseAsync(r.labels.textBefore, e), t.labels.font = r.labels.font, t.labels.placement = r.labels.placement, t.labels.step = r.labels.step, t.labels.wordWrap = r.labels.wordWrap, t.labels.width = r.labels.width
             }
             static renderAxisStartFromZero(t, r) {
                 if (r.is(lc)) {
                     let e = r;
-                    null != e && e.startFromZero != Tn.Auto && (t.startFromZero = e.startFromZero != Tn.False)
+                    null != e && e.startFromZero != Fn.Auto && (t.startFromZero = e.startFromZero != Fn.False)
                 }
                 if (r.is(nc)) {
                     let e = r;
                     null != e && (t.startFromZero = e.startFromZero)
                 }
             }
             static renderAxisShowEdgeValues(t, r) {
                 if (r.is(lc)) {
                     let e = r;
-                    null != e && e.showEdgeValues != Tn.Auto && (t.showEdgeValues = e.showEdgeValues != Tn.False)
+                    null != e && e.showEdgeValues != Fn.Auto && (t.showEdgeValues = e.showEdgeValues != Fn.False)
                 }
             }
             static renderAxisRange(e, t) {
                 t[L.System.StiObject.stimulsoft]().getType() != lc && t[L.System.StiObject.stimulsoft]().getType() != nc || (e.auto = t.range.auto, e.maximum = t.range.maximum, e.minimum = t.range.minimum)
             }
             static renderAxisLabelsTitleColor(e, t, r, i) {
                 if (!N.transparent.equals(r.color)) return void(t.color = r.color);
@@ -12755,15 +12765,15 @@
                 if (!N.transparent.equals(e.legend.title.color)) return void(t.legend.titleColor = e.legend.title.color);
                 e.style == o.Custom && !N.transparent.equals(t.legend.titleColor) || (t.legend.titleColor = r)
             }
             static renderSeriesLabelsLegendValueType(e, t) {
                 let r = 0;
                 t.series.toList().cast().where(e => null != e.arguments).toList().forEach(e => {
                     r += e.arguments[L.System.StiObject.stimulsoft]().toList().count2(e => null != e)
-                }), null == e.legend.labels.valueType ? 0 < r && 1 < t.series.count ? t.seriesLabels.legendValueType = Sn.SeriesTitleArgument : 1 == r && 1 == t.series.count && (e.isPieChart || e.isPie3dChart || e.isDoughnutChart) ? t.seriesLabels.legendValueType = Sn.SeriesTitle : 0 < r && 1 == t.series.count ? t.seriesLabels.legendValueType = Sn.Argument : 0 == r && 1 < t.series.count ? t.seriesLabels.legendValueType = Sn.SeriesTitle : t.seriesLabels.legendValueType = e.isBubbleChart ? Sn.Weight : Sn.Value : t.seriesLabels.legendValueType = e.legend.labels.valueType
+                }), null == e.legend.labels.valueType ? 0 < r && 1 < t.series.count ? t.seriesLabels.legendValueType = wn.SeriesTitleArgument : 1 == r && 1 == t.series.count && (e.isPieChart || e.isPie3dChart || e.isDoughnutChart) ? t.seriesLabels.legendValueType = wn.SeriesTitle : 0 < r && 1 == t.series.count ? t.seriesLabels.legendValueType = wn.Argument : 0 == r && 1 < t.series.count ? t.seriesLabels.legendValueType = wn.SeriesTitle : t.seriesLabels.legendValueType = e.isBubbleChart ? wn.Weight : wn.Value : t.seriesLabels.legendValueType = e.legend.labels.valueType
             }
             static renderLegendLabelsColor(e, t, r) {
                 if (!N.transparent.equals(e.legend.labels.color)) return void(t.legend.labelsColor = e.legend.labels.color);
                 e.style == o.Custom && !N.transparent.equals(t.legend.labelsColor) || (t.legend.labelsColor = r)
             }
             static async renderConditions(e, t, r, i) {
                 let s = null != r.chartConditions ? r.chartConditions.where(e => e.keyValueMeter == i.key) : null,
@@ -12846,25 +12856,25 @@
                 var i;
                 let s = null == (i = e.trendLines) ? void 0 : i.where(e => e.keyValueMeter == r.key).toList();
                 t.trendLines.clear();
                 for (let e of s) t.trendLines.add(this.getTrendLine(e, t.chart))
             }
             static getTrendLine(t, r) {
                 switch (t.type) {
-                    case Rn.None:
+                    case En.None:
                         return new L.Report.Chart["StiTrendLineNone"];
-                    case Rn.Exponential: {
+                    case En.Exponential: {
                         let e = new L.Report.Chart["StiTrendLineExponential"];
                         return e.allowApplyStyle = !1, e.lineColor = N.transparent.equals(t.lineColor) ? r.style.core.trendLineColor : t.lineColor, e.lineStyle = t.lineStyle, e.lineWidth = t.lineWidth, e.showShadow = !1, e
                     }
-                    case Rn.Linear: {
+                    case En.Linear: {
                         let e = new L.Report.Chart["StiTrendLineLinear"];
                         return e.allowApplyStyle = !1, e.lineColor = N.transparent.equals(t.lineColor) ? r.style.core.trendLineColor : t.lineColor, e.lineStyle = t.lineStyle, e.lineWidth = t.lineWidth, e.showShadow = !1, e
                     }
-                    case Rn.Logarithmic: {
+                    case En.Logarithmic: {
                         let e = new L.Report.Chart["StiTrendLineLogarithmic"];
                         return e.allowApplyStyle = !1, e.lineColor = N.transparent.equals(t.lineColor) ? r.style.core.trendLineColor : t.lineColor, e.lineStyle = t.lineStyle, e.lineWidth = t.lineWidth, e.showShadow = !1, e
                     }
                 }
             }
             async renderSeriesLabels(t, r) {
                 if (!(t.isPieChart || t.isPie3dChart || t.isFunnelChart || t.isPictorialStackedChart || t.isDoughnutChart || t.isTreemapChart || t.isAxisAreaChart || t.isSunburstChart || t.isRadarChart || t.isWaterfallChart || t.isAxisAreaChart3D || t.isLineChart3D)) return void(r.seriesLabels.visible = !1);
@@ -13133,63 +13143,63 @@
                         break
                 }
             }
             static renderPieLabelsStyle(e, t) {
                 let r = t.seriesLabels.as(Jm);
                 switch (e.labels.style) {
                     case Wm.PercentOfTotal:
-                        r.showInPercent = !0, r.valueType = Sn.Value;
+                        r.showInPercent = !0, r.valueType = wn.Value;
                         break;
                     case Wm.Category:
-                        r.showInPercent = !1, r.valueType = e.arguments.any() ? Sn.Argument : Sn.SeriesTitle;
+                        r.showInPercent = !1, r.valueType = e.arguments.any() ? wn.Argument : wn.SeriesTitle;
                         break;
                     case Wm.CategoryPercentOfTotal:
-                        r.showInPercent = !0, r.valueType = e.arguments.any() ? Sn.ArgumentValue : Sn.SeriesTitleValue;
+                        r.showInPercent = !0, r.valueType = e.arguments.any() ? wn.ArgumentValue : wn.SeriesTitleValue;
                         break;
                     case Wm.CategoryValue:
-                        r.showInPercent = !1, r.valueType = e.arguments.any() ? Sn.ArgumentValue : Sn.SeriesTitleValue;
+                        r.showInPercent = !1, r.valueType = e.arguments.any() ? wn.ArgumentValue : wn.SeriesTitleValue;
                         break;
                     case Wm.Value:
-                        r.showInPercent = !1, r.valueType = Sn.Value;
+                        r.showInPercent = !1, r.valueType = wn.Value;
                         break
                 }
             }
             static renderLabelsStyle(e, t) {
                 let r = t.seriesLabels;
                 switch (e.labels.style) {
                     case Wm.PercentOfTotal:
-                        r.valueType = Sn.Value;
+                        r.valueType = wn.Value;
                         break;
                     case Wm.Category:
-                        r.valueType = e.arguments.any() ? Sn.Argument : Sn.SeriesTitle;
+                        r.valueType = e.arguments.any() ? wn.Argument : wn.SeriesTitle;
                         break;
                     case Wm.CategoryPercentOfTotal:
-                        r.valueType = e.arguments.any() ? Sn.ArgumentValue : Sn.SeriesTitleValue;
+                        r.valueType = e.arguments.any() ? wn.ArgumentValue : wn.SeriesTitleValue;
                         break;
                     case Wm.CategoryValue:
-                        r.valueType = e.arguments.any() ? Sn.ArgumentValue : Sn.SeriesTitleValue;
+                        r.valueType = e.arguments.any() ? wn.ArgumentValue : wn.SeriesTitleValue;
                         break;
                     case Wm.Value:
-                        r.valueType = Sn.Value;
+                        r.valueType = wn.Value;
                         break
                 }
             }
             async renderSeriesInteraction(r, i, e, s) {
                 if (r.chart.isDesigning) return;
                 let n = null == i ? void 0 : i.report,
                     l = 0,
                     t = i.dashboardInteraction;
                 if (t.onHover == Vr.ShowToolTip) {
-                    r.toolTips = Ln.create(String, e);
+                    r.toolTips = Bn.create(String, e);
                     for (let t of r.arguments) {
                         let e = "";
                         l < r.values.length && null != r.values[l] && (e = r.values[l].toString()), r.toolTips[l] = await this.getToolTip(r.chart.style, i, i.dashboardInteraction.toolTip, this.getString(i.argumentFormat, t, n), this.getString(i.valueFormat, e, n), s), l++
                     }
                 }
-                l = 0, r.hyperlinks = Ln.create(String, e);
+                l = 0, r.hyperlinks = Bn.create(String, e);
                 for (let t of r.arguments) {
                     let e = "";
                     l < r.values.length && null != r.values[l] && (e = r.values[l].toString()), r.hyperlinks[l] = await this.getHyperlink(i, i.dashboardInteraction.hyperlink, null === t || void 0 === t ? void 0 : t.toString(), e, r.titleValue), l++
                 }
                 r.drillDownEnabled = !0
             }
             async getToolTip(r, e, t, i, s, n) {
@@ -13232,22 +13242,22 @@
             }
             simplifyValues(e) {
                 let t = 0;
                 while (t < e.series.count) {
                     let r = e.series.getByIndex(t);
                     if (800 < r.values.length) {
                         let t = this.getShorterListPoints(r);
-                        r.values = Ln.create(Number, t.length), r.arguments = Ln.create(Object, t.length);
+                        r.values = Bn.create(Number, t.length), r.arguments = Bn.create(Object, t.length);
                         for (let e = 0; e < t.length; e++) r.values[e] = t[e].x, r.arguments[e] = t[e].y
                     }
                     t++
                 }
             }
             getShorterListPoints(t) {
-                let r = Ln.create(Yl, t.values.length);
+                let r = Bn.create(Yl, t.values.length);
                 for (let e = 0; e < t.values.length; e++) r[e] = new Yl(t.values[e], e);
                 let i = [.3, .6, 1, 5, 9, 15, 20, 25, 30, 40],
                     s = null,
                     n = null;
                 for (let e = 0; e < i.length; e++) {
                     if ((s = L.Report.Chart["StiSimplifyHelper"].simplify(r, e, !0)[L.System.StiObject.stimulsoft]().toList()).length / r.length < .02 && s.length < 900 && null != n) {
                         s = n;
@@ -13255,26 +13265,26 @@
                     }
                     n = s
                 }
                 return s
             }
             getString(r, i, s) {
                 if (null == i) return "";
-                if (Ln.isArray(i)) {
+                if (Bn.isArray(i)) {
                     let t = new P;
                     for (let e of i) t.add(this.getFormatValue(r, e, s));
                     return B.join(" - ", t)
                 }
                 return this.getFormatValue(r, i, s)
             }
             getFormatValue(e, t, r) {
                 if (null == t) return "";
                 if (t instanceof w) return e.is2(Xr) || e.is2(Gr) || e.is2(ic) ? e.format(t) : t.toShortDateString();
                 let i = null == r ? void 0 : r.getParsedCulture();
-                if (li.isEligable(t, i)) return li.convert(t, i);
+                if (ai.isEligable(t, i)) return ai.convert(t, i);
                 if (null != e) return e.format(t);
                 return t.toString()
             }
             async calculateIndicatorValue(r) {
                 if (null == r.indicatorValue || null != r.indicatorValue && B.isNullOrEmpty(r.indicatorValue.expression)) return;
                 let i = bl.getKey(r);
                 if (Rm.existsInCache(i)) this.indicatorValueValue = Rm.getFromCache(i);
@@ -13298,31 +13308,31 @@
             }
             getArgumentMeterIndexes(t) {
                 if (null == t) return null;
                 return this.getArgumentMeters(t).select(e => t.meters.indexOf(e)).toList()
             }
             getSeriesMeterIndex(e) {
                 if (null == e) return -1;
-                let t = e.meters.firstOrDefault(e => e.is(Ps));
+                let t = e.meters.firstOrDefault(e => e.is(js));
                 return null != t ? e.meters.indexOf(t) : -1
             }
             getArgumentKeys(e, t) {
                 if (null == t) return null;
                 let r = this.getArgumentMeters(t),
                     i = r.select(e => t.meters.indexOf(e)).toList(),
                     s = t.rows.groupBy2(t => i.select(e => t[e])[L.System.StiObject.stimulsoft]().toArray(), new Mh);
                 return s.select(e => e.key[L.System.StiObject.stimulsoft]().toArray())
             }
             getValueMeters(e) {
                 if (null == e) return null;
-                return e.meters.where(e => e.is(Bs)).cast()
+                return e.meters.where(e => e.is(Ps)).cast()
             }
             getArgumentMeters(e) {
                 if (null == e) return null;
-                return e.meters.where(e => e.is(Ls)).cast()
+                return e.meters.where(e => e.is(Bs)).cast()
             }
         }
         F.i.StiChartElementBuilder = S
     }
     let Mc = L.Report.Chart.IStiBubbleSeries,
         Tc = (F.i.StiBubbleChartElementBuilder = class extends F.i.StiChartElementBuilder {
             async renderElements(u, h, m) {
@@ -13354,15 +13364,15 @@
                 return s.coreTitle = this.getSeriesTitle(e, r, t), s.isDashboard = !0, i.series.add(s), s
             }
             async renderSeriesInteraction(l, e, t, a) {
                 let o = l.as(Mc);
                 if (null == o) return;
                 let u = e.dashboardInteraction;
                 if (u.onHover == Vr.ShowToolTip) {
-                    l.toolTips = Ln.create(String, t);
+                    l.toolTips = Bn.create(String, t);
                     for (let n = 0; n < t; n++) {
                         let r = "",
                             i = "",
                             s = "";
                         if (n < l.values.length && null != l.values[n] && (r = l.values[n].toString()), n < l.arguments.length && null != l.arguments[n] && (i = `` + l.arguments[n]), n < o.weights.length && (s = o.weights[n].toString()), B.isNullOrEmpty(u.toolTip)) {
                             let e = '"StiColor":"{0}","StiValue":"{1}","StiArgument":"{2}","StiWeight":"{3}"{4}',
                                 t = await this.getToolTipStyle(l.chart.style);
@@ -13388,15 +13398,15 @@
             }
             getWeightMeterIndexes(t) {
                 if (null == t) return null;
                 return this.getWeightMeters(t).select(e => t.meters.indexOf(e)).toList()
             }
             getWeightMeters(e) {
                 if (null == e) return null;
-                return e.meters.where(e => e.is(Es)).cast()
+                return e.meters.where(e => e.is(Os)).cast()
             }
             getValueMeters(e) {
                 if (null == e) return null;
                 return e.meters.where(e => e.is(_n)).cast()
             }
             getArgumentMeters(e) {
                 if (null == e) return null;
@@ -13438,23 +13448,23 @@
                         let a = this.getArgumentIndex(g, e),
                             o = (-1 != a && (t.arguments = i.getArrayItem(a).select(e => this.getString(c.argumentFormat, e, p))[L.System.StiObject.stimulsoft]().toArray()), h++, Math.min(t.values.length, t.arguments.length));
                         await this.renderSeriesInteraction(t, c, o, m)
                     }
                 }
             }
             renderSeries(e, t, r, i) {
-                let s = Pn.neww2(t.as(Os).seriesType);
+                let s = Pn.neww2(t.as(Vs).seriesType);
                 return s.coreTitle = this.getSeriesTitle(e, r, t), s.isDashboard = !0, i.series.add(s), s
             }
             async renderSeriesInteraction(o, e, t, r) {
                 let u = o.as(Tc);
                 if (null == u) return;
                 let i = e.dashboardInteraction;
                 if (i.onHover == Vr.ShowToolTip) {
-                    o.toolTips = Ln.create(String, t);
+                    o.toolTips = Bn.create(String, t);
                     for (let a = 0; a < t; a++) {
                         let e = "",
                             t = "",
                             r = "",
                             i = "",
                             s = "",
                             n = (a < u.valuesOpen.length && null != u.valuesOpen[a] && (e = u.valuesOpen[a].toString()), a < u.valuesClose.length && (t = u.valuesClose[a].toString()), a < u.valuesLow.length && (r = u.valuesLow[a].toString()), a < u.valuesHigh.length && (i = u.valuesHigh[a].toString()), a < o.arguments.length && null != o.arguments[a] && (s = `` + o.arguments[a]), '"StiColor":"{0}","StiOpenValue":"{1}","StiCloseValue":"{2}","StiLowValue":"{3}","StiHighValue":"{4}","StiArgument":"{5}"{6}'),
@@ -13485,15 +13495,15 @@
                 }
                 let t = c.area.as(ac),
                     r = (t.yAxis.range.auto = !1, t.yAxis.range.minimum = d, t.yAxis.range.maximum = g, t.yAxis.range.maximum - t.yAxis.range.minimum);
                 t.yAxis.labels.step = 2 < r ? Math.round(r / 10) : ae.round2(r / 10, 4)
             }
             getValueMeters(e) {
                 if (null == e) return null;
-                return e.meters.where(e => e.is(Os)).cast()
+                return e.meters.where(e => e.is(Vs)).cast()
             }
             getCloseValueIndex(e, t) {
                 if (null == e) return -1;
                 let r = this.getCloseMeterIndexes(e);
                 if (null == r || !r.any()) return -1;
                 if (1 == r.length) return r.toList().firstOrDefault();
                 if (r.length > t) return r[t];
@@ -13501,15 +13511,15 @@
             }
             getCloseMeterIndexes(t) {
                 if (null == t) return null;
                 return this.getCloseMeters(t).select(e => t.meters.indexOf(e)).toList()
             }
             getCloseMeters(e) {
                 if (null == e) return null;
-                return e.meters.where(e => e.is(Vs)).cast()
+                return e.meters.where(e => e.is(ks)).cast()
             }
             getLowValueIndex(e, t) {
                 if (null == e) return -1;
                 let r = this.getLowMeterIndexes(e);
                 if (null == r || !r.any()) return -1;
                 if (1 == r.length) return r.toList().firstOrDefault();
                 if (r.length > t) return r[t];
@@ -13517,15 +13527,15 @@
             }
             getLowMeterIndexes(t) {
                 if (null == t) return null;
                 return this.getLowMeters(t).select(e => t.meters.indexOf(e)).toList()
             }
             getLowMeters(e) {
                 if (null == e) return null;
-                return e.meters.where(e => e.is(ks)).cast()
+                return e.meters.where(e => e.is(Ns)).cast()
             }
             getHighValueIndex(e, t) {
                 if (null == e) return -1;
                 let r = this.getHighMeterIndexes(e);
                 if (null == r) return -1;
                 if (!r.any()) return -1;
                 if (1 == r.length) return r.toList().firstOrDefault();
@@ -13534,15 +13544,15 @@
             }
             getHighMeterIndexes(t) {
                 if (null == t) return null;
                 return this.getHighMeters(t).select(e => t.meters.indexOf(e)).toList()
             }
             getHighMeters(e) {
                 if (null == e) return null;
-                return e.meters.where(e => e.is(Ns)).cast()
+                return e.meters.where(e => e.is(Ls)).cast()
             }
         }, L.Report.Chart.IStiRangeSeries),
         vc = (F.i.StiRangeChartElementBuilder = class extends F.i.StiChartElementBuilder {
             async renderElements(u, h, m) {
                 let c = null == h ? void 0 : h.report,
                     d = this.getSeriesMeterIndex(m),
                     e = this.getSeriesKeys(m, d),
@@ -13590,15 +13600,15 @@
             async renderSeriesInteraction(s, n, e, l) {
                 var a, o;
                 let u = null == n ? void 0 : n.report,
                     h = s.as(Fc);
                 if (null == h) return;
                 let t = n.dashboardInteraction.as(zn);
                 if (t.onHover == Vr.ShowToolTip) {
-                    s.toolTips = Ln.create(String, e);
+                    s.toolTips = Bn.create(String, e);
                     for (let i = 0; i < e; i++) {
                         let e = "",
                             t = "",
                             r = "";
                         i < s.values.length && null != s.values[i] && (e = (s.core.isDateTimeValues ? w.fromOADate(s.values[i]) : s.values[i]).toString()), null != h.valuesEnd && i < h.valuesEnd.length && (t = s.core.isDateTimeValues ? null == (a = w.fromOADate(h.valuesEnd[i])) ? void 0 : a.toString() : null == (o = h.valuesEnd[i]) ? void 0 : o.toString()), i < s.arguments.length && null != s.arguments[i] && (r = `` + s.arguments[i]), s.toolTips[i] = await this.getToolTip2(s.chart.style, n, n.dashboardInteraction.toolTip, this.getString(n.argumentFormat, r, u), this.getString(n.valueFormat, e, u), this.getString(n.valueFormat, t, u), l)
                     }
                 }
@@ -13632,15 +13642,15 @@
             }
             getEndValueMeterIndexes(t) {
                 if (null == t) return null;
                 return this.getEndValueMeters(t).select(e => t.meters.indexOf(e)).toList()
             }
             getEndValueMeters(e) {
                 if (null == e) return null;
-                return e.meters.where(e => e.is(js)).cast()
+                return e.meters.where(e => e.is(Hs)).cast()
             }
         }, L.Report.Components.StiShape),
         Ac = (F.i.StiShapeElementBuilder = class {
             render(e) {
                 let t = new vc;
                 return t.shapeType = e.shapeType, t.brush = e.fill, t.borderColor = e.stroke, t.size = e.size, t
             }
@@ -13765,15 +13775,15 @@
             let t = this.getArgumentMeters(n),
                 l = this.getValueMeters(n).firstOrDefault(),
                 a = this.getValueMeterIndexes(n)[L.System.StiObject.stimulsoft]().toList().firstOrDefault();
             for (let e = 0; e < t.length; e++) {
                 let t = this.getArgumentMeterIndexes(n)[e],
                     r = this.renderSeries(i, l, "", s);
                 if (null == r) continue;
-                r.values = Ln.create(Number, n.rows.length), r.arguments = Ln.create(Object, n.rows.length);
+                r.values = Bn.create(Number, n.rows.length), r.arguments = Bn.create(Object, n.rows.length);
                 for (let e = 0; e < n.rows.length; e++) r.values[e] = V.tryToNullableNumber(n.rows[e][a]), r.arguments[e] = n.rows[e][t];
                 await this.renderSeriesInteraction(r, i, r.arguments.length, "")
             }
         }
         renderSeries(e, t, r, i) {
             let s = Pn.neww2(t.seriesType);
             return s.core.seriesColors = null != e.seriesColors && 0 < e.seriesColors.length ? e.seriesColors : null, s.isDashboard = !0, i.series.add(s), s
@@ -13810,15 +13820,15 @@
             }
             getTextValues() {
                 let i = new P,
                     s = this.getTargetValues();
                 for (let r = 0; r < this.iterations.length; r++) {
                     let e = s[r],
                         t = 0 != e ? Math.abs(this.iterations[r].value) / e : 0;
-                    i.add(ts.formatAsPercentage2(this.element.report, this.element.textFormat, t))
+                    i.add(rs.formatAsPercentage2(this.element.report, this.element.textFormat, t))
                 }
                 return i
             }
             getColor(e) {
                 return this.element.colorEach ? this.getColors(this.iterations.length)[e] : this.style.bandColor
             }
             getColors(e) {
@@ -13857,15 +13867,15 @@
                         break;
                     case Lo.Target:
                         s = i.target;
                         break;
                     case Lo.Percentage: {
                         let e = this.getVariation(i),
                             t = new Ur,
-                            r = (t.decimalDigits = 3, ts.formatAsPercentage2(this.element.report, t, e));
+                            r = (t.decimalDigits = 3, rs.formatAsPercentage2(this.element.report, t, e));
                         s = r.replace("%", "")[L.System.StiObject.stimulsoft]().toNumber();
                         break
                     }
                 }
                 let e = !1,
                     r = this.getConditionValue(t);
                 if (null != s) {
@@ -13944,16 +13954,16 @@
                 return e
             }
             processFontStyle(e, t) {
                 let r = this.processFontBold(e.bold, t),
                     i = this.processFontItalic(e.italic, t),
                     s = this.processFontUnderline(e.underline, t),
                     n = this.processFontStrikeout(e.strikeout, t),
-                    l = hn.Regular;
-                return r && (l ^= hn.Bold), i && (l ^= hn.Italic), s && (l ^= hn.Underline), n && (l ^= hn.Strikeout), l
+                    l = mn.Regular;
+                return r && (l ^= mn.Bold), i && (l ^= mn.Italic), s && (l ^= mn.Underline), n && (l ^= mn.Strikeout), l
             }
             processFontStrikeout(e, t) {
                 for (let e of this.element.progressConditions)
                     if (0 < (e.permissions & Bo.FontStyleStrikeout) && this.getConditionResult(t, e)) return e.font.strikeout;
                 return e
             }
             processFontUnderline(e, t) {
@@ -14002,16 +14012,15 @@
                     f = this.getTargetValues(),
                     y = !1;
                 h.pushClip(m);
                 for (let u = 0; u < this.iterations.length; u++) {
                     let e = f[u],
                         t = this.iterations[u],
                         r = c[u],
-                        i = (!y && (1 < r.right - m.right || 1 < r.bottom - m.bottom) && (y = !0),
-                            r.x + r.width / 2),
+                        i = (!y && (1 < r.right - m.right || 1 < r.bottom - m.bottom) && (y = !0), r.x + r.width / 2),
                         s = r.y + g + (d.height - g) / 2,
                         n = new Yl(i, s),
                         l = new j(n.x - w, n.y - w, b, b),
                         a = new j(l.x + l.width / 2 - p / 2, l.top - g, p, g),
                         o = this.processColor(this.getColor(u), this.iterations[u]);
                     this.drawPieProgress(h, l, a, e, t, S, o)
                 }
@@ -14068,15 +14077,15 @@
             for (let t of this.iterations.where(e => !B.isNullOrEmpty(e.series))) {
                 let e = Xu.getFontSize(g, new j(0, 0, C, y), t.series, r);
                 (null == T || T > e) && (T = e)
             }
             let F = (e - (y = null != T && T < f.size ? this.getTitleHeight(e, T) : y)) / 2 * .8,
                 v = null,
                 i = new j(b.x - F * w, b.y - .79 * F, 2 * F * w, 2 * F * w),
-                s = new H(this.element.font.name, 1, hn.Bold, Sh.Pixel);
+                s = new H(this.element.font.name, 1, mn.Bold, Sh.Pixel);
             for (let t = 0; t < this.iterations.length; t++) {
                 let e = Xu.getFontSize(g, i, M[t], s);
                 (null == v || v > e) && (v = e)
             }
             T < this.minFontSize && (y = 0, T = 0, F = e / 2 * .8);
             let A = 2 * F,
                 I = F / 5,
@@ -14097,15 +14106,15 @@
                     a = 0 != l ? 360 / l * Math.abs(this.iterations[d].value) : 0,
                     o = -90,
                     u = (360 < a && (a = 360), new P),
                     h = (u.add(new Oc(c, o, a)), u.add(new Pu(this.getPoint(m, F, o + a), this.getPoint(m, D, o + a))), u.add(new Oc(i, o + a, -a)), u.add(new Pu(this.getPoint(m, D, o), this.getPoint(m, F, o))), this.processColor(this.getColor(d), this.iterations[d]));
                 if (g.fillPath(h, u, c, null), v >= this.minFontSize) {
                     let e = new j(m.x - F * w, m.y - .79 * F, 2 * F * w, 2 * F * w),
                         t = M[d],
-                        r = new H(this.element.font.name, v, hn.Bold, Sh.Pixel),
+                        r = new H(this.element.font.name, v, mn.Bold, Sh.Pixel),
                         i = this.processFontStyle(r, this.iterations[d]),
                         s = new Nu(r.name, r.size, i, r.unit),
                         n = this.processForeColor(this.iterations[d]);
                     g.drawRotatedString5(t, s, n, e, Xu.getStringFormatGeom(g), Lu.CenterCenter, 0, !0)
                 }
                 if (T >= this.minFontSize) {
                     let e = new j(m.x - C / 2, c.top - y, C, y),
@@ -14166,15 +14175,15 @@
                     t = this.processFontStyle(T, this.iterations[g]),
                     n = new H(e, T.size, t),
                     r = y[g],
                     i = S.y + (w + F) * g,
                     l = new j(S.x, i, f, b),
                     s = this.processTrackColor(this.style.trackColor, this.iterations[g]),
                     a = (p.fillRectangle(s, l, null), 0 != r ? Math.abs(this.iterations[g].value) / r : 0),
-                    o = ts.formatAsPercentage2(this.element.report, this.element.textFormat, a),
+                    o = rs.formatAsPercentage2(this.element.report, this.element.textFormat, a),
                     u = J.getForeColor(this.element);
                 if (x >= this.minFontSize) {
                     let e = new Nu(C.fontFamily.name, M, n.style, n.unit),
                         t = p.measureString(o, e),
                         r = new j(l.right - t.width, l.top + .05 * l.height, t.width, l.height);
                     u = this.processForeColor(this.iterations[g]), p.drawRotatedString5(o, e, u, r, Xu.getStringFormatGeom(p), Lu.CenterCenter, 0, !0)
                 }
@@ -14640,15 +14649,15 @@
             }
             renderEmptyDataMessage(t, r, i, e) {
                 var s;
                 if (!e.is(zc) || e.renderEmptyContent) return !1;
                 if (t.is(Jo) && t.dataFrom == Wo.Manual) return !1;
                 if (t.is(Ha) && (null != t.image || null != t.icon || !B.isNullOrEmpty(t.imageHyperlink))) return !1;
                 if (t.is(yu) && (!B.isNullOrEmpty(t.url) || !B.isNullOrEmpty(t.embedCode))) return !1;
-                if (0 < t.getMeters().length || (null == (s = t.as(rh)) ? void 0 : s.dataMode) == Vn.ManuallyEnteringData) return !1;
+                if (0 < t.getMeters().length || (null == (s = t.as(rh)) ? void 0 : s.dataMode) == kn.ManuallyEnteringData) return !1;
                 let n = i.size,
                     l = new H("Arial", 9),
                     a = t.is(yu) ? b.get("FormStyleDesigner", "NotSpecified") : t.is(Ha) ? b.get("Dashboard", "ImageNotSpecified") : b.get("Dashboard", "DragDropDataFromDictionary"),
                     o = oh.measureString(a, l);
                 if (i.y += i.height / 2 - 48, i.height = Math.min(32, i.height), 48 <= n.width && 64 <= n.height) {
                     i.y += n.width > o.width + 16 ? 16 : 32;
                     let e = new ad(new j(i.width / 2 - 16, i.y, 32, 32));
@@ -14661,15 +14670,15 @@
                 }
                 return !0
             }
             format(e, t) {
                 var r, i;
                 if (null != t && null != e) {
                     if (t instanceof w && !e.textFormat.is(Xr)) return t.toShortDateString();
-                    return li.isEligable(t, null == (r = null == e ? void 0 : e.report) ? void 0 : r.culture) ? li.convert(t, null == (i = null == e ? void 0 : e.report) ? void 0 : i.culture) : e.textFormat.format(t)
+                    return ai.isEligable(t, null == (r = null == e ? void 0 : e.report) ? void 0 : r.culture) ? ai.convert(t, null == (i = null == e ? void 0 : e.report) ? void 0 : i.culture) : e.textFormat.format(t)
                 }
                 return ""
             }
             getEmptyDataImage(e) {
                 if (e.is(L.Report.Dashboard.IStiTableElement)) return "data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACAAAAAgCAYAAABzenr0AAAAGXRFWHRTb2Z0d2FyZQBBZG9iZSBJbWFnZVJlYWR5ccllPAAAA4RpVFh0WE1MOmNvbS5hZG9iZS54bXAAAAAAADw/eHBhY2tldCBiZWdpbj0i77u/IiBpZD0iVzVNME1wQ2VoaUh6cmVTek5UY3prYzlkIj8+IDx4OnhtcG1ldGEgeG1sbnM6eD0iYWRvYmU6bnM6bWV0YS8iIHg6eG1wdGs9IkFkb2JlIFhNUCBDb3JlIDUuNi1jMTM4IDc5LjE1OTgyNCwgMjAxNi8wOS8xNC0wMTowOTowMSAgICAgICAgIj4gPHJkZjpSREYgeG1sbnM6cmRmPSJodHRwOi8vd3d3LnczLm9yZy8xOTk5LzAyLzIyLXJkZi1zeW50YXgtbnMjIj4gPHJkZjpEZXNjcmlwdGlvbiByZGY6YWJvdXQ9IiIgeG1sbnM6eG1wTU09Imh0dHA6Ly9ucy5hZG9iZS5jb20veGFwLzEuMC9tbS8iIHhtbG5zOnN0UmVmPSJodHRwOi8vbnMuYWRvYmUuY29tL3hhcC8xLjAvc1R5cGUvUmVzb3VyY2VSZWYjIiB4bWxuczp4bXA9Imh0dHA6Ly9ucy5hZG9iZS5jb20veGFwLzEuMC8iIHhtcE1NOk9yaWdpbmFsRG9jdW1lbnRJRD0ieG1wLmRpZDo4M2I5YzlhNS1lZGRmLTU0NGItODFmMi1mMzVmMDgyNTUzMTciIHhtcE1NOkRvY3VtZW50SUQ9InhtcC5kaWQ6OTIzODI0M0M3MzI1MTFFN0E4QTI5RjYzRTdGNDREM0MiIHhtcE1NOkluc3RhbmNlSUQ9InhtcC5paWQ6OTIzODI0M0I3MzI1MTFFN0E4QTI5RjYzRTdGNDREM0MiIHhtcDpDcmVhdG9yVG9vbD0iQWRvYmUgUGhvdG9zaG9wIENDIDIwMTcgKFdpbmRvd3MpIj4gPHhtcE1NOkRlcml2ZWRGcm9tIHN0UmVmOmluc3RhbmNlSUQ9InhtcC5paWQ6NWU4YzI0ZGYtNjI5ZS1jNDQwLTg2NjMtMjlmM2VlODA4MGFjIiBzdFJlZjpkb2N1bWVudElEPSJhZG9iZTpkb2NpZDpwaG90b3Nob3A6YWM1MjY1OGUtNzMxZC0xMWU3LWE0ZGMtODFhMmMxY2EwMjcyIi8+IDwvcmRmOkRlc2NyaXB0aW9uPiA8L3JkZjpSREY+IDwveDp4bXBtZXRhPiA8P3hwYWNrZXQgZW5kPSJyIj8+9Pfr+wAAAINJREFUeNrsl8EJwCAQBD2xoOu/Ce1CrgqDEIJGMQQMm8fuRxbmsRzzUUopDpmQUsIOOF/UGSS0TVUHYnahnZxvi5m5Vf+C6wbknC+ovrXPspOTGCPUAe/ACSth7vI8MW+5wQFE4APgEtIBOkAH6AAdoAN0gAN+I6HALoD+HcMdOAQYAAB9hUYI2ET/AAAAAElFTkSuQmCC";
                 if (e.is(L.Report.Dashboard.IStiCardsElement)) return "data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACAAAAAgCAYAAABzenr0AAAAGXRFWHRTb2Z0d2FyZQBBZG9iZSBJbWFnZVJlYWR5ccllPAAAA4RpVFh0WE1MOmNvbS5hZG9iZS54bXAAAAAAADw/eHBhY2tldCBiZWdpbj0i77u/IiBpZD0iVzVNME1wQ2VoaUh6cmVTek5UY3prYzlkIj8+IDx4OnhtcG1ldGEgeG1sbnM6eD0iYWRvYmU6bnM6bWV0YS8iIHg6eG1wdGs9IkFkb2JlIFhNUCBDb3JlIDYuMC1jMDA2IDc5LjE2NDc1MywgMjAyMS8wMi8xNS0xMTo1MjoxMyAgICAgICAgIj4gPHJkZjpSREYgeG1sbnM6cmRmPSJodHRwOi8vd3d3LnczLm9yZy8xOTk5LzAyLzIyLXJkZi1zeW50YXgtbnMjIj4gPHJkZjpEZXNjcmlwdGlvbiByZGY6YWJvdXQ9IiIgeG1sbnM6eG1wTU09Imh0dHA6Ly9ucy5hZG9iZS5jb20veGFwLzEuMC9tbS8iIHhtbG5zOnN0UmVmPSJodHRwOi8vbnMuYWRvYmUuY29tL3hhcC8xLjAvc1R5cGUvUmVzb3VyY2VSZWYjIiB4bWxuczp4bXA9Imh0dHA6Ly9ucy5hZG9iZS5jb20veGFwLzEuMC8iIHhtcE1NOk9yaWdpbmFsRG9jdW1lbnRJRD0ieG1wLmRpZDo4M2I5YzlhNS1lZGRmLTU0NGItODFmMi1mMzVmMDgyNTUzMTciIHhtcE1NOkRvY3VtZW50SUQ9InhtcC5kaWQ6NUIzNTA2OThGNDM4MTFFQjg0MDZGNjlFNzQyNzdDRTQiIHhtcE1NOkluc3RhbmNlSUQ9InhtcC5paWQ6NUIzNTA2OTdGNDM4MTFFQjg0MDZGNjlFNzQyNzdDRTQiIHhtcDpDcmVhdG9yVG9vbD0iQWRvYmUgUGhvdG9zaG9wIENDIDIwMTcgKFdpbmRvd3MpIj4gPHhtcE1NOkRlcml2ZWRGcm9tIHN0UmVmOmluc3RhbmNlSUQ9InhtcC5paWQ6Mjc2NTY1N2UtZjU3OS03OTQxLWIwYTgtZGU3MjdiYjI3MDhhIiBzdFJlZjpkb2N1bWVudElEPSJhZG9iZTpkb2NpZDpwaG90b3Nob3A6OWZmYzA0NGMtNTQyYS03NTRkLWI0YzUtOTIwZWRkMTVlYjRlIi8+IDwvcmRmOkRlc2NyaXB0aW9uPiA8L3JkZjpSREY+IDwveDp4bXBtZXRhPiA8P3hwYWNrZXQgZW5kPSJyIj8+/5jbrAAAAG1JREFUeNrslzEOgDAMAxOU/+T/z8iLzMLACkZyAXvqUvWUNCclAYQyW4hTMyN7vLujjvPdPiR5V98CAxjAAHWeSWaeWQCZiOqhSl6tAvwJDbCcB9iABbCIKJlYRAb4jIiYJfG9Isrfb8e7AAMAInAVUndCPVIAAAAASUVORK5CYII=";
                 if (e.is(L.Report.Dashboard.IStiChartElement)) return "data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACAAAAAgCAYAAABzenr0AAAAGXRFWHRTb2Z0d2FyZQBBZG9iZSBJbWFnZVJlYWR5ccllPAAAAGNJREFUeNpi/P//P8NAAsaBdgATiDh//vz/AXXAgIfAQAIWYhXiiiZDQ0PG0SigSxTQKnpGo2DUAYMrF9CisCFk5mgUjDpg1AGjDhh1wKgDRh0A7hsOVNcMVCUzjvjeMUCAAQAQtyafO9RmPQAAAABJRU5ErkJggg==";
@@ -14804,33 +14813,41 @@
             static
             export (e, t) {
                 let r;
                 return r = t instanceof Cd ? t : t instanceof Lc ? F.z.StiExportSettingsHelper.getDashboardExportSettings(t) : F.z.StiExportSettingsHelper.getDashboardExportSettings2(t), this.exportToStream(e, r)
             }
             static async exportToStream(e, r) {
                 var t;
-                let s = new _h,
-                    i = (s.isDocument = !0, s.reportUnit = qh.HundredthsOfInch, L.Report.Painters.StiGdiMapContextPainter.isSvgExport = !0, s.renderedPages.getByIndex(0)),
-                    n = (i.orientation = r.orientation, i.paperSize = r.paperSize, (r.is(td) || r.is($c) || r.is(ed)) && (i.margins = new be(0)), r),
-                    l = ("width" in r && null != n && 0 < n.width && 0 < n.height && (i.width = n.width, i.height = n.height), null == (t = e.as(ue)) ? void 0 : t.dashboardWatermark);
+                let n = new _h,
+                    i = (n.isDocument = !0, n.reportUnit = qh.HundredthsOfInch, L.Report.Painters.StiGdiMapContextPainter.isSvgExport = !0, n.renderedPages.getByIndex(0)),
+                    s = (i.orientation = r.orientation, i.paperSize = r.paperSize, (r.is(td) || r.is($c) || r.is(ed)) && (i.margins = new be(0)), r),
+                    l = ("width" in r && null != s && 0 < s.width && 0 < s.height && (i.width = s.width, i.height = s.height), null == (t = e.as(ue)) ? void 0 : t.dashboardWatermark);
                 if (i.tagValue = l, null == i.tagValue && (i.tagValue = "*Dashboards*"), e.is(yd)) {
                     let t = e.fetchPages().where(e => e.is(Ae)).cast();
-                    for (let e = 0; e < t.length; e++) 0 < e && (i = i.clone(!0, !1), s.renderedPages.add(i)), await this.renderDashboardAsync(i, t[e], r)
-                } else e.is(Ae) ? (e.report && s.dictionary.resources.addRange(e.report.dictionary.resources), await this.renderDashboardAsync(i, e, r)) : e.is(Fe) && (s.reportAlias = e.name, e.is(Jo) && s.dictionary.resources.addRange(e.report.dictionary.resources), await this.renderSingleElementAsync(i, e, r));
-                for (let i of s.renderedPages.list) i.components.toList().where(e => e.is(re)).cast().forEach(e => {
+                    for (let e = 0; e < t.length; e++) 0 < e && (i = i.clone(!0, !1), n.renderedPages.add(i)), await this.renderDashboardAsync(i, t[e], r)
+                } else e.is(Ae) ? (e.report && n.dictionary.resources.addRange(e.report.dictionary.resources), await this.renderDashboardAsync(i, e, r)) : e.is(Fe) && (n.reportAlias = e.name, e.is(Jo) && n.dictionary.resources.addRange(e.report.dictionary.resources), await this.renderSingleElementAsync(i, e, r));
+                for (let i of n.renderedPages.list) i.components.toList().where(e => e.is(re)).cast().forEach(e => {
                     let t = i.components.indexOf(e) + 1,
                         r = e.getComponentsList();
                     for (let e = 0; e < r.length; e++) r[e].page = i, r[e].setDirectDisplayRectangle(r[e].componentToPage(r[e].displayRectangle)), i.components.insert(t + e, r[e]);
                     e.components.clear()
                 });
+                if (0 < n.renderedPages.count && !(L.Base.xKYzs.DuaNK.NoLPE() || L.Base.xKYzs.DuaNK.QpAFN() || (L.Base.xKYzs.DuaNK.OLBIj() || L.Base.xKYzs.DuaNK.ohTGO() || L.Base.xKYzs.DuaNK.RWIXN()) && L.System.NodeJs.isStandaloneVersion)) {
+                    let e = n.renderedPages.getByIndex(0),
+                        t = e.report.unit.convertFromHInches(200),
+                        r = e.report.unit.convertFromHInches(52),
+                        i = new j((e.width - t) / 2, e.height - r, t, r),
+                        s = new ad(i);
+                    s.stretch = !0, s.printable = !1, s.image = L.Report.Export.StiExportUtils.getAdditionalData2(192), s.name = L.Report.StiNameValidator.correctName(L.System.Guid.newGuidString().substring(0, 8)), s.componentPlacement = "pf.PageFooterBand", e.components.add(s)
+                }
                 let a, o = null == r ? Xc.Document : dd.convert(r.format);
-                if (o == Xc.Document) a = L.System.Text.Encoding.UTF8.getBytes(s.saveDocumentToJsonString());
+                if (o == Xc.Document) a = L.System.Text.Encoding.UTF8.getBytes(n.saveDocumentToJsonString());
                 else {
                     let e = cd.getExportSettings(r),
-                        t = await s.exportDocumentAsync2(o, null, e);
+                        t = await n.exportDocumentAsync2(o, null, e);
                     a = "string" == typeof t ? L.System.Text.Encoding.UTF8.getBytes(t) : "undefined" != typeof Buffer && Buffer.isBuffer(t) ? t.toJSON().data : t
                 }
                 return L.Report.Painters.StiGdiMapContextPainter.isSvgExport = !1, a
             }
             static async renderDashboardAsync(e, t, r) {
                 if (null == t) return;
                 null != r && (r.renderSinglePage = !0, r.renderSingleElement = !1);
@@ -14920,15 +14937,15 @@
                 }
             }
             static drawText(e, t, r, i, s, n, l) {
                 if (B.isNullOrWhiteSpace(s)) return;
                 t.width -= 2;
                 let a = new Md,
                     o = U.Table.Font.getGdiFont(i, null, n);
-                a.lineAlignment = mn.Center, a.alignment = this.toAlignment(r), a.trimming = Ru.None, a.formatFlags |= Td.NoWrap, e.drawString(s, o, l, t.clone(), a)
+                a.lineAlignment = cn.Center, a.alignment = this.toAlignment(r), a.trimming = Ru.None, a.formatFlags |= Td.NoWrap, e.drawString(s, o, l, t.clone(), a)
             }
             static measureText(e, t, r) {
                 if (B.isNullOrWhiteSpace(t)) return 0;
                 let i = U.Table.Font.getGdiFont(e, null, r);
                 return Vu.measureString(null, t, i).width
             }
             static calculateIndicatorRect(t, e, r, i) {
@@ -14946,15 +14963,15 @@
                         break
                     }
                 }
                 return t.inflate(-4 * r, -4 * r), t
             }
             static getCellText(e, t, r) {
                 if (null == r) return "";
-                return ts.formatAsPercentage2(e.report, t.textFormat, r)
+                return rs.formatAsPercentage2(e.report, t.textFormat, r)
             }
             static calculateTextRect(e, t) {
                 let r = e.width / 4;
                 switch (this.getHorAlignment(t)) {
                     case z.Left:
                         return new j(e.x + r, e.y, e.width - r, e.height);
                     case z.Right:
@@ -14967,47 +14984,47 @@
             static getColor(e, t, r) {
                 if (!N.transparent.equals(e.foreColor)) return e.foreColor;
                 if (0 < t) return r.cellIndicatorPositive;
                 if (t < 0) return r.cellIndicatorNegative;
                 return r.cellIndicatorNeutral
             }
             static toAlignment2(e) {
-                if (e[L.System.StiObject.stimulsoft]().is(mn)) return e;
+                if (e[L.System.StiObject.stimulsoft]().is(cn)) return e;
                 let t = e[L.System.StiObject.stimulsoft]().as(Cr);
-                if (null == t) return mn.Center;
+                if (null == t) return cn.Center;
                 return this.toAlignment(t.horAlignment)
             }
             static toAlignment(e) {
                 switch (e) {
                     case z.Left:
-                        return mn.Near;
+                        return cn.Near;
                     case z.Center:
-                        return mn.Center;
+                        return cn.Center;
                     case z.Right:
-                        return mn.Far
+                        return cn.Far
                 }
-                return mn.Center
+                return cn.Center
             }
             static getHorAlignment(e) {
                 let t = e;
                 return null != t ? t.horAlignment : z.Right
             }
         }, F.C.StiIndicatorCellPainter),
         vd = L.Data.Engine.StiDataSortRuleHelper;
     {
         class tg {
             static getBackgroundColor(e, t) {
                 return t ? e.alternatingCellBackColor : e.cellBackColor
             }
             static measureColumn(e, t, r, i, s) {
                 let n, l = U.Table.getHeight(r.font, r.zoom);
-                if (i.is2($i)) n = this.measureSparklinesCell(r, 0, r.zoom);
-                else if (i.is2(Qi)) n = this.measureIndicatorCell(e, r, i, s, r.zoom);
-                else if (i.is2(_i)) n = this.measureDataBarsCell(e, r, i, s, r.zoom);
-                else if (i.is2(Gi)) n = this.measureBubbleCell(e, r, i, s, r.zoom);
+                if (i.is2(es)) n = this.measureSparklinesCell(r, 0, r.zoom);
+                else if (i.is2(qi)) n = this.measureIndicatorCell(e, r, i, s, r.zoom);
+                else if (i.is2($i)) n = this.measureDataBarsCell(e, r, i, s, r.zoom);
+                else if (i.is2(Xi)) n = this.measureBubbleCell(e, r, i, s, r.zoom);
                 else if (Bu.isImage(s)) return new W(0, U.Table.getHeight(r.font, r.zoom));
                 return new W(n.width, Math.max(n.height, l))
             }
             static getArrowSize(e, t) {
                 let r = U.Table.getHeight(e.headerFont, e.zoom),
                     i = vd.getSortDirection(e.userSorts, t.key);
                 if (i != mh.None) return new W(1.5 * r, r);
@@ -15024,29 +15041,29 @@
             static measureIndicatorCell(e, t, r, i, s) {
                 let n = r,
                     l = Fd.getCellText(t, n, V.tryToNullableNumber(i)),
                     a = this.measureCell2(e, l, t.font, r);
                 return a.width = (a.width + 4) * s * 1.25, a
             }
             static measureDataBarsCell(e, t, r, i, s) {
-                let n = ts.formatBasedOnColumnType(t, r, i),
+                let n = rs.formatBasedOnColumnType(t, r, i),
                     l = this.measureCell2(e, n, t.font, r);
-                return l.width *= s, r.horAlignment != z.Center && (l.width *= 2), r.is(_i) && 0 < r.width && (l.width = s * r.width), l
+                return l.width *= s, r.horAlignment != z.Center && (l.width *= 2), r.is($i) && 0 < r.width && (l.width = s * r.width), l
             }
             static measureBubbleCell(r, i, s, n, e) {
                 let l = U.Table.getHeight(i.font, i.zoom);
                 if (s.horAlignment == z.Center) return l -= 2, new W(l, U.Table.getHeight(i.font));
                 {
-                    let e = ts.formatBasedOnColumnType(i, s, n),
+                    let e = rs.formatBasedOnColumnType(i, s, n),
                         t = this.measureCell2(r, e, i.font, s);
                     return t.width += l, t
                 }
             }
             static measureCommonCell(e, t, r, i, s, n) {
-                let l = ts.formatBasedOnColumnType(t, r, i),
+                let l = rs.formatBasedOnColumnType(t, r, i),
                     a = new W(s, 0);
                 return Bu.isImage(l) || ((a = this.measureCell2(e, l, t.font, r)).width *= n, a.height *= n), a
             }
             static measureHeader(e, t) {
                 return this.measureHeader2(null, e, t)
             }
             static measureHeader2(e, t, r) {
@@ -15088,22 +15105,22 @@
         }
         tg.captionSizeCache = new xo, F.q.StiTableElementGdiPainter = tg
     }
     let Ad = L.System.Drawing.SolidBrush,
         Id = (F.C.StiBubbleCellPainter = class {
             static draw(s, e, t, n, r, l, i, a, o, u, h = !0) {
                 if (0 == l) return;
-                let m = ts.formatBasedOnColumnType(t, n, l),
+                let m = rs.formatBasedOnColumnType(t, n, l),
                     c = (0 < i && (i = 0), a < 0 && (a = 0), n.horAlignment),
                     d = e,
                     g = (d.inflate(-2, -2), this.calculateTextRect(t, d, n)),
                     p = (d = this.calculateBubbleRect(t, d, n, Math.abs(l), i, a), J.getTableStyle(t)),
                     S = this.getForeColor(t, n, p, o, u);
                 if (h && c != z.Center && s.drawString(m, t.font, S, g, null), 0 < d.width && 0 < d.height) {
-                    let e = n.as(Gi),
+                    let e = n.as(Xi),
                         t = e.allowCustomColors ? e.positiveColor : p.cellDataBarsPositive,
                         r = e.allowCustomColors ? e.negativeColor : p.cellDataBarsNegative,
                         i = new Ad(l < 0 ? r : t);
                     s.fillEllipse(d, i)
                 }
             }
             static getForeColor(e, t, r, i, s) {
@@ -15140,15 +15157,15 @@
                             r = new Ve(r.x + e, r.y, r.width - e, r.height);
                             break
                     }
                 }
                 return r.inflate(-2, -2), r
             }
             static getCellText(e, t, r) {
-                return ts.formatBasedOnColumnType(e, t, r)
+                return rs.formatBasedOnColumnType(e, t, r)
             }
         }, F.C.StiColorScaleCellPainter = class {
             static getScaleColor(t, r, i, e, s, n) {
                 let l = (i - r) / 2,
                     a = (t = Math.min(t, i), t = Math.max(t, r), 0),
                     o, u, h = e.cellBackColor;
                 if (l < t) {
@@ -15166,15 +15183,15 @@
             }
         }, F.K.StiTableElementConditionHelper),
         Dd = F.K.StiDataBarsDirection,
         Rd = F.K.StiDataBarsBrushType,
         Ed = L.Base.Drawing.StiGradientBrush,
         Od = (F.C.StiDataBarsCellPainter = class {
             static async draw(e, t, r, i, s, n, l, a, o, u, h, m, c = !0, d = Dd.LeftToRight, g = Rd.Solid) {
-                let p = ts.formatBasedOnColumnType(r, n, a);
+                let p = rs.formatBasedOnColumnType(r, n, a);
                 await this.draw2(e, t, a, o, u, l, p, r, i, s, n, h, m, c, d, g)
             }
             static async draw2(s, e, n, t, r, i, l, a, o, u, h, m, c, d = !0, g = Dd.LeftToRight, p = Rd.Solid) {
                 if (null == n || 0 == n) return;
                 let S = h,
                     w = (B.isNullOrWhiteSpace(S.minimum) || (t = V.tryToNumber(O.parse2(S.minimum, a.report))), B.isNullOrWhiteSpace(S.maximum) || (r = V.tryToNumber(O.parse2(S.maximum, a.report))), t = Math.min(t, 0), !1),
                     b = ((r = Math.max(r, 0)) < n && (w = !0, n = r), n < t && (w = !0, n = t), h.horAlignment),
@@ -15251,15 +15268,15 @@
                         break
                 }
                 return e.inflate(-2, -2), e
             }
         }, F.C.StiSparklinesCellPainter = class {
             static draw(e, t, r, i, s) {}
             static castToArray(e) {
-                return Ln.isArray(e) ? e : null
+                return Bn.isArray(e) ? e : null
             }
         }, F.C.StiTableColumnSizeHelper = class {
             getUniqueCode() {
                 let e = 0;
                 return e = 397 * (e = 397 * (e = 397 * (e = 397 * e ^ this.Width) ^ this.MinWidth) ^ this.MaxWidth) ^ this.WordWrap[L.System.StiObject.stimulsoft]().getHashCode(), Math.abs(e)
             }
             getColumnWidth(e, t = !1) {
@@ -15269,21 +15286,21 @@
             }
             getColumnHeight(e) {
                 if (!this.IsMeasurable) return e;
                 if (this.MaxHeight < e) return this.MaxHeight;
                 return e
             }
             static isWordWrap(e) {
-                let t = e.as(mi);
+                let t = e.as(ci);
                 if (null == (null == t ? void 0 : t.size)) return !1;
                 return t.size.wordWrap
             }
             constructor(e, t) {
                 this.Width = 0, this.MinWidth = 30, this.MaxWidth = 300, this.MaxHeight = 0, this.WordWrap = !1, this.FontUniqueCode = 0, this.IsMeasurable = !1;
-                let r = (this.Column = t).as(mi);
+                let r = (this.Column = t).as(ci);
                 if (null == (null == r ? void 0 : r.size)) return;
                 this.IsMeasurable = !0, this.FontUniqueCode = e.getHashCode();
                 let i = r.size;
                 this.Width = i.width, this.MinWidth = i.minWidth, this.MaxWidth = i.maxWidth, this.MaxHeight = i.wordWrap ? Number.MAX_VALUE : Math.round(e.getHeight()) + 1, this.WordWrap = i.wordWrap
             }
         }, F.y.IStiSizeExportSettings = new L.System.Interface("IStiSizeExportSettings"), L.Report.Dashboard.IStiControlElement),
         Vd = F.p.StiLocHelper,
@@ -15324,20 +15341,20 @@
                         let t = -1 != m ? e[m] : null,
                             r = -1 != c ? e[c] : null;
                         null == t && null == r || (w = (t || r).toString())
                     } if (this.renderElement(s, i, n, this.format(i.as(Od), w)), p.selectionMode == gl.Multi && !d) {
                     let t = n;
                     if (S.userFilters.any()) {
                         let r = S.userFilters;
-                        if (r.all(e => e.condition == Zi.NotEqualTo)) {
+                        if (r.all(e => e.condition == Yi.NotEqualTo)) {
                             r = new P;
                             for (let e of o.rows) {
                                 let t = null == (l = e[1]) ? void 0 : l[L.System.StiObject.stimulsoft]().toString();
                                 if (S.userFilters.any(e => e.value == t)) continue;
-                                r.add(new f(null, null, Zi.EqualTo, t))
+                                r.add(new f(null, null, Yi.EqualTo, t))
                             }
                         }
                         for (let e of r) {
                             if (!(t.x + t.width <= n.x + n.width)) {
                                 while (1 < s.components.count) s.components.removeAt(1);
                                 this.renderItem(s, i, n, B.format(b.get("Dashboard", "NSelected"), S.userFilters.length));
                                 break
@@ -15405,15 +15422,15 @@
                     e.name = t.name + `_Content`, e.allowHtmlTags = !0, e.vertAlignment = Wt.Center, e.textBrush = new v(a), e.brush = new v(o), e.text = this.getDateTimeString(n, l), e.font = n.font, r.components.add(e), null != this.storedCulture && (ni.currentCulture = this.storedCulture)
                 }
             }
             getDateTimeString(r, e) {
                 var t, i;
                 let s = Nd.getDefaultValue(r);
                 if (El.isVariableSpecifiedAsExpression(r, null == (t = null == r ? void 0 : r.valueMeter) ? void 0 : t.expression)) {
-                    let e = null == (i = Nd.getVariableSpecifiedAsValue(r)) ? void 0 : i.as(zs);
+                    let e = null == (i = Nd.getVariableSpecifiedAsValue(r)) ? void 0 : i.as(Gs);
                     if (Al.isRangeType(null == e ? void 0 : e.type) && r.initialRangeSelectionSource == xl.Selection) {
                         let e = {
                                 ref: null
                             },
                             t = {
                                 ref: null
                             };
@@ -15467,15 +15484,15 @@
                 0 < o.components.count && (h += o.getComponentsList()[L.System.StiObject.stimulsoft]().toList().min(e => e.top));
                 while (1) {
                     let e = o.getComponentsList(),
                         i = 0;
                     for (let r of e) {
                         let e = r.bottom,
                             t = r.left;
-                        r.is(jd) && (e += U.ListBox.ItemHeight / 3), null != a ? (a.orientation == Ys.Vertical && e <= s.height || a.orientation == Ys.Horizontal && t <= s.width || 0 == i) && (o.components.remove(r), s.components.add(r)) : e <= s.height && (o.components.remove(r), s.components.add(r)), i++
+                        r.is(jd) && (e += U.ListBox.ItemHeight / 3), null != a ? (a.orientation == Ks.Vertical && e <= s.height || a.orientation == Ks.Horizontal && t <= s.width || 0 == i) && (o.components.remove(r), s.components.add(r)) : e <= s.height && (o.components.remove(r), s.components.add(r)), i++
                     }
                     if (r.renderSinglePage || 0 == o.components.count) break;
                     let t = o.getComponentsList()[L.System.StiObject.stimulsoft]().toList().min(e => e.top);
                     o.getComponentsList().forEach(e => e.top = e.top - t + 1), n.renderedPages.count <= ++u && n.renderedPages.add(l.clone(!0, !1)), l = n.renderedPages.getByIndex(u), s = s.clone(!0, !1), r.renderSingleElement ? (s.top = 0, s.left = 0) : s.top = h, l.components.add(s)
                 }
                 for (let e of s.report.renderedPages.list) e.getComponentsList().forEach(e => {
                     e.report = n, e.page = l
@@ -15483,16 +15500,16 @@
             }
             static getCheckStyle(e, t) {
                 let r = e,
                     i = e.is(pm) && e.as(pm).selectionMode == gl.One && e.as(pm).selectionType == so.RadioButton,
                     s = i ? Pd.DotCircle : Pd.CheckRectangle,
                     n = i ? Pd.NoneCircle : Pd.NoneRectangle;
                 if (!r.userFilters.any()) return i ? n : s;
-                if (r.userFilters.any(e => e.condition == Zi.IsFalse)) return n;
-                if (r.userFilters.any(e => e.condition == Zi.EqualTo && e.value == (null == t ? void 0 : t.toString()))) return s;
+                if (r.userFilters.any(e => e.condition == Yi.IsFalse)) return n;
+                if (r.userFilters.any(e => e.condition == Yi.EqualTo && e.value == (null == t ? void 0 : t.toString()))) return s;
                 return n
             }
             async renderItems(i, s, n) {
                 let e = await bl.tryToGetOrCreate(n);
                 if (null == e) return;
                 let t = n,
                     l = Ld.fetchItems(t, e, t.showBlanks);
@@ -15505,26 +15522,26 @@
             }
             renderItems2(s, n, l, a, o, u) {
                 var e;
                 let h = l,
                     m = h.selectionMode == gl.Multi,
                     c = h.selectionMode == gl.One && l.is(pm) && l.as(pm).selectionType == so.RadioButton,
                     d = m || c,
-                    g = l.is(lo) && l.orientation == Ys.Horizontal,
+                    g = l.is(lo) && l.orientation == Ks.Horizontal,
                     p = (null == (e = h[L.System.StiObject.stimulsoft]().as(ar)) ? void 0 : e.font) || new H("Arial", 8),
                     S = l,
                     w = g ? this.getHorizontalItemAutoWidth(h, p, a, n.width, d) : n.width,
                     b = g ? n.height : U.ListBox.ItemHeight,
                     f = n.x,
                     y = n.y;
                 if (h.showAllValue) {
                     g && 0 == w && (w = this.measureItemWidth(Vd.locAll, p, d));
                     let e = new j(f, y, w, b),
                         t = c ? Pd.DotCircle : Pd.CheckRectangle;
-                    S.userFilters.any() && (t = c ? Pd.NoneCircle : S.userFilters.any(e => e.condition == Zi.IsFalse) ? Pd.NoneRectangle : Pd.DotRectangle), this.renderItem(s, e, l, Vd.locAll, t, g ? G.Right : G.Bottom, m, c, !1), g ? f += w + 1 : y += b + 1
+                    S.userFilters.any() && (t = c ? Pd.NoneCircle : S.userFilters.any(e => e.condition == Yi.IsFalse) ? Pd.NoneRectangle : Pd.DotRectangle), this.renderItem(s, e, l, Vd.locAll, t, g ? G.Right : G.Bottom, m, c, !1), g ? f += w + 1 : y += b + 1
                 }
                 if (null != a) {
                     let i = 0;
                     for (let r = 0; r < a.count2(); r++) {
                         g && 0 == w && (w = this.measureItemWidth(a[r], p, d));
                         let e = new j(f + i, y, w - i, b),
                             t = o[r];
@@ -15544,29 +15561,29 @@
                     s = oh.measureString(e, i, 1e6),
                     n = s.width;
                 return r && (n += U.ListBox.CheckBoxWidth), n
             }
             renderItem(t, r, i, e, s, n, l, a, o) {
                 var u;
                 if (l || a) {
-                    let e = i.is(lo) && i.orientation == Ys.Horizontal;
+                    let e = i.is(lo) && i.orientation == Ks.Horizontal;
                     op.renderCheckControl(t, r.clone(), i, s, e ? G.None : n, a), r.x += U.ListBox.CheckBoxWidth, r.width -= U.ListBox.CheckBoxWidth
                 }
                 let h = J.getForeColor(i),
                     m = J.getBackColor(i, null, !0),
                     c = (null == (u = i[L.System.StiObject.stimulsoft]().as(ar)) ? void 0 : u.font) || new H("Arial", 8),
                     d = this.format(i.as(Od), e),
                     g = new Du(r),
-                    p = (g.name = i.name + `_Item`, g.allowHtmlTags = !0, g.margins = l || a ? new be(1, 0, 0, 0) : be.empty, g.border = n != G.None ? new ie(n, N.gray, 1, Ri.Solid) : new ie(G.None, N.transparent, 0, Ri.None), g.brush = new v(m), g.horAlignment = X.Left, g.vertAlignment = Wt.Center, g.text = d, g.textBrush = new v(h), g.wordWrap = !1, g.font = c, i.as(Od));
+                    p = (g.name = i.name + `_Item`, g.allowHtmlTags = !0, g.margins = l || a ? new be(1, 0, 0, 0) : be.empty, g.border = n != G.None ? new ie(n, N.gray, 1, Ei.Solid) : new ie(G.None, N.transparent, 0, Ei.None), g.brush = new v(m), g.horAlignment = X.Left, g.vertAlignment = Wt.Center, g.text = d, g.textBrush = new v(h), g.wordWrap = !1, g.font = c, i.as(Od));
                 null == p || p.textFormat.is(Jt) || (g.excelDataValue = d), t.components.add(g)
             }
             static renderCheckControl(e, t, r, i, s, n) {
                 let l = J.getForeColor(r),
                     a = (t = new j(t.x, t.y, U.ListBox.CheckBoxWidth, t.height), new Bd(t));
-                a.name = r.name + `_ItemCheckBox`, a.border = s != G.None ? new ie(s, N.gray, 1, Ri.Solid) : new ie(G.None, N.transparent, 0, Ri.None), a.contourColor = N.transparent, a.textBrush = new v(l), a.checkStyleForTrue = i, a.checkStyleForFalse = n ? Pd.NoneCircle : Pd.NoneRectangle, a.checkedValue = i != Pd.NoneRectangle && i != Pd.NoneCircle, e.components.add(a)
+                a.name = r.name + `_ItemCheckBox`, a.border = s != G.None ? new ie(s, N.gray, 1, Ei.Solid) : new ie(G.None, N.transparent, 0, Ei.None), a.contourColor = N.transparent, a.textBrush = new v(l), a.checkStyleForTrue = i, a.checkStyleForFalse = n ? Pd.NoneCircle : Pd.NoneRectangle, a.checkedValue = i != Pd.NoneRectangle && i != Pd.NoneCircle, e.components.add(a)
             }
         }
         F.A.StiListBoxElementExportTool = op
     }
     let Hd = L.Report.Components.StiVerticalLinePrimitive,
         zd = L.Report.Components.StiFlowchartSortShapeType;
     {
@@ -15734,15 +15751,15 @@
                         }
                     }
                 }
                 null != u && (u.width = d.right - d.left + 1, a.add(u)), null != h && (h.width = a.max(e => e.x) - d.right, a.add(h));
                 let g = J.getPivotTableStyle(t),
                     p = a.max(e => e.y) + 1,
                     S = a.max(e => e.x) + 1,
-                    w = Ln.create2(Kh, S, p);
+                    w = Bn.create2(Kh, S, p);
                 for (let i of a)
                     if (w[i.x][i.y] = i.cell, i.cell.width = i.width, i.cell.height = i.height, 0 <= i.cellRow)
                         for (l = i.y; l < i.y + i.height; l++) {
                             let r = d.right + 1;
                             for (let e = i.width; e < n.length; e++)
                                 if (0 <= o.indexOf(e)) {
                                     w[r++][l] = n[e][i.cellRow + l - i.y], w[r - 1][l].field.border.side = e == n.length - 1 ? G.None : G.Right;
@@ -15750,22 +15767,22 @@
                                     if (null != t && null != t.field && t.field.brush.is(v)) {
                                         let e = t.field.brush.color;
                                         (e.equals(g.alternatingCellBackColor) || e.equals(g.cellBackColor)) && (t.field.brush = new v(l % 2 != 0 ? g.alternatingCellBackColor : g.cellBackColor), t.field.textBrush = new v(l % 2 != 0 ? g.alternatingCellForeColor : g.cellForeColor))
                                     }
                                     null != t && null != t.field && (t.field.brush = null != t.field.conditionBrush ? t.field.conditionBrush : t.field.brush, t.field.textBrush = null != t.field.conditionTextBrush ? t.field.conditionTextBrush : t.field.textBrush)
                                 }
                         }
-                n = Ln.create2(Kh, S, 0);
+                n = Bn.create2(Kh, S, 0);
                 for (let t = 0; t < S; t++) {
-                    n[t] = Ln.create(Kh, p);
+                    n[t] = Bn.create(Kh, p);
                     for (let e = 0; e < p; e++) n[t][e] = null != w[t][e] ? w[t][e] : new Kh, null != n[t][e].field && t == S - 1 && (n[t][e].field.border.side |= G.Top), 0 < e && (n[t][e].parentCell = n[t][e])
                 }
-                let b = Ln.create(Number, p),
-                    f = Ln.create(Number, S);
-                Ln.copy(e.crossTabInfo.cross.heights, 0, b, p), Ln.copy(e.crossTabInfo.cross.widths, 0, f, S), e.crossTabInfo.cross.cells = n, e.crossTabInfo.cross.widths = f, e.crossTabInfo.cross.heights = b, e.crossTabInfo.cross.doAutoSize()
+                let b = Bn.create(Number, p),
+                    f = Bn.create(Number, S);
+                Bn.copy(e.crossTabInfo.cross.heights, 0, b, p), Bn.copy(e.crossTabInfo.cross.widths, 0, f, S), e.crossTabInfo.cross.cells = n, e.crossTabInfo.cross.widths = f, e.crossTabInfo.cross.heights = b, e.crossTabInfo.cross.doAutoSize()
             }
             static renderCells(e, t, r, i, s, n) {
                 s.page.unlimitedHeight = !0, e.canBreak = !0, e.dockStyle = Wd.None;
                 let l = new Ud,
                     a = (l.startColumn = 0, l.startRow = 0, l.destinationContainer = e, l.destinationRectangle = r, l.forceNoBreak = n, new Jd);
                 a.renderCrossTabUnlimitedBreakable(l, s, e, t.clone())
             }
@@ -15848,31 +15865,31 @@
                 let m = e.as(ym);
                 if (null == m) return null;
                 let c = await bl.getOrCreate(m);
                 if (null == c) return null;
                 let d = 1,
                     g = [],
                     p = U.Table.getHeight(m.font, d),
-                    S = c.meters.where(e => e.is(Cs)).cast(),
+                    S = c.meters.where(e => e.is(xs)).cast(),
                     t = null != S.firstOrDefault(e => e.showTotalSummary),
                     w = (delete m.cacheStyle, 0);
                 for (let u of S) {
                     u.cache = {};
                     let e = await this.getColumnVisibilityState(u, m.report);
                     if (!e) {
                         w++;
                         continue
                     }
                     let n = cp.measureHeader(m, u, d);
-                    if (u.is($i)) n = cp.measureSparklinesCell(d, n);
+                    if (u.is(es)) n = cp.measureSparklinesCell(d, n);
                     else {
                         for (let r of c.rows) {
                             let e = r[w],
                                 t;
-                            t = u.is2(Qi) ? cp.measureIndicatorCell(m, u, d, e) : u.is2(_i) ? cp.measureDataBarsCell(m, u, d, e) : cp.measureCommonCell(m, u, d, e, n).width, n = Math.max(n, t)
+                            t = u.is2(qi) ? cp.measureIndicatorCell(m, u, d, e) : u.is2($i) ? cp.measureDataBarsCell(m, u, d, e) : cp.measureCommonCell(m, u, d, e, n).width, n = Math.max(n, t)
                         }
                         if (u.showTotalSummary) {
                             let e = rg.calculateTotal(u, w, c),
                                 t = this.measureFooter(m, u, d, e);
                             n = Math.max(n, t)
                         }
                     }
@@ -15891,41 +15908,41 @@
                         }
                         if ("boolean" == typeof t) i["boolValue"] = t;
                         else
                             for (let e of r.components.list)
                                 if (e.is(Du)) {
                                     if (i["text"] = e.text, i["textColor"] = Tu.toHtml(Se.toColor(e.textBrush)), i["backColor"] = Tu.toHtml(Se.toColor(e.brush)), i["textWidth"] = e.width, i["textHeight"] = e.height, 0 < m.tableConditions.length) {
                                         let e = null == (h = m.as(ar)) ? void 0 : h.font,
-                                            t = 0 < m.tableConditions.length ? await Id.processFontStyle(e, u.key, m, s, S.select(e => e.key)) : hn.Regular,
+                                            t = 0 < m.tableConditions.length ? await Id.processFontStyle(e, u.key, m, s, S.select(e => e.key)) : mn.Regular,
                                             r = (e = new H(e.fontFamily.name, e.size, t), {});
                                         r["bold"] = e.bold, r["italic"] = e.italic, r["underline"] = e.underline, r["strikeout"] = e.strikeout, i["textFontStyle"] = r
                                     }
                                     null != t && t.toString() != i["text"] && (i["value"] = t.toString())
                                 } else e.is(ad) ? (i["image"] = null != e.imageToDraw ? L.Base.Drawing.StiImageConverter.imageToString(e.imageToDraw) : null, i["imageWidth"] = e.width, i["imageHeight"] = e.height) : e.is(_d) && (i["sparkline"] = L.Report.Export.StiHtmlExportService.getSparklineData(null, e, e.width, e.height), i["sparklineWidth"] = e.width, i["sparklineHeight"] = e.height);
                         null == i["boolValue"] && null == i["text"] && null == i["image"] && (i["text"] = t), g[o].push(i), o++
                     }
                     if (t) {
                         g.length < c.rows.length + 1 && g.push([]);
                         let t = {};
                         if (t["text"] = "", u.showTotalSummary) {
                             let e = rg.calculateTotal(u, w, c);
-                            t["text"] = u.summaryType == Kr.Count ? ae.trunc(e).toString() : ts.formatBasedOnColumnType(m, u, e)
+                            t["text"] = u.summaryType == Kr.Count ? ae.trunc(e).toString() : rs.formatBasedOnColumnType(m, u, e)
                         }
                         g[g.length - 1].push(t)
                     }
                     w++
                 }
                 return g
             }
             static async renderCells(u, h, m, c, d, g, i) {
                 let p = await bl.tryToGetOrCreate(m);
                 if (null == p) return;
                 let t = U.Table.getHeight(m.headerFont, c),
                     e = U.Table.getHeight(m.font, c),
-                    S = p.meters.where(e => e.is(Cs)).cast(),
+                    S = p.meters.where(e => e.is(xs)).cast(),
                     r = null != S.firstOrDefault(e => e.showTotalSummary),
                     s = i ? 0 : m.currentPageIndex,
                     n = 0 != m.rowsPerPage && -1 != s,
                     l = 1,
                     w = (n && (l = Yd.getNumberOfPages(p.rows.length, m.rowsPerPage)) <= 1 && (n = !1), p.rows);
                 if (n) {
                     let e = w.skip(m.rowsPerPage * s).take(m.rowsPerPage);
@@ -15954,21 +15971,21 @@
                         let n = e;
                         x = -1;
                         for (let s of S) {
                             x++;
                             let e = await Kd.getVisible(s, m.report);
                             if (!e) continue;
                             let i = y[x];
-                            if (s.is($i)) i = this.measureSparklinesCell(c, i);
+                            if (s.is(es)) i = this.measureSparklinesCell(c, i);
                             else {
                                 let t = l[x],
                                     r;
-                                if (s.is2(Qi)) r = this.measureIndicatorCell(m, s, c, t);
-                                else if (s.is2(_i)) r = this.measureDataBarsCell(m, s, c, t);
-                                else if (s.is2(Gi)) r = cp.measureBubbleCell(m, s, c, t);
+                                if (s.is2(qi)) r = this.measureIndicatorCell(m, s, c, t);
+                                else if (s.is2($i)) r = this.measureDataBarsCell(m, s, c, t);
+                                else if (s.is2(Xi)) r = cp.measureBubbleCell(m, s, c, t);
                                 else {
                                     let e = this.measureCommonCell(m, s, c, t, i);
                                     r = e.width, n = Math.max(e.height, n)
                                 }
                                 i = Math.max(i, r)
                             }
                             y[x] = i
@@ -15981,16 +15998,16 @@
                     let t = h.width / y.sum(),
                         e = ((1 < t || !i) && (y = y.select(e => e * t).toList()), -1);
                     for (let n of w) {
                         if (++e >= C.length) break;
                         x = -1;
                         let s = C[e];
                         for (let i of S) {
-                            if (x++, i.is2(Qi) || i.is2(_i)) continue;
-                            if (i.is(mi)) {
+                            if (x++, i.is2(qi) || i.is2($i)) continue;
+                            if (i.is(ci)) {
                                 let e = i,
                                     t = e.size.width,
                                     r = (e.size.width = y[x] - 4, this.measureCommonCell(m, i, c, n[x], e.size.width));
                                 s = Math.max(r.height, s), e.size.width = t
                             }
                         }
                         C[e] = s
@@ -16036,67 +16053,67 @@
             static measureSparklinesCell(e, t) {
                 return Math.max(t, 80 * e)
             }
             static measureHeader(e, t, r) {
                 return tg.measureHeader(e, t).width * r
             }
             static measureFooter(e, t, r, i) {
-                let s = ts.formatBasedOnColumnType(e, t, i);
+                let s = rs.formatBasedOnColumnType(e, t, i);
                 return tg.measureCell(s, e.footerFont, t).width * r
             }
             static measureIndicatorCell(e, t, r, i) {
-                let s = t.as(Qi),
+                let s = t.as(qi),
                     n = Fd.getCellText(e, s, V.tryToNullableNumber(i)),
                     l = tg.measureCell(n, e.font, t).width * r;
                 return l *= 1.25
             }
             static measureDataBarsCell(e, t, r, i) {
-                let s = ts.formatBasedOnColumnType(e, t, i),
+                let s = rs.formatBasedOnColumnType(e, t, i),
                     n = tg.measureCell(s, e.font, t).width * r;
-                return t.horAlignment != z.Center && (n *= 2), n = t.is(_i) && 0 < t.width ? r * t.width : n
+                return t.horAlignment != z.Center && (n *= 2), n = t.is($i) && 0 < t.width ? r * t.width : n
             }
             static measureBubbleCell(e, t, r, i) {
-                let s = ts.formatBasedOnColumnType(e, t, i),
+                let s = rs.formatBasedOnColumnType(e, t, i),
                     n = tg.measureCell(s, e.font, t).width * r,
                     l = U.Table.getHeight(e.font, r);
                 if (t.horAlignment == z.Center) return l;
                 return n += l
             }
             static measureCommonCell(e, t, r, i, s) {
                 if (Bu.isImage(i)) return new W(s, 0);
-                let n = ts.formatBasedOnColumnType(e, t, i),
+                let n = rs.formatBasedOnColumnType(e, t, i),
                     l = tg.measureCell(n, e.font, t);
                 return l.width *= r, l.height *= r, l
             }
             static renderHeader(e, t, r, i, s, n, l) {
                 let a = null != i ? Nh.getLabel(i) : "",
                     o = B.isNullOrWhiteSpace(a) ? r.name + `_Column` : eg.correctName(a),
                     u = J.getTableStyle(r),
                     h = 0 != r.columns.indexOf(i) && t.left < e.width && !l,
                     m = r.columns.indexOf(i) != r.columns.length - 1 && t.right <= e.width && !l,
                     c = (h ? G.Left : G.None) | (m ? G.Right : G.None),
                     d = l ? N.black : this.getHeaderForeColor(r),
                     g = l ? N.transparent : u.headerBackColor,
-                    p = l ? new H("Arial", 10, hn.Bold) : r.headerFont,
+                    p = l ? new H("Arial", 10, mn.Bold) : r.headerFont,
                     S = new Du(t);
-                S.name = o, S.allowHtmlTags = !0, S.autoWidth = !1, S.horAlignment = this.getHeaderAlignment(i), S.vertAlignment = Wt.Center, S.wordWrap = !1, S.border = new ie(c, u.lineColor, 1, Ri.Solid), S.brush = new v(g), S.font = U.Table.Font.getGdiFont(s, null, p), S.text = a, S.textFormat = null != i.textFormat ? i.textFormat.clone() : null, S.textBrush = new v(d), S.componentPlacement = `h.` + r.name, e.components.add(S)
+                S.name = o, S.allowHtmlTags = !0, S.autoWidth = !1, S.horAlignment = this.getHeaderAlignment(i), S.vertAlignment = Wt.Center, S.wordWrap = !1, S.border = new ie(c, u.lineColor, 1, Ei.Solid), S.brush = new v(g), S.font = U.Table.Font.getGdiFont(s, null, p), S.text = a, S.textFormat = null != i.textFormat ? i.textFormat.clone() : null, S.textBrush = new v(d), S.componentPlacement = `h.` + r.name, e.components.add(S)
             }
             static getHeaderAlignment(e) {
                 if (e.headerAlignment == z.Left) return X.Left;
                 if (e.headerAlignment == z.Right) return X.Right;
                 return X.Center
             }
             static renderFooter(e, t, r, i, s, n, l) {
                 let a = J.getTableStyle(r),
                     o = this.getFooterForeColor(r),
                     u = a.footerColor,
                     h = r.footerFont,
                     m = "",
                     c = 0,
-                    d = (i.showTotalSummary && (c = rg.calculateTotal(i, s, l), m = i.summaryType == Kr.Count ? ae.trunc(c).toString() : ts.formatBasedOnColumnType(r, i, c)), X.Right),
+                    d = (i.showTotalSummary && (c = rg.calculateTotal(i, s, l), m = i.summaryType == Kr.Count ? ae.trunc(c).toString() : rs.formatBasedOnColumnType(r, i, c)), X.Right),
                     g = (i.summaryAlignment == z.Left ? d = X.Left : i.summaryAlignment == z.Center && (d = X.Center), new Du(t)),
                     p = (g.name = r.name + `_FooterCell`, null != i.textFormat && i.textFormat.is(Jt) ? null : m);
                 null != i.textFormat && (i.textFormat.is(Jr) || i.textFormat.is(Wr) || i.textFormat.is(Ur)) && (p = c.toString()), g.border = this.getBorderSides(e, t, r, i, G.All), g.brush = new v(u), g.excelDataValue = p, g.font = U.Table.Font.getGdiFont(n, null, h), g.horAlignment = d, g.vertAlignment = Wt.Center, g.text = m, g.textBrush = new v(o), g.textFormat = null != i.textFormat ? i.textFormat.clone() : null, g.wordWrap = !1, g.componentPlacement = `f.` + r.name, e.components.add(g)
             }
             static renderCurrentPageNumber(e, t, r, i, s) {
                 let n = J.getTableStyle(r),
                     l = this.getFooterForeColor(r),
@@ -16105,58 +16122,58 @@
                     u = new Du(t);
                 u.name = r.name + `_CurrentPage`, u.brush = new v(a), u.font = U.Table.Font.getGdiFont(i, null, o), u.horAlignment = X.Center, u.vertAlignment = Wt.Center, u.margins = new be(0, 0, 1, 0), u.textQuality = ag.Typographic, u.text = s, u.textBrush = new v(l), u.wordWrap = !1, u.componentPlacement = `f.` + r.name, e.components.add(u)
             }
             static async renderCell(e, t, r, i, s, n, l, a, o, u, h, m, c) {
                 let d = J.getTableStyle(r),
                     g = this.getForeColor(r, n, d, h),
                     p = tg.getBackgroundColor(d, null != h && h);
-                p = 0 < r.tableConditions.length ? await Id.processBackColor(p, n.key, r, i, s) : p, c ? await this.renderTextCell(e, t, r, i, s, n, l, a, G.None, N.black, N.transparent, m, !0) : n.is2(_i) || n.is2($i) || n.is2(Qi) || n.is2(Gi) ? await this.renderGraphicCell(e, t, r, i, s, n, l, a, o, u, p, d, null != h && h, m) : n.is2(qi) ? await this.drawColorScaleColumn(e, t, r, i, s, n, l, a, o, u, d, m) : Bu.isImage(a) ? this.renderImageCell(e, t, r, n, a, p, m) : "boolean" == typeof a ? await this.renderBoolCell2(e, t, r, i, s, n, l, a, g, p, m) : await this.renderTextCell(e, t, r, i, s, n, l, a, G.All, g, p, m, !1)
+                p = 0 < r.tableConditions.length ? await Id.processBackColor(p, n.key, r, i, s) : p, c ? await this.renderTextCell(e, t, r, i, s, n, l, a, G.None, N.black, N.transparent, m, !0) : n.is2($i) || n.is2(es) || n.is2(qi) || n.is2(Xi) ? await this.renderGraphicCell(e, t, r, i, s, n, l, a, o, u, p, d, null != h && h, m) : n.is2(_i) ? await this.drawColorScaleColumn(e, t, r, i, s, n, l, a, o, u, d, m) : Bu.isImage(a) ? this.renderImageCell(e, t, r, n, a, p, m) : "boolean" == typeof a ? await this.renderBoolCell2(e, t, r, i, s, n, l, a, g, p, m) : await this.renderTextCell(e, t, r, i, s, n, l, a, G.All, g, p, m, !1)
             }
             static processRowValue(e, t, r) {
                 var i;
                 let s = r.textFormat,
-                    n = (null != t && t[L.System.StiObject.stimulsoft]().is($d) && (t = t == $d.Line && null != s ? s.format(e + 1) : es.getSystemVariable(null == t ? void 0 : t[L.System.StiObject.stimulsoft]().as($d), e + 1)), r.ident == Ju.SparklinesColumn);
+                    n = (null != t && t[L.System.StiObject.stimulsoft]().is($d) && (t = t == $d.Line && null != s ? s.format(e + 1) : ts.getSystemVariable(null == t ? void 0 : t[L.System.StiObject.stimulsoft]().as($d), e + 1)), r.ident == Ju.SparklinesColumn);
                 return t = Wu.isList(t) ? n ? Wu.toList(t) : null == (i = Wu.toList(t)) ? void 0 : i.firstOrDefault() : t
             }
             static async renderGraphicCell(s, n, l, t, r, a, i, o, u, h, m, c, d, g) {
                 let p = "",
                     S = n,
                     w = this.getForeColor(l, a, c, d),
                     b = new ld(ul.UTF8);
-                if (b.indentation = -1, b.writeStartElement("svg"), b.writeAttributeString("version", "1.1"), b.writeAttributeString("baseProfile", "full"), b.writeAttributeString("xmlns", "http://www.w3.org/2000/svg"), b.writeAttributeString("xmlns:xlink", "http://www.w3.org/1999/xlink"), b.writeAttributeString("xmlns:ev", "http://www.w3.org/2001/xml-events"), b.writeAttributeString("height", sg.toUnits(n.height)), b.writeAttributeString("width", sg.toUnits(n.width)), b.writeStartElement("rect"), b.writeAttributeString("x", "0"), b.writeAttributeString("y", "0"), b.writeAttributeString("width", sg.toUnits(n.width)), b.writeAttributeString("height", sg.toUnits(n.height)), b.writeAttributeString("style", sg.writeFillBrush(b, m, n)), b.writeEndElement(), a.is2($i)) {
+                if (b.indentation = -1, b.writeStartElement("svg"), b.writeAttributeString("version", "1.1"), b.writeAttributeString("baseProfile", "full"), b.writeAttributeString("xmlns", "http://www.w3.org/2000/svg"), b.writeAttributeString("xmlns:xlink", "http://www.w3.org/1999/xlink"), b.writeAttributeString("xmlns:ev", "http://www.w3.org/2001/xml-events"), b.writeAttributeString("height", sg.toUnits(n.height)), b.writeAttributeString("width", sg.toUnits(n.width)), b.writeStartElement("rect"), b.writeAttributeString("x", "0"), b.writeAttributeString("y", "0"), b.writeAttributeString("width", sg.toUnits(n.width)), b.writeAttributeString("height", sg.toUnits(n.height)), b.writeAttributeString("style", sg.writeFillBrush(b, m, n)), b.writeEndElement(), a.is2(es)) {
                     let e = qd.castToArray(o),
                         t = null == e ? void 0 : e[L.System.StiObject.stimulsoft]().toList().select(e => null == e ? void 0 : e[L.System.StiObject.stimulsoft]().toNumber()),
-                        r = a.as($i),
+                        r = a.as(es),
                         i = new _d(n);
                     return i.values = t, i.positiveColor = r.allowCustomColors ? r.positiveColor : c.cellSparkline, i.negativeColor = r.allowCustomColors ? r.negativeColor : c.cellWinLossNegative, i.showFirstLastPoints = r.showFirstLastPoints, i.showHighLowPoints = r.showHighLowPoints, i.type = r.type, i.brush = new v(m), i.componentPlacement = `d.` + l.name, void s.components.add(i)
                 }
                 let f = new ng(b),
                     y = G.None,
                     C = "GraphicCell",
                     x = new j(0, 0, n.width, n.height),
                     M = a.horAlignment;
-                if (a.is2(_i)) {
-                    await ig.draw(f, x, l, t, r, a, i, V.tryToNumber(o), u, h, d, !1, !1), g != F.f.StiDashboardExportFormat.Data && (S = ig.calculateTextRect(n.clone(), a)).inflate(2, 2), p = ts.formatBasedOnColumnType(l, a, o), w = ig.getForeColor(l, a, c, d, !1);
+                if (a.is2($i)) {
+                    await ig.draw(f, x, l, t, r, a, i, V.tryToNumber(o), u, h, d, !1, !1), g != F.f.StiDashboardExportFormat.Data && (S = ig.calculateTextRect(n.clone(), a)).inflate(2, 2), p = rs.formatBasedOnColumnType(l, a, o), w = ig.getForeColor(l, a, c, d, !1);
                     let e = V.tryToNumber(o);
                     e < 0 && ph.isNegativeInRed(a.textFormat) && (w = Z.Engine.negativeColor), w = 0 < l.tableConditions.length ? await Id.processForeColor(w, a.key, l, t, r) : w, y = G.Right, C = "DataBarsCell"
-                } else if (a.is2(Qi)) Fd.draw(f, x, l, a, i, V.tryToNullableNumber(o), c, !1), S = Fd.calculateTextRect(n.clone(), a), p = Fd.getCellText(l, a, V.tryToNullableNumber(o)), w = Fd.getColor(a, V.tryToNullableNumber(o), c), w = 0 < l.tableConditions.length ? await Id.processForeColor(w, a.key, l, t, r) : w, y = G.None, C = "IndicatorCell";
-                else if (a.is2(Gi)) {
+                } else if (a.is2(qi)) Fd.draw(f, x, l, a, i, V.tryToNullableNumber(o), c, !1), S = Fd.calculateTextRect(n.clone(), a), p = Fd.getCellText(l, a, V.tryToNullableNumber(o)), w = Fd.getColor(a, V.tryToNullableNumber(o), c), w = 0 < l.tableConditions.length ? await Id.processForeColor(w, a.key, l, t, r) : w, y = G.None, C = "IndicatorCell";
+                else if (a.is2(Xi)) {
                     Qd.draw(f, x, l, a, i, V.tryToNullableNumber(o), u, h, d, !1, !1), g != F.f.StiDashboardExportFormat.Data && (S = Qd.calculateTextRect(l, n.clone(), a)).inflate(2, 2), p = Qd.getCellText(l, a, V.tryToNullableNumber(o)), w = ig.getForeColor(l, a, c, d, !1), w = 0 < l.tableConditions.length ? await Id.processForeColor(w, a.key, l, t, r) : w, y = G.None, C = "BubbleCell";
                     let e = a[L.System.StiObject.stimulsoft]().as(Cr);
                     null != e && (e.horAlignment == z.Center && g != F.f.StiDashboardExportFormat.Data && (p = null), e.horAlignment == z.Left && (M = z.Right), e.horAlignment == z.Right) && (M = z.Left)
                 }
-                if (b.writeFullEndElement(), b.flush(), g != F.f.StiDashboardExportFormat.Data && !a.is2($i)) {
+                if (b.writeFullEndElement(), b.flush(), g != F.f.StiDashboardExportFormat.Data && !a.is2(es)) {
                     let e = new ad(n),
-                        t = (e.name = l.name + `_` + C, e.border = this.getBorderSides(s, n, l, a, G.All), e.stretch = !0, e.aspectRatio = a.is2(Qi) || a.is2(Gi), b.textWriter.getStringBuilder().toString());
+                        t = (e.name = l.name + `_` + C, e.border = this.getBorderSides(s, n, l, a, G.All), e.stretch = !0, e.aspectRatio = a.is2(qi) || a.is2(Xi), b.textWriter.getStringBuilder().toString());
                     e.image = Pa.stringToImage(L.System.Convert.toBase64String(t)), e.brush = new v(m), e.horAlignment = M, s.components.add(e)
                 }
                 g != F.f.StiDashboardExportFormat.Data && B.isNullOrEmpty(p) || await this.renderTextCell(s, S, l, t, r, a, i, o, y, w, m, g, !1, !1)
             }
             static async drawColorScaleColumn(e, t, r, i, s, n, l, a, o, u, h, m) {
-                let c = n.as(qi),
+                let c = n.as(_i),
                     d = this.getForeColor(r, n, h, !1),
                     g = lg.getScaleColor(V.tryToNumber(a), o, u, h, c.minimumColor, c.maximumColor),
                     p = r.tableConditions.length ? await Id.processForeAndBackColor(d, g, n.key, r, i, s) : {
                         foreColor: d,
                         backColor: g
                     };
                 await this.renderTextCell(e, t, r, i, s, n, l, a, G.All, p.foreColor, p.backColor, m, !1)
@@ -16171,31 +16188,31 @@
                         t = u ? Pd.CheckRectangle : Pd.NoneRectangle,
                         r = new Bd(s);
                     r.name = n.name + `_Cell`, r.border = this.getBorderSides(i, s, n, o, G.All), r.contourColor = N.transparent, r.textBrush = new v(e.foreColor), r.brush = new v(e.backColor), r.checkStyleForTrue = t, r.checkStyleForFalse = Pd.NoneRectangle, r.checkedValue = t != Pd.NoneRectangle, r.excelDataValue = u.toString(), r.componentPlacement = `d.` + n.name, i.components.add(r)
                 }
             }
             static async renderTextCell(e, t, s, n, l, r, i, a, o, u, h, m, c, d = null) {
                 var g;
-                let p = ts.formatBasedOnColumnType(s, r, a),
+                let p = rs.formatBasedOnColumnType(s, r, a),
                     S = c ? new H("Arial", 10) : s.font,
-                    w = (r.is(rs) && r.showHyperlink && (S = new H(S.fontFamily.name, S.size, S.style | hn.Underline)), 0 < s.tableConditions.length ? await Id.processFontStyle(S, r.key, s, n, l) : hn.Regular),
+                    w = (r.is(is) && r.showHyperlink && (S = new H(S.fontFamily.name, S.size, S.style | mn.Underline)), 0 < s.tableConditions.length ? await Id.processFontStyle(S, r.key, s, n, l) : mn.Regular),
                     b = (S = new H(S.fontFamily.name, S.size, w), V.tryToNumber(a));
-                if (b < 0 && ph.isNegativeInRed(r.textFormat) && (u = Z.Engine.negativeColor), r.is($i)) {
+                if (b < 0 && ph.isNegativeInRed(r.textFormat) && (u = Z.Engine.negativeColor), r.is(es)) {
                     let e = qd.castToArray(a),
                         t = null == e ? void 0 : e[L.System.StiObject.stimulsoft]().toList().select(e => e.toString());
                     p = B.join(" ", t)
                 }
                 let f = 0 < s.tableConditions.length ? await Id.processForeAndBackColor(u, h, r.key, s, n, l) : {
                         foreColor: u,
                         backColor: h
                     },
                     y = Sd.convert(r.horAlignment),
-                    C = (r.is(Gi) && (y = X.Right), r.as(mi)),
+                    C = (r.is(Xi) && (y = X.Right), r.as(ci)),
                     x = (null != C && null == d && (d = C.size.wordWrap), null);
-                if (r.is(rs) && r.showHyperlink && !B.isNullOrWhiteSpace(r.hyperlinkPattern)) {
+                if (r.is(is) && r.showHyperlink && !B.isNullOrWhiteSpace(r.hyperlinkPattern)) {
                     let i = new L.System.Collections.Hashtable;
                     i.add("Value", a);
                     for (let r = 0; r < l.length; r++) {
                         let e = s.columns.firstOrDefault(e => e.key == l[r]),
                             t = "Row." + eg.correctName(e.label, !0);
                         i.add(t, null == (g = n[r]) ? void 0 : g.toString())
                     }
@@ -16215,23 +16232,23 @@
             static async renderBoolCell(e, t, r, i, s, n, l, a, o, u, h) {
                 if (h == F.f.StiDashboardExportFormat.Data) return void await this.renderTextCell(e, t, r, i, s, n, l, a, o, null, u, h, !1);
                 let m = 0 != r.columns.indexOf(n),
                     c = r.columns.indexOf(n) != r.columns.length - 1,
                     d = (m ? G.Left : G.None) | (c ? G.Right : G.None),
                     g = J.getTableStyle(r),
                     p = new ad(t);
-                p.name = r.name + `_Cell`, p.border = o ? new ie(d, g.lineColor, 1, Ri.Solid) : new ie(G.None, N.transparent, 0, Ri.None), p.brush = new v(u), p.horAlignment = z.Center, p.vertAlignment = Wt.Center, e.components.add(p)
+                p.name = r.name + `_Cell`, p.border = o ? new ie(d, g.lineColor, 1, Ei.Solid) : new ie(G.None, N.transparent, 0, Ei.None), p.brush = new v(u), p.horAlignment = z.Center, p.vertAlignment = Wt.Center, e.components.add(p)
             }
             static async getColumnVisibilityState(e, t) {
                 if (e.visibility == Hr.TrueAndHidden) return !1;
                 return Kd.getVisible(e, t)
             }
             static getForeColor(e, t, r, i) {
                 if (!N.transparent.equals(t.foreColor)) return t.foreColor;
-                if (t.is(rs) && t.showHyperlink) return vr.get("165dc8");
+                if (t.is(is) && t.showHyperlink) return vr.get("165dc8");
                 let s = jl.getForeColor(e, e.foreColor);
                 if (!N.transparent.equals(s)) return s;
                 return null != r ? i ? r.alternatingCellForeColor : r.cellForeColor : U.Table.Font.Color
             }
             static getHeaderForeColor(e) {
                 if (!N.transparent.equals(e.headerForeColor)) return e.headerForeColor;
                 let t = J.getTableStyle(e);
@@ -16245,30 +16262,30 @@
             static getBorderSides(e, t, r, i, s) {
                 let n = J.getTableStyle(r),
                     l = 0 != (s & G.Left) && 0 != r.columns.indexOf(i) && t.left < e.width,
                     a = 0 != (s & G.Right) && r.columns.indexOf(i) != r.columns.length - 1 && t.right <= e.width,
                     o = (l ? G.Left : G.None) | (a ? G.Right : G.None),
                     u = o != G.None ? 1 : 0,
                     h = o != G.None ? n.lineColor : N.transparent;
-                return new ie(o, h, u, Ri.Solid)
+                return new ie(o, h, u, Ei.Solid)
             }
         }
         F.A.StiTableElementExportTool = cp
     }
     let og = F.h.StiAutoSizeHtmlTextHelper,
         ug = (F.A.StiTextElementExportTool = class extends F.A.StiElementExportTool {
             async render(e, t, s, r) {
                 if (this.renderEmptyDataMessage(e, t, s.clone(), r)) return;
                 let n = e.as(fm),
                     l = "";
-                if (Z.Engine.dashboardTextElementExpressionParser == au.ReportParser || Rs.isTimeExpression(n.text)) l = await O.parseAsync(n.text, n, !1);
+                if (Z.Engine.dashboardTextElementExpressionParser == au.ReportParser || Es.isTimeExpression(n.text)) l = await O.parseAsync(n.text, n, !1);
                 else if (n.isQuerable) {
                     let e = await bl.tryToGetOrCreate(n),
                         t = new P(null == e ? void 0 : e.rows.firstOrDefault()).select(e => V.tryToString(e)).toList();
-                    null != t && (l = Rs.replaceExpressionBlocksByValues(n.text, t))
+                    null != t && (l = Es.replaceExpressionBlocksByValues(n.text, t))
                 } else l = n.text;
                 if (!B.isNullOrEmpty(l) && l.toLowerCase()[L.System.StiObject.stimulsoft]().replaceAll(" ", "")[L.System.StiObject.stimulsoft]().contains("javascript:") && (l = l.toLowerCase()[L.System.StiObject.stimulsoft]().replaceAll("javascript", "")), n.sizeMode == Dt.Fit) {
                     let i, e = 3;
                     do {
                         let e = og.measure(null, s.clone(), l, n),
                             t = e.width > s.width ? s.width / e.width : 1,
                             r = e.height > s.height ? s.height / e.height : 1;
@@ -16300,22 +16317,22 @@
         class dp extends F.A.StiListBoxElementExportTool {
             async render(e, t, r, i) {
                 return super.render(e, t, r, i)
             }
             getCheckStyle(t, r) {
                 let e = t;
                 if (!e.userFilters.any()) return Pd.CheckRectangle;
-                if (e.userFilters.any(e => e.condition == Zi.IsFalse)) return Pd.NoneRectangle;
+                if (e.userFilters.any(e => e.condition == Yi.IsFalse)) return Pd.NoneRectangle;
                 if (null != r.items) {
                     let e = r.items.select(e => this.getCheckStyle(t, e));
                     if (e.all(e => e == Pd.CheckRectangle)) return Pd.CheckRectangle;
                     if (e.all(e => e == Pd.NoneRectangle)) return Pd.NoneRectangle;
                     return Pd.DotRectangle
                 }
-                if (e.userFilters.any(e => e.condition == Zi.EqualTo && e.value == r.toString())) return Pd.CheckRectangle;
+                if (e.userFilters.any(e => e.condition == Yi.EqualTo && e.value == r.toString())) return Pd.CheckRectangle;
                 return Pd.NoneRectangle
             }
             async renderItems(e, t, r) {
                 var i;
                 let s = await bl.tryToGetOrCreate(r);
                 if (null == s) return;
                 let n = !1,
@@ -16328,15 +16345,15 @@
             }
             renderItem(e, t, r, i, s, n, l, a, o) {
                 i != Vd.locAll && (dp.renderExpander(e, t.clone(), r, o), t.x += U.ListBox.CheckBoxWidth / 2, t.width -= U.ListBox.CheckBoxWidth / 2), super.renderItem(e, t.clone(), r, i, s, n, l, a, o)
             }
             static renderExpander(e, t, r, i) {
                 t = new j(t.x, t.y + t.height / 2 - t.height / 8, U.ListBox.CheckBoxWidth / 3, t.height / 4);
                 let s = new vc(t);
-                s.name = r.name + `_ItemExpander`, s.shapeType = new hg(i ? ug.Down : ug.Right), s.brush = new v(N.dimGray), s.style = Ri.None, e.components.add(s)
+                s.name = r.name + `_ItemExpander`, s.shapeType = new hg(i ? ug.Down : ug.Right), s.brush = new v(N.dimGray), s.style = Ei.None, e.components.add(s)
             }
         }
         F.A.StiTreeViewElementExportTool = dp
     }
     let mg = L.Report.Components.StiHorizontalLinePrimitive;
     F.A.StiWebContentElementExportTool = class extends F.A.StiElementExportTool {
         async render(e, i, s, t) {
@@ -16350,25 +16367,25 @@
                     r = 20;
                 this.paintHeader(i, n, new j(s.x, s.top, s.width, e), l), this.paintSeparator(i, n, new j(s.x + r, s.top + e, s.width - 2 * r, t)), this.paintWebContent(i, n, new j(s.x, s.top + e + t, s.width, e), a, !0)
             } else this.paintWebContent(i, n, new j(s.x, s.top, s.width, s.height), a)
         }
         paintHeader(e, t, r, i) {
             let s = J.getForeColor(t),
                 n = new Du(r);
-            n.name = t.name + `__WebContentHeader`, n.vertAlignment = Wt.Center, n.horAlignment = X.Left, n.textBrush = new v(s), n.brush = new v(N.transparent), n.margins = new be(20, 0, 0, 0), n.text = i, n.font = new H("Arial", 8, hn.Bold), e.components.add(n)
+            n.name = t.name + `__WebContentHeader`, n.vertAlignment = Wt.Center, n.horAlignment = X.Left, n.textBrush = new v(s), n.brush = new v(N.transparent), n.margins = new be(20, 0, 0, 0), n.text = i, n.font = new H("Arial", 8, mn.Bold), e.components.add(n)
         }
         paintSeparator(e, t, r) {
             let i = J.getForeColor(t),
                 s = new mg(r);
             s.name = t.name + `_WebContentSep`, s.color = i, e.components.add(s)
         }
         paintWebContent(e, t, r, i, s = !1) {
             let n = J.getForeColor(t),
                 l = new Du(r);
-            l.name = t.name + `__WebContentContent`, l.vertAlignment = s ? Wt.Center : Wt.Top, l.horAlignment = X.Left, l.textBrush = new v(n), l.brush = new v(N.transparent), l.margins = new be(s ? 20 : 0, 0, 0, 0), l.text = i, l.font = new H("Arial", 8, hn.Bold), l.allowHtmlTags = !s, e.components.add(l)
+            l.name = t.name + `__WebContentContent`, l.vertAlignment = s ? Wt.Center : Wt.Top, l.horAlignment = X.Left, l.textBrush = new v(n), l.brush = new v(N.transparent), l.margins = new be(s ? 20 : 0, 0, 0, 0), l.text = i, l.font = new H("Arial", 8, mn.Bold), l.allowHtmlTags = !s, e.components.add(l)
         }
     };
     {
         class gp {
             static run(i, s) {
                 if (void 0 === i) return void gp.run(L, "Stimulsoft");
                 if ("Stimulsoft.ExternalLibrary" == s || "Stimulsoft.Blockly" == s) return;
```

### Comparing `stimulsoft_dashboards-2024.2.5/stimulsoft_dashboards.egg-info/PKG-INFO` & `stimulsoft_dashboards-2024.2.6/stimulsoft_dashboards.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stimulsoft-dashboards
-Version: 2024.2.5
+Version: 2024.2.6
 Summary: Data visualization in Python applications.
 Home-page: https://www.stimulsoft.com/en/products/dashboards-python
 Author: Stimulsoft
 Author-email: info@stimulsoft.com
 License: https://www.stimulsoft.com/en/licensing/developers
 Classifier: License :: Other/Proprietary License
 Classifier: Framework :: Django
```

### Comparing `stimulsoft_dashboards-2024.2.5/stimulsoft_dashboards.egg-info/SOURCES.txt` & `stimulsoft_dashboards-2024.2.6/stimulsoft_dashboards.egg-info/SOURCES.txt`

 * *Files identical despite different names*

