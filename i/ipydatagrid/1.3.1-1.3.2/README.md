# Comparing `tmp/ipydatagrid-1.3.1.tar.gz` & `tmp/ipydatagrid-1.3.2.tar.gz`

## Comparing `ipydatagrid-1.3.1.tar` & `ipydatagrid-1.3.2.tar`

### file list

```diff
@@ -1,97 +1,97 @@
--rw-r--r--   0        0        0     7548 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/RELEASE.md
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/babel.config.js
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid.json
--rw-r--r--   0        0        0     5321 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/package.json
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/tsconfig.json
--rw-r--r--   0        0        0     2852 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/webpack.config.js
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/webpack.lab.config.js
--rw-r--r--   0        0        0   403706 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/yarn.lock
--rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/__init__.py
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/_frontend.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/_version.py
--rw-r--r--   0        0        0     7812 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/cellrenderer.py
--rw-r--r--   0        0        0    34516 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/datagrid.py
--rw-r--r--   0        0        0     5437 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/labextension/package.json
--rw-r--r--   0        0        0    17303 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/labextension/static/109.bdd9793b392cc2fe87da.js
--rw-r--r--   0        0        0     4982 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/labextension/static/142.025e64e0cbb8aa528385.js
--rw-r--r--   0        0        0    26563 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/labextension/static/143.171db67c9b56d395ae64.js
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/labextension/static/14ad542071f6e259fbe2.png
--rw-r--r--   0        0        0     9449 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/labextension/static/271.c6d995708c863e1b27ed.js
--rw-r--r--   0        0        0     7708 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/labextension/static/296.d2eeaa2e543e597ac586.js
--rw-r--r--   0        0        0    32396 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/labextension/static/351.372e5eec3c9010a57cf3.js
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/labextension/static/3546b939aba74f121f34.png
--rw-r--r--   0        0        0     2801 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/labextension/static/400.95b73fc6eb3f120b823f.js
--rw-r--r--   0        0        0    17303 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/labextension/static/41.1846c3ba970651a706b6.js
--rw-r--r--   0        0        0    17304 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/labextension/static/433.75ed253aaa8060b28c81.js
--rw-r--r--   0        0        0    17304 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/labextension/static/455.25b625d30041b5a1671c.js
--rw-r--r--   0        0        0     4293 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/labextension/static/456.afd75d5e116998d22e56.js
--rw-r--r--   0        0        0     4982 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/labextension/static/462.68e4d74f02bf2411528e.js
--rw-r--r--   0        0        0    12212 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/labextension/static/48.732e43cec274cf5b8cf5.js
--rw-r--r--   0        0        0     5161 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/labextension/static/481.911a23288443c8041987.js
--rw-r--r--   0        0        0    17304 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/labextension/static/513.73d1ca46ed758871d49a.js
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/labextension/static/568.2b5bb2c0c4fdfa06786c.js
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/labextension/static/5b5469a81198fb5e6aa1.png
--rw-r--r--   0        0        0    11919 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/labextension/static/642.730227a42292c5f89120.js
--rw-r--r--   0        0        0    17304 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/labextension/static/643.a265dd26cb50ebd06923.js
--rw-r--r--   0        0        0   136897 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/labextension/static/679.e174128fe156c1cd0d10.js
--rw-r--r--   0        0        0    12508 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/labextension/static/683.efe59705c1680a8f8b3a.js
--rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/labextension/static/700.7f792a9e7380bfde28dc.js
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/labextension/static/733684aa1ae47c885305.png
--rw-r--r--   0        0        0   292706 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/labextension/static/762.42901b906691b1301214.js
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/labextension/static/762.42901b906691b1301214.js.LICENSE.txt
--rw-r--r--   0        0        0    20610 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/labextension/static/781.ef3f9c2a235c4a40bdc0.js
--rw-r--r--   0        0        0   105961 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/labextension/static/787.47c1e167bb24294e1e7e.js
--rw-r--r--   0        0        0    22076 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/labextension/static/794.d7c23e15137c8752365e.js
--rw-r--r--   0        0        0    10377 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/labextension/static/811.a135ebc21be585e6d76d.js
--rw-r--r--   0        0        0     5901 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/labextension/static/823.18e09aad57c7797df987.js
--rw-r--r--   0        0        0    26563 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/labextension/static/917.b972bc5b41fae8990bff.js
--rw-r--r--   0        0        0    35000 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/labextension/static/939.04c5876588e4898127e3.js
--rw-r--r--   0        0        0    11847 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/labextension/static/941.23c8b1f0eb18afd531e9.js
--rw-r--r--   0        0        0     5901 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/labextension/static/990.e35c256305f259cdaeb9.js
--rw-r--r--   0        0        0    13315 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/labextension/static/remoteEntry.6d509d1468636d15eab8.js
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/labextension/static/style.js
--rw-r--r--   0        0        0    40475 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/nbextension/extension.js
--rw-r--r--   0        0        0  2613456 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/nbextension/index.js
--rw-r--r--   0        0        0     2167 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/ipydatagrid/nbextension/index.js.LICENSE.txt
--rw-r--r--   0        0        0    16722 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/js/cellrenderer.ts
--rw-r--r--   0        0        0    25051 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/js/datagrid.ts
--rw-r--r--   0        0        0     3560 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/js/datasource.ts
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/js/extension.ts
--rw-r--r--   0        0        0    31969 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/js/feathergrid.ts
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/js/index.ts
--rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/js/keyhandler.ts
--rw-r--r--   0        0        0     4832 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/js/mousehandler.ts
--rw-r--r--   0        0        0     2197 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/js/plugin.ts
--rw-r--r--   0        0        0     9492 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/js/utils.ts
--rw-r--r--   0        0        0     4151 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/js/vegaexpr.ts
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/js/version.ts
--rw-r--r--   0        0        0     6282 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/js/core/barrenderer.ts
--rw-r--r--   0        0        0    45377 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/js/core/filterMenu.ts
--rw-r--r--   0        0        0     7846 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/js/core/gridContextMenu.ts
--rw-r--r--   0        0        0    15136 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/js/core/headerRenderer.ts
--rw-r--r--   0        0        0     8567 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/js/core/htmlRenderer.ts
--rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/js/core/transform.ts
--rw-r--r--   0        0        0    11413 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/js/core/transformExecutors.ts
--rw-r--r--   0        0        0     6994 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/js/core/transformStateManager.ts
--rw-r--r--   0        0        0     4899 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/js/core/valueRenderer.ts
--rw-r--r--   0        0        0     7540 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/js/core/view.ts
--rw-r--r--   0        0        0    19073 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/js/core/viewbasedjsonmodel.ts
--rw-r--r--   0        0        0  1526055 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/static/ipydatagrid_1.gif
--rw-r--r--   0        0        0  1526560 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/static/ipydatagrid_2.gif
--rw-r--r--   0        0        0  2696451 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/static/ipydatagrid_3.gif
--rw-r--r--   0        0        0   203865 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/static/ipydatagrid_4.gif
--rw-r--r--   0        0        0    52546 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/static/ipydatagrid_5.gif
--rw-r--r--   0        0        0     4544 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/style/feathergrid.css
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/style/jupyter-widget.css
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/style/icons/arrow-down-short-dark.svg
--rwxr-xr-x   0        0        0      416 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/style/icons/arrow-down-short.svg
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/style/icons/arrow-up-short-dark.svg
--rwxr-xr-x   0        0        0      400 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/style/icons/arrow-up-short.svg
--rwxr-xr-x   0        0        0      349 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/style/icons/filter-dark.svg
--rwxr-xr-x   0        0        0      349 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/style/icons/filter.svg
--rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/.gitignore
--rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/LICENSE.txt
--rw-r--r--   0        0        0     4897 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/README.md
--rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/pyproject.toml
--rw-r--r--   0        0        0     6036 2020-02-02 00:00:00.000000 ipydatagrid-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0     7548 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/RELEASE.md
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/babel.config.js
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/ipydatagrid.json
+-rw-r--r--   0        0        0     5321 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/package.json
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/tsconfig.json
+-rw-r--r--   0        0        0     2852 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/webpack.config.js
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/webpack.lab.config.js
+-rw-r--r--   0        0        0   403706 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/yarn.lock
+-rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/ipydatagrid/__init__.py
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/ipydatagrid/_frontend.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/ipydatagrid/_version.py
+-rw-r--r--   0        0        0     7812 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/ipydatagrid/cellrenderer.py
+-rw-r--r--   0        0        0    34859 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/ipydatagrid/datagrid.py
+-rw-r--r--   0        0        0     5437 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/ipydatagrid/labextension/package.json
+-rw-r--r--   0        0        0    17303 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/ipydatagrid/labextension/static/109.bdd9793b392cc2fe87da.js
+-rw-r--r--   0        0        0     4982 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/ipydatagrid/labextension/static/142.025e64e0cbb8aa528385.js
+-rw-r--r--   0        0        0    26563 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/ipydatagrid/labextension/static/143.171db67c9b56d395ae64.js
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/ipydatagrid/labextension/static/14ad542071f6e259fbe2.png
+-rw-r--r--   0        0        0     9449 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/ipydatagrid/labextension/static/271.c6d995708c863e1b27ed.js
+-rw-r--r--   0        0        0     7708 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/ipydatagrid/labextension/static/296.59cf43ce555ff3a1e3f1.js
+-rw-r--r--   0        0        0    32396 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/ipydatagrid/labextension/static/351.372e5eec3c9010a57cf3.js
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/ipydatagrid/labextension/static/3546b939aba74f121f34.png
+-rw-r--r--   0        0        0     2801 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/ipydatagrid/labextension/static/400.95b73fc6eb3f120b823f.js
+-rw-r--r--   0        0        0    17303 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/ipydatagrid/labextension/static/41.1846c3ba970651a706b6.js
+-rw-r--r--   0        0        0    17304 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/ipydatagrid/labextension/static/433.75ed253aaa8060b28c81.js
+-rw-r--r--   0        0        0    17304 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/ipydatagrid/labextension/static/455.25b625d30041b5a1671c.js
+-rw-r--r--   0        0        0     4293 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/ipydatagrid/labextension/static/456.afd75d5e116998d22e56.js
+-rw-r--r--   0        0        0     4982 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/ipydatagrid/labextension/static/462.68e4d74f02bf2411528e.js
+-rw-r--r--   0        0        0    12212 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/ipydatagrid/labextension/static/48.732e43cec274cf5b8cf5.js
+-rw-r--r--   0        0        0     5161 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/ipydatagrid/labextension/static/481.911a23288443c8041987.js
+-rw-r--r--   0        0        0    17304 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/ipydatagrid/labextension/static/513.73d1ca46ed758871d49a.js
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/ipydatagrid/labextension/static/568.2b5bb2c0c4fdfa06786c.js
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/ipydatagrid/labextension/static/5b5469a81198fb5e6aa1.png
+-rw-r--r--   0        0        0    11919 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/ipydatagrid/labextension/static/642.730227a42292c5f89120.js
+-rw-r--r--   0        0        0    17304 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/ipydatagrid/labextension/static/643.a265dd26cb50ebd06923.js
+-rw-r--r--   0        0        0   136897 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/ipydatagrid/labextension/static/679.e174128fe156c1cd0d10.js
+-rw-r--r--   0        0        0    12508 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/ipydatagrid/labextension/static/683.efe59705c1680a8f8b3a.js
+-rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/ipydatagrid/labextension/static/700.7f792a9e7380bfde28dc.js
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/ipydatagrid/labextension/static/733684aa1ae47c885305.png
+-rw-r--r--   0        0        0   292706 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/ipydatagrid/labextension/static/762.42901b906691b1301214.js
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/ipydatagrid/labextension/static/762.42901b906691b1301214.js.LICENSE.txt
+-rw-r--r--   0        0        0    20610 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/ipydatagrid/labextension/static/781.ef3f9c2a235c4a40bdc0.js
+-rw-r--r--   0        0        0   106066 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/ipydatagrid/labextension/static/787.b52e0074e2cbca59f4b7.js
+-rw-r--r--   0        0        0    22076 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/ipydatagrid/labextension/static/794.d7c23e15137c8752365e.js
+-rw-r--r--   0        0        0    10377 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/ipydatagrid/labextension/static/811.a135ebc21be585e6d76d.js
+-rw-r--r--   0        0        0     5901 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/ipydatagrid/labextension/static/823.18e09aad57c7797df987.js
+-rw-r--r--   0        0        0    26563 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/ipydatagrid/labextension/static/917.b972bc5b41fae8990bff.js
+-rw-r--r--   0        0        0    35000 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/ipydatagrid/labextension/static/939.04c5876588e4898127e3.js
+-rw-r--r--   0        0        0    11847 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/ipydatagrid/labextension/static/941.23c8b1f0eb18afd531e9.js
+-rw-r--r--   0        0        0     5901 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/ipydatagrid/labextension/static/990.e35c256305f259cdaeb9.js
+-rw-r--r--   0        0        0    13315 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/ipydatagrid/labextension/static/remoteEntry.91868686b1e0561ea123.js
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/ipydatagrid/labextension/static/style.js
+-rw-r--r--   0        0        0    40475 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/ipydatagrid/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/ipydatagrid/nbextension/extension.js
+-rw-r--r--   0        0        0  2613561 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/ipydatagrid/nbextension/index.js
+-rw-r--r--   0        0        0     2167 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/ipydatagrid/nbextension/index.js.LICENSE.txt
+-rw-r--r--   0        0        0    16722 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/js/cellrenderer.ts
+-rw-r--r--   0        0        0    25421 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/js/datagrid.ts
+-rw-r--r--   0        0        0     3560 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/js/datasource.ts
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/js/extension.ts
+-rw-r--r--   0        0        0    31969 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/js/feathergrid.ts
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/js/index.ts
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/js/keyhandler.ts
+-rw-r--r--   0        0        0     4832 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/js/mousehandler.ts
+-rw-r--r--   0        0        0     2197 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/js/plugin.ts
+-rw-r--r--   0        0        0     9492 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/js/utils.ts
+-rw-r--r--   0        0        0     4151 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/js/vegaexpr.ts
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/js/version.ts
+-rw-r--r--   0        0        0     6282 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/js/core/barrenderer.ts
+-rw-r--r--   0        0        0    45377 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/js/core/filterMenu.ts
+-rw-r--r--   0        0        0     7846 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/js/core/gridContextMenu.ts
+-rw-r--r--   0        0        0    15136 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/js/core/headerRenderer.ts
+-rw-r--r--   0        0        0     8567 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/js/core/htmlRenderer.ts
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/js/core/transform.ts
+-rw-r--r--   0        0        0    11413 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/js/core/transformExecutors.ts
+-rw-r--r--   0        0        0     6994 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/js/core/transformStateManager.ts
+-rw-r--r--   0        0        0     4899 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/js/core/valueRenderer.ts
+-rw-r--r--   0        0        0     7540 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/js/core/view.ts
+-rw-r--r--   0        0        0    19073 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/js/core/viewbasedjsonmodel.ts
+-rw-r--r--   0        0        0  1526055 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/static/ipydatagrid_1.gif
+-rw-r--r--   0        0        0  1526560 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/static/ipydatagrid_2.gif
+-rw-r--r--   0        0        0  2696451 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/static/ipydatagrid_3.gif
+-rw-r--r--   0        0        0   203865 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/static/ipydatagrid_4.gif
+-rw-r--r--   0        0        0    52546 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/static/ipydatagrid_5.gif
+-rw-r--r--   0        0        0     4544 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/style/feathergrid.css
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/style/jupyter-widget.css
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/style/icons/arrow-down-short-dark.svg
+-rwxr-xr-x   0        0        0      416 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/style/icons/arrow-down-short.svg
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/style/icons/arrow-up-short-dark.svg
+-rwxr-xr-x   0        0        0      400 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/style/icons/arrow-up-short.svg
+-rwxr-xr-x   0        0        0      349 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/style/icons/filter-dark.svg
+-rwxr-xr-x   0        0        0      349 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/style/icons/filter.svg
+-rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/.gitignore
+-rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/LICENSE.txt
+-rw-r--r--   0        0        0     4897 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/README.md
+-rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0     6036 2020-02-02 00:00:00.000000 ipydatagrid-1.3.2/PKG-INFO
```

### Comparing `ipydatagrid-1.3.1/RELEASE.md` & `ipydatagrid-1.3.2/RELEASE.md`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.1/package.json` & `ipydatagrid-1.3.2/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9705882352941176%*

 * *Differences: {"'version'": "'1.3.2'"}*

```diff
@@ -166,9 +166,9 @@
         "test": "jest --verbose",
         "watch": "npm-run-all -p watch:lib watch:labextension watch:nbextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:lib": "tsc -w",
         "watch:nbextension": "webpack --watch"
     },
     "types": "./lib/index.d.ts",
-    "version": "1.3.1"
+    "version": "1.3.2"
 }
```

### Comparing `ipydatagrid-1.3.1/tsconfig.json` & `ipydatagrid-1.3.2/tsconfig.json`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.1/webpack.config.js` & `ipydatagrid-1.3.2/webpack.config.js`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.1/yarn.lock` & `ipydatagrid-1.3.2/yarn.lock`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.1/ipydatagrid/__init__.py` & `ipydatagrid-1.3.2/ipydatagrid/__init__.py`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.1/ipydatagrid/cellrenderer.py` & `ipydatagrid-1.3.2/ipydatagrid/cellrenderer.py`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.1/ipydatagrid/datagrid.py` & `ipydatagrid-1.3.2/ipydatagrid/datagrid.py`

 * *Files 1% similar despite different names*

```diff
@@ -429,23 +429,25 @@
         self._cell_change_handlers = CallbackDispatcher()
         self.on_msg(self.__handle_custom_msg)
         self._set_renderer_defaults()
 
     def __handle_custom_msg(self, _, content, buffers):  # noqa: U101,U100
         if content["event_type"] == "cell-changed":
             row = content["row"]
-            column = content["column"]
+            column = self._column_index_to_name(
+                self._data, content["column_index"]
+            )
             value = content["value"]
             # update data on kernel
             self._data["data"].loc[row, column] = value
             # notify python listeners
             self._cell_change_handlers(
                 {
                     "row": row,
-                    "column": content["column"],
+                    "column": column,
                     "column_index": content["column_index"],
                     "value": value,
                 }
             )
         elif content["event_type"] == "cell-click":
             # notify python listeners
             self._cell_click_handlers(
@@ -466,14 +468,15 @@
             df = pd.DataFrame(self._data["data"])
         else:
             df = pd.DataFrame(
                 {value["name"]: [] for value in self._data["schema"]["fields"]}
             )
         final_df = df.set_index(trimmed_primary_key)
         final_df = final_df[final_df.columns[:-1]]
+        final_df.drop(columns=["ipydguuid"], inplace=True, errors="ignore")
         return final_df
 
     @data.setter
     def data(self, dataframe):
         # Reference for the original frame column and index names
         # This is used to when returning the view data model
         self.__dataframe_reference_index_names = dataframe.index.names
@@ -758,32 +761,38 @@
         with keys 'r': row and 'c': column
         """
         return SelectionHelper(
             self._data, self.selections, self.selection_mode
         ).all()
 
     @property
-    def selected_cell_values(self):
+    def selected_visible_cell_iterator(self):
         """
-        List of values for all selected cells.
+        An iterator to traverse selected visible cells one by one.
         """
         # Copy of the front-end data model
         view_data = self.get_visible_data()
 
         # Get primary key from dataframe
         index_key = self.get_dataframe_index(view_data)
 
         # Serielize to JSON table schema
         view_data_object = self.generate_data_object(
             view_data, "ipydguuid", index_key
         )
-
         return SelectionHelper(
             view_data_object, self.selections, self.selection_mode
-        ).all_values()
+        )
+
+    @property
+    def selected_cell_values(self):
+        """
+        List of values for all selected cells.
+        """
+        return self.selected_visible_cell_iterator.all_values()
 
     @property
     def selected_cell_iterator(self):
         """
         An iterator to traverse selected cells one by one.
         """
         return SelectionHelper(self._data, self.selections, self.selection_mode)
```

### Comparing `ipydatagrid-1.3.1/ipydatagrid/labextension/package.json` & `ipydatagrid-1.3.2/ipydatagrid/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9698529411764706%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.91868686b1e0561ea123.js'}}",*

 * * "'version'": "'1.3.2'"}*

```diff
@@ -82,15 +82,15 @@
         "dist/*.png",
         "style/**/*.*"
     ],
     "homepage": "https://github.com/Bloomberg/ipydatagrid",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.6d509d1468636d15eab8.js"
+            "load": "static/remoteEntry.91868686b1e0561ea123.js"
         },
         "extension": "lib/plugin",
         "outputDir": "./ipydatagrid/labextension",
         "sharedPackages": {
             "@jupyter-widgets/base": {
                 "bundled": false,
                 "singleton": true
@@ -170,9 +170,9 @@
         "test": "jest --verbose",
         "watch": "npm-run-all -p watch:lib watch:labextension watch:nbextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:lib": "tsc -w",
         "watch:nbextension": "webpack --watch"
     },
     "types": "./lib/index.d.ts",
-    "version": "1.3.1"
+    "version": "1.3.2"
 }
```

### Comparing `ipydatagrid-1.3.1/ipydatagrid/labextension/static/109.bdd9793b392cc2fe87da.js` & `ipydatagrid-1.3.2/ipydatagrid/labextension/static/109.bdd9793b392cc2fe87da.js`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.1/ipydatagrid/labextension/static/142.025e64e0cbb8aa528385.js` & `ipydatagrid-1.3.2/ipydatagrid/labextension/static/142.025e64e0cbb8aa528385.js`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.1/ipydatagrid/labextension/static/143.171db67c9b56d395ae64.js` & `ipydatagrid-1.3.2/ipydatagrid/labextension/static/143.171db67c9b56d395ae64.js`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.1/ipydatagrid/labextension/static/271.c6d995708c863e1b27ed.js` & `ipydatagrid-1.3.2/ipydatagrid/labextension/static/271.c6d995708c863e1b27ed.js`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.1/ipydatagrid/labextension/static/296.d2eeaa2e543e597ac586.js` & `ipydatagrid-1.3.2/ipydatagrid/labextension/static/296.59cf43ce555ff3a1e3f1.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -27,15 +27,15 @@
                         for (var t in e) "default" !== t && Object.prototype.hasOwnProperty.call(e, t) && r(n, e, t);
                     return i(n, e), n
                 };
             Object.defineProperty(n, "__esModule", {
                 value: !0
             });
             const a = t(6664),
-                s = t(1464),
+                s = t(3712),
                 d = o(t(5787)),
                 c = t(8657),
                 l = {
                     id: "ipydatagrid:plugin",
                     requires: [a.IJupyterWidgetRegistry],
                     optional: [s.IThemeManager],
                     activate: function(e, n, t) {
```

### Comparing `ipydatagrid-1.3.1/ipydatagrid/labextension/static/351.372e5eec3c9010a57cf3.js` & `ipydatagrid-1.3.2/ipydatagrid/labextension/static/351.372e5eec3c9010a57cf3.js`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.1/ipydatagrid/labextension/static/400.95b73fc6eb3f120b823f.js` & `ipydatagrid-1.3.2/ipydatagrid/labextension/static/400.95b73fc6eb3f120b823f.js`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.1/ipydatagrid/labextension/static/41.1846c3ba970651a706b6.js` & `ipydatagrid-1.3.2/ipydatagrid/labextension/static/41.1846c3ba970651a706b6.js`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.1/ipydatagrid/labextension/static/433.75ed253aaa8060b28c81.js` & `ipydatagrid-1.3.2/ipydatagrid/labextension/static/433.75ed253aaa8060b28c81.js`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.1/ipydatagrid/labextension/static/455.25b625d30041b5a1671c.js` & `ipydatagrid-1.3.2/ipydatagrid/labextension/static/455.25b625d30041b5a1671c.js`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.1/ipydatagrid/labextension/static/456.afd75d5e116998d22e56.js` & `ipydatagrid-1.3.2/ipydatagrid/labextension/static/456.afd75d5e116998d22e56.js`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.1/ipydatagrid/labextension/static/462.68e4d74f02bf2411528e.js` & `ipydatagrid-1.3.2/ipydatagrid/labextension/static/462.68e4d74f02bf2411528e.js`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.1/ipydatagrid/labextension/static/48.732e43cec274cf5b8cf5.js` & `ipydatagrid-1.3.2/ipydatagrid/labextension/static/48.732e43cec274cf5b8cf5.js`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.1/ipydatagrid/labextension/static/481.911a23288443c8041987.js` & `ipydatagrid-1.3.2/ipydatagrid/labextension/static/481.911a23288443c8041987.js`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.1/ipydatagrid/labextension/static/513.73d1ca46ed758871d49a.js` & `ipydatagrid-1.3.2/ipydatagrid/labextension/static/513.73d1ca46ed758871d49a.js`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.1/ipydatagrid/labextension/static/568.2b5bb2c0c4fdfa06786c.js` & `ipydatagrid-1.3.2/ipydatagrid/labextension/static/568.2b5bb2c0c4fdfa06786c.js`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.1/ipydatagrid/labextension/static/642.730227a42292c5f89120.js` & `ipydatagrid-1.3.2/ipydatagrid/labextension/static/642.730227a42292c5f89120.js`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.1/ipydatagrid/labextension/static/643.a265dd26cb50ebd06923.js` & `ipydatagrid-1.3.2/ipydatagrid/labextension/static/643.a265dd26cb50ebd06923.js`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.1/ipydatagrid/labextension/static/679.e174128fe156c1cd0d10.js` & `ipydatagrid-1.3.2/ipydatagrid/labextension/static/679.e174128fe156c1cd0d10.js`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.1/ipydatagrid/labextension/static/683.efe59705c1680a8f8b3a.js` & `ipydatagrid-1.3.2/ipydatagrid/labextension/static/683.efe59705c1680a8f8b3a.js`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.1/ipydatagrid/labextension/static/700.7f792a9e7380bfde28dc.js` & `ipydatagrid-1.3.2/ipydatagrid/labextension/static/700.7f792a9e7380bfde28dc.js`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.1/ipydatagrid/labextension/static/762.42901b906691b1301214.js` & `ipydatagrid-1.3.2/ipydatagrid/labextension/static/762.42901b906691b1301214.js`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.1/ipydatagrid/labextension/static/781.ef3f9c2a235c4a40bdc0.js` & `ipydatagrid-1.3.2/ipydatagrid/labextension/static/781.ef3f9c2a235c4a40bdc0.js`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.1/ipydatagrid/labextension/static/787.47c1e167bb24294e1e7e.js` & `ipydatagrid-1.3.2/ipydatagrid/labextension/static/787.b52e0074e2cbca59f4b7.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -2172,15 +2172,14 @@
                             break;
                         case "cell-edit-event":
                             const e = this.get("_data");
                             e.data[t.column][t.row] = t.value, this.set("_data", e), this.send({
                                 event_type: "cell-changed",
                                 region: t.region,
                                 row: t.row,
-                                column: t.column,
                                 column_index: t.columnIndex,
                                 value: t.value
                             }, Object.assign({}, this._view_callbacks));
                             break;
                         default:
                             throw "unreachable"
                     }
@@ -2275,15 +2274,26 @@
                                 const r = new Array(t.length);
                                 let n = 0;
                                 for (const i of t) r[n++] = i[e];
                                 i[e] = r
                             }
                             return new f.DataSource(i, e.fields, e.schema, !0)
                         }
-                        for (const r of Object.keys(e.data)) i[r] = [], Array.isArray(e.data[r]) ? i[r] = e.data[r] : "raw" == e.data[r].type ? i[r] = b(e.data[r].value) : 0 !== e.data[r].value.length && (i[r] = u.array_or_json_serializer.deserialize(e.data[r], t));
+                        for (const r of Object.keys(e.data))
+                            if (i[r] = [], Array.isArray(e.data[r])) i[r] = e.data[r];
+                            else if ("raw" == e.data[r].type) i[r] = b(e.data[r].value);
+                        else if (0 !== e.data[r].value.length) {
+                            let n = u.array_or_json_serializer.deserialize(e.data[r], t);
+                            if ("date" === n.type) {
+                                const e = n;
+                                n = [];
+                                for (let t = 0; t < e.length; t++) n[t] = new Date(e[t]).toISOString()
+                            }
+                            i[r] = n
+                        }
                         return new f.DataSource(i, e.fields, e.schema, !0)
                     },
                     serialize: function(e, t) {
                         const i = {};
                         for (const r of Object.keys(e.data)) i[r] = u.array_or_json_serializer.serialize(e.data[r], t);
                         return {
                             data: i,
@@ -3478,11 +3488,11 @@
         7888: e => {
             e.exports = "data:image/svg+xml,%3csvg class='bi bi-filter' width='1em' height='1em' viewBox='0 0 20 20' fill='white' xmlns='http://www.w3.org/2000/svg'%3e %3cpath fill-rule='evenodd' d='M7.5 13a.5.5 0 01.5-.5h4a.5.5 0 010 1H8a.5.5 0 01-.5-.5zm-2-3a.5.5 0 01.5-.5h8a.5.5 0 010 1H6a.5.5 0 01-.5-.5zm-2-3a.5.5 0 01.5-.5h12a.5.5 0 010 1H4a.5.5 0 01-.5-.5z' clip-rule='evenodd'/%3e %3c/svg%3e"
         },
         7509: e => {
             e.exports = "data:image/svg+xml,%3csvg class='bi bi-filter' width='1em' height='1em' viewBox='0 0 20 20' fill='black' xmlns='http://www.w3.org/2000/svg'%3e %3cpath fill-rule='evenodd' d='M7.5 13a.5.5 0 01.5-.5h4a.5.5 0 010 1H8a.5.5 0 01-.5-.5zm-2-3a.5.5 0 01.5-.5h8a.5.5 0 010 1H6a.5.5 0 01-.5-.5zm-2-3a.5.5 0 01.5-.5h12a.5.5 0 010 1H4a.5.5 0 01-.5-.5z' clip-rule='evenodd'/%3e %3c/svg%3e"
         },
         4147: e => {
-            e.exports = JSON.parse('{"name":"ipydatagrid","version":"1.3.1","description":"Fast Datagrid widget for the Jupyter Notebook and JupyterLab","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","lib/**/*.js.map","lib/**/*.ts","dist/*.js","dist/*.js.map","dist/*.png","style/**/*.*"],"homepage":"https://github.com/Bloomberg/ipydatagrid","bugs":{"url":"https://github.com/Bloomberg/ipydatagrid/issues"},"license":"BSD-3-Clause","author":{"name":"Bloomberg","email":""},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/Bloomberg/ipydatagrid"},"scripts":{"build":"jlpm run build:lib && jlpm run build:nbextension && jlpm run build:labextension","build:dev":"jlpm run build:lib && jlpm run build:nbextension && jlpm run build:labextension:dev","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack --mode=production --no-devtool","build:widget-examples":"cd widget-examples/basic && webpack --mode=production","build:all":"jlpm run build:labextension && jlpm run build:nbextension && jlpm run build:widget-examples","clean":"rimraf dist && jlpm run clean:lib && jlpm run clean:labextension && jlpm run clean:nbextension","clean:lib":"rimraf lib","clean:labextension":"rimraf ipydatagrid/labextension","clean:nbextension":"rimraf ipydatagrid/nbextension/index.*","lint":"eslint \'js/**/*.{js,ts}\' --quiet --fix","prepack":"jlpm run build:labextension && jlpm run build:nbextension","test":"jest --verbose","watch":"npm-run-all -p watch:lib watch:labextension watch:nbextension","watch:lib":"tsc -w","watch:nbextension":"webpack --watch","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^2 || ^3 || ^4 || ^6","@jupyterlab/apputils":"^3 || ^4","@lumino/algorithm":"^1 || ^2","@lumino/application":"^1 || ^2","@lumino/commands":"^1 || ^2","@lumino/coreutils":"^1 || ^2","@lumino/datagrid":"^1 || ^2","@lumino/default-theme":"^1 || ^2","@lumino/domutils":"^1 || ^2","@lumino/messaging":"^1 || ^2","@lumino/signaling":"^1 || ^2","@lumino/virtualdom":"^1 || ^2","@lumino/widgets":"^1 || ^2","bqplot":"^0.5","core-js-pure":"^3.30.2","d3-array":"^2.2.0","d3-color":"^3.1.0","d3-format":"^1.3.2","d3-scale":"^3.0.0","d3-time-format":"^2.1.3","jest-environment-jsdom":"^28.1.3","moment":"^2.24.0","underscore":"^1.13.6","vega-expression":"^2.6.0","vega-format":"^1.1.1","vega-functions":"^5.3.0"},"devDependencies":{"@babel/cli":"^7.6.3","@babel/core":"^7.6.3","@babel/preset-env":"^7.6.3","@babel/preset-typescript":"^7.6.0","@jupyterlab/builder":"^4.0.5","@types/jest":"^27.4.1","@types/node":"^10.11.6","@types/underscore":"^1.11.4","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.5.0","@typescript-eslint/parser":"^3.5.0","acorn":"^6.2.0","babel-jest":"^28.1.3","babel-plugin-transform-es2015-modules-commonjs":"^6.26.2","css-loader":"^6.8.1","eslint":"^7.3.1","eslint-config-prettier":"^6.11.0","eslint-plugin-prettier":"^3.1.4","fs-extra":"^7.0.0","jest":"^28.1.3","jest-raw-loader":"^1.0.1","lint-staged":"^10.2.11","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.0.5","raw-loader":"^4.0.2","rimraf":"^2.6.2","source-map-loader":"^0.2.4","style-loader":"^3.3.3","svg-url-loader":"~3.0.3","ts-jest":"^28.0.8","ts-loader":"^6.0.4","typescript":"~4.2.4","url-loader":"^4.1.0","webpack":"^5.88.2","webpack-cli":"^4.4.0"},"jupyterlab":{"extension":"lib/plugin","webpackConfig":"webpack.lab.config.js","outputDir":"./ipydatagrid/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true},"bqplot":{"bundled":false,"singleton":true},"@lumino/algorithm":{"bundled":false,"singleton":true},"@lumino/commands":{"bundled":false,"singleton":true},"@lumino/coreutils":{"bundled":false,"singleton":true},"@lumino/datagrid":{"bundled":false,"singleton":true},"@lumino/default-theme":{"bundled":false,"singleton":true},"@lumino/domutils":{"bundled":false,"singleton":true},"@lumino/messaging":{"bundled":false,"singleton":true},"@lumino/virtualdom":{"bundled":false,"singleton":true},"@lumino/widgets":{"bundled":false,"singleton":true}}},"packageManager":"yarn@3.7.0"}')
+            e.exports = JSON.parse('{"name":"ipydatagrid","version":"1.3.2","description":"Fast Datagrid widget for the Jupyter Notebook and JupyterLab","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","lib/**/*.js.map","lib/**/*.ts","dist/*.js","dist/*.js.map","dist/*.png","style/**/*.*"],"homepage":"https://github.com/Bloomberg/ipydatagrid","bugs":{"url":"https://github.com/Bloomberg/ipydatagrid/issues"},"license":"BSD-3-Clause","author":{"name":"Bloomberg","email":""},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/Bloomberg/ipydatagrid"},"scripts":{"build":"jlpm run build:lib && jlpm run build:nbextension && jlpm run build:labextension","build:dev":"jlpm run build:lib && jlpm run build:nbextension && jlpm run build:labextension:dev","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack --mode=production --no-devtool","build:widget-examples":"cd widget-examples/basic && webpack --mode=production","build:all":"jlpm run build:labextension && jlpm run build:nbextension && jlpm run build:widget-examples","clean":"rimraf dist && jlpm run clean:lib && jlpm run clean:labextension && jlpm run clean:nbextension","clean:lib":"rimraf lib","clean:labextension":"rimraf ipydatagrid/labextension","clean:nbextension":"rimraf ipydatagrid/nbextension/index.*","lint":"eslint \'js/**/*.{js,ts}\' --quiet --fix","prepack":"jlpm run build:labextension && jlpm run build:nbextension","test":"jest --verbose","watch":"npm-run-all -p watch:lib watch:labextension watch:nbextension","watch:lib":"tsc -w","watch:nbextension":"webpack --watch","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^2 || ^3 || ^4 || ^6","@jupyterlab/apputils":"^3 || ^4","@lumino/algorithm":"^1 || ^2","@lumino/application":"^1 || ^2","@lumino/commands":"^1 || ^2","@lumino/coreutils":"^1 || ^2","@lumino/datagrid":"^1 || ^2","@lumino/default-theme":"^1 || ^2","@lumino/domutils":"^1 || ^2","@lumino/messaging":"^1 || ^2","@lumino/signaling":"^1 || ^2","@lumino/virtualdom":"^1 || ^2","@lumino/widgets":"^1 || ^2","bqplot":"^0.5","core-js-pure":"^3.30.2","d3-array":"^2.2.0","d3-color":"^3.1.0","d3-format":"^1.3.2","d3-scale":"^3.0.0","d3-time-format":"^2.1.3","jest-environment-jsdom":"^28.1.3","moment":"^2.24.0","underscore":"^1.13.6","vega-expression":"^2.6.0","vega-format":"^1.1.1","vega-functions":"^5.3.0"},"devDependencies":{"@babel/cli":"^7.6.3","@babel/core":"^7.6.3","@babel/preset-env":"^7.6.3","@babel/preset-typescript":"^7.6.0","@jupyterlab/builder":"^4.0.5","@types/jest":"^27.4.1","@types/node":"^10.11.6","@types/underscore":"^1.11.4","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.5.0","@typescript-eslint/parser":"^3.5.0","acorn":"^6.2.0","babel-jest":"^28.1.3","babel-plugin-transform-es2015-modules-commonjs":"^6.26.2","css-loader":"^6.8.1","eslint":"^7.3.1","eslint-config-prettier":"^6.11.0","eslint-plugin-prettier":"^3.1.4","fs-extra":"^7.0.0","jest":"^28.1.3","jest-raw-loader":"^1.0.1","lint-staged":"^10.2.11","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.0.5","raw-loader":"^4.0.2","rimraf":"^2.6.2","source-map-loader":"^0.2.4","style-loader":"^3.3.3","svg-url-loader":"~3.0.3","ts-jest":"^28.0.8","ts-loader":"^6.0.4","typescript":"~4.2.4","url-loader":"^4.1.0","webpack":"^5.88.2","webpack-cli":"^4.4.0"},"jupyterlab":{"extension":"lib/plugin","webpackConfig":"webpack.lab.config.js","outputDir":"./ipydatagrid/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true},"bqplot":{"bundled":false,"singleton":true},"@lumino/algorithm":{"bundled":false,"singleton":true},"@lumino/commands":{"bundled":false,"singleton":true},"@lumino/coreutils":{"bundled":false,"singleton":true},"@lumino/datagrid":{"bundled":false,"singleton":true},"@lumino/default-theme":{"bundled":false,"singleton":true},"@lumino/domutils":{"bundled":false,"singleton":true},"@lumino/messaging":{"bundled":false,"singleton":true},"@lumino/virtualdom":{"bundled":false,"singleton":true},"@lumino/widgets":{"bundled":false,"singleton":true}}},"packageManager":"yarn@3.7.0"}')
         }
     }
 ]);
```

### Comparing `ipydatagrid-1.3.1/ipydatagrid/labextension/static/794.d7c23e15137c8752365e.js` & `ipydatagrid-1.3.2/ipydatagrid/labextension/static/794.d7c23e15137c8752365e.js`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.1/ipydatagrid/labextension/static/811.a135ebc21be585e6d76d.js` & `ipydatagrid-1.3.2/ipydatagrid/labextension/static/811.a135ebc21be585e6d76d.js`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.1/ipydatagrid/labextension/static/823.18e09aad57c7797df987.js` & `ipydatagrid-1.3.2/ipydatagrid/labextension/static/823.18e09aad57c7797df987.js`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.1/ipydatagrid/labextension/static/917.b972bc5b41fae8990bff.js` & `ipydatagrid-1.3.2/ipydatagrid/labextension/static/917.b972bc5b41fae8990bff.js`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.1/ipydatagrid/labextension/static/939.04c5876588e4898127e3.js` & `ipydatagrid-1.3.2/ipydatagrid/labextension/static/939.04c5876588e4898127e3.js`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.1/ipydatagrid/labextension/static/941.23c8b1f0eb18afd531e9.js` & `ipydatagrid-1.3.2/ipydatagrid/labextension/static/941.23c8b1f0eb18afd531e9.js`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.1/ipydatagrid/labextension/static/990.e35c256305f259cdaeb9.js` & `ipydatagrid-1.3.2/ipydatagrid/labextension/static/990.e35c256305f259cdaeb9.js`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.1/ipydatagrid/labextension/static/remoteEntry.6d509d1468636d15eab8.js` & `ipydatagrid-1.3.2/ipydatagrid/labextension/static/remoteEntry.91868686b1e0561ea123.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -52,15 +52,15 @@
         109: "bdd9793b392cc2fe87da",
         112: "4ddba6fd51d10d391fa0",
         142: "025e64e0cbb8aa528385",
         143: "171db67c9b56d395ae64",
         159: "40dbdd4ec4a2fec3a0e0",
         268: "88ce57d2bfbde9012162",
         271: "c6d995708c863e1b27ed",
-        296: "d2eeaa2e543e597ac586",
+        296: "59cf43ce555ff3a1e3f1",
         351: "372e5eec3c9010a57cf3",
         400: "95b73fc6eb3f120b823f",
         433: "75ed253aaa8060b28c81",
         455: "25b625d30041b5a1671c",
         456: "afd75d5e116998d22e56",
         462: "68e4d74f02bf2411528e",
         481: "911a23288443c8041987",
@@ -71,15 +71,15 @@
         643: "a265dd26cb50ebd06923",
         679: "e174128fe156c1cd0d10",
         683: "efe59705c1680a8f8b3a",
         689: "3cdb49d94599b1683563",
         700: "7f792a9e7380bfde28dc",
         762: "42901b906691b1301214",
         781: "ef3f9c2a235c4a40bdc0",
-        787: "47c1e167bb24294e1e7e",
+        787: "b52e0074e2cbca59f4b7",
         794: "d7c23e15137c8752365e",
         811: "a135ebc21be585e6d76d",
         823: "18e09aad57c7797df987",
         917: "b972bc5b41fae8990bff",
         939: "04c5876588e4898127e3",
         941: "23c8b1f0eb18afd531e9",
         990: "e35c256305f259cdaeb9"
@@ -89,15 +89,15 @@
         109: "bdd9793b392cc2fe87da",
         112: "4ddba6fd51d10d391fa0",
         142: "025e64e0cbb8aa528385",
         143: "171db67c9b56d395ae64",
         159: "40dbdd4ec4a2fec3a0e0",
         268: "88ce57d2bfbde9012162",
         271: "c6d995708c863e1b27ed",
-        296: "d2eeaa2e543e597ac586",
+        296: "59cf43ce555ff3a1e3f1",
         351: "372e5eec3c9010a57cf3",
         400: "95b73fc6eb3f120b823f",
         433: "75ed253aaa8060b28c81",
         455: "25b625d30041b5a1671c",
         456: "afd75d5e116998d22e56",
         462: "68e4d74f02bf2411528e",
         481: "911a23288443c8041987",
@@ -108,15 +108,15 @@
         643: "a265dd26cb50ebd06923",
         679: "e174128fe156c1cd0d10",
         683: "efe59705c1680a8f8b3a",
         689: "3cdb49d94599b1683563",
         700: "7f792a9e7380bfde28dc",
         762: "42901b906691b1301214",
         781: "ef3f9c2a235c4a40bdc0",
-        787: "47c1e167bb24294e1e7e",
+        787: "b52e0074e2cbca59f4b7",
         794: "d7c23e15137c8752365e",
         811: "a135ebc21be585e6d76d",
         823: "18e09aad57c7797df987",
         917: "b972bc5b41fae8990bff",
         939: "04c5876588e4898127e3",
         941: "23c8b1f0eb18afd531e9",
         990: "e35c256305f259cdaeb9"
@@ -175,15 +175,15 @@
                         (!f || !f.loaded && (!r != !f.eager ? r : o > f.from)) && (d[a] = {
                             get: t,
                             from: o,
                             eager: !!r
                         })
                     },
                     i = [];
-                return "default" === t && (f("d3-array", "3.2.4", (() => P.e(433).then((() => () => P(3433))))), f("d3-array", "3.2.4", (() => P.e(455).then((() => () => P(2455))))), f("d3-array", "3.2.4", (() => P.e(513).then((() => () => P(5513))))), f("d3-array", "3.2.4", (() => P.e(643).then((() => () => P(8643))))), f("d3-array", "3.2.4", (() => P.e(41).then((() => () => P(8041))))), f("d3-array", "3.2.4", (() => P.e(109).then((() => () => P(109))))), f("d3-color", "3.1.0", (() => P.e(811).then((() => () => P(4811))))), f("d3-format", "1.4.5", (() => P.e(481).then((() => () => P(8481))))), f("d3-format", "3.1.0", (() => P.e(142).then((() => () => P(2142))))), f("d3-format", "3.1.0", (() => P.e(462).then((() => () => P(7271))))), f("d3-scale", "4.0.2", (() => Promise.all([P.e(781), P.e(622), P.e(112), P.e(456)]).then((() => () => P(2781))))), f("d3-time-format", "2.3.0", (() => P.e(48).then((() => () => P(4048))))), f("d3-time-format", "4.1.0", (() => P.e(941).then((() => () => P(6941))))), f("d3-time-format", "4.1.0", (() => P.e(683).then((() => () => P(271))))), f("ipydatagrid", "1.3.1", (() => Promise.all([P.e(939), P.e(268), P.e(787), P.e(568)]).then((() => () => P(1568))))), f("moment", "2.29.4", (() => Promise.all([P.e(762), P.e(700)]).then((() => () => P(381))))), f("underscore", "1.13.6", (() => P.e(794).then((() => () => P(7794))))), f("vega-expression", "2.7.0", (() => P.e(351).then((() => () => P(6351))))), f("vega-expression", "5.1.0", (() => Promise.all([P.e(143), P.e(823)]).then((() => () => P(8143))))), f("vega-expression", "5.1.0", (() => Promise.all([P.e(917), P.e(990)]).then((() => () => P(9917))))), f("vega-format", "1.1.1", (() => Promise.all([P.e(642), P.e(689), P.e(400)]).then((() => () => P(7400))))), f("vega-functions", "5.14.0", (() => Promise.all([P.e(642), P.e(679), P.e(268), P.e(622), P.e(689), P.e(159)]).then((() => () => P(679)))))), e[t] = i.length ? Promise.all(i).then((() => e[t] = 1)) : 1
+                return "default" === t && (f("d3-array", "3.2.4", (() => P.e(433).then((() => () => P(3433))))), f("d3-array", "3.2.4", (() => P.e(455).then((() => () => P(2455))))), f("d3-array", "3.2.4", (() => P.e(513).then((() => () => P(5513))))), f("d3-array", "3.2.4", (() => P.e(643).then((() => () => P(8643))))), f("d3-array", "3.2.4", (() => P.e(41).then((() => () => P(8041))))), f("d3-array", "3.2.4", (() => P.e(109).then((() => () => P(109))))), f("d3-color", "3.1.0", (() => P.e(811).then((() => () => P(4811))))), f("d3-format", "1.4.5", (() => P.e(481).then((() => () => P(8481))))), f("d3-format", "3.1.0", (() => P.e(142).then((() => () => P(2142))))), f("d3-format", "3.1.0", (() => P.e(462).then((() => () => P(7271))))), f("d3-scale", "4.0.2", (() => Promise.all([P.e(781), P.e(622), P.e(112), P.e(456)]).then((() => () => P(2781))))), f("d3-time-format", "2.3.0", (() => P.e(48).then((() => () => P(4048))))), f("d3-time-format", "4.1.0", (() => P.e(941).then((() => () => P(6941))))), f("d3-time-format", "4.1.0", (() => P.e(683).then((() => () => P(271))))), f("ipydatagrid", "1.3.2", (() => Promise.all([P.e(939), P.e(268), P.e(787), P.e(568)]).then((() => () => P(1568))))), f("moment", "2.29.4", (() => Promise.all([P.e(762), P.e(700)]).then((() => () => P(381))))), f("underscore", "1.13.6", (() => P.e(794).then((() => () => P(7794))))), f("vega-expression", "2.7.0", (() => P.e(351).then((() => () => P(6351))))), f("vega-expression", "5.1.0", (() => Promise.all([P.e(143), P.e(823)]).then((() => () => P(8143))))), f("vega-expression", "5.1.0", (() => Promise.all([P.e(917), P.e(990)]).then((() => () => P(9917))))), f("vega-format", "1.1.1", (() => Promise.all([P.e(642), P.e(689), P.e(400)]).then((() => () => P(7400))))), f("vega-functions", "5.14.0", (() => Promise.all([P.e(642), P.e(679), P.e(268), P.e(622), P.e(689), P.e(159)]).then((() => () => P(679)))))), e[t] = i.length ? Promise.all(i).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         P.g.importScripts && (e = P.g.location + "");
         var a = P.g.document;
         if (!e && a && (a.currentScript && (e = a.currentScript.src), !e)) {
@@ -306,15 +306,15 @@
         ]),
         6697: () => b("default", "@lumino/algorithm", [1, 2, 0, 0]),
         7120: () => b("default", "@lumino/commands", [1, 2, 0, 1]),
         7831: () => p("default", "d3-time-format", [1, 2, 1, 3], (() => P.e(48).then((() => () => P(4048))))),
         7930: () => b("default", "@lumino/coreutils", [1, 2, 0, 0]),
         8624: () => p("default", "vega-functions", [1, 5, 3, 0], (() => Promise.all([P.e(642), P.e(679), P.e(622), P.e(689), P.e(159)]).then((() => () => P(679))))),
         9704: () => p("default", "vega-expression", [1, 2, 6, 0], (() => P.e(351).then((() => () => P(6351))))),
-        1464: () => b("default", "@jupyterlab/apputils", [1, 4, 2, 6]),
+        3712: () => b("default", "@jupyterlab/apputils", [1, 4, 3, 0]),
         3622: () => p("default", "d3-color", [, [1, 3],
             [-1, 3], 1, [0, 1], 2
         ], (() => P.e(811).then((() => () => P(4811))))),
         1573: () => p("default", "d3-array", [, [1, 3],
             [-1, 3], 1, [0, 2, 10, 0], 2
         ], (() => P.e(513).then((() => () => P(5513))))),
         3919: () => p("default", "d3-array", [, [1, 3],
@@ -340,15 +340,15 @@
         6476: () => p("default", "vega-expression", [1, 5, 1, 0], (() => P.e(143).then((() => () => P(8143))))),
         8581: () => p("default", "d3-array", [1, 3, 2, 2], (() => P.e(41).then((() => () => P(8041))))),
         8933: () => p("default", "d3-array", [4, 3, 2, 4], (() => P.e(643).then((() => () => P(8643)))))
     }, g = {
         112: [1573, 3919, 4603, 5551],
         159: [127, 519, 2112, 4620, 4826, 6476, 8581, 8933],
         268: [2969, 6886],
-        296: [1464],
+        296: [3712],
         400: [2257, 7751, 7868],
         622: [3622],
         689: [689],
         787: [2297, 2544, 4031, 4059, 4882, 4901, 5058, 5593, 5633, 6479, 6664, 6697, 7120, 7831, 7930, 8624, 9704]
     }, P.f.consumes = (e, a) => {
         P.o(g, e) && g[e].forEach((e => {
             if (P.o(m, e)) return a.push(m[e]);
```

### Comparing `ipydatagrid-1.3.1/ipydatagrid/labextension/static/third-party-licenses.json` & `ipydatagrid-1.3.2/ipydatagrid/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.1/ipydatagrid/nbextension/index.js` & `ipydatagrid-1.3.2/ipydatagrid/nbextension/index.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -90091,15 +90091,14 @@
                                 break;
                             case "cell-edit-event":
                                 const e = this.get("_data");
                                 e.data[t.column][t.row] = t.value, this.set("_data", e), this.send({
                                     event_type: "cell-changed",
                                     region: t.region,
                                     row: t.row,
-                                    column: t.column,
                                     column_index: t.columnIndex,
                                     value: t.value
                                 }, Object.assign({}, this._view_callbacks));
                                 break;
                             default:
                                 throw "unreachable"
                         }
@@ -90194,15 +90193,26 @@
                                     const i = new Array(t.length);
                                     let r = 0;
                                     for (const n of t) i[r++] = n[e];
                                     n[e] = i
                                 }
                                 return new g.DataSource(n, e.fields, e.schema, !0)
                             }
-                            for (const i of Object.keys(e.data)) n[i] = [], Array.isArray(e.data[i]) ? n[i] = e.data[i] : "raw" == e.data[i].type ? n[i] = y(e.data[i].value) : 0 !== e.data[i].value.length && (n[i] = d.array_or_json_serializer.deserialize(e.data[i], t));
+                            for (const i of Object.keys(e.data))
+                                if (n[i] = [], Array.isArray(e.data[i])) n[i] = e.data[i];
+                                else if ("raw" == e.data[i].type) n[i] = y(e.data[i].value);
+                            else if (0 !== e.data[i].value.length) {
+                                let r = d.array_or_json_serializer.deserialize(e.data[i], t);
+                                if ("date" === r.type) {
+                                    const e = r;
+                                    r = [];
+                                    for (let t = 0; t < e.length; t++) r[t] = new Date(e[t]).toISOString()
+                                }
+                                n[i] = r
+                            }
                             return new g.DataSource(n, e.fields, e.schema, !0)
                         },
                         serialize: function(e, t) {
                             const n = {};
                             for (const i of Object.keys(e.data)) n[i] = d.array_or_json_serializer.serialize(e.data[i], t);
                             return {
                                 data: n,
@@ -93267,15 +93277,15 @@
                 "use strict";
                 e.exports = {
                     version: "0.5.43"
                 }
             },
             4147: e => {
                 "use strict";
-                e.exports = JSON.parse('{"name":"ipydatagrid","version":"1.3.1","description":"Fast Datagrid widget for the Jupyter Notebook and JupyterLab","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","lib/**/*.js.map","lib/**/*.ts","dist/*.js","dist/*.js.map","dist/*.png","style/**/*.*"],"homepage":"https://github.com/Bloomberg/ipydatagrid","bugs":{"url":"https://github.com/Bloomberg/ipydatagrid/issues"},"license":"BSD-3-Clause","author":{"name":"Bloomberg","email":""},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/Bloomberg/ipydatagrid"},"scripts":{"build":"jlpm run build:lib && jlpm run build:nbextension && jlpm run build:labextension","build:dev":"jlpm run build:lib && jlpm run build:nbextension && jlpm run build:labextension:dev","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack --mode=production --no-devtool","build:widget-examples":"cd widget-examples/basic && webpack --mode=production","build:all":"jlpm run build:labextension && jlpm run build:nbextension && jlpm run build:widget-examples","clean":"rimraf dist && jlpm run clean:lib && jlpm run clean:labextension && jlpm run clean:nbextension","clean:lib":"rimraf lib","clean:labextension":"rimraf ipydatagrid/labextension","clean:nbextension":"rimraf ipydatagrid/nbextension/index.*","lint":"eslint \'js/**/*.{js,ts}\' --quiet --fix","prepack":"jlpm run build:labextension && jlpm run build:nbextension","test":"jest --verbose","watch":"npm-run-all -p watch:lib watch:labextension watch:nbextension","watch:lib":"tsc -w","watch:nbextension":"webpack --watch","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^2 || ^3 || ^4 || ^6","@jupyterlab/apputils":"^3 || ^4","@lumino/algorithm":"^1 || ^2","@lumino/application":"^1 || ^2","@lumino/commands":"^1 || ^2","@lumino/coreutils":"^1 || ^2","@lumino/datagrid":"^1 || ^2","@lumino/default-theme":"^1 || ^2","@lumino/domutils":"^1 || ^2","@lumino/messaging":"^1 || ^2","@lumino/signaling":"^1 || ^2","@lumino/virtualdom":"^1 || ^2","@lumino/widgets":"^1 || ^2","bqplot":"^0.5","core-js-pure":"^3.30.2","d3-array":"^2.2.0","d3-color":"^3.1.0","d3-format":"^1.3.2","d3-scale":"^3.0.0","d3-time-format":"^2.1.3","jest-environment-jsdom":"^28.1.3","moment":"^2.24.0","underscore":"^1.13.6","vega-expression":"^2.6.0","vega-format":"^1.1.1","vega-functions":"^5.3.0"},"devDependencies":{"@babel/cli":"^7.6.3","@babel/core":"^7.6.3","@babel/preset-env":"^7.6.3","@babel/preset-typescript":"^7.6.0","@jupyterlab/builder":"^4.0.5","@types/jest":"^27.4.1","@types/node":"^10.11.6","@types/underscore":"^1.11.4","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.5.0","@typescript-eslint/parser":"^3.5.0","acorn":"^6.2.0","babel-jest":"^28.1.3","babel-plugin-transform-es2015-modules-commonjs":"^6.26.2","css-loader":"^6.8.1","eslint":"^7.3.1","eslint-config-prettier":"^6.11.0","eslint-plugin-prettier":"^3.1.4","fs-extra":"^7.0.0","jest":"^28.1.3","jest-raw-loader":"^1.0.1","lint-staged":"^10.2.11","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.0.5","raw-loader":"^4.0.2","rimraf":"^2.6.2","source-map-loader":"^0.2.4","style-loader":"^3.3.3","svg-url-loader":"~3.0.3","ts-jest":"^28.0.8","ts-loader":"^6.0.4","typescript":"~4.2.4","url-loader":"^4.1.0","webpack":"^5.88.2","webpack-cli":"^4.4.0"},"jupyterlab":{"extension":"lib/plugin","webpackConfig":"webpack.lab.config.js","outputDir":"./ipydatagrid/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true},"bqplot":{"bundled":false,"singleton":true},"@lumino/algorithm":{"bundled":false,"singleton":true},"@lumino/commands":{"bundled":false,"singleton":true},"@lumino/coreutils":{"bundled":false,"singleton":true},"@lumino/datagrid":{"bundled":false,"singleton":true},"@lumino/default-theme":{"bundled":false,"singleton":true},"@lumino/domutils":{"bundled":false,"singleton":true},"@lumino/messaging":{"bundled":false,"singleton":true},"@lumino/virtualdom":{"bundled":false,"singleton":true},"@lumino/widgets":{"bundled":false,"singleton":true}}},"packageManager":"yarn@3.7.0"}')
+                e.exports = JSON.parse('{"name":"ipydatagrid","version":"1.3.2","description":"Fast Datagrid widget for the Jupyter Notebook and JupyterLab","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","lib/**/*.js.map","lib/**/*.ts","dist/*.js","dist/*.js.map","dist/*.png","style/**/*.*"],"homepage":"https://github.com/Bloomberg/ipydatagrid","bugs":{"url":"https://github.com/Bloomberg/ipydatagrid/issues"},"license":"BSD-3-Clause","author":{"name":"Bloomberg","email":""},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/Bloomberg/ipydatagrid"},"scripts":{"build":"jlpm run build:lib && jlpm run build:nbextension && jlpm run build:labextension","build:dev":"jlpm run build:lib && jlpm run build:nbextension && jlpm run build:labextension:dev","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack --mode=production --no-devtool","build:widget-examples":"cd widget-examples/basic && webpack --mode=production","build:all":"jlpm run build:labextension && jlpm run build:nbextension && jlpm run build:widget-examples","clean":"rimraf dist && jlpm run clean:lib && jlpm run clean:labextension && jlpm run clean:nbextension","clean:lib":"rimraf lib","clean:labextension":"rimraf ipydatagrid/labextension","clean:nbextension":"rimraf ipydatagrid/nbextension/index.*","lint":"eslint \'js/**/*.{js,ts}\' --quiet --fix","prepack":"jlpm run build:labextension && jlpm run build:nbextension","test":"jest --verbose","watch":"npm-run-all -p watch:lib watch:labextension watch:nbextension","watch:lib":"tsc -w","watch:nbextension":"webpack --watch","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^2 || ^3 || ^4 || ^6","@jupyterlab/apputils":"^3 || ^4","@lumino/algorithm":"^1 || ^2","@lumino/application":"^1 || ^2","@lumino/commands":"^1 || ^2","@lumino/coreutils":"^1 || ^2","@lumino/datagrid":"^1 || ^2","@lumino/default-theme":"^1 || ^2","@lumino/domutils":"^1 || ^2","@lumino/messaging":"^1 || ^2","@lumino/signaling":"^1 || ^2","@lumino/virtualdom":"^1 || ^2","@lumino/widgets":"^1 || ^2","bqplot":"^0.5","core-js-pure":"^3.30.2","d3-array":"^2.2.0","d3-color":"^3.1.0","d3-format":"^1.3.2","d3-scale":"^3.0.0","d3-time-format":"^2.1.3","jest-environment-jsdom":"^28.1.3","moment":"^2.24.0","underscore":"^1.13.6","vega-expression":"^2.6.0","vega-format":"^1.1.1","vega-functions":"^5.3.0"},"devDependencies":{"@babel/cli":"^7.6.3","@babel/core":"^7.6.3","@babel/preset-env":"^7.6.3","@babel/preset-typescript":"^7.6.0","@jupyterlab/builder":"^4.0.5","@types/jest":"^27.4.1","@types/node":"^10.11.6","@types/underscore":"^1.11.4","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.5.0","@typescript-eslint/parser":"^3.5.0","acorn":"^6.2.0","babel-jest":"^28.1.3","babel-plugin-transform-es2015-modules-commonjs":"^6.26.2","css-loader":"^6.8.1","eslint":"^7.3.1","eslint-config-prettier":"^6.11.0","eslint-plugin-prettier":"^3.1.4","fs-extra":"^7.0.0","jest":"^28.1.3","jest-raw-loader":"^1.0.1","lint-staged":"^10.2.11","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.0.5","raw-loader":"^4.0.2","rimraf":"^2.6.2","source-map-loader":"^0.2.4","style-loader":"^3.3.3","svg-url-loader":"~3.0.3","ts-jest":"^28.0.8","ts-loader":"^6.0.4","typescript":"~4.2.4","url-loader":"^4.1.0","webpack":"^5.88.2","webpack-cli":"^4.4.0"},"jupyterlab":{"extension":"lib/plugin","webpackConfig":"webpack.lab.config.js","outputDir":"./ipydatagrid/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true},"bqplot":{"bundled":false,"singleton":true},"@lumino/algorithm":{"bundled":false,"singleton":true},"@lumino/commands":{"bundled":false,"singleton":true},"@lumino/coreutils":{"bundled":false,"singleton":true},"@lumino/datagrid":{"bundled":false,"singleton":true},"@lumino/default-theme":{"bundled":false,"singleton":true},"@lumino/domutils":{"bundled":false,"singleton":true},"@lumino/messaging":{"bundled":false,"singleton":true},"@lumino/virtualdom":{"bundled":false,"singleton":true},"@lumino/widgets":{"bundled":false,"singleton":true}}},"packageManager":"yarn@3.7.0"}')
             }
         },
         n = {};
 
     function i(e) {
         var r = n[e];
         if (void 0 !== r) return r.exports;
```

### Comparing `ipydatagrid-1.3.1/ipydatagrid/nbextension/index.js.LICENSE.txt` & `ipydatagrid-1.3.2/ipydatagrid/nbextension/index.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.1/js/cellrenderer.ts` & `ipydatagrid-1.3.2/js/cellrenderer.ts`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.1/js/datagrid.ts` & `ipydatagrid-1.3.2/js/datagrid.ts`

 * *Files 1% similar despite different names*

```diff
@@ -115,18 +115,30 @@
       continue;
     }
 
     if (data.data[column].type == 'raw') {
       deserialized_data[column] = unpack_raw_data(data.data[column].value);
     } else {
       if (data.data[column].value.length !== 0) {
-        deserialized_data[column] = array_or_json_serializer.deserialize(
+        let deserialized_array = array_or_json_serializer.deserialize(
           data.data[column],
           manager,
         );
+
+        // Turning back float32 dates into isoformat
+        if (deserialized_array.type === 'date') {
+          const float32Array = deserialized_array;
+          deserialized_array = [];
+
+          for (let i = 0; i < float32Array.length; i++) {
+            deserialized_array[i] = new Date(float32Array[i]).toISOString();
+          }
+        }
+
+        deserialized_data[column] = deserialized_array;
       }
     }
   }
   return new DataSource(deserialized_data, data.fields, data.schema, true);
 }
 
 export class DataGridModel extends DOMWidgetModel {
@@ -203,15 +215,14 @@
         this.set('_data', newData);
 
         this.send(
           {
             event_type: 'cell-changed',
             region: msg.region,
             row: msg.row,
-            column: msg.column,
             column_index: msg.columnIndex,
             value: msg.value,
           },
           { ...this._view_callbacks },
         );
         break;
       default:
```

### Comparing `ipydatagrid-1.3.1/js/datasource.ts` & `ipydatagrid-1.3.2/js/datasource.ts`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.1/js/extension.ts` & `ipydatagrid-1.3.2/js/extension.ts`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.1/js/feathergrid.ts` & `ipydatagrid-1.3.2/js/feathergrid.ts`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.1/js/keyhandler.ts` & `ipydatagrid-1.3.2/js/keyhandler.ts`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.1/js/mousehandler.ts` & `ipydatagrid-1.3.2/js/mousehandler.ts`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.1/js/plugin.ts` & `ipydatagrid-1.3.2/js/plugin.ts`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.1/js/utils.ts` & `ipydatagrid-1.3.2/js/utils.ts`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.1/js/vegaexpr.ts` & `ipydatagrid-1.3.2/js/vegaexpr.ts`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.1/js/core/barrenderer.ts` & `ipydatagrid-1.3.2/js/core/barrenderer.ts`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.1/js/core/filterMenu.ts` & `ipydatagrid-1.3.2/js/core/filterMenu.ts`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.1/js/core/gridContextMenu.ts` & `ipydatagrid-1.3.2/js/core/gridContextMenu.ts`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.1/js/core/headerRenderer.ts` & `ipydatagrid-1.3.2/js/core/headerRenderer.ts`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.1/js/core/htmlRenderer.ts` & `ipydatagrid-1.3.2/js/core/htmlRenderer.ts`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.1/js/core/transform.ts` & `ipydatagrid-1.3.2/js/core/transform.ts`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.1/js/core/transformExecutors.ts` & `ipydatagrid-1.3.2/js/core/transformExecutors.ts`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.1/js/core/transformStateManager.ts` & `ipydatagrid-1.3.2/js/core/transformStateManager.ts`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.1/js/core/valueRenderer.ts` & `ipydatagrid-1.3.2/js/core/valueRenderer.ts`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.1/js/core/view.ts` & `ipydatagrid-1.3.2/js/core/view.ts`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.1/js/core/viewbasedjsonmodel.ts` & `ipydatagrid-1.3.2/js/core/viewbasedjsonmodel.ts`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.1/static/ipydatagrid_1.gif` & `ipydatagrid-1.3.2/static/ipydatagrid_1.gif`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.1/static/ipydatagrid_2.gif` & `ipydatagrid-1.3.2/static/ipydatagrid_2.gif`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.1/static/ipydatagrid_3.gif` & `ipydatagrid-1.3.2/static/ipydatagrid_3.gif`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.1/static/ipydatagrid_4.gif` & `ipydatagrid-1.3.2/static/ipydatagrid_4.gif`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.1/static/ipydatagrid_5.gif` & `ipydatagrid-1.3.2/static/ipydatagrid_5.gif`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.1/style/feathergrid.css` & `ipydatagrid-1.3.2/style/feathergrid.css`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.1/.gitignore` & `ipydatagrid-1.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.1/LICENSE.txt` & `ipydatagrid-1.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.1/README.md` & `ipydatagrid-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `ipydatagrid-1.3.1/pyproject.toml` & `ipydatagrid-1.3.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 requires = [
   "hatchling>=1.18",
   "jupyterlab>=4.0.5",
 ]
 
 [project]
 name = "ipydatagrid"
-version = "1.3.1"
+version = "1.3.2"
 description = "Fast Datagrid widget for the Jupyter Notebook and JupyterLab"
 readme = "README.md"
 keywords = [
   "IPython",
   "Jupyter",
   "Widgets",
 ]
@@ -115,15 +115,15 @@
 [tool.tbump]
 field = [
     { name = "channel", default = "" },
     { name = "release", default = "" },
 ]
 
 [tool.tbump.version]
-current = "1.3.1"
+current = "1.3.2"
 regex = "(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)((?P<channel>a|b|rc|.dev)(?P<release>\\d+))?"
 
 [tool.tbump.git]
 message_template = "Bump to {new_version}"
 tag_template = "v{new_version}"
 
 [[tool.tbump.file]]
```

### Comparing `ipydatagrid-1.3.1/PKG-INFO` & `ipydatagrid-1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ipydatagrid
-Version: 1.3.1
+Version: 1.3.2
 Summary: Fast Datagrid widget for the Jupyter Notebook and JupyterLab
 Project-URL: Homepage, https://github.com/bloomberg/ipydatagrid
 Author: Bloomberg
 License-File: LICENSE.txt
 Keywords: IPython,Jupyter,Widgets
 Classifier: Framework :: Jupyter
 Classifier: Intended Audience :: Developers
```

