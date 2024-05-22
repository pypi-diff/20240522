# Comparing `tmp/jupyterlab_language_pack_zh_cn-4.1.post2.tar.gz` & `tmp/jupyterlab_language_pack_zh_cn-4.2.post0.tar.gz`

## Comparing `jupyterlab_language_pack_zh_cn-4.1.post2.tar` & `jupyterlab_language_pack_zh_cn-4.2.post0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 jupyterlab_language_pack_zh_cn-4.1.post2/.copier-answers.yml
--rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 jupyterlab_language_pack_zh_cn-4.1.post2/CONTRIBUTORS.md
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 jupyterlab_language_pack_zh_cn-4.1.post2/jupyterlab_language_pack_zh_CN/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_language_pack_zh_cn-4.1.post2/jupyterlab_language_pack_zh_CN/locale/zh_CN/LC_MESSAGES/.gitkeep
--rw-r--r--   0        0        0     5146 2020-02-02 00:00:00.000000 jupyterlab_language_pack_zh_cn-4.1.post2/jupyterlab_language_pack_zh_CN/locale/zh_CN/LC_MESSAGES/dask_labextension.po
--rw-r--r--   0        0        0     3136 2020-02-02 00:00:00.000000 jupyterlab_language_pack_zh_cn-4.1.post2/jupyterlab_language_pack_zh_CN/locale/zh_CN/LC_MESSAGES/jupyter_archive.po
--rw-r--r--   0        0        0     5313 2020-02-02 00:00:00.000000 jupyterlab_language_pack_zh_cn-4.1.post2/jupyterlab_language_pack_zh_CN/locale/zh_CN/LC_MESSAGES/jupyter_collaboration.po
--rw-r--r--   0        0        0    10223 2020-02-02 00:00:00.000000 jupyterlab_language_pack_zh_cn-4.1.post2/jupyterlab_language_pack_zh_CN/locale/zh_CN/LC_MESSAGES/jupyter_resource_usage.po
--rw-r--r--   0        0        0   255704 2020-02-02 00:00:00.000000 jupyterlab_language_pack_zh_cn-4.1.post2/jupyterlab_language_pack_zh_CN/locale/zh_CN/LC_MESSAGES/jupyterlab.po
--rw-r--r--   0        0        0   149651 2020-02-02 00:00:00.000000 jupyterlab_language_pack_zh_cn-4.1.post2/jupyterlab_language_pack_zh_CN/locale/zh_CN/LC_MESSAGES/jupyterlab_git.po
--rw-r--r--   0        0        0    64794 2020-02-02 00:00:00.000000 jupyterlab_language_pack_zh_cn-4.1.post2/jupyterlab_language_pack_zh_CN/locale/zh_CN/LC_MESSAGES/jupyterlab_lsp.po
--rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 jupyterlab_language_pack_zh_cn-4.1.post2/jupyterlab_language_pack_zh_CN/locale/zh_CN/LC_MESSAGES/jupyterlab_recents.po
--rw-r--r--   0        0        0     5825 2020-02-02 00:00:00.000000 jupyterlab_language_pack_zh_cn-4.1.post2/jupyterlab_language_pack_zh_CN/locale/zh_CN/LC_MESSAGES/jupyterlab_search_replace.po
--rw-r--r--   0        0        0     3652 2020-02-02 00:00:00.000000 jupyterlab_language_pack_zh_cn-4.1.post2/jupyterlab_language_pack_zh_CN/locale/zh_CN/LC_MESSAGES/jupyterlab_spreadsheet_editor.po
--rw-r--r--   0        0        0    16924 2020-02-02 00:00:00.000000 jupyterlab_language_pack_zh_cn-4.1.post2/jupyterlab_language_pack_zh_CN/locale/zh_CN/LC_MESSAGES/jupyterlab_tour.po
--rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 jupyterlab_language_pack_zh_cn-4.1.post2/jupyterlab_language_pack_zh_CN/locale/zh_CN/LC_MESSAGES/jupyterlab_widgets.po
--rw-r--r--   0        0        0     7855 2020-02-02 00:00:00.000000 jupyterlab_language_pack_zh_cn-4.1.post2/jupyterlab_language_pack_zh_CN/locale/zh_CN/LC_MESSAGES/jupytext.po
--rw-r--r--   0        0        0     6843 2020-02-02 00:00:00.000000 jupyterlab_language_pack_zh_cn-4.1.post2/jupyterlab_language_pack_zh_CN/locale/zh_CN/LC_MESSAGES/nbdime.po
--rw-r--r--   0        0        0    13357 2020-02-02 00:00:00.000000 jupyterlab_language_pack_zh_cn-4.1.post2/jupyterlab_language_pack_zh_CN/locale/zh_CN/LC_MESSAGES/notebook.po
--rw-r--r--   0        0        0     5481 2020-02-02 00:00:00.000000 jupyterlab_language_pack_zh_cn-4.1.post2/jupyterlab_language_pack_zh_CN/locale/zh_CN/LC_MESSAGES/retrolab.po
--rw-r--r--   0        0        0     6655 2020-02-02 00:00:00.000000 jupyterlab_language_pack_zh_cn-4.1.post2/jupyterlab_language_pack_zh_CN/locale/zh_CN/LC_MESSAGES/spellchecker.po
--rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 jupyterlab_language_pack_zh_cn-4.1.post2/.gitignore
--rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 jupyterlab_language_pack_zh_cn-4.1.post2/LICENSE.txt
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 jupyterlab_language_pack_zh_cn-4.1.post2/README.md
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 jupyterlab_language_pack_zh_cn-4.1.post2/pyproject.toml
--rw-r--r--   0        0        0     2764 2020-02-02 00:00:00.000000 jupyterlab_language_pack_zh_cn-4.1.post2/PKG-INFO
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 jupyterlab_language_pack_zh_cn-4.2.post0/.copier-answers.yml
+-rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 jupyterlab_language_pack_zh_cn-4.2.post0/CONTRIBUTORS.md
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 jupyterlab_language_pack_zh_cn-4.2.post0/jupyterlab_language_pack_zh_CN/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_language_pack_zh_cn-4.2.post0/jupyterlab_language_pack_zh_CN/locale/zh_CN/LC_MESSAGES/.gitkeep
+-rw-r--r--   0        0        0     5146 2020-02-02 00:00:00.000000 jupyterlab_language_pack_zh_cn-4.2.post0/jupyterlab_language_pack_zh_CN/locale/zh_CN/LC_MESSAGES/dask_labextension.po
+-rw-r--r--   0        0        0     3136 2020-02-02 00:00:00.000000 jupyterlab_language_pack_zh_cn-4.2.post0/jupyterlab_language_pack_zh_CN/locale/zh_CN/LC_MESSAGES/jupyter_archive.po
+-rw-r--r--   0        0        0     5313 2020-02-02 00:00:00.000000 jupyterlab_language_pack_zh_cn-4.2.post0/jupyterlab_language_pack_zh_CN/locale/zh_CN/LC_MESSAGES/jupyter_collaboration.po
+-rw-r--r--   0        0        0    10223 2020-02-02 00:00:00.000000 jupyterlab_language_pack_zh_cn-4.2.post0/jupyterlab_language_pack_zh_CN/locale/zh_CN/LC_MESSAGES/jupyter_resource_usage.po
+-rw-r--r--   0        0        0   319353 2020-02-02 00:00:00.000000 jupyterlab_language_pack_zh_cn-4.2.post0/jupyterlab_language_pack_zh_CN/locale/zh_CN/LC_MESSAGES/jupyterlab.po
+-rw-r--r--   0        0        0   149651 2020-02-02 00:00:00.000000 jupyterlab_language_pack_zh_cn-4.2.post0/jupyterlab_language_pack_zh_CN/locale/zh_CN/LC_MESSAGES/jupyterlab_git.po
+-rw-r--r--   0        0        0    64794 2020-02-02 00:00:00.000000 jupyterlab_language_pack_zh_cn-4.2.post0/jupyterlab_language_pack_zh_CN/locale/zh_CN/LC_MESSAGES/jupyterlab_lsp.po
+-rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 jupyterlab_language_pack_zh_cn-4.2.post0/jupyterlab_language_pack_zh_CN/locale/zh_CN/LC_MESSAGES/jupyterlab_recents.po
+-rw-r--r--   0        0        0     5825 2020-02-02 00:00:00.000000 jupyterlab_language_pack_zh_cn-4.2.post0/jupyterlab_language_pack_zh_CN/locale/zh_CN/LC_MESSAGES/jupyterlab_search_replace.po
+-rw-r--r--   0        0        0     3652 2020-02-02 00:00:00.000000 jupyterlab_language_pack_zh_cn-4.2.post0/jupyterlab_language_pack_zh_CN/locale/zh_CN/LC_MESSAGES/jupyterlab_spreadsheet_editor.po
+-rw-r--r--   0        0        0    17038 2020-02-02 00:00:00.000000 jupyterlab_language_pack_zh_cn-4.2.post0/jupyterlab_language_pack_zh_CN/locale/zh_CN/LC_MESSAGES/jupyterlab_tour.po
+-rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 jupyterlab_language_pack_zh_cn-4.2.post0/jupyterlab_language_pack_zh_CN/locale/zh_CN/LC_MESSAGES/jupyterlab_widgets.po
+-rw-r--r--   0        0        0     7855 2020-02-02 00:00:00.000000 jupyterlab_language_pack_zh_cn-4.2.post0/jupyterlab_language_pack_zh_CN/locale/zh_CN/LC_MESSAGES/jupytext.po
+-rw-r--r--   0        0        0     6843 2020-02-02 00:00:00.000000 jupyterlab_language_pack_zh_cn-4.2.post0/jupyterlab_language_pack_zh_CN/locale/zh_CN/LC_MESSAGES/nbdime.po
+-rw-r--r--   0        0        0    13357 2020-02-02 00:00:00.000000 jupyterlab_language_pack_zh_cn-4.2.post0/jupyterlab_language_pack_zh_CN/locale/zh_CN/LC_MESSAGES/notebook.po
+-rw-r--r--   0        0        0     5481 2020-02-02 00:00:00.000000 jupyterlab_language_pack_zh_cn-4.2.post0/jupyterlab_language_pack_zh_CN/locale/zh_CN/LC_MESSAGES/retrolab.po
+-rw-r--r--   0        0        0     6655 2020-02-02 00:00:00.000000 jupyterlab_language_pack_zh_cn-4.2.post0/jupyterlab_language_pack_zh_CN/locale/zh_CN/LC_MESSAGES/spellchecker.po
+-rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 jupyterlab_language_pack_zh_cn-4.2.post0/.gitignore
+-rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 jupyterlab_language_pack_zh_cn-4.2.post0/LICENSE.txt
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 jupyterlab_language_pack_zh_cn-4.2.post0/README.md
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 jupyterlab_language_pack_zh_cn-4.2.post0/pyproject.toml
+-rw-r--r--   0        0        0     2764 2020-02-02 00:00:00.000000 jupyterlab_language_pack_zh_cn-4.2.post0/PKG-INFO
```

### Comparing `jupyterlab_language_pack_zh_cn-4.1.post2/CONTRIBUTORS.md` & `jupyterlab_language_pack_zh_cn-4.2.post0/CONTRIBUTORS.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_zh_cn-4.1.post2/jupyterlab_language_pack_zh_CN/locale/zh_CN/LC_MESSAGES/dask_labextension.po` & `jupyterlab_language_pack_zh_cn-4.2.post0/jupyterlab_language_pack_zh_CN/locale/zh_CN/LC_MESSAGES/dask_labextension.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_zh_cn-4.1.post2/jupyterlab_language_pack_zh_CN/locale/zh_CN/LC_MESSAGES/jupyter_archive.po` & `jupyterlab_language_pack_zh_cn-4.2.post0/jupyterlab_language_pack_zh_CN/locale/zh_CN/LC_MESSAGES/jupyter_archive.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_zh_cn-4.1.post2/jupyterlab_language_pack_zh_CN/locale/zh_CN/LC_MESSAGES/jupyter_collaboration.po` & `jupyterlab_language_pack_zh_cn-4.2.post0/jupyterlab_language_pack_zh_CN/locale/zh_CN/LC_MESSAGES/jupyter_collaboration.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_zh_cn-4.1.post2/jupyterlab_language_pack_zh_CN/locale/zh_CN/LC_MESSAGES/jupyter_resource_usage.po` & `jupyterlab_language_pack_zh_cn-4.2.post0/jupyterlab_language_pack_zh_CN/locale/zh_CN/LC_MESSAGES/jupyter_resource_usage.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_zh_cn-4.1.post2/jupyterlab_language_pack_zh_CN/locale/zh_CN/LC_MESSAGES/jupyterlab.po` & `jupyterlab_language_pack_zh_cn-4.2.post0/jupyterlab_language_pack_zh_CN/locale/zh_CN/LC_MESSAGES/jupyterlab.po`

 * *Files 13% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 "X-Crowdin-Project: jupyterlab\n"
 "X-Crowdin-Project-ID: 409874\n"
 "X-Crowdin-Language: zh-CN\n"
 "X-Crowdin-File: /main/jupyterlab/locale/jupyterlab.pot\n"
 "X-Crowdin-File-ID: 191\n"
 "Language-Team: Chinese Simplified\n"
 "Language: zh_CN\n"
-"PO-Revision-Date: 2024-02-08 06:44\n"
+"PO-Revision-Date: 2024-05-10 05:59\n"
 
 #: /examples/federated/md_package/schema/plugin.json:/description /packages/markdownviewer-extension/schema/plugin.json:/description
 msgctxt "schema"
 msgid "Markdown viewer settings."
 msgstr "Markdown 查看器设置。"
 
 #: /examples/federated/md_package/schema/plugin.json:/jupyter.lab.setting-icon-label /packages/markdownviewer-extension/schema/plugin.json:/jupyter.lab.setting-icon-label
@@ -1037,14 +1037,24 @@
 msgstr "在磁盘上和在客户端上最后修改时间戳的最大可接受差异区间，单位毫秒"
 
 #: /packages/docmanager-extension/schema/plugin.json:/properties/lastModifiedCheckMargin/title
 msgctxt "settings"
 msgid "Margin for last modified timestamp check"
 msgstr "最后修改时间检查的范围区间"
 
+#: /packages/docmanager-extension/schema/plugin.json:/properties/maxNumberRecents/description
+msgctxt "settings"
+msgid "Number of recently opened/closed files and directories to remember."
+msgstr "要记住的最近打开/关闭的文件和目录的数量。"
+
+#: /packages/docmanager-extension/schema/plugin.json:/properties/maxNumberRecents/title
+msgctxt "settings"
+msgid "Recent Items Number"
+msgstr "最近文档项数"
+
 #: /packages/docmanager-extension/schema/plugin.json:/properties/renameUntitledFileOnSave/description
 msgctxt "settings"
 msgid "Whether to prompt to rename untitled file on first manual save."
 msgstr "是否在第一次手动保存时提示重命名无标题文件。"
 
 #: /packages/docmanager-extension/schema/plugin.json:/properties/renameUntitledFileOnSave/title
 msgctxt "settings"
@@ -1139,29 +1149,49 @@
 msgstr "文件浏览器"
 
 #: /packages/filebrowser-extension/schema/browser.json:/properties/filterDirectories/description
 msgctxt "settings"
 msgid "Whether to apply the search on directories"
 msgstr "是否在目录上进行搜索"
 
+#: /packages/filebrowser-extension/schema/browser.json:/properties/filterDirectories/description
+msgctxt "settings"
+msgid "Whether to apply the search on folders"
+msgstr "是否在文件夹中应用搜索"
+
 #: /packages/filebrowser-extension/schema/browser.json:/properties/filterDirectories/title
 msgctxt "settings"
 msgid "Filter directories"
 msgstr "筛选目录"
 
+#: /packages/filebrowser-extension/schema/browser.json:/properties/filterDirectories/title
+msgctxt "settings"
+msgid "Filter folders"
+msgstr "筛选文件夹"
+
 #: /packages/filebrowser-extension/schema/browser.json:/properties/navigateToCurrentDirectory/description
 msgctxt "settings"
 msgid "Whether to automatically navigate to a document's current directory"
 msgstr "是否自动导航到文档的当前目录"
 
+#: /packages/filebrowser-extension/schema/browser.json:/properties/navigateToCurrentDirectory/description
+msgctxt "settings"
+msgid "Whether to automatically navigate to a document's current folder"
+msgstr "是否自动导航到文档的当前文件夹"
+
 #: /packages/filebrowser-extension/schema/browser.json:/properties/navigateToCurrentDirectory/title
 msgctxt "settings"
 msgid "Navigate to current directory"
 msgstr "导航到当前目录"
 
+#: /packages/filebrowser-extension/schema/browser.json:/properties/navigateToCurrentDirectory/title
+msgctxt "settings"
+msgid "Navigate to current folder"
+msgstr "导航到当前文件夹"
+
 #: /packages/filebrowser-extension/schema/browser.json:/properties/showFileCheckboxes/description
 msgctxt "settings"
 msgid "Whether to show checkboxes next to files and folders"
 msgstr "是否显示文件和文件夹旁边的复选框"
 
 #: /packages/filebrowser-extension/schema/browser.json:/properties/showFileCheckboxes/title
 msgctxt "settings"
@@ -1774,14 +1804,19 @@
 #: /packages/notebook-extension/schema/export.json:/description
 msgctxt "schema"
 msgid "Notebook Export settings."
 msgstr "笔记本导出设置。"
 
 #: /packages/notebook-extension/schema/export.json:/jupyter.lab.menus/main[0]/items[1]/submenu/label
 msgctxt "menu"
+msgid "Save and Export Notebook As"
+msgstr "保存并导出笔记本为"
+
+#: /packages/notebook-extension/schema/export.json:/jupyter.lab.menus/main[0]/items[1]/submenu/label
+msgctxt "menu"
 msgid "Save and Export Notebook As…"
 msgstr "保存并导出笔记本为…"
 
 #: /packages/notebook-extension/schema/export.json:/title
 msgctxt "schema"
 msgid "Notebook Export"
 msgstr "笔记本导出"
@@ -2447,51 +2482,74 @@
 msgstr "本地化字符串前缀"
 
 #: /packages/translation-extension/schema/plugin.json:/title
 msgctxt "schema"
 msgid "Language"
 msgstr "语言"
 
-#: packages/application-extension/src/index.tsx:1143 packages/application-extension/src/index.tsx:1148
+#: /packages/workspaces-extension/schema/menu.json:/description /packages/workspaces-extension/schema/menu.json:/title
+msgctxt "schema"
+msgid "Workspaces Menu"
+msgstr "工作区菜单"
+
+#: /packages/workspaces-extension/schema/menu.json:/jupyter.lab.menus/main[0]/items[0]/submenu/label
+msgctxt "menu"
+msgid "Workspaces"
+msgstr "工作区"
+
+#: /packages/workspaces-extension/schema/sidebar.json:/description /packages/workspaces-extension/schema/sidebar.json:/title
+msgctxt "schema"
+msgid "Workspaces Sidebar"
+msgstr "工作区侧边栏"
+
+#: packages/application-extension/src/index.tsx:1005 packages/application-extension/src/index.tsx:990
+msgid "The path: %1 was not found. JupyterLab redirected to: %2"
+msgstr "路径：%1 未找到。JupyterLab 将会重定向到：%2"
+
+#: packages/application-extension/src/index.tsx:1014 packages/application-extension/src/index.tsx:999
+msgid "Path Not Found"
+msgstr "未找到路径"
+
+#: packages/application-extension/src/index.tsx:1143 packages/application-extension/src/index.tsx:1148 packages/application-extension/src/index.tsx:1158 packages/application-extension/src/index.tsx:1163
 msgid "Property Inspector"
 msgstr "属性检查器"
 
-#: packages/application-extension/src/index.tsx:1236
+#: packages/application-extension/src/index.tsx:1236 packages/application-extension/src/index.tsx:1251
 msgid "Simple Interface (%1)"
 msgstr "简易界面（%1）"
 
-#: packages/application-extension/src/index.tsx:1238 packages/application-extension/src/index.tsx:450
+#: packages/application-extension/src/index.tsx:1238 packages/application-extension/src/index.tsx:1253 packages/application-extension/src/index.tsx:450 packages/application-extension/src/index.tsx:471
 msgid "Simple Interface"
 msgstr "简易界面"
 
-#: packages/application-extension/src/index.tsx:1246
+#: packages/application-extension/src/index.tsx:1246 packages/application-extension/src/index.tsx:1261
 msgid "Simple"
 msgstr "简易界面"
 
-#: packages/application-extension/src/index.tsx:1286 packages/application-extension/src/index.tsx:856 packages/apputils/src/toolbar/factory.ts:33 packages/extensionmanager/src/model.ts:529 packages/extensionmanager/src/model.ts:551 packages/mainmenu-extension/src/index.ts:770
+#: packages/application-extension/src/index.tsx:1286 packages/application-extension/src/index.tsx:1301 packages/application-extension/src/index.tsx:856 packages/application-extension/src/index.tsx:871 packages/apputils/src/toolbar/factory.ts:33 packages/extensionmanager/src/model.ts:529 packages/extensionmanager/src/model.ts:551 packages/mainmenu-extension/src/index.ts:767 packages/mainmenu-extension/src/index.ts:770
 msgid "Information"
 msgstr "信息"
 
-#: packages/application-extension/src/index.tsx:1287
+#: packages/application-extension/src/index.tsx:1287 packages/application-extension/src/index.tsx:1302
 msgid "Context menu customization has changed. You will need to reload JupyterLab to see the changes."
 msgstr "上下文菜单自定义已更改。您需要重新加载 JupyterLab 来查看改动。"
 
-#: packages/application-extension/src/index.tsx:1292 packages/application-extension/src/index.tsx:862 packages/apputils/src/toolbar/factory.ts:39 packages/docmanager-extension/src/index.tsx:750 packages/mainmenu-extension/src/index.ts:776
+#: packages/application-extension/src/index.tsx:1292 packages/application-extension/src/index.tsx:1307 packages/application-extension/src/index.tsx:862 packages/application-extension/src/index.tsx:877 packages/apputils/src/toolbar/factory.ts:39 packages/docmanager-extension/src/index.tsx:750 packages/docmanager-extension/src/index.tsx:762 packages/mainmenu-extension/src/index.ts:773 packages/mainmenu-extension/src/index.ts:776
 msgid "Reload"
 msgstr "重新加载"
 
-#: packages/application-extension/src/index.tsx:135 packages/apputils-extension/src/index.ts:319 packages/documentsearch-extension/src/index.ts:463 packages/logconsole-extension/src/index.tsx:246 packages/mainmenu-extension/src/index.ts:236 packages/mainmenu-extension/src/index.ts:240 packages/mainmenu-extension/src/index.ts:250 packages/statusbar-extension/src/index.ts:48
+#: packages/application-extension/src/index.tsx:135 packages/apputils-extension/src/index.ts:319 packages/apputils-extension/src/index.ts:323 packages/documentsearch-extension/src/index.ts:463 packages/documentsearch-extension/src/index.ts:469 packages/logconsole-extension/src/index.tsx:246 packages/mainmenu-extension/src/index.ts:236 packages/mainmenu-extension/src/index.ts:237 packages/mainmenu-extension/src/index.ts:240 packages/mainmenu-extension/src/index.ts:241 packages/mainmenu-extension/src/index.ts:250 packages/mainmenu-extension/src/index.ts:251 packages/statusbar-extension/src/index.ts:48
 msgid "Main Area"
 msgstr "主工作区"
 
 #: packages/application-extension/src/index.tsx:139
 msgid "Shift+Right Click for Browser Menu"
 msgstr "使用 Shift+右键点击调出浏览器菜单"
 
-#: packages/application-extension/src/index.tsx:1468
+#: packages/application-extension/src/index.tsx:1468 packages/application-extension/src/index.tsx:1483
 msgid "Switch Sidebar Side"
 msgstr "侧边栏位置切换"
 
 #: packages/application-extension/src/index.tsx:239
 msgid "Close Tab"
 msgstr "关闭标签页"
 
@@ -2499,168 +2557,172 @@
 msgid "Close All Other Tabs"
 msgstr "关闭所有其它标签页"
 
 #: packages/application-extension/src/index.tsx:273
 msgid "Close Tabs to Right"
 msgstr "关闭右侧标签页"
 
-#: packages/application-extension/src/index.tsx:288
+#: packages/application-extension/src/index.tsx:288 packages/application-extension/src/index.tsx:296
 msgid "Activate Next Tab"
 msgstr "激活下一标签页"
 
-#: packages/application-extension/src/index.tsx:295
+#: packages/application-extension/src/index.tsx:295 packages/application-extension/src/index.tsx:303
 msgid "Activate Previous Tab"
 msgstr "激活上一标签页"
 
-#: packages/application-extension/src/index.tsx:302
+#: packages/application-extension/src/index.tsx:302 packages/application-extension/src/index.tsx:310
 msgid "Activate Next Tab Bar"
 msgstr "激活下一标签栏"
 
-#: packages/application-extension/src/index.tsx:309
+#: packages/application-extension/src/index.tsx:309 packages/application-extension/src/index.tsx:317
 msgid "Activate Previous Tab Bar"
 msgstr "激活上一标签栏"
 
-#: packages/application-extension/src/index.tsx:316
+#: packages/application-extension/src/index.tsx:316 packages/application-extension/src/index.tsx:324
 msgid "Close All Tabs"
 msgstr "关闭所有标签页"
 
-#: packages/application-extension/src/index.tsx:323
+#: packages/application-extension/src/index.tsx:323 packages/application-extension/src/index.tsx:331
 msgid "Show Header"
 msgstr "显示页头"
 
-#: packages/application-extension/src/index.tsx:334
+#: packages/application-extension/src/index.tsx:334 packages/application-extension/src/index.tsx:342
 msgid "Show Left Sidebar"
 msgstr "显示左侧边栏"
 
-#: packages/application-extension/src/index.tsx:350
+#: packages/application-extension/src/index.tsx:350 packages/application-extension/src/index.tsx:358
 msgid "Show Right Sidebar"
 msgstr "显示右侧边栏"
 
-#: packages/application-extension/src/index.tsx:366
+#: packages/application-extension/src/index.tsx:366 packages/application-extension/src/index.tsx:378
 msgid "Toggle Sidebar Element"
 msgstr "切换侧边栏元素"
 
-#: packages/application-extension/src/index.tsx:399
+#: packages/application-extension/src/index.tsx:380
+msgid "Toggle Element %1 in Right Sidebar"
+msgstr "在右侧边栏中切换元素 %1"
+
+#: packages/application-extension/src/index.tsx:384
+msgid "Toggle Element %1 in Left Sidebar"
+msgstr "在左侧边栏中切换元素 %1"
+
+#: packages/application-extension/src/index.tsx:399 packages/application-extension/src/index.tsx:420
 msgid "Show Right Activity Bar"
 msgstr "显示右侧活动栏"
 
-#: packages/application-extension/src/index.tsx:400
+#: packages/application-extension/src/index.tsx:400 packages/application-extension/src/index.tsx:421
 msgid "Show Left Activity Bar"
 msgstr "显示左侧活动栏"
 
-#: packages/application-extension/src/index.tsx:419
+#: packages/application-extension/src/index.tsx:419 packages/application-extension/src/index.tsx:440
 msgid "Presentation Mode"
 msgstr "演示模式"
 
-#: packages/application-extension/src/index.tsx:430
+#: packages/application-extension/src/index.tsx:430 packages/application-extension/src/index.tsx:451
 msgid "Set %1 mode."
 msgstr "设定 %1 模式。"
 
-#: packages/application-extension/src/index.tsx:431
+#: packages/application-extension/src/index.tsx:431 packages/application-extension/src/index.tsx:452
 msgid "Set the layout `mode`."
 msgstr "设置布局`模式'。"
 
-#: packages/application-extension/src/index.tsx:432
+#: packages/application-extension/src/index.tsx:432 packages/application-extension/src/index.tsx:453
 msgid "The layout `mode` can be \"single-document\" or \"multiple-document\"."
 msgstr "布局 `模式` 可以是“单文档”或“多文档”。"
 
-#: packages/application-extension/src/index.tsx:462
+#: packages/application-extension/src/index.tsx:462 packages/application-extension/src/index.tsx:483
 msgid "Reset Default Layout"
 msgstr "重置为默认布局"
 
-#: packages/application-extension/src/index.tsx:592
+#: packages/application-extension/src/index.tsx:592 packages/application-extension/src/index.tsx:613
 msgid "Error Registering Plugins"
 msgstr "注册插件时出错"
 
-#: packages/application-extension/src/index.tsx:642
+#: packages/application-extension/src/index.tsx:642 packages/application-extension/src/index.tsx:657
 msgid "Build Complete"
 msgstr "构建完成"
 
-#: packages/application-extension/src/index.tsx:645
+#: packages/application-extension/src/index.tsx:645 packages/application-extension/src/index.tsx:660
 msgid "Build successfully completed, reload page?"
 msgstr "构建已成功完成，重新加载页面？"
 
-#: packages/application-extension/src/index.tsx:647
+#: packages/application-extension/src/index.tsx:647 packages/application-extension/src/index.tsx:662
 msgid "You will lose any unsaved changes."
 msgstr "您将丢失任何未保存的更改。"
 
-#: packages/application-extension/src/index.tsx:652
+#: packages/application-extension/src/index.tsx:652 packages/application-extension/src/index.tsx:667
 msgid "Reload Without Saving"
 msgstr "重新加载且不保存当前更改"
 
-#: packages/application-extension/src/index.tsx:655
+#: packages/application-extension/src/index.tsx:655 packages/application-extension/src/index.tsx:670
 msgid "Save and Reload"
 msgstr "保存并重新加载"
 
-#: packages/application-extension/src/index.tsx:668
+#: packages/application-extension/src/index.tsx:668 packages/application-extension/src/index.tsx:683
 msgid "Save Failed"
 msgstr "保存失败"
 
-#: packages/application-extension/src/index.tsx:677
+#: packages/application-extension/src/index.tsx:677 packages/application-extension/src/index.tsx:692
 msgid "Build Failed"
 msgstr "编译失败"
 
-#: packages/application-extension/src/index.tsx:695
+#: packages/application-extension/src/index.tsx:695 packages/application-extension/src/index.tsx:710
 msgid "JupyterLab build is suggested:"
 msgstr "建议重新构建 JupyterLab："
 
-#: packages/application-extension/src/index.tsx:702
+#: packages/application-extension/src/index.tsx:702 packages/application-extension/src/index.tsx:717
 msgid "Build Recommended"
 msgstr "建议重新编译"
 
-#: packages/application-extension/src/index.tsx:706
+#: packages/application-extension/src/index.tsx:706 packages/application-extension/src/index.tsx:721
 msgid "Build"
 msgstr "编译"
 
-#: packages/application-extension/src/index.tsx:772
+#: packages/application-extension/src/index.tsx:772 packages/application-extension/src/index.tsx:787
 msgid "Are you sure you want to exit JupyterLab?\n\n"
 "Any unsaved changes will be lost."
 msgstr "您确定要退出登录吗？所有未保存的操作都会丢失。"
 
-#: packages/application-extension/src/index.tsx:857
+#: packages/application-extension/src/index.tsx:857 packages/application-extension/src/index.tsx:872
 msgid "User layout customization has changed. You may need to reload JupyterLab to see the changes."
 msgstr "用户布局自定义已更改。您可能需要重新加载JupyterLab才能看到更改。"
 
-#: packages/application-extension/src/index.tsx:990
-msgid "The path: %1 was not found. JupyterLab redirected to: %2"
-msgstr "路径：%1 未找到。JupyterLab 将会重定向到：%2"
-
-#: packages/application-extension/src/index.tsx:999
-msgid "Path Not Found"
-msgstr "未找到路径"
-
 #: packages/application/src/connectionlost.ts:19
 msgid "Server Connection Error"
 msgstr "服务器连接错误"
 
 #: packages/application/src/connectionlost.ts:20
 msgid "A connection to the Jupyter server could not be established.\n"
 "JupyterLab will continue trying to reconnect.\n"
 "Check your network connection or Jupyter server configuration.\n"
 msgstr "无法连接到 Jupyter 服务器。\n"
 "JupyterLab 将继续尝试重新连接。\n"
 "请检查您的网络连接或 Jupyter 服务器配置。\n"
 
-#: packages/application/src/shell.ts:734
+#: packages/application/src/shell.ts:734 packages/application/src/shell.ts:741
 msgid "main menu"
 msgstr "主菜单"
 
-#: packages/application/src/shell.ts:738 packages/application/src/shell.ts:742
+#: packages/application/src/shell.ts:738 packages/application/src/shell.ts:742 packages/application/src/shell.ts:745 packages/application/src/shell.ts:749
 msgid "main sidebar"
 msgstr "主侧边栏"
 
-#: packages/application/src/shell.ts:746 packages/application/src/shell.ts:750
+#: packages/application/src/shell.ts:746 packages/application/src/shell.ts:750 packages/application/src/shell.ts:753 packages/application/src/shell.ts:757
 msgid "alternate sidebar"
 msgstr "备选侧边栏"
 
-#: packages/application/src/utils.ts:148
+#: packages/application/src/utils.ts:148 packages/application/src/utils.ts:253
 msgid "%1 and %2"
 msgstr "%1 和 %2"
 
 #: packages/apputils-extension/src/announcements.ts:102
+msgid "Would you like to get notified about official Jupyter news?"
+msgstr "您是否希望接收有关官方 Jupyter 新闻的通知？"
+
+#: packages/apputils-extension/src/announcements.ts:102
 msgid "Would you like to receive official Jupyter news?\n"
 "Please read the privacy policy."
 msgstr "您想要接收官方的Jupyter新闻吗？\n"
 "请阅读隐私政策。"
 
 #: packages/apputils-extension/src/announcements.ts:110
 msgid "Open privacy policy"
@@ -2711,47 +2773,51 @@
 msgid "Clear Workspace"
 msgstr "清除工作区"
 
 #: packages/apputils-extension/src/index.ts:290
 msgid "Print…"
 msgstr "打印…"
 
-#: packages/apputils-extension/src/index.ts:321
+#: packages/apputils-extension/src/index.ts:321 packages/apputils-extension/src/index.ts:325
 msgid "Show Header Above Content"
 msgstr "在内容上方显示页头"
 
-#: packages/apputils-extension/src/index.ts:429
+#: packages/apputils-extension/src/index.ts:429 packages/apputils-extension/src/index.ts:438
 msgid "Load state for the current workspace."
 msgstr "加载当前工作区的状态。"
 
-#: packages/apputils-extension/src/index.ts:493
+#: packages/apputils-extension/src/index.ts:493 packages/apputils-extension/src/index.ts:502
 msgid "Reset Application State"
 msgstr "重置应用程序状态"
 
-#: packages/apputils-extension/src/index.ts:504
+#: packages/apputils-extension/src/index.ts:504 packages/apputils-extension/src/index.ts:513
 msgid "Reset state when loading for the workspace."
 msgstr "重置工作区加载时的状态。"
 
-#: packages/apputils-extension/src/index.ts:595
+#: packages/apputils-extension/src/index.ts:595 packages/apputils-extension/src/index.ts:604
 msgid "Run First Enabled Command"
 msgstr "运行第一个启用的命令"
 
-#: packages/apputils-extension/src/index.ts:613
+#: packages/apputils-extension/src/index.ts:613 packages/apputils-extension/src/index.ts:622
 msgid "Run All Enabled Commands Passed as Args"
 msgstr "运行所有从参数传递过来的已启用的命令"
 
 #: packages/apputils-extension/src/index.ts:644
 msgid "Show Keyboard Shortcuts"
 msgstr "显示键盘快捷键"
 
-#: packages/apputils-extension/src/index.ts:645
+#: packages/apputils-extension/src/index.ts:645 packages/apputils-extension/src/index.ts:654
 msgid "Show relevant keyboard shortcuts for the current active widget"
 msgstr "显示当前活动小部件的相关键盘快捷键"
 
-#: packages/apputils-extension/src/index.ts:662 packages/help-extension/src/index.tsx:183 packages/help-extension/src/index.tsx:296 packages/help-extension/src/index.tsx:500 packages/help-extension/src/index.tsx:90
+#: packages/apputils-extension/src/index.ts:653
+msgid "Show Keyboard Shortcuts…"
+msgstr "显示键盘快捷键..."
+
+#: packages/apputils-extension/src/index.ts:662 packages/apputils-extension/src/index.ts:671 packages/help-extension/src/index.tsx:183 packages/help-extension/src/index.tsx:296 packages/help-extension/src/index.tsx:500 packages/help-extension/src/index.tsx:90
 msgid "Help"
 msgstr "帮助"
 
 #: packages/apputils-extension/src/notificationplugin.tsx:167 packages/apputils-extension/src/notificationplugin.tsx:354
 msgid "%1 notification"
 msgid_plural "%1 notifications"
 msgstr[0] "%1 条通知"
@@ -2824,15 +2890,15 @@
 msgid "Command Palette"
 msgstr "命令面板"
 
 #: packages/apputils-extension/src/shortcuts.tsx:193
 msgid "Keyboard Shortcuts"
 msgstr "键盘快捷键"
 
-#: packages/apputils-extension/src/shortcuts.tsx:197 packages/docmanager/src/widgetmanager.ts:397 packages/filebrowser/src/listing.ts:1415 packages/running-extension/src/opentabs.ts:86
+#: packages/apputils-extension/src/shortcuts.tsx:197 packages/docmanager/src/widgetmanager.ts:397 packages/docmanager/src/widgetmanager.ts:468 packages/filebrowser/src/listing.ts:1415 packages/filebrowser/src/listing.ts:1436 packages/filebrowser/src/listing.ts:1488 packages/running-extension/src/opentabs.ts:86
 msgid "Close"
 msgstr "关闭"
 
 #: packages/apputils-extension/src/themesplugins.ts:118
 msgid "Switch to the provided `theme`."
 msgstr "切换到提供的`主题`。"
 
@@ -2880,15 +2946,15 @@
 msgid "Increase Content Font Size"
 msgstr "增大内容字号"
 
 #: packages/apputils-extension/src/themesplugins.ts:217
 msgid "Increase UI Font Size"
 msgstr "增大界面字号"
 
-#: packages/apputils-extension/src/themesplugins.ts:219 packages/fileeditor-extension/src/commands.ts:281
+#: packages/apputils-extension/src/themesplugins.ts:219 packages/fileeditor-extension/src/commands.ts:281 packages/fileeditor-extension/src/commands.ts:282
 msgid "Increase Font Size"
 msgstr "增大字号"
 
 #: packages/apputils-extension/src/themesplugins.ts:229
 msgid "Decrease Code Font Size"
 msgstr "减小代码字号"
 
@@ -2896,51 +2962,55 @@
 msgid "Decrease Content Font Size"
 msgstr "减少内容字号"
 
 #: packages/apputils-extension/src/themesplugins.ts:233
 msgid "Decrease UI Font Size"
 msgstr "减小界面字号"
 
-#: packages/apputils-extension/src/themesplugins.ts:235 packages/fileeditor-extension/src/commands.ts:285
+#: packages/apputils-extension/src/themesplugins.ts:235 packages/fileeditor-extension/src/commands.ts:285 packages/fileeditor-extension/src/commands.ts:286
 msgid "Decrease Font Size"
 msgstr "减小字号"
 
-#: packages/apputils-extension/src/themesplugins.ts:295 packages/codemirror/src/extension.ts:982
+#: packages/apputils-extension/src/themesplugins.ts:295 packages/codemirror/src/extension.ts:1006 packages/codemirror/src/extension.ts:982
 msgid "Theme"
 msgstr "主题"
 
-#: packages/apputils-extension/src/workspacesplugin.ts:181
+#: packages/apputils-extension/src/workspacesplugin.ts:181 packages/apputils-extension/src/workspacesplugin.ts:95
 msgid "Workspace loader"
 msgstr "工作区加载器"
 
-#: packages/apputils-extension/src/workspacesplugin.ts:271 packages/apputils-extension/src/workspacesplugin.ts:279 packages/docmanager/src/widgetmanager.ts:442 packages/docregistry/src/context.ts:1043
+#: packages/apputils-extension/src/workspacesplugin.ts:271 packages/apputils-extension/src/workspacesplugin.ts:279 packages/docmanager/src/widgetmanager.ts:442 packages/docmanager/src/widgetmanager.ts:513 packages/docregistry/src/context.ts:1041 packages/docregistry/src/context.ts:1043 packages/workspaces-extension/src/commands.ts:587
 msgid "Save"
 msgstr "保存"
 
-#: packages/apputils-extension/src/workspacesplugin.ts:272 packages/apputils-extension/src/workspacesplugin.ts:93
+#: packages/apputils-extension/src/workspacesplugin.ts:272 packages/apputils-extension/src/workspacesplugin.ts:93 packages/workspaces-extension/src/commands.ts:458
 msgid "Save Current Workspace"
 msgstr "保存当前工作区"
 
-#: packages/apputils-extension/src/workspacesplugin.ts:275 packages/apputils-extension/src/workspacesplugin.ts:79
+#: packages/apputils-extension/src/workspacesplugin.ts:275 packages/apputils-extension/src/workspacesplugin.ts:79 packages/workspaces-extension/src/commands.ts:449 packages/workspaces-extension/src/commands.ts:584
 msgid "Save Current Workspace As…"
 msgstr "保存当前工作区为…"
 
 #: packages/apputils-extension/src/workspacesplugin.ts:72
+msgid "JupyterLab Workspace File"
+msgstr "JupyterLab 工作区文件"
+
+#: packages/apputils-extension/src/workspacesplugin.ts:72
 msgid "JupyterLab workspace File"
 msgstr "JupyterLab 工作区文件"
 
-#: packages/apputils/src/dialog.tsx:47 packages/help-extension/src/index.tsx:153 packages/help-extension/src/index.tsx:425 packages/hub-extension/src/index.ts:180 packages/lsp/src/adapters/adapter.ts:497 packages/mainmenu-extension/src/index.ts:548
+#: packages/apputils/src/dialog.tsx:47 packages/help-extension/src/index.tsx:153 packages/help-extension/src/index.tsx:425 packages/hub-extension/src/index.ts:180 packages/lsp/src/adapters/adapter.ts:497 packages/mainmenu-extension/src/index.ts:545 packages/mainmenu-extension/src/index.ts:548
 msgid "Dismiss"
 msgstr "忽略"
 
-#: packages/apputils/src/dialog.tsx:770 packages/apputils/src/dialog.tsx:870 packages/apputils/src/sessioncontext.tsx:1335 packages/debugger-extension/src/index.ts:739 packages/debugger-extension/src/index.ts:840 packages/filebrowser/src/listing.ts:433 packages/filebrowser/src/model.ts:449 packages/notebook/src/searchprovider.ts:527 packages/settingeditor/src/plugineditor.ts:132 packages/shortcuts-extension/src/components/ShortcutItem.tsx:224 packages/translation-extension/src/index.ts:156
+#: packages/apputils/src/dialog.tsx:770 packages/apputils/src/dialog.tsx:793 packages/apputils/src/dialog.tsx:870 packages/apputils/src/dialog.tsx:893 packages/apputils/src/sessioncontext.tsx:1335 packages/debugger-extension/src/index.ts:739 packages/debugger-extension/src/index.ts:840 packages/filebrowser/src/listing.ts:433 packages/filebrowser/src/listing.ts:436 packages/filebrowser/src/model.ts:442 packages/filebrowser/src/model.ts:449 packages/notebook/src/searchprovider.ts:516 packages/notebook/src/searchprovider.ts:519 packages/notebook/src/searchprovider.ts:527 packages/settingeditor/src/plugineditor.ts:132 packages/shortcuts-extension/src/components/ShortcutItem.tsx:224 packages/shortcuts-extension/src/components/ShortcutItem.tsx:341 packages/translation-extension/src/index.ts:156
 msgid "Cancel"
 msgstr "取消"
 
-#: packages/apputils/src/dialog.tsx:770 packages/extensionmanager/src/dialog.tsx:37 packages/extensionmanager/src/model.ts:533 packages/extensionmanager/src/model.ts:556 packages/notebook/src/model.ts:377 packages/notebook/src/panel.ts:228 packages/notebook/src/searchprovider.ts:528 packages/settingeditor/src/plugineditor.ts:133
+#: packages/apputils/src/dialog.tsx:770 packages/apputils/src/dialog.tsx:793 packages/extensionmanager/src/dialog.tsx:37 packages/extensionmanager/src/model.ts:533 packages/extensionmanager/src/model.ts:556 packages/notebook/src/model.ts:377 packages/notebook/src/panel.ts:228 packages/notebook/src/searchprovider.ts:517 packages/notebook/src/searchprovider.ts:520 packages/notebook/src/searchprovider.ts:528 packages/settingeditor/src/plugineditor.ts:133
 msgid "Ok"
 msgstr "确认"
 
 #: packages/apputils/src/kernelstatuses.tsx:221 packages/apputils/src/sessioncontext.tsx:1757 packages/apputils/src/sessioncontext.tsx:631
 msgid "No Kernel"
 msgstr "无内核"
 
@@ -3008,15 +3078,15 @@
 msgid "%1 Terminals, %2 Kernel sessions"
 msgstr "%1 个终端，%2 个内核会话"
 
 #: packages/apputils/src/sessioncontext.tsx:1051
 msgid "Error Starting Kernel"
 msgstr "启动内核时出错"
 
-#: packages/apputils/src/sessioncontext.tsx:1344 packages/filebrowser/src/opendialog.ts:95
+#: packages/apputils/src/sessioncontext.tsx:1344 packages/filebrowser/src/opendialog.ts:106 packages/filebrowser/src/opendialog.ts:95
 msgid "Select"
 msgstr "选择"
 
 #: packages/apputils/src/sessioncontext.tsx:1345 packages/apputils/src/sessioncontext.tsx:1353
 msgid "Select Kernel"
 msgstr "选择内核"
 
@@ -3108,44 +3178,44 @@
 msgid "Switch kernel"
 msgstr "切换内核"
 
 #: packages/apputils/src/toolbar/widget.tsx:210
 msgid "Kernel %1"
 msgstr "内核 %1"
 
-#: packages/apputils/src/toolbar/widget.tsx:56 packages/mainmenu-extension/src/index.ts:469 packages/notebook-extension/src/index.ts:2529
+#: packages/apputils/src/toolbar/widget.tsx:56 packages/mainmenu-extension/src/index.ts:467 packages/mainmenu-extension/src/index.ts:469 packages/notebook-extension/src/index.ts:2529 packages/notebook-extension/src/index.ts:2536 packages/notebook-extension/src/index.ts:2547
 msgid "Interrupt the kernel"
 msgstr "中断内核"
 
-#: packages/apputils/src/toolbar/widget.tsx:80 packages/mainmenu-extension/src/index.ts:494 packages/notebook-extension/src/index.ts:2377
+#: packages/apputils/src/toolbar/widget.tsx:80 packages/mainmenu-extension/src/index.ts:492 packages/mainmenu-extension/src/index.ts:494 packages/notebook-extension/src/index.ts:2377 packages/notebook-extension/src/index.ts:2384 packages/notebook-extension/src/index.ts:2395
 msgid "Restart the kernel"
 msgstr "重启内核"
 
 #: packages/cells/src/placeholder.ts:85
 msgid "Click to expand"
 msgstr "点击展开"
 
-#: packages/cells/src/widget.ts:1010 packages/cells/src/widget.ts:1099 packages/cells/src/widget.ts:1506
+#: packages/cells/src/widget.ts:1010 packages/cells/src/widget.ts:1012 packages/cells/src/widget.ts:1075 packages/cells/src/widget.ts:1099 packages/cells/src/widget.ts:1101 packages/cells/src/widget.ts:1225 packages/cells/src/widget.ts:1506 packages/cells/src/widget.ts:1508 packages/cells/src/widget.ts:1509 packages/cells/src/widget.ts:1646
 msgid "Code Cell Content"
 msgstr "代码单元格内容"
 
-#: packages/cells/src/widget.ts:1011 packages/cells/src/widget.ts:1100 packages/cells/src/widget.ts:1507
+#: packages/cells/src/widget.ts:1011 packages/cells/src/widget.ts:1013 packages/cells/src/widget.ts:1076 packages/cells/src/widget.ts:1100 packages/cells/src/widget.ts:1102 packages/cells/src/widget.ts:1226 packages/cells/src/widget.ts:1507 packages/cells/src/widget.ts:1509 packages/cells/src/widget.ts:1510 packages/cells/src/widget.ts:1647
 msgid "Code Cell Content with Output"
 msgstr "代码单元格内容及其输出"
 
-#: packages/cells/src/widget.ts:1931
+#: packages/cells/src/widget.ts:1931 packages/cells/src/widget.ts:1933 packages/cells/src/widget.ts:1935 packages/cells/src/widget.ts:1936 packages/cells/src/widget.ts:2076
 msgid "Markdown Cell Content"
 msgstr "Markdown 单元格内容"
 
-#: packages/cells/src/widget.ts:2174
+#: packages/cells/src/widget.ts:2174 packages/cells/src/widget.ts:2176 packages/cells/src/widget.ts:2178 packages/cells/src/widget.ts:2179 packages/cells/src/widget.ts:2319
 msgid "%1 cell hidden"
 msgid_plural "%1 cells hidden"
 msgstr[0] "已隐藏第 %1 个单元格"
 
-#: packages/cells/src/widget.ts:2397
+#: packages/cells/src/widget.ts:2397 packages/cells/src/widget.ts:2399 packages/cells/src/widget.ts:2401 packages/cells/src/widget.ts:2402 packages/cells/src/widget.ts:2542
 msgid "Raw Cell Content"
 msgstr "原始单元格内容"
 
 #: packages/celltags-extension/src/celltag.tsx:211
 msgid "Add Tag"
 msgstr "添加标签"
 
@@ -3169,775 +3239,795 @@
 msgid "Ln %1, Col %2"
 msgstr "行 %1，列 %2"
 
 #: packages/codeeditor/src/lineCol.tsx:253
 msgid "Go to line number…"
 msgstr "转到行号…"
 
-#: packages/codemirror/src/extension.ts:1000
+#: packages/codemirror-extension/src/commands.ts:107
+msgid "Select Next Occurrence"
+msgstr "选择下一个出现的位置"
+
+#: packages/codemirror-extension/src/commands.ts:68
+msgid "Delete the current line"
+msgstr "删除当前行"
+
+#: packages/codemirror-extension/src/commands.ts:80
+msgid "Toggle Block Comment"
+msgstr "切换块注释"
+
+#: packages/codemirror-extension/src/commands.ts:81
+msgid "Toggles block commends in languages which support it (e.g. C, JavaScript)"
+msgstr "在支持块注释的语言（例如 C、JavaScript）中切换块注释"
+
+#: packages/codemirror-extension/src/commands.ts:95
+msgid "Toggle Comment"
+msgstr "切换注释"
+
+#: packages/codemirror/src/extension.ts:1000 packages/codemirror/src/extension.ts:1024
 msgid "Folded lines"
 msgstr "折叠的行"
 
-#: packages/codemirror/src/extension.ts:1001
+#: packages/codemirror/src/extension.ts:1001 packages/codemirror/src/extension.ts:1025
 msgid "Unfolded lines"
 msgstr "展开的行"
 
-#: packages/codemirror/src/extension.ts:1002
+#: packages/codemirror/src/extension.ts:1002 packages/codemirror/src/extension.ts:1026
 msgid "to"
 msgstr "至"
 
-#: packages/codemirror/src/extension.ts:1003
+#: packages/codemirror/src/extension.ts:1003 packages/codemirror/src/extension.ts:1027
 msgid "folded code"
 msgstr "折叠的代码"
 
-#: packages/codemirror/src/extension.ts:1004
+#: packages/codemirror/src/extension.ts:1004 packages/codemirror/src/extension.ts:1028
 msgid "unfold"
 msgstr "展开"
 
-#: packages/codemirror/src/extension.ts:1005
+#: packages/codemirror/src/extension.ts:1005 packages/codemirror/src/extension.ts:1029
 msgid "Fold line"
 msgstr "折叠一行"
 
-#: packages/codemirror/src/extension.ts:1006
+#: packages/codemirror/src/extension.ts:1006 packages/codemirror/src/extension.ts:1030
 msgid "Unfold line"
 msgstr "展开一行"
 
-#: packages/codemirror/src/extension.ts:1008
+#: packages/codemirror/src/extension.ts:1007 packages/codemirror/src/extension.ts:983
+msgid "CodeMirror theme"
+msgstr "CodeMirror 主题"
+
+#: packages/codemirror/src/extension.ts:1008 packages/codemirror/src/extension.ts:1032
 msgid "Go to line"
 msgstr "跳转到行"
 
-#: packages/codemirror/src/extension.ts:1009
+#: packages/codemirror/src/extension.ts:1009 packages/codemirror/src/extension.ts:1033
 msgid "go"
 msgstr "转至"
 
-#: packages/codemirror/src/extension.ts:1010 packages/documentsearch/src/searchview.tsx:173 packages/documentsearch/src/searchview.tsx:178
+#: packages/codemirror/src/extension.ts:1010 packages/codemirror/src/extension.ts:1034 packages/documentsearch/src/searchview.tsx:173 packages/documentsearch/src/searchview.tsx:178
 msgid "Find"
 msgstr "查找"
 
-#: packages/codemirror/src/extension.ts:1011 packages/documentsearch/src/searchview.tsx:236 packages/documentsearch/src/searchview.tsx:240 packages/documentsearch/src/searchview.tsx:267
+#: packages/codemirror/src/extension.ts:1011 packages/codemirror/src/extension.ts:1035 packages/documentsearch/src/searchview.tsx:236 packages/documentsearch/src/searchview.tsx:240 packages/documentsearch/src/searchview.tsx:267
 msgid "Replace"
 msgstr "替换"
 
-#: packages/codemirror/src/extension.ts:1012
+#: packages/codemirror/src/extension.ts:1012 packages/codemirror/src/extension.ts:1036
 msgid "next"
 msgstr "下一个"
 
-#: packages/codemirror/src/extension.ts:1013
+#: packages/codemirror/src/extension.ts:1013 packages/codemirror/src/extension.ts:1037
 msgid "previous"
 msgstr "上一个"
 
-#: packages/codemirror/src/extension.ts:1014
+#: packages/codemirror/src/extension.ts:1014 packages/codemirror/src/extension.ts:1038
 msgid "all"
 msgstr "全部"
 
-#: packages/codemirror/src/extension.ts:1015
+#: packages/codemirror/src/extension.ts:1015 packages/codemirror/src/extension.ts:1039
 msgid "match case"
 msgstr "区分大小写"
 
-#: packages/codemirror/src/extension.ts:1016
+#: packages/codemirror/src/extension.ts:1016 packages/codemirror/src/extension.ts:1040
 msgid "replace"
 msgstr "替换"
 
-#: packages/codemirror/src/extension.ts:1017
+#: packages/codemirror/src/extension.ts:1017 packages/codemirror/src/extension.ts:1041
 msgid "replace all"
 msgstr "全部替换"
 
-#: packages/codemirror/src/extension.ts:1018
+#: packages/codemirror/src/extension.ts:1018 packages/codemirror/src/extension.ts:1042
 msgid "close"
 msgstr "关闭"
 
-#: packages/codemirror/src/extension.ts:1019
+#: packages/codemirror/src/extension.ts:1019 packages/codemirror/src/extension.ts:1043
 msgid "current match"
 msgstr "当前匹配项"
 
-#: packages/codemirror/src/extension.ts:1020
+#: packages/codemirror/src/extension.ts:1020 packages/codemirror/src/extension.ts:1044
 msgid "replaced $ matches"
 msgstr "已替换 $ 个匹配项"
 
-#: packages/codemirror/src/extension.ts:1021
+#: packages/codemirror/src/extension.ts:1020 packages/codemirror/src/extension.ts:996
+msgid "Control character"
+msgstr "控制字符"
+
+#: packages/codemirror/src/extension.ts:1021 packages/codemirror/src/extension.ts:1045
 msgid "replaced match on line $"
 msgstr "已替换第 $ 行的匹配项"
 
-#: packages/codemirror/src/extension.ts:1022
+#: packages/codemirror/src/extension.ts:1022 packages/codemirror/src/extension.ts:1046
 msgid "on line"
 msgstr "在行上"
 
-#: packages/codemirror/src/extension.ts:1024
+#: packages/codemirror/src/extension.ts:1022 packages/codemirror/src/extension.ts:998
+msgid "Selection deleted"
+msgstr "选区已删除"
+
+#: packages/codemirror/src/extension.ts:1024 packages/codemirror/src/extension.ts:1048
 msgid "Completions"
 msgstr "补全"
 
-#: packages/codemirror/src/extension.ts:1026
+#: packages/codemirror/src/extension.ts:1026 packages/codemirror/src/extension.ts:1050
 msgid "Diagnostics"
 msgstr "诊断信息"
 
-#: packages/codemirror/src/extension.ts:1027
+#: packages/codemirror/src/extension.ts:1027 packages/codemirror/src/extension.ts:1051
 msgid "No diagnostics"
 msgstr "无诊断信息"
 
-#: packages/codemirror/src/extension.ts:619
+#: packages/codemirror/src/extension.ts:618 packages/codemirror/src/extension.ts:619
 msgid "Auto Closing Brackets"
 msgstr "自动闭合括号"
 
-#: packages/codemirror/src/extension.ts:628
+#: packages/codemirror/src/extension.ts:627 packages/codemirror/src/extension.ts:628
 msgid "Code Folding"
 msgstr "代码折叠"
 
-#: packages/codemirror/src/extension.ts:640
+#: packages/codemirror/src/extension.ts:639 packages/codemirror/src/extension.ts:640
 msgid "Cursor blinking rate"
 msgstr "光标闪烁频率"
 
-#: packages/codemirror/src/extension.ts:641
+#: packages/codemirror/src/extension.ts:640 packages/codemirror/src/extension.ts:641
 msgid "Half-period in milliseconds used for cursor blinking. The default blink rate is 1200ms. By setting this to zero, blinking can be disabled."
 msgstr "光标闪烁所用的半个时间段，以毫秒为单位。默认闪烁率是1200毫秒。通过设置这个为零，闪烁可以被禁用。"
 
-#: packages/codemirror/src/extension.ts:652
+#: packages/codemirror/src/extension.ts:651 packages/codemirror/src/extension.ts:652
 msgid "Highlight the active line"
 msgstr "高亮显示活动行"
 
-#: packages/codemirror/src/extension.ts:661
+#: packages/codemirror/src/extension.ts:660 packages/codemirror/src/extension.ts:661
 msgid "Highlight special characters"
 msgstr "高亮显示特殊字符"
 
-#: packages/codemirror/src/extension.ts:671
+#: packages/codemirror/src/extension.ts:670 packages/codemirror/src/extension.ts:671
 msgid "Highlight trailing white spaces"
 msgstr "高亮尾随的空格"
 
-#: packages/codemirror/src/extension.ts:680
+#: packages/codemirror/src/extension.ts:679 packages/codemirror/src/extension.ts:680
 msgid "Highlight white spaces"
 msgstr "突出显示空格"
 
-#: packages/codemirror/src/extension.ts:694
+#: packages/codemirror/src/extension.ts:693 packages/codemirror/src/extension.ts:694
 msgid "Indentation unit"
 msgstr "缩进单位"
 
-#: packages/codemirror/src/extension.ts:695
+#: packages/codemirror/src/extension.ts:694 packages/codemirror/src/extension.ts:695
 msgid "The indentation is a `Tab` or the number of spaces. This defaults to 4 spaces."
 msgstr "缩进可以是 `Tab` 或者空格的数量。默认情况下，缩进为 4 个空格。"
 
-#: packages/codemirror/src/extension.ts:730
+#: packages/codemirror/src/extension.ts:730 packages/codemirror/src/extension.ts:755
 msgid "Line Numbers"
 msgstr "行号"
 
-#: packages/codemirror/src/extension.ts:739
+#: packages/codemirror/src/extension.ts:739 packages/codemirror/src/extension.ts:764
 msgid "Line Wrap"
 msgstr "换行"
 
-#: packages/codemirror/src/extension.ts:753 packages/fileeditor-extension/src/commands.ts:422 packages/fileeditor-extension/src/commands.ts:429 packages/mainmenu-extension/src/index.ts:588
+#: packages/codemirror/src/extension.ts:753 packages/codemirror/src/extension.ts:778 packages/fileeditor-extension/src/commands.ts:422 packages/fileeditor-extension/src/commands.ts:423 packages/fileeditor-extension/src/commands.ts:429 packages/fileeditor-extension/src/commands.ts:430 packages/mainmenu-extension/src/index.ts:584 packages/mainmenu-extension/src/index.ts:588
 msgid "Match Brackets"
 msgstr "高亮显示括号对"
 
-#: packages/codemirror/src/extension.ts:766
+#: packages/codemirror/src/extension.ts:766 packages/codemirror/src/extension.ts:791
 msgid "Rectangular selection"
 msgstr "矩形选区"
 
-#: packages/codemirror/src/extension.ts:767
+#: packages/codemirror/src/extension.ts:767 packages/codemirror/src/extension.ts:792
 msgid "Rectangular (block) selection can be created by dragging the mouse pointer while holding the left mouse button and the Alt key. When the Alt key is pressed, a crosshair cursor will appear, indicating that the rectangular selection mode is active."
 msgstr "可以通过按住鼠标左键和Alt键拖动鼠标指针来创建矩形（块）选区。当按下Alt键时，将出现十字光标，表示矩形选区模式已激活。"
 
-#: packages/codemirror/src/extension.ts:792
+#: packages/codemirror/src/extension.ts:792 packages/codemirror/src/extension.ts:817
 msgid "Rulers"
 msgstr "标尺"
 
-#: packages/codemirror/src/extension.ts:860
+#: packages/codemirror/src/extension.ts:860 packages/codemirror/src/extension.ts:884
 msgid "Smart Indentation"
 msgstr "智能缩进"
 
-#: packages/codemirror/src/extension.ts:908
+#: packages/codemirror/src/extension.ts:908 packages/codemirror/src/extension.ts:932
 msgid "Tab size"
 msgstr "制表符宽度"
 
-#: packages/codemirror/src/extension.ts:933
+#: packages/codemirror/src/extension.ts:933 packages/codemirror/src/extension.ts:957
 msgid "Multiple selections"
 msgstr "多重选择"
 
-#: packages/codemirror/src/extension.ts:948
+#: packages/codemirror/src/extension.ts:948 packages/codemirror/src/extension.ts:972
 msgid "Custom editor styles"
 msgstr "自定义编辑器样式"
 
-#: packages/codemirror/src/extension.ts:953
+#: packages/codemirror/src/extension.ts:953 packages/codemirror/src/extension.ts:977
 msgid "Font Family"
 msgstr "字体集"
 
-#: packages/codemirror/src/extension.ts:959
+#: packages/codemirror/src/extension.ts:959 packages/codemirror/src/extension.ts:983
 msgid "Font Size"
 msgstr "字体大小"
 
-#: packages/codemirror/src/extension.ts:963
+#: packages/codemirror/src/extension.ts:963 packages/codemirror/src/extension.ts:987
 msgid "Line Height"
 msgstr "行高"
 
-#: packages/codemirror/src/extension.ts:983
-msgid "CodeMirror theme"
-msgstr "CodeMirror 主题"
-
-#: packages/codemirror/src/extension.ts:996
-msgid "Control character"
-msgstr "控制字符"
-
-#: packages/codemirror/src/extension.ts:998
-msgid "Selection deleted"
-msgstr "选区已删除"
+#: packages/codemirror/src/language.ts:1003 packages/codemirror/src/language.ts:996
+msgid "IDL"
+msgstr "IDL"
 
-#: packages/codemirror/src/language.ts:1006
+#: packages/codemirror/src/language.ts:1006 packages/codemirror/src/language.ts:1013
 msgid "JSON-LD"
 msgstr "JSON-LD"
 
-#: packages/codemirror/src/language.ts:1017
+#: packages/codemirror/src/language.ts:1017 packages/codemirror/src/language.ts:1024
 msgid "Jinja2"
 msgstr "Jinja2"
 
-#: packages/codemirror/src/language.ts:1027
+#: packages/codemirror/src/language.ts:1027 packages/codemirror/src/language.ts:1034
 msgid "Julia"
 msgstr "Julia"
 
-#: packages/codemirror/src/language.ts:1037
+#: packages/codemirror/src/language.ts:1037 packages/codemirror/src/language.ts:1044
 msgid "Kotlin"
 msgstr "Kotlin"
 
-#: packages/codemirror/src/language.ts:1047
+#: packages/codemirror/src/language.ts:1047 packages/codemirror/src/language.ts:1054
 msgid "LESS"
 msgstr "LESS"
 
-#: packages/codemirror/src/language.ts:1057
+#: packages/codemirror/src/language.ts:1057 packages/codemirror/src/language.ts:1064
 msgid "LiveScript"
 msgstr "LiveScript"
 
-#: packages/codemirror/src/language.ts:1068
+#: packages/codemirror/src/language.ts:1068 packages/codemirror/src/language.ts:1075
 msgid "Lua"
 msgstr "Lua"
 
-#: packages/codemirror/src/language.ts:1078
+#: packages/codemirror/src/language.ts:1078 packages/codemirror/src/language.ts:1085
 msgid "mIRC"
 msgstr "mIRC"
 
-#: packages/codemirror/src/language.ts:1087
+#: packages/codemirror/src/language.ts:1087 packages/codemirror/src/language.ts:1094
 msgid "Mathematica"
 msgstr "Mathematica"
 
-#: packages/codemirror/src/language.ts:1097
+#: packages/codemirror/src/language.ts:1097 packages/codemirror/src/language.ts:1104
 msgid "Modelica"
 msgstr "Modelica"
 
-#: packages/codemirror/src/language.ts:1107
+#: packages/codemirror/src/language.ts:1107 packages/codemirror/src/language.ts:1114
 msgid "MUMPS"
 msgstr "MUMPS"
 
-#: packages/codemirror/src/language.ts:1117
+#: packages/codemirror/src/language.ts:1117 packages/codemirror/src/language.ts:1124
 msgid "mbox"
 msgstr "mbox"
 
-#: packages/codemirror/src/language.ts:1127
+#: packages/codemirror/src/language.ts:1127 packages/codemirror/src/language.ts:1134
 msgid "Nginx"
 msgstr "Nginx"
 
-#: packages/codemirror/src/language.ts:1137
+#: packages/codemirror/src/language.ts:1137 packages/codemirror/src/language.ts:1144
 msgid "NSIS"
 msgstr "NSIS"
 
-#: packages/codemirror/src/language.ts:1147
+#: packages/codemirror/src/language.ts:1147 packages/codemirror/src/language.ts:1154
 msgid "NTriples"
 msgstr "NTriples"
 
-#: packages/codemirror/src/language.ts:1161
+#: packages/codemirror/src/language.ts:1161 packages/codemirror/src/language.ts:1168
 msgid "Objective-C"
 msgstr "Objective-C"
 
-#: packages/codemirror/src/language.ts:1172
+#: packages/codemirror/src/language.ts:1172 packages/codemirror/src/language.ts:1179
 msgid "Objective-C++"
 msgstr "Objective-C++"
 
-#: packages/codemirror/src/language.ts:1183
+#: packages/codemirror/src/language.ts:1183 packages/codemirror/src/language.ts:1190
 msgid "OCaml"
 msgstr "OCaml"
 
-#: packages/codemirror/src/language.ts:1193
+#: packages/codemirror/src/language.ts:1193 packages/codemirror/src/language.ts:1200
 msgid "Octave"
 msgstr "Octave"
 
-#: packages/codemirror/src/language.ts:1203
+#: packages/codemirror/src/language.ts:1203 packages/codemirror/src/language.ts:1210
 msgid "Oz"
 msgstr "Oz"
 
-#: packages/codemirror/src/language.ts:1213
+#: packages/codemirror/src/language.ts:1213 packages/codemirror/src/language.ts:1220
 msgid "Pascal"
 msgstr "Pascal"
 
-#: packages/codemirror/src/language.ts:1223
+#: packages/codemirror/src/language.ts:1223 packages/codemirror/src/language.ts:1230
 msgid "Perl"
 msgstr "Perl"
 
-#: packages/codemirror/src/language.ts:1233
+#: packages/codemirror/src/language.ts:1233 packages/codemirror/src/language.ts:1240
 msgid "Pig"
 msgstr "Pig"
 
-#: packages/codemirror/src/language.ts:1243
+#: packages/codemirror/src/language.ts:1243 packages/codemirror/src/language.ts:1250
 msgid "PowerShell"
 msgstr "PowerShell"
 
-#: packages/codemirror/src/language.ts:1253
+#: packages/codemirror/src/language.ts:1253 packages/codemirror/src/language.ts:1260
 msgid "Properties files"
 msgstr "属性文件"
 
-#: packages/codemirror/src/language.ts:1264
+#: packages/codemirror/src/language.ts:1264 packages/codemirror/src/language.ts:1271
 msgid "ProtoBuf"
 msgstr "ProtoBuf"
 
-#: packages/codemirror/src/language.ts:1274
+#: packages/codemirror/src/language.ts:1274 packages/codemirror/src/language.ts:1281
 msgid "Puppet"
 msgstr "Puppet"
 
-#: packages/codemirror/src/language.ts:1284
+#: packages/codemirror/src/language.ts:1284 packages/codemirror/src/language.ts:1291
 msgid "Q"
 msgstr "Q"
 
-#: packages/codemirror/src/language.ts:1294
+#: packages/codemirror/src/language.ts:1294 packages/codemirror/src/language.ts:1301
 msgid "R"
 msgstr "R"
 
-#: packages/codemirror/src/language.ts:1305
+#: packages/codemirror/src/language.ts:1305 packages/codemirror/src/language.ts:1312
 msgid "RPM Changes"
 msgstr "RPM 更改"
 
-#: packages/codemirror/src/language.ts:1314
+#: packages/codemirror/src/language.ts:1314 packages/codemirror/src/language.ts:1321
 msgid "RPM Spec"
 msgstr "RPM 规范"
 
-#: packages/codemirror/src/language.ts:1324
+#: packages/codemirror/src/language.ts:1324 packages/codemirror/src/language.ts:1331
 msgid "Ruby"
 msgstr "Ruby"
 
-#: packages/codemirror/src/language.ts:1335
+#: packages/codemirror/src/language.ts:1335 packages/codemirror/src/language.ts:1342
 msgid "SAS"
 msgstr "SAS"
 
-#: packages/codemirror/src/language.ts:1345
+#: packages/codemirror/src/language.ts:1345 packages/codemirror/src/language.ts:1352
 msgid "Scala"
 msgstr "Scata"
 
-#: packages/codemirror/src/language.ts:1355
+#: packages/codemirror/src/language.ts:1355 packages/codemirror/src/language.ts:1362
 msgid "Scheme"
 msgstr "Scheme"
 
-#: packages/codemirror/src/language.ts:1365
+#: packages/codemirror/src/language.ts:1365 packages/codemirror/src/language.ts:1372
 msgid "SCSS"
 msgstr "SCSS"
 
-#: packages/codemirror/src/language.ts:1375
+#: packages/codemirror/src/language.ts:1375 packages/codemirror/src/language.ts:1382
 msgid "Shell"
 msgstr "Shell"
 
-#: packages/codemirror/src/language.ts:1387
+#: packages/codemirror/src/language.ts:1387 packages/codemirror/src/language.ts:1394
 msgid "Sieve"
 msgstr "Sieve"
 
-#: packages/codemirror/src/language.ts:1397
+#: packages/codemirror/src/language.ts:1397 packages/codemirror/src/language.ts:1404
 msgid "Smalltalk"
 msgstr "Smalltalk"
 
-#: packages/codemirror/src/language.ts:1407
+#: packages/codemirror/src/language.ts:1407 packages/codemirror/src/language.ts:1414
 msgid "Solr"
 msgstr "Solr"
 
-#: packages/codemirror/src/language.ts:1416
+#: packages/codemirror/src/language.ts:1416 packages/codemirror/src/language.ts:1423
 msgid "SML"
 msgstr "SML"
 
-#: packages/codemirror/src/language.ts:1426
+#: packages/codemirror/src/language.ts:1426 packages/codemirror/src/language.ts:1433
 msgid "SPARQL"
 msgstr "SPARQL"
 
-#: packages/codemirror/src/language.ts:1437
+#: packages/codemirror/src/language.ts:1437 packages/codemirror/src/language.ts:1444
 msgid "Spreadsheet"
 msgstr "电子表格"
 
-#: packages/codemirror/src/language.ts:1447
+#: packages/codemirror/src/language.ts:1447 packages/codemirror/src/language.ts:1454
 msgid "Squirrel"
 msgstr "Squirrel"
 
-#: packages/codemirror/src/language.ts:1457
+#: packages/codemirror/src/language.ts:1457 packages/codemirror/src/language.ts:1464
 msgid "Stylus"
 msgstr "Stylus"
 
-#: packages/codemirror/src/language.ts:1467
+#: packages/codemirror/src/language.ts:1467 packages/codemirror/src/language.ts:1474
 msgid "Swift"
 msgstr "Swift"
 
-#: packages/codemirror/src/language.ts:1477
+#: packages/codemirror/src/language.ts:1477 packages/codemirror/src/language.ts:1484
 msgid "sTeX"
 msgstr "sTeX"
 
-#: packages/codemirror/src/language.ts:1486 packages/notebook-extension/src/index.ts:3800
+#: packages/codemirror/src/language.ts:1486 packages/codemirror/src/language.ts:1493 packages/notebook-extension/src/index.ts:3800 packages/notebook-extension/src/index.ts:3807 packages/notebook-extension/src/index.ts:3866
 msgid "LaTeX"
 msgstr "LaTeX"
 
-#: packages/codemirror/src/language.ts:1497
+#: packages/codemirror/src/language.ts:1497 packages/codemirror/src/language.ts:1504
 msgid "SystemVerilog"
 msgstr "SystemVerilog"
 
-#: packages/codemirror/src/language.ts:1507
+#: packages/codemirror/src/language.ts:1507 packages/codemirror/src/language.ts:1514
 msgid "Tcl"
 msgstr "Tcl"
 
-#: packages/codemirror/src/language.ts:1517
+#: packages/codemirror/src/language.ts:1517 packages/codemirror/src/language.ts:1524
 msgid "Textile"
 msgstr "家纺"
 
-#: packages/codemirror/src/language.ts:1527
+#: packages/codemirror/src/language.ts:1527 packages/codemirror/src/language.ts:1534
 msgid "TiddlyWiki"
 msgstr "TiddlyWiki"
 
-#: packages/codemirror/src/language.ts:1536
+#: packages/codemirror/src/language.ts:1536 packages/codemirror/src/language.ts:1543
 msgid "Tiki wiki"
 msgstr "Tiki wiki"
 
-#: packages/codemirror/src/language.ts:1545
+#: packages/codemirror/src/language.ts:1545 packages/codemirror/src/language.ts:1552
 msgid "TOML"
 msgstr "TOML"
 
-#: packages/codemirror/src/language.ts:1555
+#: packages/codemirror/src/language.ts:1555 packages/codemirror/src/language.ts:1562
 msgid "troff"
 msgstr "troff"
 
-#: packages/codemirror/src/language.ts:1565
+#: packages/codemirror/src/language.ts:1565 packages/codemirror/src/language.ts:1572
 msgid "TTCN"
 msgstr "TTCN"
 
-#: packages/codemirror/src/language.ts:1575
+#: packages/codemirror/src/language.ts:1575 packages/codemirror/src/language.ts:1582
 msgid "TTCN_CFG"
 msgstr "TTCN_CFG"
 
-#: packages/codemirror/src/language.ts:1585
+#: packages/codemirror/src/language.ts:1585 packages/codemirror/src/language.ts:1592
 msgid "Turtle"
 msgstr "Turtle"
 
-#: packages/codemirror/src/language.ts:1595
+#: packages/codemirror/src/language.ts:1595 packages/codemirror/src/language.ts:1602
 msgid "Web IDL"
 msgstr "Web IDL"
 
-#: packages/codemirror/src/language.ts:1605
+#: packages/codemirror/src/language.ts:1605 packages/codemirror/src/language.ts:1612
 msgid "VB.NET"
 msgstr "VB.NET"
 
-#: packages/codemirror/src/language.ts:1615
+#: packages/codemirror/src/language.ts:1615 packages/codemirror/src/language.ts:1622
 msgid "VBScript"
 msgstr "VBScript"
 
-#: packages/codemirror/src/language.ts:1625
+#: packages/codemirror/src/language.ts:1625 packages/codemirror/src/language.ts:1632
 msgid "Velocity"
 msgstr "Velocity"
 
-#: packages/codemirror/src/language.ts:1635
+#: packages/codemirror/src/language.ts:1635 packages/codemirror/src/language.ts:1642
 msgid "Verilog"
 msgstr "Verilog"
 
-#: packages/codemirror/src/language.ts:1645
+#: packages/codemirror/src/language.ts:1645 packages/codemirror/src/language.ts:1652
 msgid "VHDL"
 msgstr "VHDL"
 
-#: packages/codemirror/src/language.ts:1655
+#: packages/codemirror/src/language.ts:1655 packages/codemirror/src/language.ts:1662
 msgid "XQuery"
 msgstr "XQuery"
 
-#: packages/codemirror/src/language.ts:1665
+#: packages/codemirror/src/language.ts:1665 packages/codemirror/src/language.ts:1672
 msgid "Yacas"
 msgstr "Yacas"
 
-#: packages/codemirror/src/language.ts:1675
+#: packages/codemirror/src/language.ts:1675 packages/codemirror/src/language.ts:1682
 msgid "YAML"
 msgstr "YAML"
 
-#: packages/codemirror/src/language.ts:1686
+#: packages/codemirror/src/language.ts:1686 packages/codemirror/src/language.ts:1693
 msgid "Z80"
 msgstr "Z80"
 
-#: packages/codemirror/src/language.ts:1696
+#: packages/codemirror/src/language.ts:1696 packages/codemirror/src/language.ts:1703
 msgid "mscgen"
 msgstr "mscgen"
 
-#: packages/codemirror/src/language.ts:1706
+#: packages/codemirror/src/language.ts:1706 packages/codemirror/src/language.ts:1713
 msgid "xu"
 msgstr "xu"
 
-#: packages/codemirror/src/language.ts:1716
+#: packages/codemirror/src/language.ts:1716 packages/codemirror/src/language.ts:1723
 msgid "msgenny"
 msgstr "msgenny"
 
-#: packages/codemirror/src/language.ts:307
+#: packages/codemirror/src/language.ts:307 packages/codemirror/src/language.ts:308
 msgid "C"
 msgstr "C"
 
-#: packages/codemirror/src/language.ts:317
+#: packages/codemirror/src/language.ts:317 packages/codemirror/src/language.ts:318
 msgid "C++"
 msgstr "C++"
 
-#: packages/codemirror/src/language.ts:327
+#: packages/codemirror/src/language.ts:327 packages/codemirror/src/language.ts:328
 msgid "CQL"
 msgstr "CQL"
 
-#: packages/codemirror/src/language.ts:336
+#: packages/codemirror/src/language.ts:336 packages/codemirror/src/language.ts:337
 msgid "CSS"
 msgstr "CSS"
 
-#: packages/codemirror/src/language.ts:346 packages/notebook-extension/src/index.ts:3799
+#: packages/codemirror/src/language.ts:346 packages/codemirror/src/language.ts:347 packages/notebook-extension/src/index.ts:3799 packages/notebook-extension/src/index.ts:3806 packages/notebook-extension/src/index.ts:3865
 msgid "HTML"
 msgstr "HTML"
 
-#: packages/codemirror/src/language.ts:357
+#: packages/codemirror/src/language.ts:357 packages/codemirror/src/language.ts:358
 msgid "Java"
 msgstr "Java"
 
-#: packages/codemirror/src/language.ts:367
+#: packages/codemirror/src/language.ts:367 packages/codemirror/src/language.ts:368
 msgid "Javascript"
 msgstr "JavaScript"
 
-#: packages/codemirror/src/language.ts:384
+#: packages/codemirror/src/language.ts:384 packages/codemirror/src/language.ts:385
 msgid "JSON"
 msgstr "JSON"
 
-#: packages/codemirror/src/language.ts:395
+#: packages/codemirror/src/language.ts:395 packages/codemirror/src/language.ts:396
 msgid "JSX"
 msgstr "JSX"
 
-#: packages/codemirror/src/language.ts:405
+#: packages/codemirror/src/language.ts:405 packages/codemirror/src/language.ts:406
 msgid "MariaDB SQL"
 msgstr "MariaDB SQL"
 
-#: packages/codemirror/src/language.ts:413 packages/notebook-extension/src/index.ts:3801 packages/notebook/src/default-toolbar.tsx:379
+#: packages/codemirror/src/language.ts:413 packages/codemirror/src/language.ts:414 packages/notebook-extension/src/index.ts:3801 packages/notebook-extension/src/index.ts:3808 packages/notebook-extension/src/index.ts:3867 packages/notebook/src/default-toolbar.tsx:379
 msgid "Markdown"
 msgstr "Markdown"
 
-#: packages/codemirror/src/language.ts:423
+#: packages/codemirror/src/language.ts:423 packages/codemirror/src/language.ts:424
 msgid "MS SQL"
 msgstr "MS SQL"
 
-#: packages/codemirror/src/language.ts:431
+#: packages/codemirror/src/language.ts:431 packages/codemirror/src/language.ts:432
 msgid "MySQL"
 msgstr "MySQL"
 
-#: packages/codemirror/src/language.ts:439
+#: packages/codemirror/src/language.ts:439 packages/codemirror/src/language.ts:440
 msgid "PHP"
 msgstr "PHP"
 
-#: packages/codemirror/src/language.ts:453
+#: packages/codemirror/src/language.ts:453 packages/codemirror/src/language.ts:454
 msgid "PLSQL"
 msgstr "PLSQL"
 
-#: packages/codemirror/src/language.ts:462
+#: packages/codemirror/src/language.ts:462 packages/codemirror/src/language.ts:463
 msgid "PostgreSQL"
 msgstr "PostgreSQL"
 
-#: packages/codemirror/src/language.ts:470
+#: packages/codemirror/src/language.ts:470 packages/codemirror/src/language.ts:471
 msgid "Python"
 msgstr "Python"
 
-#: packages/codemirror/src/language.ts:481
+#: packages/codemirror/src/language.ts:481 packages/codemirror/src/language.ts:485
 msgid "ipython"
 msgstr "ipython"
 
-#: packages/codemirror/src/language.ts:493
+#: packages/codemirror/src/language.ts:493 packages/codemirror/src/language.ts:500
 msgid "Rust"
 msgstr "Rust"
 
-#: packages/codemirror/src/language.ts:503
+#: packages/codemirror/src/language.ts:503 packages/codemirror/src/language.ts:510
 msgid "SQL"
 msgstr "SQL"
 
-#: packages/codemirror/src/language.ts:512
+#: packages/codemirror/src/language.ts:512 packages/codemirror/src/language.ts:519
 msgid "SQLite"
 msgstr "SQLite"
 
-#: packages/codemirror/src/language.ts:520
+#: packages/codemirror/src/language.ts:520 packages/codemirror/src/language.ts:527
 msgid "TSX"
 msgstr "TSX"
 
-#: packages/codemirror/src/language.ts:531
+#: packages/codemirror/src/language.ts:531 packages/codemirror/src/language.ts:538
 msgid "TypeScript"
 msgstr "TypeScript"
 
-#: packages/codemirror/src/language.ts:542
+#: packages/codemirror/src/language.ts:542 packages/codemirror/src/language.ts:549
 msgid "WebAssembly"
 msgstr "WebAssembly"
 
-#: packages/codemirror/src/language.ts:552
+#: packages/codemirror/src/language.ts:552 packages/codemirror/src/language.ts:559
 msgid "XML"
 msgstr "XML"
 
-#: packages/codemirror/src/language.ts:564
+#: packages/codemirror/src/language.ts:564 packages/codemirror/src/language.ts:571
 msgid "APL"
 msgstr "APL"
 
-#: packages/codemirror/src/language.ts:574
+#: packages/codemirror/src/language.ts:574 packages/codemirror/src/language.ts:581
 msgid "PGP"
 msgstr "PGP"
 
-#: packages/codemirror/src/language.ts:590
+#: packages/codemirror/src/language.ts:590 packages/codemirror/src/language.ts:597
 msgid "ASN.1"
 msgstr "ASN.1"
 
-#: packages/codemirror/src/language.ts:600
+#: packages/codemirror/src/language.ts:600 packages/codemirror/src/language.ts:607
 msgid "Asterisk"
 msgstr "Asterisk"
 
-#: packages/codemirror/src/language.ts:610
+#: packages/codemirror/src/language.ts:610 packages/codemirror/src/language.ts:617
 msgid "Brainfuck"
 msgstr "Brainfuck"
 
-#: packages/codemirror/src/language.ts:620
+#: packages/codemirror/src/language.ts:620 packages/codemirror/src/language.ts:627
 msgid "Cobol"
 msgstr "Cobol"
 
-#: packages/codemirror/src/language.ts:630
+#: packages/codemirror/src/language.ts:630 packages/codemirror/src/language.ts:637
 msgid "C#"
 msgstr "C#"
 
-#: packages/codemirror/src/language.ts:641
+#: packages/codemirror/src/language.ts:641 packages/codemirror/src/language.ts:648
 msgid "Clojure"
 msgstr "Clojure"
 
-#: packages/codemirror/src/language.ts:651
+#: packages/codemirror/src/language.ts:651 packages/codemirror/src/language.ts:658
 msgid "ClojureScript"
 msgstr "ClojureScript"
 
-#: packages/codemirror/src/language.ts:661
+#: packages/codemirror/src/language.ts:661 packages/codemirror/src/language.ts:668
 msgid "Closure Stylesheets (GSS)"
 msgstr "Closure Stylesheets (GSS)"
 
-#: packages/codemirror/src/language.ts:671
+#: packages/codemirror/src/language.ts:671 packages/codemirror/src/language.ts:678
 msgid "CMake"
 msgstr "CMake"
 
-#: packages/codemirror/src/language.ts:682
+#: packages/codemirror/src/language.ts:682 packages/codemirror/src/language.ts:689
 msgid "CoffeeScript"
 msgstr "CoffeeScript"
 
-#: packages/codemirror/src/language.ts:697
+#: packages/codemirror/src/language.ts:697 packages/codemirror/src/language.ts:704
 msgid "Common Lisp"
 msgstr "Common Lisp"
 
-#: packages/codemirror/src/language.ts:708
+#: packages/codemirror/src/language.ts:708 packages/codemirror/src/language.ts:715
 msgid "Cypher"
 msgstr "Cypher"
 
-#: packages/codemirror/src/language.ts:718
+#: packages/codemirror/src/language.ts:718 packages/codemirror/src/language.ts:725
 msgid "Cython"
 msgstr "Cython"
 
-#: packages/codemirror/src/language.ts:728
+#: packages/codemirror/src/language.ts:728 packages/codemirror/src/language.ts:735
 msgid "Crystal"
 msgstr "Crystal"
 
-#: packages/codemirror/src/language.ts:738
+#: packages/codemirror/src/language.ts:738 packages/codemirror/src/language.ts:745
 msgid "D"
 msgstr "D"
 
-#: packages/codemirror/src/language.ts:748
+#: packages/codemirror/src/language.ts:748 packages/codemirror/src/language.ts:755
 msgid "Dart"
 msgstr "Dart"
 
-#: packages/codemirror/src/language.ts:758
+#: packages/codemirror/src/language.ts:758 packages/codemirror/src/language.ts:765
 msgid "diff"
 msgstr "差异对比"
 
-#: packages/codemirror/src/language.ts:768
+#: packages/codemirror/src/language.ts:768 packages/codemirror/src/language.ts:775
 msgid "Dockerfile"
 msgstr "Dockerfile"
 
-#: packages/codemirror/src/language.ts:778
+#: packages/codemirror/src/language.ts:778 packages/codemirror/src/language.ts:785
 msgid "DTD"
 msgstr "DTD"
 
-#: packages/codemirror/src/language.ts:788
+#: packages/codemirror/src/language.ts:788 packages/codemirror/src/language.ts:795
 msgid "Dylan"
 msgstr "Dylan"
 
-#: packages/codemirror/src/language.ts:798
+#: packages/codemirror/src/language.ts:798 packages/codemirror/src/language.ts:805
 msgid "EBNF"
 msgstr "EBNF"
 
-#: packages/codemirror/src/language.ts:807
+#: packages/codemirror/src/language.ts:807 packages/codemirror/src/language.ts:814
 msgid "ECL"
 msgstr "ECL"
 
-#: packages/codemirror/src/language.ts:817
+#: packages/codemirror/src/language.ts:817 packages/codemirror/src/language.ts:824
 msgid "edn"
 msgstr "edn"
 
-#: packages/codemirror/src/language.ts:827
+#: packages/codemirror/src/language.ts:827 packages/codemirror/src/language.ts:834
 msgid "Eiffel"
 msgstr "Eiffel"
 
-#: packages/codemirror/src/language.ts:837
+#: packages/codemirror/src/language.ts:837 packages/codemirror/src/language.ts:844
 msgid "Elm"
 msgstr "Elm"
 
-#: packages/codemirror/src/language.ts:847
+#: packages/codemirror/src/language.ts:847 packages/codemirror/src/language.ts:854
 msgid "Erlang"
 msgstr "Erlang"
 
-#: packages/codemirror/src/language.ts:857
+#: packages/codemirror/src/language.ts:857 packages/codemirror/src/language.ts:864
 msgid "Esper"
 msgstr "Esper"
 
-#: packages/codemirror/src/language.ts:866
+#: packages/codemirror/src/language.ts:866 packages/codemirror/src/language.ts:873
 msgid "Factor"
 msgstr "Factor"
 
-#: packages/codemirror/src/language.ts:876
+#: packages/codemirror/src/language.ts:876 packages/codemirror/src/language.ts:883
 msgid "FCL"
 msgstr "FCL"
 
-#: packages/codemirror/src/language.ts:885
+#: packages/codemirror/src/language.ts:885 packages/codemirror/src/language.ts:892
 msgid "Forth"
 msgstr "Forth"
 
-#: packages/codemirror/src/language.ts:895
+#: packages/codemirror/src/language.ts:895 packages/codemirror/src/language.ts:902
 msgid "Fortran"
 msgstr "Fortran"
 
-#: packages/codemirror/src/language.ts:905
+#: packages/codemirror/src/language.ts:905 packages/codemirror/src/language.ts:912
 msgid "F#"
 msgstr "F#"
 
-#: packages/codemirror/src/language.ts:916
+#: packages/codemirror/src/language.ts:916 packages/codemirror/src/language.ts:923
 msgid "Gas"
 msgstr "Gas"
 
-#: packages/codemirror/src/language.ts:926
+#: packages/codemirror/src/language.ts:926 packages/codemirror/src/language.ts:933
 msgid "Gherkin"
 msgstr "Gherkin"
 
-#: packages/codemirror/src/language.ts:936
+#: packages/codemirror/src/language.ts:936 packages/codemirror/src/language.ts:943
 msgid "Go"
 msgstr "Go"
 
-#: packages/codemirror/src/language.ts:946
+#: packages/codemirror/src/language.ts:946 packages/codemirror/src/language.ts:953
 msgid "Groovy"
 msgstr "Groovy"
 
-#: packages/codemirror/src/language.ts:957
+#: packages/codemirror/src/language.ts:957 packages/codemirror/src/language.ts:964
 msgid "Haskell"
 msgstr "Haskell"
 
-#: packages/codemirror/src/language.ts:967
+#: packages/codemirror/src/language.ts:967 packages/codemirror/src/language.ts:974
 msgid "Haxe"
 msgstr "Haxe"
 
-#: packages/codemirror/src/language.ts:977
+#: packages/codemirror/src/language.ts:977 packages/codemirror/src/language.ts:984
 msgid "HXML"
 msgstr "HXML"
 
-#: packages/codemirror/src/language.ts:987
+#: packages/codemirror/src/language.ts:987 packages/codemirror/src/language.ts:994
 msgid "HTTP"
 msgstr "HTTP"
 
-#: packages/codemirror/src/language.ts:996
-msgid "IDL"
-msgstr "IDL"
-
-#: packages/codemirror/src/theme.ts:234
+#: packages/codemirror/src/theme.ts:234 packages/codemirror/src/theme.ts:238
 msgid "codemirror"
 msgstr "codemirror"
 
 #: packages/completer-extension/src/index.ts:138
 msgid "Previous"
 msgstr "上一个"
 
@@ -4009,151 +4099,159 @@
 msgid "%1/%2"
 msgstr "%1/%2"
 
 #: packages/completer/src/inline.ts:393
 msgid "Provider: %1"
 msgstr "提供者：%1"
 
-#: packages/console-extension/src/foreign.ts:66 packages/console-extension/src/index.ts:262 packages/console-extension/src/index.ts:311 packages/console-extension/src/index.ts:530 packages/console/src/panel.ts:333 packages/launcher/src/widget.tsx:116 packages/launcher/src/widget.tsx:121
+#: packages/console-extension/src/foreign.ts:66 packages/console-extension/src/index.ts:262 packages/console-extension/src/index.ts:271 packages/console-extension/src/index.ts:275 packages/console-extension/src/index.ts:311 packages/console-extension/src/index.ts:320 packages/console-extension/src/index.ts:324 packages/console-extension/src/index.ts:530 packages/console-extension/src/index.ts:539 packages/console-extension/src/index.ts:542 packages/console/src/panel.ts:333 packages/console/src/panel.ts:341 packages/launcher/src/widget.tsx:116 packages/launcher/src/widget.tsx:121
 msgid "Console"
 msgstr "控制台"
 
 #: packages/console-extension/src/foreign.ts:80
 msgid "Show All Kernel Activity"
 msgstr "显示所有内核动态"
 
-#: packages/console-extension/src/index.ts:464
+#: packages/console-extension/src/index.ts:464 packages/console-extension/src/index.ts:473 packages/console-extension/src/index.ts:478
 msgid "Auto Close Brackets for Code Console Prompt"
 msgstr "为控制台提示符自动闭合代码"
 
-#: packages/console-extension/src/index.ts:490
+#: packages/console-extension/src/index.ts:490 packages/console-extension/src/index.ts:499 packages/console-extension/src/index.ts:503
 msgid "Open a console for the provided `path`."
 msgstr "为提供的`路径`打开控制台。"
 
-#: packages/console-extension/src/index.ts:519
+#: packages/console-extension/src/index.ts:519 packages/console-extension/src/index.ts:528 packages/console-extension/src/index.ts:531
 msgid "New Console"
 msgstr "新建控制台"
 
-#: packages/console-extension/src/index.ts:554
+#: packages/console-extension/src/index.ts:554 packages/console-extension/src/index.ts:631 packages/console-extension/src/index.ts:634
 msgid "Clear Console Cells"
 msgstr "清除控制台单元格"
 
-#: packages/console-extension/src/index.ts:566
+#: packages/console-extension/src/index.ts:566 packages/console-extension/src/index.ts:643 packages/console-extension/src/index.ts:646
 msgid "Run Cell (unforced)"
 msgstr "运行单元格 (非强制)"
 
-#: packages/console-extension/src/index.ts:578
+#: packages/console-extension/src/index.ts:578 packages/console-extension/src/index.ts:655 packages/console-extension/src/index.ts:658
 msgid "Run Cell (forced)"
 msgstr "运行单元格 (强制)"
 
-#: packages/console-extension/src/index.ts:590
+#: packages/console-extension/src/index.ts:590 packages/console-extension/src/index.ts:667 packages/console-extension/src/index.ts:670
 msgid "Insert Line Break"
 msgstr "插入换行符"
 
-#: packages/console-extension/src/index.ts:602
+#: packages/console-extension/src/index.ts:593 packages/console-extension/src/index.ts:596 packages/fileeditor-extension/src/commands.ts:853 packages/fileeditor-extension/src/commands.ts:854 packages/mainmenu-extension/src/index.ts:277 packages/notebook-extension/src/index.ts:3122 packages/notebook-extension/src/index.ts:3129 packages/notebook-extension/src/index.ts:3152
+msgid "Undo"
+msgstr "撤消"
+
+#: packages/console-extension/src/index.ts:602 packages/console-extension/src/index.ts:679 packages/console-extension/src/index.ts:682
 msgid "Replace Selection in Console"
 msgstr "在控制台中替换选择"
 
-#: packages/console-extension/src/index.ts:615 packages/mainmenu-extension/src/index.ts:468 packages/notebook-extension/src/index.ts:2528
+#: packages/console-extension/src/index.ts:615 packages/console-extension/src/index.ts:692 packages/console-extension/src/index.ts:695 packages/mainmenu-extension/src/index.ts:466 packages/mainmenu-extension/src/index.ts:468 packages/notebook-extension/src/index.ts:2528 packages/notebook-extension/src/index.ts:2535 packages/notebook-extension/src/index.ts:2546
 msgid "Interrupt Kernel"
 msgstr "中断内核"
 
-#: packages/console-extension/src/index.ts:630 packages/mainmenu-extension/src/index.ts:493 packages/notebook-extension/src/index.ts:2376
+#: packages/console-extension/src/index.ts:627 packages/console-extension/src/index.ts:630 packages/fileeditor-extension/src/commands.ts:883 packages/fileeditor-extension/src/commands.ts:884 packages/fileeditor-extension/src/commands.ts:885 packages/mainmenu-extension/src/index.ts:287 packages/mainmenu-extension/src/index.ts:288 packages/notebook-extension/src/index.ts:3108 packages/notebook-extension/src/index.ts:3115 packages/notebook-extension/src/index.ts:3138
+msgid "Redo"
+msgstr "重做"
+
+#: packages/console-extension/src/index.ts:630 packages/console-extension/src/index.ts:707 packages/console-extension/src/index.ts:710 packages/mainmenu-extension/src/index.ts:491 packages/mainmenu-extension/src/index.ts:493 packages/notebook-extension/src/index.ts:2376 packages/notebook-extension/src/index.ts:2383 packages/notebook-extension/src/index.ts:2394
 msgid "Restart Kernel…"
 msgstr "重启内核…"
 
-#: packages/console-extension/src/index.ts:642 packages/lsp-extension/src/index.ts:303 packages/mainmenu-extension/src/index.ts:375 packages/mainmenu-extension/src/index.ts:385 packages/running/src/index.tsx:161 packages/terminal-extension/src/index.ts:322
+#: packages/console-extension/src/index.ts:642 packages/console-extension/src/index.ts:719 packages/console-extension/src/index.ts:722 packages/lsp-extension/src/index.ts:303 packages/mainmenu-extension/src/index.ts:371 packages/mainmenu-extension/src/index.ts:375 packages/mainmenu-extension/src/index.ts:381 packages/mainmenu-extension/src/index.ts:385 packages/running/src/index.tsx:161 packages/running/src/index.tsx:221 packages/terminal-extension/src/index.ts:322
 msgid "Shut Down"
 msgstr "关闭"
 
-#: packages/console-extension/src/index.ts:654
+#: packages/console-extension/src/index.ts:654 packages/console-extension/src/index.ts:731 packages/console-extension/src/index.ts:734
 msgid "Close and Shut Down…"
 msgstr "关闭并终止…"
 
-#: packages/console-extension/src/index.ts:661
+#: packages/console-extension/src/index.ts:661 packages/console-extension/src/index.ts:738 packages/console-extension/src/index.ts:741
 msgid "Shut down the console?"
 msgstr "关闭控制台？"
 
-#: packages/console-extension/src/index.ts:662 packages/notebook-extension/src/index.ts:2414
+#: packages/console-extension/src/index.ts:662 packages/console-extension/src/index.ts:739 packages/console-extension/src/index.ts:742 packages/notebook-extension/src/index.ts:2414 packages/notebook-extension/src/index.ts:2421 packages/notebook-extension/src/index.ts:2432
 msgid "Are you sure you want to close \"%1\"?"
 msgstr "您确定要关闭「%1」吗？"
 
-#: packages/console-extension/src/index.ts:668
+#: packages/console-extension/src/index.ts:668 packages/console-extension/src/index.ts:745 packages/console-extension/src/index.ts:748
 msgid "Cancel console Shut Down"
 msgstr "取消关停控制台"
 
-#: packages/console-extension/src/index.ts:671
+#: packages/console-extension/src/index.ts:671 packages/console-extension/src/index.ts:748 packages/console-extension/src/index.ts:751
 msgid "Confirm console Shut Down"
 msgstr "确认关停控制台"
 
-#: packages/console-extension/src/index.ts:691
+#: packages/console-extension/src/index.ts:691 packages/console-extension/src/index.ts:768 packages/console-extension/src/index.ts:771
 msgid "Inject some code in a console."
 msgstr "在控制台中注入一些代码。"
 
-#: packages/console-extension/src/index.ts:712 packages/mainmenu-extension/src/index.ts:519 packages/notebook-extension/src/index.ts:3136
+#: packages/console-extension/src/index.ts:712 packages/console-extension/src/index.ts:789 packages/console-extension/src/index.ts:792 packages/mainmenu-extension/src/index.ts:518 packages/mainmenu-extension/src/index.ts:519 packages/notebook-extension/src/index.ts:3136 packages/notebook-extension/src/index.ts:3143 packages/notebook-extension/src/index.ts:3166
 msgid "Change Kernel…"
 msgstr "更改内核…"
 
-#: packages/console-extension/src/index.ts:724 packages/mainmenu-extension/src/index.ts:754 packages/notebook-extension/src/index.ts:3147
+#: packages/console-extension/src/index.ts:724 packages/console-extension/src/index.ts:801 packages/console-extension/src/index.ts:804 packages/mainmenu-extension/src/index.ts:752 packages/mainmenu-extension/src/index.ts:754 packages/notebook-extension/src/index.ts:3147 packages/notebook-extension/src/index.ts:3154 packages/notebook-extension/src/index.ts:3177
 msgid "Get Kernel"
 msgstr "获取内核"
 
-#: packages/console-extension/src/index.ts:806
+#: packages/console-extension/src/index.ts:806 packages/console-extension/src/index.ts:893 packages/console-extension/src/index.ts:907
 msgid "Execute with Shift+Enter"
 msgstr "用 Shift+Enter 执行"
 
-#: packages/console-extension/src/index.ts:807
+#: packages/console-extension/src/index.ts:807 packages/console-extension/src/index.ts:894 packages/console-extension/src/index.ts:908
 msgid "Execute with Enter"
 msgstr "用 Enter 执行"
 
-#: packages/console-extension/src/index.ts:851 packages/fileeditor-extension/src/commands.ts:1012 packages/notebook-extension/src/index.ts:2027
+#: packages/console-extension/src/index.ts:851 packages/console-extension/src/index.ts:938 packages/console-extension/src/index.ts:952 packages/fileeditor-extension/src/commands.ts:1010 packages/fileeditor-extension/src/commands.ts:1012 packages/fileeditor-extension/src/commands.ts:1041 packages/notebook-extension/src/index.ts:2027 packages/notebook-extension/src/index.ts:2034 packages/notebook-extension/src/index.ts:2045
 msgid "Display the completion helper."
 msgstr "显示补全助手。"
 
-#: packages/console-extension/src/index.ts:862 packages/fileeditor-extension/src/commands.ts:1023 packages/notebook-extension/src/index.ts:2037
+#: packages/console-extension/src/index.ts:862 packages/console-extension/src/index.ts:949 packages/console-extension/src/index.ts:963 packages/fileeditor-extension/src/commands.ts:1021 packages/fileeditor-extension/src/commands.ts:1023 packages/fileeditor-extension/src/commands.ts:1052 packages/notebook-extension/src/index.ts:2037 packages/notebook-extension/src/index.ts:2044 packages/notebook-extension/src/index.ts:2055
 msgid "Select the completion suggestion."
 msgstr "选择补全建议。"
 
-#: packages/console/src/panel.ts:316
+#: packages/console/src/panel.ts:316 packages/console/src/panel.ts:324
 msgid "Name: %1\n"
 msgstr "名称：%1\n"
 
-#: packages/console/src/panel.ts:317
+#: packages/console/src/panel.ts:317 packages/console/src/panel.ts:325
 msgid "Directory: %1\n"
 msgstr "目录: %1\n"
 
-#: packages/console/src/panel.ts:318
+#: packages/console/src/panel.ts:318 packages/console/src/panel.ts:326
 msgid "Kernel: %1"
 msgstr "内核：%1"
 
-#: packages/console/src/panel.ts:321
+#: packages/console/src/panel.ts:321 packages/console/src/panel.ts:329
 msgid "\n"
 "Connected: %1"
 msgstr "\n"
 "已连接: %1"
 
-#: packages/console/src/panel.ts:328
+#: packages/console/src/panel.ts:328 packages/console/src/panel.ts:336
 msgid "\n"
 "Last Execution: %1"
 msgstr "\n"
 "上次执行: %1"
 
-#: packages/console/src/panel.ts:66
+#: packages/console/src/panel.ts:66 packages/console/src/panel.ts:68
 msgid "Console %1"
 msgstr "控制台 %1"
 
 #: packages/csvviewer-extension/src/index.ts:134
 msgid "CSV Viewer"
 msgstr "CSV 查看器"
 
-#: packages/csvviewer-extension/src/index.ts:216 packages/csvviewer-extension/src/index.ts:223 packages/csvviewer-extension/src/index.ts:370 packages/csvviewer-extension/src/index.ts:377
+#: packages/csvviewer-extension/src/index.ts:216 packages/csvviewer-extension/src/index.ts:223 packages/csvviewer-extension/src/index.ts:370 packages/csvviewer-extension/src/index.ts:376 packages/csvviewer-extension/src/index.ts:377 packages/csvviewer-extension/src/index.ts:383
 msgid "Go to Line"
 msgstr "跳转到行"
 
-#: packages/csvviewer-extension/src/index.ts:288
+#: packages/csvviewer-extension/src/index.ts:288 packages/csvviewer-extension/src/index.ts:294
 msgid "TSV Viewer"
 msgstr "TSV 查看器"
 
 #: packages/csvviewer/src/toolbar.ts:119
 msgid "tab"
 msgstr "标签页"
 
@@ -4303,14 +4401,18 @@
 
 #: packages/debugger/src/panels/kernelSources/body.tsx:88
 msgid "Fail to get '%1' source:\n"
 "%2"
 msgstr "无法获取「%1」源：\n"
 "%2"
 
+#: packages/debugger/src/panels/kernelSources/filter.tsx:33
+msgid "Filter the kernel sources"
+msgstr "筛选内核来源"
+
 #: packages/debugger/src/panels/kernelSources/index.tsx:33
 msgid "Kernel Sources"
 msgstr "内核源"
 
 #: packages/debugger/src/panels/kernelSources/index.tsx:49
 msgid "Toggle search filter"
 msgstr "切换搜索过滤器"
@@ -4325,15 +4427,15 @@
 msgstr "无法获取内核源：\n"
 "%2"
 
 #: packages/debugger/src/panels/kernelSources/index.tsx:66
 msgid "Refresh kernel sources"
 msgstr "刷新内核源"
 
-#: packages/debugger/src/panels/sources/index.tsx:29 packages/shortcuts-extension/src/components/TopNav.tsx:186
+#: packages/debugger/src/panels/sources/index.tsx:29 packages/shortcuts-extension/src/components/TopNav.tsx:134 packages/shortcuts-extension/src/components/TopNav.tsx:186
 msgid "Source"
 msgstr "源文件"
 
 #: packages/debugger/src/panels/sources/index.tsx:42
 msgid "Open in the Main Area"
 msgstr "在主区域打开"
 
@@ -4341,15 +4443,15 @@
 msgid "Type"
 msgstr "类型"
 
 #: packages/debugger/src/panels/variables/gridpanel.ts:218
 msgid "Value"
 msgstr "值"
 
-#: packages/debugger/src/panels/variables/gridpanel.ts:221 packages/filebrowser/src/listing.ts:2277
+#: packages/debugger/src/panels/variables/gridpanel.ts:221 packages/filebrowser/src/listing.ts:2277 packages/filebrowser/src/listing.ts:2298 packages/filebrowser/src/listing.ts:2371
 msgid "Name"
 msgstr "名称"
 
 #: packages/debugger/src/panels/variables/index.ts:33
 msgid "Variables"
 msgstr "变量"
 
@@ -4373,71 +4475,79 @@
 msgid "Render variable: %1"
 msgstr "渲染变量：%1"
 
 #: packages/debugger/src/service.ts:378
 msgid "Globals"
 msgstr "全局"
 
-#: packages/docmanager-extension/src/index.tsx:1007 packages/docmanager-extension/src/index.tsx:871 packages/docmanager-extension/src/index.tsx:889 packages/notebook/src/default-toolbar.tsx:68
+#: packages/docmanager-extension/src/index.tsx:1007 packages/docmanager-extension/src/index.tsx:1019 packages/docmanager-extension/src/index.tsx:871 packages/docmanager-extension/src/index.tsx:883 packages/docmanager-extension/src/index.tsx:889 packages/docmanager-extension/src/index.tsx:901 packages/notebook/src/default-toolbar.tsx:68
 msgid "Cannot Save"
 msgstr "无法保存"
 
-#: packages/docmanager-extension/src/index.tsx:1008 packages/docmanager-extension/src/index.tsx:485 packages/docmanager-extension/src/index.tsx:737 packages/docmanager-extension/src/index.tsx:782 packages/docmanager-extension/src/index.tsx:872
+#: packages/docmanager-extension/src/index.tsx:1008 packages/docmanager-extension/src/index.tsx:1020 packages/docmanager-extension/src/index.tsx:485 packages/docmanager-extension/src/index.tsx:495 packages/docmanager-extension/src/index.tsx:737 packages/docmanager-extension/src/index.tsx:749 packages/docmanager-extension/src/index.tsx:782 packages/docmanager-extension/src/index.tsx:794 packages/docmanager-extension/src/index.tsx:872 packages/docmanager-extension/src/index.tsx:884
 msgid "No context found for current widget!"
 msgstr "没有找到当前小组件的上下文！"
 
-#: packages/docmanager-extension/src/index.tsx:1039
+#: packages/docmanager-extension/src/index.tsx:1010 packages/docmanager-extension/src/index.tsx:998
+msgid "Save %1 As…"
+msgstr "将 %1 另存为…"
+
+#: packages/docmanager-extension/src/index.tsx:1011 packages/docmanager-extension/src/index.tsx:999
+msgid "Save with new path"
+msgstr "使用新路径保存"
+
+#: packages/docmanager-extension/src/index.tsx:1039 packages/docmanager-extension/src/index.tsx:1063
 msgid "Autosave Documents"
 msgstr "自动保存文档"
 
-#: packages/docmanager-extension/src/index.tsx:1100
+#: packages/docmanager-extension/src/index.tsx:1100 packages/docmanager-extension/src/index.tsx:1124
 msgid "New View for %1"
 msgstr "%1 新建视图"
 
-#: packages/docmanager-extension/src/index.tsx:1124
+#: packages/docmanager-extension/src/index.tsx:1124 packages/docmanager-extension/src/index.tsx:1148
 msgid "Rename%1…"
 msgstr "重命名%1…"
 
-#: packages/docmanager-extension/src/index.tsx:1138
+#: packages/docmanager-extension/src/index.tsx:1138 packages/docmanager-extension/src/index.tsx:1162
 msgid "Duplicate %1"
 msgstr "创建 %1 副本"
 
-#: packages/docmanager-extension/src/index.tsx:1153
+#: packages/docmanager-extension/src/index.tsx:1153 packages/docmanager-extension/src/index.tsx:1177 packages/workspaces-extension/src/sidebar.ts:99
 msgid "Delete %1"
 msgstr "删除 %1"
 
-#: packages/docmanager-extension/src/index.tsx:1163 packages/docmanager-extension/src/index.tsx:1167 packages/filebrowser-extension/src/index.ts:929 packages/filebrowser/src/listing.ts:430 packages/filebrowser/src/listing.ts:434
+#: packages/docmanager-extension/src/index.tsx:1163 packages/docmanager-extension/src/index.tsx:1167 packages/docmanager-extension/src/index.tsx:1187 packages/docmanager-extension/src/index.tsx:1191 packages/filebrowser-extension/src/index.ts:929 packages/filebrowser-extension/src/index.ts:937 packages/filebrowser/src/listing.ts:430 packages/filebrowser/src/listing.ts:433 packages/filebrowser/src/listing.ts:434 packages/filebrowser/src/listing.ts:437 packages/workspaces-extension/src/commands.ts:199
 msgid "Delete"
 msgstr "删除"
 
-#: packages/docmanager-extension/src/index.tsx:1164
+#: packages/docmanager-extension/src/index.tsx:1164 packages/docmanager-extension/src/index.tsx:1188
 msgid "Are you sure you want to delete %1"
 msgstr "您确定要删除 %1 吗？"
 
-#: packages/docmanager-extension/src/index.tsx:1181
+#: packages/docmanager-extension/src/index.tsx:1181 packages/docmanager-extension/src/index.tsx:1205
 msgid "Show in File Browser"
 msgstr "在文件浏览器中显示"
 
-#: packages/docmanager-extension/src/index.tsx:1247
+#: packages/docmanager-extension/src/index.tsx:1247 packages/docmanager-extension/src/index.tsx:1283
 msgid "Are you sure you want to revert the %1 to checkpoint? "
 msgstr "您确定要将 %1 还原到检查点吗？ "
 
-#: packages/docmanager-extension/src/index.tsx:1253
+#: packages/docmanager-extension/src/index.tsx:1253 packages/docmanager-extension/src/index.tsx:1289
 msgid "This cannot be undone."
 msgstr "此操作不可撤销。"
 
-#: packages/docmanager-extension/src/index.tsx:1260
+#: packages/docmanager-extension/src/index.tsx:1260 packages/docmanager-extension/src/index.tsx:1296
 msgid "The checkpoint was last updated at: "
 msgstr "检查点最后一次更新于: "
 
-#: packages/docmanager-extension/src/index.tsx:1294
+#: packages/docmanager-extension/src/index.tsx:1294 packages/docmanager-extension/src/index.tsx:1330
 msgid "Choose a checkpoint"
 msgstr "选择一个检查点"
 
-#: packages/docmanager-extension/src/index.tsx:345
+#: packages/docmanager-extension/src/index.tsx:345 packages/docmanager-extension/src/index.tsx:355
 msgid "Overrides for the default viewers for file types.\n"
 "Specify a mapping from file type name to document viewer name, for example:\n\n"
 "defaultViewers: {\n"
 "  markdown: \"Markdown Preview\"\n"
 "}\n\n"
 "If you specify non-existent file types or viewers, or if a viewer cannot\n"
 "open a given file type, the override will not function.\n\n"
@@ -4451,159 +4561,167 @@
 "}\n\n"
 "如果您指定了不存在的文件类型或查看器，或者如果查看器无法打开指定的文件类型，覆盖将不会生效。\n\n"
 "可用的查看器：\n"
 "%1\n\n"
 "可用的文件类型：\n"
 "%2"
 
-#: packages/docmanager-extension/src/index.tsx:475 packages/filebrowser-extension/src/index.ts:374
+#: packages/docmanager-extension/src/index.tsx:475 packages/docmanager-extension/src/index.tsx:485 packages/filebrowser-extension/src/index.ts:374 packages/filebrowser-extension/src/index.ts:405
 msgid "Download"
 msgstr "下载"
 
-#: packages/docmanager-extension/src/index.tsx:476
+#: packages/docmanager-extension/src/index.tsx:476 packages/docmanager-extension/src/index.tsx:486
 msgid "Download the file to your computer"
 msgstr "将文件下载到您的计算机"
 
-#: packages/docmanager-extension/src/index.tsx:484
+#: packages/docmanager-extension/src/index.tsx:484 packages/docmanager-extension/src/index.tsx:494
 msgid "Cannot Download"
 msgstr "无法下载"
 
-#: packages/docmanager-extension/src/index.tsx:494 packages/docmanager-extension/src/index.tsx:635 packages/filebrowser-extension/src/index.ts:1081 packages/filebrowser-extension/src/index.ts:573 packages/filebrowser-extension/src/index.ts:899 packages/htmlviewer-extension/src/index.tsx:206
+#: packages/docmanager-extension/src/index.tsx:494 packages/docmanager-extension/src/index.tsx:508 packages/docmanager-extension/src/index.tsx:635 packages/docmanager-extension/src/index.tsx:650 packages/filebrowser-extension/src/index.ts:1081 packages/filebrowser-extension/src/index.ts:1089 packages/filebrowser-extension/src/index.ts:573 packages/filebrowser-extension/src/index.ts:581 packages/filebrowser-extension/src/index.ts:899 packages/filebrowser-extension/src/index.ts:907 packages/htmlviewer-extension/src/index.tsx:206 packages/htmlviewer-extension/src/index.tsx:211
 msgid "File Operations"
 msgstr "文件操作"
 
-#: packages/docmanager-extension/src/index.tsx:543 packages/filebrowser-extension/src/index.ts:779
+#: packages/docmanager-extension/src/index.tsx:543 packages/docmanager-extension/src/index.tsx:557 packages/filebrowser-extension/src/index.ts:779 packages/filebrowser-extension/src/index.ts:787
 msgid "Open in New Browser Tab"
 msgstr "在新的浏览器标签页中打开"
 
 #: packages/docmanager-extension/src/index.tsx:652
 msgid "%1 is permissioned as read-only. Use \"save as...\" instead."
 msgstr "只有 %1 的只读权限。请改用“另存为...”功能。"
 
-#: packages/docmanager-extension/src/index.tsx:681 packages/filebrowser/src/browser.ts:261 packages/logconsole-extension/src/index.tsx:376
+#: packages/docmanager-extension/src/index.tsx:667
+msgid "%1 is read-only. Use \"Save as…\" instead."
+msgstr "%1 是只读的。请改用\"另存为...\"。"
+
+#: packages/docmanager-extension/src/index.tsx:681 packages/docmanager-extension/src/index.tsx:693 packages/filebrowser/src/browser.ts:261 packages/filebrowser/src/browser.ts:267 packages/logconsole-extension/src/index.tsx:376
 msgid "Error"
 msgstr "错误"
 
-#: packages/docmanager-extension/src/index.tsx:715
+#: packages/docmanager-extension/src/index.tsx:715 packages/docmanager-extension/src/index.tsx:727
 msgid "Open the provided `path`."
 msgstr "打开提供的`路径`。"
 
-#: packages/docmanager-extension/src/index.tsx:721 packages/docmanager-extension/src/index.tsx:743
+#: packages/docmanager-extension/src/index.tsx:721 packages/docmanager-extension/src/index.tsx:733 packages/docmanager-extension/src/index.tsx:743 packages/docmanager-extension/src/index.tsx:755
 msgid "Reload %1 from Disk"
 msgstr "从磁盘重新加载 %1"
 
-#: packages/docmanager-extension/src/index.tsx:725
+#: packages/docmanager-extension/src/index.tsx:725 packages/docmanager-extension/src/index.tsx:737
 msgid "Reload contents from disk"
 msgstr "从磁盘重新加载内容"
 
-#: packages/docmanager-extension/src/index.tsx:736
+#: packages/docmanager-extension/src/index.tsx:736 packages/docmanager-extension/src/index.tsx:748
 msgid "Cannot Reload"
 msgstr "无法重载"
 
-#: packages/docmanager-extension/src/index.tsx:744
+#: packages/docmanager-extension/src/index.tsx:744 packages/docmanager-extension/src/index.tsx:756
 msgid "Are you sure you want to reload the %1 from the disk?"
 msgstr "您确定要从磁盘重新加载 %1 吗？"
 
-#: packages/docmanager-extension/src/index.tsx:767
+#: packages/docmanager-extension/src/index.tsx:767 packages/docmanager-extension/src/index.tsx:779
 msgid "Revert %1 to Checkpoint…"
 msgstr "恢复 %1 到检查点…"
 
-#: packages/docmanager-extension/src/index.tsx:771
+#: packages/docmanager-extension/src/index.tsx:771 packages/docmanager-extension/src/index.tsx:783
 msgid "Revert contents to previous checkpoint"
 msgstr "撤回内容到之前的检查点"
 
-#: packages/docmanager-extension/src/index.tsx:781
+#: packages/docmanager-extension/src/index.tsx:781 packages/docmanager-extension/src/index.tsx:793
 msgid "Cannot Revert"
 msgstr "无法撤回"
 
-#: packages/docmanager-extension/src/index.tsx:790
+#: packages/docmanager-extension/src/index.tsx:790 packages/docmanager-extension/src/index.tsx:802
 msgid "No checkpoints"
 msgstr "无检查点"
 
-#: packages/docmanager-extension/src/index.tsx:791
+#: packages/docmanager-extension/src/index.tsx:791 packages/docmanager-extension/src/index.tsx:803
 msgid "No checkpoints are available for this %1."
 msgstr "%1 没有可用的检查站。"
 
-#: packages/docmanager-extension/src/index.tsx:804
+#: packages/docmanager-extension/src/index.tsx:804 packages/docmanager-extension/src/index.tsx:816
 msgid "Revert %1 to checkpoint"
 msgstr "将 %1 撤回至检查点"
 
-#: packages/docmanager-extension/src/index.tsx:809 packages/docregistry/src/context.ts:827
+#: packages/docmanager-extension/src/index.tsx:809 packages/docmanager-extension/src/index.tsx:821 packages/docregistry/src/context.ts:825 packages/docregistry/src/context.ts:827
 msgid "Revert"
 msgstr "撤回"
 
-#: packages/docmanager-extension/src/index.tsx:810
+#: packages/docmanager-extension/src/index.tsx:810 packages/docmanager-extension/src/index.tsx:822
 msgid "Revert to Checkpoint"
 msgstr "恢复到检查点"
 
-#: packages/docmanager-extension/src/index.tsx:834
+#: packages/docmanager-extension/src/index.tsx:834 packages/docmanager-extension/src/index.tsx:846
 msgid "In collaborative mode, the document is saved automatically after every change"
 msgstr "在协作模式下，文档在每次更改后都自动保存"
 
 #: packages/docmanager-extension/src/index.tsx:839
 msgid "document is permissioned readonly; \"save\" is disabled, use \"save as...\" instead"
 msgstr "只有文档的只读权限，因此不能使用“保存”功能，请改用“另存为...”功能。"
 
-#: packages/docmanager-extension/src/index.tsx:845
+#: packages/docmanager-extension/src/index.tsx:845 packages/docmanager-extension/src/index.tsx:857
 msgid "Save and create checkpoint"
 msgstr "保存并创建检查点"
 
-#: packages/docmanager-extension/src/index.tsx:851
+#: packages/docmanager-extension/src/index.tsx:851 packages/docmanager-extension/src/index.tsx:863
 msgid "Save %1"
 msgstr "保存 %1"
 
-#: packages/docmanager-extension/src/index.tsx:890 packages/notebook/src/default-toolbar.tsx:69
+#: packages/docmanager-extension/src/index.tsx:851 packages/docregistry/src/components.tsx:25
+msgid "Document is read-only. \"Save\" is disabled; use \"Save as…\" instead"
+msgstr "文档是只读的。\"保存\"功能被禁用，请改用\"另存为...\"。"
+
+#: packages/docmanager-extension/src/index.tsx:890 packages/docmanager-extension/src/index.tsx:902 packages/notebook/src/default-toolbar.tsx:69
 msgid "Document is read-only"
 msgstr "文档为只读状态"
 
-#: packages/docmanager-extension/src/index.tsx:906
+#: packages/docmanager-extension/src/index.tsx:906 packages/docmanager-extension/src/index.tsx:918
 msgid "Rename file"
 msgstr "重命名文件"
 
-#: packages/docmanager-extension/src/index.tsx:907 packages/docmanager/src/dialogs.ts:58 packages/filebrowser-extension/src/index.ts:1204
+#: packages/docmanager-extension/src/index.tsx:907 packages/docmanager-extension/src/index.tsx:919 packages/docmanager/src/dialogs.ts:58 packages/filebrowser-extension/src/index.ts:1204 packages/filebrowser-extension/src/index.ts:1212 packages/workspaces-extension/src/commands.ts:285
 msgid "Rename"
 msgstr "重命名"
 
-#: packages/docmanager-extension/src/index.tsx:908
+#: packages/docmanager-extension/src/index.tsx:908 packages/docmanager-extension/src/index.tsx:920
 msgid "File name"
 msgstr "文件名"
 
-#: packages/docmanager-extension/src/index.tsx:912 packages/docmanager/src/widgetmanager.ts:420
+#: packages/docmanager-extension/src/index.tsx:912 packages/docmanager-extension/src/index.tsx:924 packages/docmanager/src/widgetmanager.ts:420 packages/docmanager/src/widgetmanager.ts:491
 msgid "Do not ask me again."
 msgstr "不再询问"
 
-#: packages/docmanager-extension/src/index.tsx:913
+#: packages/docmanager-extension/src/index.tsx:913 packages/docmanager-extension/src/index.tsx:925
 msgid "If checked, you will not be asked to rename future untitled files when saving them."
 msgstr "如果选中此项，之后保存无标题文件时不会被要求重命名。"
 
-#: packages/docmanager-extension/src/index.tsx:970
+#: packages/docmanager-extension/src/index.tsx:970 packages/docmanager-extension/src/index.tsx:982
 msgid "Save All"
 msgstr "保存全部"
 
-#: packages/docmanager-extension/src/index.tsx:971
+#: packages/docmanager-extension/src/index.tsx:971 packages/docmanager-extension/src/index.tsx:983
 msgid "Save all open documents"
 msgstr "保存全部打开的文档"
 
-#: packages/docmanager-extension/src/index.tsx:998
-msgid "Save %1 As…"
-msgstr "将 %1 另存为…"
-
-#: packages/docmanager-extension/src/index.tsx:999
-msgid "Save with new path"
-msgstr "使用新路径保存"
+#: packages/docmanager-extension/src/recents.ts:73
+msgid "Clear Recent Documents"
+msgstr "清除最近文档记录"
+
+#: packages/docmanager-extension/src/recents.ts:74
+msgid "Clear the list of recently opened items."
+msgstr "清除最近打开项目的列表。"
 
 #: packages/docmanager/src/dialogs.ts:117
 msgid "Overwrite file?"
 msgstr "覆盖文件？"
 
 #: packages/docmanager/src/dialogs.ts:118
 msgid "\"%1\" already exists, overwrite?"
 msgstr "文件「%1」已存在，是否覆盖？"
 
-#: packages/docmanager/src/dialogs.ts:122 packages/docregistry/src/context.ts:831 packages/docregistry/src/context.ts:867 packages/shortcuts-extension/src/components/ShortcutInput.tsx:495 packages/shortcuts-extension/src/components/ShortcutItem.tsx:231
+#: packages/docmanager/src/dialogs.ts:122 packages/docregistry/src/context.ts:829 packages/docregistry/src/context.ts:831 packages/docregistry/src/context.ts:865 packages/docregistry/src/context.ts:867 packages/shortcuts-extension/src/components/ShortcutInput.tsx:495 packages/shortcuts-extension/src/components/ShortcutInput.tsx:496 packages/shortcuts-extension/src/components/ShortcutItem.tsx:231 packages/shortcuts-extension/src/components/ShortcutItem.tsx:348
 msgid "Overwrite"
 msgstr "覆盖"
 
 #: packages/docmanager/src/dialogs.ts:123
 msgid "Overwrite Existing File"
 msgstr "覆盖现有文件"
 
@@ -4615,15 +4733,15 @@
 msgid "New Name"
 msgstr "新名称"
 
 #: packages/docmanager/src/dialogs.ts:52 packages/docmanager/src/dialogs.ts:59
 msgid "Rename File"
 msgstr "重命名文件"
 
-#: packages/docmanager/src/dialogs.ts:68 packages/filebrowser/src/listing.ts:1891
+#: packages/docmanager/src/dialogs.ts:68 packages/filebrowser/src/listing.ts:1891 packages/filebrowser/src/listing.ts:1912 packages/filebrowser/src/listing.ts:1964
 msgid "Rename Error"
 msgstr "重命名错误"
 
 #: packages/docmanager/src/dialogs.ts:70
 msgid "\"%1\" is not a valid name for a file. Names must have nonzero length, and cannot include \"/\", \"\\\", or \":\""
 msgstr "「%1」不是一个有效的文件名。文件名必须具有非零长度，且不包含「/」、「\\」或「:」"
 
@@ -4635,187 +4753,187 @@
 msgid "Saving started"
 msgstr "已开始保存"
 
 #: packages/docmanager/src/savingstatus.tsx:60
 msgid "Saving failed"
 msgstr "保存失败"
 
-#: packages/docmanager/src/widgetmanager.ts:296
+#: packages/docmanager/src/widgetmanager.ts:296 packages/docmanager/src/widgetmanager.ts:307
 msgid "Name: %1\n"
 "Path: %2\n"
 msgstr "名称: %1\n"
 "路径: %2\n"
 
-#: packages/docmanager/src/widgetmanager.ts:302
+#: packages/docmanager/src/widgetmanager.ts:302 packages/docmanager/src/widgetmanager.ts:313
 msgid "Read-only"
 msgstr "只读"
 
-#: packages/docmanager/src/widgetmanager.ts:305
+#: packages/docmanager/src/widgetmanager.ts:305 packages/docmanager/src/widgetmanager.ts:316
 msgid "Last Saved: %1\n"
 msgstr "上次保存: %1\n"
 
-#: packages/docmanager/src/widgetmanager.ts:306
+#: packages/docmanager/src/widgetmanager.ts:306 packages/docmanager/src/widgetmanager.ts:317
 msgid "Last Checkpoint: %1"
 msgstr "上一检查点: %1"
 
-#: packages/docmanager/src/widgetmanager.ts:397
+#: packages/docmanager/src/widgetmanager.ts:397 packages/docmanager/src/widgetmanager.ts:468
 msgid "Close and save"
 msgstr "关闭并保存"
 
-#: packages/docmanager/src/widgetmanager.ts:399
+#: packages/docmanager/src/widgetmanager.ts:399 packages/docmanager/src/widgetmanager.ts:470
 msgid "Close and save Document"
 msgstr "关闭并保存文档"
 
-#: packages/docmanager/src/widgetmanager.ts:400
+#: packages/docmanager/src/widgetmanager.ts:400 packages/docmanager/src/widgetmanager.ts:471
 msgid "Close Document"
 msgstr "关闭文档"
 
-#: packages/docmanager/src/widgetmanager.ts:408
+#: packages/docmanager/src/widgetmanager.ts:408 packages/docmanager/src/widgetmanager.ts:479
 msgid "Close without saving"
 msgstr "不保存并关闭"
 
-#: packages/docmanager/src/widgetmanager.ts:409
+#: packages/docmanager/src/widgetmanager.ts:409 packages/docmanager/src/widgetmanager.ts:480
 msgid "Close Document without saving"
 msgstr "不保存，直接关闭文档"
 
-#: packages/docmanager/src/widgetmanager.ts:415 packages/notebook/src/searchprovider.ts:522
+#: packages/docmanager/src/widgetmanager.ts:415 packages/docmanager/src/widgetmanager.ts:486 packages/notebook/src/searchprovider.ts:511 packages/notebook/src/searchprovider.ts:514 packages/notebook/src/searchprovider.ts:522
 msgid "Confirmation"
 msgstr "确认"
 
-#: packages/docmanager/src/widgetmanager.ts:416
+#: packages/docmanager/src/widgetmanager.ts:416 packages/docmanager/src/widgetmanager.ts:487
 msgid "Please confirm you want to close \"%1\"."
 msgstr "请确认您想要关闭“%1”。"
 
-#: packages/docmanager/src/widgetmanager.ts:421
+#: packages/docmanager/src/widgetmanager.ts:421 packages/docmanager/src/widgetmanager.ts:492
 msgid "If checked, no confirmation to close a document will be asked in the future."
 msgstr "如果选中此项，以后关闭文档不再要求确认。"
 
-#: packages/docmanager/src/widgetmanager.ts:443
+#: packages/docmanager/src/widgetmanager.ts:443 packages/docmanager/src/widgetmanager.ts:514
 msgid "Save as"
 msgstr "另存为"
 
-#: packages/docmanager/src/widgetmanager.ts:445
+#: packages/docmanager/src/widgetmanager.ts:445 packages/docmanager/src/widgetmanager.ts:516
 msgid "Save your work"
 msgstr "保存您的工作"
 
-#: packages/docmanager/src/widgetmanager.ts:446
+#: packages/docmanager/src/widgetmanager.ts:446 packages/docmanager/src/widgetmanager.ts:517
 msgid "Save changes in \"%1\" before closing?"
 msgstr "关闭前是否要保存对「%1」的修改？"
 
-#: packages/docmanager/src/widgetmanager.ts:450
+#: packages/docmanager/src/widgetmanager.ts:450 packages/docmanager/src/widgetmanager.ts:521
 msgid "Discard"
 msgstr "丢弃"
 
-#: packages/docmanager/src/widgetmanager.ts:451
+#: packages/docmanager/src/widgetmanager.ts:451 packages/docmanager/src/widgetmanager.ts:522
 msgid "Discard changes to file"
 msgstr "放弃对文件的更改"
 
 #: packages/docregistry/src/components.tsx:25
 msgid "Document is permissioned read-only; \"save\" is disabled, use \"save as...\" instead"
 msgstr "只有文档的只读权限，因此不能使用“保存”功能，请改用“另存为...”功能。"
 
 #: packages/docregistry/src/components.tsx:29
 msgid "%1 is read-only"
 msgstr "%1 是只读的"
 
-#: packages/docregistry/src/context.ts:1045
+#: packages/docregistry/src/context.ts:1043 packages/docregistry/src/context.ts:1045
 msgid "Save File As…"
 msgstr "文件另存为..."
 
-#: packages/docregistry/src/context.ts:616 packages/docregistry/src/context.ts:916
+#: packages/docregistry/src/context.ts:614 packages/docregistry/src/context.ts:616 packages/docregistry/src/context.ts:914 packages/docregistry/src/context.ts:916
 msgid "File Save Error for %1"
 msgstr "保存文件 %1 时出错"
 
-#: packages/docregistry/src/context.ts:681
+#: packages/docregistry/src/context.ts:679 packages/docregistry/src/context.ts:681
 msgid "File Load Error for %1"
 msgstr "加载文件 %1 时出错"
 
-#: packages/docregistry/src/context.ts:820
+#: packages/docregistry/src/context.ts:818 packages/docregistry/src/context.ts:820
 msgid "\"%1\" has changed on disk since the last time it was opened or saved.\n"
 "Do you want to overwrite the file on disk with the version open here,\n"
 "or load the version on disk (revert)?"
 msgstr "「%1」自上次打开或保存后在磁盘上已经改变。您想要用这里打开的版本覆盖磁盘上的文件， 还是加载磁盘上的版本（复原）？"
 
-#: packages/docregistry/src/context.ts:836
+#: packages/docregistry/src/context.ts:834 packages/docregistry/src/context.ts:836
 msgid "File Changed"
 msgstr "文件已更改"
 
-#: packages/docregistry/src/context.ts:862
+#: packages/docregistry/src/context.ts:860 packages/docregistry/src/context.ts:862
 msgid "\"%1\" already exists. Do you want to replace it?"
 msgstr "「%1」已经存在。您想要替换它么？"
 
-#: packages/docregistry/src/context.ts:871
+#: packages/docregistry/src/context.ts:869 packages/docregistry/src/context.ts:871
 msgid "File Overwrite?"
 msgstr "要覆盖文件吗？"
 
 #: packages/docregistry/src/mimedocument.ts:175 packages/docregistry/src/mimedocument.ts:71 packages/markdownviewer/src/widget.ts:211
 msgid "Renderer Failure: %1"
 msgstr "渲染失败：%1"
 
-#: packages/docregistry/src/registry.ts:1287
+#: packages/docregistry/src/registry.ts:1287 packages/docregistry/src/registry.ts:1297
 msgid "default"
 msgstr "默认"
 
-#: packages/docregistry/src/registry.ts:1310
+#: packages/docregistry/src/registry.ts:1310 packages/docregistry/src/registry.ts:1320
 msgid "Text"
 msgstr "文本"
 
-#: packages/docregistry/src/registry.ts:1333 packages/launcher/src/widget.tsx:115 packages/launcher/src/widget.tsx:120 packages/notebook-extension/src/index.ts:1243 packages/notebook-extension/src/index.ts:1955 packages/notebook-extension/src/index.ts:1991
+#: packages/docregistry/src/registry.ts:1333 packages/docregistry/src/registry.ts:1343 packages/launcher/src/widget.tsx:115 packages/launcher/src/widget.tsx:120 packages/notebook-extension/src/index.ts:1243 packages/notebook-extension/src/index.ts:1247 packages/notebook-extension/src/index.ts:1255 packages/notebook-extension/src/index.ts:1955 packages/notebook-extension/src/index.ts:1960 packages/notebook-extension/src/index.ts:1971 packages/notebook-extension/src/index.ts:1991 packages/notebook-extension/src/index.ts:1998 packages/notebook-extension/src/index.ts:2009
 msgid "Notebook"
 msgstr "笔记本"
 
-#: packages/docregistry/src/registry.ts:1358
+#: packages/docregistry/src/registry.ts:1358 packages/docregistry/src/registry.ts:1368
 msgid "Directory"
 msgstr "目录"
 
-#: packages/docregistry/src/registry.ts:1385 packages/fileeditor-extension/src/commands.ts:817
+#: packages/docregistry/src/registry.ts:1385 packages/docregistry/src/registry.ts:1395 packages/fileeditor-extension/src/commands.ts:817 packages/fileeditor-extension/src/commands.ts:818
 msgid "Markdown File"
 msgstr "Markdown 文件"
 
-#: packages/docregistry/src/registry.ts:1392
+#: packages/docregistry/src/registry.ts:1392 packages/docregistry/src/registry.ts:1402
 msgid "PDF File"
 msgstr "PDF文件"
 
-#: packages/docregistry/src/registry.ts:1399 packages/fileeditor-extension/src/index.ts:331
+#: packages/docregistry/src/registry.ts:1399 packages/docregistry/src/registry.ts:1409 packages/fileeditor-extension/src/index.ts:331
 msgid "Python File"
 msgstr "Python 文件"
 
-#: packages/docregistry/src/registry.ts:1406
+#: packages/docregistry/src/registry.ts:1406 packages/docregistry/src/registry.ts:1416
 msgid "JSON File"
 msgstr "JSON 文件"
 
-#: packages/docregistry/src/registry.ts:1413
+#: packages/docregistry/src/registry.ts:1413 packages/docregistry/src/registry.ts:1423
 msgid "JSONLines File"
 msgstr "JSONLines 文件"
 
-#: packages/docregistry/src/registry.ts:1424 packages/fileeditor-extension/src/index.ts:343
+#: packages/docregistry/src/registry.ts:1424 packages/docregistry/src/registry.ts:1434 packages/fileeditor-extension/src/index.ts:343
 msgid "Julia File"
 msgstr "Julia 文件"
 
-#: packages/docregistry/src/registry.ts:1431
+#: packages/docregistry/src/registry.ts:1431 packages/docregistry/src/registry.ts:1441
 msgid "CSV File"
 msgstr "CSV 文件"
 
-#: packages/docregistry/src/registry.ts:1438
+#: packages/docregistry/src/registry.ts:1438 packages/docregistry/src/registry.ts:1448
 msgid "TSV File"
 msgstr "TSV 文件"
 
-#: packages/docregistry/src/registry.ts:1445 packages/fileeditor-extension/src/index.ts:355
+#: packages/docregistry/src/registry.ts:1445 packages/docregistry/src/registry.ts:1455 packages/fileeditor-extension/src/index.ts:355
 msgid "R File"
 msgstr "R 文件"
 
-#: packages/docregistry/src/registry.ts:1452
+#: packages/docregistry/src/registry.ts:1452 packages/docregistry/src/registry.ts:1462
 msgid "YAML File"
 msgstr "YAML 文件"
 
-#: packages/docregistry/src/registry.ts:1459 packages/docregistry/src/registry.ts:1467 packages/docregistry/src/registry.ts:1475 packages/docregistry/src/registry.ts:1483 packages/docregistry/src/registry.ts:1491 packages/docregistry/src/registry.ts:1499 packages/docregistry/src/registry.ts:1507 packages/imageviewer-extension/src/index.ts:119
+#: packages/docregistry/src/registry.ts:1459 packages/docregistry/src/registry.ts:1467 packages/docregistry/src/registry.ts:1469 packages/docregistry/src/registry.ts:1475 packages/docregistry/src/registry.ts:1477 packages/docregistry/src/registry.ts:1483 packages/docregistry/src/registry.ts:1485 packages/docregistry/src/registry.ts:1491 packages/docregistry/src/registry.ts:1493 packages/docregistry/src/registry.ts:1499 packages/docregistry/src/registry.ts:1501 packages/docregistry/src/registry.ts:1507 packages/docregistry/src/registry.ts:1509 packages/docregistry/src/registry.ts:1517 packages/imageviewer-extension/src/index.ts:119
 msgid "Image"
 msgstr "图片"
 
-#: packages/documentsearch-extension/src/index.ts:326 packages/fileeditor-extension/src/commands.ts:526 packages/json-extension/src/component.tsx:78
+#: packages/documentsearch-extension/src/index.ts:326 packages/fileeditor-extension/src/commands.ts:526 packages/fileeditor-extension/src/commands.ts:527 packages/json-extension/src/component.tsx:78
 msgid "Find…"
 msgstr "查找…"
 
 #: packages/documentsearch-extension/src/index.ts:363
 msgid "Find and Replace…"
 msgstr "查找和替换…"
 
@@ -4855,30 +4973,42 @@
 msgid "Replace All"
 msgstr "替换全部"
 
 #: packages/documentsearch/src/searchview.tsx:313
 msgid "Previous Match"
 msgstr "上一个匹配"
 
-#: packages/documentsearch/src/searchview.tsx:324
+#: packages/documentsearch/src/searchview.tsx:324 packages/documentsearch/src/searchview.tsx:328
 msgid "Next Match"
 msgstr "下一个匹配"
 
-#: packages/documentsearch/src/searchview.tsx:374
+#: packages/documentsearch/src/searchview.tsx:374 packages/documentsearch/src/searchview.tsx:385
 msgid "Hide Search Filters"
 msgstr "隐藏搜索筛选器"
 
-#: packages/documentsearch/src/searchview.tsx:375
+#: packages/documentsearch/src/searchview.tsx:375 packages/documentsearch/src/searchview.tsx:386
 msgid "Show Search Filters"
 msgstr "显示搜索筛选器"
 
 #: packages/documentsearch/src/searchview.tsx:685
 msgid "Toggle Replace"
 msgstr "切换替换"
 
+#: packages/documentsearch/src/searchview.tsx:703
+msgid "Hide Replace"
+msgstr "隐藏替换"
+
+#: packages/documentsearch/src/searchview.tsx:704
+msgid "Show Replace"
+msgstr "显示替换"
+
+#: packages/documentsearch/src/searchview.tsx:753
+msgid "Close Search Box"
+msgstr "关闭搜索框"
+
 #: packages/extensionmanager-extension/src/index.ts:131 packages/extensionmanager-extension/src/index.ts:153 packages/extensionmanager-extension/src/index.ts:59
 msgid "Extension Manager"
 msgstr "插件管理器"
 
 #: packages/extensionmanager-extension/src/index.ts:141
 msgid "Enable Extension Manager"
 msgstr "启用扩展管理器"
@@ -5057,366 +5187,370 @@
 msgid "Version: %1"
 msgstr "版本: %1"
 
 #: packages/extensionmanager/src/widget.tsx:97
 msgid "%1 extension is not allowed anymore. Please uninstall it immediately or contact your administrator."
 msgstr "不再允许使用扩展 %1。请立即卸载它或联系您的管理员。"
 
-#: packages/filebrowser-extension/src/index.ts:1021
-msgid "Open from Path…"
-msgstr "从路径打开…"
-
-#: packages/filebrowser-extension/src/index.ts:1021 packages/filebrowser-extension/src/index.ts:1023 packages/filebrowser-extension/src/index.ts:844 packages/filebrowser-extension/src/index.ts:846
+#: packages/filebrowser-extension/src/index.ts:1021 packages/filebrowser-extension/src/index.ts:1023 packages/filebrowser-extension/src/index.ts:1029 packages/filebrowser-extension/src/index.ts:1031 packages/filebrowser-extension/src/index.ts:844 packages/filebrowser-extension/src/index.ts:846 packages/filebrowser-extension/src/index.ts:852 packages/filebrowser-extension/src/index.ts:854
 msgid "Open %1"
 msgstr "打开 %1"
 
-#: packages/filebrowser-extension/src/index.ts:1023
+#: packages/filebrowser-extension/src/index.ts:1021 packages/filebrowser-extension/src/index.ts:1029
+msgid "Open from Path…"
+msgstr "从路径打开…"
+
+#: packages/filebrowser-extension/src/index.ts:1023 packages/filebrowser-extension/src/index.ts:1031
 msgid "Open from path"
 msgstr "从路径打开"
 
-#: packages/filebrowser-extension/src/index.ts:1032
+#: packages/filebrowser-extension/src/index.ts:1032 packages/filebrowser-extension/src/index.ts:1040
 msgid "Path"
 msgstr "路径"
 
-#: packages/filebrowser-extension/src/index.ts:1034
+#: packages/filebrowser-extension/src/index.ts:1034 packages/filebrowser-extension/src/index.ts:1042
 msgid "Open Path"
 msgstr "打开路径"
 
-#: packages/filebrowser-extension/src/index.ts:1035 packages/filebrowser-extension/src/index.ts:1124 packages/filebrowser-extension/src/index.ts:856
+#: packages/filebrowser-extension/src/index.ts:1035 packages/filebrowser-extension/src/index.ts:1043 packages/filebrowser-extension/src/index.ts:1124 packages/filebrowser-extension/src/index.ts:1132 packages/filebrowser-extension/src/index.ts:856 packages/filebrowser-extension/src/index.ts:864
 msgid "Open"
 msgstr "打开"
 
-#: packages/filebrowser-extension/src/index.ts:1070
+#: packages/filebrowser-extension/src/index.ts:1070 packages/filebrowser-extension/src/index.ts:1078
 msgid "Could not find path: %1"
 msgstr "找不到路径 %1"
 
-#: packages/filebrowser-extension/src/index.ts:1072
+#: packages/filebrowser-extension/src/index.ts:1072 packages/filebrowser-extension/src/index.ts:1080
 msgid "Cannot open"
 msgstr "无法打开"
 
-#: packages/filebrowser-extension/src/index.ts:1137 packages/fileeditor-extension/src/commands.ts:981 packages/terminal-extension/src/index.ts:494
+#: packages/filebrowser-extension/src/index.ts:1137 packages/filebrowser-extension/src/index.ts:1145 packages/fileeditor-extension/src/commands.ts:979 packages/fileeditor-extension/src/commands.ts:980 packages/fileeditor-extension/src/commands.ts:981 packages/terminal-extension/src/index.ts:494
 msgid "Paste"
 msgstr "粘贴"
 
-#: packages/filebrowser-extension/src/index.ts:1150 packages/filebrowser/src/opendialog.ts:172
+#: packages/filebrowser-extension/src/index.ts:1150 packages/filebrowser-extension/src/index.ts:1158 packages/filebrowser/src/opendialog.ts:172 packages/filebrowser/src/opendialog.ts:184
 msgid "New Folder"
 msgstr "新建文件夹"
 
-#: packages/filebrowser-extension/src/index.ts:1162
+#: packages/filebrowser-extension/src/index.ts:1162 packages/filebrowser-extension/src/index.ts:1170
 msgid "New File"
 msgstr "新建文件"
 
-#: packages/filebrowser-extension/src/index.ts:1174 packages/fileeditor-extension/src/commands.ts:816
+#: packages/filebrowser-extension/src/index.ts:1174 packages/filebrowser-extension/src/index.ts:1182 packages/fileeditor-extension/src/commands.ts:816 packages/fileeditor-extension/src/commands.ts:817
 msgid "New Markdown File"
 msgstr "新建Markdown文件"
 
-#: packages/filebrowser-extension/src/index.ts:1186
+#: packages/filebrowser-extension/src/index.ts:1186 packages/filebrowser-extension/src/index.ts:1194
 msgid "Refresh the file browser."
 msgstr "刷新文件浏览器。"
 
-#: packages/filebrowser-extension/src/index.ts:1187 packages/filebrowser/src/opendialog.ts:187
+#: packages/filebrowser-extension/src/index.ts:1187 packages/filebrowser-extension/src/index.ts:1195 packages/filebrowser/src/opendialog.ts:187 packages/filebrowser/src/opendialog.ts:199
 msgid "Refresh File List"
 msgstr "刷新文件列表"
 
-#: packages/filebrowser-extension/src/index.ts:1235
+#: packages/filebrowser-extension/src/index.ts:1235 packages/filebrowser-extension/src/index.ts:1243
 msgid "Copy Path"
 msgstr "复制路径"
 
-#: packages/filebrowser-extension/src/index.ts:1247 packages/mainmenu-extension/src/index.ts:531 packages/notebook-extension/src/index.ts:2389 packages/running-extension/src/kernels.ts:118 packages/running-extension/src/kernels.ts:66
+#: packages/filebrowser-extension/src/index.ts:1247 packages/filebrowser-extension/src/index.ts:1255 packages/mainmenu-extension/src/index.ts:529 packages/mainmenu-extension/src/index.ts:531 packages/notebook-extension/src/index.ts:2389 packages/notebook-extension/src/index.ts:2396 packages/notebook-extension/src/index.ts:2407 packages/running-extension/src/kernels.ts:118 packages/running-extension/src/kernels.ts:66 packages/running-extension/src/kernels.tsx:139 packages/running-extension/src/kernels.tsx:86
 msgid "Shut Down Kernel"
 msgstr "关闭内核"
 
-#: packages/filebrowser-extension/src/index.ts:1251
+#: packages/filebrowser-extension/src/index.ts:1251 packages/filebrowser-extension/src/index.ts:1259
 msgid "Show Last Modified Column"
 msgstr "切换最后修改列"
 
-#: packages/filebrowser-extension/src/index.ts:1267
+#: packages/filebrowser-extension/src/index.ts:1267 packages/filebrowser-extension/src/index.ts:1275
 msgid "Show Full Path"
 msgstr "显示完整路径"
 
-#: packages/filebrowser-extension/src/index.ts:1283
+#: packages/filebrowser-extension/src/index.ts:1283 packages/filebrowser-extension/src/index.ts:1291
 msgid "Sort Notebooks Above Files"
 msgstr "将笔记本排序在文件之前。"
 
-#: packages/filebrowser-extension/src/index.ts:1299
+#: packages/filebrowser-extension/src/index.ts:1299 packages/filebrowser-extension/src/index.ts:1307
 msgid "Show File Size Column"
 msgstr "显示文件大小栏"
 
-#: packages/filebrowser-extension/src/index.ts:1315
+#: packages/filebrowser-extension/src/index.ts:1315 packages/filebrowser-extension/src/index.ts:1323
 msgid "Show Hidden Files"
 msgstr "显示隐藏文件"
 
-#: packages/filebrowser-extension/src/index.ts:1332
+#: packages/filebrowser-extension/src/index.ts:1332 packages/filebrowser-extension/src/index.ts:1340
 msgid "Show File Checkboxes"
 msgstr "显示文件复选框"
 
-#: packages/filebrowser-extension/src/index.ts:1348
+#: packages/filebrowser-extension/src/index.ts:1348 packages/filebrowser-extension/src/index.ts:1356
 msgid "Search on File Names"
 msgstr "搜索文件名"
 
-#: packages/filebrowser-extension/src/index.ts:1417
+#: packages/filebrowser-extension/src/index.ts:1417 packages/filebrowser-extension/src/index.ts:1425
 msgid "No browser for path"
 msgstr "路径没有浏览器"
 
-#: packages/filebrowser-extension/src/index.ts:396
-msgid "Copy Download Link"
-msgstr "复制下载链接"
-
-#: packages/filebrowser-extension/src/index.ts:439
+#: packages/filebrowser-extension/src/index.ts:340 packages/filebrowser-extension/src/index.ts:439
 msgid "File Browser Section"
 msgstr "文件浏览器部分"
 
-#: packages/filebrowser-extension/src/index.ts:450
+#: packages/filebrowser-extension/src/index.ts:342 packages/filebrowser-extension/src/index.ts:354 packages/filebrowser-extension/src/index.ts:452 packages/filebrowser-extension/src/index.ts:504 packages/filebrowser-extension/src/index.ts:512 packages/filebrowser/src/browser.ts:73 packages/filebrowser/src/browser.ts:74
+msgid "File Browser"
+msgstr "文件管理器"
+
+#: packages/filebrowser-extension/src/index.ts:352 packages/filebrowser-extension/src/index.ts:450
 msgid "File Browser (%1)"
 msgstr "文件浏览器 (%1)"
 
-#: packages/filebrowser-extension/src/index.ts:452 packages/filebrowser-extension/src/index.ts:504 packages/filebrowser/src/browser.ts:73
-msgid "File Browser"
-msgstr "文件管理器"
+#: packages/filebrowser-extension/src/index.ts:396 packages/filebrowser-extension/src/index.ts:427
+msgid "Copy Download Link"
+msgstr "复制下载链接"
 
-#: packages/filebrowser-extension/src/index.ts:482
+#: packages/filebrowser-extension/src/index.ts:482 packages/filebrowser-extension/src/index.ts:490
 msgid "Filter files by name"
 msgstr "按文件名过滤"
 
-#: packages/filebrowser-extension/src/index.ts:515
+#: packages/filebrowser-extension/src/index.ts:515 packages/filebrowser-extension/src/index.ts:523
 msgid "Open the file browser for the provided `path`."
 msgstr "打开文件浏览器，查看提供的 `路径`。"
 
-#: packages/filebrowser-extension/src/index.ts:547
+#: packages/filebrowser-extension/src/index.ts:547 packages/filebrowser-extension/src/index.ts:555
 msgid "Hide the file browser."
 msgstr "隐藏文件浏览器。"
 
-#: packages/filebrowser-extension/src/index.ts:557
+#: packages/filebrowser-extension/src/index.ts:557 packages/filebrowser-extension/src/index.ts:565
 msgid "Show Active File in File Browser"
 msgstr "在文件浏览器中显示活动文件"
 
-#: packages/filebrowser-extension/src/index.ts:654
+#: packages/filebrowser-extension/src/index.ts:654 packages/filebrowser-extension/src/index.ts:662
 msgid "Copy Shareable Link"
 msgstr "复制共享链接"
 
-#: packages/filebrowser-extension/src/index.ts:778
+#: packages/filebrowser-extension/src/index.ts:778 packages/filebrowser-extension/src/index.ts:786
 msgid "Open in Simple Mode"
 msgstr "以简易模式打开"
 
-#: packages/filebrowser-extension/src/index.ts:844
+#: packages/filebrowser-extension/src/index.ts:844 packages/filebrowser-extension/src/index.ts:852
 msgid "Open from URL…"
 msgstr "从 URL 打开…"
 
-#: packages/filebrowser-extension/src/index.ts:846
+#: packages/filebrowser-extension/src/index.ts:846 packages/filebrowser-extension/src/index.ts:854
 msgid "Open from URL"
 msgstr "从链接打开"
 
-#: packages/filebrowser-extension/src/index.ts:853
+#: packages/filebrowser-extension/src/index.ts:853 packages/filebrowser-extension/src/index.ts:861
 msgid "URL"
 msgstr "链接"
 
-#: packages/filebrowser-extension/src/index.ts:855
+#: packages/filebrowser-extension/src/index.ts:855 packages/filebrowser-extension/src/index.ts:863
 msgid "Open URL"
 msgstr "打开链接"
 
-#: packages/filebrowser-extension/src/index.ts:874
+#: packages/filebrowser-extension/src/index.ts:874 packages/filebrowser-extension/src/index.ts:882
 msgid "Could not open URL: %1"
 msgstr "无法打开 URL：%1"
 
-#: packages/filebrowser-extension/src/index.ts:876
+#: packages/filebrowser-extension/src/index.ts:876 packages/filebrowser-extension/src/index.ts:884
 msgid "Cannot fetch"
 msgstr "无法获取"
 
-#: packages/filebrowser-extension/src/index.ts:889 packages/filebrowser/src/upload.ts:52
+#: packages/filebrowser-extension/src/index.ts:889 packages/filebrowser-extension/src/index.ts:897 packages/filebrowser/src/upload.ts:52
 msgctxt "showErrorMessage"
 msgid "Upload Error"
 msgstr "上传错误"
 
-#: packages/filebrowser-extension/src/index.ts:942 packages/fileeditor-extension/src/commands.ts:954 packages/terminal-extension/src/index.ts:469
+#: packages/filebrowser-extension/src/index.ts:942 packages/filebrowser-extension/src/index.ts:950 packages/fileeditor-extension/src/commands.ts:952 packages/fileeditor-extension/src/commands.ts:953 packages/fileeditor-extension/src/commands.ts:954 packages/terminal-extension/src/index.ts:469
 msgid "Copy"
 msgstr "复制"
 
-#: packages/filebrowser-extension/src/index.ts:955 packages/fileeditor-extension/src/commands.ts:920
+#: packages/filebrowser-extension/src/index.ts:955 packages/filebrowser-extension/src/index.ts:963 packages/fileeditor-extension/src/commands.ts:918 packages/fileeditor-extension/src/commands.ts:919 packages/fileeditor-extension/src/commands.ts:920
 msgid "Cut"
 msgstr "剪切"
 
-#: packages/filebrowser-extension/src/index.ts:967
+#: packages/filebrowser-extension/src/index.ts:967 packages/filebrowser-extension/src/index.ts:975
 msgid "Duplicate"
 msgstr "创建副本"
 
-#: packages/filebrowser-extension/src/index.ts:971
+#: packages/filebrowser-extension/src/index.ts:971 packages/filebrowser-extension/src/index.ts:979
 msgid "Update the file browser to display the provided `path`."
 msgstr "更新文件浏览器以显示提供的 `路径`。"
 
-#: packages/filebrowser/src/browser.ts:397
+#: packages/filebrowser/src/browser.ts:397 packages/filebrowser/src/browser.ts:403
 msgid "Directory not found"
 msgstr "找不到目录"
 
-#: packages/filebrowser/src/browser.ts:398 packages/filebrowser/src/model.ts:298
+#: packages/filebrowser/src/browser.ts:398 packages/filebrowser/src/browser.ts:404 packages/filebrowser/src/model.ts:291 packages/filebrowser/src/model.ts:298
 msgid "Directory not found: \"%1\""
 msgstr "找不到目录：「%1」"
 
-#: packages/filebrowser/src/browser.ts:67
+#: packages/filebrowser/src/browser.ts:67 packages/filebrowser/src/browser.ts:68
 msgid "file browser"
 msgstr "文件浏览器"
 
 #: packages/filebrowser/src/crumbs.ts:192 packages/filebrowser/src/crumbs.ts:219
 msgid "Open Error"
 msgstr "打开出错"
 
 #: packages/filebrowser/src/crumbs.ts:327
 msgid "Move Error"
 msgstr "移动出错"
 
-#: packages/filebrowser/src/listing.ts:1136
+#: packages/filebrowser/src/listing.ts:1136 packages/filebrowser/src/listing.ts:1157 packages/filebrowser/src/listing.ts:1209
 msgctxt "showErrorMessage"
 msgid "Open directory"
 msgstr "打开目录"
 
-#: packages/filebrowser/src/listing.ts:1411
+#: packages/filebrowser/src/listing.ts:1411 packages/filebrowser/src/listing.ts:1432 packages/filebrowser/src/listing.ts:1484
 msgid "Error Uploading Folder"
 msgstr "上传文件夹时出错"
 
-#: packages/filebrowser/src/listing.ts:1412
+#: packages/filebrowser/src/listing.ts:1412 packages/filebrowser/src/listing.ts:1433 packages/filebrowser/src/listing.ts:1485
 msgid "Drag and Drop is currently not supported for folders"
 msgstr "文件夹目前不支持拖放。"
 
-#: packages/filebrowser/src/listing.ts:1531
+#: packages/filebrowser/src/listing.ts:1531 packages/filebrowser/src/listing.ts:1552 packages/filebrowser/src/listing.ts:1604
 msgctxt "showErrorMessage"
 msgid "Error while copying/moving files"
 msgstr "复制或移动文件时出错"
 
-#: packages/filebrowser/src/listing.ts:1830
+#: packages/filebrowser/src/listing.ts:1830 packages/filebrowser/src/listing.ts:1851 packages/filebrowser/src/listing.ts:1903
 msgctxt "showErrorMessage"
 msgid "Delete Failed"
 msgstr "删除失败"
 
-#: packages/filebrowser/src/listing.ts:1893
+#: packages/filebrowser/src/listing.ts:1893 packages/filebrowser/src/listing.ts:1914 packages/filebrowser/src/listing.ts:1966
 msgctxt "showErrorMessage"
 msgid "\"%1\" is not a valid name for a file. Names must have nonzero length, and cannot include \"/\", \"\\\", or \":\""
 msgstr "「%1」不是一个有效的文件名。文件名必须具有非零长度，且不包含「/」、「\\」或「:」"
 
-#: packages/filebrowser/src/listing.ts:1912
+#: packages/filebrowser/src/listing.ts:1912 packages/filebrowser/src/listing.ts:1933 packages/filebrowser/src/listing.ts:1985
 msgctxt "showErrorMessage"
 msgid "Rename Error"
 msgstr "重命名错误"
 
-#: packages/filebrowser/src/listing.ts:2279
+#: packages/filebrowser/src/listing.ts:2279 packages/filebrowser/src/listing.ts:2300 packages/filebrowser/src/listing.ts:2375
 msgid "Last Modified"
 msgstr "修改时间"
 
-#: packages/filebrowser/src/listing.ts:2280
+#: packages/filebrowser/src/listing.ts:2280 packages/filebrowser/src/listing.ts:2301 packages/filebrowser/src/listing.ts:2377
 msgid "File Size"
 msgstr "文件大小"
 
-#: packages/filebrowser/src/listing.ts:2568
+#: packages/filebrowser/src/listing.ts:2374 packages/settingeditor/src/pluginlist.tsx:461
+msgid "Modified"
+msgstr "已修改"
+
+#: packages/filebrowser/src/listing.ts:2568 packages/filebrowser/src/listing.ts:2589 packages/filebrowser/src/listing.ts:2696
 msgid "Name: %1"
 msgstr "名称：%1"
 
-#: packages/filebrowser/src/listing.ts:2574
+#: packages/filebrowser/src/listing.ts:2574 packages/filebrowser/src/listing.ts:2595 packages/filebrowser/src/listing.ts:2702
 msgid "\n"
 "Size: %1"
 msgstr "\n"
 "大小: %1"
 
-#: packages/filebrowser/src/listing.ts:2584
+#: packages/filebrowser/src/listing.ts:2584 packages/filebrowser/src/listing.ts:2605 packages/filebrowser/src/listing.ts:2712
 msgid "\n"
 "Path: %1"
 msgstr "\n"
 "路径: %1"
 
-#: packages/filebrowser/src/listing.ts:2591
+#: packages/filebrowser/src/listing.ts:2591 packages/filebrowser/src/listing.ts:2612 packages/filebrowser/src/listing.ts:2719
 msgid "\n"
 "Created: %1"
 msgstr "\n"
 "创建时间：%1"
 
-#: packages/filebrowser/src/listing.ts:2597
+#: packages/filebrowser/src/listing.ts:2597 packages/filebrowser/src/listing.ts:2618 packages/filebrowser/src/listing.ts:2725
 msgid "\n"
 "Modified: %1"
 msgstr "\n"
 "修改时间：%1"
 
-#: packages/filebrowser/src/listing.ts:2602
+#: packages/filebrowser/src/listing.ts:2602 packages/filebrowser/src/listing.ts:2623 packages/filebrowser/src/listing.ts:2730
 msgid "\n"
 "Writable: %1"
 msgstr "\n"
 "可写：%1"
 
-#: packages/filebrowser/src/listing.ts:2627
+#: packages/filebrowser/src/listing.ts:2627 packages/filebrowser/src/listing.ts:2648 packages/filebrowser/src/listing.ts:2755
 msgid "Deselect directory \"%1\""
 msgstr "取消选择目录“%1”"
 
-#: packages/filebrowser/src/listing.ts:2628
+#: packages/filebrowser/src/listing.ts:2628 packages/filebrowser/src/listing.ts:2649 packages/filebrowser/src/listing.ts:2756
 msgid "Select directory \"%1\""
 msgstr "选择目录“%1”"
 
-#: packages/filebrowser/src/listing.ts:2631
+#: packages/filebrowser/src/listing.ts:2631 packages/filebrowser/src/listing.ts:2652 packages/filebrowser/src/listing.ts:2759
 msgid "Deselect file \"%1\""
 msgstr "取消选择文件 \"%1\""
 
-#: packages/filebrowser/src/listing.ts:2632
+#: packages/filebrowser/src/listing.ts:2632 packages/filebrowser/src/listing.ts:2653 packages/filebrowser/src/listing.ts:2760
 msgid "Select file \"%1\""
 msgstr "选择文件 \"%1\""
 
-#: packages/filebrowser/src/listing.ts:2706
+#: packages/filebrowser/src/listing.ts:2706 packages/filebrowser/src/listing.ts:2727 packages/filebrowser/src/listing.ts:2833
 msgid "%1 Item"
 msgid_plural "%1 Items"
 msgstr[0] "%1 项"
 
-#: packages/filebrowser/src/listing.ts:400
+#: packages/filebrowser/src/listing.ts:400 packages/filebrowser/src/listing.ts:403
 msgctxt "showErrorMessage"
 msgid "Paste Error"
 msgstr "粘贴出错"
 
-#: packages/filebrowser/src/listing.ts:420
+#: packages/filebrowser/src/listing.ts:420 packages/filebrowser/src/listing.ts:423
 msgid "Are you sure you want to permanently delete: %1?"
 msgstr "您确定要删除「%1」吗？"
 
-#: packages/filebrowser/src/listing.ts:424
+#: packages/filebrowser/src/listing.ts:424 packages/filebrowser/src/listing.ts:427
 msgid "Are you sure you want to permanently delete the %1 selected item?"
 msgid_plural "Are you sure you want to permanently delete the %1 selected items?"
 msgstr[0] "您确实要永久删除 %1 个选定的项目吗？"
 
-#: packages/filebrowser/src/listing.ts:476
+#: packages/filebrowser/src/listing.ts:476 packages/filebrowser/src/listing.ts:479
 msgctxt "showErrorMessage"
 msgid "Duplicate file"
 msgstr "重复的文件"
 
-#: packages/filebrowser/src/listing.ts:516
+#: packages/filebrowser/src/listing.ts:516 packages/filebrowser/src/listing.ts:519
 msgctxt "showErrorMessage"
 msgid "Shut down kernel"
 msgstr "终止内核"
 
-#: packages/filebrowser/src/listing.ts:856
+#: packages/filebrowser/src/listing.ts:856 packages/filebrowser/src/listing.ts:877 packages/filebrowser/src/listing.ts:974
 msgid "Deselect all files and directories"
 msgstr "取消选择全部文件和目录"
 
-#: packages/filebrowser/src/listing.ts:857
+#: packages/filebrowser/src/listing.ts:857 packages/filebrowser/src/listing.ts:878 packages/filebrowser/src/listing.ts:975
 msgid "Select all files and directories"
 msgstr "选择全部文件和目录"
 
-#: packages/filebrowser/src/listing.ts:910
+#: packages/filebrowser/src/listing.ts:899 packages/filebrowser/src/listing.ts:910 packages/filebrowser/src/listing.ts:931
 msgid "unknown"
 msgstr "未知"
 
-#: packages/filebrowser/src/listing.ts:912
+#: packages/filebrowser/src/listing.ts:901 packages/filebrowser/src/listing.ts:912 packages/filebrowser/src/listing.ts:933
 msgid "%1\n"
 "Kernel: %2"
 msgstr "%1\n"
 "内核：%2"
 
-#: packages/filebrowser/src/model.ts:414
+#: packages/filebrowser/src/model.ts:407 packages/filebrowser/src/model.ts:414
 msgid "Cannot upload file (>%1 MB). %2"
 msgstr "无法上传文件（大于 %1 MB）。%2"
 
-#: packages/filebrowser/src/model.ts:443
+#: packages/filebrowser/src/model.ts:436 packages/filebrowser/src/model.ts:443
 msgid "Large file size warning"
 msgstr "大型文件警告"
 
-#: packages/filebrowser/src/model.ts:444
+#: packages/filebrowser/src/model.ts:437 packages/filebrowser/src/model.ts:444
 msgid "The file size is %1 MB. Do you still want to upload it?"
 msgstr "文件大小是 %1 MB。您仍然想要上传它吗？"
 
-#: packages/filebrowser/src/model.ts:450
+#: packages/filebrowser/src/model.ts:443 packages/filebrowser/src/model.ts:450
 msgid "Upload"
 msgstr "上传"
 
 #: packages/filebrowser/src/model.ts:83
 msgid "Files still uploading"
 msgstr "文件还在上传"
 
@@ -5428,140 +5562,132 @@
 msgid "Uploading…"
 msgstr "正在上传…"
 
 #: packages/filebrowser/src/uploadstatus.tsx:96
 msgid "Complete!"
 msgstr "完成！"
 
-#: packages/fileeditor-extension/src/commands.ts:1107 packages/fileeditor-extension/src/commands.ts:1121 packages/fileeditor-extension/src/commands.ts:1137 packages/launcher/src/widget.tsx:117 packages/launcher/src/widget.tsx:127 packages/launcher/src/widget.tsx:296 packages/terminal-extension/src/index.ts:271
+#: packages/fileeditor-extension/src/commands.ts:1105 packages/fileeditor-extension/src/commands.ts:1107 packages/fileeditor-extension/src/commands.ts:1119 packages/fileeditor-extension/src/commands.ts:1121 packages/fileeditor-extension/src/commands.ts:1135 packages/fileeditor-extension/src/commands.ts:1136 packages/fileeditor-extension/src/commands.ts:1137 packages/fileeditor-extension/src/commands.ts:1150 packages/fileeditor-extension/src/commands.ts:1166 packages/launcher/src/widget.tsx:117 packages/launcher/src/widget.tsx:127 packages/launcher/src/widget.tsx:296 packages/terminal-extension/src/index.ts:271
 msgid "Other"
 msgstr "其他"
 
-#: packages/fileeditor-extension/src/commands.ts:1167 packages/fileeditor-extension/src/commands.ts:1189 packages/fileeditor-extension/src/commands.ts:1204 packages/fileeditor-extension/src/commands.ts:1219 packages/fileeditor-extension/src/commands.ts:1237
+#: packages/fileeditor-extension/src/commands.ts:1165 packages/fileeditor-extension/src/commands.ts:1167 packages/fileeditor-extension/src/commands.ts:1187 packages/fileeditor-extension/src/commands.ts:1189 packages/fileeditor-extension/src/commands.ts:1196 packages/fileeditor-extension/src/commands.ts:1202 packages/fileeditor-extension/src/commands.ts:1204 packages/fileeditor-extension/src/commands.ts:1217 packages/fileeditor-extension/src/commands.ts:1218 packages/fileeditor-extension/src/commands.ts:1219 packages/fileeditor-extension/src/commands.ts:1233 packages/fileeditor-extension/src/commands.ts:1235 packages/fileeditor-extension/src/commands.ts:1237 packages/fileeditor-extension/src/commands.ts:1248 packages/fileeditor-extension/src/commands.ts:1266
 msgid "Text Editor"
 msgstr "文本编辑器"
 
-#: packages/fileeditor-extension/src/commands.ts:1367
+#: packages/fileeditor-extension/src/commands.ts:1365 packages/fileeditor-extension/src/commands.ts:1367 packages/fileeditor-extension/src/commands.ts:1396
 msgid "Code Viewer"
 msgstr "代码查看器"
 
-#: packages/fileeditor-extension/src/commands.ts:1386
+#: packages/fileeditor-extension/src/commands.ts:1384 packages/fileeditor-extension/src/commands.ts:1386 packages/fileeditor-extension/src/commands.ts:1415
 msgid "Open Code Viewer"
 msgstr "打开代码查看器"
 
-#: packages/fileeditor-extension/src/commands.ts:280
+#: packages/fileeditor-extension/src/commands.ts:280 packages/fileeditor-extension/src/commands.ts:281
 msgid "Increase Text Editor Font Size"
 msgstr "增加文本编辑器字体大小"
 
-#: packages/fileeditor-extension/src/commands.ts:284
+#: packages/fileeditor-extension/src/commands.ts:284 packages/fileeditor-extension/src/commands.ts:285
 msgid "Decrease Text Editor Font Size"
 msgstr "减小文本编辑器字体大小"
 
-#: packages/fileeditor-extension/src/commands.ts:307 packages/fileeditor-extension/src/commands.ts:311 packages/mainmenu-extension/src/index.ts:576 packages/notebook-extension/src/index.ts:3040
+#: packages/fileeditor-extension/src/commands.ts:307 packages/fileeditor-extension/src/commands.ts:308 packages/fileeditor-extension/src/commands.ts:311 packages/fileeditor-extension/src/commands.ts:312 packages/mainmenu-extension/src/index.ts:573 packages/mainmenu-extension/src/index.ts:576 packages/notebook-extension/src/index.ts:3040 packages/notebook-extension/src/index.ts:3047 packages/notebook-extension/src/index.ts:3070
 msgid "Show Line Numbers"
 msgstr "显示行号"
 
-#: packages/fileeditor-extension/src/commands.ts:312
+#: packages/fileeditor-extension/src/commands.ts:312 packages/fileeditor-extension/src/commands.ts:313
 msgid "Show the line numbers for the current file."
 msgstr "显示当前文件的行号。"
 
-#: packages/fileeditor-extension/src/commands.ts:352
+#: packages/fileeditor-extension/src/commands.ts:352 packages/fileeditor-extension/src/commands.ts:353
 msgid "Word Wrap"
 msgstr "换行"
 
-#: packages/fileeditor-extension/src/commands.ts:356 packages/mainmenu-extension/src/index.ts:600
+#: packages/fileeditor-extension/src/commands.ts:356 packages/fileeditor-extension/src/commands.ts:357 packages/mainmenu-extension/src/index.ts:595 packages/mainmenu-extension/src/index.ts:600
 msgid "Wrap Words"
 msgstr "换行"
 
-#: packages/fileeditor-extension/src/commands.ts:357
+#: packages/fileeditor-extension/src/commands.ts:357 packages/fileeditor-extension/src/commands.ts:358
 msgid "Wrap words for the current file."
 msgstr "将当前文件中的单词换行。"
 
-#: packages/fileeditor-extension/src/commands.ts:383 packages/fileeditor-extension/src/index.ts:147
+#: packages/fileeditor-extension/src/commands.ts:383 packages/fileeditor-extension/src/commands.ts:384 packages/fileeditor-extension/src/index.ts:147
 msgctxt "v4"
 msgid "Spaces: %1"
 msgstr "空格：%1"
 
-#: packages/fileeditor-extension/src/commands.ts:385 packages/fileeditor-extension/src/index.ts:140
+#: packages/fileeditor-extension/src/commands.ts:385 packages/fileeditor-extension/src/commands.ts:386 packages/fileeditor-extension/src/index.ts:140
 msgid "Indent with Tab"
 msgstr "使用 Tab 缩进"
 
-#: packages/fileeditor-extension/src/commands.ts:430
+#: packages/fileeditor-extension/src/commands.ts:430 packages/fileeditor-extension/src/commands.ts:431
 msgid "Change match brackets for the current file."
 msgstr "更改当前文件的匹配括号。"
 
-#: packages/fileeditor-extension/src/commands.ts:468
+#: packages/fileeditor-extension/src/commands.ts:468 packages/fileeditor-extension/src/commands.ts:469
 msgid "Auto Close Brackets in Text Editor"
 msgstr "在文本编辑器中自动关闭括号"
 
-#: packages/fileeditor-extension/src/commands.ts:496
+#: packages/fileeditor-extension/src/commands.ts:496 packages/fileeditor-extension/src/commands.ts:497
 msgid "Auto Close Brackets"
 msgstr "自动关闭启动器"
 
-#: packages/fileeditor-extension/src/commands.ts:511
+#: packages/fileeditor-extension/src/commands.ts:511 packages/fileeditor-extension/src/commands.ts:512
 msgid "Editor Theme"
 msgstr "编辑器主题"
 
-#: packages/fileeditor-extension/src/commands.ts:539 packages/mainmenu-extension/src/index.ts:324
+#: packages/fileeditor-extension/src/commands.ts:539 packages/fileeditor-extension/src/commands.ts:540 packages/mainmenu-extension/src/index.ts:320 packages/mainmenu-extension/src/index.ts:324
 msgid "Go to Line…"
 msgstr "跳至行..."
 
-#: packages/fileeditor-extension/src/commands.ts:564
+#: packages/fileeditor-extension/src/commands.ts:564 packages/fileeditor-extension/src/commands.ts:565
 msgid "Change editor language."
 msgstr "更改编辑器语言。"
 
-#: packages/fileeditor-extension/src/commands.ts:608
+#: packages/fileeditor-extension/src/commands.ts:608 packages/fileeditor-extension/src/commands.ts:609
 msgid "Replace Selection in Editor"
 msgstr "在编辑器中替换选择"
 
-#: packages/fileeditor-extension/src/commands.ts:626
+#: packages/fileeditor-extension/src/commands.ts:626 packages/fileeditor-extension/src/commands.ts:627
 msgid "Create Console for Editor"
 msgstr "为编辑器创建控制台"
 
-#: packages/fileeditor-extension/src/commands.ts:647
+#: packages/fileeditor-extension/src/commands.ts:647 packages/fileeditor-extension/src/commands.ts:648
 msgid "Restart Kernel"
 msgstr "重启内核"
 
-#: packages/fileeditor-extension/src/commands.ts:712
+#: packages/fileeditor-extension/src/commands.ts:712 packages/fileeditor-extension/src/commands.ts:713
 msgid "Run Selected Code"
 msgstr "运行选中的代码"
 
-#: packages/fileeditor-extension/src/commands.ts:750
+#: packages/fileeditor-extension/src/commands.ts:750 packages/fileeditor-extension/src/commands.ts:751
 msgid "Run All Code"
 msgstr "运行全部代码"
 
-#: packages/fileeditor-extension/src/commands.ts:777
+#: packages/fileeditor-extension/src/commands.ts:777 packages/fileeditor-extension/src/commands.ts:778
 msgid "Show Markdown Preview"
 msgstr "显示 Markdown 预览"
 
-#: packages/fileeditor-extension/src/commands.ts:788
+#: packages/fileeditor-extension/src/commands.ts:788 packages/fileeditor-extension/src/commands.ts:789
 msgid "New Text File"
 msgstr "新建文本文件"
 
-#: packages/fileeditor-extension/src/commands.ts:790
+#: packages/fileeditor-extension/src/commands.ts:790 packages/fileeditor-extension/src/commands.ts:791
 msgid "Text File"
 msgstr "文本文件"
 
-#: packages/fileeditor-extension/src/commands.ts:793
+#: packages/fileeditor-extension/src/commands.ts:793 packages/fileeditor-extension/src/commands.ts:794
 msgid "Create a new text file"
 msgstr "新建一个文本文件"
 
-#: packages/fileeditor-extension/src/commands.ts:818
+#: packages/fileeditor-extension/src/commands.ts:818 packages/fileeditor-extension/src/commands.ts:819
 msgid "Create a new markdown file"
 msgstr "新建一个 Markdown 文件"
 
-#: packages/fileeditor-extension/src/commands.ts:854 packages/mainmenu-extension/src/index.ts:277 packages/notebook-extension/src/index.ts:3122
-msgid "Undo"
-msgstr "撤消"
-
-#: packages/fileeditor-extension/src/commands.ts:885 packages/mainmenu-extension/src/index.ts:288 packages/notebook-extension/src/index.ts:3108
-msgid "Redo"
-msgstr "重做"
-
-#: packages/fileeditor-extension/src/commands.ts:999
+#: packages/fileeditor-extension/src/commands.ts:997 packages/fileeditor-extension/src/commands.ts:998 packages/fileeditor-extension/src/commands.ts:999
 msgid "Select All"
 msgstr "全选"
 
 #: packages/fileeditor-extension/src/index.ts:309
 msgid "Editor"
 msgstr "编辑器"
 
@@ -5774,15 +5900,15 @@
 msgid "Hub Control Panel"
 msgstr "Hub 控制面板"
 
 #: packages/hub-extension/src/index.ts:83
 msgid "Open the Hub control panel in a new browser tab"
 msgstr "在新的游览器选项卡中打开 Hub 控制面板"
 
-#: packages/hub-extension/src/index.ts:90 packages/mainmenu-extension/src/index.ts:443
+#: packages/hub-extension/src/index.ts:90 packages/mainmenu-extension/src/index.ts:440 packages/mainmenu-extension/src/index.ts:443
 msgid "Log Out"
 msgstr "注销"
 
 #: packages/hub-extension/src/index.ts:91
 msgid "Log out of the Hub"
 msgstr "退出 Hub"
 
@@ -5854,19 +5980,19 @@
 msgid "Are you sure that you want to run arbitrary Javascript within your JupyterLab session?"
 msgstr "您确定要在您的 JupyterLab 会话中运行任意的 JavaScript 吗？"
 
 #: packages/javascript-extension/src/index.ts:45 packages/rendermime/src/renderers.ts:66
 msgid "Run"
 msgstr "运行"
 
-#: packages/launcher-extension/src/index.ts:148 packages/launcher-extension/src/index.ts:94
+#: packages/launcher-extension/src/index.ts:138 packages/launcher-extension/src/index.ts:148 packages/launcher-extension/src/index.ts:84 packages/launcher-extension/src/index.ts:94
 msgid "Launcher"
 msgstr "启动页"
 
-#: packages/launcher-extension/src/index.ts:72 packages/ui-components/src/icon/widgets/tabbarsvg.ts:31
+#: packages/launcher-extension/src/index.ts:62 packages/launcher-extension/src/index.ts:72 packages/ui-components/src/icon/widgets/tabbarsvg.ts:31
 msgid "New Launcher"
 msgstr "新建启动页"
 
 #: packages/launcher/src/widget.tsx:273
 msgctxt "Error"
 msgid "Launcher Error"
 msgstr "启动页错误"
@@ -5935,15 +6061,15 @@
 msgid "No log messages."
 msgstr "无日志消息。"
 
 #: packages/lsp-extension/src/index.ts:285
 msgid "Language servers"
 msgstr "语言服务器"
 
-#: packages/lsp-extension/src/index.ts:304 packages/mainmenu-extension/src/index.ts:549 packages/running-extension/src/kernels.ts:67 packages/running/src/index.tsx:357 packages/terminal-extension/src/index.ts:323
+#: packages/lsp-extension/src/index.ts:304 packages/mainmenu-extension/src/index.ts:546 packages/mainmenu-extension/src/index.ts:549 packages/running-extension/src/kernels.ts:67 packages/running-extension/src/kernels.tsx:87 packages/running/src/index.tsx:357 packages/running/src/index.tsx:573 packages/terminal-extension/src/index.ts:323
 msgid "Shut Down All"
 msgstr "全部关闭"
 
 #: packages/lsp-extension/src/index.ts:305
 msgid "Are you sure you want to permanently shut down all running language servers?"
 msgstr "您确定要永久关闭所有正在运行的语言服务器吗？"
 
@@ -5967,146 +6093,190 @@
 msgid "Add server"
 msgstr "添加服务器"
 
 #: packages/lsp/src/adapters/adapter.ts:482 packages/lsp/src/adapters/adapter.ts:500
 msgid "Message from "
 msgstr "信息来源 "
 
-#: packages/mainmenu-extension/src/index.ts:193
+#: packages/mainmenu-extension/src/index.ts:193 packages/mainmenu-extension/src/index.ts:194
 msgid "Open Edit Menu"
 msgstr "打开编辑菜单"
 
-#: packages/mainmenu-extension/src/index.ts:197
+#: packages/mainmenu-extension/src/index.ts:197 packages/mainmenu-extension/src/index.ts:198
 msgid "Open File Menu"
 msgstr "打开文件菜单"
 
-#: packages/mainmenu-extension/src/index.ts:201
+#: packages/mainmenu-extension/src/index.ts:201 packages/mainmenu-extension/src/index.ts:202
 msgid "Open Kernel Menu"
 msgstr "打开内核菜单"
 
-#: packages/mainmenu-extension/src/index.ts:205
+#: packages/mainmenu-extension/src/index.ts:205 packages/mainmenu-extension/src/index.ts:206
 msgid "Open Run Menu"
 msgstr "打开运行菜单"
 
-#: packages/mainmenu-extension/src/index.ts:209
+#: packages/mainmenu-extension/src/index.ts:209 packages/mainmenu-extension/src/index.ts:210
 msgid "Open View Menu"
 msgstr "打开视图菜单"
 
-#: packages/mainmenu-extension/src/index.ts:213
+#: packages/mainmenu-extension/src/index.ts:213 packages/mainmenu-extension/src/index.ts:214
 msgid "Open Settings Menu"
 msgstr "打开设置菜单"
 
-#: packages/mainmenu-extension/src/index.ts:217
+#: packages/mainmenu-extension/src/index.ts:217 packages/mainmenu-extension/src/index.ts:218
 msgid "Open Tabs Menu"
 msgstr "打开标签页菜单"
 
-#: packages/mainmenu-extension/src/index.ts:221
+#: packages/mainmenu-extension/src/index.ts:221 packages/mainmenu-extension/src/index.ts:222
 msgid "Open Help Menu"
 msgstr "打开帮助菜单"
 
-#: packages/mainmenu-extension/src/index.ts:225
+#: packages/mainmenu-extension/src/index.ts:225 packages/mainmenu-extension/src/index.ts:226
 msgid "Open First Menu"
 msgstr "打开首个菜单"
 
-#: packages/mainmenu-extension/src/index.ts:245
+#: packages/mainmenu-extension/src/index.ts:245 packages/mainmenu-extension/src/index.ts:246
 msgid "Kernel Operations"
 msgstr "内核操作"
 
-#: packages/mainmenu-extension/src/index.ts:301
+#: packages/mainmenu-extension/src/index.ts:299 packages/mainmenu-extension/src/index.ts:301
 msgid "Clear"
 msgstr "清空"
 
-#: packages/mainmenu-extension/src/index.ts:312
+#: packages/mainmenu-extension/src/index.ts:309 packages/mainmenu-extension/src/index.ts:312
 msgid "Clear All"
 msgstr "全部清除"
 
-#: packages/mainmenu-extension/src/index.ts:352
+#: packages/mainmenu-extension/src/index.ts:348 packages/mainmenu-extension/src/index.ts:352
 msgid "Close and Shut Down"
 msgstr "关闭并停止"
 
-#: packages/mainmenu-extension/src/index.ts:368
+#: packages/mainmenu-extension/src/index.ts:365 packages/mainmenu-extension/src/index.ts:368
 msgid "New Console for Activity"
 msgstr "新建活动控制台"
 
+#: packages/mainmenu-extension/src/index.ts:372
+msgid "Shut down %1"
+msgstr "关闭 %1"
+
 #: packages/mainmenu-extension/src/index.ts:376
 msgid "Shut down JupyterLab"
 msgstr "关闭 JuputerLab"
 
-#: packages/mainmenu-extension/src/index.ts:381
+#: packages/mainmenu-extension/src/index.ts:377 packages/mainmenu-extension/src/index.ts:381
 msgid "Shutdown confirmation"
 msgstr "关闭服务确认"
 
+#: packages/mainmenu-extension/src/index.ts:378
+msgid "Please confirm you want to shut down %1."
+msgstr "请确认您要关闭 %1。"
+
 #: packages/mainmenu-extension/src/index.ts:382
 msgid "Please confirm you want to shut down JupyterLab."
 msgstr "请确认您想要关闭 JupyterLab。"
 
-#: packages/mainmenu-extension/src/index.ts:414
+#: packages/mainmenu-extension/src/index.ts:410 packages/mainmenu-extension/src/index.ts:414
 msgid "You have shut down the Jupyter server. You can now close this tab."
 msgstr "您已关闭 Jupyter 服务进程。您现在可以关闭此选项卡。"
 
+#: packages/mainmenu-extension/src/index.ts:414
+msgid "To use %1 again, you will need to relaunch it."
+msgstr "要再次使用 %1，您需要重新启动它。"
+
 #: packages/mainmenu-extension/src/index.ts:418
 msgid "To use JupyterLab again, you will need to relaunch it."
 msgstr "若要再次使用 JupyterLab，您需要重新运行它。"
 
-#: packages/mainmenu-extension/src/index.ts:425
+#: packages/mainmenu-extension/src/index.ts:422 packages/mainmenu-extension/src/index.ts:425
 msgid "Server stopped"
 msgstr "服务进程已终止"
 
+#: packages/mainmenu-extension/src/index.ts:441
+msgid "Log out of %1"
+msgstr "退出 %1"
+
 #: packages/mainmenu-extension/src/index.ts:444
 msgid "Log out of JupyterLab"
 msgstr "退出 JupyterLab"
 
-#: packages/mainmenu-extension/src/index.ts:482 packages/notebook-extension/src/index.ts:3158
+#: packages/mainmenu-extension/src/index.ts:480 packages/mainmenu-extension/src/index.ts:482 packages/notebook-extension/src/index.ts:3158 packages/notebook-extension/src/index.ts:3165 packages/notebook-extension/src/index.ts:3188
 msgid "Reconnect to Kernel"
 msgstr "重新连接至内核"
 
 #: packages/mainmenu-extension/src/index.ts:507
 msgid "Restart Kernel and Clear…"
 msgstr "重启内核并清除…"
 
-#: packages/mainmenu-extension/src/index.ts:532
+#: packages/mainmenu-extension/src/index.ts:530 packages/mainmenu-extension/src/index.ts:532
 msgid "Shut down kernel"
 msgstr "终止内核"
 
-#: packages/mainmenu-extension/src/index.ts:539
+#: packages/mainmenu-extension/src/index.ts:536 packages/mainmenu-extension/src/index.ts:539
 msgid "Shut Down All Kernels…"
 msgstr "关闭所有内核…"
 
-#: packages/mainmenu-extension/src/index.ts:545
+#: packages/mainmenu-extension/src/index.ts:542 packages/mainmenu-extension/src/index.ts:545
 msgid "Shut Down All?"
 msgstr "全部关闭？"
 
-#: packages/mainmenu-extension/src/index.ts:546
+#: packages/mainmenu-extension/src/index.ts:543 packages/mainmenu-extension/src/index.ts:546
 msgid "Shut down all kernels?"
 msgstr "关闭所有内核?"
 
-#: packages/mainmenu-extension/src/index.ts:622 packages/mainmenu-extension/src/index.ts:623
+#: packages/mainmenu-extension/src/index.ts:617 packages/mainmenu-extension/src/index.ts:618 packages/mainmenu-extension/src/index.ts:622 packages/mainmenu-extension/src/index.ts:623
 msgid "Run Selected"
 msgstr "运行选定单元格"
 
-#: packages/mainmenu-extension/src/index.ts:636 packages/mainmenu-extension/src/index.ts:637
+#: packages/mainmenu-extension/src/index.ts:632 packages/mainmenu-extension/src/index.ts:633 packages/mainmenu-extension/src/index.ts:636 packages/mainmenu-extension/src/index.ts:637
 msgid "Run All"
 msgstr "运行所有"
 
-#: packages/mainmenu-extension/src/index.ts:648 packages/mainmenu-extension/src/index.ts:649
+#: packages/mainmenu-extension/src/index.ts:644 packages/mainmenu-extension/src/index.ts:645 packages/mainmenu-extension/src/index.ts:648 packages/mainmenu-extension/src/index.ts:649
 msgid "Restart Kernel and Run All"
 msgstr "重启内核并运行所有"
 
-#: packages/mainmenu-extension/src/index.ts:677
+#: packages/mainmenu-extension/src/index.ts:674 packages/mainmenu-extension/src/index.ts:677
 msgid "Activate a widget by its `id`."
 msgstr "通过它的`id`激活一个小部件。"
 
-#: packages/mainmenu-extension/src/index.ts:694
+#: packages/mainmenu-extension/src/index.ts:691 packages/mainmenu-extension/src/index.ts:694
 msgid "Activate Previously Used Tab"
 msgstr "激活之前使用过的标签"
 
-#: packages/mainmenu-extension/src/index.ts:771
+#: packages/mainmenu-extension/src/index.ts:768 packages/mainmenu-extension/src/index.ts:771
 msgid "Menu customization has changed. You will need to reload JupyterLab to see the changes."
 msgstr "菜单自定义已更改。您需要重新加载 JupyterLab 来查看改动。"
 
+#: packages/mainmenu-extension/src/recents.ts:155
+msgid "Could Not Open Recent"
+msgstr "无法打开最近的项目"
+
+#: packages/mainmenu-extension/src/recents.ts:156
+msgid "%1 is no longer valid and will be removed from the list"
+msgstr "%1 不再有效，将从列表中移除"
+
+#: packages/mainmenu-extension/src/recents.ts:189
+msgid "Open a Recent Document (given by `recent` argument)"
+msgstr "打开最近的文档（由 `recent` 参数指定）"
+
+#: packages/mainmenu-extension/src/recents.ts:217
+msgid "Reopen %1"
+msgstr "重新打开 %1"
+
+#: packages/mainmenu-extension/src/recents.ts:218
+msgid "Reopen Closed Document"
+msgstr "重新打开已关闭的文档。"
+
+#: packages/mainmenu-extension/src/recents.ts:223
+msgid "Reopen recently closed file or notebook."
+msgstr "重新打开最近关闭的文件或笔记本。"
+
+#: packages/mainmenu-extension/src/recents.ts:232
+msgid "Open Recent"
+msgstr "打开最近的项目"
+
 #: packages/markdownviewer-extension/src/index.ts:124 packages/markdownviewer-extension/src/index.ts:150
 msgid "Markdown Preview"
 msgstr "Markdown 预览"
 
 #: packages/markdownviewer-extension/src/index.ts:185
 msgid "Show Markdown Editor"
 msgstr "显示 Markdown 编辑器"
@@ -6115,534 +6285,546 @@
 msgid "Mermaid Copy Diagram Source"
 msgstr "复制 Mermaid 图表源代码"
 
 #: packages/metadataform/src/metadataform.ts:54
 msgid "No metadata."
 msgstr "没有元数据。"
 
-#: packages/notebook-extension/src/index.ts:1146
+#: packages/notebook-extension/src/index.ts:1146 packages/notebook-extension/src/index.ts:1150 packages/notebook-extension/src/index.ts:1158
 msgid "Notebook Tools"
 msgstr "笔记本工具"
 
-#: packages/notebook-extension/src/index.ts:1298
+#: packages/notebook-extension/src/index.ts:1298 packages/notebook-extension/src/index.ts:1302 packages/notebook-extension/src/index.ts:1310
 msgid "Create New View for Cell Output"
 msgstr "为单元格输出创建新视图"
 
-#: packages/notebook-extension/src/index.ts:1368
+#: packages/notebook-extension/src/index.ts:1368 packages/notebook-extension/src/index.ts:1372 packages/notebook-extension/src/index.ts:1380
 msgid "New Console for Notebook"
 msgstr "新建笔记本控制台"
 
-#: packages/notebook-extension/src/index.ts:1386
+#: packages/notebook-extension/src/index.ts:1386 packages/notebook-extension/src/index.ts:1390 packages/notebook-extension/src/index.ts:1398
 msgid "Run Selected Text or Current Line in Console"
 msgstr "在控制台中运行所选文本或当前行"
 
-#: packages/notebook-extension/src/index.ts:1550
+#: packages/notebook-extension/src/index.ts:1550 packages/notebook-extension/src/index.ts:1554 packages/notebook-extension/src/index.ts:1562
 msgid "Copy Output to Clipboard"
 msgstr "复制输出到剪贴板"
 
-#: packages/notebook-extension/src/index.ts:1707
+#: packages/notebook-extension/src/index.ts:1707 packages/notebook-extension/src/index.ts:1712 packages/notebook-extension/src/index.ts:1723
 msgid "Auto Close Brackets for All Notebook Cell Types"
 msgstr "为所有笔记本单元格类型自动闭合括号"
 
-#: packages/notebook-extension/src/index.ts:1716
+#: packages/notebook-extension/src/index.ts:1716 packages/notebook-extension/src/index.ts:1721 packages/notebook-extension/src/index.ts:1732
 msgid "Set side-by-side ratio"
 msgstr "设置并排显示比例"
 
-#: packages/notebook-extension/src/index.ts:1719
+#: packages/notebook-extension/src/index.ts:1719 packages/notebook-extension/src/index.ts:1724 packages/notebook-extension/src/index.ts:1735
 msgid "Width of the output in side-by-side mode"
 msgstr "并排显示模式的输出宽度"
 
-#: packages/notebook-extension/src/index.ts:1953
+#: packages/notebook-extension/src/index.ts:1953 packages/notebook-extension/src/index.ts:1958 packages/notebook-extension/src/index.ts:1969
 msgid "New Notebook"
 msgstr "新建笔记本"
 
-#: packages/notebook-extension/src/index.ts:1957
+#: packages/notebook-extension/src/index.ts:1957 packages/notebook-extension/src/index.ts:1962 packages/notebook-extension/src/index.ts:1973
 msgid "Create a new notebook"
 msgstr "创建笔记本"
 
-#: packages/notebook-extension/src/index.ts:2213
+#: packages/notebook-extension/src/index.ts:2213 packages/notebook-extension/src/index.ts:2220 packages/notebook-extension/src/index.ts:2231
 msgid "Run Selected Cell"
 msgid_plural "Run Selected Cells"
 msgstr[0] "运行选中的单元格"
 
-#: packages/notebook-extension/src/index.ts:2221
+#: packages/notebook-extension/src/index.ts:2221 packages/notebook-extension/src/index.ts:2228 packages/notebook-extension/src/index.ts:2239
 msgid "Run this cell and advance"
 msgid_plural "Run these %1 cells and advance"
 msgstr[0] "运行这 %1 个单元格并向前移动"
 
-#: packages/notebook-extension/src/index.ts:2247
+#: packages/notebook-extension/src/index.ts:2247 packages/notebook-extension/src/index.ts:2254 packages/notebook-extension/src/index.ts:2265
 msgid "Run Selected Cell and Do not Advance"
 msgid_plural "Run Selected Cells and Do not Advance"
 msgstr[0] "运行选定的所有单元格且不再继续"
 
-#: packages/notebook-extension/src/index.ts:2272
+#: packages/notebook-extension/src/index.ts:2272 packages/notebook-extension/src/index.ts:2279 packages/notebook-extension/src/index.ts:2290
 msgid "Run Selected Cell and Insert Below"
 msgid_plural "Run Selected Cells and Insert Below"
 msgstr[0] "运行选中的单元格并在下面插入"
 
-#: packages/notebook-extension/src/index.ts:2295
+#: packages/notebook-extension/src/index.ts:2295 packages/notebook-extension/src/index.ts:2302 packages/notebook-extension/src/index.ts:2313
 msgid "Run All Cells"
 msgstr "运行所有单元格"
 
-#: packages/notebook-extension/src/index.ts:2296
+#: packages/notebook-extension/src/index.ts:2296 packages/notebook-extension/src/index.ts:2303 packages/notebook-extension/src/index.ts:2314
 msgid "Run all cells"
 msgstr "运行所有单元格"
 
-#: packages/notebook-extension/src/index.ts:2314
+#: packages/notebook-extension/src/index.ts:2314 packages/notebook-extension/src/index.ts:2321 packages/notebook-extension/src/index.ts:2332
 msgid "Run All Above Selected Cell"
 msgstr "运行选中单元格上方的所有单元格"
 
-#: packages/notebook-extension/src/index.ts:2339
+#: packages/notebook-extension/src/index.ts:2339 packages/notebook-extension/src/index.ts:2346 packages/notebook-extension/src/index.ts:2357
 msgid "Run Selected Cell and All Below"
 msgstr "运行选中的单元格及以下所有"
 
-#: packages/notebook-extension/src/index.ts:2365
+#: packages/notebook-extension/src/index.ts:2365 packages/notebook-extension/src/index.ts:2372 packages/notebook-extension/src/index.ts:2383
 msgid "Render All Markdown Cells"
 msgstr "渲染全部 Markdown"
 
-#: packages/notebook-extension/src/index.ts:2402
+#: packages/notebook-extension/src/index.ts:2402 packages/notebook-extension/src/index.ts:2409
 msgid "Close and Shut Down Notebook"
 msgstr "关闭并终止笔记本服务"
 
-#: packages/notebook-extension/src/index.ts:2413
+#: packages/notebook-extension/src/index.ts:2413 packages/notebook-extension/src/index.ts:2420 packages/notebook-extension/src/index.ts:2431
 msgid "Shut down the notebook?"
 msgstr "关闭笔记本？"
 
-#: packages/notebook-extension/src/index.ts:2429
+#: packages/notebook-extension/src/index.ts:2420
+msgid "Close and Shut Down Notebook…"
+msgstr "关闭并终止笔记本服务..."
+
+#: packages/notebook-extension/src/index.ts:2429 packages/notebook-extension/src/index.ts:2436 packages/notebook-extension/src/index.ts:2447
 msgid "Trust Notebook"
 msgstr "信任笔记本"
 
-#: packages/notebook-extension/src/index.ts:2440
+#: packages/notebook-extension/src/index.ts:2440 packages/notebook-extension/src/index.ts:2447 packages/notebook-extension/src/index.ts:2458
 msgid "Restart Kernel and Clear Outputs of All Cells…"
 msgstr "重新启动内核并清除所有单元格的输出…"
 
-#: packages/notebook-extension/src/index.ts:2441
+#: packages/notebook-extension/src/index.ts:2441 packages/notebook-extension/src/index.ts:2448 packages/notebook-extension/src/index.ts:2459
 msgid "Restart the kernel and clear all outputs of all cells"
 msgstr "重新启动内核并清除全部单元格的所有输出"
 
-#: packages/notebook-extension/src/index.ts:2453
+#: packages/notebook-extension/src/index.ts:2453 packages/notebook-extension/src/index.ts:2460 packages/notebook-extension/src/index.ts:2471
 msgid "Restart Kernel and Run up to Selected Cell…"
 msgstr "重启内核并运行到所选单元格…"
 
-#: packages/notebook-extension/src/index.ts:2477
+#: packages/notebook-extension/src/index.ts:2477 packages/notebook-extension/src/index.ts:2484 packages/notebook-extension/src/index.ts:2495
 msgid "Restart Kernel and Run All Cells…"
 msgstr "重启并运行所有单元格…"
 
-#: packages/notebook-extension/src/index.ts:2478
+#: packages/notebook-extension/src/index.ts:2478 packages/notebook-extension/src/index.ts:2485 packages/notebook-extension/src/index.ts:2496
 msgid "Restart the kernel and run all cells"
 msgstr "重启内核并运行所有单元格"
 
-#: packages/notebook-extension/src/index.ts:2504
+#: packages/notebook-extension/src/index.ts:2504 packages/notebook-extension/src/index.ts:2511 packages/notebook-extension/src/index.ts:2522
 msgid "Clear Outputs of All Cells"
 msgstr "清除所有单元格的输出"
 
-#: packages/notebook-extension/src/index.ts:2505
+#: packages/notebook-extension/src/index.ts:2505 packages/notebook-extension/src/index.ts:2512 packages/notebook-extension/src/index.ts:2523
 msgid "Clear all outputs of all cells"
 msgstr "清除所有单元格的全部输出"
 
-#: packages/notebook-extension/src/index.ts:2516
+#: packages/notebook-extension/src/index.ts:2516 packages/notebook-extension/src/index.ts:2523 packages/notebook-extension/src/index.ts:2534
 msgid "Clear Cell Output"
 msgstr "清除单元格输出"
 
-#: packages/notebook-extension/src/index.ts:2517
+#: packages/notebook-extension/src/index.ts:2517 packages/notebook-extension/src/index.ts:2524 packages/notebook-extension/src/index.ts:2535
 msgid "Clear outputs for the selected cells"
 msgstr "清除选中单元格的输出"
 
-#: packages/notebook-extension/src/index.ts:2547
+#: packages/notebook-extension/src/index.ts:2547 packages/notebook-extension/src/index.ts:2554 packages/notebook-extension/src/index.ts:2565
 msgid "Change to Code Cell Type"
 msgstr "更改为代码单元格类型"
 
-#: packages/notebook-extension/src/index.ts:2558
+#: packages/notebook-extension/src/index.ts:2558 packages/notebook-extension/src/index.ts:2565 packages/notebook-extension/src/index.ts:2580
 msgid "Change to Markdown Cell Type"
 msgstr "更改为 Markdown 类型"
 
-#: packages/notebook-extension/src/index.ts:2569
+#: packages/notebook-extension/src/index.ts:2569 packages/notebook-extension/src/index.ts:2576 packages/notebook-extension/src/index.ts:2595
 msgid "Change to Raw Cell Type"
 msgstr "更改为纯文本单元格类型"
 
-#: packages/notebook-extension/src/index.ts:2582
+#: packages/notebook-extension/src/index.ts:2582 packages/notebook-extension/src/index.ts:2589 packages/notebook-extension/src/index.ts:2612
 msgid "Cut Cell"
 msgid_plural "Cut Cells"
 msgstr[0] "剪切单元格"
 
-#: packages/notebook-extension/src/index.ts:2590
+#: packages/notebook-extension/src/index.ts:2590 packages/notebook-extension/src/index.ts:2597 packages/notebook-extension/src/index.ts:2620
 msgid "Cut this cell"
 msgid_plural "Cut these %1 cells"
 msgstr[0] "剪切这 %1 个单元格"
 
-#: packages/notebook-extension/src/index.ts:2609
+#: packages/notebook-extension/src/index.ts:2609 packages/notebook-extension/src/index.ts:2616 packages/notebook-extension/src/index.ts:2639
 msgid "Copy Cell"
 msgid_plural "Copy Cells"
 msgstr[0] "复制单元格"
 
-#: packages/notebook-extension/src/index.ts:2617
+#: packages/notebook-extension/src/index.ts:2617 packages/notebook-extension/src/index.ts:2624 packages/notebook-extension/src/index.ts:2647
 msgid "Copy this cell"
 msgid_plural "Copy these %1 cells"
 msgstr[0] "复制这 %1 个单元格"
 
-#: packages/notebook-extension/src/index.ts:2636
+#: packages/notebook-extension/src/index.ts:2636 packages/notebook-extension/src/index.ts:2643 packages/notebook-extension/src/index.ts:2666
 msgid "Paste Cell Below"
 msgid_plural "Paste Cells Below"
 msgstr[0] "在下面粘贴单元格"
 
-#: packages/notebook-extension/src/index.ts:2644 packages/notebook-extension/src/index.ts:2671
+#: packages/notebook-extension/src/index.ts:2644 packages/notebook-extension/src/index.ts:2651 packages/notebook-extension/src/index.ts:2671 packages/notebook-extension/src/index.ts:2674 packages/notebook-extension/src/index.ts:2678 packages/notebook-extension/src/index.ts:2701
 msgid "Paste this cell from the clipboard"
 msgid_plural "Paste these %1 cells from the clipboard"
 msgstr[0] "从剪贴板粘贴这 %1 个单元格"
 
-#: packages/notebook-extension/src/index.ts:2663
+#: packages/notebook-extension/src/index.ts:2663 packages/notebook-extension/src/index.ts:2670 packages/notebook-extension/src/index.ts:2693
 msgid "Paste Cell Above"
 msgid_plural "Paste Cells Above"
 msgstr[0] "在上方粘贴单元格"
 
-#: packages/notebook-extension/src/index.ts:2689
+#: packages/notebook-extension/src/index.ts:2689 packages/notebook-extension/src/index.ts:2696 packages/notebook-extension/src/index.ts:2719
 msgid "Duplicate Cell Below"
 msgid_plural "Duplicate Cells Below"
 msgstr[0] "复制单元格至下方"
 
-#: packages/notebook-extension/src/index.ts:2697
+#: packages/notebook-extension/src/index.ts:2697 packages/notebook-extension/src/index.ts:2704 packages/notebook-extension/src/index.ts:2727
 msgid "Create a duplicate of this cell below"
 msgid_plural "Create duplicates of %1 cells below"
 msgstr[0] "在下方创建 %1 单元格的副本"
 
-#: packages/notebook-extension/src/index.ts:2716
+#: packages/notebook-extension/src/index.ts:2716 packages/notebook-extension/src/index.ts:2723 packages/notebook-extension/src/index.ts:2746
 msgid "Paste Cell and Replace"
 msgid_plural "Paste Cells and Replace"
 msgstr[0] "粘贴单元格并替换"
 
-#: packages/notebook-extension/src/index.ts:2734
+#: packages/notebook-extension/src/index.ts:2734 packages/notebook-extension/src/index.ts:2741 packages/notebook-extension/src/index.ts:2764
 msgid "Delete Cell"
 msgid_plural "Delete Cells"
 msgstr[0] "删除单元格"
 
-#: packages/notebook-extension/src/index.ts:2742
+#: packages/notebook-extension/src/index.ts:2742 packages/notebook-extension/src/index.ts:2749 packages/notebook-extension/src/index.ts:2772
 msgid "Delete this cell"
 msgid_plural "Delete these %1 cells"
 msgstr[0] "删除这 %1 个单元格"
 
-#: packages/notebook-extension/src/index.ts:2759
+#: packages/notebook-extension/src/index.ts:2759 packages/notebook-extension/src/index.ts:2766 packages/notebook-extension/src/index.ts:2789
 msgid "Split Cell"
 msgstr "拆分单元格"
 
-#: packages/notebook-extension/src/index.ts:2770
+#: packages/notebook-extension/src/index.ts:2770 packages/notebook-extension/src/index.ts:2777 packages/notebook-extension/src/index.ts:2800
 msgid "Merge Selected Cells"
 msgstr "合并所选单元格"
 
-#: packages/notebook-extension/src/index.ts:2781
+#: packages/notebook-extension/src/index.ts:2781 packages/notebook-extension/src/index.ts:2788 packages/notebook-extension/src/index.ts:2811
 msgid "Merge Cell Above"
 msgstr "合并上方单元格"
 
-#: packages/notebook-extension/src/index.ts:2792
+#: packages/notebook-extension/src/index.ts:2792 packages/notebook-extension/src/index.ts:2799 packages/notebook-extension/src/index.ts:2822
 msgid "Merge Cell Below"
 msgstr "合并下方单元格"
 
-#: packages/notebook-extension/src/index.ts:2803
+#: packages/notebook-extension/src/index.ts:2803 packages/notebook-extension/src/index.ts:2810 packages/notebook-extension/src/index.ts:2833
 msgid "Insert Cell Above"
 msgstr "上方插入单元格"
 
-#: packages/notebook-extension/src/index.ts:2804
+#: packages/notebook-extension/src/index.ts:2804 packages/notebook-extension/src/index.ts:2811 packages/notebook-extension/src/index.ts:2834
 msgid "Insert a cell above"
 msgstr "上方插入单元格"
 
-#: packages/notebook-extension/src/index.ts:2816
+#: packages/notebook-extension/src/index.ts:2816 packages/notebook-extension/src/index.ts:2823 packages/notebook-extension/src/index.ts:2846
 msgid "Insert Cell Below"
 msgstr "下方插入单元格"
 
-#: packages/notebook-extension/src/index.ts:2817 packages/notebook/src/default-toolbar.tsx:121
+#: packages/notebook-extension/src/index.ts:2817 packages/notebook-extension/src/index.ts:2824 packages/notebook-extension/src/index.ts:2847 packages/notebook/src/default-toolbar.tsx:121
 msgid "Insert a cell below"
 msgstr "下方插入单元格"
 
-#: packages/notebook-extension/src/index.ts:2829
+#: packages/notebook-extension/src/index.ts:2829 packages/notebook-extension/src/index.ts:2836 packages/notebook-extension/src/index.ts:2859
 msgid "Select Cell Above"
 msgstr "选择上方单元格"
 
-#: packages/notebook-extension/src/index.ts:2840
+#: packages/notebook-extension/src/index.ts:2840 packages/notebook-extension/src/index.ts:2847 packages/notebook-extension/src/index.ts:2870
 msgid "Select Cell Below"
 msgstr "选择下方单元格"
 
-#: packages/notebook-extension/src/index.ts:2850
+#: packages/notebook-extension/src/index.ts:2850 packages/notebook-extension/src/index.ts:2857 packages/notebook-extension/src/index.ts:2880
 msgid "Insert Heading Above Current Heading"
 msgstr "在当前标题上方插入标题"
 
-#: packages/notebook-extension/src/index.ts:2861
+#: packages/notebook-extension/src/index.ts:2861 packages/notebook-extension/src/index.ts:2868 packages/notebook-extension/src/index.ts:2891
 msgid "Insert Heading Below Current Heading"
 msgstr "在当前标题下方插入标题"
 
-#: packages/notebook-extension/src/index.ts:2872
+#: packages/notebook-extension/src/index.ts:2872 packages/notebook-extension/src/index.ts:2879 packages/notebook-extension/src/index.ts:2902
 msgid "Select Heading Above or Collapse Heading"
 msgstr "选择上面的标题或折叠标题。"
 
-#: packages/notebook-extension/src/index.ts:2885
+#: packages/notebook-extension/src/index.ts:2885 packages/notebook-extension/src/index.ts:2892 packages/notebook-extension/src/index.ts:2915
 msgid "Select Heading Below or Expand Heading"
 msgstr "选择下面的标题或展开标题"
 
-#: packages/notebook-extension/src/index.ts:2898
+#: packages/notebook-extension/src/index.ts:2898 packages/notebook-extension/src/index.ts:2905 packages/notebook-extension/src/index.ts:2928
 msgid "Extend Selection Above"
 msgstr "向上方扩展选区"
 
-#: packages/notebook-extension/src/index.ts:2909
+#: packages/notebook-extension/src/index.ts:2909 packages/notebook-extension/src/index.ts:2916 packages/notebook-extension/src/index.ts:2939
 msgid "Extend Selection to Top"
 msgstr "将选区扩展到顶部"
 
-#: packages/notebook-extension/src/index.ts:2920
+#: packages/notebook-extension/src/index.ts:2920 packages/notebook-extension/src/index.ts:2927 packages/notebook-extension/src/index.ts:2950
 msgid "Extend Selection Below"
 msgstr "向下方扩展选区"
 
-#: packages/notebook-extension/src/index.ts:2931
+#: packages/notebook-extension/src/index.ts:2931 packages/notebook-extension/src/index.ts:2938 packages/notebook-extension/src/index.ts:2961
 msgid "Extend Selection to Bottom"
 msgstr "将选区扩展到底部"
 
-#: packages/notebook-extension/src/index.ts:2942
+#: packages/notebook-extension/src/index.ts:2942 packages/notebook-extension/src/index.ts:2949 packages/notebook-extension/src/index.ts:2972
 msgid "Select All Cells"
 msgstr "选择所有单元格"
 
-#: packages/notebook-extension/src/index.ts:2953
+#: packages/notebook-extension/src/index.ts:2953 packages/notebook-extension/src/index.ts:2960 packages/notebook-extension/src/index.ts:2983
 msgid "Deselect All Cells"
 msgstr "取消选择所有单元格"
 
-#: packages/notebook-extension/src/index.ts:2966
+#: packages/notebook-extension/src/index.ts:2966 packages/notebook-extension/src/index.ts:2973 packages/notebook-extension/src/index.ts:2996
 msgid "Move Cell Up"
 msgid_plural "Move Cells Up"
 msgstr[0] "上移单元格"
 
-#: packages/notebook-extension/src/index.ts:2974
+#: packages/notebook-extension/src/index.ts:2974 packages/notebook-extension/src/index.ts:2981 packages/notebook-extension/src/index.ts:3004
 msgid "Move this cell up"
 msgid_plural "Move these %1 cells up"
 msgstr[0] "把这 %1 个单元格上移"
 
-#: packages/notebook-extension/src/index.ts:2986
+#: packages/notebook-extension/src/index.ts:2986 packages/notebook-extension/src/index.ts:2993 packages/notebook-extension/src/index.ts:3016
 msgid "Notebook cell shifted up successfully"
 msgstr "笔记本单元格已成功上移"
 
-#: packages/notebook-extension/src/index.ts:3003
+#: packages/notebook-extension/src/index.ts:3003 packages/notebook-extension/src/index.ts:3010 packages/notebook-extension/src/index.ts:3033
 msgid "Move Cell Down"
 msgid_plural "Move Cells Down"
 msgstr[0] "下移单元格"
 
-#: packages/notebook-extension/src/index.ts:3011
+#: packages/notebook-extension/src/index.ts:3011 packages/notebook-extension/src/index.ts:3018 packages/notebook-extension/src/index.ts:3041
 msgid "Move this cell down"
 msgid_plural "Move these %1 cells down"
 msgstr[0] "把这 %1 个单元格下移"
 
-#: packages/notebook-extension/src/index.ts:3023
+#: packages/notebook-extension/src/index.ts:3023 packages/notebook-extension/src/index.ts:3030 packages/notebook-extension/src/index.ts:3053
 msgid "Notebook cell shifted down successfully"
 msgstr "笔记本单元格已成功下移"
 
-#: packages/notebook-extension/src/index.ts:3064
+#: packages/notebook-extension/src/index.ts:3064 packages/notebook-extension/src/index.ts:3071 packages/notebook-extension/src/index.ts:3094
 msgid "Enter Command Mode"
 msgstr "进入命令模式"
 
-#: packages/notebook-extension/src/index.ts:3075
+#: packages/notebook-extension/src/index.ts:3075 packages/notebook-extension/src/index.ts:3082 packages/notebook-extension/src/index.ts:3105
 msgid "Enter Edit Mode"
 msgstr "进入编辑模式"
 
-#: packages/notebook-extension/src/index.ts:3086
+#: packages/notebook-extension/src/index.ts:3086 packages/notebook-extension/src/index.ts:3093 packages/notebook-extension/src/index.ts:3116
 msgid "Undo Cell Operation"
 msgstr "撤销单元格操作"
 
-#: packages/notebook-extension/src/index.ts:3097
+#: packages/notebook-extension/src/index.ts:3097 packages/notebook-extension/src/index.ts:3104 packages/notebook-extension/src/index.ts:3127
 msgid "Redo Cell Operation"
 msgstr "重做单元格操作"
 
-#: packages/notebook-extension/src/index.ts:3175
+#: packages/notebook-extension/src/index.ts:3175 packages/notebook-extension/src/index.ts:3182 packages/notebook-extension/src/index.ts:3205
 msgid "Change to Heading 1"
 msgstr "更改为标题 1"
 
-#: packages/notebook-extension/src/index.ts:3186
+#: packages/notebook-extension/src/index.ts:3186 packages/notebook-extension/src/index.ts:3193 packages/notebook-extension/src/index.ts:3220
 msgid "Change to Heading 2"
 msgstr "更改为标题 2"
 
-#: packages/notebook-extension/src/index.ts:3197
+#: packages/notebook-extension/src/index.ts:3197 packages/notebook-extension/src/index.ts:3204 packages/notebook-extension/src/index.ts:3235
 msgid "Change to Heading 3"
 msgstr "更改为标题 3"
 
-#: packages/notebook-extension/src/index.ts:3208
+#: packages/notebook-extension/src/index.ts:3208 packages/notebook-extension/src/index.ts:3215 packages/notebook-extension/src/index.ts:3250
 msgid "Change to Heading 4"
 msgstr "更改为标题 4"
 
-#: packages/notebook-extension/src/index.ts:3219
+#: packages/notebook-extension/src/index.ts:3219 packages/notebook-extension/src/index.ts:3226 packages/notebook-extension/src/index.ts:3265
 msgid "Change to Heading 5"
 msgstr "更改为标题 5"
 
-#: packages/notebook-extension/src/index.ts:3230
+#: packages/notebook-extension/src/index.ts:3230 packages/notebook-extension/src/index.ts:3237 packages/notebook-extension/src/index.ts:3280
 msgid "Change to Heading 6"
 msgstr "更改为标题 6"
 
-#: packages/notebook-extension/src/index.ts:3241
+#: packages/notebook-extension/src/index.ts:3241 packages/notebook-extension/src/index.ts:3248 packages/notebook-extension/src/index.ts:3295
 msgid "Collapse Selected Code"
 msgstr "折叠选定的代码"
 
-#: packages/notebook-extension/src/index.ts:3252
+#: packages/notebook-extension/src/index.ts:3252 packages/notebook-extension/src/index.ts:3259 packages/notebook-extension/src/index.ts:3306
 msgid "Expand Selected Code"
 msgstr "展开选定的代码"
 
-#: packages/notebook-extension/src/index.ts:3263
+#: packages/notebook-extension/src/index.ts:3263 packages/notebook-extension/src/index.ts:3270 packages/notebook-extension/src/index.ts:3317
 msgid "Collapse All Code"
 msgstr "折叠所有代码"
 
-#: packages/notebook-extension/src/index.ts:3274
+#: packages/notebook-extension/src/index.ts:3274 packages/notebook-extension/src/index.ts:3281 packages/notebook-extension/src/index.ts:3328
 msgid "Expand All Code"
 msgstr "展开所有代码"
 
-#: packages/notebook-extension/src/index.ts:3285
+#: packages/notebook-extension/src/index.ts:3285 packages/notebook-extension/src/index.ts:3292 packages/notebook-extension/src/index.ts:3339
 msgid "Collapse Selected Outputs"
 msgstr "折叠选中的输出"
 
-#: packages/notebook-extension/src/index.ts:3296
+#: packages/notebook-extension/src/index.ts:3296 packages/notebook-extension/src/index.ts:3303 packages/notebook-extension/src/index.ts:3350
 msgid "Expand Selected Outputs"
 msgstr "展开选定的输出"
 
-#: packages/notebook-extension/src/index.ts:3307
+#: packages/notebook-extension/src/index.ts:3307 packages/notebook-extension/src/index.ts:3314 packages/notebook-extension/src/index.ts:3361
 msgid "Collapse All Outputs"
 msgstr "折叠全部输出"
 
-#: packages/notebook-extension/src/index.ts:3319
+#: packages/notebook-extension/src/index.ts:3319 packages/notebook-extension/src/index.ts:3326 packages/notebook-extension/src/index.ts:3373
 msgid "Render Side-by-Side"
 msgstr "并排渲染"
 
-#: packages/notebook-extension/src/index.ts:3341
+#: packages/notebook-extension/src/index.ts:3341 packages/notebook-extension/src/index.ts:3348 packages/notebook-extension/src/index.ts:3395
 msgid "Expand All Outputs"
 msgstr "展开全部输出"
 
-#: packages/notebook-extension/src/index.ts:3352
+#: packages/notebook-extension/src/index.ts:3352 packages/notebook-extension/src/index.ts:3359 packages/notebook-extension/src/index.ts:3406
 msgid "Enable Scrolling for Outputs"
 msgstr "启用滚动输出功能"
 
-#: packages/notebook-extension/src/index.ts:3363
+#: packages/notebook-extension/src/index.ts:3363 packages/notebook-extension/src/index.ts:3370 packages/notebook-extension/src/index.ts:3417
 msgid "Disable Scrolling for Outputs"
 msgstr "禁用滚动输出功能"
 
-#: packages/notebook-extension/src/index.ts:3374
+#: packages/notebook-extension/src/index.ts:3374 packages/notebook-extension/src/index.ts:3381 packages/notebook-extension/src/index.ts:3428
 msgid "Select current running or last run cell"
 msgstr "选择正在运行或最后运行的单元格"
 
-#: packages/notebook-extension/src/index.ts:3385
+#: packages/notebook-extension/src/index.ts:3385 packages/notebook-extension/src/index.ts:3392 packages/notebook-extension/src/index.ts:3439
 msgid "Replace Selection in Notebook Cell"
 msgstr "在笔记本单元格中替换选择"
 
-#: packages/notebook-extension/src/index.ts:3397
+#: packages/notebook-extension/src/index.ts:3397 packages/notebook-extension/src/index.ts:3404 packages/notebook-extension/src/index.ts:3451
 msgid "Toggle Collapse Notebook Heading"
 msgstr "切换折叠笔记本标题"
 
-#: packages/notebook-extension/src/index.ts:3407 packages/toc-extension/src/index.ts:141
+#: packages/notebook-extension/src/index.ts:3407 packages/notebook-extension/src/index.ts:3414 packages/notebook-extension/src/index.ts:3461 packages/toc-extension/src/index.ts:141
 msgid "Collapse All Headings"
 msgstr "折叠全部标题"
 
-#: packages/notebook-extension/src/index.ts:3416 packages/toc-extension/src/index.ts:140
+#: packages/notebook-extension/src/index.ts:3416 packages/notebook-extension/src/index.ts:3423 packages/notebook-extension/src/index.ts:3470 packages/toc-extension/src/index.ts:140
 msgid "Expand All Headings"
 msgstr "展开全部标题"
 
-#: packages/notebook-extension/src/index.ts:3425
+#: packages/notebook-extension/src/index.ts:3425 packages/notebook-extension/src/index.ts:3432 packages/notebook-extension/src/index.ts:3479
 msgid "Select and Run Cell(s) for this Heading"
 msgstr "选择并运行此标题下的单元格。"
 
-#: packages/notebook-extension/src/index.ts:3466
+#: packages/notebook-extension/src/index.ts:3466 packages/notebook-extension/src/index.ts:3473 packages/notebook-extension/src/index.ts:3520
 msgid "Access Previous Kernel History Entry"
 msgstr "访问上一条内核历史记录"
 
-#: packages/notebook-extension/src/index.ts:3475
+#: packages/notebook-extension/src/index.ts:3475 packages/notebook-extension/src/index.ts:3482 packages/notebook-extension/src/index.ts:3529
 msgid "Access Next Kernel History Entry"
 msgstr "访问下一条内核历史记录"
 
-#: packages/notebook-extension/src/index.ts:3484
+#: packages/notebook-extension/src/index.ts:3484 packages/notebook-extension/src/index.ts:3491 packages/notebook-extension/src/index.ts:3539
 msgid "Virtual Scrollbar"
 msgstr "虚拟滚动条"
 
-#: packages/notebook-extension/src/index.ts:3485
+#: packages/notebook-extension/src/index.ts:3485 packages/notebook-extension/src/index.ts:3492 packages/notebook-extension/src/index.ts:3540
 msgid "Toggle virtual scrollbar (enabled with windowing mode: full)"
 msgstr "切换虚拟滚动条（在窗口模式为全屏时启用）"
 
-#: packages/notebook-extension/src/index.ts:3519 packages/notebook-extension/src/index.ts:670
+#: packages/notebook-extension/src/index.ts:3519 packages/notebook-extension/src/index.ts:3526 packages/notebook-extension/src/index.ts:3585 packages/notebook-extension/src/index.ts:670 packages/notebook-extension/src/index.ts:674 packages/notebook-extension/src/index.ts:681
 msgid "Notebook Operations"
 msgstr "笔记本操作"
 
-#: packages/notebook-extension/src/index.ts:3557
+#: packages/notebook-extension/src/index.ts:3557 packages/notebook-extension/src/index.ts:3564 packages/notebook-extension/src/index.ts:3623
 msgid "Notebook Cell Operations"
 msgstr "笔记本单元格操作"
 
-#: packages/notebook-extension/src/index.ts:3802
+#: packages/notebook-extension/src/index.ts:3802 packages/notebook-extension/src/index.ts:3809 packages/notebook-extension/src/index.ts:3868
 msgid "PDF"
 msgstr "PDF"
 
-#: packages/notebook-extension/src/index.ts:3803
+#: packages/notebook-extension/src/index.ts:3803 packages/notebook-extension/src/index.ts:3810 packages/notebook-extension/src/index.ts:3869
 msgid "ReStructured Text"
 msgstr "ReStructured 文本"
 
-#: packages/notebook-extension/src/index.ts:3804
+#: packages/notebook-extension/src/index.ts:3804 packages/notebook-extension/src/index.ts:3811 packages/notebook-extension/src/index.ts:3870
 msgid "Executable Script"
 msgstr "可执行脚本"
 
-#: packages/notebook-extension/src/index.ts:3805
+#: packages/notebook-extension/src/index.ts:3805 packages/notebook-extension/src/index.ts:3812 packages/notebook-extension/src/index.ts:3871
 msgid "Reveal.js Slides"
 msgstr "Reveal.js 幻灯片"
 
-#: packages/notebook-extension/src/index.ts:3859
+#: packages/notebook-extension/src/index.ts:3859 packages/notebook-extension/src/index.ts:3866 packages/notebook-extension/src/index.ts:3925
 msgid "For Notebook: %1"
 msgstr "对笔记本：%1"
 
-#: packages/notebook-extension/src/index.ts:3860
+#: packages/notebook-extension/src/index.ts:3860 packages/notebook-extension/src/index.ts:3867 packages/notebook-extension/src/index.ts:3926
 msgid "For Notebook:"
 msgstr "对 Notebook:"
 
-#: packages/notebook-extension/src/index.ts:582
+#: packages/notebook-extension/src/index.ts:582 packages/notebook-extension/src/index.ts:586 packages/notebook-extension/src/index.ts:593
 msgid "Save and Export Notebook to the given `format`."
 msgstr "保存并导出笔记本为指定的 `格式`。"
 
-#: packages/notebook-extension/src/index.ts:586
+#: packages/notebook-extension/src/index.ts:586 packages/notebook-extension/src/index.ts:590 packages/notebook-extension/src/index.ts:597
 msgid "Save and Export Notebook: %1"
 msgstr "保存并导出笔记本：%1"
 
-#: packages/notebook/src/actions.tsx:2094
+#: packages/notebook/src/actions.tsx:2094 packages/notebook/src/actions.tsx:2099 packages/notebook/src/actions.tsx:2107
 msgid "A trusted Jupyter notebook may execute hidden malicious code when you open it."
 msgstr "受信任的 Jupyter 笔记本可能会在您打开它时执行隐藏的恶意代码。"
 
-#: packages/notebook/src/actions.tsx:2098
+#: packages/notebook/src/actions.tsx:2098 packages/notebook/src/actions.tsx:2103 packages/notebook/src/actions.tsx:2111
 msgid "Selecting \"Trust\" will re-render this notebook in a trusted state."
 msgstr "选择“信任”将使此笔记本在受信任的状态下重新渲染。"
 
-#: packages/notebook/src/actions.tsx:2102
+#: packages/notebook/src/actions.tsx:2102 packages/notebook/src/actions.tsx:2107 packages/notebook/src/actions.tsx:2115
 msgid "For more information, see"
 msgstr "更多信息，请参阅"
 
-#: packages/notebook/src/actions.tsx:2108
+#: packages/notebook/src/actions.tsx:2108 packages/notebook/src/actions.tsx:2113 packages/notebook/src/actions.tsx:2121
 msgid "the Jupyter security documentation"
 msgstr "Jupyter 安全文档"
 
-#: packages/notebook/src/actions.tsx:2116
+#: packages/notebook/src/actions.tsx:2116 packages/notebook/src/actions.tsx:2121 packages/notebook/src/actions.tsx:2129
 msgid "Notebook is already trusted"
 msgstr "笔记本已被信任。"
 
-#: packages/notebook/src/actions.tsx:2123
+#: packages/notebook/src/actions.tsx:2123 packages/notebook/src/actions.tsx:2128 packages/notebook/src/actions.tsx:2136
 msgid "Trust this notebook?"
 msgstr "信任此笔记本？"
 
-#: packages/notebook/src/actions.tsx:2127
+#: packages/notebook/src/actions.tsx:2127 packages/notebook/src/actions.tsx:2132 packages/notebook/src/actions.tsx:2140
 msgid "Trust"
 msgstr "信任"
 
-#: packages/notebook/src/actions.tsx:2128
+#: packages/notebook/src/actions.tsx:2128 packages/notebook/src/actions.tsx:2133 packages/notebook/src/actions.tsx:2141
 msgid "Confirm Trusting this notebook"
 msgstr "确认信任此笔记本"
 
-#: packages/notebook/src/actions.tsx:2488
+#: packages/notebook/src/actions.tsx:2488 packages/notebook/src/actions.tsx:2493 packages/notebook/src/cellexecutor.ts:46
 msgid "Kernel Terminating"
 msgstr "正在终止内核"
 
-#: packages/notebook/src/actions.tsx:2489
+#: packages/notebook/src/actions.tsx:2489 packages/notebook/src/actions.tsx:2494 packages/notebook/src/cellexecutor.ts:47
 msgid "The kernel for %1 appears to be terminating. You can not run any cell for now."
 msgstr "%1 的内核似乎正在终止。您现在不能运行任何单元格。"
 
-#: packages/notebook/src/actions.tsx:2499
+#: packages/notebook/src/actions.tsx:2499 packages/notebook/src/actions.tsx:2504 packages/notebook/src/cellexecutor.ts:57
 msgid "Cell not executed due to pending input"
 msgstr "由于包含待定输入，单元格未被执行"
 
-#: packages/notebook/src/actions.tsx:2500
+#: packages/notebook/src/actions.tsx:2500 packages/notebook/src/actions.tsx:2505 packages/notebook/src/cellexecutor.ts:58
 msgid "The cell has not been executed to avoid kernel deadlock as there is another pending input! Submit your pending input and try again."
 msgstr "当前含有未被执行的输入内容，为了防止内核死锁，此单元格尚未被执行。清提交您当前未执行的输入然后再试。"
 
+#: packages/notebook/src/actions.tsx:2610
+msgid "Cell type not changed due to pending input"
+msgstr "由于存在待处理的输入，单元格类型未更改"
+
+#: packages/notebook/src/actions.tsx:2611
+msgid "The cell type has not been changed to avoid kernel deadlock as this cell has pending input! Submit your pending input and try again."
+msgstr "为了避免内核死锁，单元格类型未更改，因为该单元格存在待处理的输入！请提交您的待处理输入，然后再试一次。"
+
 #: packages/notebook/src/default-toolbar.tsx:141
 msgid "Cut the selected cells"
 msgstr "剪切选中的单元格"
 
 #: packages/notebook/src/default-toolbar.tsx:161
 msgid "Copy the selected cells"
 msgstr "复制选中的单元格"
@@ -6721,15 +6903,15 @@
 msgid "Notebook converted"
 msgstr "笔记本已转换"
 
 #: packages/notebook/src/modestatus.tsx:29
 msgid "Mode: %1"
 msgstr "模式：%1"
 
-#: packages/notebook/src/modestatus.tsx:71 packages/shortcuts-extension/src/components/TopNav.tsx:182
+#: packages/notebook/src/modestatus.tsx:71 packages/shortcuts-extension/src/components/TopNav.tsx:130 packages/shortcuts-extension/src/components/TopNav.tsx:182
 msgid "Command"
 msgstr "命令"
 
 #: packages/notebook/src/modestatus.tsx:72 packages/shortcuts-extension/src/components/ShortcutItem.tsx:61
 msgid "Edit"
 msgstr "编辑"
 
@@ -6745,61 +6927,69 @@
 msgid "Kernel Restarting"
 msgstr "正在重启内核"
 
 #: packages/notebook/src/panel.ts:224
 msgid "The kernel for %1 appears to have died. It will restart automatically."
 msgstr "%1 的内核似乎已经死亡。它将自动重启。"
 
-#: packages/notebook/src/searchprovider.ts:237
+#: packages/notebook/src/searchprovider.ts:234 packages/notebook/src/searchprovider.ts:237
 msgid "Search Cell Outputs"
 msgstr "搜索单元格输出"
 
-#: packages/notebook/src/searchprovider.ts:238
+#: packages/notebook/src/searchprovider.ts:235 packages/notebook/src/searchprovider.ts:238
 msgid "Search in the cell outputs."
 msgstr "在单元格输出中搜索。"
 
-#: packages/notebook/src/searchprovider.ts:245
+#: packages/notebook/src/searchprovider.ts:236
+msgid "Search in the cell outputs (not available when replace options are shown)."
+msgstr "在单元格输出中搜索（在显示替换选项时不可用）。"
+
+#: packages/notebook/src/searchprovider.ts:242 packages/notebook/src/searchprovider.ts:245
 msgid "Search in %1 Selected Cell"
 msgid_plural "Search in %1 Selected Cells"
 msgstr[0] "在 %1 个选中的单元格中搜索"
 
-#: packages/notebook/src/searchprovider.ts:250
+#: packages/notebook/src/searchprovider.ts:247 packages/notebook/src/searchprovider.ts:250
 msgid "Search in %1 Selected Line"
 msgid_plural "Search in %1 Selected Lines"
 msgstr[0] "在选中的 %1 行中搜索"
 
-#: packages/notebook/src/searchprovider.ts:255
+#: packages/notebook/src/searchprovider.ts:252 packages/notebook/src/searchprovider.ts:255
 msgid "Search only in the selected cells or text (depending on edit/command mode)."
 msgstr "只在选定的单元格或文本中搜索(取决于编辑/命令模式)。"
 
-#: packages/notebook/src/searchprovider.ts:523
+#: packages/notebook/src/searchprovider.ts:512 packages/notebook/src/searchprovider.ts:523
 msgid "Searching outputs is expensive and requires to first rendered all outputs. Are you sure you want to search in the cell outputs?"
 msgstr "搜索输出结果是比较耗费资源的，需要先渲染所有输出。您确定要在单元格输出中搜索吗？"
 
+#: packages/notebook/src/searchprovider.ts:515
+msgid "Searching outputs requires you to run all cells and render their outputs. Are you sure you want to search in the cell outputs?"
+msgstr "搜索输出需要运行所有单元格并渲染它们的输出。您确定要在单元格输出中进行搜索吗？"
+
 #: packages/notebook/src/truststatus.tsx:30
 msgid "Notebook trusted: %1 of %2 code cells trusted."
 msgstr "受信任的笔记本：%2 个代码单元格中的 %1 个受到信任。"
 
 #: packages/notebook/src/truststatus.tsx:36
 msgid "Active cell trusted: %1 of %2 code cells trusted."
 msgstr "受信任的活动单元格：%2 个代码单元格中的 %1 个受到信任。"
 
 #: packages/notebook/src/truststatus.tsx:42
 msgid "Notebook not trusted: %1 of %2 code cells trusted."
 msgstr "未受信任的笔记本：%2 个代码单元格中的 %1 个受到信任。"
 
-#: packages/notebook/src/widget.ts:444
+#: packages/notebook/src/widget.ts:444 packages/notebook/src/widget.ts:453 packages/notebook/src/widget.ts:470
 msgid "The notebook is empty. Click the + button on the toolbar to add a new cell."
 msgstr "笔记本为空。点击工具栏上的 + 按钮添加一个新的单元格。"
 
-#: packages/outputarea/src/widget.ts:1096
+#: packages/outputarea/src/widget.ts:1096 packages/outputarea/src/widget.ts:1097 packages/outputarea/src/widget.ts:1128
 msgid "↑↓ for history. Search history with c-↑/c-↓"
 msgstr "使用↑↓键翻阅历史记录。使用c-↑/c-↓键搜索历史记录。"
 
-#: packages/outputarea/src/widget.ts:640
+#: packages/outputarea/src/widget.ts:640 packages/outputarea/src/widget.ts:662
 msgid "Javascript Error: %1"
 msgstr "JavaScript 错误：%1"
 
 #: packages/pluginmanager-extension/src/index.ts:100 packages/pluginmanager-extension/src/index.ts:64 packages/settingeditor-extension/src/index.ts:154
 msgid "Plugin Manager"
 msgstr "插件管理器"
 
@@ -6919,71 +7109,131 @@
 msgid "Handle Local Link"
 msgstr "处理本地链接"
 
 #: packages/rendermime/src/renderers.ts:62
 msgid "This HTML output contains inline scripts. Are you sure that you want to run arbitrary Javascript within your JupyterLab session?"
 msgstr "此 HTML 输出包含内嵌脚本。您确定要在您的 JupyterLab 会话中运行任意的 JavaScript 吗？"
 
-#: packages/rendermime/src/widgets.ts:464
+#: packages/rendermime/src/widgets.ts:464 packages/rendermime/src/widgets.ts:492
 msgid "JavaScript output is disabled in JupyterLab"
 msgstr "JavaScript 输出在 JupyterLab 中被禁用"
 
-#: packages/running-extension/src/index.ts:66
-msgid "Running Terminals and Kernels"
-msgstr "正在运行终端和内核"
-
-#: packages/running-extension/src/index.ts:69
+#: packages/running-extension/src/index.ts:101 packages/running-extension/src/index.ts:69
 msgid "Running Sessions section"
 msgstr "正在运行的会话部分"
 
-#: packages/running-extension/src/index.ts:86
+#: packages/running-extension/src/index.ts:115 packages/running-extension/src/index.ts:86
 msgid "Sessions and Tabs"
 msgstr "会话和标签"
 
-#: packages/running-extension/src/kernels.ts:107
+#: packages/running-extension/src/index.ts:171
+msgid "Tabs and Running Sessions"
+msgstr "选项卡和正在运行的会话"
+
+#: packages/running-extension/src/index.ts:179
+msgid "Search Tabs and Running Sessions"
+msgstr "搜索选项卡和正在运行的会话"
+
+#: packages/running-extension/src/index.ts:184
+msgid "Running"
+msgstr "正在运行"
+
+#: packages/running-extension/src/index.ts:66 packages/running-extension/src/index.ts:96
+msgid "Running Terminals and Kernels"
+msgstr "正在运行终端和内核"
+
+#: packages/running-extension/src/kernels.ts:107 packages/running-extension/src/kernels.tsx:128
 msgid "Unknown Session"
 msgstr "未知会话"
 
-#: packages/running-extension/src/kernels.ts:250
+#: packages/running-extension/src/kernels.ts:250 packages/running-extension/src/kernels.tsx:320
 msgid "%1\n"
 "Path: %2"
 msgstr "%1 路径： %2"
 
-#: packages/running-extension/src/kernels.ts:49
+#: packages/running-extension/src/kernels.ts:49 packages/running-extension/src/kernels.tsx:54
 msgid "Kernels"
 msgstr "内核"
 
-#: packages/running-extension/src/kernels.ts:68
+#: packages/running-extension/src/kernels.ts:68 packages/running-extension/src/kernels.tsx:88
 msgid "Are you sure you want to permanently shut down all running kernels?"
 msgstr "您确定要永久关闭所有正在运行的内核吗？"
 
-#: packages/running-extension/src/kernels.ts:77
+#: packages/running-extension/src/kernels.ts:77 packages/running-extension/src/kernels.tsx:98
 msgid "New Console for Kernel"
 msgstr "内核的新控制台"
 
-#: packages/running-extension/src/kernels.ts:88
+#: packages/running-extension/src/kernels.ts:88 packages/running-extension/src/kernels.tsx:109
 msgid "New Notebook for Kernel"
 msgstr "内核的新笔记本"
 
+#: packages/running-extension/src/kernels.tsx:329
+msgid "No sessions connected"
+msgstr "没有连接的会话"
+
+#: packages/running-extension/src/kernels.tsx:333
+msgid "%1 and %2 more"
+msgstr "%1 和另外 %2"
+
 #: packages/running-extension/src/opentabs.ts:70
 msgid "Open Tabs"
 msgstr "开启的标签页"
 
 #: packages/running-extension/src/opentabs.ts:87
 msgid "Close All"
 msgstr "全部关闭"
 
 #: packages/running-extension/src/opentabs.ts:88
 msgid "Are you sure you want to close all open tabs?"
 msgstr "您确定要关闭所有打开的标签页吗？"
 
-#: packages/running/src/index.tsx:445
+#: packages/running-extension/src/recents.ts:31
+msgid "Recently Closed"
+msgstr "最近关闭"
+
+#: packages/running-extension/src/recents.ts:46
+msgid "Forget"
+msgstr "不记录"
+
+#: packages/running-extension/src/recents.ts:47
+msgid "Forget All"
+msgstr "全部不记录"
+
+#: packages/running-extension/src/recents.ts:48
+msgid "Are you sure you want to clear recently closed tabs?"
+msgstr "您确定要清除最近关闭的选项卡吗？"
+
+#: packages/running/src/index.tsx:366
+msgid "Search"
+msgstr "搜索"
+
+#: packages/running/src/index.tsx:445 packages/running/src/index.tsx:765
 msgid "Refresh List"
 msgstr "刷新列表"
 
+#: packages/running/src/index.tsx:614
+msgid "Switch to List View"
+msgstr "切换到列表视图"
+
+#: packages/running/src/index.tsx:615
+msgid "Switch to Tree View"
+msgstr "切换到树视图"
+
+#: packages/running/src/index.tsx:627
+msgid "Collapse All"
+msgstr "全部折叠"
+
+#: packages/running/src/index.tsx:628
+msgid "Expand All"
+msgstr "全部展开"
+
+#: packages/running/src/index.tsx:885
+msgid "No matches"
+msgstr "没有匹配项"
+
 #: packages/settingeditor-extension/src/index.ts:165
 msgid "JSON Settings Editor"
 msgstr "JSON 设置编辑器"
 
 #: packages/settingeditor-extension/src/index.ts:172 packages/settingeditor-extension/src/index.ts:207 packages/settingeditor-extension/src/index.ts:339 packages/settingeditor/src/pluginlist.tsx:467
 msgid "Settings"
 msgstr "设置"
@@ -7060,18 +7310,14 @@
 msgid "Your changes were not saved."
 msgstr "您的更改没有保存。"
 
 #: packages/settingeditor/src/pluginlist.tsx:454
 msgid "Search settings…"
 msgstr "搜索设置..."
 
-#: packages/settingeditor/src/pluginlist.tsx:461
-msgid "Modified"
-msgstr "已修改"
-
 #: packages/settingeditor/src/pluginlist.tsx:473
 msgid "No items match your search."
 msgstr "没有匹配的搜索项目。"
 
 #: packages/settingeditor/src/raweditor.ts:368
 msgid "System Defaults"
 msgstr "系统默认值"
@@ -7084,31 +7330,43 @@
 msgid "Unsaved changes due to validation error. Continue without saving?"
 msgstr "由于验证错误导致有未保存的改动。继续而不保存？"
 
 #: packages/settingeditor/src/settingseditor.tsx:135
 msgid "Some changes have not been saved. Continue without saving?"
 msgstr "一些改动尚未保存。继续而不保存？"
 
-#: packages/shortcuts-extension/src/components/ShortcutInput.tsx:445
+#: packages/shortcuts-extension/src/components/ShortcutInput.tsx:389 packages/shortcuts-extension/src/components/ShortcutInput.tsx:445 packages/shortcuts-extension/src/components/ShortcutInput.tsx:446
 msgid "press keys"
 msgstr "按下按键"
 
-#: packages/shortcuts-extension/src/components/ShortcutItem.tsx:218
-msgid "Shortcut already in use by %1. Overwrite it?"
-msgstr "快捷键已被 %1 使用。是否覆盖？"
+#: packages/shortcuts-extension/src/components/ShortcutItem.tsx:123
+msgid "(Command label missing)"
+msgstr "(命令标签缺失)"
 
-#: packages/shortcuts-extension/src/components/ShortcutItem.tsx:260 packages/shortcuts-extension/src/components/ShortcutItem.tsx:76
+#: packages/shortcuts-extension/src/components/ShortcutItem.tsx:135 packages/shortcuts-extension/src/components/ShortcutItem.tsx:260 packages/shortcuts-extension/src/components/ShortcutItem.tsx:76 packages/workspaces-extension/src/commands.ts:327
 msgid "Reset"
 msgstr "重置"
 
-#: packages/shortcuts-extension/src/components/ShortcutItem.tsx:332
+#: packages/shortcuts-extension/src/components/ShortcutItem.tsx:147
+msgid "Custom"
+msgstr "自定义"
+
+#: packages/shortcuts-extension/src/components/ShortcutItem.tsx:147
+msgid "Default"
+msgstr "默认"
+
+#: packages/shortcuts-extension/src/components/ShortcutItem.tsx:194 packages/shortcuts-extension/src/components/ShortcutItem.tsx:332
 msgid "or"
 msgstr "或"
 
-#: packages/shortcuts-extension/src/components/ShortcutItem.tsx:416 packages/shortcuts-extension/src/components/ShortcutItem.tsx:66 packages/shortcuts-extension/src/components/ShortcutItem.tsx:71 packages/ui-components/src/components/form.tsx:212
+#: packages/shortcuts-extension/src/components/ShortcutItem.tsx:218 packages/shortcuts-extension/src/components/ShortcutItem.tsx:333
+msgid "Shortcut already in use by %1. Overwrite it?"
+msgstr "快捷键已被 %1 使用。是否覆盖？"
+
+#: packages/shortcuts-extension/src/components/ShortcutItem.tsx:266 packages/shortcuts-extension/src/components/ShortcutItem.tsx:416 packages/shortcuts-extension/src/components/ShortcutItem.tsx:66 packages/shortcuts-extension/src/components/ShortcutItem.tsx:71 packages/ui-components/src/components/form.tsx:212
 msgid "Add"
 msgstr "添加"
 
 #: packages/shortcuts-extension/src/components/ShortcutItem.tsx:51
 msgid "Edit First"
 msgstr "编辑第一个"
 
@@ -7128,59 +7386,83 @@
 msgid "Add another shortcut"
 msgstr "添加另一个快捷键"
 
 #: packages/shortcuts-extension/src/components/ShortcutItem.tsx:77
 msgid "Reset shortcut back to default"
 msgstr "重置快捷键为默认值"
 
-#: packages/shortcuts-extension/src/components/TopNav.tsx:126
-msgid "Toggle Selectors"
-msgstr "切换选择器"
-
-#: packages/shortcuts-extension/src/components/TopNav.tsx:127
-msgid "Toggle command selectors"
-msgstr "切换命令选择器"
-
-#: packages/shortcuts-extension/src/components/TopNav.tsx:136 packages/shortcuts-extension/src/components/TopNav.tsx:92
-msgid "Reset All"
-msgstr "全部重置"
-
-#: packages/shortcuts-extension/src/components/TopNav.tsx:137
-msgid "Reset all shortcuts"
-msgstr "重设所有快速键"
-
-#: packages/shortcuts-extension/src/components/TopNav.tsx:165
+#: packages/shortcuts-extension/src/components/TopNav.tsx:113 packages/shortcuts-extension/src/components/TopNav.tsx:165
 msgid "Search shortcuts"
 msgstr "搜索快捷键..."
 
-#: packages/shortcuts-extension/src/components/TopNav.tsx:168
+#: packages/shortcuts-extension/src/components/TopNav.tsx:117 packages/shortcuts-extension/src/components/TopNav.tsx:168
 msgid "Search…"
 msgstr "搜索…"
 
-#: packages/shortcuts-extension/src/components/TopNav.tsx:181
+#: packages/shortcuts-extension/src/components/TopNav.tsx:126 packages/shortcuts-extension/src/index.ts:159
+msgid "Toggle Selectors"
+msgstr "切换选择器"
+
+#: packages/shortcuts-extension/src/components/TopNav.tsx:127 packages/shortcuts-extension/src/index.ts:160
+msgid "Toggle command selectors"
+msgstr "切换命令选择器"
+
+#: packages/shortcuts-extension/src/components/TopNav.tsx:129 packages/shortcuts-extension/src/components/TopNav.tsx:181
 msgid "Category"
 msgstr "分类"
 
-#: packages/shortcuts-extension/src/components/TopNav.tsx:184
+#: packages/shortcuts-extension/src/components/TopNav.tsx:132 packages/shortcuts-extension/src/components/TopNav.tsx:184
 msgid "Shortcut"
 msgstr "快捷键"
 
-#: packages/shortcuts-extension/src/components/TopNav.tsx:188
+#: packages/shortcuts-extension/src/components/TopNav.tsx:136 packages/shortcuts-extension/src/components/TopNav.tsx:188
 msgid "Selectors"
 msgstr "选择器"
 
-#: packages/shortcuts-extension/src/components/TopNav.tsx:85
+#: packages/shortcuts-extension/src/components/TopNav.tsx:136 packages/shortcuts-extension/src/components/TopNav.tsx:69 packages/shortcuts-extension/src/components/TopNav.tsx:92 packages/shortcuts-extension/src/index.ts:169
+msgid "Reset All"
+msgstr "全部重置"
+
+#: packages/shortcuts-extension/src/components/TopNav.tsx:137 packages/shortcuts-extension/src/index.ts:170
+msgid "Reset all shortcuts"
+msgstr "重设所有快速键"
+
+#: packages/shortcuts-extension/src/components/TopNav.tsx:62 packages/shortcuts-extension/src/components/TopNav.tsx:85
 msgid "Hide Selectors"
 msgstr "隐藏选择器"
 
-#: packages/shortcuts-extension/src/components/TopNav.tsx:86
+#: packages/shortcuts-extension/src/components/TopNav.tsx:63 packages/shortcuts-extension/src/components/TopNav.tsx:86
 msgid "Show Selectors"
 msgstr "显示选择器"
 
-#: packages/shortcuts-extension/src/index.ts:152
+#: packages/shortcuts-extension/src/index.ts:107
+msgid "Edit Keybinding"
+msgstr "编辑按键绑定"
+
+#: packages/shortcuts-extension/src/index.ts:108
+msgid "Edit existing keybinding"
+msgstr "编辑现有的按键绑定"
+
+#: packages/shortcuts-extension/src/index.ts:125
+msgid "Delete Keybinding"
+msgstr "删除按键绑定"
+
+#: packages/shortcuts-extension/src/index.ts:126
+msgid "Delete chosen keybinding"
+msgstr "删除选中的按键绑定"
+
+#: packages/shortcuts-extension/src/index.ts:143
+msgid "Add Keybinding"
+msgstr "添加按键绑定"
+
+#: packages/shortcuts-extension/src/index.ts:144
+msgid "Add new keybinding for existing shortcut target"
+msgstr "为现有的快捷方式目标添加新的按键绑定"
+
+#: packages/shortcuts-extension/src/index.ts:152 packages/shortcuts-extension/src/index.ts:232
 msgid "Note: To disable a system default shortcut,\n"
 "copy it to User Preferences and add the\n"
 "\"disabled\" key, for example:\n"
 "{\n"
 "    \"command\": \"application:activate-next-tab\",\n"
 "    \"keys\": [\n"
 "        \"Ctrl Shift ]\"\n"
@@ -7287,14 +7569,18 @@
 msgid "Terminal %1"
 msgstr "终端 %1"
 
 #: packages/theme-dark-extension/src/index.ts:31
 msgid "JupyterLab Dark"
 msgstr "JupyterLab 暗色"
 
+#: packages/theme-dark-high-contrast-extension/src/index.ts:31
+msgid "JupyterLab Dark High Contrast"
+msgstr "JupyterLab 暗色高对比度"
+
 #: packages/theme-light-extension/src/index.ts:31
 msgid "JupyterLab Light"
 msgstr "JupyterLab 亮色"
 
 #: packages/toc-extension/src/index.ts:113
 msgid "Show output headings"
 msgstr "显示输出标题"
@@ -7371,19 +7657,176 @@
 msgid "side panel actions"
 msgstr "侧面板操作"
 
 #: packages/ui-components/src/components/sidepanel.ts:41
 msgid "side panel content"
 msgstr "侧面板内容"
 
-#: packages/ui-components/src/components/toolbar.tsx:1140
+#: packages/ui-components/src/components/toolbar.tsx:1140 packages/ui-components/src/components/toolbar.tsx:1180 packages/ui-components/src/components/toolbar.tsx:1191 packages/ui-components/src/components/toolbar.tsx:1192
 msgid "More commands"
 msgstr "更多命令"
 
 #: packages/ui-components/src/icon/widgets/tabbarsvg.ts:51
 msgid "Close %1"
 msgstr "关闭 %1"
 
 #: packages/ui-components/src/icon/widgets/tabbarsvg.ts:52
 msgid "Close tab"
 msgstr "关闭标签页"
 
+#: packages/workspaces-extension/src/commands.ts:104
+msgid "Naming the workspace will create a unique URL. The name may contain letters, numbers, hyphens (-), and underscores (_)."
+msgstr "为工作区命名将创建唯一的 URL。名称可以包含字母、数字、连字符（-）和下划线（_）。"
+
+#: packages/workspaces-extension/src/commands.ts:120
+msgid "workspace-name"
+msgstr "工作区名称"
+
+#: packages/workspaces-extension/src/commands.ts:132
+msgid "Open Workspace"
+msgstr "打开工作区"
+
+#: packages/workspaces-extension/src/commands.ts:133
+msgid "Open Workspace…"
+msgstr "打开工作区…"
+
+#: packages/workspaces-extension/src/commands.ts:140
+msgid "Choose Workspace To Open"
+msgstr "选择要打开的工作区"
+
+#: packages/workspaces-extension/src/commands.ts:141
+msgid "Choose an existing workspace to open."
+msgstr "选择要打开的现有工作区。"
+
+#: packages/workspaces-extension/src/commands.ts:143 packages/workspaces-extension/src/commands.ts:180 packages/workspaces-extension/src/commands.ts:243 packages/workspaces-extension/src/commands.ts:406
+msgid "Choose"
+msgstr "选择"
+
+#: packages/workspaces-extension/src/commands.ts:169
+msgid "Delete Workspace…"
+msgstr "删除工作区..."
+
+#: packages/workspaces-extension/src/commands.ts:177
+msgid "Choose Workspace To Delete"
+msgstr "选择要删除的工作区"
+
+#: packages/workspaces-extension/src/commands.ts:178
+msgid "Choose an existing workspace to delete."
+msgstr "选择要删除的现有工作区。"
+
+#: packages/workspaces-extension/src/commands.ts:192
+msgid "Delete workspace"
+msgstr "删除工作区"
+
+#: packages/workspaces-extension/src/commands.ts:193
+msgid "Deleting workspace \"%1\" will also delete its URL. A deleted workspace cannot be recovered."
+msgstr "删除工作区 \"%1\" 将同时删除其 URL。已删除的工作区无法恢复。"
+
+#: packages/workspaces-extension/src/commands.ts:211
+msgid "Create New Workspace…"
+msgstr "创建新的工作区..."
+
+#: packages/workspaces-extension/src/commands.ts:217
+msgid "Create New Workspace"
+msgstr "创建新的工作区"
+
+#: packages/workspaces-extension/src/commands.ts:218
+msgid "Create"
+msgstr "创建"
+
+#: packages/workspaces-extension/src/commands.ts:233
+msgid "Clone Workspace…"
+msgstr "克隆工作区..."
+
+#: packages/workspaces-extension/src/commands.ts:240
+msgid "Choose Workspace To Clone"
+msgstr "选择要克隆的工作区"
+
+#: packages/workspaces-extension/src/commands.ts:241
+msgid "Choose an existing workspace to clone."
+msgstr "选择要克隆的现有工作区。"
+
+#: packages/workspaces-extension/src/commands.ts:252
+msgid "Clone Workspace"
+msgstr "克隆工作区"
+
+#: packages/workspaces-extension/src/commands.ts:253
+msgid "%1-clone"
+msgstr "%1-副本"
+
+#: packages/workspaces-extension/src/commands.ts:254
+msgid "Clone"
+msgstr "克隆"
+
+#: packages/workspaces-extension/src/commands.ts:273
+msgid "Rename Workspace…"
+msgstr "重命名工作区..."
+
+#: packages/workspaces-extension/src/commands.ts:283
+msgid "Rename Workspace"
+msgstr "重命名工作区"
+
+#: packages/workspaces-extension/src/commands.ts:304
+msgid "Reset Workspace…"
+msgstr "重置工作区..."
+
+#: packages/workspaces-extension/src/commands.ts:318
+msgid "Reset Workspace"
+msgstr "重置工作区"
+
+#: packages/workspaces-extension/src/commands.ts:319
+msgid "Resetting workspace %2 will close its %1 tab and return to default layout."
+msgid_plural "Resetting workspace %2 will close its %1 tabs and return to default layout."
+msgstr[0] "重置工作区 %2 将关闭其 %1 选项卡并返回默认布局。"
+
+#: packages/workspaces-extension/src/commands.ts:354
+msgid "Import Workspace…"
+msgstr "导入工作区…"
+
+#: packages/workspaces-extension/src/commands.ts:359
+msgid "Select Workspace Files to Import"
+msgstr "选择要导入的工作区文件"
+
+#: packages/workspaces-extension/src/commands.ts:364
+msgid "You choose one or more workspace files to import. A Jupyter Workspace File has %1 extension."
+msgstr "您选择一个或多个要导入的工作区文件。Jupyter 工作区文件的扩展名为 %1。"
+
+#: packages/workspaces-extension/src/commands.ts:390
+msgid "Export Workspace…"
+msgstr "导出工作区..."
+
+#: packages/workspaces-extension/src/commands.ts:403
+msgid "Choose Workspace To Export"
+msgstr "选择要导出的工作区"
+
+#: packages/workspaces-extension/src/commands.ts:404
+msgid "Choose an existing workspace to export."
+msgstr "选择要导出的现有工作区。"
+
+#: packages/workspaces-extension/src/commands.ts:417
+msgid "Choose Workspace Export Directory"
+msgstr "选择工作区导出目录"
+
+#: packages/workspaces-extension/src/commands.ts:420
+msgid "The \"%1\" workspace will be saved in the chosen directory as \"%1%2\"."
+msgstr "工作区 \"%1\" 将以 \"%1%2\" 的名称保存在所选择的目录中。"
+
+#: packages/workspaces-extension/src/commands.ts:472 packages/workspaces-extension/src/sidebar.ts:81
+msgid "Workspaces"
+msgstr "工作区"
+
+#: packages/workspaces-extension/src/commands.ts:586
+msgid "Path to save the workspace in"
+msgstr "保存工作区的路径"
+
+#: packages/workspaces-extension/src/sidebar.ts:100
+msgid "Delete All"
+msgstr "全部刪除"
+
+#: packages/workspaces-extension/src/sidebar.ts:101
+msgid "Are you sure you want to delete all workspaces? Deleted workspaces cannot be recovered."
+msgstr "您确定要删除所有工作区吗？已删除的工作区无法恢复。"
+
+#: packages/workspaces-extension/src/sidebar.ts:69
+msgid "%1 workspace with %2 tabs, last modified on %3"
+msgstr "%1 工作区包含 %2 个选项卡，上次修改时间为 %3"
+
```

### Comparing `jupyterlab_language_pack_zh_cn-4.1.post2/jupyterlab_language_pack_zh_CN/locale/zh_CN/LC_MESSAGES/jupyterlab_git.po` & `jupyterlab_language_pack_zh_cn-4.2.post0/jupyterlab_language_pack_zh_CN/locale/zh_CN/LC_MESSAGES/jupyterlab_git.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_zh_cn-4.1.post2/jupyterlab_language_pack_zh_CN/locale/zh_CN/LC_MESSAGES/jupyterlab_lsp.po` & `jupyterlab_language_pack_zh_cn-4.2.post0/jupyterlab_language_pack_zh_CN/locale/zh_CN/LC_MESSAGES/jupyterlab_lsp.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_zh_cn-4.1.post2/jupyterlab_language_pack_zh_CN/locale/zh_CN/LC_MESSAGES/jupyterlab_recents.po` & `jupyterlab_language_pack_zh_cn-4.2.post0/jupyterlab_language_pack_zh_CN/locale/zh_CN/LC_MESSAGES/jupyterlab_recents.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_zh_cn-4.1.post2/jupyterlab_language_pack_zh_CN/locale/zh_CN/LC_MESSAGES/jupyterlab_search_replace.po` & `jupyterlab_language_pack_zh_cn-4.2.post0/jupyterlab_language_pack_zh_CN/locale/zh_CN/LC_MESSAGES/jupyterlab_search_replace.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_zh_cn-4.1.post2/jupyterlab_language_pack_zh_CN/locale/zh_CN/LC_MESSAGES/jupyterlab_spreadsheet_editor.po` & `jupyterlab_language_pack_zh_cn-4.2.post0/jupyterlab_language_pack_zh_CN/locale/zh_CN/LC_MESSAGES/jupyterlab_spreadsheet_editor.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_zh_cn-4.1.post2/jupyterlab_language_pack_zh_CN/locale/zh_CN/LC_MESSAGES/jupyterlab_tour.po` & `jupyterlab_language_pack_zh_cn-4.2.post0/jupyterlab_language_pack_zh_CN/locale/zh_CN/LC_MESSAGES/jupyterlab_tour.po`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 "X-Crowdin-Project: jupyterlab\n"
 "X-Crowdin-Project-ID: 409874\n"
 "X-Crowdin-Language: zh-CN\n"
 "X-Crowdin-File: /main/extensions/jupyterlab_tour/locale/jupyterlab_tour.pot\n"
 "X-Crowdin-File-ID: 205\n"
 "Language-Team: Chinese Simplified\n"
 "Language: zh_CN\n"
-"PO-Revision-Date: 2023-11-10 02:46\n"
+"PO-Revision-Date: 2024-03-29 11:18\n"
 
 #: /schema/user-tours.json:/description
 msgctxt "schema"
 msgid "Configuration for user-defined tours. This schema is generated from https://github.com/gilbarbara/react-joyride/blob/master/types/index.d.ts"
 msgstr "用户定义的向导配置。这个模式（schema）生成自 https://github.com/gilmabita/react-joyride/blob/master/types/index.d.ts"
 
 #: /schema/user-tours.json:/jupyter.lab.setting-icon-label
@@ -135,15 +135,15 @@
 msgid "Settings"
 msgstr "设置"
 
 #: src/defaults.tsx:138
 msgid ": common settings and an advanced settings editor"
 msgstr ": 常见设置和高级设置编辑器"
 
-#: src/defaults.tsx:141 src/defaults.tsx:636 src/plugin.tsx:143
+#: src/defaults.tsx:141 src/defaults.tsx:636 src/plugin.tsx:143 src/plugin.tsx:144
 msgid "Help"
 msgstr "帮助"
 
 #: src/defaults.tsx:142 src/defaults.tsx:637
 msgid ": help links"
 msgstr ": 帮助链接"
 
@@ -395,42 +395,42 @@
 msgid "Validation errors found: fix them in Advanced Settings"
 msgstr "发现验证错误：请在高级设置中进行修复"
 
 #: src/notebookTourManager.ts:124
 msgid "Error encountered adding notebook tour %1 (%2)"
 msgstr "添加笔记本导览 %1 (%2) 时遇到错误"
 
-#: src/plugin.tsx:104
+#: src/plugin.tsx:100 src/plugin.tsx:99
+msgid "Launch a Tour"
+msgstr "启动导览"
+
+#: src/plugin.tsx:104 src/plugin.tsx:105
 msgid "Launch a tour.\n"
 "If no id provided, prompt the user.\n"
 "Arguments {id: Tour ID}"
 msgstr "启动导览。\n"
 "如果未提供 id，则提示用户。\n"
 "参数 {id: Tour ID}"
 
-#: src/plugin.tsx:115
+#: src/plugin.tsx:115 src/plugin.tsx:116
 msgid "Choose a tour"
 msgstr "选择一个导览"
 
-#: src/plugin.tsx:132
+#: src/plugin.tsx:132 src/plugin.tsx:133
 msgid "Add a tour"
 msgstr "添加一个导览"
 
-#: src/plugin.tsx:133
+#: src/plugin.tsx:133 src/plugin.tsx:134
 msgid "Add a tour and returns it.\n"
 "Arguments {tour: ITour}\n"
 "Returns `null` if a failure occurs."
 msgstr "添加一个导览并返回它。\n"
 "参数 {tour: ITour}\n"
 "如果出现错误，则返回 `null`。"
 
-#: src/plugin.tsx:99
-msgid "Launch a Tour"
-msgstr "启动导览"
-
 #: src/tourManager.ts:142
 msgid "Fail to add tour '%1' (%2)"
 msgstr "添加向导「%1」（%2）失败"
 
 #: src/tourManager.ts:172
 msgid "Error creating new tour. TourHandler id's must be unique.\n"
 "Tutorial with the id: '%1' already exists."
```

### Comparing `jupyterlab_language_pack_zh_cn-4.1.post2/jupyterlab_language_pack_zh_CN/locale/zh_CN/LC_MESSAGES/jupyterlab_widgets.po` & `jupyterlab_language_pack_zh_cn-4.2.post0/jupyterlab_language_pack_zh_CN/locale/zh_CN/LC_MESSAGES/jupyterlab_widgets.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_zh_cn-4.1.post2/jupyterlab_language_pack_zh_CN/locale/zh_CN/LC_MESSAGES/jupytext.po` & `jupyterlab_language_pack_zh_cn-4.2.post0/jupyterlab_language_pack_zh_CN/locale/zh_CN/LC_MESSAGES/jupytext.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_zh_cn-4.1.post2/jupyterlab_language_pack_zh_CN/locale/zh_CN/LC_MESSAGES/nbdime.po` & `jupyterlab_language_pack_zh_cn-4.2.post0/jupyterlab_language_pack_zh_CN/locale/zh_CN/LC_MESSAGES/nbdime.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_zh_cn-4.1.post2/jupyterlab_language_pack_zh_CN/locale/zh_CN/LC_MESSAGES/notebook.po` & `jupyterlab_language_pack_zh_cn-4.2.post0/jupyterlab_language_pack_zh_CN/locale/zh_CN/LC_MESSAGES/notebook.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_zh_cn-4.1.post2/jupyterlab_language_pack_zh_CN/locale/zh_CN/LC_MESSAGES/retrolab.po` & `jupyterlab_language_pack_zh_cn-4.2.post0/jupyterlab_language_pack_zh_CN/locale/zh_CN/LC_MESSAGES/retrolab.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_zh_cn-4.1.post2/jupyterlab_language_pack_zh_CN/locale/zh_CN/LC_MESSAGES/spellchecker.po` & `jupyterlab_language_pack_zh_cn-4.2.post0/jupyterlab_language_pack_zh_CN/locale/zh_CN/LC_MESSAGES/spellchecker.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_zh_cn-4.1.post2/.gitignore` & `jupyterlab_language_pack_zh_cn-4.2.post0/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_zh_cn-4.1.post2/LICENSE.txt` & `jupyterlab_language_pack_zh_cn-4.2.post0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_zh_cn-4.1.post2/pyproject.toml` & `jupyterlab_language_pack_zh_cn-4.2.post0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_zh_cn-4.1.post2/PKG-INFO` & `jupyterlab_language_pack_zh_cn-4.2.post0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: jupyterlab-language-pack-zh-CN
-Version: 4.1.post2
+Version: 4.2.post0
 Summary: JupyterLab Chinese (Simplified, China) Language Pack
 Project-URL: homepage, https://github.com/jupyterlab/language-packs
 Author-email: Project Jupyter Contributors <jupyter@googlegroups.com>
 License: Copyright (c) 2023 Project Jupyter Contributors
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
```

