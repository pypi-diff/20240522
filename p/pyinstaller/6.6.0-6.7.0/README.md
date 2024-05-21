# Comparing `tmp/pyinstaller-6.6.0.tar.gz` & `tmp/pyinstaller-6.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyinstaller-6.6.0.tar", last modified: Sat Apr 13 09:53:11 2024, max compression
+gzip compressed data, was "pyinstaller-6.7.0.tar", last modified: Tue May 21 22:38:37 2024, max compression
```

## Comparing `pyinstaller-6.6.0.tar` & `pyinstaller-6.7.0.tar`

### file list

```diff
@@ -1,1653 +1,1654 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.300429 pyinstaller-6.6.0/
--rwxrwxrwx   0 root         (0) root         (0)      339 2023-09-30 18:27:19.000000 pyinstaller-6.6.0/.dockerignore
--rwxrwxrwx   0 root         (0) root         (0)      230 2023-09-30 18:27:19.000000 pyinstaller-6.6.0/.editorconfig
--rwxrwxrwx   0 root         (0) root         (0)      813 2023-09-30 18:27:19.000000 pyinstaller-6.6.0/.gitattributes
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:10.775084 pyinstaller-6.6.0/.github/
--rwxrwxrwx   0 root         (0) root         (0)      100 2023-09-30 18:27:19.000000 pyinstaller-6.6.0/.github/CONTRIBUTING.md
--rwxrwxrwx   0 root         (0) root         (0)       17 2023-09-30 18:27:19.000000 pyinstaller-6.6.0/.github/FUNDING.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:10.776875 pyinstaller-6.6.0/.github/ISSUE_TEMPLATE/
--rwxrwxrwx   0 root         (0) root         (0)     8019 2024-02-27 22:30:02.000000 pyinstaller-6.6.0/.github/ISSUE_TEMPLATE/antivirus.md
--rwxrwxrwx   0 root         (0) root         (0)      286 2023-09-30 18:27:19.000000 pyinstaller-6.6.0/.github/ISSUE_TEMPLATE/blank.md
--rwxrwxrwx   0 root         (0) root         (0)     2764 2023-09-30 18:27:19.000000 pyinstaller-6.6.0/.github/ISSUE_TEMPLATE/bug_report.md
--rwxrwxrwx   0 root         (0) root         (0)      404 2023-09-30 18:27:19.000000 pyinstaller-6.6.0/.github/ISSUE_TEMPLATE/config.yml
--rwxrwxrwx   0 root         (0) root         (0)     1016 2023-09-30 18:27:19.000000 pyinstaller-6.6.0/.github/ISSUE_TEMPLATE/feature_request.md
--rwxrwxrwx   0 root         (0) root         (0)      193 2023-09-30 18:27:19.000000 pyinstaller-6.6.0/.github/SECURITY.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:10.779374 pyinstaller-6.6.0/.github/workflows/
--rwxrwxrwx   0 root         (0) root         (0)      387 2024-03-10 15:20:02.000000 pyinstaller-6.6.0/.github/workflows/cancel.yml
--rwxrwxrwx   0 root         (0) root         (0)     8040 2024-03-24 20:46:04.000000 pyinstaller-6.6.0/.github/workflows/ci.yml
--rwxrwxrwx   0 root         (0) root         (0)      997 2024-03-24 20:46:04.000000 pyinstaller-6.6.0/.github/workflows/lint.yml
--rwxrwxrwx   0 root         (0) root         (0)      391 2024-03-24 20:46:04.000000 pyinstaller-6.6.0/.github/workflows/lock-threads.yml
--rwxrwxrwx   0 root         (0) root         (0)      463 2024-03-24 20:46:04.000000 pyinstaller-6.6.0/.github/workflows/validate-new-news.yml
--rwxrwxrwx   0 root         (0) root         (0)      679 2024-03-24 20:46:04.000000 pyinstaller-6.6.0/.github/workflows/wheel-builder.yml
--rwxrwxrwx   0 root         (0) root         (0)     2077 2023-09-30 18:27:19.000000 pyinstaller-6.6.0/.gitignore
--rwxrwxrwx   0 root         (0) root         (0)     1089 2023-09-30 18:27:19.000000 pyinstaller-6.6.0/.pylintrc
--rwxrwxrwx   0 root         (0) root         (0)      403 2023-09-30 18:27:19.000000 pyinstaller-6.6.0/.pyup.yml
--rwxrwxrwx   0 root         (0) root         (0)      276 2023-09-30 18:27:19.000000 pyinstaller-6.6.0/.readthedocs.yml
--rwxrwxrwx   0 root         (0) root         (0)      646 2023-09-30 18:27:19.000000 pyinstaller-6.6.0/.yapfignore
--rwxrwxrwx   0 root         (0) root         (0)    32138 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/COPYING.txt
--rwxrwxrwx   0 root         (0) root         (0)      856 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/MANIFEST.in
--rwxrwxrwx   0 root         (0) root         (0)     8277 2024-04-13 09:53:11.300344 pyinstaller-6.6.0/PKG-INFO
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:10.782670 pyinstaller-6.6.0/PyInstaller/
--rwxrwxrwx   0 root         (0) root         (0)     2983 2024-04-13 09:45:27.000000 pyinstaller-6.6.0/PyInstaller/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     8580 2024-02-10 12:19:40.000000 pyinstaller-6.6.0/PyInstaller/__main__.py
--rwxrwxrwx   0 root         (0) root         (0)     1821 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/_recursion_too_deep_message.py
--rwxrwxrwx   0 root         (0) root         (0)     3911 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/_shared_with_waf.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:10.783913 pyinstaller-6.6.0/PyInstaller/archive/
--rwxrwxrwx   0 root         (0) root         (0)       22 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/archive/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      747 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/archive/pyz_crypto.py
--rwxrwxrwx   0 root         (0) root         (0)     8489 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/archive/readers.py
--rwxrwxrwx   0 root         (0) root         (0)    18052 2024-04-04 21:05:01.000000 pyinstaller-6.6.0/PyInstaller/archive/writers.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:10.754100 pyinstaller-6.6.0/PyInstaller/bootloader/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:10.787859 pyinstaller-6.6.0/PyInstaller/bootloader/Darwin-64bit/
--rwxrwxrwx   0 root         (0) root         (0)   189024 2024-04-13 09:51:54.000000 pyinstaller-6.6.0/PyInstaller/bootloader/Darwin-64bit/run
--rwxrwxrwx   0 root         (0) root         (0)   189000 2024-04-13 09:51:54.000000 pyinstaller-6.6.0/PyInstaller/bootloader/Darwin-64bit/run_d
--rwxrwxrwx   0 root         (0) root         (0)   191800 2024-04-13 09:51:54.000000 pyinstaller-6.6.0/PyInstaller/bootloader/Darwin-64bit/runw
--rwxrwxrwx   0 root         (0) root         (0)   224712 2024-04-13 09:51:54.000000 pyinstaller-6.6.0/PyInstaller/bootloader/Darwin-64bit/runw_d
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:10.792992 pyinstaller-6.6.0/PyInstaller/bootloader/Windows-32bit-intel/
--rwxrwxrwx   0 root         (0) root         (0)   226304 2024-04-13 09:51:54.000000 pyinstaller-6.6.0/PyInstaller/bootloader/Windows-32bit-intel/run.exe
--rwxrwxrwx   0 root         (0) root         (0)   230912 2024-04-13 09:51:54.000000 pyinstaller-6.6.0/PyInstaller/bootloader/Windows-32bit-intel/run_d.exe
--rwxrwxrwx   0 root         (0) root         (0)   226304 2024-04-13 09:51:54.000000 pyinstaller-6.6.0/PyInstaller/bootloader/Windows-32bit-intel/runw.exe
--rwxrwxrwx   0 root         (0) root         (0)   231424 2024-04-13 09:51:54.000000 pyinstaller-6.6.0/PyInstaller/bootloader/Windows-32bit-intel/runw_d.exe
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:10.798150 pyinstaller-6.6.0/PyInstaller/bootloader/Windows-64bit-intel/
--rwxrwxrwx   0 root         (0) root         (0)   270336 2024-04-13 09:51:54.000000 pyinstaller-6.6.0/PyInstaller/bootloader/Windows-64bit-intel/run.exe
--rwxrwxrwx   0 root         (0) root         (0)   275456 2024-04-13 09:51:54.000000 pyinstaller-6.6.0/PyInstaller/bootloader/Windows-64bit-intel/run_d.exe
--rwxrwxrwx   0 root         (0) root         (0)   270336 2024-04-13 09:51:54.000000 pyinstaller-6.6.0/PyInstaller/bootloader/Windows-64bit-intel/runw.exe
--rwxrwxrwx   0 root         (0) root         (0)   275456 2024-04-13 09:51:54.000000 pyinstaller-6.6.0/PyInstaller/bootloader/Windows-64bit-intel/runw_d.exe
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:10.801356 pyinstaller-6.6.0/PyInstaller/bootloader/images/
--rwxrwxrwx   0 root         (0) root         (0)   106001 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/bootloader/images/icon-console.icns
--rwxrwxrwx   0 root         (0) root         (0)    59521 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/bootloader/images/icon-console.ico
--rwxrwxrwx   0 root         (0) root         (0)   110199 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/bootloader/images/icon-windowed.icns
--rwxrwxrwx   0 root         (0) root         (0)    60690 2023-10-12 17:16:03.000000 pyinstaller-6.6.0/PyInstaller/bootloader/images/icon-windowed.ico
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:10.805326 pyinstaller-6.6.0/PyInstaller/building/
--rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/building/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    65488 2024-04-04 21:05:01.000000 pyinstaller-6.6.0/PyInstaller/building/api.py
--rwxrwxrwx   0 root         (0) root         (0)    55894 2024-04-13 09:44:10.000000 pyinstaller-6.6.0/PyInstaller/building/build_main.py
--rwxrwxrwx   0 root         (0) root         (0)    17435 2024-04-04 21:05:01.000000 pyinstaller-6.6.0/PyInstaller/building/datastruct.py
--rwxrwxrwx   0 root         (0) root         (0)     4015 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/building/icon.py
--rwxrwxrwx   0 root         (0) root         (0)    35246 2024-04-04 21:05:01.000000 pyinstaller-6.6.0/PyInstaller/building/makespec.py
--rwxrwxrwx   0 root         (0) root         (0)    41573 2024-04-04 21:05:01.000000 pyinstaller-6.6.0/PyInstaller/building/osx.py
--rwxrwxrwx   0 root         (0) root         (0)    22800 2023-11-26 23:20:35.000000 pyinstaller-6.6.0/PyInstaller/building/splash.py
--rwxrwxrwx   0 root         (0) root         (0)     7453 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/building/splash_templates.py
--rwxrwxrwx   0 root         (0) root         (0)     3146 2024-04-04 21:05:01.000000 pyinstaller-6.6.0/PyInstaller/building/templates.py
--rwxrwxrwx   0 root         (0) root         (0)    36047 2024-04-04 21:05:01.000000 pyinstaller-6.6.0/PyInstaller/building/utils.py
--rwxrwxrwx   0 root         (0) root         (0)    30624 2024-04-04 21:05:01.000000 pyinstaller-6.6.0/PyInstaller/compat.py
--rwxrwxrwx   0 root         (0) root         (0)     1852 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/config.py
--rwxrwxrwx   0 root         (0) root         (0)     4160 2023-11-26 23:20:35.000000 pyinstaller-6.6.0/PyInstaller/configure.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:10.808068 pyinstaller-6.6.0/PyInstaller/depend/
--rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/depend/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    49122 2024-03-09 19:48:33.000000 pyinstaller-6.6.0/PyInstaller/depend/analysis.py
--rwxrwxrwx   0 root         (0) root         (0)    40731 2024-02-10 12:19:40.000000 pyinstaller-6.6.0/PyInstaller/depend/bindepend.py
--rwxrwxrwx   0 root         (0) root         (0)    12952 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/depend/bytecode.py
--rwxrwxrwx   0 root         (0) root         (0)    13110 2024-03-09 19:48:33.000000 pyinstaller-6.6.0/PyInstaller/depend/dylib.py
--rwxrwxrwx   0 root         (0) root         (0)    25462 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/depend/imphook.py
--rwxrwxrwx   0 root         (0) root         (0)    20617 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/depend/imphookapi.py
--rwxrwxrwx   0 root         (0) root         (0)    16550 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/depend/utils.py
--rwxrwxrwx   0 root         (0) root         (0)     2987 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/exceptions.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:10.808398 pyinstaller-6.6.0/PyInstaller/fake-modules/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:10.809478 pyinstaller-6.6.0/PyInstaller/fake-modules/_pyi_rth_utils/
--rwxrwxrwx   0 root         (0) root         (0)     1413 2024-02-10 12:19:40.000000 pyinstaller-6.6.0/PyInstaller/fake-modules/_pyi_rth_utils/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    11564 2024-02-10 12:19:40.000000 pyinstaller-6.6.0/PyInstaller/fake-modules/_pyi_rth_utils/_win32.py
--rwxrwxrwx   0 root         (0) root         (0)     4204 2024-03-09 19:48:33.000000 pyinstaller-6.6.0/PyInstaller/fake-modules/_pyi_rth_utils/qt.py
--rwxrwxrwx   0 root         (0) root         (0)     2262 2023-11-11 15:22:30.000000 pyinstaller-6.6.0/PyInstaller/fake-modules/_pyi_rth_utils/tempfile.py
--rwxrwxrwx   0 root         (0) root         (0)     8519 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/fake-modules/pyi_splash.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:10.899660 pyinstaller-6.6.0/PyInstaller/hooks/
--rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      845 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PIL.Image.py
--rwxrwxrwx   0 root         (0) root         (0)      589 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PIL.ImageFilter.py
--rwxrwxrwx   0 root         (0) root         (0)      773 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PIL.SpiderImagePlugin.py
--rwxrwxrwx   0 root         (0) root         (0)     1100 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PIL.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.QAxContainer.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.Qsci.py
--rwxrwxrwx   0 root         (0) root         (0)     1274 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.Qt.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.Qt3DAnimation.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.Qt3DCore.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.Qt3DExtras.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.Qt3DInput.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.Qt3DLogic.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.Qt3DRender.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.QtBluetooth.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.QtChart.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.QtCore.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.QtDBus.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.QtDataVisualization.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.QtDesigner.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.QtGui.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.QtHelp.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.QtLocation.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.QtMacExtras.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.QtMultimedia.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.QtMultimediaWidgets.py
--rwxrwxrwx   0 root         (0) root         (0)      710 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.QtNetwork.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.QtNetworkAuth.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.QtNfc.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.QtOpenGL.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.QtPositioning.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.QtPrintSupport.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.QtPurchasing.py
--rwxrwxrwx   0 root         (0) root         (0)      764 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.QtQml.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.QtQuick.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.QtQuick3D.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.QtQuickWidgets.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.QtRemoteObjects.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.QtScript.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.QtSensors.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.QtSerialPort.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.QtSql.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.QtSvg.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.QtTest.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.QtTextToSpeech.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.QtWebChannel.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.QtWebEngine.py
--rwxrwxrwx   0 root         (0) root         (0)      995 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.QtWebEngineCore.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.QtWebEngineWidgets.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.QtWebKit.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.QtWebKitWidgets.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.QtWebSockets.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.QtWidgets.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.QtWinExtras.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.QtX11Extras.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.QtXml.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.QtXmlPatterns.py
--rwxrwxrwx   0 root         (0) root         (0)     1182 2024-03-09 19:48:33.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.py
--rwxrwxrwx   0 root         (0) root         (0)      979 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.uic.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.QAxContainer.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.Qsci.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.Qt3DAnimation.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.Qt3DCore.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.Qt3DExtras.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.Qt3DInput.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.Qt3DLogic.py
--rwxrwxrwx   0 root         (0) root         (0)      670 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.Qt3DRender.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.QtBluetooth.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.QtCharts.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.QtCore.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.QtDBus.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.QtDataVisualization.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.QtDesigner.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.QtGui.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.QtHelp.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.QtMultimedia.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.QtMultimediaWidgets.py
--rwxrwxrwx   0 root         (0) root         (0)      710 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.QtNetwork.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.QtNetworkAuth.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.QtNfc.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.QtOpenGL.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.QtOpenGLWidgets.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.QtPdf.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.QtPdfWidgets.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.QtPositioning.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.QtPrintSupport.py
--rwxrwxrwx   0 root         (0) root         (0)      764 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.QtQml.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.QtQuick.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.QtQuick3D.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.QtQuickWidgets.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.QtRemoteObjects.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.QtSensors.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.QtSerialPort.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.QtSpatialAudio.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.QtSql.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.QtSvg.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.QtSvgWidgets.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.QtTest.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.QtTextToSpeech.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.QtWebChannel.py
--rwxrwxrwx   0 root         (0) root         (0)     1351 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.QtWebEngineCore.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.QtWebEngineQuick.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.QtWebEngineWidgets.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.QtWebSockets.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.QtWidgets.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.QtXml.py
--rwxrwxrwx   0 root         (0) root         (0)     1025 2024-03-09 19:48:33.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.py
--rwxrwxrwx   0 root         (0) root         (0)      979 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.uic.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.Qt3DAnimation.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.Qt3DCore.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.Qt3DExtras.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.Qt3DInput.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.Qt3DLogic.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.Qt3DRender.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.QtAxContainer.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.QtCharts.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.QtConcurrent.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.QtCore.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.QtDataVisualization.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.QtGui.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.QtHelp.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.QtLocation.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.QtMacExtras.py
--rwxrwxrwx   0 root         (0) root         (0)      979 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.QtMultimedia.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.QtMultimediaWidgets.py
--rwxrwxrwx   0 root         (0) root         (0)      714 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.QtNetwork.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.QtOpenGL.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.QtOpenGLFunctions.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.QtPositioning.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.QtPrintSupport.py
--rwxrwxrwx   0 root         (0) root         (0)      804 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.QtQml.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.QtQuick.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.QtQuickControls2.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.QtQuickWidgets.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.QtRemoteObjects.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.QtScript.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.QtScriptTools.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.QtScxml.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.QtSensors.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.QtSerialPort.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.QtSql.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.QtSvg.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.QtTest.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.QtTextToSpeech.py
--rwxrwxrwx   0 root         (0) root         (0)      710 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.QtUiTools.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.QtWebChannel.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.QtWebEngine.py
--rwxrwxrwx   0 root         (0) root         (0)     1003 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.QtWebEngineCore.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.QtWebEngineWidgets.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.QtWebKit.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.QtWebKitWidgets.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.QtWebSockets.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.QtWidgets.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.QtWinExtras.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.QtX11Extras.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.QtXml.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.QtXmlPatterns.py
--rwxrwxrwx   0 root         (0) root         (0)      972 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.Qwt5.py
--rwxrwxrwx   0 root         (0) root         (0)     1141 2024-03-09 19:48:33.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.Qt3DAnimation.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.Qt3DCore.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.Qt3DExtras.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.Qt3DInput.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.Qt3DLogic.py
--rwxrwxrwx   0 root         (0) root         (0)     1122 2024-04-13 09:44:10.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.Qt3DRender.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtAxContainer.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtBluetooth.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtCharts.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtConcurrent.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtCore.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtDBus.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtDataVisualization.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtDesigner.py
--rwxrwxrwx   0 root         (0) root         (0)      628 2023-11-04 13:41:36.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtGraphs.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtGui.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtHelp.py
--rwxrwxrwx   0 root         (0) root         (0)      837 2023-10-12 17:16:14.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtHttpServer.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtLocation.py
--rwxrwxrwx   0 root         (0) root         (0)      981 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtMultimedia.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtMultimediaWidgets.py
--rwxrwxrwx   0 root         (0) root         (0)      714 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtNetwork.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtNetworkAuth.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtNfc.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtOpenGL.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtOpenGLWidgets.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtPdf.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtPdfWidgets.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtPositioning.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtPrintSupport.py
--rwxrwxrwx   0 root         (0) root         (0)      768 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtQml.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtQuick.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtQuick3D.py
--rwxrwxrwx   0 root         (0) root         (0)      671 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtQuickControls2.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtQuickWidgets.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtRemoteObjects.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtScxml.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtSensors.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtSerialBus.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtSerialPort.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtSpatialAudio.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtSql.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtStateMachine.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtSvg.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtSvgWidgets.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtTest.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtTextToSpeech.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtUiTools.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtWebChannel.py
--rwxrwxrwx   0 root         (0) root         (0)     1410 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtWebEngineCore.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtWebEngineQuick.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtWebEngineWidgets.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtWebSockets.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtWidgets.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtXml.py
--rwxrwxrwx   0 root         (0) root         (0)     1279 2024-03-09 19:48:33.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.py
--rwxrwxrwx   0 root         (0) root         (0)      680 2023-11-11 15:22:30.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-_pyi_rth_utils.py
--rwxrwxrwx   0 root         (0) root         (0)     1327 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-_tkinter.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-babel.py
--rwxrwxrwx   0 root         (0) root         (0)      577 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-difflib.py
--rwxrwxrwx   0 root         (0) root         (0)      606 2023-11-04 13:41:36.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-distutils.command.check.py
--rwxrwxrwx   0 root         (0) root         (0)     1859 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-distutils.py
--rwxrwxrwx   0 root         (0) root         (0)      661 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-distutils.util.py
--rwxrwxrwx   0 root         (0) root         (0)      635 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-django.contrib.sessions.py
--rwxrwxrwx   0 root         (0) root         (0)      629 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-django.core.cache.py
--rwxrwxrwx   0 root         (0) root         (0)     1069 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-django.core.mail.py
--rwxrwxrwx   0 root         (0) root         (0)      942 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-django.core.management.py
--rwxrwxrwx   0 root         (0) root         (0)      611 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-django.db.backends.mysql.base.py
--rwxrwxrwx   0 root         (0) root         (0)      563 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-django.db.backends.oracle.base.py
--rwxrwxrwx   0 root         (0) root         (0)      983 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-django.db.backends.py
--rwxrwxrwx   0 root         (0) root         (0)     3922 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-django.py
--rwxrwxrwx   0 root         (0) root         (0)      626 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-django.template.loaders.py
--rwxrwxrwx   0 root         (0) root         (0)      612 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-encodings.py
--rwxrwxrwx   0 root         (0) root         (0)     1011 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-gevent.py
--rwxrwxrwx   0 root         (0) root         (0)      552 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.py
--rwxrwxrwx   0 root         (0) root         (0)      698 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.Adw.py
--rwxrwxrwx   0 root         (0) root         (0)      710 2024-01-13 17:57:57.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.AppIndicator3.py
--rwxrwxrwx   0 root         (0) root         (0)     1084 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.Atk.py
--rwxrwxrwx   0 root         (0) root         (0)      717 2024-01-13 17:57:57.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.AyatanaAppIndicator3.py
--rwxrwxrwx   0 root         (0) root         (0)      707 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.Champlain.py
--rwxrwxrwx   0 root         (0) root         (0)      704 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.Clutter.py
--rwxrwxrwx   0 root         (0) root         (0)      701 2024-01-13 17:57:57.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.DBus.py
--rwxrwxrwx   0 root         (0) root         (0)      709 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.GIRepository.py
--rwxrwxrwx   0 root         (0) root         (0)     1490 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.GLib.py
--rwxrwxrwx   0 root         (0) root         (0)      704 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.GModule.py
--rwxrwxrwx   0 root         (0) root         (0)      905 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.GObject.py
--rwxrwxrwx   0 root         (0) root         (0)     1393 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.Gdk.py
--rwxrwxrwx   0 root         (0) root         (0)     6318 2023-11-26 23:20:35.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.GdkPixbuf.py
--rwxrwxrwx   0 root         (0) root         (0)     2605 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.Gio.py
--rwxrwxrwx   0 root         (0) root         (0)      705 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.Graphene.py
--rwxrwxrwx   0 root         (0) root         (0)      700 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.Gsk.py
--rwxrwxrwx   0 root         (0) root         (0)     3461 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.Gst.py
--rwxrwxrwx   0 root         (0) root         (0)      710 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.GstAllocators.py
--rwxrwxrwx   0 root         (0) root         (0)      703 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.GstApp.py
--rwxrwxrwx   0 root         (0) root         (0)      705 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.GstAudio.py
--rwxrwxrwx   0 root         (0) root         (0)      708 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.GstBadAudio.py
--rwxrwxrwx   0 root         (0) root         (0)      704 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.GstBase.py
--rwxrwxrwx   0 root         (0) root         (0)      705 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.GstCheck.py
--rwxrwxrwx   0 root         (0) root         (0)      706 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.GstCodecs.py
--rwxrwxrwx   0 root         (0) root         (0)      710 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.GstController.py
--rwxrwxrwx   0 root         (0) root         (0)      702 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.GstGL.py
--rwxrwxrwx   0 root         (0) root         (0)      705 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.GstGLEGL.py
--rwxrwxrwx   0 root         (0) root         (0)      709 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.GstGLWayland.py
--rwxrwxrwx   0 root         (0) root         (0)      705 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.GstGLX11.py
--rwxrwxrwx   0 root         (0) root         (0)      709 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.GstInsertBin.py
--rwxrwxrwx   0 root         (0) root         (0)      706 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.GstMpegts.py
--rwxrwxrwx   0 root         (0) root         (0)      703 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.GstNet.py
--rwxrwxrwx   0 root         (0) root         (0)      707 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.GstPbutils.py
--rwxrwxrwx   0 root         (0) root         (0)      704 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.GstPlay.py
--rwxrwxrwx   0 root         (0) root         (0)      706 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.GstPlayer.py
--rwxrwxrwx   0 root         (0) root         (0)      703 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.GstRtp.py
--rwxrwxrwx   0 root         (0) root         (0)      704 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.GstRtsp.py
--rwxrwxrwx   0 root         (0) root         (0)      710 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.GstRtspServer.py
--rwxrwxrwx   0 root         (0) root         (0)      703 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.GstSdp.py
--rwxrwxrwx   0 root         (0) root         (0)      703 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.GstTag.py
--rwxrwxrwx   0 root         (0) root         (0)      710 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.GstTranscoder.py
--rwxrwxrwx   0 root         (0) root         (0)      705 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.GstVideo.py
--rwxrwxrwx   0 root         (0) root         (0)      706 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.GstVulkan.py
--rwxrwxrwx   0 root         (0) root         (0)      713 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.GstVulkanWayland.py
--rwxrwxrwx   0 root         (0) root         (0)      709 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.GstVulkanXCB.py
--rwxrwxrwx   0 root         (0) root         (0)      706 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.GstWebRTC.py
--rwxrwxrwx   0 root         (0) root         (0)     2150 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.Gtk.py
--rwxrwxrwx   0 root         (0) root         (0)      710 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.GtkChamplain.py
--rwxrwxrwx   0 root         (0) root         (0)      707 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.GtkClutter.py
--rwxrwxrwx   0 root         (0) root         (0)     1297 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.GtkSource.py
--rwxrwxrwx   0 root         (0) root         (0)      781 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.GtkosxApplication.py
--rwxrwxrwx   0 root         (0) root         (0)      705 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.HarfBuzz.py
--rwxrwxrwx   0 root         (0) root         (0)      702 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.Pango.py
--rwxrwxrwx   0 root         (0) root         (0)      707 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.PangoCairo.py
--rwxrwxrwx   0 root         (0) root         (0)      702 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.cairo.py
--rwxrwxrwx   0 root         (0) root         (0)      706 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.freetype2.py
--rwxrwxrwx   0 root         (0) root         (0)      701 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.xlib.py
--rwxrwxrwx   0 root         (0) root         (0)      578 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-heapq.py
--rwxrwxrwx   0 root         (0) root         (0)      602 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-idlelib.py
--rwxrwxrwx   0 root         (0) root         (0)     1350 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-importlib_metadata.py
--rwxrwxrwx   0 root         (0) root         (0)     1015 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-importlib_resources.py
--rwxrwxrwx   0 root         (0) root         (0)      888 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-keyring.py
--rwxrwxrwx   0 root         (0) root         (0)     1126 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-kivy.py
--rwxrwxrwx   0 root         (0) root         (0)      653 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-lib2to3.py
--rwxrwxrwx   0 root         (0) root         (0)      894 2024-03-09 19:48:33.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-matplotlib.backends.backend_qtagg.py
--rwxrwxrwx   0 root         (0) root         (0)      896 2024-03-09 19:48:33.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-matplotlib.backends.backend_qtcairo.py
--rwxrwxrwx   0 root         (0) root         (0)     9657 2024-03-09 19:48:33.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-matplotlib.backends.py
--rwxrwxrwx   0 root         (0) root         (0)     1284 2024-03-09 19:48:33.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-matplotlib.backends.qt_compat.py
--rwxrwxrwx   0 root         (0) root         (0)      683 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-matplotlib.numerix.py
--rwxrwxrwx   0 root         (0) root         (0)     1568 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-matplotlib.py
--rwxrwxrwx   0 root         (0) root         (0)      791 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-multiprocessing.util.py
--rwxrwxrwx   0 root         (0) root         (0)     2331 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-numpy.py
--rwxrwxrwx   0 root         (0) root         (0)      577 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-packaging.py
--rwxrwxrwx   0 root         (0) root         (0)     1156 2024-03-09 19:48:33.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-pandas.io.clipboard.py
--rwxrwxrwx   0 root         (0) root         (0)      751 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-pandas.io.formats.style.py
--rwxrwxrwx   0 root         (0) root         (0)      938 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-pandas.plotting.py
--rwxrwxrwx   0 root         (0) root         (0)      955 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-pandas.py
--rwxrwxrwx   0 root         (0) root         (0)      589 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-pickle.py
--rwxrwxrwx   0 root         (0) root         (0)     2952 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-pkg_resources.py
--rwxrwxrwx   0 root         (0) root         (0)      713 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-platform.py
--rwxrwxrwx   0 root         (0) root         (0)     1184 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-pygments.py
--rwxrwxrwx   0 root         (0) root         (0)      734 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-pytz.py
--rwxrwxrwx   0 root         (0) root         (0)      603 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-pytzdata.py
--rwxrwxrwx   0 root         (0) root         (0)      792 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-qtawesome.py
--rwxrwxrwx   0 root         (0) root         (0)     1179 2024-03-09 19:48:33.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-qtpy.py
--rwxrwxrwx   0 root         (0) root         (0)      930 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-scapy.layers.all.py
--rwxrwxrwx   0 root         (0) root         (0)      655 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-scipy.io.matlab.py
--rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-scipy.linalg.py
--rwxrwxrwx   0 root         (0) root         (0)     1604 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-scipy.py
--rwxrwxrwx   0 root         (0) root         (0)      611 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-scipy.sparse.csgraph.py
--rwxrwxrwx   0 root         (0) root         (0)      793 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-scipy.spatial.transform.rotation.py
--rwxrwxrwx   0 root         (0) root         (0)     1317 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-scipy.special._ellip_harm_2.py
--rwxrwxrwx   0 root         (0) root         (0)     1042 2024-04-13 09:44:10.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-scipy.special._ufuncs.py
--rwxrwxrwx   0 root         (0) root         (0)      656 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-scipy.stats._stats.py
--rwxrwxrwx   0 root         (0) root         (0)      819 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-scrapy.py
--rwxrwxrwx   0 root         (0) root         (0)      606 2023-11-04 13:41:36.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-setuptools._distutils.command.check.py
--rwxrwxrwx   0 root         (0) root         (0)      599 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-setuptools.msvc.py
--rwxrwxrwx   0 root         (0) root         (0)     2149 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-setuptools.py
--rwxrwxrwx   0 root         (0) root         (0)      603 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-shelve.py
--rwxrwxrwx   0 root         (0) root         (0)      766 2023-11-04 13:41:36.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-shiboken6.py
--rwxrwxrwx   0 root         (0) root         (0)     1998 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-sphinx.py
--rwxrwxrwx   0 root         (0) root         (0)     3076 2023-11-26 23:20:35.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-sqlalchemy.py
--rwxrwxrwx   0 root         (0) root         (0)      813 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-sqlite3.py
--rwxrwxrwx   0 root         (0) root         (0)     1558 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-sysconfig.py
--rwxrwxrwx   0 root         (0) root         (0)      602 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-wcwidth.py
--rwxrwxrwx   0 root         (0) root         (0)      993 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-win32ctypes.core.py
--rwxrwxrwx   0 root         (0) root         (0)      569 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-xml.dom.domreg.py
--rwxrwxrwx   0 root         (0) root         (0)      615 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-xml.etree.cElementTree.py
--rwxrwxrwx   0 root         (0) root         (0)      569 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-xml.py
--rwxrwxrwx   0 root         (0) root         (0)      539 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/hook-zope.interface.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:10.900899 pyinstaller-6.6.0/PyInstaller/hooks/pre_find_module_path/
--rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/pre_find_module_path/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      696 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/pre_find_module_path/hook-PyQt5.uic.port_v2.py
--rwxrwxrwx   0 root         (0) root         (0)      905 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/pre_find_module_path/hook-_pyi_rth_utils.py
--rwxrwxrwx   0 root         (0) root         (0)     2347 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/pre_find_module_path/hook-distutils.py
--rwxrwxrwx   0 root         (0) root         (0)     1412 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/pre_find_module_path/hook-pyi_splash.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:10.918044 pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/
--rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1772 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-distutils.py
--rwxrwxrwx   0 root         (0) root         (0)     1955 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.py
--rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.Adw.py
--rwxrwxrwx   0 root         (0) root         (0)      783 2024-01-13 17:57:57.000000 pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.AppIndicator3.py
--rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.Atk.py
--rwxrwxrwx   0 root         (0) root         (0)      783 2024-01-13 17:57:57.000000 pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.AyatanaAppIndicator3.py
--rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.Champlain.py
--rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.Clutter.py
--rwxrwxrwx   0 root         (0) root         (0)      783 2024-01-13 17:57:57.000000 pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.DBus.py
--rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GIRepository.py
--rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GLib.py
--rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GModule.py
--rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GObject.py
--rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.Gdk.py
--rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GdkPixbuf.py
--rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.Gio.py
--rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.Graphene.py
--rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.Gsk.py
--rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.Gst.py
--rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstAllocators.py
--rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstApp.py
--rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstAudio.py
--rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstBadAudio.py
--rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstBase.py
--rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstCheck.py
--rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstCodecs.py
--rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstController.py
--rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstGL.py
--rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstGLEGL.py
--rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstGLWayland.py
--rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstGLX11.py
--rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstInsertBin.py
--rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstMpegts.py
--rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstNet.py
--rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstPbutils.py
--rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstPlay.py
--rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstPlayer.py
--rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstRtp.py
--rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstRtsp.py
--rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstRtspServer.py
--rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstSdp.py
--rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstTag.py
--rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstTranscoder.py
--rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstVideo.py
--rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstVulkan.py
--rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstVulkanWayland.py
--rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstVulkanXCB.py
--rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstWebRTC.py
--rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.Gtk.py
--rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GtkChamplain.py
--rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GtkClutter.py
--rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GtkSource.py
--rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GtkosxApplication.py
--rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.HarfBuzz.py
--rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.Pango.py
--rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.PangoCairo.py
--rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.cairo.py
--rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.freetype2.py
--rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.xlib.py
--rwxrwxrwx   0 root         (0) root         (0)     1629 2024-01-13 17:57:57.000000 pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-setuptools.extern.six.moves.py
--rwxrwxrwx   0 root         (0) root         (0)     3744 2024-01-13 17:57:57.000000 pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-six.moves.py
--rwxrwxrwx   0 root         (0) root         (0)     1380 2024-01-13 17:57:57.000000 pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-urllib3.packages.six.moves.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:10.923897 pyinstaller-6.6.0/PyInstaller/hooks/rthooks/
--rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/rthooks/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1248 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/rthooks/pyi_rth__tkinter.py
--rwxrwxrwx   0 root         (0) root         (0)     1111 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/rthooks/pyi_rth_django.py
--rwxrwxrwx   0 root         (0) root         (0)     1437 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/rthooks/pyi_rth_gdkpixbuf.py
--rwxrwxrwx   0 root         (0) root         (0)      632 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/rthooks/pyi_rth_gi.py
--rwxrwxrwx   0 root         (0) root         (0)      631 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/rthooks/pyi_rth_gio.py
--rwxrwxrwx   0 root         (0) root         (0)     1444 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/rthooks/pyi_rth_glib.py
--rwxrwxrwx   0 root         (0) root         (0)     1175 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/rthooks/pyi_rth_gstreamer.py
--rwxrwxrwx   0 root         (0) root         (0)      886 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/rthooks/pyi_rth_gtk.py
--rwxrwxrwx   0 root         (0) root         (0)     2094 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/rthooks/pyi_rth_inspect.py
--rwxrwxrwx   0 root         (0) root         (0)      737 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/rthooks/pyi_rth_kivy.py
--rwxrwxrwx   0 root         (0) root         (0)     1808 2023-11-11 15:22:30.000000 pyinstaller-6.6.0/PyInstaller/hooks/rthooks/pyi_rth_mplconfig.py
--rwxrwxrwx   0 root         (0) root         (0)     4814 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/rthooks/pyi_rth_multiprocessing.py
--rwxrwxrwx   0 root         (0) root         (0)     7889 2023-11-11 15:22:30.000000 pyinstaller-6.6.0/PyInstaller/hooks/rthooks/pyi_rth_pkgres.py
--rwxrwxrwx   0 root         (0) root         (0)     6072 2024-01-13 17:58:01.000000 pyinstaller-6.6.0/PyInstaller/hooks/rthooks/pyi_rth_pkgutil.py
--rwxrwxrwx   0 root         (0) root         (0)     3542 2024-03-09 19:48:33.000000 pyinstaller-6.6.0/PyInstaller/hooks/rthooks/pyi_rth_pyqt5.py
--rwxrwxrwx   0 root         (0) root         (0)     3803 2024-03-09 19:48:33.000000 pyinstaller-6.6.0/PyInstaller/hooks/rthooks/pyi_rth_pyqt6.py
--rwxrwxrwx   0 root         (0) root         (0)     3235 2024-03-09 19:48:33.000000 pyinstaller-6.6.0/PyInstaller/hooks/rthooks/pyi_rth_pyside2.py
--rwxrwxrwx   0 root         (0) root         (0)     3730 2024-03-09 19:48:33.000000 pyinstaller-6.6.0/PyInstaller/hooks/rthooks/pyi_rth_pyside6.py
--rwxrwxrwx   0 root         (0) root         (0)     1430 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/hooks/rthooks/pyi_rth_setuptools.py
--rwxrwxrwx   0 root         (0) root         (0)      956 2024-02-23 20:40:55.000000 pyinstaller-6.6.0/PyInstaller/hooks/rthooks.dat
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:10.924627 pyinstaller-6.6.0/PyInstaller/isolated/
--rwxrwxrwx   0 root         (0) root         (0)     1524 2024-03-09 19:48:33.000000 pyinstaller-6.6.0/PyInstaller/isolated/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     3757 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/isolated/_child.py
--rwxrwxrwx   0 root         (0) root         (0)    17407 2023-10-12 17:16:03.000000 pyinstaller-6.6.0/PyInstaller/isolated/_parent.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:10.925199 pyinstaller-6.6.0/PyInstaller/lib/
--rwxrwxrwx   0 root         (0) root         (0)     1333 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/lib/README.rst
--rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/lib/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:10.927037 pyinstaller-6.6.0/PyInstaller/lib/modulegraph/
--rwxrwxrwx   0 root         (0) root         (0)       21 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/lib/modulegraph/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     2653 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/lib/modulegraph/__main__.py
--rwxrwxrwx   0 root         (0) root         (0)     1754 2023-11-26 23:20:35.000000 pyinstaller-6.6.0/PyInstaller/lib/modulegraph/find_modules.py
--rwxrwxrwx   0 root         (0) root         (0)   129871 2023-11-26 23:20:35.000000 pyinstaller-6.6.0/PyInstaller/lib/modulegraph/modulegraph.py
--rwxrwxrwx   0 root         (0) root         (0)      849 2023-11-26 23:20:35.000000 pyinstaller-6.6.0/PyInstaller/lib/modulegraph/util.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:10.928736 pyinstaller-6.6.0/PyInstaller/loader/
--rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/loader/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     3712 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/loader/pyiboot01_bootstrap.py
--rwxrwxrwx   0 root         (0) root         (0)     6059 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/loader/pyimod01_archive.py
--rwxrwxrwx   0 root         (0) root         (0)    28111 2023-11-11 15:22:30.000000 pyinstaller-6.6.0/PyInstaller/loader/pyimod02_importers.py
--rwxrwxrwx   0 root         (0) root         (0)     4915 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/loader/pyimod03_ctypes.py
--rwxrwxrwx   0 root         (0) root         (0)     2936 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/loader/pyimod04_pywin32.py
--rwxrwxrwx   0 root         (0) root         (0)     2058 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/log.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:10.931645 pyinstaller-6.6.0/PyInstaller/utils/
--rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/utils/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      451 2023-10-12 17:16:03.000000 pyinstaller-6.6.0/PyInstaller/utils/_gitrevision.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:10.933694 pyinstaller-6.6.0/PyInstaller/utils/cliutils/
--rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/utils/cliutils/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     9259 2023-11-04 13:41:36.000000 pyinstaller-6.6.0/PyInstaller/utils/cliutils/archive_viewer.py
--rwxrwxrwx   0 root         (0) root         (0)     1844 2023-11-04 13:41:36.000000 pyinstaller-6.6.0/PyInstaller/utils/cliutils/bindepend.py
--rwxrwxrwx   0 root         (0) root         (0)     1857 2023-11-04 13:41:36.000000 pyinstaller-6.6.0/PyInstaller/utils/cliutils/grab_version.py
--rwxrwxrwx   0 root         (0) root         (0)     1640 2023-11-04 13:41:36.000000 pyinstaller-6.6.0/PyInstaller/utils/cliutils/makespec.py
--rwxrwxrwx   0 root         (0) root         (0)     1503 2023-11-04 13:41:36.000000 pyinstaller-6.6.0/PyInstaller/utils/cliutils/set_version.py
--rwxrwxrwx   0 root         (0) root         (0)    23544 2023-11-26 23:20:35.000000 pyinstaller-6.6.0/PyInstaller/utils/conftest.py
--rwxrwxrwx   0 root         (0) root         (0)     2014 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/utils/git.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:10.935737 pyinstaller-6.6.0/PyInstaller/utils/hooks/
--rwxrwxrwx   0 root         (0) root         (0)    50777 2023-11-26 23:20:35.000000 pyinstaller-6.6.0/PyInstaller/utils/hooks/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    14694 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/utils/hooks/conda.py
--rwxrwxrwx   0 root         (0) root         (0)     6100 2024-01-13 17:58:01.000000 pyinstaller-6.6.0/PyInstaller/utils/hooks/django.py
--rwxrwxrwx   0 root         (0) root         (0)    17414 2023-11-26 23:20:35.000000 pyinstaller-6.6.0/PyInstaller/utils/hooks/gi.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:10.936735 pyinstaller-6.6.0/PyInstaller/utils/hooks/qt/
--rwxrwxrwx   0 root         (0) root         (0)    74721 2024-03-09 19:48:33.000000 pyinstaller-6.6.0/PyInstaller/utils/hooks/qt/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    25226 2023-11-04 13:41:36.000000 pyinstaller-6.6.0/PyInstaller/utils/hooks/qt/_modules_info.py
--rwxrwxrwx   0 root         (0) root         (0)    10707 2023-11-26 23:20:35.000000 pyinstaller-6.6.0/PyInstaller/utils/hooks/tcl_tk.py
--rwxrwxrwx   0 root         (0) root         (0)     7030 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/utils/misc.py
--rwxrwxrwx   0 root         (0) root         (0)    29386 2024-01-13 17:58:01.000000 pyinstaller-6.6.0/PyInstaller/utils/osx.py
--rwxrwxrwx   0 root         (0) root         (0)       87 2023-10-12 17:16:03.000000 pyinstaller-6.6.0/PyInstaller/utils/pytest.ini
--rwxrwxrwx   0 root         (0) root         (0)     2875 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/utils/run_tests.py
--rwxrwxrwx   0 root         (0) root         (0)     5711 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/utils/tests.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:10.938912 pyinstaller-6.6.0/PyInstaller/utils/win32/
--rwxrwxrwx   0 root         (0) root         (0)       22 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/utils/win32/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     9327 2024-02-23 20:40:55.000000 pyinstaller-6.6.0/PyInstaller/utils/win32/icon.py
--rwxrwxrwx   0 root         (0) root         (0)    20594 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/utils/win32/versioninfo.py
--rwxrwxrwx   0 root         (0) root         (0)    10639 2023-10-12 17:16:03.000000 pyinstaller-6.6.0/PyInstaller/utils/win32/winmanifest.py
--rwxrwxrwx   0 root         (0) root         (0)     7625 2023-11-04 13:41:36.000000 pyinstaller-6.6.0/PyInstaller/utils/win32/winresource.py
--rwxrwxrwx   0 root         (0) root         (0)     9175 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/PyInstaller/utils/win32/winutils.py
--rwxrwxrwx   0 root         (0) root         (0)     5375 2024-04-13 09:45:34.000000 pyinstaller-6.6.0/README.rst
--rwxrwxrwx   0 root         (0) root         (0)     1955 2024-01-13 17:58:01.000000 pyinstaller-6.6.0/alpine.dockerfile
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:10.944858 pyinstaller-6.6.0/bootloader/
--rwxrwxrwx   0 root         (0) root         (0)       11 2023-09-30 18:27:19.000000 pyinstaller-6.6.0/bootloader/.gitattributes
--rwxrwxrwx   0 root         (0) root         (0)     2053 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/Dockerfile
--rwxrwxrwx   0 root         (0) root         (0)     3924 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/Dockerfile.osxcross
--rwxrwxrwx   0 root         (0) root         (0)      950 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/README.txt
--rwxrwxrwx   0 root         (0) root         (0)    15148 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/Vagrantfile
--rwxrwxrwx   0 root         (0) root         (0)     1489 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/build.sh
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:10.957482 pyinstaller-6.6.0/bootloader/src/
--rwxrwxrwx   0 root         (0) root         (0)     2599 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/src/main.c
--rwxrwxrwx   0 root         (0) root         (0)      875 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/src/mkdtemp.h
--rwxrwxrwx   0 root         (0) root         (0)    29474 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/src/pyi_apple_events.c
--rwxrwxrwx   0 root         (0) root         (0)     1825 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/src/pyi_apple_events.h
--rwxrwxrwx   0 root         (0) root         (0)    21690 2024-03-24 20:46:04.000000 pyinstaller-6.6.0/bootloader/src/pyi_archive.c
--rwxrwxrwx   0 root         (0) root         (0)     5752 2023-10-12 17:16:14.000000 pyinstaller-6.6.0/bootloader/src/pyi_archive.h
--rwxrwxrwx   0 root         (0) root         (0)    13273 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/src/pyi_exception_dialog.c
--rwxrwxrwx   0 root         (0) root         (0)      822 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/src/pyi_exception_dialog.h
--rwxrwxrwx   0 root         (0) root         (0)     7203 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/src/pyi_global.c
--rwxrwxrwx   0 root         (0) root         (0)     8411 2023-11-20 00:50:49.000000 pyinstaller-6.6.0/bootloader/src/pyi_global.h
--rwxrwxrwx   0 root         (0) root         (0)    25023 2023-11-20 00:50:49.000000 pyinstaller-6.6.0/bootloader/src/pyi_launch.c
--rwxrwxrwx   0 root         (0) root         (0)     2092 2023-10-12 17:16:14.000000 pyinstaller-6.6.0/bootloader/src/pyi_launch.h
--rwxrwxrwx   0 root         (0) root         (0)    20800 2024-03-24 20:46:04.000000 pyinstaller-6.6.0/bootloader/src/pyi_main.c
--rwxrwxrwx   0 root         (0) root         (0)      564 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/src/pyi_main.h
--rwxrwxrwx   0 root         (0) root         (0)    16553 2024-04-04 21:05:01.000000 pyinstaller-6.6.0/bootloader/src/pyi_path.c
--rwxrwxrwx   0 root         (0) root         (0)     1567 2024-04-04 21:05:01.000000 pyinstaller-6.6.0/bootloader/src/pyi_path.h
--rwxrwxrwx   0 root         (0) root         (0)    19484 2024-02-23 20:40:55.000000 pyinstaller-6.6.0/bootloader/src/pyi_pyconfig.c
--rwxrwxrwx   0 root         (0) root         (0)     1925 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/src/pyi_pyconfig.h
--rwxrwxrwx   0 root         (0) root         (0)     2348 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/src/pyi_pyconfig_v310.h
--rwxrwxrwx   0 root         (0) root         (0)     2503 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/src/pyi_pyconfig_v311.h
--rwxrwxrwx   0 root         (0) root         (0)     2526 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/src/pyi_pyconfig_v312.h
--rwxrwxrwx   0 root         (0) root         (0)     2250 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/src/pyi_pyconfig_v38.h
--rwxrwxrwx   0 root         (0) root         (0)     2336 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/src/pyi_pyconfig_v39.h
--rwxrwxrwx   0 root         (0) root         (0)     3997 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/src/pyi_python.c
--rwxrwxrwx   0 root         (0) root         (0)     8491 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/src/pyi_python.h
--rwxrwxrwx   0 root         (0) root         (0)    14251 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/src/pyi_pythonlib.c
--rwxrwxrwx   0 root         (0) root         (0)     1071 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/src/pyi_pythonlib.h
--rwxrwxrwx   0 root         (0) root         (0)    37395 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/src/pyi_splash.c
--rwxrwxrwx   0 root         (0) root         (0)     6094 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/src/pyi_splash.h
--rwxrwxrwx   0 root         (0) root         (0)     3386 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/src/pyi_splashlib.c
--rwxrwxrwx   0 root         (0) root         (0)     4517 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/src/pyi_splashlib.h
--rwxrwxrwx   0 root         (0) root         (0)    42745 2023-10-12 17:16:14.000000 pyinstaller-6.6.0/bootloader/src/pyi_utils.c
--rwxrwxrwx   0 root         (0) root         (0)     2452 2023-10-12 17:16:14.000000 pyinstaller-6.6.0/bootloader/src/pyi_utils.h
--rwxrwxrwx   0 root         (0) root         (0)    20248 2024-02-10 12:19:40.000000 pyinstaller-6.6.0/bootloader/src/pyi_win32_utils.c
--rwxrwxrwx   0 root         (0) root         (0)     1356 2024-02-10 12:19:40.000000 pyinstaller-6.6.0/bootloader/src/pyi_win32_utils.h
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:10.958893 pyinstaller-6.6.0/bootloader/tests/
--rwxrwxrwx   0 root         (0) root         (0)     3854 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/tests/test_launch.c
--rwxrwxrwx   0 root         (0) root         (0)     7906 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/tests/test_path.c
--rwxrwxrwx   0 root         (0) root         (0)     1770 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/tests/wscript
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:10.959169 pyinstaller-6.6.0/bootloader/tools/
--rwxrwxrwx   0 root         (0) root         (0)     1768 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/tools/strip.py
--rwxrwxrwx   0 root         (0) root         (0)    80769 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/uncrustify.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1820 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/update-waf.sh
--rwxrwxrwx   0 root         (0) root         (0)     1581 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/waf
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:10.964535 pyinstaller-6.6.0/bootloader/waflib/
--rwxrwxrwx   0 root         (0) root         (0)    30209 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/waflib/Build.py
--rwxrwxrwx   0 root         (0) root         (0)     5179 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/waflib/ConfigSet.py
--rwxrwxrwx   0 root         (0) root         (0)    14831 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/waflib/Configure.py
--rwxrwxrwx   0 root         (0) root         (0)    14805 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/waflib/Context.py
--rwxrwxrwx   0 root         (0) root         (0)     1248 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/waflib/Errors.py
--rwxrwxrwx   0 root         (0) root         (0)     7207 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/waflib/Logs.py
--rwxrwxrwx   0 root         (0) root         (0)    15286 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/waflib/Node.py
--rwxrwxrwx   0 root         (0) root         (0)    11367 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/waflib/Options.py
--rwxrwxrwx   0 root         (0) root         (0)    13041 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/waflib/Runner.py
--rwxrwxrwx   0 root         (0) root         (0)    15382 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/waflib/Scripting.py
--rwxrwxrwx   0 root         (0) root         (0)    28095 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/waflib/Task.py
--rwxrwxrwx   0 root         (0) root         (0)    17611 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/waflib/TaskGen.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:10.998792 pyinstaller-6.6.0/bootloader/waflib/Tools/
--rwxrwxrwx   0 root         (0) root         (0)      120 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/waflib/Tools/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      360 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/waflib/Tools/ar.py
--rwxrwxrwx   0 root         (0) root         (0)     2090 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/waflib/Tools/asm.py
--rwxrwxrwx   0 root         (0) root         (0)      933 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/waflib/Tools/bison.py
--rwxrwxrwx   0 root         (0) root         (0)     1220 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/waflib/Tools/c.py
--rwxrwxrwx   0 root         (0) root         (0)     1893 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/waflib/Tools/c_aliases.py
--rwxrwxrwx   0 root         (0) root         (0)    31523 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/waflib/Tools/c_config.py
--rwxrwxrwx   0 root         (0) root         (0)     5203 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/waflib/Tools/c_osx.py
--rwxrwxrwx   0 root         (0) root         (0)    25054 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/waflib/Tools/c_preproc.py
--rwxrwxrwx   0 root         (0) root         (0)     5042 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/waflib/Tools/c_tests.py
--rwxrwxrwx   0 root         (0) root         (0)    19729 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/waflib/Tools/ccroot.py
--rwxrwxrwx   0 root         (0) root         (0)      594 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/waflib/Tools/clang.py
--rwxrwxrwx   0 root         (0) root         (0)      606 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/waflib/Tools/clangxx.py
--rwxrwxrwx   0 root         (0) root         (0)     2165 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/waflib/Tools/compiler_c.py
--rwxrwxrwx   0 root         (0) root         (0)     2178 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/waflib/Tools/compiler_cxx.py
--rwxrwxrwx   0 root         (0) root         (0)     1689 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/waflib/Tools/compiler_d.py
--rwxrwxrwx   0 root         (0) root         (0)     2006 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/waflib/Tools/compiler_fc.py
--rwxrwxrwx   0 root         (0) root         (0)     4439 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/waflib/Tools/cs.py
--rwxrwxrwx   0 root         (0) root         (0)     1295 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/waflib/Tools/cxx.py
--rwxrwxrwx   0 root         (0) root         (0)     2297 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/waflib/Tools/d.py
--rwxrwxrwx   0 root         (0) root         (0)     1306 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/waflib/Tools/d_config.py
--rwxrwxrwx   0 root         (0) root         (0)     4337 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/waflib/Tools/d_scan.py
--rwxrwxrwx   0 root         (0) root         (0)     1227 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/waflib/Tools/dbus.py
--rwxrwxrwx   0 root         (0) root         (0)     1643 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/waflib/Tools/dmd.py
--rwxrwxrwx   0 root         (0) root         (0)     8302 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/waflib/Tools/errcheck.py
--rwxrwxrwx   0 root         (0) root         (0)     5373 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/waflib/Tools/fc.py
--rwxrwxrwx   0 root         (0) root         (0)    11313 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/waflib/Tools/fc_config.py
--rwxrwxrwx   0 root         (0) root         (0)     2414 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/waflib/Tools/fc_scan.py
--rwxrwxrwx   0 root         (0) root         (0)     1377 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/waflib/Tools/flex.py
--rwxrwxrwx   0 root         (0) root         (0)     1599 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/waflib/Tools/g95.py
--rwxrwxrwx   0 root         (0) root         (0)      385 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/waflib/Tools/gas.py
--rwxrwxrwx   0 root         (0) root         (0)     2985 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/waflib/Tools/gcc.py
--rwxrwxrwx   0 root         (0) root         (0)      998 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/waflib/Tools/gdc.py
--rwxrwxrwx   0 root         (0) root         (0)     2225 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/waflib/Tools/gfortran.py
--rwxrwxrwx   0 root         (0) root         (0)    12984 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/waflib/Tools/glib2.py
--rwxrwxrwx   0 root         (0) root         (0)     3104 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/waflib/Tools/gnu_dirs.py
--rwxrwxrwx   0 root         (0) root         (0)     3054 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/waflib/Tools/gxx.py
--rwxrwxrwx   0 root         (0) root         (0)      553 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/waflib/Tools/icc.py
--rwxrwxrwx   0 root         (0) root         (0)      553 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/waflib/Tools/icpc.py
--rwxrwxrwx   0 root         (0) root         (0)    11869 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/waflib/Tools/ifort.py
--rwxrwxrwx   0 root         (0) root         (0)     4385 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/waflib/Tools/intltool.py
--rwxrwxrwx   0 root         (0) root         (0)     1096 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/waflib/Tools/irixcc.py
--rwxrwxrwx   0 root         (0) root         (0)    13193 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/waflib/Tools/javaw.py
--rwxrwxrwx   0 root         (0) root         (0)     1068 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/waflib/Tools/ldc2.py
--rwxrwxrwx   0 root         (0) root         (0)      641 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/waflib/Tools/lua.py
--rwxrwxrwx   0 root         (0) root         (0)      801 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/waflib/Tools/md5_tstamp.py
--rwxrwxrwx   0 root         (0) root         (0)    33374 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/waflib/Tools/msvc.py
--rwxrwxrwx   0 root         (0) root         (0)      686 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/waflib/Tools/nasm.py
--rwxrwxrwx   0 root         (0) root         (0)      305 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/waflib/Tools/nobuild.py
--rwxrwxrwx   0 root         (0) root         (0)     3446 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/waflib/Tools/perl.py
--rwxrwxrwx   0 root         (0) root         (0)    21797 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/waflib/Tools/python.py
--rwxrwxrwx   0 root         (0) root         (0)    20211 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/waflib/Tools/qt5.py
--rwxrwxrwx   0 root         (0) root         (0)     4384 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/waflib/Tools/ruby.py
--rwxrwxrwx   0 root         (0) root         (0)     1324 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/waflib/Tools/suncc.py
--rwxrwxrwx   0 root         (0) root         (0)     1358 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/waflib/Tools/suncxx.py
--rwxrwxrwx   0 root         (0) root         (0)    13995 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/waflib/Tools/tex.py
--rwxrwxrwx   0 root         (0) root         (0)    10164 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/waflib/Tools/vala.py
--rwxrwxrwx   0 root         (0) root         (0)     7884 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/waflib/Tools/waf_unit_test.py
--rwxrwxrwx   0 root         (0) root         (0)     2097 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/waflib/Tools/winres.py
--rwxrwxrwx   0 root         (0) root         (0)     1204 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/waflib/Tools/xlc.py
--rwxrwxrwx   0 root         (0) root         (0)     1247 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/waflib/Tools/xlcxx.py
--rwxrwxrwx   0 root         (0) root         (0)    19314 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/waflib/Utils.py
--rwxrwxrwx   0 root         (0) root         (0)      120 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/waflib/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    12079 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/waflib/ansiterm.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:10.999369 pyinstaller-6.6.0/bootloader/waflib/extras/
--rwxrwxrwx   0 root         (0) root         (0)      120 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/waflib/extras/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1509 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/waflib/fixpy2.py
--rwxrwxrwx   0 root         (0) root         (0)     1764 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/waflib/processor.py
--rwxrwxrwx   0 root         (0) root         (0)    37246 2024-03-09 19:48:33.000000 pyinstaller-6.6.0/bootloader/wscript
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.013646 pyinstaller-6.6.0/bootloader/zlib/
--rwxrwxrwx   0 root         (0) root         (0)      278 2024-02-10 12:19:40.000000 pyinstaller-6.6.0/bootloader/zlib/README
--rwxrwxrwx   0 root         (0) root         (0)     4964 2024-02-10 12:19:40.000000 pyinstaller-6.6.0/bootloader/zlib/adler32.c
--rwxrwxrwx   0 root         (0) root         (0)    31605 2024-02-10 12:19:40.000000 pyinstaller-6.6.0/bootloader/zlib/crc32.c
--rwxrwxrwx   0 root         (0) root         (0)   591749 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/zlib/crc32.h
--rwxrwxrwx   0 root         (0) root         (0)     6676 2024-02-10 12:19:40.000000 pyinstaller-6.6.0/bootloader/zlib/gzguts.h
--rwxrwxrwx   0 root         (0) root         (0)    12924 2024-02-10 12:19:40.000000 pyinstaller-6.6.0/bootloader/zlib/inffast.c
--rwxrwxrwx   0 root         (0) root         (0)      422 2024-02-10 12:19:40.000000 pyinstaller-6.6.0/bootloader/zlib/inffast.h
--rwxrwxrwx   0 root         (0) root         (0)     6332 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/zlib/inffixed.h
--rwxrwxrwx   0 root         (0) root         (0)    55519 2024-02-10 12:19:40.000000 pyinstaller-6.6.0/bootloader/zlib/inflate.c
--rwxrwxrwx   0 root         (0) root         (0)     6683 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/bootloader/zlib/inflate.h
--rwxrwxrwx   0 root         (0) root         (0)    13024 2024-02-10 12:19:40.000000 pyinstaller-6.6.0/bootloader/zlib/inftrees.c
--rwxrwxrwx   0 root         (0) root         (0)     2920 2024-02-10 12:19:40.000000 pyinstaller-6.6.0/bootloader/zlib/inftrees.h
--rwxrwxrwx   0 root         (0) root         (0)    16500 2024-02-10 12:19:40.000000 pyinstaller-6.6.0/bootloader/zlib/zconf.h
--rwxrwxrwx   0 root         (0) root         (0)    96829 2024-02-10 12:19:40.000000 pyinstaller-6.6.0/bootloader/zlib/zlib.h
--rwxrwxrwx   0 root         (0) root         (0)     7179 2024-02-10 12:19:40.000000 pyinstaller-6.6.0/bootloader/zlib/zutil.c
--rwxrwxrwx   0 root         (0) root         (0)     6677 2024-02-10 12:19:40.000000 pyinstaller-6.6.0/bootloader/zlib/zutil.h
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.024732 pyinstaller-6.6.0/doc/
--rwxrwxrwx   0 root         (0) root         (0)    10417 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/doc/CHANGES-1.rst
--rwxrwxrwx   0 root         (0) root         (0)     6193 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/doc/CHANGES-2.rst
--rwxrwxrwx   0 root         (0) root         (0)    51520 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/doc/CHANGES-3.rst
--rwxrwxrwx   0 root         (0) root         (0)   149992 2024-04-13 09:45:28.000000 pyinstaller-6.6.0/doc/CHANGES.rst
--rwxrwxrwx   0 root         (0) root         (0)    20828 2024-04-13 09:45:34.000000 pyinstaller-6.6.0/doc/CREDITS.rst
--rwxrwxrwx   0 root         (0) root         (0)     7447 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/doc/Makefile
--rwxrwxrwx   0 root         (0) root         (0)     4327 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/doc/_common_definitions.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.026038 pyinstaller-6.6.0/doc/_static/
--rwxrwxrwx   0 root         (0) root         (0)     3986 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/doc/_static/CArchive.png
--rwxrwxrwx   0 root         (0) root         (0)     3058 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/doc/_static/SE_exe.png
--rwxrwxrwx   0 root         (0) root         (0)     3521 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/doc/_static/ZlibArchive.png
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.027207 pyinstaller-6.6.0/doc/_static/css/
--rwxrwxrwx   0 root         (0) root         (0)      963 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/doc/_static/css/pyinstaller.css
--rwxrwxrwx   0 root         (0) root         (0)    16059 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/doc/_static/pyinstaller-draft1a-100_trans.png
--rwxrwxrwx   0 root         (0) root         (0)   217780 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/doc/_static/pyinstaller-draft1a.ico
--rwxrwxrwx   0 root         (0) root         (0)    24495 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/doc/advanced-topics.rst
--rwxrwxrwx   0 root         (0) root         (0)    18719 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/doc/bootloader-building.rst
--rwxrwxrwx   0 root         (0) root         (0)    20792 2024-01-13 17:58:01.000000 pyinstaller-6.6.0/doc/common-issues-and-pitfalls.rst
--rwxrwxrwx   0 root         (0) root         (0)    14400 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/doc/conf.py
--rwxrwxrwx   0 root         (0) root         (0)     3322 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/doc/contributing.rst
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.030103 pyinstaller-6.6.0/doc/development/
--rwxrwxrwx   0 root         (0) root         (0)     1749 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/doc/development/branch-model.rst
--rwxrwxrwx   0 root         (0) root         (0)     2755 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/doc/development/changelog-entries.rst
--rwxrwxrwx   0 root         (0) root         (0)     1025 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/doc/development/coding-conventions.rst
--rwxrwxrwx   0 root         (0) root         (0)     9608 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/doc/development/commit-messages.rst
--rwxrwxrwx   0 root         (0) root         (0)     2681 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/doc/development/documentation.rst
--rwxrwxrwx   0 root         (0) root         (0)      811 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/doc/development/git.rst
--rwxrwxrwx   0 root         (0) root         (0)      415 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/doc/development/index.rst
--rwxrwxrwx   0 root         (0) root         (0)     3473 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/doc/development/pull-requests.rst
--rwxrwxrwx   0 root         (0) root         (0)     2221 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/doc/development/quickstart.rst
--rwxrwxrwx   0 root         (0) root         (0)     2100 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/doc/development/testing.rst
--rwxrwxrwx   0 root         (0) root         (0)     1204 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/doc/development/venv.rst
--rwxrwxrwx   0 root         (0) root         (0)    75507 2024-04-04 21:05:01.000000 pyinstaller-6.6.0/doc/feature-notes.rst
--rwxrwxrwx   0 root         (0) root         (0)     4432 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/doc/help2rst.py
--rwxrwxrwx   0 root         (0) root         (0)    16431 2024-03-09 19:48:33.000000 pyinstaller-6.6.0/doc/hooks-config.rst
--rwxrwxrwx   0 root         (0) root         (0)    26257 2024-01-13 17:58:01.000000 pyinstaller-6.6.0/doc/hooks.rst
--rwxrwxrwx   0 root         (0) root         (0)     2280 2024-01-13 17:58:01.000000 pyinstaller-6.6.0/doc/index.rst
--rwxrwxrwx   0 root         (0) root         (0)     4402 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/doc/installation.rst
--rwxrwxrwx   0 root         (0) root         (0)     1024 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/doc/license.rst
--rwxrwxrwx   0 root         (0) root         (0)     6994 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/doc/make.bat
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.030613 pyinstaller-6.6.0/doc/man/
--rwxrwxrwx   0 root         (0) root         (0)     1495 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/doc/man/pyi-makespec.rst
--rwxrwxrwx   0 root         (0) root         (0)     1663 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/doc/man/pyinstaller.rst
--rwxrwxrwx   0 root         (0) root         (0)       96 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/doc/man-pages.rst
--rwxrwxrwx   0 root         (0) root         (0)    11767 2024-04-04 21:05:01.000000 pyinstaller-6.6.0/doc/operating-mode.rst
--rwxrwxrwx   0 root         (0) root         (0)    13299 2024-04-13 09:45:33.000000 pyinstaller-6.6.0/doc/pyi-makespec.1
--rwxrwxrwx   0 root         (0) root         (0)    14185 2024-04-13 09:45:33.000000 pyinstaller-6.6.0/doc/pyinstaller.1
--rwxrwxrwx   0 root         (0) root         (0)     2004 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/doc/requirements.rst
--rwxrwxrwx   0 root         (0) root         (0)      677 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/doc/requirements.txt
--rwxrwxrwx   0 root         (0) root         (0)     9176 2024-02-10 12:19:40.000000 pyinstaller-6.6.0/doc/runtime-information.rst
--rwxrwxrwx   0 root         (0) root         (0)    30301 2024-04-04 21:05:01.000000 pyinstaller-6.6.0/doc/spec-files.rst
--rwxrwxrwx   0 root         (0) root         (0)    32897 2024-04-04 21:05:01.000000 pyinstaller-6.6.0/doc/usage.rst
--rwxrwxrwx   0 root         (0) root         (0)    14242 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/doc/when-things-go-wrong.rst
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.037096 pyinstaller-6.6.0/icons/
--rwxrwxrwx   0 root         (0) root         (0)   266950 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/icons/github_logo.png
--rwxrwxrwx   0 root         (0) root         (0)   339276 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/icons/icon-console.svg
--rwxrwxrwx   0 root         (0) root         (0)   339293 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/icons/icon-windowed.svg
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.040831 pyinstaller-6.6.0/news/
--rwxrwxrwx   0 root         (0) root         (0)       12 2023-09-30 18:27:19.000000 pyinstaller-6.6.0/news/.gitignore
--rwxrwxrwx   0 root         (0) root         (0)     2755 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/news/README.txt
--rwxrwxrwx   0 root         (0) root         (0)     1065 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/news/_template.rst
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.043271 pyinstaller-6.6.0/pyinstaller.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     8277 2024-04-13 09:53:10.000000 pyinstaller-6.6.0/pyinstaller.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)    67299 2024-04-13 09:53:10.000000 pyinstaller-6.6.0/pyinstaller.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2024-04-13 09:53:10.000000 pyinstaller-6.6.0/pyinstaller.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)      376 2024-04-13 09:53:10.000000 pyinstaller-6.6.0/pyinstaller.egg-info/entry_points.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2024-04-13 09:52:51.000000 pyinstaller-6.6.0/pyinstaller.egg-info/not-zip-safe
--rwxrwxrwx   0 root         (0) root         (0)      319 2024-04-13 09:53:10.000000 pyinstaller-6.6.0/pyinstaller.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       12 2024-04-13 09:53:10.000000 pyinstaller-6.6.0/pyinstaller.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)     2551 2024-02-10 12:19:40.000000 pyinstaller-6.6.0/pyproject.toml
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.044294 pyinstaller-6.6.0/release/
--rwxrwxrwx   0 root         (0) root         (0)     2036 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/release/README.rst
--rwxrwxrwx   0 root         (0) root         (0)      487 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/release/build-manylinux
--rwxrwxrwx   0 root         (0) root         (0)     4344 2024-02-10 13:48:07.000000 pyinstaller-6.6.0/release/release.fish
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.046455 pyinstaller-6.6.0/scripts/
--rwxrwxrwx   0 root         (0) root         (0)      166 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/scripts/clean
--rwxrwxrwx   0 root         (0) root         (0)       68 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/scripts/clean.bat
--rwxrwxrwx   0 root         (0) root         (0)     1876 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/scripts/find-empty-hooks.py
--rwxrwxrwx   0 root         (0) root         (0)     6327 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/scripts/update-copyright
--rwxrwxrwx   0 root         (0) root         (0)      362 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/scripts/update-readme-versions.sh
--rwxrwxrwx   0 root         (0) root         (0)     2048 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/scripts/verify-news-fragments.py
--rwxrwxrwx   0 root         (0) root         (0)     3980 2024-04-13 09:53:11.301500 pyinstaller-6.6.0/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)    10872 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.049171 pyinstaller-6.6.0/tests/
--rwxrwxrwx   0 root         (0) root         (0)     4442 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.067183 pyinstaller-6.6.0/tests/functional/
--rwxrwxrwx   0 root         (0) root         (0)      208 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/README
--rwxrwxrwx   0 root         (0) root         (0)       98 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/conftest.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:10.757237 pyinstaller-6.6.0/tests/functional/data/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.067766 pyinstaller-6.6.0/tests/functional/data/PIL_images/
--rwxrwxrwx   0 root         (0) root         (0)     5758 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/data/PIL_images/tinysample.tiff
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.068381 pyinstaller-6.6.0/tests/functional/data/Qt_Ui_file/
--rwxrwxrwx   0 root         (0) root         (0)      862 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/data/Qt_Ui_file/gui.ui
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.068885 pyinstaller-6.6.0/tests/functional/data/app_with_plugin/
--rwxrwxrwx   0 root         (0) root         (0)      624 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/data/app_with_plugin/static_plugin.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.073604 pyinstaller-6.6.0/tests/functional/data/appimage/
--rwxrwxrwx   0 root         (0) root         (0)   339293 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/data/appimage/AppIcon.svg
--rwxrwxrwx   0 root         (0) root         (0)    20448 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/data/appimage/DirIcon.png
--rwxrwxrwx   0 root         (0) root         (0)     1019 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/data/appimage/create.sh
--rwxrwxrwx   0 root         (0) root         (0)      775 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/data/appimage/org.pyinstaller.appimage.test.appdata.xml
--rwxrwxrwx   0 root         (0) root         (0)      243 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/data/appimage/org.pyinstaller.appimage.test.desktop
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.073942 pyinstaller-6.6.0/tests/functional/data/ctypes_dylib/
--rwxrwxrwx   0 root         (0) root         (0)      695 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/data/ctypes_dylib/ctypes_dylib.c
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.076806 pyinstaller-6.6.0/tests/functional/data/django/
--rwxrwxrwx   0 root         (0) root         (0)   131072 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/data/django/db.sqlite3
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.078750 pyinstaller-6.6.0/tests/functional/data/django/django_site/
--rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/data/django/django_site/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      399 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/data/django/django_site/asgi.py
--rwxrwxrwx   0 root         (0) root         (0)     3230 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/data/django/django_site/settings.py
--rwxrwxrwx   0 root         (0) root         (0)      753 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/data/django/django_site/urls.py
--rwxrwxrwx   0 root         (0) root         (0)      399 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/data/django/django_site/wsgi.py
--rwxrwxrwx   0 root         (0) root         (0)      667 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/data/django/manage.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.079033 pyinstaller-6.6.0/tests/functional/data/invalid_icon/
--rwxrwxrwx   0 root         (0) root         (0)      587 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/data/invalid_icon/pyi_icon.png
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.079318 pyinstaller-6.6.0/tests/functional/data/name_clash_with_entry_point/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.079847 pyinstaller-6.6.0/tests/functional/data/name_clash_with_entry_point/matching_name/
--rwxrwxrwx   0 root         (0) root         (0)       56 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/data/name_clash_with_entry_point/matching_name/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       57 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/data/name_clash_with_entry_point/matching_name/submodule.py
--rwxrwxrwx   0 root         (0) root         (0)       83 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/data/name_clash_with_entry_point/matching_name.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.080362 pyinstaller-6.6.0/tests/functional/data/requests/
--rwxrwxrwx   0 root         (0) root         (0)      294 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/data/requests/openssl.conf
--rwxrwxrwx   0 root         (0) root         (0)     5524 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/data/requests/server.pem
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.082452 pyinstaller-6.6.0/tests/functional/data/set_icon/
--rwxrwxrwx   0 root         (0) root         (0)   108027 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/data/set_icon/pyi_icon.icns
--rwxrwxrwx   0 root         (0) root         (0)    56493 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/data/set_icon/pyi_icon.ico
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.084265 pyinstaller-6.6.0/tests/functional/data/sphinx/
--rwxrwxrwx   0 root         (0) root         (0)     9476 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/data/sphinx/conf.py
--rwxrwxrwx   0 root         (0) root         (0)      489 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/data/sphinx/index.rst
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.084551 pyinstaller-6.6.0/tests/functional/data/splash/
--rwxrwxrwx   0 root         (0) root         (0)    20448 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/data/splash/image.png
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.091789 pyinstaller-6.6.0/tests/functional/logs/
--rwxrwxrwx   0 root         (0) root         (0)       66 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/logs/multipackage1_B.toc
--rwxrwxrwx   0 root         (0) root         (0)       41 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/logs/multipackage2_B.toc
--rwxrwxrwx   0 root         (0) root         (0)       78 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/logs/multipackage3_B.toc
--rwxrwxrwx   0 root         (0) root         (0)       41 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/logs/multipackage4_B.toc
--rwxrwxrwx   0 root         (0) root         (0)       41 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/logs/multipackage5_B.toc
--rwxrwxrwx   0 root         (0) root         (0)      146 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/logs/multipackage5_C.toc
--rwxrwxrwx   0 root         (0) root         (0)      375 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/logs/pyi_import_relative.toc
--rwxrwxrwx   0 root         (0) root         (0)       54 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/logs/test_hiddenimport.toc
--rwxrwxrwx   0 root         (0) root         (0)       74 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/logs/test_keyring.toc
--rwxrwxrwx   0 root         (0) root         (0)      117 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/logs/test_multipackage1.toc
--rwxrwxrwx   0 root         (0) root         (0)      149 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/logs/test_multipackage2.toc
--rwxrwxrwx   0 root         (0) root         (0)      117 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/logs/test_multipackage3.toc
--rwxrwxrwx   0 root         (0) root         (0)      149 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/logs/test_multipackage4.toc
--rwxrwxrwx   0 root         (0) root         (0)      149 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/logs/test_multipackage5.toc
--rwxrwxrwx   0 root         (0) root         (0)       79 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/logs/test_nspkg1.toc
--rwxrwxrwx   0 root         (0) root         (0)       49 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/logs/test_nspkg1_bbb_zzz.toc
--rwxrwxrwx   0 root         (0) root         (0)       15 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/logs/test_nspkg1_empty.toc
--rwxrwxrwx   0 root         (0) root         (0)       79 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/logs/test_nspkg2.toc
--rwxrwxrwx   0 root         (0) root         (0)       75 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/logs/test_nspkg3.toc
--rwxrwxrwx   0 root         (0) root         (0)       30 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/logs/test_nspkg3_aaa.toc
--rwxrwxrwx   0 root         (0) root         (0)       49 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/logs/test_nspkg3_bbb_zzz.toc
--rwxrwxrwx   0 root         (0) root         (0)       15 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/logs/test_nspkg3_empty.toc
--rwxrwxrwx   0 root         (0) root         (0)      140 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/logs/test_nspkg_pep420.toc
--rwxrwxrwx   0 root         (0) root         (0)      221 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/logs/test_option_verbose.toc
--rwxrwxrwx   0 root         (0) root         (0)       14 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/logs/test_pil_FixTk.toc
--rwxrwxrwx   0 root         (0) root         (0)       32 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/logs/test_pil_PyQt5.toc
--rwxrwxrwx   0 root         (0) root         (0)       44 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/logs/test_pkg_without_hook_for_pkg.toc
--rwxrwxrwx   0 root         (0) root         (0)       14 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/logs/test_tkinter_FixTk.toc
--rwxrwxrwx   0 root         (0) root         (0)       35 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/logs/test_zope_interface.toc
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.096430 pyinstaller-6.6.0/tests/functional/modules/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.097458 pyinstaller-6.6.0/tests/functional/modules/a_hidden_import/
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/a_hidden_import/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/a_hidden_import/submodule.py
--rwxrwxrwx   0 root         (0) root         (0)      523 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/error_during_import2.py
--rwxrwxrwx   0 root         (0) root         (0)      547 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/module_with_coding_utf8.py
--rwxrwxrwx   0 root         (0) root         (0)      615 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/module_with_utf8_emoji.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:10.757618 pyinstaller-6.6.0/tests/functional/modules/nspkg-pep420/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:10.757548 pyinstaller-6.6.0/tests/functional/modules/nspkg-pep420/path1/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.097823 pyinstaller-6.6.0/tests/functional/modules/nspkg-pep420/path1/package/
--rwxrwxrwx   0 root         (0) root         (0)       21 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/nspkg-pep420/path1/package/sub2.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:10.757648 pyinstaller-6.6.0/tests/functional/modules/nspkg-pep420/path2/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.098102 pyinstaller-6.6.0/tests/functional/modules/nspkg-pep420/path2/package/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.098375 pyinstaller-6.6.0/tests/functional/modules/nspkg-pep420/path2/package/nspkg/
--rwxrwxrwx   0 root         (0) root         (0)       26 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/nspkg-pep420/path2/package/nspkg/mod.py
--rwxrwxrwx   0 root         (0) root         (0)       21 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/nspkg-pep420/path2/package/sub1.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.098952 pyinstaller-6.6.0/tests/functional/modules/nspkg-pep420/path2/package/subpackage/
--rwxrwxrwx   0 root         (0) root         (0)       27 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/nspkg-pep420/path2/package/subpackage/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       31 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/nspkg-pep420/path2/package/subpackage/sub.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.099726 pyinstaller-6.6.0/tests/functional/modules/nspkg1-pkg/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:10.757979 pyinstaller-6.6.0/tests/functional/modules/nspkg1-pkg/nspkg1_aaa.egg/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.101668 pyinstaller-6.6.0/tests/functional/modules/nspkg1-pkg/nspkg1_aaa.egg/EGG-INFO/
--rwxrwxrwx   0 root         (0) root         (0)      205 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/nspkg1-pkg/nspkg1_aaa.egg/EGG-INFO/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      262 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/nspkg1-pkg/nspkg1_aaa.egg/EGG-INFO/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/nspkg1-pkg/nspkg1_aaa.egg/EGG-INFO/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)        7 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/nspkg1-pkg/nspkg1_aaa.egg/EGG-INFO/namespace_packages.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/nspkg1-pkg/nspkg1_aaa.egg/EGG-INFO/not-zip-safe
--rwxrwxrwx   0 root         (0) root         (0)        7 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/nspkg1-pkg/nspkg1_aaa.egg/EGG-INFO/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.101913 pyinstaller-6.6.0/tests/functional/modules/nspkg1-pkg/nspkg1_aaa.egg/nspkg1/
--rwxrwxrwx   0 root         (0) root         (0)       64 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/nspkg1-pkg/nspkg1_aaa.egg/nspkg1/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.102266 pyinstaller-6.6.0/tests/functional/modules/nspkg1-pkg/nspkg1_aaa.egg/nspkg1/aaa/
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/nspkg1-pkg/nspkg1_aaa.egg/nspkg1/aaa/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1545 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/nspkg1-pkg/nspkg1_bbb.egg
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:10.758197 pyinstaller-6.6.0/tests/functional/modules/nspkg1-pkg/nspkg1_ccc.egg/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.104140 pyinstaller-6.6.0/tests/functional/modules/nspkg1-pkg/nspkg1_ccc.egg/EGG-INFO/
--rwxrwxrwx   0 root         (0) root         (0)      205 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/nspkg1-pkg/nspkg1_ccc.egg/EGG-INFO/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      253 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/nspkg1-pkg/nspkg1_ccc.egg/EGG-INFO/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/nspkg1-pkg/nspkg1_ccc.egg/EGG-INFO/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)        7 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/nspkg1-pkg/nspkg1_ccc.egg/EGG-INFO/namespace_packages.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/nspkg1-pkg/nspkg1_ccc.egg/EGG-INFO/not-zip-safe
--rwxrwxrwx   0 root         (0) root         (0)        7 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/nspkg1-pkg/nspkg1_ccc.egg/EGG-INFO/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.104766 pyinstaller-6.6.0/tests/functional/modules/nspkg1-pkg/nspkg1_ccc.egg/nspkg1/
--rwxrwxrwx   0 root         (0) root         (0)       64 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/nspkg1-pkg/nspkg1_ccc.egg/nspkg1/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/nspkg1-pkg/nspkg1_ccc.egg/nspkg1/ccc.py
--rwxrwxrwx   0 root         (0) root         (0)     1193 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/nspkg1-pkg/nspkg1_empty.egg
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.106308 pyinstaller-6.6.0/tests/functional/modules/nspkg2-pkg/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.106638 pyinstaller-6.6.0/tests/functional/modules/nspkg2-pkg/nspkg2/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.106958 pyinstaller-6.6.0/tests/functional/modules/nspkg2-pkg/nspkg2/aaa/
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/nspkg2-pkg/nspkg2/aaa/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:10.758475 pyinstaller-6.6.0/tests/functional/modules/nspkg2-pkg/nspkg2/bbb/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.107278 pyinstaller-6.6.0/tests/functional/modules/nspkg2-pkg/nspkg2/bbb/zzz/
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/nspkg2-pkg/nspkg2/bbb/zzz/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/nspkg2-pkg/nspkg2/ccc.py
--rwxrwxrwx   0 root         (0) root         (0)      307 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/nspkg2-pkg/nspkg2_aaa-nspkg.pth
--rwxrwxrwx   0 root         (0) root         (0)      676 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/nspkg2-pkg/nspkg2_bbb-nspkg.pth
--rwxrwxrwx   0 root         (0) root         (0)      307 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/nspkg2-pkg/nspkg2_ccc-nspkg.pth
--rwxrwxrwx   0 root         (0) root         (0)      305 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/nspkg2-pkg/nspkg2_empty-nspkg.pth
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.108167 pyinstaller-6.6.0/tests/functional/modules/nspkg3-pkg/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:10.758715 pyinstaller-6.6.0/tests/functional/modules/nspkg3-pkg/nspkg3_aaa.egg/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.110427 pyinstaller-6.6.0/tests/functional/modules/nspkg3-pkg/nspkg3_aaa.egg/EGG-INFO/
--rwxrwxrwx   0 root         (0) root         (0)      205 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/nspkg3-pkg/nspkg3_aaa.egg/EGG-INFO/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      262 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/nspkg3-pkg/nspkg3_aaa.egg/EGG-INFO/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/nspkg3-pkg/nspkg3_aaa.egg/EGG-INFO/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)        7 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/nspkg3-pkg/nspkg3_aaa.egg/EGG-INFO/namespace_packages.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/nspkg3-pkg/nspkg3_aaa.egg/EGG-INFO/not-zip-safe
--rwxrwxrwx   0 root         (0) root         (0)        7 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/nspkg3-pkg/nspkg3_aaa.egg/EGG-INFO/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.110737 pyinstaller-6.6.0/tests/functional/modules/nspkg3-pkg/nspkg3_aaa.egg/nspkg3/
--rwxrwxrwx   0 root         (0) root         (0)       76 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/nspkg3-pkg/nspkg3_aaa.egg/nspkg3/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.111045 pyinstaller-6.6.0/tests/functional/modules/nspkg3-pkg/nspkg3_aaa.egg/nspkg3/aaa/
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/nspkg3-pkg/nspkg3_aaa.egg/nspkg3/aaa/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1560 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/nspkg3-pkg/nspkg3_bbb.egg
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:10.758937 pyinstaller-6.6.0/tests/functional/modules/nspkg3-pkg/nspkg3_ccc.egg/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.112919 pyinstaller-6.6.0/tests/functional/modules/nspkg3-pkg/nspkg3_ccc.egg/EGG-INFO/
--rwxrwxrwx   0 root         (0) root         (0)      205 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/nspkg3-pkg/nspkg3_ccc.egg/EGG-INFO/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      253 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/nspkg3-pkg/nspkg3_ccc.egg/EGG-INFO/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/nspkg3-pkg/nspkg3_ccc.egg/EGG-INFO/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)        7 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/nspkg3-pkg/nspkg3_ccc.egg/EGG-INFO/namespace_packages.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/nspkg3-pkg/nspkg3_ccc.egg/EGG-INFO/not-zip-safe
--rwxrwxrwx   0 root         (0) root         (0)        7 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/nspkg3-pkg/nspkg3_ccc.egg/EGG-INFO/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.113535 pyinstaller-6.6.0/tests/functional/modules/nspkg3-pkg/nspkg3_ccc.egg/nspkg3/
--rwxrwxrwx   0 root         (0) root         (0)       76 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/nspkg3-pkg/nspkg3_ccc.egg/nspkg3/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/nspkg3-pkg/nspkg3_ccc.egg/nspkg3/ccc.py
--rwxrwxrwx   0 root         (0) root         (0)     1202 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/nspkg3-pkg/nspkg3_empty.egg
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.114157 pyinstaller-6.6.0/tests/functional/modules/pkg3/
--rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pkg3/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       57 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pkg3/sample-data.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.114468 pyinstaller-6.6.0/tests/functional/modules/pkg_without_hook_for_pkg/
--rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pkg_without_hook_for_pkg/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.114777 pyinstaller-6.6.0/tests/functional/modules/pkg_without_hook_for_pkg/sub1/
--rwxrwxrwx   0 root         (0) root         (0)      281 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pkg_without_hook_for_pkg/sub1/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.115088 pyinstaller-6.6.0/tests/functional/modules/pkg_without_hook_for_pkg/sub1/sub11/
--rwxrwxrwx   0 root         (0) root         (0)       31 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pkg_without_hook_for_pkg/sub1/sub11/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      577 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_collect_submodules_mod.py
--rwxrwxrwx   0 root         (0) root         (0)      230 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_dummy_module.py
--rwxrwxrwx   0 root         (0) root         (0)     1399 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_egg_zipped.egg
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:10.759374 pyinstaller-6.6.0/tests/functional/modules/pyi_excluded_relative_imports/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.115413 pyinstaller-6.6.0/tests/functional/modules/pyi_excluded_relative_imports/hooks/
--rwxrwxrwx   0 root         (0) root         (0)      165 2023-11-11 15:22:30.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_excluded_relative_imports/hooks/hook-mypackage.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.116329 pyinstaller-6.6.0/tests/functional/modules/pyi_excluded_relative_imports/mypackage/
--rwxrwxrwx   0 root         (0) root         (0)      636 2023-11-11 15:22:30.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_excluded_relative_imports/mypackage/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      130 2023-11-11 15:22:30.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_excluded_relative_imports/mypackage/forbidden1.py
--rwxrwxrwx   0 root         (0) root         (0)      437 2023-11-11 15:22:30.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_excluded_relative_imports/mypackage/submod1.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.117260 pyinstaller-6.6.0/tests/functional/modules/pyi_excluded_relative_imports/mypackage/subpkg1/
--rwxrwxrwx   0 root         (0) root         (0)      545 2023-11-11 15:22:30.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_excluded_relative_imports/mypackage/subpkg1/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      130 2023-11-11 15:22:30.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_excluded_relative_imports/mypackage/subpkg1/forbidden2.py
--rwxrwxrwx   0 root         (0) root         (0)      426 2023-11-11 15:22:30.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_excluded_relative_imports/mypackage/subpkg1/submod2.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.118180 pyinstaller-6.6.0/tests/functional/modules/pyi_excluded_relative_imports/mypackage/subpkg1/subpkg2/
--rwxrwxrwx   0 root         (0) root         (0)      538 2023-11-11 15:22:30.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_excluded_relative_imports/mypackage/subpkg1/subpkg2/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      130 2023-11-11 15:22:30.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_excluded_relative_imports/mypackage/subpkg1/subpkg2/forbidden3.py
--rwxrwxrwx   0 root         (0) root         (0)      424 2023-11-11 15:22:30.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_excluded_relative_imports/mypackage/subpkg1/subpkg2/submod3.py
--rwxrwxrwx   0 root         (0) root         (0)     1277 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_get_datadir.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:10.759601 pyinstaller-6.6.0/tests/functional/modules/pyi_import_main/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.118815 pyinstaller-6.6.0/tests/functional/modules/pyi_import_main/hooks/
--rwxrwxrwx   0 root         (0) root         (0)       94 2023-10-12 17:16:14.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_import_main/hooks/hook-PyInstaller.py
--rwxrwxrwx   0 root         (0) root         (0)       84 2023-10-12 17:16:14.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_import_main/hooks/hook-pytest.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:10.759715 pyinstaller-6.6.0/tests/functional/modules/pyi_import_pyqt_uic_port/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.119431 pyinstaller-6.6.0/tests/functional/modules/pyi_import_pyqt_uic_port/PyQt5/
--rwxrwxrwx   0 root         (0) root         (0)      371 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_import_pyqt_uic_port/PyQt5/QtCore.py
--rwxrwxrwx   0 root         (0) root         (0)       88 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_import_pyqt_uic_port/PyQt5/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.119740 pyinstaller-6.6.0/tests/functional/modules/pyi_import_pyqt_uic_port/PyQt5/uic/
--rwxrwxrwx   0 root         (0) root         (0)      118 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_import_pyqt_uic_port/PyQt5/uic/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.120358 pyinstaller-6.6.0/tests/functional/modules/pyi_import_pyqt_uic_port/PyQt5/uic/port_v2/
--rwxrwxrwx   0 root         (0) root         (0)      148 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_import_pyqt_uic_port/PyQt5/uic/port_v2/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      151 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_import_pyqt_uic_port/PyQt5/uic/port_v2/test.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.120972 pyinstaller-6.6.0/tests/functional/modules/pyi_import_pyqt_uic_port/PyQt5/uic/port_v3/
--rwxrwxrwx   0 root         (0) root         (0)      148 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_import_pyqt_uic_port/PyQt5/uic/port_v3/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      152 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_import_pyqt_uic_port/PyQt5/uic/port_v3/test.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:10.759999 pyinstaller-6.6.0/tests/functional/modules/pyi_inspect_getmodule_from_stackframes/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.121592 pyinstaller-6.6.0/tests/functional/modules/pyi_inspect_getmodule_from_stackframes/helper_package/
--rwxrwxrwx   0 root         (0) root         (0)      138 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_inspect_getmodule_from_stackframes/helper_package/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      290 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_inspect_getmodule_from_stackframes/helper_package/helper_module.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:10.760108 pyinstaller-6.6.0/tests/functional/modules/pyi_issue_4141/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.121917 pyinstaller-6.6.0/tests/functional/modules/pyi_issue_4141/app/
--rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_issue_4141/app/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:10.760333 pyinstaller-6.6.0/tests/functional/modules/pyi_missing_relative_import/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.122258 pyinstaller-6.6.0/tests/functional/modules/pyi_missing_relative_import/hooks/
--rwxrwxrwx   0 root         (0) root         (0)       55 2023-11-04 13:41:36.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_missing_relative_import/hooks/hook-myotherpackage.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.122565 pyinstaller-6.6.0/tests/functional/modules/pyi_missing_relative_import/myotherpackage/
--rwxrwxrwx   0 root         (0) root         (0)       22 2023-11-04 13:41:36.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_missing_relative_import/myotherpackage/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.122868 pyinstaller-6.6.0/tests/functional/modules/pyi_missing_relative_import/mypackage/
--rwxrwxrwx   0 root         (0) root         (0)      391 2023-11-04 13:41:36.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_missing_relative_import/mypackage/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:10.760514 pyinstaller-6.6.0/tests/functional/modules/pyi_module_exclusion/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.124108 pyinstaller-6.6.0/tests/functional/modules/pyi_module_exclusion/hooks/
--rwxrwxrwx   0 root         (0) root         (0)       65 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_module_exclusion/hooks/hook-mymodule_feature1.py
--rwxrwxrwx   0 root         (0) root         (0)      387 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_module_exclusion/hooks/hook-mymodule_feature2.py
--rwxrwxrwx   0 root         (0) root         (0)      507 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_module_exclusion/hooks/hook-mymodule_feature3.py
--rwxrwxrwx   0 root         (0) root         (0)      155 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_module_exclusion/hooks/hook-mymodule_main.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:10.760666 pyinstaller-6.6.0/tests/functional/modules/pyi_module_exclusion/modules/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.124428 pyinstaller-6.6.0/tests/functional/modules/pyi_module_exclusion/modules/mymodule_feature1/
--rwxrwxrwx   0 root         (0) root         (0)       22 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_module_exclusion/modules/mymodule_feature1/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.124736 pyinstaller-6.6.0/tests/functional/modules/pyi_module_exclusion/modules/mymodule_feature2/
--rwxrwxrwx   0 root         (0) root         (0)       22 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_module_exclusion/modules/mymodule_feature2/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.125640 pyinstaller-6.6.0/tests/functional/modules/pyi_module_exclusion/modules/mymodule_main/
--rwxrwxrwx   0 root         (0) root         (0)      619 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_module_exclusion/modules/mymodule_main/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      210 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_module_exclusion/modules/mymodule_main/submodule_feature3.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.126567 pyinstaller-6.6.0/tests/functional/modules/pyi_module_with_invalid_encoding/
--rwxrwxrwx   0 root         (0) root         (0)      885 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_module_with_invalid_encoding/mymodule1.py
--rwxrwxrwx   0 root         (0) root         (0)     1666 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_module_with_invalid_encoding/mymodule2.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:10.760906 pyinstaller-6.6.0/tests/functional/modules/pyi_namespace_package_with_data/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.127192 pyinstaller-6.6.0/tests/functional/modules/pyi_namespace_package_with_data/hooks/
--rwxrwxrwx   0 root         (0) root         (0)      174 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_namespace_package_with_data/hooks/hook-pyi_test_nspkg.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:10.760938 pyinstaller-6.6.0/tests/functional/modules/pyi_namespace_package_with_data/package/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.127885 pyinstaller-6.6.0/tests/functional/modules/pyi_namespace_package_with_data/package/pyi_test_nspkg/
--rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_namespace_package_with_data/package/pyi_test_nspkg/a.py
--rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_namespace_package_with_data/package/pyi_test_nspkg/b.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.128886 pyinstaller-6.6.0/tests/functional/modules/pyi_namespace_package_with_data/package/pyi_test_nspkg/data/
--rwxrwxrwx   0 root         (0) root         (0)       14 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_namespace_package_with_data/package/pyi_test_nspkg/data/data_file1.txt
--rwxrwxrwx   0 root         (0) root         (0)       14 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_namespace_package_with_data/package/pyi_test_nspkg/data/data_file2.txt
--rwxrwxrwx   0 root         (0) root         (0)       14 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_namespace_package_with_data/package/pyi_test_nspkg/data/data_file3.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:10.761114 pyinstaller-6.6.0/tests/functional/modules/pyi_optimization/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.129200 pyinstaller-6.6.0/tests/functional/modules/pyi_optimization/mypackage/
--rwxrwxrwx   0 root         (0) root         (0)      864 2024-04-04 21:05:01.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_optimization/mypackage/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:10.761284 pyinstaller-6.6.0/tests/functional/modules/pyi_pkg_resources_provider/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.129749 pyinstaller-6.6.0/tests/functional/modules/pyi_pkg_resources_provider/hooks/
--rwxrwxrwx   0 root         (0) root         (0)      642 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_pkg_resources_provider/hooks/hook-pyi_pkgres_testpkg.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.130080 pyinstaller-6.6.0/tests/functional/modules/pyi_pkg_resources_provider/package/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.131376 pyinstaller-6.6.0/tests/functional/modules/pyi_pkg_resources_provider/package/pyi_pkgres_testpkg/
--rwxrwxrwx   0 root         (0) root         (0)       87 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_pkg_resources_provider/package/pyi_pkgres_testpkg/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_pkg_resources_provider/package/pyi_pkgres_testpkg/a.py
--rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_pkg_resources_provider/package/pyi_pkgres_testpkg/b.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.132389 pyinstaller-6.6.0/tests/functional/modules/pyi_pkg_resources_provider/package/pyi_pkgres_testpkg/subpkg1/
--rwxrwxrwx   0 root         (0) root         (0)       33 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_pkg_resources_provider/package/pyi_pkgres_testpkg/subpkg1/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_pkg_resources_provider/package/pyi_pkgres_testpkg/subpkg1/c.py
--rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_pkg_resources_provider/package/pyi_pkgres_testpkg/subpkg1/d.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.133317 pyinstaller-6.6.0/tests/functional/modules/pyi_pkg_resources_provider/package/pyi_pkgres_testpkg/subpkg1/data/
--rwxrwxrwx   0 root         (0) root         (0)       31 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_pkg_resources_provider/package/pyi_pkgres_testpkg/subpkg1/data/entry1.txt
--rwxrwxrwx   0 root         (0) root         (0)       33 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_pkg_resources_provider/package/pyi_pkgres_testpkg/subpkg1/data/entry2.md
--rwxrwxrwx   0 root         (0) root         (0)       35 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_pkg_resources_provider/package/pyi_pkgres_testpkg/subpkg1/data/entry3.rst
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.133627 pyinstaller-6.6.0/tests/functional/modules/pyi_pkg_resources_provider/package/pyi_pkgres_testpkg/subpkg1/data/extra/
--rwxrwxrwx   0 root         (0) root         (0)       63 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_pkg_resources_provider/package/pyi_pkgres_testpkg/subpkg1/data/extra/extra_entry1.json
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.134249 pyinstaller-6.6.0/tests/functional/modules/pyi_pkg_resources_provider/package/pyi_pkgres_testpkg/subpkg2/
--rwxrwxrwx   0 root         (0) root         (0)       72 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_pkg_resources_provider/package/pyi_pkgres_testpkg/subpkg2/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_pkg_resources_provider/package/pyi_pkgres_testpkg/subpkg2/mod.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.134867 pyinstaller-6.6.0/tests/functional/modules/pyi_pkg_resources_provider/package/pyi_pkgres_testpkg/subpkg2/subsubpkg21/
--rwxrwxrwx   0 root         (0) root         (0)       32 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_pkg_resources_provider/package/pyi_pkgres_testpkg/subpkg2/subsubpkg21/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_pkg_resources_provider/package/pyi_pkgres_testpkg/subpkg2/subsubpkg21/mod.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.135501 pyinstaller-6.6.0/tests/functional/modules/pyi_pkg_resources_provider/package/pyi_pkgres_testpkg/subpkg3/
--rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_pkg_resources_provider/package/pyi_pkgres_testpkg/subpkg3/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       42 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_pkg_resources_provider/package/pyi_pkgres_testpkg/subpkg3/_datafile.json
--rwxrwxrwx   0 root         (0) root         (0)     1128 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_pkg_resources_provider/package/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:10.761891 pyinstaller-6.6.0/tests/functional/modules/pyi_pkgutil_itermodules/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.135818 pyinstaller-6.6.0/tests/functional/modules/pyi_pkgutil_itermodules/hooks/
--rwxrwxrwx   0 root         (0) root         (0)      672 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_pkgutil_itermodules/hooks/hook-mypackage.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:10.761923 pyinstaller-6.6.0/tests/functional/modules/pyi_pkgutil_itermodules/package/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.137735 pyinstaller-6.6.0/tests/functional/modules/pyi_pkgutil_itermodules/package/mypackage/
--rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_pkgutil_itermodules/package/mypackage/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       22 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_pkgutil_itermodules/package/mypackage/datafile.txt
--rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_pkgutil_itermodules/package/mypackage/submodule_a.py
--rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_pkgutil_itermodules/package/mypackage/submodule_b.py
--rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_pkgutil_itermodules/package/mypackage/submodule_c.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.138366 pyinstaller-6.6.0/tests/functional/modules/pyi_single_file_metadata/
--rwxrwxrwx   0 root         (0) root         (0)      196 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_single_file_metadata/README
--rwxrwxrwx   0 root         (0) root         (0)      290 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_single_file_metadata/my_test_package-1.0.egg-info
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:10.762186 pyinstaller-6.6.0/tests/functional/modules/pyi_test_egg/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.138688 pyinstaller-6.6.0/tests/functional/modules/pyi_test_egg/hooks/
--rwxrwxrwx   0 root         (0) root         (0)       99 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_test_egg/hooks/hook-unzipped_egg.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:10.762275 pyinstaller-6.6.0/tests/functional/modules/pyi_test_egg/pyi_egg_unzipped.egg/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.140255 pyinstaller-6.6.0/tests/functional/modules/pyi_test_egg/pyi_egg_unzipped.egg/EGG-INFO/
--rwxrwxrwx   0 root         (0) root         (0)      215 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_test_egg/pyi_egg_unzipped.egg/EGG-INFO/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      232 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_test_egg/pyi_egg_unzipped.egg/EGG-INFO/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_test_egg/pyi_egg_unzipped.egg/EGG-INFO/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_test_egg/pyi_egg_unzipped.egg/EGG-INFO/not-zip-safe
--rwxrwxrwx   0 root         (0) root         (0)       13 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_test_egg/pyi_egg_unzipped.egg/EGG-INFO/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.140569 pyinstaller-6.6.0/tests/functional/modules/pyi_test_egg/pyi_egg_unzipped.egg/unzipped_egg/
--rwxrwxrwx   0 root         (0) root         (0)      678 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_test_egg/pyi_egg_unzipped.egg/unzipped_egg/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.141123 pyinstaller-6.6.0/tests/functional/modules/pyi_test_egg/pyi_egg_unzipped.egg/unzipped_egg/data/
--rwxrwxrwx   0 root         (0) root         (0)       34 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_test_egg/pyi_egg_unzipped.egg/unzipped_egg/data/datafile.txt
--rwxrwxrwx   0 root         (0) root         (0)     1139 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_dynamic.py
--rwxrwxrwx   0 root         (0) root         (0)     1311 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_gettemp.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.141450 pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_metapath1/
--rwxrwxrwx   0 root         (0) root         (0)     1654 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_metapath1/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.142575 pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_metapath1/_vendor/
--rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_metapath1/_vendor/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      558 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_metapath1/_vendor/aaa.py
--rwxrwxrwx   0 root         (0) root         (0)      558 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_metapath1/_vendor/bbb.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.143211 pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_metapath1/_vendor/ccc/
--rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_metapath1/_vendor/ccc/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      817 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_metapath1/_vendor/ccc/ddd.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.144119 pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_metapath1/_vendor/ccc/eee/
--rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_metapath1/_vendor/ccc/eee/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      555 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_metapath1/_vendor/ccc/eee/fff.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.144446 pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_metapath1/extern/
--rwxrwxrwx   0 root         (0) root         (0)     4109 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_metapath1/extern/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.145132 pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_missing_submod/
--rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_missing_submod/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.145490 pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_missing_submod/aaa/
--rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_missing_submod/aaa/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.146171 pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_nameclash/
--rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_nameclash/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       57 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_nameclash/nameclash.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.147039 pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_path/
--rwxrwxrwx   0 root         (0) root         (0)      697 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_path/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.147363 pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_path/a/
--rwxrwxrwx   0 root         (0) root         (0)      507 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_path/a/b.py
--rwxrwxrwx   0 root         (0) root         (0)      525 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_path/b.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.148982 pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_relimp/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.150260 pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_relimp/B/
--rwxrwxrwx   0 root         (0) root         (0)     1030 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_relimp/B/C.py
--rwxrwxrwx   0 root         (0) root         (0)      589 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_relimp/B/D.py
--rwxrwxrwx   0 root         (0) root         (0)      538 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_relimp/B/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      538 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_relimp/E.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.150933 pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_relimp/F/
--rwxrwxrwx   0 root         (0) root         (0)      540 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_relimp/F/G.py
--rwxrwxrwx   0 root         (0) root         (0)      585 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_relimp/F/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      536 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_relimp/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.152221 pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_relimp/pyi_testmod_relimp/
--rwxrwxrwx   0 root         (0) root         (0)      555 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_relimp/pyi_testmod_relimp/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1251 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_relimp/pyi_testmod_relimp/relimp2.py
--rwxrwxrwx   0 root         (0) root         (0)      563 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_relimp/pyi_testmod_relimp/relimp3.py
--rwxrwxrwx   0 root         (0) root         (0)      945 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_relimp/relimp1.py
--rwxrwxrwx   0 root         (0) root         (0)      544 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_relimp/relimp2.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.152553 pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_relimp2/
--rwxrwxrwx   0 root         (0) root         (0)      507 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_relimp2/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.153214 pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_relimp2/bar/
--rwxrwxrwx   0 root         (0) root         (0)      556 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_relimp2/bar/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.153548 pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_relimp2/bar/bar2/
--rwxrwxrwx   0 root         (0) root         (0)      557 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_relimp2/bar/bar2/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      559 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_relimp2/bar/baz.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.154168 pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_relimp3a/
--rwxrwxrwx   0 root         (0) root         (0)      507 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_relimp3a/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.155402 pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_relimp3a/aa/
--rwxrwxrwx   0 root         (0) root         (0)      507 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_relimp3a/aa/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      853 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_relimp3a/aa/a1.py
--rwxrwxrwx   0 root         (0) root         (0)      547 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_relimp3a/aa/pyi_testmod_relimp3c.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.156053 pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_relimp3a/pyi_testmod_relimp3b/
--rwxrwxrwx   0 root         (0) root         (0)      507 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_relimp3a/pyi_testmod_relimp3b/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      540 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_relimp3a/pyi_testmod_relimp3b/b1.py
--rwxrwxrwx   0 root         (0) root         (0)      525 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_relimp3a/pyi_testmod_relimp3c.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.156706 pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_relimp3b/
--rwxrwxrwx   0 root         (0) root         (0)      507 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_relimp3b/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      525 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_relimp3b/b1.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.157028 pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_relimp3c/
--rwxrwxrwx   0 root         (0) root         (0)      527 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_relimp3c/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.157641 pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_submodule_from_aliased_pkg/
--rwxrwxrwx   0 root         (0) root         (0)        3 2023-11-23 19:10:52.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_submodule_from_aliased_pkg/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)        3 2023-11-23 19:10:52.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_submodule_from_aliased_pkg/submodule.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.158556 pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_submodule_global_shadowed/
--rwxrwxrwx   0 root         (0) root         (0)      963 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_submodule_global_shadowed/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      750 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_submodule_global_shadowed/submodule.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.159664 pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_submodule_global_unshadowed/
--rwxrwxrwx   0 root         (0) root         (0)     1605 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_submodule_global_unshadowed/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      756 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_submodule_global_unshadowed/submodule.py
--rwxrwxrwx   0 root         (0) root         (0)      611 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_threading.py
--rwxrwxrwx   0 root         (0) root         (0)      703 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/modules/resources_testmod.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.191085 pyinstaller-6.6.0/tests/functional/scripts/
--rwxrwxrwx   0 root         (0) root         (0)      706 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/scripts/list_pytest11_entry_point.py
--rwxrwxrwx   0 root         (0) root         (0)     1155 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/scripts/pkg_resource_res_string.py
--rwxrwxrwx   0 root         (0) root         (0)      914 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/scripts/pkgutil_get_data.py
--rwxrwxrwx   0 root         (0) root         (0)      896 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/scripts/pkgutil_get_data__main__.py
--rwxrwxrwx   0 root         (0) root         (0)     1490 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/scripts/pyi_absolute_ld_library_path.py
--rwxrwxrwx   0 root         (0) root         (0)     1221 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/scripts/pyi_absolute_python_path.py
--rwxrwxrwx   0 root         (0) root         (0)     1948 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/scripts/pyi_app_with_plugin.py
--rwxrwxrwx   0 root         (0) root         (0)      177 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/scripts/pyi_arbitrary_ext.foo
--rwxrwxrwx   0 root         (0) root         (0)     1559 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/scripts/pyi_c_extension.py
--rwxrwxrwx   0 root         (0) root         (0)      870 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/scripts/pyi_codecs.py
--rwxrwxrwx   0 root         (0) root         (0)      634 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/scripts/pyi_filename.py
--rwxrwxrwx   0 root         (0) root         (0)     1824 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/scripts/pyi_frozen_stdlib_modules.py
--rwxrwxrwx   0 root         (0) root         (0)     3636 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/scripts/pyi_future.py
--rwxrwxrwx   0 root         (0) root         (0)     1325 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/scripts/pyi_get_meipass_value.py
--rwxrwxrwx   0 root         (0) root         (0)     1138 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/scripts/pyi_getfilesystemencoding.py
--rwxrwxrwx   0 root         (0) root         (0)      531 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/scripts/pyi_helloworld.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.193340 pyinstaller-6.6.0/tests/functional/scripts/pyi_hooks/
--rwxrwxrwx   0 root         (0) root         (0)       56 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/scripts/pyi_hooks/hook-pkg_without_hook_for_pkg.sub1.py
--rwxrwxrwx   0 root         (0) root         (0)      621 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/scripts/pyi_hooks/hook-pyi_collect_submodules_mod.py
--rwxrwxrwx   0 root         (0) root         (0)      770 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/scripts/pyi_hooks/hook-pyi_testmod_metapath1.py
--rwxrwxrwx   0 root         (0) root         (0)      821 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/scripts/pyi_hooks/hook-pyi_testmod_path.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.193935 pyinstaller-6.6.0/tests/functional/scripts/pyi_hooks/pre_safe_import_module/
--rwxrwxrwx   0 root         (0) root         (0)      524 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/scripts/pyi_hooks/pre_safe_import_module/hook-alias_name.py
--rwxrwxrwx   0 root         (0) root         (0)     1266 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/scripts/pyi_import_pyqt5_uic_port.py
--rwxrwxrwx   0 root         (0) root         (0)    16548 2024-03-24 20:46:04.000000 pyinstaller-6.6.0/tests/functional/scripts/pyi_importlib_resources.py
--rwxrwxrwx   0 root         (0) root         (0)     1191 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/scripts/pyi_interact_pyi_splash.py
--rwxrwxrwx   0 root         (0) root         (0)     1329 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/scripts/pyi_issue_4141.py
--rwxrwxrwx   0 root         (0) root         (0)     1093 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/scripts/pyi_lazy_import.py
--rwxrwxrwx   0 root         (0) root         (0)      774 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/scripts/pyi_lib_PIL_img_conversion.py
--rwxrwxrwx   0 root         (0) root         (0)     1031 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/scripts/pyi_lib_PyQt5-uic.py
--rwxrwxrwx   0 root         (0) root         (0)     3112 2023-11-04 13:41:36.000000 pyinstaller-6.6.0/tests/functional/scripts/pyi_lib_requests.py
--rwxrwxrwx   0 root         (0) root         (0)     1401 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/scripts/pyi_lib_sphinx.py
--rwxrwxrwx   0 root         (0) root         (0)     2161 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/scripts/pyi_lib_tkinter.py
--rwxrwxrwx   0 root         (0) root         (0)     1058 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/scripts/pyi_load_dll_using_ctypes.py
--rwxrwxrwx   0 root         (0) root         (0)     1334 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/scripts/pyi_module__file__attribute.py
--rwxrwxrwx   0 root         (0) root         (0)     2556 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/scripts/pyi_module_attributes.py
--rwxrwxrwx   0 root         (0) root         (0)     1383 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/scripts/pyi_module_reload.py
--rwxrwxrwx   0 root         (0) root         (0)     1254 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/scripts/pyi_multiprocessing_main_module_code_in_process.py
--rwxrwxrwx   0 root         (0) root         (0)     2028 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/scripts/pyi_multiprocessing_nested_process.py
--rwxrwxrwx   0 root         (0) root         (0)     1178 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/scripts/pyi_multiprocessing_pool.py
--rwxrwxrwx   0 root         (0) root         (0)     1198 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/scripts/pyi_multiprocessing_process.py
--rwxrwxrwx   0 root         (0) root         (0)     2397 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/scripts/pyi_multiprocessing_process_start_in_threads.py
--rwxrwxrwx   0 root         (0) root         (0)     1593 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/scripts/pyi_multiprocessing_queue.py
--rwxrwxrwx   0 root         (0) root         (0)     1171 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/scripts/pyi_multiprocessing_semaphore.py
--rwxrwxrwx   0 root         (0) root         (0)     1663 2024-04-04 21:05:01.000000 pyinstaller-6.6.0/tests/functional/scripts/pyi_optimization.py
--rwxrwxrwx   0 root         (0) root         (0)    11714 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/scripts/pyi_osx_aevent_logger_carbon.py
--rwxrwxrwx   0 root         (0) root         (0)     1058 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/scripts/pyi_path_encoding.py
--rwxrwxrwx   0 root         (0) root         (0)    14974 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/scripts/pyi_pkg_resources_provider.py
--rwxrwxrwx   0 root         (0) root         (0)     1658 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/scripts/pyi_pkgutil_iter_modules.py
--rwxrwxrwx   0 root         (0) root         (0)      933 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/scripts/pyi_python_home.py
--rwxrwxrwx   0 root         (0) root         (0)     1868 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/scripts/pyi_site_module_disabled.py
--rwxrwxrwx   0 root         (0) root         (0)      455 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/scripts/pyi_spec_options.py
--rwxrwxrwx   0 root         (0) root         (0)     1131 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/scripts/pyi_stderr_encoding.py
--rwxrwxrwx   0 root         (0) root         (0)     1130 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/scripts/pyi_stdout_encoding.py
--rwxrwxrwx   0 root         (0) root         (0)     1462 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/scripts/pyi_symlink_basename_is_kept.py
--rwxrwxrwx   0 root         (0) root         (0)     2958 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/scripts/pyi_symlinks_test.py
--rwxrwxrwx   0 root         (0) root         (0)     2283 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/scripts/pyi_threading_module2.py
--rwxrwxrwx   0 root         (0) root         (0)     2232 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/scripts/pyi_unbuffered_output.py
--rwxrwxrwx   0 root         (0) root         (0)     1697 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/scripts/pyi_win_py3_no_shortpathname.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.203521 pyinstaller-6.6.0/tests/functional/specs/
--rwxrwxrwx   0 root         (0) root         (0)     1190 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/specs/list_pytest11_entry_point.spec
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.207582 pyinstaller-6.6.0/tests/functional/specs/multipackage-scripts/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.207894 pyinstaller-6.6.0/tests/functional/specs/multipackage-scripts/extra-hooks/
--rwxrwxrwx   0 root         (0) root         (0)      616 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/specs/multipackage-scripts/extra-hooks/hook-multipackage_test_pkg.py
--rwxrwxrwx   0 root         (0) root         (0)      576 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/specs/multipackage-scripts/multipackage1_B.py
--rwxrwxrwx   0 root         (0) root         (0)      576 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/specs/multipackage-scripts/multipackage2_B.py
--rwxrwxrwx   0 root         (0) root         (0)      576 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/specs/multipackage-scripts/multipackage3_B.py
--rwxrwxrwx   0 root         (0) root         (0)      576 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/specs/multipackage-scripts/multipackage4_B.py
--rwxrwxrwx   0 root         (0) root         (0)      576 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/specs/multipackage-scripts/multipackage5_B.py
--rwxrwxrwx   0 root         (0) root         (0)      576 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/specs/multipackage-scripts/multipackage5_C.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.208582 pyinstaller-6.6.0/tests/functional/specs/multipackage-scripts/multipackage_test_pkg/
--rwxrwxrwx   0 root         (0) root         (0)     1413 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/specs/multipackage-scripts/multipackage_test_pkg/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.209111 pyinstaller-6.6.0/tests/functional/specs/multipackage-scripts/multipackage_test_pkg/data/
--rwxrwxrwx   0 root         (0) root         (0)       11 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/specs/multipackage-scripts/multipackage_test_pkg/data/secret.txt
--rwxrwxrwx   0 root         (0) root         (0)      576 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/specs/multipackage-scripts/test_multipackage1.py
--rwxrwxrwx   0 root         (0) root         (0)      576 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/specs/multipackage-scripts/test_multipackage2.py
--rwxrwxrwx   0 root         (0) root         (0)      576 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/specs/multipackage-scripts/test_multipackage3.py
--rwxrwxrwx   0 root         (0) root         (0)      576 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/specs/multipackage-scripts/test_multipackage4.py
--rwxrwxrwx   0 root         (0) root         (0)      576 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/specs/multipackage-scripts/test_multipackage5.py
--rwxrwxrwx   0 root         (0) root         (0)     2415 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/specs/pyi_osx_aevent_handling_carbon.spec
--rwxrwxrwx   0 root         (0) root         (0)     1613 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/specs/pyi_osx_override_info_plist.spec
--rwxrwxrwx   0 root         (0) root         (0)     1205 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/specs/pyi_spec_options.spec
--rwxrwxrwx   0 root         (0) root         (0)     1170 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/specs/pyi_unbuffered_output.spec
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.210404 pyinstaller-6.6.0/tests/functional/specs/several-scripts/
--rwxrwxrwx   0 root         (0) root         (0)       94 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/specs/several-scripts/basemod.py
--rwxrwxrwx   0 root         (0) root         (0)      366 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/specs/several-scripts/main-script1.py
--rwxrwxrwx   0 root         (0) root         (0)      136 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/specs/several-scripts/main-script2.py
--rwxrwxrwx   0 root         (0) root         (0)      198 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/specs/several-scripts/rt-hook-script.py
--rwxrwxrwx   0 root         (0) root         (0)     1025 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/specs/several-scripts1.spec
--rwxrwxrwx   0 root         (0) root         (0)     1003 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/specs/several-scripts2.spec
--rwxrwxrwx   0 root         (0) root         (0)     1029 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/specs/spec-with-utf8.spec
--rwxrwxrwx   0 root         (0) root         (0)     2022 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/specs/spec_with_splash.spec
--rwxrwxrwx   0 root         (0) root         (0)     1583 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/specs/symlink_basename_is_kept.spec
--rwxrwxrwx   0 root         (0) root         (0)     1699 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/specs/test_multipackage1.spec
--rwxrwxrwx   0 root         (0) root         (0)     1936 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/specs/test_multipackage2.spec
--rwxrwxrwx   0 root         (0) root         (0)     1962 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/specs/test_multipackage3.spec
--rwxrwxrwx   0 root         (0) root         (0)     2170 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/specs/test_multipackage4.spec
--rwxrwxrwx   0 root         (0) root         (0)     2734 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/specs/test_multipackage5.spec
--rwxrwxrwx   0 root         (0) root         (0)    15836 2024-03-24 20:46:04.000000 pyinstaller-6.6.0/tests/functional/test_apple_events.py
--rwxrwxrwx   0 root         (0) root         (0)    31118 2024-02-23 20:40:55.000000 pyinstaller-6.6.0/tests/functional/test_basic.py
--rwxrwxrwx   0 root         (0) root         (0)     4428 2024-04-04 21:05:01.000000 pyinstaller-6.6.0/tests/functional/test_binary_vs_data_reclassification.py
--rwxrwxrwx   0 root         (0) root         (0)     1480 2024-01-13 17:57:57.000000 pyinstaller-6.6.0/tests/functional/test_cliutils.py
--rwxrwxrwx   0 root         (0) root         (0)     1759 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/test_django.py
--rwxrwxrwx   0 root         (0) root         (0)     1439 2023-11-26 23:20:35.000000 pyinstaller-6.6.0/tests/functional/test_hook_utilities.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.214038 pyinstaller-6.6.0/tests/functional/test_hooks/
--rwxrwxrwx   0 root         (0) root         (0)     2423 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/test_hooks/test_gi.py
--rwxrwxrwx   0 root         (0) root         (0)     4748 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/test_hooks/test_matplotlib.py
--rwxrwxrwx   0 root         (0) root         (0)     4032 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/test_hooks/test_pil.py
--rwxrwxrwx   0 root         (0) root         (0)      837 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/test_hooks/test_pkg_resources.py
--rwxrwxrwx   0 root         (0) root         (0)     2107 2023-11-04 13:41:36.000000 pyinstaller-6.6.0/tests/functional/test_hooks/test_scipy.py
--rwxrwxrwx   0 root         (0) root         (0)     1037 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/test_hooks/test_six.py
--rwxrwxrwx   0 root         (0) root         (0)    25798 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/test_import.py
--rwxrwxrwx   0 root         (0) root         (0)     1456 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/test_import_lazy_loader.py
--rwxrwxrwx   0 root         (0) root         (0)     3321 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/test_import_pep302.py
--rwxrwxrwx   0 root         (0) root         (0)     7584 2023-11-11 15:22:30.000000 pyinstaller-6.6.0/tests/functional/test_importlib_resources.py
--rwxrwxrwx   0 root         (0) root         (0)     1979 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/test_interactive.py
--rwxrwxrwx   0 root         (0) root         (0)    13513 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/test_libraries.py
--rwxrwxrwx   0 root         (0) root         (0)     1937 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/test_linux_appimage.py
--rwxrwxrwx   0 root         (0) root         (0)    56164 2023-11-26 23:20:35.000000 pyinstaller-6.6.0/tests/functional/test_macos_bundle_structure.py
--rwxrwxrwx   0 root         (0) root         (0)    18017 2024-04-04 21:05:01.000000 pyinstaller-6.6.0/tests/functional/test_misc.py
--rwxrwxrwx   0 root         (0) root         (0)     2015 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/test_module_exclusion.py
--rwxrwxrwx   0 root         (0) root         (0)      672 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/test_multipackage.py
--rwxrwxrwx   0 root         (0) root         (0)     4481 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/test_multiprocessing.py
--rwxrwxrwx   0 root         (0) root         (0)     5519 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/test_path_encodings.py
--rwxrwxrwx   0 root         (0) root         (0)     2872 2023-11-11 15:22:30.000000 pyinstaller-6.6.0/tests/functional/test_pkg_resources_provider.py
--rwxrwxrwx   0 root         (0) root         (0)     9562 2024-01-13 17:58:01.000000 pyinstaller-6.6.0/tests/functional/test_pkgutil.py
--rwxrwxrwx   0 root         (0) root         (0)     3160 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/test_pywin32.py
--rwxrwxrwx   0 root         (0) root         (0)    25023 2024-02-10 12:19:40.000000 pyinstaller-6.6.0/tests/functional/test_qt.py
--rwxrwxrwx   0 root         (0) root         (0)     5603 2023-11-04 13:41:36.000000 pyinstaller-6.6.0/tests/functional/test_regression.py
--rwxrwxrwx   0 root         (0) root         (0)      918 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/test_runtime.py
--rwxrwxrwx   0 root         (0) root         (0)     3428 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/test_signals.py
--rwxrwxrwx   0 root         (0) root         (0)    21197 2024-04-04 21:05:01.000000 pyinstaller-6.6.0/tests/functional/test_symlinks.py
--rwxrwxrwx   0 root         (0) root         (0)     3000 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/functional/test_unbuffered_stdio.py
--rwxrwxrwx   0 root         (0) root         (0)      709 2024-03-24 20:46:04.000000 pyinstaller-6.6.0/tests/requirements-base.txt
--rwxrwxrwx   0 root         (0) root         (0)      895 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/requirements-developer.txt
--rwxrwxrwx   0 root         (0) root         (0)     3789 2024-04-13 09:44:10.000000 pyinstaller-6.6.0/tests/requirements-libraries.txt
--rwxrwxrwx   0 root         (0) root         (0)      844 2024-01-13 17:58:01.000000 pyinstaller-6.6.0/tests/requirements-tools.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.217224 pyinstaller-6.6.0/tests/scripts/
--rwxrwxrwx   0 root         (0) root         (0)      947 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/scripts/Dockerfile
--rwxrwxrwx   0 root         (0) root         (0)       66 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/scripts/README
--rwxrwxrwx   0 root         (0) root         (0)     2573 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/scripts/check-pefile-arch.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.220134 pyinstaller-6.6.0/tests/scripts/eggs4testing/
--rwxrwxrwx   0 root         (0) root         (0)      119 2023-09-30 18:27:19.000000 pyinstaller-6.6.0/tests/scripts/eggs4testing/.gitignore
--rwxrwxrwx   0 root         (0) root         (0)      240 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/scripts/eggs4testing/README.txt
--rwxrwxrwx   0 root         (0) root         (0)     4204 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/scripts/eggs4testing/build-nspkg-tests.py
--rwxrwxrwx   0 root         (0) root         (0)     3258 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/scripts/eggs4testing/make.sh
--rwxrwxrwx   0 root         (0) root         (0)      829 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/scripts/eggs4testing/setup-unzipped.py
--rwxrwxrwx   0 root         (0) root         (0)      801 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/scripts/eggs4testing/setup-zipped.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.220690 pyinstaller-6.6.0/tests/scripts/eggs4testing/unzipped_egg/
--rwxrwxrwx   0 root         (0) root         (0)      678 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/scripts/eggs4testing/unzipped_egg/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.221176 pyinstaller-6.6.0/tests/scripts/eggs4testing/unzipped_egg/data/
--rwxrwxrwx   0 root         (0) root         (0)       34 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/scripts/eggs4testing/unzipped_egg/data/datafile.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.221516 pyinstaller-6.6.0/tests/scripts/eggs4testing/zipped_egg/
--rwxrwxrwx   0 root         (0) root         (0)      678 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/scripts/eggs4testing/zipped_egg/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.222119 pyinstaller-6.6.0/tests/scripts/eggs4testing/zipped_egg/data/
--rwxrwxrwx   0 root         (0) root         (0)       32 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/scripts/eggs4testing/zipped_egg/data/datafile.txt
--rwxrwxrwx   0 root         (0) root         (0)       77 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/scripts/printShortLongCWD.cmd
--rwxrwxrwx   0 root         (0) root         (0)     1190 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/scripts/test-cliutils.sh
--rwxrwxrwx   0 root         (0) root         (0)     1300 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/scripts/test-docker.sh
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.222437 pyinstaller-6.6.0/tests/speed/
--rwxrwxrwx   0 root         (0) root         (0)     1705 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/speed/speed_pefile.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.235931 pyinstaller-6.6.0/tests/unit/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.238732 pyinstaller-6.6.0/tests/unit/Tree_files/
--rwxrwxrwx   0 root         (0) root         (0)        3 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/Tree_files/dynamiclib.dll
--rwxrwxrwx   0 root         (0) root         (0)        3 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/Tree_files/dynamiclib.dylib
--rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/Tree_files/init__.py
--rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/Tree_files/nine.dat
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.239352 pyinstaller-6.6.0/tests/unit/Tree_files/py_files_not_in_package/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.239658 pyinstaller-6.6.0/tests/unit/Tree_files/py_files_not_in_package/data/
--rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/Tree_files/py_files_not_in_package/data/eleven.dat
--rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/Tree_files/py_files_not_in_package/one.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.240266 pyinstaller-6.6.0/tests/unit/Tree_files/py_files_not_in_package/sub_pkg/
--rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/Tree_files/py_files_not_in_package/sub_pkg/init__.py
--rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/Tree_files/py_files_not_in_package/sub_pkg/three.py
--rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/Tree_files/py_files_not_in_package/ten.dat
--rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/Tree_files/pyextension.pyd
--rwxrwxrwx   0 root         (0) root         (0)        3 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/Tree_files/pyextension.so
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.241180 pyinstaller-6.6.0/tests/unit/Tree_files/subpkg/
--rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/Tree_files/subpkg/init__.py
--rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/Tree_files/subpkg/thirteen.txt
--rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/Tree_files/subpkg/twelve.py
--rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/Tree_files/two.py
--rwxrwxrwx   0 root         (0) root         (0)      791 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/conftest.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.242069 pyinstaller-6.6.0/tests/unit/hook_order_hooks/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/hook_order_hooks/MANIFEST.in
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.242990 pyinstaller-6.6.0/tests/unit/hook_order_hooks/pyi_example_package/
--rwxrwxrwx   0 root         (0) root         (0)       89 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/hook_order_hooks/pyi_example_package/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       46 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/hook_order_hooks/pyi_example_package/hook-pyi_example_package.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.243299 pyinstaller-6.6.0/tests/unit/hook_order_hooks/pyi_example_package/rthooks/
--rwxrwxrwx   0 root         (0) root         (0)       46 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/hook_order_hooks/pyi_example_package/rthooks/pyi_rth_naughty.py
--rwxrwxrwx   0 root         (0) root         (0)       53 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/hook_order_hooks/pyi_example_package/rthooks.dat
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.243617 pyinstaller-6.6.0/tests/unit/hook_order_hooks/rthooks/
--rwxrwxrwx   0 root         (0) root         (0)      507 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/hook_order_hooks/rthooks/pyi_rth_good.py
--rwxrwxrwx   0 root         (0) root         (0)       50 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/hook_order_hooks/rthooks.dat
--rwxrwxrwx   0 root         (0) root         (0)      286 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/hook_order_hooks/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.243928 pyinstaller-6.6.0/tests/unit/hookutils_files/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.246439 pyinstaller-6.6.0/tests/unit/hookutils_files/hookutils_package/
--rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/hookutils_files/hookutils_package/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)        3 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/hookutils_files/hookutils_package/dynamiclib.dll
--rwxrwxrwx   0 root         (0) root         (0)        3 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/hookutils_files/hookutils_package/dynamiclib.dylib
--rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/hookutils_files/hookutils_package/nine.dat
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.247054 pyinstaller-6.6.0/tests/unit/hookutils_files/hookutils_package/py_files_not_in_package/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.247360 pyinstaller-6.6.0/tests/unit/hookutils_files/hookutils_package/py_files_not_in_package/data/
--rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/hookutils_files/hookutils_package/py_files_not_in_package/data/eleven.dat
--rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/hookutils_files/hookutils_package/py_files_not_in_package/one.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.247972 pyinstaller-6.6.0/tests/unit/hookutils_files/hookutils_package/py_files_not_in_package/sub_pkg/
--rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/hookutils_files/hookutils_package/py_files_not_in_package/sub_pkg/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/hookutils_files/hookutils_package/py_files_not_in_package/sub_pkg/three.py
--rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/hookutils_files/hookutils_package/py_files_not_in_package/ten.dat
--rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/hookutils_files/hookutils_package/pyextension.pyd
--rwxrwxrwx   0 root         (0) root         (0)        3 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/hookutils_files/hookutils_package/pyextension.so
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.248585 pyinstaller-6.6.0/tests/unit/hookutils_files/hookutils_package/raises_error_on_import_1/
--rwxrwxrwx   0 root         (0) root         (0)       34 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/hookutils_files/hookutils_package/raises_error_on_import_1/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/hookutils_files/hookutils_package/raises_error_on_import_1/foo.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.249162 pyinstaller-6.6.0/tests/unit/hookutils_files/hookutils_package/raises_error_on_import_2/
--rwxrwxrwx   0 root         (0) root         (0)       34 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/hookutils_files/hookutils_package/raises_error_on_import_2/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/hookutils_files/hookutils_package/raises_error_on_import_2/foo.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.250022 pyinstaller-6.6.0/tests/unit/hookutils_files/hookutils_package/subpkg/
--rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/hookutils_files/hookutils_package/subpkg/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/hookutils_files/hookutils_package/subpkg/thirteen.txt
--rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/hookutils_files/hookutils_package/subpkg/twelve.py
--rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/hookutils_files/hookutils_package/two.py
--rwxrwxrwx   0 root         (0) root         (0)      939 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/hookutils_files/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:10.766030 pyinstaller-6.6.0/tests/unit/hookutils_files2/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.250335 pyinstaller-6.6.0/tests/unit/hookutils_files2/foo/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/hookutils_files2/foo/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.250585 pyinstaller-6.6.0/tests/unit/hookutils_files2/foo/bar/
--rwxrwxrwx   0 root         (0) root         (0)       50 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/hookutils_files2/foo/bar/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     9513 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_TOC.py
--rwxrwxrwx   0 root         (0) root         (0)     2664 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_Tree.py
--rwxrwxrwx   0 root         (0) root         (0)     1115 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_additionalfilescache.py
--rwxrwxrwx   0 root         (0) root         (0)      991 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_bindepend.py
--rwxrwxrwx   0 root         (0) root         (0)     5305 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_building_utils.py
--rwxrwxrwx   0 root         (0) root         (0)     6668 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_bytecode.py
--rwxrwxrwx   0 root         (0) root         (0)     2142 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_compat.py
--rwxrwxrwx   0 root         (0) root         (0)     4211 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_depend_utils.py
--rwxrwxrwx   0 root         (0) root         (0)     1189 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_hook_order.py
--rwxrwxrwx   0 root         (0) root         (0)    15548 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_hookutils.py
--rwxrwxrwx   0 root         (0) root         (0)      772 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_hookutils_gi.py
--rwxrwxrwx   0 root         (0) root         (0)    10804 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_isolation.py
--rwxrwxrwx   0 root         (0) root         (0)     3189 2024-01-13 17:57:57.000000 pyinstaller-6.6.0/tests/unit/test_makespec.py
--rwxrwxrwx   0 root         (0) root         (0)     8414 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_miscutils.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.258842 pyinstaller-6.6.0/tests/unit/test_modulegraph/
--rwxrwxrwx   0 root         (0) root         (0)       26 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1312 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/test_basic.py
--rwxrwxrwx   0 root         (0) root         (0)     2267 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/test_compiled_modules.py
--rwxrwxrwx   0 root         (0) root         (0)    23244 2023-11-26 23:20:35.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/test_edge_data.py
--rwxrwxrwx   0 root         (0) root         (0)     2892 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/test_implies.py
--rwxrwxrwx   0 root         (0) root         (0)     2979 2023-11-26 23:20:35.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/test_import_from_init.py
--rwxrwxrwx   0 root         (0) root         (0)    20640 2023-11-26 23:20:35.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/test_imports.py
--rwxrwxrwx   0 root         (0) root         (0)    30291 2023-11-26 23:20:35.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/test_modulegraph.py
--rwxrwxrwx   0 root         (0) root         (0)     4134 2023-11-26 23:20:35.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/test_pep420_nspkg.py
--rwxrwxrwx   0 root         (0) root         (0)     1325 2023-11-26 23:20:35.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/test_pycompat_pkg.py
--rwxrwxrwx   0 root         (0) root         (0)     1351 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/test_relimport2.py
--rwxrwxrwx   0 root         (0) root         (0)     3675 2023-11-26 23:20:35.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/test_setuptools_nspkg.py
--rwxrwxrwx   0 root         (0) root         (0)     1538 2023-11-26 23:20:35.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/test_swig.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.261915 pyinstaller-6.6.0/tests/unit/test_modulegraph/testdata/
--rwxrwxrwx   0 root         (0) root         (0)       58 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testdata/script
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.262585 pyinstaller-6.6.0/tests/unit/test_modulegraph/testdata/subdir/
--rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testdata/subdir/file1.txt
--rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testdata/subdir/file2.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.264716 pyinstaller-6.6.0/tests/unit/test_modulegraph/testdata/syspath/
--rwxrwxrwx   0 root         (0) root         (0)       23 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testdata/syspath/myext.pyd
--rwxrwxrwx   0 root         (0) root         (0)       23 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testdata/syspath/myext.so
--rwxrwxrwx   0 root         (0) root         (0)       20 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testdata/syspath/mymodule.py
--rwxrwxrwx   0 root         (0) root         (0)       20 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testdata/syspath/mymodule2.pyc
--rwxrwxrwx   0 root         (0) root         (0)       21 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testdata/syspath/mymodule3.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.264969 pyinstaller-6.6.0/tests/unit/test_modulegraph/testdata/syspath/mypkg/
--rwxrwxrwx   0 root         (0) root         (0)       21 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testdata/syspath/mypkg/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     2065 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testdata/syspath.egg
--rwxrwxrwx   0 root         (0) root         (0)     1825 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testdata/syspath.zip
--rwxrwxrwx   0 root         (0) root         (0)      760 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testdata/test.egg
--rwxrwxrwx   0 root         (0) root         (0)       17 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testdata/test.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:10.766494 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-compatmodule/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.266155 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-compatmodule/pkg/
--rwxrwxrwx   0 root         (0) root         (0)       12 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-compatmodule/pkg/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      113 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-compatmodule/pkg/api.py
--rwxrwxrwx   0 root         (0) root         (0)      149 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-compatmodule/pkg/api2.py
--rwxrwxrwx   0 root         (0) root         (0)      171 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-compatmodule/pkg/api3.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:10.766723 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-compiled/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.266479 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-compiled/compiled/
--rwxrwxrwx   0 root         (0) root         (0)       18 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-compiled/compiled/script.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.267690 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-compiled/source/
--rwxrwxrwx   0 root         (0) root         (0)       33 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-compiled/source/mod1.py
--rwxrwxrwx   0 root         (0) root         (0)       66 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-compiled/source/mod2.py
--rwxrwxrwx   0 root         (0) root         (0)       31 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-compiled/source/mod3.py
--rwxrwxrwx   0 root         (0) root         (0)       41 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-compiled/source/mod4.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.273546 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-edgedata/
--rwxrwxrwx   0 root         (0) root         (0)       15 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-edgedata/function_class_existing.py
--rwxrwxrwx   0 root         (0) root         (0)       15 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-edgedata/function_conditional_existing.py
--rwxrwxrwx   0 root         (0) root         (0)       15 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-edgedata/function_conditional_import2_existing.py
--rwxrwxrwx   0 root         (0) root         (0)       15 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-edgedata/function_conditional_import_existing.py
--rwxrwxrwx   0 root         (0) root         (0)       15 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-edgedata/function_existing.py
--rwxrwxrwx   0 root         (0) root         (0)       15 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-edgedata/function_import2_existing.py
--rwxrwxrwx   0 root         (0) root         (0)       15 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-edgedata/function_import_existing.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.278268 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-edgedata/pkg/
--rwxrwxrwx   0 root         (0) root         (0)       21 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-edgedata/pkg/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       15 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-edgedata/pkg/function_class_existing.py
--rwxrwxrwx   0 root         (0) root         (0)       15 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-edgedata/pkg/function_conditional_existing.py
--rwxrwxrwx   0 root         (0) root         (0)       15 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-edgedata/pkg/function_conditional_import2_existing.py
--rwxrwxrwx   0 root         (0) root         (0)       15 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-edgedata/pkg/function_conditional_import_existing.py
--rwxrwxrwx   0 root         (0) root         (0)       15 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-edgedata/pkg/function_existing.py
--rwxrwxrwx   0 root         (0) root         (0)       15 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-edgedata/pkg/function_import2_existing.py
--rwxrwxrwx   0 root         (0) root         (0)       15 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-edgedata/pkg/function_import_existing.py
--rwxrwxrwx   0 root         (0) root         (0)       15 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-edgedata/pkg/toplevel_class_existing.py
--rwxrwxrwx   0 root         (0) root         (0)       15 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-edgedata/pkg/toplevel_conditional_existing.py
--rwxrwxrwx   0 root         (0) root         (0)       15 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-edgedata/pkg/toplevel_conditional_import2_existing.py
--rwxrwxrwx   0 root         (0) root         (0)       15 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-edgedata/pkg/toplevel_conditional_import_existing.py
--rwxrwxrwx   0 root         (0) root         (0)       15 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-edgedata/pkg/toplevel_existing.py
--rwxrwxrwx   0 root         (0) root         (0)       15 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-edgedata/pkg/toplevel_import2_existing.py
--rwxrwxrwx   0 root         (0) root         (0)       15 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-edgedata/pkg/toplevel_import_existing.py
--rwxrwxrwx   0 root         (0) root         (0)     1384 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-edgedata/script.py
--rwxrwxrwx   0 root         (0) root         (0)     1551 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-edgedata/script_from_import.py
--rwxrwxrwx   0 root         (0) root         (0)      265 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-edgedata/script_multi_import.py
--rwxrwxrwx   0 root         (0) root         (0)       15 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-edgedata/toplevel_class_existing.py
--rwxrwxrwx   0 root         (0) root         (0)       15 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-edgedata/toplevel_conditional_existing.py
--rwxrwxrwx   0 root         (0) root         (0)       15 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-edgedata/toplevel_conditional_import2_existing.py
--rwxrwxrwx   0 root         (0) root         (0)       15 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-edgedata/toplevel_conditional_import_existing.py
--rwxrwxrwx   0 root         (0) root         (0)       15 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-edgedata/toplevel_existing.py
--rwxrwxrwx   0 root         (0) root         (0)       15 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-edgedata/toplevel_import2_existing.py
--rwxrwxrwx   0 root         (0) root         (0)       15 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-edgedata/toplevel_import_existing.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.278581 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-import-from-init/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.279166 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-import-from-init/pkg/
--rwxrwxrwx   0 root         (0) root         (0)       12 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-import-from-init/pkg/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.279919 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-import-from-init/pkg/subpkg/
--rwxrwxrwx   0 root         (0) root         (0)       75 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-import-from-init/pkg/subpkg/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       49 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-import-from-init/pkg/subpkg/_collections.py
--rwxrwxrwx   0 root         (0) root         (0)       39 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-import-from-init/pkg/subpkg/compat.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.280169 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-import-from-init/pkg2/
--rwxrwxrwx   0 root         (0) root         (0)       22 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-import-from-init/pkg2/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.280902 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-import-from-init/pkg2/subpkg/
--rwxrwxrwx   0 root         (0) root         (0)       78 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-import-from-init/pkg2/subpkg/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       50 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-import-from-init/pkg2/subpkg/_collections.py
--rwxrwxrwx   0 root         (0) root         (0)       40 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-import-from-init/pkg2/subpkg/compat.py
--rwxrwxrwx   0 root         (0) root         (0)       37 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-import-from-init/script.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.281154 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-packages/
--rwxrwxrwx   0 root         (0) root         (0)       11 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-packages/main_script.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.281654 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-packages/pkg/
--rwxrwxrwx   0 root         (0) root         (0)       17 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-packages/pkg/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.282163 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-packages/pkg/sub1/
--rwxrwxrwx   0 root         (0) root         (0)       22 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-packages/pkg/sub1/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       22 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-packages/pkg/sub1/modA.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.282658 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-packages/pkg/sub2/
--rwxrwxrwx   0 root         (0) root         (0)       22 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-packages/pkg/sub2/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       21 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-packages/pkg/sub2/mod.py
--rwxrwxrwx   0 root         (0) root         (0)       17 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-packages/pkg/sub3.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:10.767624 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-pep420-namespace/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:10.767553 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-pep420-namespace/path1/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.282917 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-pep420-namespace/path1/package/
--rwxrwxrwx   0 root         (0) root         (0)       21 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-pep420-namespace/path1/package/sub2.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:10.767656 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-pep420-namespace/path2/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.283166 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-pep420-namespace/path2/package/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.283411 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-pep420-namespace/path2/package/nspkg/
--rwxrwxrwx   0 root         (0) root         (0)       26 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-pep420-namespace/path2/package/nspkg/mod.py
--rwxrwxrwx   0 root         (0) root         (0)       21 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-pep420-namespace/path2/package/sub1.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.283904 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-pep420-namespace/path2/package/subpackage/
--rwxrwxrwx   0 root         (0) root         (0)       27 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-pep420-namespace/path2/package/subpackage/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       31 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-pep420-namespace/path2/package/subpackage/sub.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.284154 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-regr1/
--rwxrwxrwx   0 root         (0) root         (0)       18 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-regr1/main_script.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.284882 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-regr1/pkg/
--rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-regr1/pkg/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       16 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-regr1/pkg/a.py
--rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-regr1/pkg/b.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.285128 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-regr2/
--rwxrwxrwx   0 root         (0) root         (0)       11 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-regr2/main_script.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.285866 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-regr2/pkg/
--rwxrwxrwx   0 root         (0) root         (0)      153 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-regr2/pkg/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       21 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-regr2/pkg/base.py
--rwxrwxrwx   0 root         (0) root         (0)       15 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-regr2/pkg/pkg.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.286106 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-regr3/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.286346 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-regr3/mypkg/
--rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-regr3/mypkg/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.286826 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-regr3/mypkg/json/
--rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-regr3/mypkg/json/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       68 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-regr3/mypkg/json/encoder.py
--rwxrwxrwx   0 root         (0) root         (0)       31 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-regr3/script.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.287068 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-regr4/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.287315 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-regr4/pkg/
--rwxrwxrwx   0 root         (0) root         (0)       21 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-regr4/pkg/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.288275 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-regr4/pkg/core/
--rwxrwxrwx   0 root         (0) root         (0)       26 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-regr4/pkg/core/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       99 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-regr4/pkg/core/callables.py
--rwxrwxrwx   0 root         (0) root         (0)      160 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-regr4/pkg/core/listener.py
--rwxrwxrwx   0 root         (0) root         (0)       84 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-regr4/pkg/core/listenerimpl.py
--rwxrwxrwx   0 root         (0) root         (0)       49 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-regr4/script.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.288529 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-regr7/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.289033 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-regr7/pkg/
--rwxrwxrwx   0 root         (0) root         (0)       16 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-regr7/pkg/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       65 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-regr7/pkg/mod.py
--rwxrwxrwx   0 root         (0) root         (0)       20 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-regr7/script.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.289513 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-regr8/
--rwxrwxrwx   0 root         (0) root         (0)       30 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-regr8/mod.py
--rwxrwxrwx   0 root         (0) root         (0)       11 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-regr8/script.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.289995 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-relimport/
--rwxrwxrwx   0 root         (0) root         (0)       24 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-relimport/mod.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.291478 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-relimport/pkg/
--rwxrwxrwx   0 root         (0) root         (0)       18 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-relimport/pkg/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       25 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-relimport/pkg/mod.py
--rwxrwxrwx   0 root         (0) root         (0)       11 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-relimport/pkg/oldstyle.py
--rwxrwxrwx   0 root         (0) root         (0)       57 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-relimport/pkg/relative.py
--rwxrwxrwx   0 root         (0) root         (0)       22 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-relimport/pkg/relimport.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.291978 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-relimport/pkg/sub2/
--rwxrwxrwx   0 root         (0) root         (0)       17 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-relimport/pkg/sub2/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       21 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-relimport/pkg/sub2/mod.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.292950 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-relimport/pkg/subpkg/
--rwxrwxrwx   0 root         (0) root         (0)       19 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-relimport/pkg/subpkg/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      117 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-relimport/pkg/subpkg/mod2.py
--rwxrwxrwx   0 root         (0) root         (0)       86 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-relimport/pkg/subpkg/relative.py
--rwxrwxrwx   0 root         (0) root         (0)      106 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-relimport/pkg/subpkg/relative2.py
--rwxrwxrwx   0 root         (0) root         (0)       50 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-relimport/pkg/toplevel.py
--rwxrwxrwx   0 root         (0) root         (0)      175 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-relimport/script.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.293191 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-relimport2/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.294146 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-relimport2/pkg/
--rwxrwxrwx   0 root         (0) root         (0)       39 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-relimport2/pkg/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       13 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-relimport2/pkg/mod1.py
--rwxrwxrwx   0 root         (0) root         (0)       13 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-relimport2/pkg/mod2.py
--rwxrwxrwx   0 root         (0) root         (0)       13 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-relimport2/pkg/mod3.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.294394 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-relimport2/pkg/sub/
--rwxrwxrwx   0 root         (0) root         (0)       65 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-relimport2/pkg/sub/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       17 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-relimport2/toplevel.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.294643 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-setuptools-namespace/
--rwxrwxrwx   0 root         (0) root         (0)      221 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-setuptools-namespace/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:10.769204 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-setuptools-namespace/src/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.295138 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-setuptools-namespace/src/nspkg/
--rwxrwxrwx   0 root         (0) root         (0)      200 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-setuptools-namespace/src/nspkg/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       21 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-setuptools-namespace/src/nspkg/module.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.297487 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-setuptools-namespace/src/nspkg/nssubpkg/
--rwxrwxrwx   0 root         (0) root         (0)      200 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-setuptools-namespace/src/nspkg/nssubpkg/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       26 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-setuptools-namespace/src/nspkg/nssubpkg/sub.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.297000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-setuptools-namespace/src/nspkg.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)      177 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-setuptools-namespace/src/nspkg.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      313 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-setuptools-namespace/src/nspkg.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-setuptools-namespace/src/nspkg.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       21 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-setuptools-namespace/src/nspkg.egg-info/namespace_packages.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-setuptools-namespace/src/nspkg.egg-info/not-zip-safe
--rwxrwxrwx   0 root         (0) root         (0)        6 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-setuptools-namespace/src/nspkg.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:10.769369 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-swig/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 09:53:11.298452 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-swig/pkg/
--rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-swig/pkg/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-swig/pkg/_sample.py
--rwxrwxrwx   0 root         (0) root         (0)       21 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-swig/pkg/sample.i
--rwxrwxrwx   0 root         (0) root         (0)     1974 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-swig/pkg/sample.py
--rwxrwxrwx   0 root         (0) root         (0)    25812 2023-11-26 23:20:35.000000 pyinstaller-6.6.0/tests/unit/test_modulegraph_more.py
--rwxrwxrwx   0 root         (0) root         (0)     3052 2023-11-26 23:20:35.000000 pyinstaller-6.6.0/tests/unit/test_normalize_icon_type.py
--rwxrwxrwx   0 root         (0) root         (0)     8742 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_pyimodulegraph.py
--rwxrwxrwx   0 root         (0) root         (0)     3075 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_recursion_limit.py
--rwxrwxrwx   0 root         (0) root         (0)     1278 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_systemexit.py
--rwxrwxrwx   0 root         (0) root         (0)     7495 2024-04-04 21:05:01.000000 pyinstaller-6.6.0/tests/unit/test_toc_normalization.py
--rwxrwxrwx   0 root         (0) root         (0)    22223 2023-09-30 18:27:26.000000 pyinstaller-6.6.0/tests/unit/test_winmanifest.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.926145 pyinstaller-6.7.0/
+-rwxrwxrwx   0 root         (0) root         (0)      339 2023-09-30 18:27:19.000000 pyinstaller-6.7.0/.dockerignore
+-rwxrwxrwx   0 root         (0) root         (0)      230 2023-09-30 18:27:19.000000 pyinstaller-6.7.0/.editorconfig
+-rwxrwxrwx   0 root         (0) root         (0)      813 2023-09-30 18:27:19.000000 pyinstaller-6.7.0/.gitattributes
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.537386 pyinstaller-6.7.0/.github/
+-rwxrwxrwx   0 root         (0) root         (0)      100 2023-09-30 18:27:19.000000 pyinstaller-6.7.0/.github/CONTRIBUTING.md
+-rwxrwxrwx   0 root         (0) root         (0)       17 2023-09-30 18:27:19.000000 pyinstaller-6.7.0/.github/FUNDING.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.538851 pyinstaller-6.7.0/.github/ISSUE_TEMPLATE/
+-rwxrwxrwx   0 root         (0) root         (0)     8019 2024-02-27 22:30:02.000000 pyinstaller-6.7.0/.github/ISSUE_TEMPLATE/antivirus.md
+-rwxrwxrwx   0 root         (0) root         (0)      286 2023-09-30 18:27:19.000000 pyinstaller-6.7.0/.github/ISSUE_TEMPLATE/blank.md
+-rwxrwxrwx   0 root         (0) root         (0)     2764 2023-09-30 18:27:19.000000 pyinstaller-6.7.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rwxrwxrwx   0 root         (0) root         (0)      404 2023-09-30 18:27:19.000000 pyinstaller-6.7.0/.github/ISSUE_TEMPLATE/config.yml
+-rwxrwxrwx   0 root         (0) root         (0)     1016 2023-09-30 18:27:19.000000 pyinstaller-6.7.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rwxrwxrwx   0 root         (0) root         (0)      193 2023-09-30 18:27:19.000000 pyinstaller-6.7.0/.github/SECURITY.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.541248 pyinstaller-6.7.0/.github/workflows/
+-rwxrwxrwx   0 root         (0) root         (0)      387 2024-03-10 15:20:02.000000 pyinstaller-6.7.0/.github/workflows/cancel.yml
+-rwxrwxrwx   0 root         (0) root         (0)     8040 2024-03-24 20:46:04.000000 pyinstaller-6.7.0/.github/workflows/ci.yml
+-rwxrwxrwx   0 root         (0) root         (0)      997 2024-03-24 20:46:04.000000 pyinstaller-6.7.0/.github/workflows/lint.yml
+-rwxrwxrwx   0 root         (0) root         (0)      429 2024-05-01 21:08:24.000000 pyinstaller-6.7.0/.github/workflows/lock-threads.yml
+-rwxrwxrwx   0 root         (0) root         (0)      463 2024-03-24 20:46:04.000000 pyinstaller-6.7.0/.github/workflows/validate-new-news.yml
+-rwxrwxrwx   0 root         (0) root         (0)     3282 2024-05-01 21:08:24.000000 pyinstaller-6.7.0/.github/workflows/viruscheck.yml
+-rwxrwxrwx   0 root         (0) root         (0)      679 2024-03-24 20:46:04.000000 pyinstaller-6.7.0/.github/workflows/wheel-builder.yml
+-rwxrwxrwx   0 root         (0) root         (0)     2077 2023-09-30 18:27:19.000000 pyinstaller-6.7.0/.gitignore
+-rwxrwxrwx   0 root         (0) root         (0)     1089 2023-09-30 18:27:19.000000 pyinstaller-6.7.0/.pylintrc
+-rwxrwxrwx   0 root         (0) root         (0)      403 2023-09-30 18:27:19.000000 pyinstaller-6.7.0/.pyup.yml
+-rwxrwxrwx   0 root         (0) root         (0)      276 2023-09-30 18:27:19.000000 pyinstaller-6.7.0/.readthedocs.yml
+-rwxrwxrwx   0 root         (0) root         (0)      646 2023-09-30 18:27:19.000000 pyinstaller-6.7.0/.yapfignore
+-rwxrwxrwx   0 root         (0) root         (0)    32138 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/COPYING.txt
+-rwxrwxrwx   0 root         (0) root         (0)      856 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/MANIFEST.in
+-rwxrwxrwx   0 root         (0) root         (0)     8277 2024-05-21 22:38:37.926070 pyinstaller-6.7.0/PKG-INFO
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.543423 pyinstaller-6.7.0/PyInstaller/
+-rwxrwxrwx   0 root         (0) root         (0)     2983 2024-05-21 22:34:43.000000 pyinstaller-6.7.0/PyInstaller/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     8580 2024-02-10 12:19:40.000000 pyinstaller-6.7.0/PyInstaller/__main__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1821 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/_recursion_too_deep_message.py
+-rwxrwxrwx   0 root         (0) root         (0)     3911 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/_shared_with_waf.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.544057 pyinstaller-6.7.0/PyInstaller/archive/
+-rwxrwxrwx   0 root         (0) root         (0)       22 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/archive/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      747 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/archive/pyz_crypto.py
+-rwxrwxrwx   0 root         (0) root         (0)     8489 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/archive/readers.py
+-rwxrwxrwx   0 root         (0) root         (0)    18052 2024-04-04 21:05:01.000000 pyinstaller-6.7.0/PyInstaller/archive/writers.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.521518 pyinstaller-6.7.0/PyInstaller/bootloader/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.546292 pyinstaller-6.7.0/PyInstaller/bootloader/Darwin-64bit/
+-rwxrwxrwx   0 root         (0) root         (0)   189024 2024-04-13 09:51:54.000000 pyinstaller-6.7.0/PyInstaller/bootloader/Darwin-64bit/run
+-rwxrwxrwx   0 root         (0) root         (0)   189000 2024-04-13 09:51:54.000000 pyinstaller-6.7.0/PyInstaller/bootloader/Darwin-64bit/run_d
+-rwxrwxrwx   0 root         (0) root         (0)   191800 2024-04-13 09:51:54.000000 pyinstaller-6.7.0/PyInstaller/bootloader/Darwin-64bit/runw
+-rwxrwxrwx   0 root         (0) root         (0)   224712 2024-04-13 09:51:54.000000 pyinstaller-6.7.0/PyInstaller/bootloader/Darwin-64bit/runw_d
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.549827 pyinstaller-6.7.0/PyInstaller/bootloader/Windows-32bit-intel/
+-rwxrwxrwx   0 root         (0) root         (0)   226304 2024-04-13 09:51:54.000000 pyinstaller-6.7.0/PyInstaller/bootloader/Windows-32bit-intel/run.exe
+-rwxrwxrwx   0 root         (0) root         (0)   230912 2024-04-13 09:51:54.000000 pyinstaller-6.7.0/PyInstaller/bootloader/Windows-32bit-intel/run_d.exe
+-rwxrwxrwx   0 root         (0) root         (0)   226304 2024-04-13 09:51:54.000000 pyinstaller-6.7.0/PyInstaller/bootloader/Windows-32bit-intel/runw.exe
+-rwxrwxrwx   0 root         (0) root         (0)   231424 2024-04-13 09:51:54.000000 pyinstaller-6.7.0/PyInstaller/bootloader/Windows-32bit-intel/runw_d.exe
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.553433 pyinstaller-6.7.0/PyInstaller/bootloader/Windows-64bit-intel/
+-rwxrwxrwx   0 root         (0) root         (0)   270336 2024-04-13 09:51:54.000000 pyinstaller-6.7.0/PyInstaller/bootloader/Windows-64bit-intel/run.exe
+-rwxrwxrwx   0 root         (0) root         (0)   275456 2024-04-13 09:51:54.000000 pyinstaller-6.7.0/PyInstaller/bootloader/Windows-64bit-intel/run_d.exe
+-rwxrwxrwx   0 root         (0) root         (0)   270336 2024-04-13 09:51:54.000000 pyinstaller-6.7.0/PyInstaller/bootloader/Windows-64bit-intel/runw.exe
+-rwxrwxrwx   0 root         (0) root         (0)   275456 2024-04-13 09:51:54.000000 pyinstaller-6.7.0/PyInstaller/bootloader/Windows-64bit-intel/runw_d.exe
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.555704 pyinstaller-6.7.0/PyInstaller/bootloader/images/
+-rwxrwxrwx   0 root         (0) root         (0)   106001 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/bootloader/images/icon-console.icns
+-rwxrwxrwx   0 root         (0) root         (0)    59521 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/bootloader/images/icon-console.ico
+-rwxrwxrwx   0 root         (0) root         (0)   110199 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/bootloader/images/icon-windowed.icns
+-rwxrwxrwx   0 root         (0) root         (0)    60690 2023-10-12 17:16:03.000000 pyinstaller-6.7.0/PyInstaller/bootloader/images/icon-windowed.ico
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.558299 pyinstaller-6.7.0/PyInstaller/building/
+-rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/building/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    65488 2024-04-04 21:05:01.000000 pyinstaller-6.7.0/PyInstaller/building/api.py
+-rwxrwxrwx   0 root         (0) root         (0)    56356 2024-05-01 21:08:24.000000 pyinstaller-6.7.0/PyInstaller/building/build_main.py
+-rwxrwxrwx   0 root         (0) root         (0)    17435 2024-04-04 21:05:01.000000 pyinstaller-6.7.0/PyInstaller/building/datastruct.py
+-rwxrwxrwx   0 root         (0) root         (0)     4015 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/building/icon.py
+-rwxrwxrwx   0 root         (0) root         (0)    35427 2024-05-01 21:08:24.000000 pyinstaller-6.7.0/PyInstaller/building/makespec.py
+-rwxrwxrwx   0 root         (0) root         (0)    41573 2024-04-04 21:05:01.000000 pyinstaller-6.7.0/PyInstaller/building/osx.py
+-rwxrwxrwx   0 root         (0) root         (0)    22800 2023-11-26 23:20:35.000000 pyinstaller-6.7.0/PyInstaller/building/splash.py
+-rwxrwxrwx   0 root         (0) root         (0)     7453 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/building/splash_templates.py
+-rwxrwxrwx   0 root         (0) root         (0)     3146 2024-04-04 21:05:01.000000 pyinstaller-6.7.0/PyInstaller/building/templates.py
+-rwxrwxrwx   0 root         (0) root         (0)    36047 2024-04-04 21:05:01.000000 pyinstaller-6.7.0/PyInstaller/building/utils.py
+-rwxrwxrwx   0 root         (0) root         (0)    30350 2024-05-01 21:08:24.000000 pyinstaller-6.7.0/PyInstaller/compat.py
+-rwxrwxrwx   0 root         (0) root         (0)     1852 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/config.py
+-rwxrwxrwx   0 root         (0) root         (0)     4160 2023-11-26 23:20:35.000000 pyinstaller-6.7.0/PyInstaller/configure.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.560089 pyinstaller-6.7.0/PyInstaller/depend/
+-rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/depend/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    49122 2024-03-09 19:48:33.000000 pyinstaller-6.7.0/PyInstaller/depend/analysis.py
+-rwxrwxrwx   0 root         (0) root         (0)    40310 2024-05-01 21:08:24.000000 pyinstaller-6.7.0/PyInstaller/depend/bindepend.py
+-rwxrwxrwx   0 root         (0) root         (0)    12952 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/depend/bytecode.py
+-rwxrwxrwx   0 root         (0) root         (0)    13110 2024-03-09 19:48:33.000000 pyinstaller-6.7.0/PyInstaller/depend/dylib.py
+-rwxrwxrwx   0 root         (0) root         (0)    25436 2024-05-01 21:08:24.000000 pyinstaller-6.7.0/PyInstaller/depend/imphook.py
+-rwxrwxrwx   0 root         (0) root         (0)    20617 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/depend/imphookapi.py
+-rwxrwxrwx   0 root         (0) root         (0)    16550 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/depend/utils.py
+-rwxrwxrwx   0 root         (0) root         (0)     2987 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/exceptions.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.560315 pyinstaller-6.7.0/PyInstaller/fake-modules/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.560984 pyinstaller-6.7.0/PyInstaller/fake-modules/_pyi_rth_utils/
+-rwxrwxrwx   0 root         (0) root         (0)     1413 2024-02-10 12:19:40.000000 pyinstaller-6.7.0/PyInstaller/fake-modules/_pyi_rth_utils/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    11564 2024-02-10 12:19:40.000000 pyinstaller-6.7.0/PyInstaller/fake-modules/_pyi_rth_utils/_win32.py
+-rwxrwxrwx   0 root         (0) root         (0)     4204 2024-03-09 19:48:33.000000 pyinstaller-6.7.0/PyInstaller/fake-modules/_pyi_rth_utils/qt.py
+-rwxrwxrwx   0 root         (0) root         (0)     2262 2023-11-11 15:22:30.000000 pyinstaller-6.7.0/PyInstaller/fake-modules/_pyi_rth_utils/tempfile.py
+-rwxrwxrwx   0 root         (0) root         (0)     8519 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/fake-modules/pyi_splash.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.620722 pyinstaller-6.7.0/PyInstaller/hooks/
+-rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      845 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PIL.Image.py
+-rwxrwxrwx   0 root         (0) root         (0)      589 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PIL.ImageFilter.py
+-rwxrwxrwx   0 root         (0) root         (0)      773 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PIL.SpiderImagePlugin.py
+-rwxrwxrwx   0 root         (0) root         (0)     1100 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PIL.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.QAxContainer.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.Qsci.py
+-rwxrwxrwx   0 root         (0) root         (0)     1274 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.Qt.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.Qt3DAnimation.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.Qt3DCore.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.Qt3DExtras.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.Qt3DInput.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.Qt3DLogic.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.Qt3DRender.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.QtBluetooth.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.QtChart.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.QtCore.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.QtDBus.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.QtDataVisualization.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.QtDesigner.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.QtGui.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.QtHelp.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.QtLocation.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.QtMacExtras.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.QtMultimedia.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.QtMultimediaWidgets.py
+-rwxrwxrwx   0 root         (0) root         (0)      710 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.QtNetwork.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.QtNetworkAuth.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.QtNfc.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.QtOpenGL.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.QtPositioning.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.QtPrintSupport.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.QtPurchasing.py
+-rwxrwxrwx   0 root         (0) root         (0)      764 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.QtQml.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.QtQuick.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.QtQuick3D.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.QtQuickWidgets.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.QtRemoteObjects.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.QtScript.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.QtSensors.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.QtSerialPort.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.QtSql.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.QtSvg.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.QtTest.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.QtTextToSpeech.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.QtWebChannel.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.QtWebEngine.py
+-rwxrwxrwx   0 root         (0) root         (0)      995 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.QtWebEngineCore.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.QtWebEngineWidgets.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.QtWebKit.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.QtWebKitWidgets.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.QtWebSockets.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.QtWidgets.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.QtWinExtras.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.QtX11Extras.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.QtXml.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.QtXmlPatterns.py
+-rwxrwxrwx   0 root         (0) root         (0)     1182 2024-03-09 19:48:33.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.py
+-rwxrwxrwx   0 root         (0) root         (0)      979 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.uic.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.QAxContainer.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.Qsci.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.Qt3DAnimation.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.Qt3DCore.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.Qt3DExtras.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.Qt3DInput.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.Qt3DLogic.py
+-rwxrwxrwx   0 root         (0) root         (0)      670 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.Qt3DRender.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.QtBluetooth.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.QtCharts.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.QtCore.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.QtDBus.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.QtDataVisualization.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.QtDesigner.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.QtGui.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.QtHelp.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.QtMultimedia.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.QtMultimediaWidgets.py
+-rwxrwxrwx   0 root         (0) root         (0)      710 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.QtNetwork.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.QtNetworkAuth.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.QtNfc.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.QtOpenGL.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.QtOpenGLWidgets.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.QtPdf.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.QtPdfWidgets.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.QtPositioning.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.QtPrintSupport.py
+-rwxrwxrwx   0 root         (0) root         (0)      764 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.QtQml.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.QtQuick.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.QtQuick3D.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.QtQuickWidgets.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.QtRemoteObjects.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.QtSensors.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.QtSerialPort.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.QtSpatialAudio.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.QtSql.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.QtSvg.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.QtSvgWidgets.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.QtTest.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.QtTextToSpeech.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.QtWebChannel.py
+-rwxrwxrwx   0 root         (0) root         (0)     1351 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.QtWebEngineCore.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.QtWebEngineQuick.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.QtWebEngineWidgets.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.QtWebSockets.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.QtWidgets.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.QtXml.py
+-rwxrwxrwx   0 root         (0) root         (0)     1025 2024-03-09 19:48:33.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.py
+-rwxrwxrwx   0 root         (0) root         (0)      979 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.uic.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.Qt3DAnimation.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.Qt3DCore.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.Qt3DExtras.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.Qt3DInput.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.Qt3DLogic.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.Qt3DRender.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.QtAxContainer.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.QtCharts.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.QtConcurrent.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.QtCore.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.QtDataVisualization.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.QtGui.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.QtHelp.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.QtLocation.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.QtMacExtras.py
+-rwxrwxrwx   0 root         (0) root         (0)      979 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.QtMultimedia.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.QtMultimediaWidgets.py
+-rwxrwxrwx   0 root         (0) root         (0)      714 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.QtNetwork.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.QtOpenGL.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.QtOpenGLFunctions.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.QtPositioning.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.QtPrintSupport.py
+-rwxrwxrwx   0 root         (0) root         (0)      804 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.QtQml.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.QtQuick.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.QtQuickControls2.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.QtQuickWidgets.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.QtRemoteObjects.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.QtScript.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.QtScriptTools.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.QtScxml.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.QtSensors.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.QtSerialPort.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.QtSql.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.QtSvg.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.QtTest.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.QtTextToSpeech.py
+-rwxrwxrwx   0 root         (0) root         (0)      710 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.QtUiTools.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.QtWebChannel.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.QtWebEngine.py
+-rwxrwxrwx   0 root         (0) root         (0)     1003 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.QtWebEngineCore.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.QtWebEngineWidgets.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.QtWebKit.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.QtWebKitWidgets.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.QtWebSockets.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.QtWidgets.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.QtWinExtras.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.QtX11Extras.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.QtXml.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.QtXmlPatterns.py
+-rwxrwxrwx   0 root         (0) root         (0)      972 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.Qwt5.py
+-rwxrwxrwx   0 root         (0) root         (0)     1141 2024-03-09 19:48:33.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.Qt3DAnimation.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.Qt3DCore.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.Qt3DExtras.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.Qt3DInput.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.Qt3DLogic.py
+-rwxrwxrwx   0 root         (0) root         (0)     1122 2024-04-13 09:44:10.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.Qt3DRender.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtAxContainer.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtBluetooth.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtCharts.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtConcurrent.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtCore.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtDBus.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtDataVisualization.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtDesigner.py
+-rwxrwxrwx   0 root         (0) root         (0)      628 2023-11-04 13:41:36.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtGraphs.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtGui.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtHelp.py
+-rwxrwxrwx   0 root         (0) root         (0)      837 2023-10-12 17:16:14.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtHttpServer.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtLocation.py
+-rwxrwxrwx   0 root         (0) root         (0)      981 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtMultimedia.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtMultimediaWidgets.py
+-rwxrwxrwx   0 root         (0) root         (0)      714 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtNetwork.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtNetworkAuth.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtNfc.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtOpenGL.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtOpenGLWidgets.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtPdf.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtPdfWidgets.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtPositioning.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtPrintSupport.py
+-rwxrwxrwx   0 root         (0) root         (0)      768 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtQml.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtQuick.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtQuick3D.py
+-rwxrwxrwx   0 root         (0) root         (0)      671 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtQuickControls2.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtQuickWidgets.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtRemoteObjects.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtScxml.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtSensors.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtSerialBus.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtSerialPort.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtSpatialAudio.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtSql.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtStateMachine.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtSvg.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtSvgWidgets.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtTest.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtTextToSpeech.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtUiTools.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtWebChannel.py
+-rwxrwxrwx   0 root         (0) root         (0)     1410 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtWebEngineCore.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtWebEngineQuick.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtWebEngineWidgets.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtWebSockets.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtWidgets.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtXml.py
+-rwxrwxrwx   0 root         (0) root         (0)     1279 2024-03-09 19:48:33.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.py
+-rwxrwxrwx   0 root         (0) root         (0)      680 2023-11-11 15:22:30.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-_pyi_rth_utils.py
+-rwxrwxrwx   0 root         (0) root         (0)     1327 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-_tkinter.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-babel.py
+-rwxrwxrwx   0 root         (0) root         (0)      577 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-difflib.py
+-rwxrwxrwx   0 root         (0) root         (0)      606 2023-11-04 13:41:36.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-distutils.command.check.py
+-rwxrwxrwx   0 root         (0) root         (0)     1859 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-distutils.py
+-rwxrwxrwx   0 root         (0) root         (0)      661 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-distutils.util.py
+-rwxrwxrwx   0 root         (0) root         (0)      635 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-django.contrib.sessions.py
+-rwxrwxrwx   0 root         (0) root         (0)      629 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-django.core.cache.py
+-rwxrwxrwx   0 root         (0) root         (0)     1069 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-django.core.mail.py
+-rwxrwxrwx   0 root         (0) root         (0)      942 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-django.core.management.py
+-rwxrwxrwx   0 root         (0) root         (0)      611 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-django.db.backends.mysql.base.py
+-rwxrwxrwx   0 root         (0) root         (0)      563 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-django.db.backends.oracle.base.py
+-rwxrwxrwx   0 root         (0) root         (0)      983 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-django.db.backends.py
+-rwxrwxrwx   0 root         (0) root         (0)     3922 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-django.py
+-rwxrwxrwx   0 root         (0) root         (0)      626 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-django.template.loaders.py
+-rwxrwxrwx   0 root         (0) root         (0)      612 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-encodings.py
+-rwxrwxrwx   0 root         (0) root         (0)     1011 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-gevent.py
+-rwxrwxrwx   0 root         (0) root         (0)      552 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.py
+-rwxrwxrwx   0 root         (0) root         (0)      698 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.Adw.py
+-rwxrwxrwx   0 root         (0) root         (0)      710 2024-01-13 17:57:57.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.AppIndicator3.py
+-rwxrwxrwx   0 root         (0) root         (0)     1084 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.Atk.py
+-rwxrwxrwx   0 root         (0) root         (0)      717 2024-01-13 17:57:57.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.AyatanaAppIndicator3.py
+-rwxrwxrwx   0 root         (0) root         (0)      707 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.Champlain.py
+-rwxrwxrwx   0 root         (0) root         (0)      704 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.Clutter.py
+-rwxrwxrwx   0 root         (0) root         (0)      701 2024-01-13 17:57:57.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.DBus.py
+-rwxrwxrwx   0 root         (0) root         (0)      709 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.GIRepository.py
+-rwxrwxrwx   0 root         (0) root         (0)     1490 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.GLib.py
+-rwxrwxrwx   0 root         (0) root         (0)      704 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.GModule.py
+-rwxrwxrwx   0 root         (0) root         (0)      905 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.GObject.py
+-rwxrwxrwx   0 root         (0) root         (0)     1393 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.Gdk.py
+-rwxrwxrwx   0 root         (0) root         (0)     6318 2023-11-26 23:20:35.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.GdkPixbuf.py
+-rwxrwxrwx   0 root         (0) root         (0)     2605 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.Gio.py
+-rwxrwxrwx   0 root         (0) root         (0)      705 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.Graphene.py
+-rwxrwxrwx   0 root         (0) root         (0)      700 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.Gsk.py
+-rwxrwxrwx   0 root         (0) root         (0)     3461 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.Gst.py
+-rwxrwxrwx   0 root         (0) root         (0)      710 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.GstAllocators.py
+-rwxrwxrwx   0 root         (0) root         (0)      703 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.GstApp.py
+-rwxrwxrwx   0 root         (0) root         (0)      705 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.GstAudio.py
+-rwxrwxrwx   0 root         (0) root         (0)      708 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.GstBadAudio.py
+-rwxrwxrwx   0 root         (0) root         (0)      704 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.GstBase.py
+-rwxrwxrwx   0 root         (0) root         (0)      705 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.GstCheck.py
+-rwxrwxrwx   0 root         (0) root         (0)      706 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.GstCodecs.py
+-rwxrwxrwx   0 root         (0) root         (0)      710 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.GstController.py
+-rwxrwxrwx   0 root         (0) root         (0)      702 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.GstGL.py
+-rwxrwxrwx   0 root         (0) root         (0)      705 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.GstGLEGL.py
+-rwxrwxrwx   0 root         (0) root         (0)      709 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.GstGLWayland.py
+-rwxrwxrwx   0 root         (0) root         (0)      705 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.GstGLX11.py
+-rwxrwxrwx   0 root         (0) root         (0)      709 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.GstInsertBin.py
+-rwxrwxrwx   0 root         (0) root         (0)      706 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.GstMpegts.py
+-rwxrwxrwx   0 root         (0) root         (0)      703 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.GstNet.py
+-rwxrwxrwx   0 root         (0) root         (0)      707 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.GstPbutils.py
+-rwxrwxrwx   0 root         (0) root         (0)      704 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.GstPlay.py
+-rwxrwxrwx   0 root         (0) root         (0)      706 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.GstPlayer.py
+-rwxrwxrwx   0 root         (0) root         (0)      703 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.GstRtp.py
+-rwxrwxrwx   0 root         (0) root         (0)      704 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.GstRtsp.py
+-rwxrwxrwx   0 root         (0) root         (0)      710 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.GstRtspServer.py
+-rwxrwxrwx   0 root         (0) root         (0)      703 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.GstSdp.py
+-rwxrwxrwx   0 root         (0) root         (0)      703 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.GstTag.py
+-rwxrwxrwx   0 root         (0) root         (0)      710 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.GstTranscoder.py
+-rwxrwxrwx   0 root         (0) root         (0)      705 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.GstVideo.py
+-rwxrwxrwx   0 root         (0) root         (0)      706 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.GstVulkan.py
+-rwxrwxrwx   0 root         (0) root         (0)      713 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.GstVulkanWayland.py
+-rwxrwxrwx   0 root         (0) root         (0)      709 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.GstVulkanXCB.py
+-rwxrwxrwx   0 root         (0) root         (0)      706 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.GstWebRTC.py
+-rwxrwxrwx   0 root         (0) root         (0)     2150 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.Gtk.py
+-rwxrwxrwx   0 root         (0) root         (0)      710 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.GtkChamplain.py
+-rwxrwxrwx   0 root         (0) root         (0)      707 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.GtkClutter.py
+-rwxrwxrwx   0 root         (0) root         (0)     1297 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.GtkSource.py
+-rwxrwxrwx   0 root         (0) root         (0)      781 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.GtkosxApplication.py
+-rwxrwxrwx   0 root         (0) root         (0)      705 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.HarfBuzz.py
+-rwxrwxrwx   0 root         (0) root         (0)      702 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.Pango.py
+-rwxrwxrwx   0 root         (0) root         (0)      707 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.PangoCairo.py
+-rwxrwxrwx   0 root         (0) root         (0)      702 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.cairo.py
+-rwxrwxrwx   0 root         (0) root         (0)      706 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.freetype2.py
+-rwxrwxrwx   0 root         (0) root         (0)      701 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.xlib.py
+-rwxrwxrwx   0 root         (0) root         (0)      578 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-heapq.py
+-rwxrwxrwx   0 root         (0) root         (0)      602 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-idlelib.py
+-rwxrwxrwx   0 root         (0) root         (0)     1350 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-importlib_metadata.py
+-rwxrwxrwx   0 root         (0) root         (0)     1015 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-importlib_resources.py
+-rwxrwxrwx   0 root         (0) root         (0)      888 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-keyring.py
+-rwxrwxrwx   0 root         (0) root         (0)     1126 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-kivy.py
+-rwxrwxrwx   0 root         (0) root         (0)      653 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-lib2to3.py
+-rwxrwxrwx   0 root         (0) root         (0)      894 2024-03-09 19:48:33.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-matplotlib.backends.backend_qtagg.py
+-rwxrwxrwx   0 root         (0) root         (0)      896 2024-03-09 19:48:33.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-matplotlib.backends.backend_qtcairo.py
+-rwxrwxrwx   0 root         (0) root         (0)     9657 2024-03-09 19:48:33.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-matplotlib.backends.py
+-rwxrwxrwx   0 root         (0) root         (0)     1284 2024-03-09 19:48:33.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-matplotlib.backends.qt_compat.py
+-rwxrwxrwx   0 root         (0) root         (0)      683 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-matplotlib.numerix.py
+-rwxrwxrwx   0 root         (0) root         (0)     1568 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-matplotlib.py
+-rwxrwxrwx   0 root         (0) root         (0)      791 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-multiprocessing.util.py
+-rwxrwxrwx   0 root         (0) root         (0)     2331 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-numpy.py
+-rwxrwxrwx   0 root         (0) root         (0)      577 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-packaging.py
+-rwxrwxrwx   0 root         (0) root         (0)     1156 2024-03-09 19:48:33.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-pandas.io.clipboard.py
+-rwxrwxrwx   0 root         (0) root         (0)      751 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-pandas.io.formats.style.py
+-rwxrwxrwx   0 root         (0) root         (0)      938 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-pandas.plotting.py
+-rwxrwxrwx   0 root         (0) root         (0)      955 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-pandas.py
+-rwxrwxrwx   0 root         (0) root         (0)      589 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-pickle.py
+-rwxrwxrwx   0 root         (0) root         (0)     3141 2024-05-21 22:30:39.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-pkg_resources.py
+-rwxrwxrwx   0 root         (0) root         (0)      713 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-platform.py
+-rwxrwxrwx   0 root         (0) root         (0)     1184 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-pygments.py
+-rwxrwxrwx   0 root         (0) root         (0)      734 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-pytz.py
+-rwxrwxrwx   0 root         (0) root         (0)      603 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-pytzdata.py
+-rwxrwxrwx   0 root         (0) root         (0)      792 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-qtawesome.py
+-rwxrwxrwx   0 root         (0) root         (0)     1179 2024-03-09 19:48:33.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-qtpy.py
+-rwxrwxrwx   0 root         (0) root         (0)      930 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-scapy.layers.all.py
+-rwxrwxrwx   0 root         (0) root         (0)      655 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-scipy.io.matlab.py
+-rwxrwxrwx   0 root         (0) root         (0)      633 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-scipy.linalg.py
+-rwxrwxrwx   0 root         (0) root         (0)     1604 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-scipy.py
+-rwxrwxrwx   0 root         (0) root         (0)      611 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-scipy.sparse.csgraph.py
+-rwxrwxrwx   0 root         (0) root         (0)      793 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-scipy.spatial.transform.rotation.py
+-rwxrwxrwx   0 root         (0) root         (0)     1317 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-scipy.special._ellip_harm_2.py
+-rwxrwxrwx   0 root         (0) root         (0)     1042 2024-04-13 09:44:10.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-scipy.special._ufuncs.py
+-rwxrwxrwx   0 root         (0) root         (0)      656 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-scipy.stats._stats.py
+-rwxrwxrwx   0 root         (0) root         (0)      819 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-scrapy.py
+-rwxrwxrwx   0 root         (0) root         (0)      606 2023-11-04 13:41:36.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-setuptools._distutils.command.check.py
+-rwxrwxrwx   0 root         (0) root         (0)      599 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-setuptools.msvc.py
+-rwxrwxrwx   0 root         (0) root         (0)     2149 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-setuptools.py
+-rwxrwxrwx   0 root         (0) root         (0)      603 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-shelve.py
+-rwxrwxrwx   0 root         (0) root         (0)      766 2023-11-04 13:41:36.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-shiboken6.py
+-rwxrwxrwx   0 root         (0) root         (0)     1998 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-sphinx.py
+-rwxrwxrwx   0 root         (0) root         (0)     3496 2024-05-21 22:30:39.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-sqlalchemy.py
+-rwxrwxrwx   0 root         (0) root         (0)      813 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-sqlite3.py
+-rwxrwxrwx   0 root         (0) root         (0)     1558 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-sysconfig.py
+-rwxrwxrwx   0 root         (0) root         (0)      602 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-wcwidth.py
+-rwxrwxrwx   0 root         (0) root         (0)     1204 2024-05-21 22:30:39.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-win32ctypes.core.py
+-rwxrwxrwx   0 root         (0) root         (0)      569 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-xml.dom.domreg.py
+-rwxrwxrwx   0 root         (0) root         (0)      615 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-xml.etree.cElementTree.py
+-rwxrwxrwx   0 root         (0) root         (0)      569 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-xml.py
+-rwxrwxrwx   0 root         (0) root         (0)      539 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/hook-zope.interface.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.621630 pyinstaller-6.7.0/PyInstaller/hooks/pre_find_module_path/
+-rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/pre_find_module_path/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      696 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/pre_find_module_path/hook-PyQt5.uic.port_v2.py
+-rwxrwxrwx   0 root         (0) root         (0)      905 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/pre_find_module_path/hook-_pyi_rth_utils.py
+-rwxrwxrwx   0 root         (0) root         (0)     2347 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/pre_find_module_path/hook-distutils.py
+-rwxrwxrwx   0 root         (0) root         (0)     1412 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/pre_find_module_path/hook-pyi_splash.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.633312 pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/
+-rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1772 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-distutils.py
+-rwxrwxrwx   0 root         (0) root         (0)     1955 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.py
+-rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.Adw.py
+-rwxrwxrwx   0 root         (0) root         (0)      783 2024-01-13 17:57:57.000000 pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.AppIndicator3.py
+-rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.Atk.py
+-rwxrwxrwx   0 root         (0) root         (0)      783 2024-01-13 17:57:57.000000 pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.AyatanaAppIndicator3.py
+-rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.Champlain.py
+-rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.Clutter.py
+-rwxrwxrwx   0 root         (0) root         (0)      783 2024-01-13 17:57:57.000000 pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.DBus.py
+-rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GIRepository.py
+-rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GLib.py
+-rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GModule.py
+-rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GObject.py
+-rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.Gdk.py
+-rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GdkPixbuf.py
+-rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.Gio.py
+-rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.Graphene.py
+-rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.Gsk.py
+-rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.Gst.py
+-rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstAllocators.py
+-rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstApp.py
+-rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstAudio.py
+-rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstBadAudio.py
+-rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstBase.py
+-rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstCheck.py
+-rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstCodecs.py
+-rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstController.py
+-rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstGL.py
+-rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstGLEGL.py
+-rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstGLWayland.py
+-rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstGLX11.py
+-rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstInsertBin.py
+-rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstMpegts.py
+-rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstNet.py
+-rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstPbutils.py
+-rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstPlay.py
+-rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstPlayer.py
+-rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstRtp.py
+-rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstRtsp.py
+-rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstRtspServer.py
+-rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstSdp.py
+-rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstTag.py
+-rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstTranscoder.py
+-rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstVideo.py
+-rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstVulkan.py
+-rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstVulkanWayland.py
+-rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstVulkanXCB.py
+-rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstWebRTC.py
+-rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.Gtk.py
+-rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GtkChamplain.py
+-rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GtkClutter.py
+-rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GtkSource.py
+-rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GtkosxApplication.py
+-rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.HarfBuzz.py
+-rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.Pango.py
+-rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.PangoCairo.py
+-rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.cairo.py
+-rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.freetype2.py
+-rwxrwxrwx   0 root         (0) root         (0)      783 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.xlib.py
+-rwxrwxrwx   0 root         (0) root         (0)     1629 2024-01-13 17:57:57.000000 pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-setuptools.extern.six.moves.py
+-rwxrwxrwx   0 root         (0) root         (0)     3744 2024-01-13 17:57:57.000000 pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-six.moves.py
+-rwxrwxrwx   0 root         (0) root         (0)     1380 2024-01-13 17:57:57.000000 pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-urllib3.packages.six.moves.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.636987 pyinstaller-6.7.0/PyInstaller/hooks/rthooks/
+-rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/rthooks/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1248 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/rthooks/pyi_rth__tkinter.py
+-rwxrwxrwx   0 root         (0) root         (0)     1111 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/rthooks/pyi_rth_django.py
+-rwxrwxrwx   0 root         (0) root         (0)     1437 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/rthooks/pyi_rth_gdkpixbuf.py
+-rwxrwxrwx   0 root         (0) root         (0)      632 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/rthooks/pyi_rth_gi.py
+-rwxrwxrwx   0 root         (0) root         (0)      631 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/rthooks/pyi_rth_gio.py
+-rwxrwxrwx   0 root         (0) root         (0)     1444 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/rthooks/pyi_rth_glib.py
+-rwxrwxrwx   0 root         (0) root         (0)     1175 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/rthooks/pyi_rth_gstreamer.py
+-rwxrwxrwx   0 root         (0) root         (0)      886 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/rthooks/pyi_rth_gtk.py
+-rwxrwxrwx   0 root         (0) root         (0)     2094 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/rthooks/pyi_rth_inspect.py
+-rwxrwxrwx   0 root         (0) root         (0)      737 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/rthooks/pyi_rth_kivy.py
+-rwxrwxrwx   0 root         (0) root         (0)     1808 2023-11-11 15:22:30.000000 pyinstaller-6.7.0/PyInstaller/hooks/rthooks/pyi_rth_mplconfig.py
+-rwxrwxrwx   0 root         (0) root         (0)     4814 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/rthooks/pyi_rth_multiprocessing.py
+-rwxrwxrwx   0 root         (0) root         (0)     7889 2023-11-11 15:22:30.000000 pyinstaller-6.7.0/PyInstaller/hooks/rthooks/pyi_rth_pkgres.py
+-rwxrwxrwx   0 root         (0) root         (0)     6072 2024-01-13 17:58:01.000000 pyinstaller-6.7.0/PyInstaller/hooks/rthooks/pyi_rth_pkgutil.py
+-rwxrwxrwx   0 root         (0) root         (0)     3542 2024-03-09 19:48:33.000000 pyinstaller-6.7.0/PyInstaller/hooks/rthooks/pyi_rth_pyqt5.py
+-rwxrwxrwx   0 root         (0) root         (0)     3803 2024-03-09 19:48:33.000000 pyinstaller-6.7.0/PyInstaller/hooks/rthooks/pyi_rth_pyqt6.py
+-rwxrwxrwx   0 root         (0) root         (0)     3235 2024-03-09 19:48:33.000000 pyinstaller-6.7.0/PyInstaller/hooks/rthooks/pyi_rth_pyside2.py
+-rwxrwxrwx   0 root         (0) root         (0)     3730 2024-03-09 19:48:33.000000 pyinstaller-6.7.0/PyInstaller/hooks/rthooks/pyi_rth_pyside6.py
+-rwxrwxrwx   0 root         (0) root         (0)     1430 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/hooks/rthooks/pyi_rth_setuptools.py
+-rwxrwxrwx   0 root         (0) root         (0)      956 2024-02-23 20:40:55.000000 pyinstaller-6.7.0/PyInstaller/hooks/rthooks.dat
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.637524 pyinstaller-6.7.0/PyInstaller/isolated/
+-rwxrwxrwx   0 root         (0) root         (0)     1524 2024-03-09 19:48:33.000000 pyinstaller-6.7.0/PyInstaller/isolated/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     3757 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/isolated/_child.py
+-rwxrwxrwx   0 root         (0) root         (0)    17407 2023-10-12 17:16:03.000000 pyinstaller-6.7.0/PyInstaller/isolated/_parent.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.637959 pyinstaller-6.7.0/PyInstaller/lib/
+-rwxrwxrwx   0 root         (0) root         (0)     1333 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/lib/README.rst
+-rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/lib/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.639248 pyinstaller-6.7.0/PyInstaller/lib/modulegraph/
+-rwxrwxrwx   0 root         (0) root         (0)       21 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/lib/modulegraph/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     2653 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/lib/modulegraph/__main__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1754 2023-11-26 23:20:35.000000 pyinstaller-6.7.0/PyInstaller/lib/modulegraph/find_modules.py
+-rwxrwxrwx   0 root         (0) root         (0)   129871 2023-11-26 23:20:35.000000 pyinstaller-6.7.0/PyInstaller/lib/modulegraph/modulegraph.py
+-rwxrwxrwx   0 root         (0) root         (0)      849 2023-11-26 23:20:35.000000 pyinstaller-6.7.0/PyInstaller/lib/modulegraph/util.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.640398 pyinstaller-6.7.0/PyInstaller/loader/
+-rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/loader/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     3712 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/loader/pyiboot01_bootstrap.py
+-rwxrwxrwx   0 root         (0) root         (0)     6059 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/loader/pyimod01_archive.py
+-rwxrwxrwx   0 root         (0) root         (0)    28111 2023-11-11 15:22:30.000000 pyinstaller-6.7.0/PyInstaller/loader/pyimod02_importers.py
+-rwxrwxrwx   0 root         (0) root         (0)     4915 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/loader/pyimod03_ctypes.py
+-rwxrwxrwx   0 root         (0) root         (0)     2936 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/loader/pyimod04_pywin32.py
+-rwxrwxrwx   0 root         (0) root         (0)     2058 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/log.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.642186 pyinstaller-6.7.0/PyInstaller/utils/
+-rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/utils/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      451 2023-10-12 17:16:03.000000 pyinstaller-6.7.0/PyInstaller/utils/_gitrevision.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.643282 pyinstaller-6.7.0/PyInstaller/utils/cliutils/
+-rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/utils/cliutils/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     9259 2023-11-04 13:41:36.000000 pyinstaller-6.7.0/PyInstaller/utils/cliutils/archive_viewer.py
+-rwxrwxrwx   0 root         (0) root         (0)     1844 2023-11-04 13:41:36.000000 pyinstaller-6.7.0/PyInstaller/utils/cliutils/bindepend.py
+-rwxrwxrwx   0 root         (0) root         (0)     1857 2023-11-04 13:41:36.000000 pyinstaller-6.7.0/PyInstaller/utils/cliutils/grab_version.py
+-rwxrwxrwx   0 root         (0) root         (0)     1640 2023-11-04 13:41:36.000000 pyinstaller-6.7.0/PyInstaller/utils/cliutils/makespec.py
+-rwxrwxrwx   0 root         (0) root         (0)     1503 2023-11-04 13:41:36.000000 pyinstaller-6.7.0/PyInstaller/utils/cliutils/set_version.py
+-rwxrwxrwx   0 root         (0) root         (0)    24057 2024-05-21 22:30:39.000000 pyinstaller-6.7.0/PyInstaller/utils/conftest.py
+-rwxrwxrwx   0 root         (0) root         (0)     2014 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/utils/git.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.644430 pyinstaller-6.7.0/PyInstaller/utils/hooks/
+-rwxrwxrwx   0 root         (0) root         (0)    50777 2023-11-26 23:20:35.000000 pyinstaller-6.7.0/PyInstaller/utils/hooks/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    14694 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/utils/hooks/conda.py
+-rwxrwxrwx   0 root         (0) root         (0)     6100 2024-01-13 17:58:01.000000 pyinstaller-6.7.0/PyInstaller/utils/hooks/django.py
+-rwxrwxrwx   0 root         (0) root         (0)    17414 2023-11-26 23:20:35.000000 pyinstaller-6.7.0/PyInstaller/utils/hooks/gi.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.645027 pyinstaller-6.7.0/PyInstaller/utils/hooks/qt/
+-rwxrwxrwx   0 root         (0) root         (0)    74721 2024-03-09 19:48:33.000000 pyinstaller-6.7.0/PyInstaller/utils/hooks/qt/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    25226 2023-11-04 13:41:36.000000 pyinstaller-6.7.0/PyInstaller/utils/hooks/qt/_modules_info.py
+-rwxrwxrwx   0 root         (0) root         (0)    10707 2023-11-26 23:20:35.000000 pyinstaller-6.7.0/PyInstaller/utils/hooks/tcl_tk.py
+-rwxrwxrwx   0 root         (0) root         (0)     7030 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/utils/misc.py
+-rwxrwxrwx   0 root         (0) root         (0)    29386 2024-01-13 17:58:01.000000 pyinstaller-6.7.0/PyInstaller/utils/osx.py
+-rwxrwxrwx   0 root         (0) root         (0)       87 2023-10-12 17:16:03.000000 pyinstaller-6.7.0/PyInstaller/utils/pytest.ini
+-rwxrwxrwx   0 root         (0) root         (0)     2875 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/utils/run_tests.py
+-rwxrwxrwx   0 root         (0) root         (0)     5711 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/utils/tests.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.646279 pyinstaller-6.7.0/PyInstaller/utils/win32/
+-rwxrwxrwx   0 root         (0) root         (0)       22 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/utils/win32/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     9327 2024-02-23 20:40:55.000000 pyinstaller-6.7.0/PyInstaller/utils/win32/icon.py
+-rwxrwxrwx   0 root         (0) root         (0)    20594 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/utils/win32/versioninfo.py
+-rwxrwxrwx   0 root         (0) root         (0)    10639 2023-10-12 17:16:03.000000 pyinstaller-6.7.0/PyInstaller/utils/win32/winmanifest.py
+-rwxrwxrwx   0 root         (0) root         (0)     7625 2023-11-04 13:41:36.000000 pyinstaller-6.7.0/PyInstaller/utils/win32/winresource.py
+-rwxrwxrwx   0 root         (0) root         (0)     9175 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/PyInstaller/utils/win32/winutils.py
+-rwxrwxrwx   0 root         (0) root         (0)     5375 2024-05-21 22:34:49.000000 pyinstaller-6.7.0/README.rst
+-rwxrwxrwx   0 root         (0) root         (0)     1955 2024-01-13 17:58:01.000000 pyinstaller-6.7.0/alpine.dockerfile
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.651310 pyinstaller-6.7.0/bootloader/
+-rwxrwxrwx   0 root         (0) root         (0)       11 2023-09-30 18:27:19.000000 pyinstaller-6.7.0/bootloader/.gitattributes
+-rwxrwxrwx   0 root         (0) root         (0)     2053 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/Dockerfile
+-rwxrwxrwx   0 root         (0) root         (0)     3924 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/Dockerfile.osxcross
+-rwxrwxrwx   0 root         (0) root         (0)      950 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/README.txt
+-rwxrwxrwx   0 root         (0) root         (0)    15148 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/Vagrantfile
+-rwxrwxrwx   0 root         (0) root         (0)     1489 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/build.sh
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.670160 pyinstaller-6.7.0/bootloader/src/
+-rwxrwxrwx   0 root         (0) root         (0)     2599 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/src/main.c
+-rwxrwxrwx   0 root         (0) root         (0)      875 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/src/mkdtemp.h
+-rwxrwxrwx   0 root         (0) root         (0)    29474 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/src/pyi_apple_events.c
+-rwxrwxrwx   0 root         (0) root         (0)     1825 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/src/pyi_apple_events.h
+-rwxrwxrwx   0 root         (0) root         (0)    21690 2024-03-24 20:46:04.000000 pyinstaller-6.7.0/bootloader/src/pyi_archive.c
+-rwxrwxrwx   0 root         (0) root         (0)     5752 2023-10-12 17:16:14.000000 pyinstaller-6.7.0/bootloader/src/pyi_archive.h
+-rwxrwxrwx   0 root         (0) root         (0)    13273 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/src/pyi_exception_dialog.c
+-rwxrwxrwx   0 root         (0) root         (0)      822 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/src/pyi_exception_dialog.h
+-rwxrwxrwx   0 root         (0) root         (0)     7203 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/src/pyi_global.c
+-rwxrwxrwx   0 root         (0) root         (0)     8411 2023-11-20 00:50:49.000000 pyinstaller-6.7.0/bootloader/src/pyi_global.h
+-rwxrwxrwx   0 root         (0) root         (0)    25023 2023-11-20 00:50:49.000000 pyinstaller-6.7.0/bootloader/src/pyi_launch.c
+-rwxrwxrwx   0 root         (0) root         (0)     2092 2023-10-12 17:16:14.000000 pyinstaller-6.7.0/bootloader/src/pyi_launch.h
+-rwxrwxrwx   0 root         (0) root         (0)    20800 2024-03-24 20:46:04.000000 pyinstaller-6.7.0/bootloader/src/pyi_main.c
+-rwxrwxrwx   0 root         (0) root         (0)      564 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/src/pyi_main.h
+-rwxrwxrwx   0 root         (0) root         (0)    16553 2024-04-04 21:05:01.000000 pyinstaller-6.7.0/bootloader/src/pyi_path.c
+-rwxrwxrwx   0 root         (0) root         (0)     1567 2024-04-04 21:05:01.000000 pyinstaller-6.7.0/bootloader/src/pyi_path.h
+-rwxrwxrwx   0 root         (0) root         (0)    19484 2024-02-23 20:40:55.000000 pyinstaller-6.7.0/bootloader/src/pyi_pyconfig.c
+-rwxrwxrwx   0 root         (0) root         (0)     1925 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/src/pyi_pyconfig.h
+-rwxrwxrwx   0 root         (0) root         (0)     2348 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/src/pyi_pyconfig_v310.h
+-rwxrwxrwx   0 root         (0) root         (0)     2503 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/src/pyi_pyconfig_v311.h
+-rwxrwxrwx   0 root         (0) root         (0)     2526 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/src/pyi_pyconfig_v312.h
+-rwxrwxrwx   0 root         (0) root         (0)     2250 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/src/pyi_pyconfig_v38.h
+-rwxrwxrwx   0 root         (0) root         (0)     2336 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/src/pyi_pyconfig_v39.h
+-rwxrwxrwx   0 root         (0) root         (0)     3997 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/src/pyi_python.c
+-rwxrwxrwx   0 root         (0) root         (0)     8491 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/src/pyi_python.h
+-rwxrwxrwx   0 root         (0) root         (0)    14251 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/src/pyi_pythonlib.c
+-rwxrwxrwx   0 root         (0) root         (0)     1071 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/src/pyi_pythonlib.h
+-rwxrwxrwx   0 root         (0) root         (0)    37395 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/src/pyi_splash.c
+-rwxrwxrwx   0 root         (0) root         (0)     6094 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/src/pyi_splash.h
+-rwxrwxrwx   0 root         (0) root         (0)     3386 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/src/pyi_splashlib.c
+-rwxrwxrwx   0 root         (0) root         (0)     4517 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/src/pyi_splashlib.h
+-rwxrwxrwx   0 root         (0) root         (0)    42745 2023-10-12 17:16:14.000000 pyinstaller-6.7.0/bootloader/src/pyi_utils.c
+-rwxrwxrwx   0 root         (0) root         (0)     2452 2023-10-12 17:16:14.000000 pyinstaller-6.7.0/bootloader/src/pyi_utils.h
+-rwxrwxrwx   0 root         (0) root         (0)    20248 2024-02-10 12:19:40.000000 pyinstaller-6.7.0/bootloader/src/pyi_win32_utils.c
+-rwxrwxrwx   0 root         (0) root         (0)     1356 2024-02-10 12:19:40.000000 pyinstaller-6.7.0/bootloader/src/pyi_win32_utils.h
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.671317 pyinstaller-6.7.0/bootloader/tests/
+-rwxrwxrwx   0 root         (0) root         (0)     3854 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/tests/test_launch.c
+-rwxrwxrwx   0 root         (0) root         (0)     7906 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/tests/test_path.c
+-rwxrwxrwx   0 root         (0) root         (0)     1770 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/tests/wscript
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.671738 pyinstaller-6.7.0/bootloader/tools/
+-rwxrwxrwx   0 root         (0) root         (0)     1768 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/tools/strip.py
+-rwxrwxrwx   0 root         (0) root         (0)    80769 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/uncrustify.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1820 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/update-waf.sh
+-rwxrwxrwx   0 root         (0) root         (0)     1581 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/waf
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.679270 pyinstaller-6.7.0/bootloader/waflib/
+-rwxrwxrwx   0 root         (0) root         (0)    30209 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/waflib/Build.py
+-rwxrwxrwx   0 root         (0) root         (0)     5179 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/waflib/ConfigSet.py
+-rwxrwxrwx   0 root         (0) root         (0)    14831 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/waflib/Configure.py
+-rwxrwxrwx   0 root         (0) root         (0)    14805 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/waflib/Context.py
+-rwxrwxrwx   0 root         (0) root         (0)     1248 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/waflib/Errors.py
+-rwxrwxrwx   0 root         (0) root         (0)     7207 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/waflib/Logs.py
+-rwxrwxrwx   0 root         (0) root         (0)    15286 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/waflib/Node.py
+-rwxrwxrwx   0 root         (0) root         (0)    11367 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/waflib/Options.py
+-rwxrwxrwx   0 root         (0) root         (0)    13041 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/waflib/Runner.py
+-rwxrwxrwx   0 root         (0) root         (0)    15382 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/waflib/Scripting.py
+-rwxrwxrwx   0 root         (0) root         (0)    28095 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/waflib/Task.py
+-rwxrwxrwx   0 root         (0) root         (0)    17611 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/waflib/TaskGen.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.706077 pyinstaller-6.7.0/bootloader/waflib/Tools/
+-rwxrwxrwx   0 root         (0) root         (0)      120 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/waflib/Tools/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      360 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/waflib/Tools/ar.py
+-rwxrwxrwx   0 root         (0) root         (0)     2090 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/waflib/Tools/asm.py
+-rwxrwxrwx   0 root         (0) root         (0)      933 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/waflib/Tools/bison.py
+-rwxrwxrwx   0 root         (0) root         (0)     1220 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/waflib/Tools/c.py
+-rwxrwxrwx   0 root         (0) root         (0)     1893 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/waflib/Tools/c_aliases.py
+-rwxrwxrwx   0 root         (0) root         (0)    31523 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/waflib/Tools/c_config.py
+-rwxrwxrwx   0 root         (0) root         (0)     5203 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/waflib/Tools/c_osx.py
+-rwxrwxrwx   0 root         (0) root         (0)    25054 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/waflib/Tools/c_preproc.py
+-rwxrwxrwx   0 root         (0) root         (0)     5042 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/waflib/Tools/c_tests.py
+-rwxrwxrwx   0 root         (0) root         (0)    19729 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/waflib/Tools/ccroot.py
+-rwxrwxrwx   0 root         (0) root         (0)      594 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/waflib/Tools/clang.py
+-rwxrwxrwx   0 root         (0) root         (0)      606 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/waflib/Tools/clangxx.py
+-rwxrwxrwx   0 root         (0) root         (0)     2165 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/waflib/Tools/compiler_c.py
+-rwxrwxrwx   0 root         (0) root         (0)     2178 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/waflib/Tools/compiler_cxx.py
+-rwxrwxrwx   0 root         (0) root         (0)     1689 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/waflib/Tools/compiler_d.py
+-rwxrwxrwx   0 root         (0) root         (0)     2006 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/waflib/Tools/compiler_fc.py
+-rwxrwxrwx   0 root         (0) root         (0)     4439 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/waflib/Tools/cs.py
+-rwxrwxrwx   0 root         (0) root         (0)     1295 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/waflib/Tools/cxx.py
+-rwxrwxrwx   0 root         (0) root         (0)     2297 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/waflib/Tools/d.py
+-rwxrwxrwx   0 root         (0) root         (0)     1306 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/waflib/Tools/d_config.py
+-rwxrwxrwx   0 root         (0) root         (0)     4337 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/waflib/Tools/d_scan.py
+-rwxrwxrwx   0 root         (0) root         (0)     1227 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/waflib/Tools/dbus.py
+-rwxrwxrwx   0 root         (0) root         (0)     1643 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/waflib/Tools/dmd.py
+-rwxrwxrwx   0 root         (0) root         (0)     8302 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/waflib/Tools/errcheck.py
+-rwxrwxrwx   0 root         (0) root         (0)     5373 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/waflib/Tools/fc.py
+-rwxrwxrwx   0 root         (0) root         (0)    11313 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/waflib/Tools/fc_config.py
+-rwxrwxrwx   0 root         (0) root         (0)     2414 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/waflib/Tools/fc_scan.py
+-rwxrwxrwx   0 root         (0) root         (0)     1377 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/waflib/Tools/flex.py
+-rwxrwxrwx   0 root         (0) root         (0)     1599 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/waflib/Tools/g95.py
+-rwxrwxrwx   0 root         (0) root         (0)      385 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/waflib/Tools/gas.py
+-rwxrwxrwx   0 root         (0) root         (0)     2985 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/waflib/Tools/gcc.py
+-rwxrwxrwx   0 root         (0) root         (0)      998 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/waflib/Tools/gdc.py
+-rwxrwxrwx   0 root         (0) root         (0)     2225 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/waflib/Tools/gfortran.py
+-rwxrwxrwx   0 root         (0) root         (0)    12984 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/waflib/Tools/glib2.py
+-rwxrwxrwx   0 root         (0) root         (0)     3104 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/waflib/Tools/gnu_dirs.py
+-rwxrwxrwx   0 root         (0) root         (0)     3054 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/waflib/Tools/gxx.py
+-rwxrwxrwx   0 root         (0) root         (0)      553 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/waflib/Tools/icc.py
+-rwxrwxrwx   0 root         (0) root         (0)      553 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/waflib/Tools/icpc.py
+-rwxrwxrwx   0 root         (0) root         (0)    11869 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/waflib/Tools/ifort.py
+-rwxrwxrwx   0 root         (0) root         (0)     4385 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/waflib/Tools/intltool.py
+-rwxrwxrwx   0 root         (0) root         (0)     1096 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/waflib/Tools/irixcc.py
+-rwxrwxrwx   0 root         (0) root         (0)    13193 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/waflib/Tools/javaw.py
+-rwxrwxrwx   0 root         (0) root         (0)     1068 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/waflib/Tools/ldc2.py
+-rwxrwxrwx   0 root         (0) root         (0)      641 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/waflib/Tools/lua.py
+-rwxrwxrwx   0 root         (0) root         (0)      801 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/waflib/Tools/md5_tstamp.py
+-rwxrwxrwx   0 root         (0) root         (0)    33374 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/waflib/Tools/msvc.py
+-rwxrwxrwx   0 root         (0) root         (0)      686 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/waflib/Tools/nasm.py
+-rwxrwxrwx   0 root         (0) root         (0)      305 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/waflib/Tools/nobuild.py
+-rwxrwxrwx   0 root         (0) root         (0)     3446 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/waflib/Tools/perl.py
+-rwxrwxrwx   0 root         (0) root         (0)    21797 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/waflib/Tools/python.py
+-rwxrwxrwx   0 root         (0) root         (0)    20211 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/waflib/Tools/qt5.py
+-rwxrwxrwx   0 root         (0) root         (0)     4384 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/waflib/Tools/ruby.py
+-rwxrwxrwx   0 root         (0) root         (0)     1324 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/waflib/Tools/suncc.py
+-rwxrwxrwx   0 root         (0) root         (0)     1358 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/waflib/Tools/suncxx.py
+-rwxrwxrwx   0 root         (0) root         (0)    13995 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/waflib/Tools/tex.py
+-rwxrwxrwx   0 root         (0) root         (0)    10164 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/waflib/Tools/vala.py
+-rwxrwxrwx   0 root         (0) root         (0)     7884 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/waflib/Tools/waf_unit_test.py
+-rwxrwxrwx   0 root         (0) root         (0)     2097 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/waflib/Tools/winres.py
+-rwxrwxrwx   0 root         (0) root         (0)     1204 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/waflib/Tools/xlc.py
+-rwxrwxrwx   0 root         (0) root         (0)     1247 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/waflib/Tools/xlcxx.py
+-rwxrwxrwx   0 root         (0) root         (0)    19314 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/waflib/Utils.py
+-rwxrwxrwx   0 root         (0) root         (0)      120 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/waflib/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    12079 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/waflib/ansiterm.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.706621 pyinstaller-6.7.0/bootloader/waflib/extras/
+-rwxrwxrwx   0 root         (0) root         (0)      120 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/waflib/extras/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1509 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/waflib/fixpy2.py
+-rwxrwxrwx   0 root         (0) root         (0)     1764 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/waflib/processor.py
+-rwxrwxrwx   0 root         (0) root         (0)    37246 2024-03-09 19:48:33.000000 pyinstaller-6.7.0/bootloader/wscript
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.718564 pyinstaller-6.7.0/bootloader/zlib/
+-rwxrwxrwx   0 root         (0) root         (0)      278 2024-02-10 12:19:40.000000 pyinstaller-6.7.0/bootloader/zlib/README
+-rwxrwxrwx   0 root         (0) root         (0)     4964 2024-02-10 12:19:40.000000 pyinstaller-6.7.0/bootloader/zlib/adler32.c
+-rwxrwxrwx   0 root         (0) root         (0)    31605 2024-02-10 12:19:40.000000 pyinstaller-6.7.0/bootloader/zlib/crc32.c
+-rwxrwxrwx   0 root         (0) root         (0)   591749 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/zlib/crc32.h
+-rwxrwxrwx   0 root         (0) root         (0)     6676 2024-02-10 12:19:40.000000 pyinstaller-6.7.0/bootloader/zlib/gzguts.h
+-rwxrwxrwx   0 root         (0) root         (0)    12924 2024-02-10 12:19:40.000000 pyinstaller-6.7.0/bootloader/zlib/inffast.c
+-rwxrwxrwx   0 root         (0) root         (0)      422 2024-02-10 12:19:40.000000 pyinstaller-6.7.0/bootloader/zlib/inffast.h
+-rwxrwxrwx   0 root         (0) root         (0)     6332 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/zlib/inffixed.h
+-rwxrwxrwx   0 root         (0) root         (0)    55519 2024-02-10 12:19:40.000000 pyinstaller-6.7.0/bootloader/zlib/inflate.c
+-rwxrwxrwx   0 root         (0) root         (0)     6683 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/bootloader/zlib/inflate.h
+-rwxrwxrwx   0 root         (0) root         (0)    13024 2024-02-10 12:19:40.000000 pyinstaller-6.7.0/bootloader/zlib/inftrees.c
+-rwxrwxrwx   0 root         (0) root         (0)     2920 2024-02-10 12:19:40.000000 pyinstaller-6.7.0/bootloader/zlib/inftrees.h
+-rwxrwxrwx   0 root         (0) root         (0)    16500 2024-02-10 12:19:40.000000 pyinstaller-6.7.0/bootloader/zlib/zconf.h
+-rwxrwxrwx   0 root         (0) root         (0)    96829 2024-02-10 12:19:40.000000 pyinstaller-6.7.0/bootloader/zlib/zlib.h
+-rwxrwxrwx   0 root         (0) root         (0)     7179 2024-02-10 12:19:40.000000 pyinstaller-6.7.0/bootloader/zlib/zutil.c
+-rwxrwxrwx   0 root         (0) root         (0)     6677 2024-02-10 12:19:40.000000 pyinstaller-6.7.0/bootloader/zlib/zutil.h
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.726724 pyinstaller-6.7.0/doc/
+-rwxrwxrwx   0 root         (0) root         (0)    10417 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/doc/CHANGES-1.rst
+-rwxrwxrwx   0 root         (0) root         (0)     6193 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/doc/CHANGES-2.rst
+-rwxrwxrwx   0 root         (0) root         (0)    51520 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/doc/CHANGES-3.rst
+-rwxrwxrwx   0 root         (0) root         (0)   152282 2024-05-21 22:34:44.000000 pyinstaller-6.7.0/doc/CHANGES.rst
+-rwxrwxrwx   0 root         (0) root         (0)    20947 2024-05-21 22:34:48.000000 pyinstaller-6.7.0/doc/CREDITS.rst
+-rwxrwxrwx   0 root         (0) root         (0)     7447 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/doc/Makefile
+-rwxrwxrwx   0 root         (0) root         (0)     4327 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/doc/_common_definitions.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.727733 pyinstaller-6.7.0/doc/_static/
+-rwxrwxrwx   0 root         (0) root         (0)     3986 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/doc/_static/CArchive.png
+-rwxrwxrwx   0 root         (0) root         (0)     3058 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/doc/_static/SE_exe.png
+-rwxrwxrwx   0 root         (0) root         (0)     3521 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/doc/_static/ZlibArchive.png
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.728643 pyinstaller-6.7.0/doc/_static/css/
+-rwxrwxrwx   0 root         (0) root         (0)      963 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/doc/_static/css/pyinstaller.css
+-rwxrwxrwx   0 root         (0) root         (0)    16059 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/doc/_static/pyinstaller-draft1a-100_trans.png
+-rwxrwxrwx   0 root         (0) root         (0)   217780 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/doc/_static/pyinstaller-draft1a.ico
+-rwxrwxrwx   0 root         (0) root         (0)    24495 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/doc/advanced-topics.rst
+-rwxrwxrwx   0 root         (0) root         (0)    18719 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/doc/bootloader-building.rst
+-rwxrwxrwx   0 root         (0) root         (0)    20792 2024-01-13 17:58:01.000000 pyinstaller-6.7.0/doc/common-issues-and-pitfalls.rst
+-rwxrwxrwx   0 root         (0) root         (0)    14400 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/doc/conf.py
+-rwxrwxrwx   0 root         (0) root         (0)     3322 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/doc/contributing.rst
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.730558 pyinstaller-6.7.0/doc/development/
+-rwxrwxrwx   0 root         (0) root         (0)     1749 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/doc/development/branch-model.rst
+-rwxrwxrwx   0 root         (0) root         (0)     2755 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/doc/development/changelog-entries.rst
+-rwxrwxrwx   0 root         (0) root         (0)     1025 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/doc/development/coding-conventions.rst
+-rwxrwxrwx   0 root         (0) root         (0)     9608 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/doc/development/commit-messages.rst
+-rwxrwxrwx   0 root         (0) root         (0)     2681 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/doc/development/documentation.rst
+-rwxrwxrwx   0 root         (0) root         (0)      811 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/doc/development/git.rst
+-rwxrwxrwx   0 root         (0) root         (0)      415 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/doc/development/index.rst
+-rwxrwxrwx   0 root         (0) root         (0)     3473 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/doc/development/pull-requests.rst
+-rwxrwxrwx   0 root         (0) root         (0)     2221 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/doc/development/quickstart.rst
+-rwxrwxrwx   0 root         (0) root         (0)     2100 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/doc/development/testing.rst
+-rwxrwxrwx   0 root         (0) root         (0)     1204 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/doc/development/venv.rst
+-rwxrwxrwx   0 root         (0) root         (0)    75507 2024-04-04 21:05:01.000000 pyinstaller-6.7.0/doc/feature-notes.rst
+-rwxrwxrwx   0 root         (0) root         (0)     4432 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/doc/help2rst.py
+-rwxrwxrwx   0 root         (0) root         (0)    16431 2024-03-09 19:48:33.000000 pyinstaller-6.7.0/doc/hooks-config.rst
+-rwxrwxrwx   0 root         (0) root         (0)    26257 2024-01-13 17:58:01.000000 pyinstaller-6.7.0/doc/hooks.rst
+-rwxrwxrwx   0 root         (0) root         (0)     2398 2024-05-07 21:13:00.000000 pyinstaller-6.7.0/doc/index.rst
+-rwxrwxrwx   0 root         (0) root         (0)     4890 2024-05-07 21:13:00.000000 pyinstaller-6.7.0/doc/installation.rst
+-rwxrwxrwx   0 root         (0) root         (0)     1024 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/doc/license.rst
+-rwxrwxrwx   0 root         (0) root         (0)     6994 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/doc/make.bat
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.730893 pyinstaller-6.7.0/doc/man/
+-rwxrwxrwx   0 root         (0) root         (0)     1495 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/doc/man/pyi-makespec.rst
+-rwxrwxrwx   0 root         (0) root         (0)     1663 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/doc/man/pyinstaller.rst
+-rwxrwxrwx   0 root         (0) root         (0)       96 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/doc/man-pages.rst
+-rwxrwxrwx   0 root         (0) root         (0)    11767 2024-04-04 21:05:01.000000 pyinstaller-6.7.0/doc/operating-mode.rst
+-rwxrwxrwx   0 root         (0) root         (0)    13299 2024-05-21 22:34:48.000000 pyinstaller-6.7.0/doc/pyi-makespec.1
+-rwxrwxrwx   0 root         (0) root         (0)    14185 2024-05-21 22:34:48.000000 pyinstaller-6.7.0/doc/pyinstaller.1
+-rwxrwxrwx   0 root         (0) root         (0)     2004 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/doc/requirements.rst
+-rwxrwxrwx   0 root         (0) root         (0)      677 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/doc/requirements.txt
+-rwxrwxrwx   0 root         (0) root         (0)     9176 2024-02-10 12:19:40.000000 pyinstaller-6.7.0/doc/runtime-information.rst
+-rwxrwxrwx   0 root         (0) root         (0)    30301 2024-04-04 21:05:01.000000 pyinstaller-6.7.0/doc/spec-files.rst
+-rwxrwxrwx   0 root         (0) root         (0)    32897 2024-04-04 21:05:01.000000 pyinstaller-6.7.0/doc/usage.rst
+-rwxrwxrwx   0 root         (0) root         (0)    14242 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/doc/when-things-go-wrong.rst
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.736572 pyinstaller-6.7.0/icons/
+-rwxrwxrwx   0 root         (0) root         (0)   266950 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/icons/github_logo.png
+-rwxrwxrwx   0 root         (0) root         (0)   339276 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/icons/icon-console.svg
+-rwxrwxrwx   0 root         (0) root         (0)   339293 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/icons/icon-windowed.svg
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.739629 pyinstaller-6.7.0/news/
+-rwxrwxrwx   0 root         (0) root         (0)       12 2023-09-30 18:27:19.000000 pyinstaller-6.7.0/news/.gitignore
+-rwxrwxrwx   0 root         (0) root         (0)     2755 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/news/README.txt
+-rwxrwxrwx   0 root         (0) root         (0)     1065 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/news/_template.rst
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.741490 pyinstaller-6.7.0/pyinstaller.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     8277 2024-05-21 22:38:37.000000 pyinstaller-6.7.0/pyinstaller.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)    67332 2024-05-21 22:38:37.000000 pyinstaller-6.7.0/pyinstaller.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2024-05-21 22:38:37.000000 pyinstaller-6.7.0/pyinstaller.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)      376 2024-05-21 22:38:37.000000 pyinstaller-6.7.0/pyinstaller.egg-info/entry_points.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2024-05-21 22:38:24.000000 pyinstaller-6.7.0/pyinstaller.egg-info/not-zip-safe
+-rwxrwxrwx   0 root         (0) root         (0)      319 2024-05-21 22:38:37.000000 pyinstaller-6.7.0/pyinstaller.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       12 2024-05-21 22:38:37.000000 pyinstaller-6.7.0/pyinstaller.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)     2551 2024-02-10 12:19:40.000000 pyinstaller-6.7.0/pyproject.toml
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.742509 pyinstaller-6.7.0/release/
+-rwxrwxrwx   0 root         (0) root         (0)     2036 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/release/README.rst
+-rwxrwxrwx   0 root         (0) root         (0)      487 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/release/build-manylinux
+-rwxrwxrwx   0 root         (0) root         (0)     1340 2024-05-21 22:37:55.000000 pyinstaller-6.7.0/release/release.fish
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.744502 pyinstaller-6.7.0/scripts/
+-rwxrwxrwx   0 root         (0) root         (0)      166 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/scripts/clean
+-rwxrwxrwx   0 root         (0) root         (0)       68 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/scripts/clean.bat
+-rwxrwxrwx   0 root         (0) root         (0)     1876 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/scripts/find-empty-hooks.py
+-rwxrwxrwx   0 root         (0) root         (0)     6327 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/scripts/update-copyright
+-rwxrwxrwx   0 root         (0) root         (0)      362 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/scripts/update-readme-versions.sh
+-rwxrwxrwx   0 root         (0) root         (0)     2048 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/scripts/verify-news-fragments.py
+-rwxrwxrwx   0 root         (0) root         (0)     3980 2024-05-21 22:38:37.926917 pyinstaller-6.7.0/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)    10872 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.746671 pyinstaller-6.7.0/tests/
+-rwxrwxrwx   0 root         (0) root         (0)     4442 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.761747 pyinstaller-6.7.0/tests/functional/
+-rwxrwxrwx   0 root         (0) root         (0)      208 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/README
+-rwxrwxrwx   0 root         (0) root         (0)       98 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/conftest.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.523769 pyinstaller-6.7.0/tests/functional/data/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.761976 pyinstaller-6.7.0/tests/functional/data/PIL_images/
+-rwxrwxrwx   0 root         (0) root         (0)     5758 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/data/PIL_images/tinysample.tiff
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.762514 pyinstaller-6.7.0/tests/functional/data/Qt_Ui_file/
+-rwxrwxrwx   0 root         (0) root         (0)      862 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/data/Qt_Ui_file/gui.ui
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.763000 pyinstaller-6.7.0/tests/functional/data/app_with_plugin/
+-rwxrwxrwx   0 root         (0) root         (0)      624 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/data/app_with_plugin/static_plugin.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.766339 pyinstaller-6.7.0/tests/functional/data/appimage/
+-rwxrwxrwx   0 root         (0) root         (0)   339293 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/data/appimage/AppIcon.svg
+-rwxrwxrwx   0 root         (0) root         (0)    20448 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/data/appimage/DirIcon.png
+-rwxrwxrwx   0 root         (0) root         (0)     1019 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/data/appimage/create.sh
+-rwxrwxrwx   0 root         (0) root         (0)      775 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/data/appimage/org.pyinstaller.appimage.test.appdata.xml
+-rwxrwxrwx   0 root         (0) root         (0)      243 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/data/appimage/org.pyinstaller.appimage.test.desktop
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.766548 pyinstaller-6.7.0/tests/functional/data/ctypes_dylib/
+-rwxrwxrwx   0 root         (0) root         (0)      695 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/data/ctypes_dylib/ctypes_dylib.c
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.768817 pyinstaller-6.7.0/tests/functional/data/django/
+-rwxrwxrwx   0 root         (0) root         (0)   131072 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/data/django/db.sqlite3
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.770635 pyinstaller-6.7.0/tests/functional/data/django/django_site/
+-rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/data/django/django_site/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      399 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/data/django/django_site/asgi.py
+-rwxrwxrwx   0 root         (0) root         (0)     3230 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/data/django/django_site/settings.py
+-rwxrwxrwx   0 root         (0) root         (0)      753 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/data/django/django_site/urls.py
+-rwxrwxrwx   0 root         (0) root         (0)      399 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/data/django/django_site/wsgi.py
+-rwxrwxrwx   0 root         (0) root         (0)      667 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/data/django/manage.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.770872 pyinstaller-6.7.0/tests/functional/data/invalid_icon/
+-rwxrwxrwx   0 root         (0) root         (0)      587 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/data/invalid_icon/pyi_icon.png
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.771113 pyinstaller-6.7.0/tests/functional/data/name_clash_with_entry_point/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.771571 pyinstaller-6.7.0/tests/functional/data/name_clash_with_entry_point/matching_name/
+-rwxrwxrwx   0 root         (0) root         (0)       56 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/data/name_clash_with_entry_point/matching_name/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       57 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/data/name_clash_with_entry_point/matching_name/submodule.py
+-rwxrwxrwx   0 root         (0) root         (0)       83 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/data/name_clash_with_entry_point/matching_name.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.772124 pyinstaller-6.7.0/tests/functional/data/requests/
+-rwxrwxrwx   0 root         (0) root         (0)      294 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/data/requests/openssl.conf
+-rwxrwxrwx   0 root         (0) root         (0)     5524 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/data/requests/server.pem
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.774273 pyinstaller-6.7.0/tests/functional/data/set_icon/
+-rwxrwxrwx   0 root         (0) root         (0)   108027 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/data/set_icon/pyi_icon.icns
+-rwxrwxrwx   0 root         (0) root         (0)    56493 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/data/set_icon/pyi_icon.ico
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.775925 pyinstaller-6.7.0/tests/functional/data/sphinx/
+-rwxrwxrwx   0 root         (0) root         (0)     9476 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/data/sphinx/conf.py
+-rwxrwxrwx   0 root         (0) root         (0)      489 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/data/sphinx/index.rst
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.776152 pyinstaller-6.7.0/tests/functional/data/splash/
+-rwxrwxrwx   0 root         (0) root         (0)    20448 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/data/splash/image.png
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.782550 pyinstaller-6.7.0/tests/functional/logs/
+-rwxrwxrwx   0 root         (0) root         (0)       66 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/logs/multipackage1_B.toc
+-rwxrwxrwx   0 root         (0) root         (0)       41 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/logs/multipackage2_B.toc
+-rwxrwxrwx   0 root         (0) root         (0)       78 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/logs/multipackage3_B.toc
+-rwxrwxrwx   0 root         (0) root         (0)       41 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/logs/multipackage4_B.toc
+-rwxrwxrwx   0 root         (0) root         (0)       41 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/logs/multipackage5_B.toc
+-rwxrwxrwx   0 root         (0) root         (0)      146 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/logs/multipackage5_C.toc
+-rwxrwxrwx   0 root         (0) root         (0)      375 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/logs/pyi_import_relative.toc
+-rwxrwxrwx   0 root         (0) root         (0)       54 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/logs/test_hiddenimport.toc
+-rwxrwxrwx   0 root         (0) root         (0)       74 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/logs/test_keyring.toc
+-rwxrwxrwx   0 root         (0) root         (0)      117 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/logs/test_multipackage1.toc
+-rwxrwxrwx   0 root         (0) root         (0)      149 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/logs/test_multipackage2.toc
+-rwxrwxrwx   0 root         (0) root         (0)      117 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/logs/test_multipackage3.toc
+-rwxrwxrwx   0 root         (0) root         (0)      149 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/logs/test_multipackage4.toc
+-rwxrwxrwx   0 root         (0) root         (0)      149 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/logs/test_multipackage5.toc
+-rwxrwxrwx   0 root         (0) root         (0)       79 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/logs/test_nspkg1.toc
+-rwxrwxrwx   0 root         (0) root         (0)       49 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/logs/test_nspkg1_bbb_zzz.toc
+-rwxrwxrwx   0 root         (0) root         (0)       15 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/logs/test_nspkg1_empty.toc
+-rwxrwxrwx   0 root         (0) root         (0)       79 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/logs/test_nspkg2.toc
+-rwxrwxrwx   0 root         (0) root         (0)       75 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/logs/test_nspkg3.toc
+-rwxrwxrwx   0 root         (0) root         (0)       30 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/logs/test_nspkg3_aaa.toc
+-rwxrwxrwx   0 root         (0) root         (0)       49 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/logs/test_nspkg3_bbb_zzz.toc
+-rwxrwxrwx   0 root         (0) root         (0)       15 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/logs/test_nspkg3_empty.toc
+-rwxrwxrwx   0 root         (0) root         (0)      140 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/logs/test_nspkg_pep420.toc
+-rwxrwxrwx   0 root         (0) root         (0)      221 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/logs/test_option_verbose.toc
+-rwxrwxrwx   0 root         (0) root         (0)       14 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/logs/test_pil_FixTk.toc
+-rwxrwxrwx   0 root         (0) root         (0)       32 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/logs/test_pil_PyQt5.toc
+-rwxrwxrwx   0 root         (0) root         (0)       44 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/logs/test_pkg_without_hook_for_pkg.toc
+-rwxrwxrwx   0 root         (0) root         (0)       14 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/logs/test_tkinter_FixTk.toc
+-rwxrwxrwx   0 root         (0) root         (0)       35 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/logs/test_zope_interface.toc
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.786459 pyinstaller-6.7.0/tests/functional/modules/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.787196 pyinstaller-6.7.0/tests/functional/modules/a_hidden_import/
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/a_hidden_import/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/a_hidden_import/submodule.py
+-rwxrwxrwx   0 root         (0) root         (0)      523 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/error_during_import2.py
+-rwxrwxrwx   0 root         (0) root         (0)      547 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/module_with_coding_utf8.py
+-rwxrwxrwx   0 root         (0) root         (0)      615 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/module_with_utf8_emoji.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.524038 pyinstaller-6.7.0/tests/functional/modules/nspkg-pep420/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.523986 pyinstaller-6.7.0/tests/functional/modules/nspkg-pep420/path1/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.787442 pyinstaller-6.7.0/tests/functional/modules/nspkg-pep420/path1/package/
+-rwxrwxrwx   0 root         (0) root         (0)       21 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/nspkg-pep420/path1/package/sub2.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.524058 pyinstaller-6.7.0/tests/functional/modules/nspkg-pep420/path2/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.787655 pyinstaller-6.7.0/tests/functional/modules/nspkg-pep420/path2/package/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.787850 pyinstaller-6.7.0/tests/functional/modules/nspkg-pep420/path2/package/nspkg/
+-rwxrwxrwx   0 root         (0) root         (0)       26 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/nspkg-pep420/path2/package/nspkg/mod.py
+-rwxrwxrwx   0 root         (0) root         (0)       21 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/nspkg-pep420/path2/package/sub1.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.788234 pyinstaller-6.7.0/tests/functional/modules/nspkg-pep420/path2/package/subpackage/
+-rwxrwxrwx   0 root         (0) root         (0)       27 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/nspkg-pep420/path2/package/subpackage/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       31 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/nspkg-pep420/path2/package/subpackage/sub.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.788950 pyinstaller-6.7.0/tests/functional/modules/nspkg1-pkg/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.524277 pyinstaller-6.7.0/tests/functional/modules/nspkg1-pkg/nspkg1_aaa.egg/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.790274 pyinstaller-6.7.0/tests/functional/modules/nspkg1-pkg/nspkg1_aaa.egg/EGG-INFO/
+-rwxrwxrwx   0 root         (0) root         (0)      205 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/nspkg1-pkg/nspkg1_aaa.egg/EGG-INFO/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      262 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/nspkg1-pkg/nspkg1_aaa.egg/EGG-INFO/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/nspkg1-pkg/nspkg1_aaa.egg/EGG-INFO/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)        7 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/nspkg1-pkg/nspkg1_aaa.egg/EGG-INFO/namespace_packages.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/nspkg1-pkg/nspkg1_aaa.egg/EGG-INFO/not-zip-safe
+-rwxrwxrwx   0 root         (0) root         (0)        7 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/nspkg1-pkg/nspkg1_aaa.egg/EGG-INFO/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.790469 pyinstaller-6.7.0/tests/functional/modules/nspkg1-pkg/nspkg1_aaa.egg/nspkg1/
+-rwxrwxrwx   0 root         (0) root         (0)       64 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/nspkg1-pkg/nspkg1_aaa.egg/nspkg1/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.790659 pyinstaller-6.7.0/tests/functional/modules/nspkg1-pkg/nspkg1_aaa.egg/nspkg1/aaa/
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/nspkg1-pkg/nspkg1_aaa.egg/nspkg1/aaa/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1545 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/nspkg1-pkg/nspkg1_bbb.egg
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.524416 pyinstaller-6.7.0/tests/functional/modules/nspkg1-pkg/nspkg1_ccc.egg/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.791808 pyinstaller-6.7.0/tests/functional/modules/nspkg1-pkg/nspkg1_ccc.egg/EGG-INFO/
+-rwxrwxrwx   0 root         (0) root         (0)      205 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/nspkg1-pkg/nspkg1_ccc.egg/EGG-INFO/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      253 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/nspkg1-pkg/nspkg1_ccc.egg/EGG-INFO/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/nspkg1-pkg/nspkg1_ccc.egg/EGG-INFO/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)        7 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/nspkg1-pkg/nspkg1_ccc.egg/EGG-INFO/namespace_packages.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/nspkg1-pkg/nspkg1_ccc.egg/EGG-INFO/not-zip-safe
+-rwxrwxrwx   0 root         (0) root         (0)        7 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/nspkg1-pkg/nspkg1_ccc.egg/EGG-INFO/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.792177 pyinstaller-6.7.0/tests/functional/modules/nspkg1-pkg/nspkg1_ccc.egg/nspkg1/
+-rwxrwxrwx   0 root         (0) root         (0)       64 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/nspkg1-pkg/nspkg1_ccc.egg/nspkg1/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/nspkg1-pkg/nspkg1_ccc.egg/nspkg1/ccc.py
+-rwxrwxrwx   0 root         (0) root         (0)     1193 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/nspkg1-pkg/nspkg1_empty.egg
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.793203 pyinstaller-6.7.0/tests/functional/modules/nspkg2-pkg/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.793398 pyinstaller-6.7.0/tests/functional/modules/nspkg2-pkg/nspkg2/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.793578 pyinstaller-6.7.0/tests/functional/modules/nspkg2-pkg/nspkg2/aaa/
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/nspkg2-pkg/nspkg2/aaa/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.524594 pyinstaller-6.7.0/tests/functional/modules/nspkg2-pkg/nspkg2/bbb/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.793750 pyinstaller-6.7.0/tests/functional/modules/nspkg2-pkg/nspkg2/bbb/zzz/
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/nspkg2-pkg/nspkg2/bbb/zzz/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/nspkg2-pkg/nspkg2/ccc.py
+-rwxrwxrwx   0 root         (0) root         (0)      307 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/nspkg2-pkg/nspkg2_aaa-nspkg.pth
+-rwxrwxrwx   0 root         (0) root         (0)      676 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/nspkg2-pkg/nspkg2_bbb-nspkg.pth
+-rwxrwxrwx   0 root         (0) root         (0)      307 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/nspkg2-pkg/nspkg2_ccc-nspkg.pth
+-rwxrwxrwx   0 root         (0) root         (0)      305 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/nspkg2-pkg/nspkg2_empty-nspkg.pth
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.794365 pyinstaller-6.7.0/tests/functional/modules/nspkg3-pkg/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.524749 pyinstaller-6.7.0/tests/functional/modules/nspkg3-pkg/nspkg3_aaa.egg/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.795777 pyinstaller-6.7.0/tests/functional/modules/nspkg3-pkg/nspkg3_aaa.egg/EGG-INFO/
+-rwxrwxrwx   0 root         (0) root         (0)      205 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/nspkg3-pkg/nspkg3_aaa.egg/EGG-INFO/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      262 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/nspkg3-pkg/nspkg3_aaa.egg/EGG-INFO/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/nspkg3-pkg/nspkg3_aaa.egg/EGG-INFO/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)        7 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/nspkg3-pkg/nspkg3_aaa.egg/EGG-INFO/namespace_packages.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/nspkg3-pkg/nspkg3_aaa.egg/EGG-INFO/not-zip-safe
+-rwxrwxrwx   0 root         (0) root         (0)        7 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/nspkg3-pkg/nspkg3_aaa.egg/EGG-INFO/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.795968 pyinstaller-6.7.0/tests/functional/modules/nspkg3-pkg/nspkg3_aaa.egg/nspkg3/
+-rwxrwxrwx   0 root         (0) root         (0)       76 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/nspkg3-pkg/nspkg3_aaa.egg/nspkg3/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.796155 pyinstaller-6.7.0/tests/functional/modules/nspkg3-pkg/nspkg3_aaa.egg/nspkg3/aaa/
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/nspkg3-pkg/nspkg3_aaa.egg/nspkg3/aaa/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1560 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/nspkg3-pkg/nspkg3_bbb.egg
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.524890 pyinstaller-6.7.0/tests/functional/modules/nspkg3-pkg/nspkg3_ccc.egg/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.797243 pyinstaller-6.7.0/tests/functional/modules/nspkg3-pkg/nspkg3_ccc.egg/EGG-INFO/
+-rwxrwxrwx   0 root         (0) root         (0)      205 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/nspkg3-pkg/nspkg3_ccc.egg/EGG-INFO/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      253 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/nspkg3-pkg/nspkg3_ccc.egg/EGG-INFO/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/nspkg3-pkg/nspkg3_ccc.egg/EGG-INFO/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)        7 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/nspkg3-pkg/nspkg3_ccc.egg/EGG-INFO/namespace_packages.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/nspkg3-pkg/nspkg3_ccc.egg/EGG-INFO/not-zip-safe
+-rwxrwxrwx   0 root         (0) root         (0)        7 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/nspkg3-pkg/nspkg3_ccc.egg/EGG-INFO/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.797566 pyinstaller-6.7.0/tests/functional/modules/nspkg3-pkg/nspkg3_ccc.egg/nspkg3/
+-rwxrwxrwx   0 root         (0) root         (0)       76 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/nspkg3-pkg/nspkg3_ccc.egg/nspkg3/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/nspkg3-pkg/nspkg3_ccc.egg/nspkg3/ccc.py
+-rwxrwxrwx   0 root         (0) root         (0)     1202 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/nspkg3-pkg/nspkg3_empty.egg
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.797893 pyinstaller-6.7.0/tests/functional/modules/pkg3/
+-rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pkg3/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       57 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pkg3/sample-data.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.798083 pyinstaller-6.7.0/tests/functional/modules/pkg_without_hook_for_pkg/
+-rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pkg_without_hook_for_pkg/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.798276 pyinstaller-6.7.0/tests/functional/modules/pkg_without_hook_for_pkg/sub1/
+-rwxrwxrwx   0 root         (0) root         (0)      281 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pkg_without_hook_for_pkg/sub1/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.798467 pyinstaller-6.7.0/tests/functional/modules/pkg_without_hook_for_pkg/sub1/sub11/
+-rwxrwxrwx   0 root         (0) root         (0)       31 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pkg_without_hook_for_pkg/sub1/sub11/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      577 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_collect_submodules_mod.py
+-rwxrwxrwx   0 root         (0) root         (0)      230 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_dummy_module.py
+-rwxrwxrwx   0 root         (0) root         (0)     1399 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_egg_zipped.egg
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.525190 pyinstaller-6.7.0/tests/functional/modules/pyi_excluded_relative_imports/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.798664 pyinstaller-6.7.0/tests/functional/modules/pyi_excluded_relative_imports/hooks/
+-rwxrwxrwx   0 root         (0) root         (0)      165 2023-11-11 15:22:30.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_excluded_relative_imports/hooks/hook-mypackage.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.799190 pyinstaller-6.7.0/tests/functional/modules/pyi_excluded_relative_imports/mypackage/
+-rwxrwxrwx   0 root         (0) root         (0)      636 2023-11-11 15:22:30.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_excluded_relative_imports/mypackage/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      130 2023-11-11 15:22:30.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_excluded_relative_imports/mypackage/forbidden1.py
+-rwxrwxrwx   0 root         (0) root         (0)      437 2023-11-11 15:22:30.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_excluded_relative_imports/mypackage/submod1.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.799674 pyinstaller-6.7.0/tests/functional/modules/pyi_excluded_relative_imports/mypackage/subpkg1/
+-rwxrwxrwx   0 root         (0) root         (0)      545 2023-11-11 15:22:30.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_excluded_relative_imports/mypackage/subpkg1/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      130 2023-11-11 15:22:30.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_excluded_relative_imports/mypackage/subpkg1/forbidden2.py
+-rwxrwxrwx   0 root         (0) root         (0)      426 2023-11-11 15:22:30.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_excluded_relative_imports/mypackage/subpkg1/submod2.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.800171 pyinstaller-6.7.0/tests/functional/modules/pyi_excluded_relative_imports/mypackage/subpkg1/subpkg2/
+-rwxrwxrwx   0 root         (0) root         (0)      538 2023-11-11 15:22:30.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_excluded_relative_imports/mypackage/subpkg1/subpkg2/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      130 2023-11-11 15:22:30.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_excluded_relative_imports/mypackage/subpkg1/subpkg2/forbidden3.py
+-rwxrwxrwx   0 root         (0) root         (0)      424 2023-11-11 15:22:30.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_excluded_relative_imports/mypackage/subpkg1/subpkg2/submod3.py
+-rwxrwxrwx   0 root         (0) root         (0)     1277 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_get_datadir.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.525334 pyinstaller-6.7.0/tests/functional/modules/pyi_import_main/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.800511 pyinstaller-6.7.0/tests/functional/modules/pyi_import_main/hooks/
+-rwxrwxrwx   0 root         (0) root         (0)       94 2023-10-12 17:16:14.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_import_main/hooks/hook-PyInstaller.py
+-rwxrwxrwx   0 root         (0) root         (0)       84 2023-10-12 17:16:14.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_import_main/hooks/hook-pytest.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.525402 pyinstaller-6.7.0/tests/functional/modules/pyi_import_pyqt_uic_port/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.800843 pyinstaller-6.7.0/tests/functional/modules/pyi_import_pyqt_uic_port/PyQt5/
+-rwxrwxrwx   0 root         (0) root         (0)      371 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_import_pyqt_uic_port/PyQt5/QtCore.py
+-rwxrwxrwx   0 root         (0) root         (0)       88 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_import_pyqt_uic_port/PyQt5/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.801010 pyinstaller-6.7.0/tests/functional/modules/pyi_import_pyqt_uic_port/PyQt5/uic/
+-rwxrwxrwx   0 root         (0) root         (0)      118 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_import_pyqt_uic_port/PyQt5/uic/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.801351 pyinstaller-6.7.0/tests/functional/modules/pyi_import_pyqt_uic_port/PyQt5/uic/port_v2/
+-rwxrwxrwx   0 root         (0) root         (0)      148 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_import_pyqt_uic_port/PyQt5/uic/port_v2/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      151 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_import_pyqt_uic_port/PyQt5/uic/port_v2/test.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.801728 pyinstaller-6.7.0/tests/functional/modules/pyi_import_pyqt_uic_port/PyQt5/uic/port_v3/
+-rwxrwxrwx   0 root         (0) root         (0)      148 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_import_pyqt_uic_port/PyQt5/uic/port_v3/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      152 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_import_pyqt_uic_port/PyQt5/uic/port_v3/test.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.525586 pyinstaller-6.7.0/tests/functional/modules/pyi_inspect_getmodule_from_stackframes/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.802107 pyinstaller-6.7.0/tests/functional/modules/pyi_inspect_getmodule_from_stackframes/helper_package/
+-rwxrwxrwx   0 root         (0) root         (0)      138 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_inspect_getmodule_from_stackframes/helper_package/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      290 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_inspect_getmodule_from_stackframes/helper_package/helper_module.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.525656 pyinstaller-6.7.0/tests/functional/modules/pyi_issue_4141/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.802302 pyinstaller-6.7.0/tests/functional/modules/pyi_issue_4141/app/
+-rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_issue_4141/app/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.525803 pyinstaller-6.7.0/tests/functional/modules/pyi_missing_relative_import/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.802499 pyinstaller-6.7.0/tests/functional/modules/pyi_missing_relative_import/hooks/
+-rwxrwxrwx   0 root         (0) root         (0)       55 2023-11-04 13:41:36.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_missing_relative_import/hooks/hook-myotherpackage.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.802686 pyinstaller-6.7.0/tests/functional/modules/pyi_missing_relative_import/myotherpackage/
+-rwxrwxrwx   0 root         (0) root         (0)       22 2023-11-04 13:41:36.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_missing_relative_import/myotherpackage/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.802871 pyinstaller-6.7.0/tests/functional/modules/pyi_missing_relative_import/mypackage/
+-rwxrwxrwx   0 root         (0) root         (0)      391 2023-11-04 13:41:36.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_missing_relative_import/mypackage/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.525918 pyinstaller-6.7.0/tests/functional/modules/pyi_module_exclusion/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.803611 pyinstaller-6.7.0/tests/functional/modules/pyi_module_exclusion/hooks/
+-rwxrwxrwx   0 root         (0) root         (0)       65 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_module_exclusion/hooks/hook-mymodule_feature1.py
+-rwxrwxrwx   0 root         (0) root         (0)      387 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_module_exclusion/hooks/hook-mymodule_feature2.py
+-rwxrwxrwx   0 root         (0) root         (0)      507 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_module_exclusion/hooks/hook-mymodule_feature3.py
+-rwxrwxrwx   0 root         (0) root         (0)      155 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_module_exclusion/hooks/hook-mymodule_main.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.526013 pyinstaller-6.7.0/tests/functional/modules/pyi_module_exclusion/modules/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.803786 pyinstaller-6.7.0/tests/functional/modules/pyi_module_exclusion/modules/mymodule_feature1/
+-rwxrwxrwx   0 root         (0) root         (0)       22 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_module_exclusion/modules/mymodule_feature1/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.803954 pyinstaller-6.7.0/tests/functional/modules/pyi_module_exclusion/modules/mymodule_feature2/
+-rwxrwxrwx   0 root         (0) root         (0)       22 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_module_exclusion/modules/mymodule_feature2/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.804575 pyinstaller-6.7.0/tests/functional/modules/pyi_module_exclusion/modules/mymodule_main/
+-rwxrwxrwx   0 root         (0) root         (0)      619 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_module_exclusion/modules/mymodule_main/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      210 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_module_exclusion/modules/mymodule_main/submodule_feature3.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.805243 pyinstaller-6.7.0/tests/functional/modules/pyi_module_with_invalid_encoding/
+-rwxrwxrwx   0 root         (0) root         (0)      885 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_module_with_invalid_encoding/mymodule1.py
+-rwxrwxrwx   0 root         (0) root         (0)     1666 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_module_with_invalid_encoding/mymodule2.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.526167 pyinstaller-6.7.0/tests/functional/modules/pyi_namespace_package_with_data/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.805726 pyinstaller-6.7.0/tests/functional/modules/pyi_namespace_package_with_data/hooks/
+-rwxrwxrwx   0 root         (0) root         (0)      174 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_namespace_package_with_data/hooks/hook-pyi_test_nspkg.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.526190 pyinstaller-6.7.0/tests/functional/modules/pyi_namespace_package_with_data/package/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.806132 pyinstaller-6.7.0/tests/functional/modules/pyi_namespace_package_with_data/package/pyi_test_nspkg/
+-rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_namespace_package_with_data/package/pyi_test_nspkg/a.py
+-rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_namespace_package_with_data/package/pyi_test_nspkg/b.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.806700 pyinstaller-6.7.0/tests/functional/modules/pyi_namespace_package_with_data/package/pyi_test_nspkg/data/
+-rwxrwxrwx   0 root         (0) root         (0)       14 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_namespace_package_with_data/package/pyi_test_nspkg/data/data_file1.txt
+-rwxrwxrwx   0 root         (0) root         (0)       14 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_namespace_package_with_data/package/pyi_test_nspkg/data/data_file2.txt
+-rwxrwxrwx   0 root         (0) root         (0)       14 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_namespace_package_with_data/package/pyi_test_nspkg/data/data_file3.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.526840 pyinstaller-6.7.0/tests/functional/modules/pyi_optimization/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.806899 pyinstaller-6.7.0/tests/functional/modules/pyi_optimization/mypackage/
+-rwxrwxrwx   0 root         (0) root         (0)      864 2024-04-04 21:05:01.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_optimization/mypackage/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.526974 pyinstaller-6.7.0/tests/functional/modules/pyi_pkg_resources_provider/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.807295 pyinstaller-6.7.0/tests/functional/modules/pyi_pkg_resources_provider/hooks/
+-rwxrwxrwx   0 root         (0) root         (0)      642 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_pkg_resources_provider/hooks/hook-pyi_pkgres_testpkg.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.807495 pyinstaller-6.7.0/tests/functional/modules/pyi_pkg_resources_provider/package/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.808342 pyinstaller-6.7.0/tests/functional/modules/pyi_pkg_resources_provider/package/pyi_pkgres_testpkg/
+-rwxrwxrwx   0 root         (0) root         (0)       87 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_pkg_resources_provider/package/pyi_pkgres_testpkg/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_pkg_resources_provider/package/pyi_pkgres_testpkg/a.py
+-rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_pkg_resources_provider/package/pyi_pkgres_testpkg/b.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.808900 pyinstaller-6.7.0/tests/functional/modules/pyi_pkg_resources_provider/package/pyi_pkgres_testpkg/subpkg1/
+-rwxrwxrwx   0 root         (0) root         (0)       33 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_pkg_resources_provider/package/pyi_pkgres_testpkg/subpkg1/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_pkg_resources_provider/package/pyi_pkgres_testpkg/subpkg1/c.py
+-rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_pkg_resources_provider/package/pyi_pkgres_testpkg/subpkg1/d.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.809456 pyinstaller-6.7.0/tests/functional/modules/pyi_pkg_resources_provider/package/pyi_pkgres_testpkg/subpkg1/data/
+-rwxrwxrwx   0 root         (0) root         (0)       31 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_pkg_resources_provider/package/pyi_pkgres_testpkg/subpkg1/data/entry1.txt
+-rwxrwxrwx   0 root         (0) root         (0)       33 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_pkg_resources_provider/package/pyi_pkgres_testpkg/subpkg1/data/entry2.md
+-rwxrwxrwx   0 root         (0) root         (0)       35 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_pkg_resources_provider/package/pyi_pkgres_testpkg/subpkg1/data/entry3.rst
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.809648 pyinstaller-6.7.0/tests/functional/modules/pyi_pkg_resources_provider/package/pyi_pkgres_testpkg/subpkg1/data/extra/
+-rwxrwxrwx   0 root         (0) root         (0)       63 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_pkg_resources_provider/package/pyi_pkgres_testpkg/subpkg1/data/extra/extra_entry1.json
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.810025 pyinstaller-6.7.0/tests/functional/modules/pyi_pkg_resources_provider/package/pyi_pkgres_testpkg/subpkg2/
+-rwxrwxrwx   0 root         (0) root         (0)       72 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_pkg_resources_provider/package/pyi_pkgres_testpkg/subpkg2/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_pkg_resources_provider/package/pyi_pkgres_testpkg/subpkg2/mod.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.810370 pyinstaller-6.7.0/tests/functional/modules/pyi_pkg_resources_provider/package/pyi_pkgres_testpkg/subpkg2/subsubpkg21/
+-rwxrwxrwx   0 root         (0) root         (0)       32 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_pkg_resources_provider/package/pyi_pkgres_testpkg/subpkg2/subsubpkg21/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_pkg_resources_provider/package/pyi_pkgres_testpkg/subpkg2/subsubpkg21/mod.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.810696 pyinstaller-6.7.0/tests/functional/modules/pyi_pkg_resources_provider/package/pyi_pkgres_testpkg/subpkg3/
+-rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_pkg_resources_provider/package/pyi_pkgres_testpkg/subpkg3/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       42 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_pkg_resources_provider/package/pyi_pkgres_testpkg/subpkg3/_datafile.json
+-rwxrwxrwx   0 root         (0) root         (0)     1128 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_pkg_resources_provider/package/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.527458 pyinstaller-6.7.0/tests/functional/modules/pyi_pkgutil_itermodules/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.810870 pyinstaller-6.7.0/tests/functional/modules/pyi_pkgutil_itermodules/hooks/
+-rwxrwxrwx   0 root         (0) root         (0)      672 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_pkgutil_itermodules/hooks/hook-mypackage.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.527484 pyinstaller-6.7.0/tests/functional/modules/pyi_pkgutil_itermodules/package/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.812101 pyinstaller-6.7.0/tests/functional/modules/pyi_pkgutil_itermodules/package/mypackage/
+-rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_pkgutil_itermodules/package/mypackage/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       22 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_pkgutil_itermodules/package/mypackage/datafile.txt
+-rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_pkgutil_itermodules/package/mypackage/submodule_a.py
+-rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_pkgutil_itermodules/package/mypackage/submodule_b.py
+-rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_pkgutil_itermodules/package/mypackage/submodule_c.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.812470 pyinstaller-6.7.0/tests/functional/modules/pyi_single_file_metadata/
+-rwxrwxrwx   0 root         (0) root         (0)      196 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_single_file_metadata/README
+-rwxrwxrwx   0 root         (0) root         (0)      290 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_single_file_metadata/my_test_package-1.0.egg-info
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.527688 pyinstaller-6.7.0/tests/functional/modules/pyi_test_egg/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.812658 pyinstaller-6.7.0/tests/functional/modules/pyi_test_egg/hooks/
+-rwxrwxrwx   0 root         (0) root         (0)       99 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_test_egg/hooks/hook-unzipped_egg.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.527759 pyinstaller-6.7.0/tests/functional/modules/pyi_test_egg/pyi_egg_unzipped.egg/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.813505 pyinstaller-6.7.0/tests/functional/modules/pyi_test_egg/pyi_egg_unzipped.egg/EGG-INFO/
+-rwxrwxrwx   0 root         (0) root         (0)      215 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_test_egg/pyi_egg_unzipped.egg/EGG-INFO/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      232 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_test_egg/pyi_egg_unzipped.egg/EGG-INFO/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_test_egg/pyi_egg_unzipped.egg/EGG-INFO/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_test_egg/pyi_egg_unzipped.egg/EGG-INFO/not-zip-safe
+-rwxrwxrwx   0 root         (0) root         (0)       13 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_test_egg/pyi_egg_unzipped.egg/EGG-INFO/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.813675 pyinstaller-6.7.0/tests/functional/modules/pyi_test_egg/pyi_egg_unzipped.egg/unzipped_egg/
+-rwxrwxrwx   0 root         (0) root         (0)      678 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_test_egg/pyi_egg_unzipped.egg/unzipped_egg/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.814115 pyinstaller-6.7.0/tests/functional/modules/pyi_test_egg/pyi_egg_unzipped.egg/unzipped_egg/data/
+-rwxrwxrwx   0 root         (0) root         (0)       34 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_test_egg/pyi_egg_unzipped.egg/unzipped_egg/data/datafile.txt
+-rwxrwxrwx   0 root         (0) root         (0)     1139 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_dynamic.py
+-rwxrwxrwx   0 root         (0) root         (0)     1311 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_gettemp.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.814298 pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_metapath1/
+-rwxrwxrwx   0 root         (0) root         (0)     1654 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_metapath1/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.815085 pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_metapath1/_vendor/
+-rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_metapath1/_vendor/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      558 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_metapath1/_vendor/aaa.py
+-rwxrwxrwx   0 root         (0) root         (0)      558 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_metapath1/_vendor/bbb.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.815580 pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_metapath1/_vendor/ccc/
+-rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_metapath1/_vendor/ccc/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      817 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_metapath1/_vendor/ccc/ddd.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.816330 pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_metapath1/_vendor/ccc/eee/
+-rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_metapath1/_vendor/ccc/eee/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      555 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_metapath1/_vendor/ccc/eee/fff.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.816550 pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_metapath1/extern/
+-rwxrwxrwx   0 root         (0) root         (0)     4109 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_metapath1/extern/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.817113 pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_missing_submod/
+-rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_missing_submod/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.817335 pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_missing_submod/aaa/
+-rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_missing_submod/aaa/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.817773 pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_nameclash/
+-rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_nameclash/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       57 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_nameclash/nameclash.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.818509 pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_path/
+-rwxrwxrwx   0 root         (0) root         (0)      697 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_path/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.818749 pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_path/a/
+-rwxrwxrwx   0 root         (0) root         (0)      507 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_path/a/b.py
+-rwxrwxrwx   0 root         (0) root         (0)      525 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_path/b.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.819990 pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_relimp/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.821002 pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_relimp/B/
+-rwxrwxrwx   0 root         (0) root         (0)     1030 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_relimp/B/C.py
+-rwxrwxrwx   0 root         (0) root         (0)      589 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_relimp/B/D.py
+-rwxrwxrwx   0 root         (0) root         (0)      538 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_relimp/B/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      538 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_relimp/E.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.821472 pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_relimp/F/
+-rwxrwxrwx   0 root         (0) root         (0)      540 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_relimp/F/G.py
+-rwxrwxrwx   0 root         (0) root         (0)      585 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_relimp/F/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      536 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_relimp/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.822478 pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_relimp/pyi_testmod_relimp/
+-rwxrwxrwx   0 root         (0) root         (0)      555 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_relimp/pyi_testmod_relimp/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1251 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_relimp/pyi_testmod_relimp/relimp2.py
+-rwxrwxrwx   0 root         (0) root         (0)      563 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_relimp/pyi_testmod_relimp/relimp3.py
+-rwxrwxrwx   0 root         (0) root         (0)      945 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_relimp/relimp1.py
+-rwxrwxrwx   0 root         (0) root         (0)      544 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_relimp/relimp2.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.822690 pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_relimp2/
+-rwxrwxrwx   0 root         (0) root         (0)      507 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_relimp2/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.823125 pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_relimp2/bar/
+-rwxrwxrwx   0 root         (0) root         (0)      556 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_relimp2/bar/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.823356 pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_relimp2/bar/bar2/
+-rwxrwxrwx   0 root         (0) root         (0)      557 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_relimp2/bar/bar2/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      559 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_relimp2/bar/baz.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.823818 pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_relimp3a/
+-rwxrwxrwx   0 root         (0) root         (0)      507 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_relimp3a/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.824783 pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_relimp3a/aa/
+-rwxrwxrwx   0 root         (0) root         (0)      507 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_relimp3a/aa/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      853 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_relimp3a/aa/a1.py
+-rwxrwxrwx   0 root         (0) root         (0)      547 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_relimp3a/aa/pyi_testmod_relimp3c.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.825259 pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_relimp3a/pyi_testmod_relimp3b/
+-rwxrwxrwx   0 root         (0) root         (0)      507 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_relimp3a/pyi_testmod_relimp3b/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      540 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_relimp3a/pyi_testmod_relimp3b/b1.py
+-rwxrwxrwx   0 root         (0) root         (0)      525 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_relimp3a/pyi_testmod_relimp3c.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.825727 pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_relimp3b/
+-rwxrwxrwx   0 root         (0) root         (0)      507 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_relimp3b/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      525 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_relimp3b/b1.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.825967 pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_relimp3c/
+-rwxrwxrwx   0 root         (0) root         (0)      527 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_relimp3c/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.826435 pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_submodule_from_aliased_pkg/
+-rwxrwxrwx   0 root         (0) root         (0)        3 2023-11-23 19:10:52.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_submodule_from_aliased_pkg/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)        3 2023-11-23 19:10:52.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_submodule_from_aliased_pkg/submodule.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.827193 pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_submodule_global_shadowed/
+-rwxrwxrwx   0 root         (0) root         (0)      963 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_submodule_global_shadowed/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      750 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_submodule_global_shadowed/submodule.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.828174 pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_submodule_global_unshadowed/
+-rwxrwxrwx   0 root         (0) root         (0)     1605 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_submodule_global_unshadowed/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      756 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_submodule_global_unshadowed/submodule.py
+-rwxrwxrwx   0 root         (0) root         (0)      611 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_threading.py
+-rwxrwxrwx   0 root         (0) root         (0)      703 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/modules/resources_testmod.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.851065 pyinstaller-6.7.0/tests/functional/scripts/
+-rwxrwxrwx   0 root         (0) root         (0)      706 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/scripts/list_pytest11_entry_point.py
+-rwxrwxrwx   0 root         (0) root         (0)     1155 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/scripts/pkg_resource_res_string.py
+-rwxrwxrwx   0 root         (0) root         (0)      914 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/scripts/pkgutil_get_data.py
+-rwxrwxrwx   0 root         (0) root         (0)      896 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/scripts/pkgutil_get_data__main__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1490 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/scripts/pyi_absolute_ld_library_path.py
+-rwxrwxrwx   0 root         (0) root         (0)     1221 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/scripts/pyi_absolute_python_path.py
+-rwxrwxrwx   0 root         (0) root         (0)     1948 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/scripts/pyi_app_with_plugin.py
+-rwxrwxrwx   0 root         (0) root         (0)      177 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/scripts/pyi_arbitrary_ext.foo
+-rwxrwxrwx   0 root         (0) root         (0)     1559 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/scripts/pyi_c_extension.py
+-rwxrwxrwx   0 root         (0) root         (0)      870 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/scripts/pyi_codecs.py
+-rwxrwxrwx   0 root         (0) root         (0)      634 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/scripts/pyi_filename.py
+-rwxrwxrwx   0 root         (0) root         (0)     1824 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/scripts/pyi_frozen_stdlib_modules.py
+-rwxrwxrwx   0 root         (0) root         (0)     3636 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/scripts/pyi_future.py
+-rwxrwxrwx   0 root         (0) root         (0)     1325 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/scripts/pyi_get_meipass_value.py
+-rwxrwxrwx   0 root         (0) root         (0)     1138 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/scripts/pyi_getfilesystemencoding.py
+-rwxrwxrwx   0 root         (0) root         (0)      531 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/scripts/pyi_helloworld.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.852556 pyinstaller-6.7.0/tests/functional/scripts/pyi_hooks/
+-rwxrwxrwx   0 root         (0) root         (0)       56 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/scripts/pyi_hooks/hook-pkg_without_hook_for_pkg.sub1.py
+-rwxrwxrwx   0 root         (0) root         (0)      621 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/scripts/pyi_hooks/hook-pyi_collect_submodules_mod.py
+-rwxrwxrwx   0 root         (0) root         (0)      770 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/scripts/pyi_hooks/hook-pyi_testmod_metapath1.py
+-rwxrwxrwx   0 root         (0) root         (0)      821 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/scripts/pyi_hooks/hook-pyi_testmod_path.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.853050 pyinstaller-6.7.0/tests/functional/scripts/pyi_hooks/pre_safe_import_module/
+-rwxrwxrwx   0 root         (0) root         (0)      524 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/scripts/pyi_hooks/pre_safe_import_module/hook-alias_name.py
+-rwxrwxrwx   0 root         (0) root         (0)     1266 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/scripts/pyi_import_pyqt5_uic_port.py
+-rwxrwxrwx   0 root         (0) root         (0)    16548 2024-03-24 20:46:04.000000 pyinstaller-6.7.0/tests/functional/scripts/pyi_importlib_resources.py
+-rwxrwxrwx   0 root         (0) root         (0)     1191 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/scripts/pyi_interact_pyi_splash.py
+-rwxrwxrwx   0 root         (0) root         (0)     1329 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/scripts/pyi_issue_4141.py
+-rwxrwxrwx   0 root         (0) root         (0)     1093 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/scripts/pyi_lazy_import.py
+-rwxrwxrwx   0 root         (0) root         (0)      774 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/scripts/pyi_lib_PIL_img_conversion.py
+-rwxrwxrwx   0 root         (0) root         (0)     1031 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/scripts/pyi_lib_PyQt5-uic.py
+-rwxrwxrwx   0 root         (0) root         (0)     3112 2023-11-04 13:41:36.000000 pyinstaller-6.7.0/tests/functional/scripts/pyi_lib_requests.py
+-rwxrwxrwx   0 root         (0) root         (0)     1401 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/scripts/pyi_lib_sphinx.py
+-rwxrwxrwx   0 root         (0) root         (0)     2161 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/scripts/pyi_lib_tkinter.py
+-rwxrwxrwx   0 root         (0) root         (0)     1058 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/scripts/pyi_load_dll_using_ctypes.py
+-rwxrwxrwx   0 root         (0) root         (0)     1334 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/scripts/pyi_module__file__attribute.py
+-rwxrwxrwx   0 root         (0) root         (0)     2556 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/scripts/pyi_module_attributes.py
+-rwxrwxrwx   0 root         (0) root         (0)     1383 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/scripts/pyi_module_reload.py
+-rwxrwxrwx   0 root         (0) root         (0)     1254 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/scripts/pyi_multiprocessing_main_module_code_in_process.py
+-rwxrwxrwx   0 root         (0) root         (0)     2028 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/scripts/pyi_multiprocessing_nested_process.py
+-rwxrwxrwx   0 root         (0) root         (0)     1178 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/scripts/pyi_multiprocessing_pool.py
+-rwxrwxrwx   0 root         (0) root         (0)     1198 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/scripts/pyi_multiprocessing_process.py
+-rwxrwxrwx   0 root         (0) root         (0)     2397 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/scripts/pyi_multiprocessing_process_start_in_threads.py
+-rwxrwxrwx   0 root         (0) root         (0)     1593 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/scripts/pyi_multiprocessing_queue.py
+-rwxrwxrwx   0 root         (0) root         (0)     1171 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/scripts/pyi_multiprocessing_semaphore.py
+-rwxrwxrwx   0 root         (0) root         (0)     1663 2024-04-04 21:05:01.000000 pyinstaller-6.7.0/tests/functional/scripts/pyi_optimization.py
+-rwxrwxrwx   0 root         (0) root         (0)    11714 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/scripts/pyi_osx_aevent_logger_carbon.py
+-rwxrwxrwx   0 root         (0) root         (0)     1058 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/scripts/pyi_path_encoding.py
+-rwxrwxrwx   0 root         (0) root         (0)    14974 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/scripts/pyi_pkg_resources_provider.py
+-rwxrwxrwx   0 root         (0) root         (0)     1658 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/scripts/pyi_pkgutil_iter_modules.py
+-rwxrwxrwx   0 root         (0) root         (0)      933 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/scripts/pyi_python_home.py
+-rwxrwxrwx   0 root         (0) root         (0)     1868 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/scripts/pyi_site_module_disabled.py
+-rwxrwxrwx   0 root         (0) root         (0)      455 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/scripts/pyi_spec_options.py
+-rwxrwxrwx   0 root         (0) root         (0)     1131 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/scripts/pyi_stderr_encoding.py
+-rwxrwxrwx   0 root         (0) root         (0)     1130 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/scripts/pyi_stdout_encoding.py
+-rwxrwxrwx   0 root         (0) root         (0)     1462 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/scripts/pyi_symlink_basename_is_kept.py
+-rwxrwxrwx   0 root         (0) root         (0)     2958 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/scripts/pyi_symlinks_test.py
+-rwxrwxrwx   0 root         (0) root         (0)     2283 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/scripts/pyi_threading_module2.py
+-rwxrwxrwx   0 root         (0) root         (0)     2232 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/scripts/pyi_unbuffered_output.py
+-rwxrwxrwx   0 root         (0) root         (0)     1697 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/scripts/pyi_win_py3_no_shortpathname.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.857943 pyinstaller-6.7.0/tests/functional/specs/
+-rwxrwxrwx   0 root         (0) root         (0)     1190 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/specs/list_pytest11_entry_point.spec
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.860231 pyinstaller-6.7.0/tests/functional/specs/multipackage-scripts/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.860427 pyinstaller-6.7.0/tests/functional/specs/multipackage-scripts/extra-hooks/
+-rwxrwxrwx   0 root         (0) root         (0)      616 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/specs/multipackage-scripts/extra-hooks/hook-multipackage_test_pkg.py
+-rwxrwxrwx   0 root         (0) root         (0)      576 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/specs/multipackage-scripts/multipackage1_B.py
+-rwxrwxrwx   0 root         (0) root         (0)      576 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/specs/multipackage-scripts/multipackage2_B.py
+-rwxrwxrwx   0 root         (0) root         (0)      576 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/specs/multipackage-scripts/multipackage3_B.py
+-rwxrwxrwx   0 root         (0) root         (0)      576 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/specs/multipackage-scripts/multipackage4_B.py
+-rwxrwxrwx   0 root         (0) root         (0)      576 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/specs/multipackage-scripts/multipackage5_B.py
+-rwxrwxrwx   0 root         (0) root         (0)      576 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/specs/multipackage-scripts/multipackage5_C.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.860733 pyinstaller-6.7.0/tests/functional/specs/multipackage-scripts/multipackage_test_pkg/
+-rwxrwxrwx   0 root         (0) root         (0)     1413 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/specs/multipackage-scripts/multipackage_test_pkg/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.861109 pyinstaller-6.7.0/tests/functional/specs/multipackage-scripts/multipackage_test_pkg/data/
+-rwxrwxrwx   0 root         (0) root         (0)       11 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/specs/multipackage-scripts/multipackage_test_pkg/data/secret.txt
+-rwxrwxrwx   0 root         (0) root         (0)      576 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/specs/multipackage-scripts/test_multipackage1.py
+-rwxrwxrwx   0 root         (0) root         (0)      576 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/specs/multipackage-scripts/test_multipackage2.py
+-rwxrwxrwx   0 root         (0) root         (0)      576 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/specs/multipackage-scripts/test_multipackage3.py
+-rwxrwxrwx   0 root         (0) root         (0)      576 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/specs/multipackage-scripts/test_multipackage4.py
+-rwxrwxrwx   0 root         (0) root         (0)      576 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/specs/multipackage-scripts/test_multipackage5.py
+-rwxrwxrwx   0 root         (0) root         (0)     2415 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/specs/pyi_osx_aevent_handling_carbon.spec
+-rwxrwxrwx   0 root         (0) root         (0)     1613 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/specs/pyi_osx_override_info_plist.spec
+-rwxrwxrwx   0 root         (0) root         (0)     1205 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/specs/pyi_spec_options.spec
+-rwxrwxrwx   0 root         (0) root         (0)     1170 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/specs/pyi_unbuffered_output.spec
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.861859 pyinstaller-6.7.0/tests/functional/specs/several-scripts/
+-rwxrwxrwx   0 root         (0) root         (0)       94 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/specs/several-scripts/basemod.py
+-rwxrwxrwx   0 root         (0) root         (0)      366 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/specs/several-scripts/main-script1.py
+-rwxrwxrwx   0 root         (0) root         (0)      136 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/specs/several-scripts/main-script2.py
+-rwxrwxrwx   0 root         (0) root         (0)      198 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/specs/several-scripts/rt-hook-script.py
+-rwxrwxrwx   0 root         (0) root         (0)     1025 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/specs/several-scripts1.spec
+-rwxrwxrwx   0 root         (0) root         (0)     1003 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/specs/several-scripts2.spec
+-rwxrwxrwx   0 root         (0) root         (0)     1029 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/specs/spec-with-utf8.spec
+-rwxrwxrwx   0 root         (0) root         (0)     2022 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/specs/spec_with_splash.spec
+-rwxrwxrwx   0 root         (0) root         (0)     1583 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/specs/symlink_basename_is_kept.spec
+-rwxrwxrwx   0 root         (0) root         (0)     1699 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/specs/test_multipackage1.spec
+-rwxrwxrwx   0 root         (0) root         (0)     1936 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/specs/test_multipackage2.spec
+-rwxrwxrwx   0 root         (0) root         (0)     1962 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/specs/test_multipackage3.spec
+-rwxrwxrwx   0 root         (0) root         (0)     2170 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/specs/test_multipackage4.spec
+-rwxrwxrwx   0 root         (0) root         (0)     2734 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/specs/test_multipackage5.spec
+-rwxrwxrwx   0 root         (0) root         (0)    15836 2024-03-24 20:46:04.000000 pyinstaller-6.7.0/tests/functional/test_apple_events.py
+-rwxrwxrwx   0 root         (0) root         (0)    31118 2024-02-23 20:40:55.000000 pyinstaller-6.7.0/tests/functional/test_basic.py
+-rwxrwxrwx   0 root         (0) root         (0)     4428 2024-04-04 21:05:01.000000 pyinstaller-6.7.0/tests/functional/test_binary_vs_data_reclassification.py
+-rwxrwxrwx   0 root         (0) root         (0)     1480 2024-01-13 17:57:57.000000 pyinstaller-6.7.0/tests/functional/test_cliutils.py
+-rwxrwxrwx   0 root         (0) root         (0)     1759 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/test_django.py
+-rwxrwxrwx   0 root         (0) root         (0)     1439 2023-11-26 23:20:35.000000 pyinstaller-6.7.0/tests/functional/test_hook_utilities.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.864106 pyinstaller-6.7.0/tests/functional/test_hooks/
+-rwxrwxrwx   0 root         (0) root         (0)     2423 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/test_hooks/test_gi.py
+-rwxrwxrwx   0 root         (0) root         (0)     4748 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/test_hooks/test_matplotlib.py
+-rwxrwxrwx   0 root         (0) root         (0)     4032 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/test_hooks/test_pil.py
+-rwxrwxrwx   0 root         (0) root         (0)      837 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/test_hooks/test_pkg_resources.py
+-rwxrwxrwx   0 root         (0) root         (0)     2107 2023-11-04 13:41:36.000000 pyinstaller-6.7.0/tests/functional/test_hooks/test_scipy.py
+-rwxrwxrwx   0 root         (0) root         (0)     1037 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/test_hooks/test_six.py
+-rwxrwxrwx   0 root         (0) root         (0)    25798 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/test_import.py
+-rwxrwxrwx   0 root         (0) root         (0)     1456 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/test_import_lazy_loader.py
+-rwxrwxrwx   0 root         (0) root         (0)     3321 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/test_import_pep302.py
+-rwxrwxrwx   0 root         (0) root         (0)     7584 2023-11-11 15:22:30.000000 pyinstaller-6.7.0/tests/functional/test_importlib_resources.py
+-rwxrwxrwx   0 root         (0) root         (0)     1979 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/test_interactive.py
+-rwxrwxrwx   0 root         (0) root         (0)    13513 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/test_libraries.py
+-rwxrwxrwx   0 root         (0) root         (0)     1937 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/test_linux_appimage.py
+-rwxrwxrwx   0 root         (0) root         (0)    56164 2023-11-26 23:20:35.000000 pyinstaller-6.7.0/tests/functional/test_macos_bundle_structure.py
+-rwxrwxrwx   0 root         (0) root         (0)    18017 2024-04-04 21:05:01.000000 pyinstaller-6.7.0/tests/functional/test_misc.py
+-rwxrwxrwx   0 root         (0) root         (0)     2015 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/test_module_exclusion.py
+-rwxrwxrwx   0 root         (0) root         (0)      672 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/test_multipackage.py
+-rwxrwxrwx   0 root         (0) root         (0)     4481 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/test_multiprocessing.py
+-rwxrwxrwx   0 root         (0) root         (0)     5519 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/test_path_encodings.py
+-rwxrwxrwx   0 root         (0) root         (0)     2872 2023-11-11 15:22:30.000000 pyinstaller-6.7.0/tests/functional/test_pkg_resources_provider.py
+-rwxrwxrwx   0 root         (0) root         (0)     9562 2024-01-13 17:58:01.000000 pyinstaller-6.7.0/tests/functional/test_pkgutil.py
+-rwxrwxrwx   0 root         (0) root         (0)     3160 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/test_pywin32.py
+-rwxrwxrwx   0 root         (0) root         (0)    25711 2024-05-01 21:08:24.000000 pyinstaller-6.7.0/tests/functional/test_qt.py
+-rwxrwxrwx   0 root         (0) root         (0)     5603 2023-11-04 13:41:36.000000 pyinstaller-6.7.0/tests/functional/test_regression.py
+-rwxrwxrwx   0 root         (0) root         (0)      918 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/test_runtime.py
+-rwxrwxrwx   0 root         (0) root         (0)     3428 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/functional/test_signals.py
+-rwxrwxrwx   0 root         (0) root         (0)    21197 2024-04-04 21:05:01.000000 pyinstaller-6.7.0/tests/functional/test_symlinks.py
+-rwxrwxrwx   0 root         (0) root         (0)     2828 2024-05-21 22:30:39.000000 pyinstaller-6.7.0/tests/functional/test_unbuffered_stdio.py
+-rwxrwxrwx   0 root         (0) root         (0)      709 2024-03-24 20:46:04.000000 pyinstaller-6.7.0/tests/requirements-base.txt
+-rwxrwxrwx   0 root         (0) root         (0)      895 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/requirements-developer.txt
+-rwxrwxrwx   0 root         (0) root         (0)     4374 2024-05-21 22:30:39.000000 pyinstaller-6.7.0/tests/requirements-libraries.txt
+-rwxrwxrwx   0 root         (0) root         (0)      844 2024-01-13 17:58:01.000000 pyinstaller-6.7.0/tests/requirements-tools.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.866710 pyinstaller-6.7.0/tests/scripts/
+-rwxrwxrwx   0 root         (0) root         (0)      947 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/scripts/Dockerfile
+-rwxrwxrwx   0 root         (0) root         (0)       66 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/scripts/README
+-rwxrwxrwx   0 root         (0) root         (0)     2573 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/scripts/check-pefile-arch.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.869062 pyinstaller-6.7.0/tests/scripts/eggs4testing/
+-rwxrwxrwx   0 root         (0) root         (0)      119 2023-09-30 18:27:19.000000 pyinstaller-6.7.0/tests/scripts/eggs4testing/.gitignore
+-rwxrwxrwx   0 root         (0) root         (0)      240 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/scripts/eggs4testing/README.txt
+-rwxrwxrwx   0 root         (0) root         (0)     4204 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/scripts/eggs4testing/build-nspkg-tests.py
+-rwxrwxrwx   0 root         (0) root         (0)     3258 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/scripts/eggs4testing/make.sh
+-rwxrwxrwx   0 root         (0) root         (0)      829 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/scripts/eggs4testing/setup-unzipped.py
+-rwxrwxrwx   0 root         (0) root         (0)      801 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/scripts/eggs4testing/setup-zipped.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.869507 pyinstaller-6.7.0/tests/scripts/eggs4testing/unzipped_egg/
+-rwxrwxrwx   0 root         (0) root         (0)      678 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/scripts/eggs4testing/unzipped_egg/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.869886 pyinstaller-6.7.0/tests/scripts/eggs4testing/unzipped_egg/data/
+-rwxrwxrwx   0 root         (0) root         (0)       34 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/scripts/eggs4testing/unzipped_egg/data/datafile.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.870129 pyinstaller-6.7.0/tests/scripts/eggs4testing/zipped_egg/
+-rwxrwxrwx   0 root         (0) root         (0)      678 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/scripts/eggs4testing/zipped_egg/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.870663 pyinstaller-6.7.0/tests/scripts/eggs4testing/zipped_egg/data/
+-rwxrwxrwx   0 root         (0) root         (0)       32 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/scripts/eggs4testing/zipped_egg/data/datafile.txt
+-rwxrwxrwx   0 root         (0) root         (0)       77 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/scripts/printShortLongCWD.cmd
+-rwxrwxrwx   0 root         (0) root         (0)     1190 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/scripts/test-cliutils.sh
+-rwxrwxrwx   0 root         (0) root         (0)     1300 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/scripts/test-docker.sh
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.870900 pyinstaller-6.7.0/tests/speed/
+-rwxrwxrwx   0 root         (0) root         (0)     1705 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/speed/speed_pefile.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.881663 pyinstaller-6.7.0/tests/unit/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.883710 pyinstaller-6.7.0/tests/unit/Tree_files/
+-rwxrwxrwx   0 root         (0) root         (0)        3 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/Tree_files/dynamiclib.dll
+-rwxrwxrwx   0 root         (0) root         (0)        3 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/Tree_files/dynamiclib.dylib
+-rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/Tree_files/init__.py
+-rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/Tree_files/nine.dat
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.884159 pyinstaller-6.7.0/tests/unit/Tree_files/py_files_not_in_package/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.884380 pyinstaller-6.7.0/tests/unit/Tree_files/py_files_not_in_package/data/
+-rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/Tree_files/py_files_not_in_package/data/eleven.dat
+-rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/Tree_files/py_files_not_in_package/one.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.884824 pyinstaller-6.7.0/tests/unit/Tree_files/py_files_not_in_package/sub_pkg/
+-rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/Tree_files/py_files_not_in_package/sub_pkg/init__.py
+-rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/Tree_files/py_files_not_in_package/sub_pkg/three.py
+-rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/Tree_files/py_files_not_in_package/ten.dat
+-rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/Tree_files/pyextension.pyd
+-rwxrwxrwx   0 root         (0) root         (0)        3 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/Tree_files/pyextension.so
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.885518 pyinstaller-6.7.0/tests/unit/Tree_files/subpkg/
+-rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/Tree_files/subpkg/init__.py
+-rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/Tree_files/subpkg/thirteen.txt
+-rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/Tree_files/subpkg/twelve.py
+-rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/Tree_files/two.py
+-rwxrwxrwx   0 root         (0) root         (0)      791 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/conftest.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.886126 pyinstaller-6.7.0/tests/unit/hook_order_hooks/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/hook_order_hooks/MANIFEST.in
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.886740 pyinstaller-6.7.0/tests/unit/hook_order_hooks/pyi_example_package/
+-rwxrwxrwx   0 root         (0) root         (0)       89 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/hook_order_hooks/pyi_example_package/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       46 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/hook_order_hooks/pyi_example_package/hook-pyi_example_package.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.886964 pyinstaller-6.7.0/tests/unit/hook_order_hooks/pyi_example_package/rthooks/
+-rwxrwxrwx   0 root         (0) root         (0)       46 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/hook_order_hooks/pyi_example_package/rthooks/pyi_rth_naughty.py
+-rwxrwxrwx   0 root         (0) root         (0)       53 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/hook_order_hooks/pyi_example_package/rthooks.dat
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.887174 pyinstaller-6.7.0/tests/unit/hook_order_hooks/rthooks/
+-rwxrwxrwx   0 root         (0) root         (0)      507 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/hook_order_hooks/rthooks/pyi_rth_good.py
+-rwxrwxrwx   0 root         (0) root         (0)       50 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/hook_order_hooks/rthooks.dat
+-rwxrwxrwx   0 root         (0) root         (0)      286 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/hook_order_hooks/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.887385 pyinstaller-6.7.0/tests/unit/hookutils_files/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.889253 pyinstaller-6.7.0/tests/unit/hookutils_files/hookutils_package/
+-rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/hookutils_files/hookutils_package/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)        3 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/hookutils_files/hookutils_package/dynamiclib.dll
+-rwxrwxrwx   0 root         (0) root         (0)        3 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/hookutils_files/hookutils_package/dynamiclib.dylib
+-rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/hookutils_files/hookutils_package/nine.dat
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.889732 pyinstaller-6.7.0/tests/unit/hookutils_files/hookutils_package/py_files_not_in_package/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.889973 pyinstaller-6.7.0/tests/unit/hookutils_files/hookutils_package/py_files_not_in_package/data/
+-rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/hookutils_files/hookutils_package/py_files_not_in_package/data/eleven.dat
+-rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/hookutils_files/hookutils_package/py_files_not_in_package/one.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.890407 pyinstaller-6.7.0/tests/unit/hookutils_files/hookutils_package/py_files_not_in_package/sub_pkg/
+-rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/hookutils_files/hookutils_package/py_files_not_in_package/sub_pkg/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/hookutils_files/hookutils_package/py_files_not_in_package/sub_pkg/three.py
+-rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/hookutils_files/hookutils_package/py_files_not_in_package/ten.dat
+-rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/hookutils_files/hookutils_package/pyextension.pyd
+-rwxrwxrwx   0 root         (0) root         (0)        3 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/hookutils_files/hookutils_package/pyextension.so
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.890815 pyinstaller-6.7.0/tests/unit/hookutils_files/hookutils_package/raises_error_on_import_1/
+-rwxrwxrwx   0 root         (0) root         (0)       34 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/hookutils_files/hookutils_package/raises_error_on_import_1/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/hookutils_files/hookutils_package/raises_error_on_import_1/foo.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.891196 pyinstaller-6.7.0/tests/unit/hookutils_files/hookutils_package/raises_error_on_import_2/
+-rwxrwxrwx   0 root         (0) root         (0)       34 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/hookutils_files/hookutils_package/raises_error_on_import_2/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/hookutils_files/hookutils_package/raises_error_on_import_2/foo.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.891886 pyinstaller-6.7.0/tests/unit/hookutils_files/hookutils_package/subpkg/
+-rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/hookutils_files/hookutils_package/subpkg/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/hookutils_files/hookutils_package/subpkg/thirteen.txt
+-rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/hookutils_files/hookutils_package/subpkg/twelve.py
+-rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/hookutils_files/hookutils_package/two.py
+-rwxrwxrwx   0 root         (0) root         (0)      939 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/hookutils_files/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.530278 pyinstaller-6.7.0/tests/unit/hookutils_files2/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.892149 pyinstaller-6.7.0/tests/unit/hookutils_files2/foo/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/hookutils_files2/foo/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.892346 pyinstaller-6.7.0/tests/unit/hookutils_files2/foo/bar/
+-rwxrwxrwx   0 root         (0) root         (0)       50 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/hookutils_files2/foo/bar/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     9513 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_TOC.py
+-rwxrwxrwx   0 root         (0) root         (0)     2664 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_Tree.py
+-rwxrwxrwx   0 root         (0) root         (0)     1115 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_additionalfilescache.py
+-rwxrwxrwx   0 root         (0) root         (0)      991 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_bindepend.py
+-rwxrwxrwx   0 root         (0) root         (0)     5305 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_building_utils.py
+-rwxrwxrwx   0 root         (0) root         (0)     6668 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_bytecode.py
+-rwxrwxrwx   0 root         (0) root         (0)     2142 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_compat.py
+-rwxrwxrwx   0 root         (0) root         (0)     4211 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_depend_utils.py
+-rwxrwxrwx   0 root         (0) root         (0)     1189 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_hook_order.py
+-rwxrwxrwx   0 root         (0) root         (0)    15548 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_hookutils.py
+-rwxrwxrwx   0 root         (0) root         (0)      772 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_hookutils_gi.py
+-rwxrwxrwx   0 root         (0) root         (0)    10804 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_isolation.py
+-rwxrwxrwx   0 root         (0) root         (0)     3189 2024-01-13 17:57:57.000000 pyinstaller-6.7.0/tests/unit/test_makespec.py
+-rwxrwxrwx   0 root         (0) root         (0)     8414 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_miscutils.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.899079 pyinstaller-6.7.0/tests/unit/test_modulegraph/
+-rwxrwxrwx   0 root         (0) root         (0)       26 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1312 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/test_basic.py
+-rwxrwxrwx   0 root         (0) root         (0)     2267 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/test_compiled_modules.py
+-rwxrwxrwx   0 root         (0) root         (0)    23244 2023-11-26 23:20:35.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/test_edge_data.py
+-rwxrwxrwx   0 root         (0) root         (0)     2892 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/test_implies.py
+-rwxrwxrwx   0 root         (0) root         (0)     2979 2023-11-26 23:20:35.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/test_import_from_init.py
+-rwxrwxrwx   0 root         (0) root         (0)    20640 2023-11-26 23:20:35.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/test_imports.py
+-rwxrwxrwx   0 root         (0) root         (0)    30291 2023-11-26 23:20:35.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/test_modulegraph.py
+-rwxrwxrwx   0 root         (0) root         (0)     4134 2023-11-26 23:20:35.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/test_pep420_nspkg.py
+-rwxrwxrwx   0 root         (0) root         (0)     1325 2023-11-26 23:20:35.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/test_pycompat_pkg.py
+-rwxrwxrwx   0 root         (0) root         (0)     1351 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/test_relimport2.py
+-rwxrwxrwx   0 root         (0) root         (0)     3675 2023-11-26 23:20:35.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/test_setuptools_nspkg.py
+-rwxrwxrwx   0 root         (0) root         (0)     1538 2023-11-26 23:20:35.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/test_swig.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.901322 pyinstaller-6.7.0/tests/unit/test_modulegraph/testdata/
+-rwxrwxrwx   0 root         (0) root         (0)       58 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testdata/script
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.901803 pyinstaller-6.7.0/tests/unit/test_modulegraph/testdata/subdir/
+-rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testdata/subdir/file1.txt
+-rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testdata/subdir/file2.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.902772 pyinstaller-6.7.0/tests/unit/test_modulegraph/testdata/syspath/
+-rwxrwxrwx   0 root         (0) root         (0)       23 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testdata/syspath/myext.pyd
+-rwxrwxrwx   0 root         (0) root         (0)       23 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testdata/syspath/myext.so
+-rwxrwxrwx   0 root         (0) root         (0)       20 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testdata/syspath/mymodule.py
+-rwxrwxrwx   0 root         (0) root         (0)       20 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testdata/syspath/mymodule2.pyc
+-rwxrwxrwx   0 root         (0) root         (0)       21 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testdata/syspath/mymodule3.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.902971 pyinstaller-6.7.0/tests/unit/test_modulegraph/testdata/syspath/mypkg/
+-rwxrwxrwx   0 root         (0) root         (0)       21 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testdata/syspath/mypkg/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     2065 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testdata/syspath.egg
+-rwxrwxrwx   0 root         (0) root         (0)     1825 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testdata/syspath.zip
+-rwxrwxrwx   0 root         (0) root         (0)      760 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testdata/test.egg
+-rwxrwxrwx   0 root         (0) root         (0)       17 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testdata/test.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.530587 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-compatmodule/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.903691 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-compatmodule/pkg/
+-rwxrwxrwx   0 root         (0) root         (0)       12 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-compatmodule/pkg/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      113 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-compatmodule/pkg/api.py
+-rwxrwxrwx   0 root         (0) root         (0)      149 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-compatmodule/pkg/api2.py
+-rwxrwxrwx   0 root         (0) root         (0)      171 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-compatmodule/pkg/api3.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.530689 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-compiled/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.903866 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-compiled/compiled/
+-rwxrwxrwx   0 root         (0) root         (0)       18 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-compiled/compiled/script.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.904502 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-compiled/source/
+-rwxrwxrwx   0 root         (0) root         (0)       33 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-compiled/source/mod1.py
+-rwxrwxrwx   0 root         (0) root         (0)       66 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-compiled/source/mod2.py
+-rwxrwxrwx   0 root         (0) root         (0)       31 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-compiled/source/mod3.py
+-rwxrwxrwx   0 root         (0) root         (0)       41 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-compiled/source/mod4.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.908014 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-edgedata/
+-rwxrwxrwx   0 root         (0) root         (0)       15 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-edgedata/function_class_existing.py
+-rwxrwxrwx   0 root         (0) root         (0)       15 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-edgedata/function_conditional_existing.py
+-rwxrwxrwx   0 root         (0) root         (0)       15 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-edgedata/function_conditional_import2_existing.py
+-rwxrwxrwx   0 root         (0) root         (0)       15 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-edgedata/function_conditional_import_existing.py
+-rwxrwxrwx   0 root         (0) root         (0)       15 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-edgedata/function_existing.py
+-rwxrwxrwx   0 root         (0) root         (0)       15 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-edgedata/function_import2_existing.py
+-rwxrwxrwx   0 root         (0) root         (0)       15 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-edgedata/function_import_existing.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.910769 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-edgedata/pkg/
+-rwxrwxrwx   0 root         (0) root         (0)       21 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-edgedata/pkg/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       15 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-edgedata/pkg/function_class_existing.py
+-rwxrwxrwx   0 root         (0) root         (0)       15 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-edgedata/pkg/function_conditional_existing.py
+-rwxrwxrwx   0 root         (0) root         (0)       15 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-edgedata/pkg/function_conditional_import2_existing.py
+-rwxrwxrwx   0 root         (0) root         (0)       15 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-edgedata/pkg/function_conditional_import_existing.py
+-rwxrwxrwx   0 root         (0) root         (0)       15 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-edgedata/pkg/function_existing.py
+-rwxrwxrwx   0 root         (0) root         (0)       15 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-edgedata/pkg/function_import2_existing.py
+-rwxrwxrwx   0 root         (0) root         (0)       15 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-edgedata/pkg/function_import_existing.py
+-rwxrwxrwx   0 root         (0) root         (0)       15 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-edgedata/pkg/toplevel_class_existing.py
+-rwxrwxrwx   0 root         (0) root         (0)       15 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-edgedata/pkg/toplevel_conditional_existing.py
+-rwxrwxrwx   0 root         (0) root         (0)       15 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-edgedata/pkg/toplevel_conditional_import2_existing.py
+-rwxrwxrwx   0 root         (0) root         (0)       15 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-edgedata/pkg/toplevel_conditional_import_existing.py
+-rwxrwxrwx   0 root         (0) root         (0)       15 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-edgedata/pkg/toplevel_existing.py
+-rwxrwxrwx   0 root         (0) root         (0)       15 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-edgedata/pkg/toplevel_import2_existing.py
+-rwxrwxrwx   0 root         (0) root         (0)       15 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-edgedata/pkg/toplevel_import_existing.py
+-rwxrwxrwx   0 root         (0) root         (0)     1384 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-edgedata/script.py
+-rwxrwxrwx   0 root         (0) root         (0)     1551 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-edgedata/script_from_import.py
+-rwxrwxrwx   0 root         (0) root         (0)      265 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-edgedata/script_multi_import.py
+-rwxrwxrwx   0 root         (0) root         (0)       15 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-edgedata/toplevel_class_existing.py
+-rwxrwxrwx   0 root         (0) root         (0)       15 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-edgedata/toplevel_conditional_existing.py
+-rwxrwxrwx   0 root         (0) root         (0)       15 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-edgedata/toplevel_conditional_import2_existing.py
+-rwxrwxrwx   0 root         (0) root         (0)       15 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-edgedata/toplevel_conditional_import_existing.py
+-rwxrwxrwx   0 root         (0) root         (0)       15 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-edgedata/toplevel_existing.py
+-rwxrwxrwx   0 root         (0) root         (0)       15 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-edgedata/toplevel_import2_existing.py
+-rwxrwxrwx   0 root         (0) root         (0)       15 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-edgedata/toplevel_import_existing.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.910950 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-import-from-init/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.911116 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-import-from-init/pkg/
+-rwxrwxrwx   0 root         (0) root         (0)       12 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-import-from-init/pkg/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.911648 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-import-from-init/pkg/subpkg/
+-rwxrwxrwx   0 root         (0) root         (0)       75 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-import-from-init/pkg/subpkg/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       49 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-import-from-init/pkg/subpkg/_collections.py
+-rwxrwxrwx   0 root         (0) root         (0)       39 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-import-from-init/pkg/subpkg/compat.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.911842 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-import-from-init/pkg2/
+-rwxrwxrwx   0 root         (0) root         (0)       22 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-import-from-init/pkg2/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.912388 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-import-from-init/pkg2/subpkg/
+-rwxrwxrwx   0 root         (0) root         (0)       78 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-import-from-init/pkg2/subpkg/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       50 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-import-from-init/pkg2/subpkg/_collections.py
+-rwxrwxrwx   0 root         (0) root         (0)       40 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-import-from-init/pkg2/subpkg/compat.py
+-rwxrwxrwx   0 root         (0) root         (0)       37 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-import-from-init/script.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.912579 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-packages/
+-rwxrwxrwx   0 root         (0) root         (0)       11 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-packages/main_script.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.912948 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-packages/pkg/
+-rwxrwxrwx   0 root         (0) root         (0)       17 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-packages/pkg/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.913315 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-packages/pkg/sub1/
+-rwxrwxrwx   0 root         (0) root         (0)       22 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-packages/pkg/sub1/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       22 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-packages/pkg/sub1/modA.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.913658 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-packages/pkg/sub2/
+-rwxrwxrwx   0 root         (0) root         (0)       22 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-packages/pkg/sub2/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       21 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-packages/pkg/sub2/mod.py
+-rwxrwxrwx   0 root         (0) root         (0)       17 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-packages/pkg/sub3.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.531264 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-pep420-namespace/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.531220 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-pep420-namespace/path1/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.913838 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-pep420-namespace/path1/package/
+-rwxrwxrwx   0 root         (0) root         (0)       21 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-pep420-namespace/path1/package/sub2.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.531286 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-pep420-namespace/path2/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.914014 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-pep420-namespace/path2/package/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.914182 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-pep420-namespace/path2/package/nspkg/
+-rwxrwxrwx   0 root         (0) root         (0)       26 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-pep420-namespace/path2/package/nspkg/mod.py
+-rwxrwxrwx   0 root         (0) root         (0)       21 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-pep420-namespace/path2/package/sub1.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.914515 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-pep420-namespace/path2/package/subpackage/
+-rwxrwxrwx   0 root         (0) root         (0)       27 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-pep420-namespace/path2/package/subpackage/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       31 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-pep420-namespace/path2/package/subpackage/sub.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.914708 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-regr1/
+-rwxrwxrwx   0 root         (0) root         (0)       18 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-regr1/main_script.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.915264 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-regr1/pkg/
+-rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-regr1/pkg/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       16 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-regr1/pkg/a.py
+-rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-regr1/pkg/b.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.915454 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-regr2/
+-rwxrwxrwx   0 root         (0) root         (0)       11 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-regr2/main_script.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.915967 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-regr2/pkg/
+-rwxrwxrwx   0 root         (0) root         (0)      153 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-regr2/pkg/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       21 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-regr2/pkg/base.py
+-rwxrwxrwx   0 root         (0) root         (0)       15 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-regr2/pkg/pkg.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.916134 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-regr3/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.916298 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-regr3/mypkg/
+-rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-regr3/mypkg/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.916618 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-regr3/mypkg/json/
+-rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-regr3/mypkg/json/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       68 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-regr3/mypkg/json/encoder.py
+-rwxrwxrwx   0 root         (0) root         (0)       31 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-regr3/script.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.916795 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-regr4/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.916967 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-regr4/pkg/
+-rwxrwxrwx   0 root         (0) root         (0)       21 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-regr4/pkg/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.917613 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-regr4/pkg/core/
+-rwxrwxrwx   0 root         (0) root         (0)       26 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-regr4/pkg/core/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       99 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-regr4/pkg/core/callables.py
+-rwxrwxrwx   0 root         (0) root         (0)      160 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-regr4/pkg/core/listener.py
+-rwxrwxrwx   0 root         (0) root         (0)       84 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-regr4/pkg/core/listenerimpl.py
+-rwxrwxrwx   0 root         (0) root         (0)       49 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-regr4/script.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.917779 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-regr7/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.918134 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-regr7/pkg/
+-rwxrwxrwx   0 root         (0) root         (0)       16 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-regr7/pkg/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       65 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-regr7/pkg/mod.py
+-rwxrwxrwx   0 root         (0) root         (0)       20 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-regr7/script.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.918513 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-regr8/
+-rwxrwxrwx   0 root         (0) root         (0)       30 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-regr8/mod.py
+-rwxrwxrwx   0 root         (0) root         (0)       11 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-regr8/script.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.918882 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-relimport/
+-rwxrwxrwx   0 root         (0) root         (0)       24 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-relimport/mod.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.919887 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-relimport/pkg/
+-rwxrwxrwx   0 root         (0) root         (0)       18 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-relimport/pkg/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       25 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-relimport/pkg/mod.py
+-rwxrwxrwx   0 root         (0) root         (0)       11 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-relimport/pkg/oldstyle.py
+-rwxrwxrwx   0 root         (0) root         (0)       57 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-relimport/pkg/relative.py
+-rwxrwxrwx   0 root         (0) root         (0)       22 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-relimport/pkg/relimport.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.920232 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-relimport/pkg/sub2/
+-rwxrwxrwx   0 root         (0) root         (0)       17 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-relimport/pkg/sub2/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       21 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-relimport/pkg/sub2/mod.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.920918 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-relimport/pkg/subpkg/
+-rwxrwxrwx   0 root         (0) root         (0)       19 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-relimport/pkg/subpkg/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      117 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-relimport/pkg/subpkg/mod2.py
+-rwxrwxrwx   0 root         (0) root         (0)       86 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-relimport/pkg/subpkg/relative.py
+-rwxrwxrwx   0 root         (0) root         (0)      106 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-relimport/pkg/subpkg/relative2.py
+-rwxrwxrwx   0 root         (0) root         (0)       50 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-relimport/pkg/toplevel.py
+-rwxrwxrwx   0 root         (0) root         (0)      175 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-relimport/script.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.921115 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-relimport2/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.921870 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-relimport2/pkg/
+-rwxrwxrwx   0 root         (0) root         (0)       39 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-relimport2/pkg/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       13 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-relimport2/pkg/mod1.py
+-rwxrwxrwx   0 root         (0) root         (0)       13 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-relimport2/pkg/mod2.py
+-rwxrwxrwx   0 root         (0) root         (0)       13 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-relimport2/pkg/mod3.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.922060 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-relimport2/pkg/sub/
+-rwxrwxrwx   0 root         (0) root         (0)       65 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-relimport2/pkg/sub/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       17 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-relimport2/toplevel.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.922250 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-setuptools-namespace/
+-rwxrwxrwx   0 root         (0) root         (0)      221 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-setuptools-namespace/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.533448 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-setuptools-namespace/src/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.922613 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-setuptools-namespace/src/nspkg/
+-rwxrwxrwx   0 root         (0) root         (0)      200 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-setuptools-namespace/src/nspkg/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       21 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-setuptools-namespace/src/nspkg/module.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.923949 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-setuptools-namespace/src/nspkg/nssubpkg/
+-rwxrwxrwx   0 root         (0) root         (0)      200 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-setuptools-namespace/src/nspkg/nssubpkg/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       26 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-setuptools-namespace/src/nspkg/nssubpkg/sub.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.923614 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-setuptools-namespace/src/nspkg.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)      177 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-setuptools-namespace/src/nspkg.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      313 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-setuptools-namespace/src/nspkg.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-setuptools-namespace/src/nspkg.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       21 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-setuptools-namespace/src/nspkg.egg-info/namespace_packages.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-setuptools-namespace/src/nspkg.egg-info/not-zip-safe
+-rwxrwxrwx   0 root         (0) root         (0)        6 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-setuptools-namespace/src/nspkg.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.533562 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-swig/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:38:37.924605 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-swig/pkg/
+-rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-swig/pkg/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)        2 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-swig/pkg/_sample.py
+-rwxrwxrwx   0 root         (0) root         (0)       21 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-swig/pkg/sample.i
+-rwxrwxrwx   0 root         (0) root         (0)     1974 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-swig/pkg/sample.py
+-rwxrwxrwx   0 root         (0) root         (0)    25812 2023-11-26 23:20:35.000000 pyinstaller-6.7.0/tests/unit/test_modulegraph_more.py
+-rwxrwxrwx   0 root         (0) root         (0)     3052 2023-11-26 23:20:35.000000 pyinstaller-6.7.0/tests/unit/test_normalize_icon_type.py
+-rwxrwxrwx   0 root         (0) root         (0)     8742 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_pyimodulegraph.py
+-rwxrwxrwx   0 root         (0) root         (0)     3075 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_recursion_limit.py
+-rwxrwxrwx   0 root         (0) root         (0)     1278 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_systemexit.py
+-rwxrwxrwx   0 root         (0) root         (0)     7495 2024-04-04 21:05:01.000000 pyinstaller-6.7.0/tests/unit/test_toc_normalization.py
+-rwxrwxrwx   0 root         (0) root         (0)    22223 2023-09-30 18:27:26.000000 pyinstaller-6.7.0/tests/unit/test_winmanifest.py
```

### Comparing `pyinstaller-6.6.0/.gitattributes` & `pyinstaller-6.7.0/.gitattributes`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/.github/ISSUE_TEMPLATE/antivirus.md` & `pyinstaller-6.7.0/.github/ISSUE_TEMPLATE/antivirus.md`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/.github/ISSUE_TEMPLATE/bug_report.md` & `pyinstaller-6.7.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/.github/ISSUE_TEMPLATE/feature_request.md` & `pyinstaller-6.7.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/.github/workflows/ci.yml` & `pyinstaller-6.7.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/.github/workflows/lint.yml` & `pyinstaller-6.7.0/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/.github/workflows/wheel-builder.yml` & `pyinstaller-6.7.0/.github/workflows/wheel-builder.yml`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/.gitignore` & `pyinstaller-6.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/.pylintrc` & `pyinstaller-6.7.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/.yapfignore` & `pyinstaller-6.7.0/.yapfignore`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/COPYING.txt` & `pyinstaller-6.7.0/COPYING.txt`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/MANIFEST.in` & `pyinstaller-6.7.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PKG-INFO` & `pyinstaller-6.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyinstaller
-Version: 6.6.0
+Version: 6.7.0
 Summary: PyInstaller bundles a Python application and all its dependencies into a single package.
 Home-page: https://www.pyinstaller.org/
 Author: Hartmut Goebel, Giovanni Bajo, David Vierra, David Cortesi, Martin Zibricky
 License: GPLv2-or-later with a special exception which allows to use PyInstaller to build and distribute non-free programs (including commercial ones)
 Project-URL: Source, https://github.com/pyinstaller/pyinstaller
 Keywords: packaging, app, apps, bundle, convert, standalone, executable,pyinstaller, cxfreeze, freeze, py2exe, py2app, bbfreeze
 Classifier: Development Status :: 6 - Mature
@@ -42,15 +42,15 @@
 Description-Content-Type: text/x-rst
 License-File: COPYING.txt
 Requires-Dist: setuptools>=42.0.0
 Requires-Dist: altgraph
 Requires-Dist: pefile>=2022.5.30; sys_platform == "win32"
 Requires-Dist: pywin32-ctypes>=0.2.1; sys_platform == "win32"
 Requires-Dist: macholib>=1.8; sys_platform == "darwin"
-Requires-Dist: pyinstaller-hooks-contrib>=2024.3
+Requires-Dist: pyinstaller-hooks-contrib>=2024.6
 Requires-Dist: importlib_metadata>=4.6; python_version < "3.10"
 Requires-Dist: packaging>=22.0
 Provides-Extra: hook-testing
 Requires-Dist: pytest>=2.7.3; extra == "hook-testing"
 Requires-Dist: execnet>=1.5.0; extra == "hook-testing"
 Requires-Dist: psutil; extra == "hook-testing"
 Provides-Extra: completion
@@ -188,21 +188,21 @@
 pyinstaller`` provided that you have an appropriate C compiler (typically
 either ``gcc`` or ``clang``) and zlib's development headers already installed.
 
 
 Support
 -------
 
-- Official debugging guide: https://pyinstaller.org/en/v6.6.0/when-things-go-wrong.html
+- Official debugging guide: https://pyinstaller.org/en/v6.7.0/when-things-go-wrong.html
 - Assorted user contributed help topics: https://github.com/pyinstaller/pyinstaller/wiki
 - Web based Q&A forums: https://github.com/pyinstaller/pyinstaller/discussions
 - Email based Q&A forums: https://groups.google.com/g/pyinstaller
 
 
 Changes in this Release
 -----------------------
 
 You can find a detailed list of changes in this release
 in the `Changelog`_ section of the manual.
 
-.. _`manual`: https://pyinstaller.org/en/v6.6.0/
-.. _`Changelog`: https://pyinstaller.org/en/v6.6.0/CHANGES.html
+.. _`manual`: https://pyinstaller.org/en/v6.7.0/
+.. _`Changelog`: https://pyinstaller.org/en/v6.7.0/CHANGES.html
```

### Comparing `pyinstaller-6.6.0/PyInstaller/__init__.py` & `pyinstaller-6.7.0/PyInstaller/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import os
 import sys
 
 from PyInstaller import compat
 from PyInstaller.utils.git import get_repo_revision
 
 # Note: Keep this variable as plain string so it could be updated automatically when doing a release.
-__version__ = '6.6.0'
+__version__ = '6.7.0'
 
 # Absolute path of this package's directory. Save this early so all submodules can use the absolute path. This is
 # required for example if the current directory changes prior to loading the hooks.
 PACKAGEPATH = os.path.abspath(os.path.dirname(__file__))
 
 HOMEPATH = os.path.dirname(PACKAGEPATH)
```

### Comparing `pyinstaller-6.6.0/PyInstaller/__main__.py` & `pyinstaller-6.7.0/PyInstaller/__main__.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/_recursion_too_deep_message.py` & `pyinstaller-6.7.0/PyInstaller/_recursion_too_deep_message.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/_shared_with_waf.py` & `pyinstaller-6.7.0/PyInstaller/_shared_with_waf.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/archive/pyz_crypto.py` & `pyinstaller-6.7.0/PyInstaller/archive/pyz_crypto.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/archive/readers.py` & `pyinstaller-6.7.0/PyInstaller/archive/readers.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/archive/writers.py` & `pyinstaller-6.7.0/PyInstaller/archive/writers.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/bootloader/Darwin-64bit/run` & `pyinstaller-6.7.0/PyInstaller/bootloader/Darwin-64bit/run`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/bootloader/Darwin-64bit/run_d` & `pyinstaller-6.7.0/PyInstaller/bootloader/Darwin-64bit/run_d`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/bootloader/Darwin-64bit/runw` & `pyinstaller-6.7.0/PyInstaller/bootloader/Darwin-64bit/runw`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/bootloader/Darwin-64bit/runw_d` & `pyinstaller-6.7.0/PyInstaller/bootloader/Darwin-64bit/runw_d`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/bootloader/Windows-32bit-intel/run.exe` & `pyinstaller-6.7.0/PyInstaller/bootloader/Windows-32bit-intel/run.exe`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/bootloader/Windows-32bit-intel/run_d.exe` & `pyinstaller-6.7.0/PyInstaller/bootloader/Windows-32bit-intel/run_d.exe`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/bootloader/Windows-32bit-intel/runw.exe` & `pyinstaller-6.7.0/PyInstaller/bootloader/Windows-32bit-intel/runw.exe`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/bootloader/Windows-32bit-intel/runw_d.exe` & `pyinstaller-6.7.0/PyInstaller/bootloader/Windows-32bit-intel/runw_d.exe`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/bootloader/Windows-64bit-intel/run.exe` & `pyinstaller-6.7.0/PyInstaller/bootloader/Windows-64bit-intel/run.exe`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/bootloader/Windows-64bit-intel/run_d.exe` & `pyinstaller-6.7.0/PyInstaller/bootloader/Windows-64bit-intel/run_d.exe`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/bootloader/Windows-64bit-intel/runw.exe` & `pyinstaller-6.7.0/PyInstaller/bootloader/Windows-64bit-intel/runw.exe`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/bootloader/Windows-64bit-intel/runw_d.exe` & `pyinstaller-6.7.0/PyInstaller/bootloader/Windows-64bit-intel/runw_d.exe`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/bootloader/images/icon-console.icns` & `pyinstaller-6.7.0/PyInstaller/bootloader/images/icon-console.icns`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/bootloader/images/icon-console.ico` & `pyinstaller-6.7.0/PyInstaller/bootloader/images/icon-console.ico`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/bootloader/images/icon-windowed.icns` & `pyinstaller-6.7.0/PyInstaller/bootloader/images/icon-windowed.icns`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/bootloader/images/icon-windowed.ico` & `pyinstaller-6.7.0/PyInstaller/bootloader/images/icon-windowed.ico`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/building/api.py` & `pyinstaller-6.7.0/PyInstaller/building/api.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/building/build_main.py` & `pyinstaller-6.7.0/PyInstaller/building/build_main.py`

 * *Files 1% similar despite different names*

```diff
@@ -465,18 +465,20 @@
 
         self.hiddenimports = hiddenimports or []
         # Include hidden imports passed via CONF['hiddenimports']; these might be populated if user has a wrapper script
         # that calls `build_main.main()` with custom `pyi_config` dictionary that contains `hiddenimports`.
         self.hiddenimports.extend(CONF.get('hiddenimports', []))
 
         self.hookspath = []
-        # Append directories in `hookspath` (`--additional-hooks-dir`) to take precedence over those from the entry
-        # points.
+        # Prepend directories in `hookspath` (`--additional-hooks-dir`) to take precedence over those from the entry
+        # points. Expand starting tilde into user's home directory, as a work-around for tilde not being expanded by
+        # shell when using ˙--additional-hooks-dir=~/path/abc` instead of ˙--additional-hooks-dir ~/path/abc` (or when
+        # the path argument is quoted).
         if hookspath:
-            self.hookspath.extend(hookspath)
+            self.hookspath.extend([os.path.expanduser(path) for path in hookspath])
 
         # Add hook directories from PyInstaller entry points.
         self.hookspath += discover_hook_directories()
 
         self.hooksconfig = {}
         if hooksconfig:
             self.hooksconfig.update(hooksconfig)
@@ -1040,20 +1042,21 @@
 
 def build(spec, distpath, workpath, clean_build):
     """
     Build the executable according to the created SPEC file.
     """
     from PyInstaller.config import CONF
 
-    # Ensure starting tilde and environment variables get expanded in distpath / workpath.
-    # '~/path/abc', '${env_var_name}/path/abc/def'
-    distpath = os.path.abspath(compat.expand_path(distpath))
-    workpath = os.path.abspath(compat.expand_path(workpath))
-    CONF['spec'] = os.path.abspath(compat.expand_path(spec))
+    # Ensure starting tilde in distpath / workpath is expanded into user's home directory. This is to work around for
+    # tilde not being expanded when using ˙--workpath=~/path/abc` instead of ˙--workpath ~/path/abc` (or when the path
+    # argument is quoted). See https://github.com/pyinstaller/pyinstaller/issues/696
+    distpath = os.path.abspath(os.path.expanduser(distpath))
+    workpath = os.path.abspath(os.path.expanduser(workpath))
 
+    CONF['spec'] = os.path.abspath(spec)
     CONF['specpath'], CONF['specnm'] = os.path.split(CONF['spec'])
     CONF['specnm'] = os.path.splitext(CONF['specnm'])[0]
 
     # Add 'specname' to workpath and distpath if they point to PyInstaller homepath.
     if os.path.dirname(distpath) == HOMEPATH:
         distpath = os.path.join(HOMEPATH, CONF['specnm'], os.path.basename(distpath))
     CONF['distpath'] = distpath
```

### Comparing `pyinstaller-6.6.0/PyInstaller/building/datastruct.py` & `pyinstaller-6.7.0/PyInstaller/building/datastruct.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/building/icon.py` & `pyinstaller-6.7.0/PyInstaller/building/icon.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/building/makespec.py` & `pyinstaller-6.7.0/PyInstaller/building/makespec.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import os
 import re
 import sys
 
 from PyInstaller import DEFAULT_SPECPATH, HOMEPATH
 from PyInstaller import log as logging
 from PyInstaller.building.templates import bundleexetmplt, bundletmplt, onedirtmplt, onefiletmplt, splashtmpl
-from PyInstaller.compat import expand_path, is_darwin, is_win
+from PyInstaller.compat import is_darwin, is_win
 
 logger = logging.getLogger(__name__)
 
 # This list gives valid choices for the ``--debug`` command-line option, except for the ``all`` choice.
 DEBUG_ARGUMENT_CHOICES = ['imports', 'bootloader', 'noarchive']
 # This is the ``all`` choice.
 DEBUG_ALL_CHOICE = ['all']
@@ -711,16 +711,17 @@
     if name is None:
         name = os.path.splitext(os.path.basename(scripts[0]))[0]
 
     # If specpath not specified - use default value - current working directory.
     if specpath is None:
         specpath = DEFAULT_SPECPATH
     else:
-        # Expand tilde to user's home directory.
-        specpath = expand_path(specpath)
+        # Expand starting tilde into user's home directory, as a work-around for tilde not being expanded by shell when
+        # using ˙--specpath=~/path/abc` instead of ˙--specpath ~/path/abc` (or when the path argument is quoted).
+        specpath = os.path.expanduser(specpath)
     # If cwd is the root directory of PyInstaller, generate the .spec file in ./appname/ subdirectory.
     if specpath == HOMEPATH:
         specpath = os.path.join(HOMEPATH, name)
     # Create directory tree if missing.
     if not os.path.exists(specpath):
         os.makedirs(specpath)
```

### Comparing `pyinstaller-6.6.0/PyInstaller/building/osx.py` & `pyinstaller-6.7.0/PyInstaller/building/osx.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/building/splash.py` & `pyinstaller-6.7.0/PyInstaller/building/splash.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/building/splash_templates.py` & `pyinstaller-6.7.0/PyInstaller/building/splash_templates.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/building/templates.py` & `pyinstaller-6.7.0/PyInstaller/building/templates.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/building/utils.py` & `pyinstaller-6.7.0/PyInstaller/building/utils.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/compat.py` & `pyinstaller-6.7.0/PyInstaller/compat.py`

 * *Files 1% similar despite different names*

```diff
@@ -538,22 +538,14 @@
     cmdargs, kwargs = __wrap_python(args, kwargs)
     return exec_command_rc(*cmdargs, **kwargs)
 
 
 # Path handling.
 
 
-def expand_path(path: str | os.PathLike):
-    """
-    Replace initial tilde '~' in path with user's home directory, and also expand environment variables
-    (i.e., ${VARNAME} on Unix, %VARNAME% on Windows).
-    """
-    return os.path.expandvars(os.path.expanduser(path))
-
-
 # Site-packages functions - use native function if available.
 def getsitepackages(prefixes: list | None = None):
     """
     Returns a list containing all global site-packages directories.
 
     For each directory present in ``prefixes`` (or the global ``PREFIXES``), this function finds its `site-packages`
     subdirectory depending on the system environment, and returns a list of full paths.
```

### Comparing `pyinstaller-6.6.0/PyInstaller/config.py` & `pyinstaller-6.7.0/PyInstaller/config.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/configure.py` & `pyinstaller-6.7.0/PyInstaller/configure.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/depend/analysis.py` & `pyinstaller-6.7.0/PyInstaller/depend/analysis.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/depend/bindepend.py` & `pyinstaller-6.7.0/PyInstaller/depend/bindepend.py`

 * *Files 2% similar despite different names*

```diff
@@ -622,22 +622,31 @@
     """
     UNIX-specific helper for resolving library path.
 
     Emulates the algorithm used by dlopen. `name` must include the prefix, e.g., ``libpython2.4.so``.
     """
     assert compat.is_unix, "Current implementation for Unix only (Linux, Solaris, AIX, FreeBSD)"
 
+    if name.endswith('.so') or '.so.' in name:
+        # We have been given full library name that includes suffix. Use `_resolve_library_path_in_search_paths` to find
+        # the exact match.
+        lib_search_func = _resolve_library_path_in_search_paths
+    else:
+        # We have been given a library name without suffix. Use `_which_library` as search function, which will try to
+        # find library with matching basename.
+        lib_search_func = _which_library
+
     # Look in the LD_LIBRARY_PATH according to platform.
     if compat.is_aix:
         lp = compat.getenv('LIBPATH', '')
     elif compat.is_darwin:
         lp = compat.getenv('DYLD_LIBRARY_PATH', '')
     else:
         lp = compat.getenv('LD_LIBRARY_PATH', '')
-    lib = _which_library(name, filter(None, lp.split(os.pathsep)))
+    lib = lib_search_func(name, filter(None, lp.split(os.pathsep)))
 
     # Look in /etc/ld.so.cache
     # Solaris does not have /sbin/ldconfig. Just check if this file exists.
     if lib is None:
         utils.load_ldconfig_cache()
         lib = utils.LDCONFIG_CACHE.get(name)
         if lib:
@@ -678,28 +687,17 @@
         elif compat.is_hpux:
             if compat.architecture == '32bit':
                 paths.append('/usr/local/lib/hpux32')
             else:
                 paths.append('/usr/local/lib/hpux64')
         elif compat.is_freebsd or compat.is_openbsd:
             paths.append('/usr/local/lib')
-        lib = _which_library(name, paths)
+        lib = lib_search_func(name, paths)
 
-    # Give up :(
-    if lib is None:
-        return None
-
-    # Resolve the file name into the soname
-    if compat.is_freebsd or compat.is_aix or compat.is_openbsd:
-        # On FreeBSD objdump does not show SONAME, and on AIX objdump does not exist, so we just return the lib we
-        # have found.
-        return lib
-    else:
-        dir = os.path.dirname(lib)
-        return os.path.join(dir, _get_so_name(lib))
+    return lib
 
 
 def _which_library(name, dirs):
     """
     Search for a shared library in a list of directories.
 
     Args:
@@ -721,30 +719,14 @@
 def _library_matcher(name):
     """
     Create a callable that matches libraries if **name** is a valid library prefix for input library full names.
     """
     return re.compile(name + r"[0-9]*\.").match
 
 
-def _get_so_name(filename):
-    """
-    Return the soname of a library.
-
-    Soname is useful when there are multiple symplinks to one library.
-    """
-    # TODO verify that objdump works on other unixes and not Linux only.
-    cmd = ["objdump", "-p", filename]
-    pattern = r'\s+SONAME\s+([^\s]+)'
-    if compat.is_solar:
-        cmd = ["elfdump", "-d", filename]
-        pattern = r'\s+SONAME\s+[^\s]+\s+([^\s]+)'
-    m = re.search(pattern, compat.exec_command(*cmd))
-    return m.group(1)
-
-
 #- Python shared library search
 
 
 def get_python_library_path():
     """
     Find dynamic Python library that will be bundled with frozen executable.
```

### Comparing `pyinstaller-6.6.0/PyInstaller/depend/bytecode.py` & `pyinstaller-6.7.0/PyInstaller/depend/bytecode.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/depend/dylib.py` & `pyinstaller-6.7.0/PyInstaller/depend/dylib.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/depend/imphook.py` & `pyinstaller-6.7.0/PyInstaller/depend/imphook.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import glob
 import os.path
 import sys
 import weakref
 
 from PyInstaller import log as logging
 from PyInstaller.building.utils import format_binaries_and_datas
-from PyInstaller.compat import expand_path, importlib_load_source
+from PyInstaller.compat import importlib_load_source
 from PyInstaller.depend.imphookapi import PostGraphAPI
 from PyInstaller.exceptions import ImportErrorWhenRunningHook
 
 logger = logging.getLogger(__name__)
 
 # Safety check: Hook module names need to be unique. Duplicate names might occur if the cached PyuModuleGraph has an
 # issue.
@@ -100,15 +100,15 @@
         ----------
         hook_dirs : list
             List of the absolute or relative paths of all directories containing hook scripts to be cached.
         """
 
         for hook_dir in hook_dirs:
             # Canonicalize this directory's path and validate its existence.
-            hook_dir = os.path.abspath(expand_path(hook_dir))
+            hook_dir = os.path.abspath(hook_dir)
             if not os.path.isdir(hook_dir):
                 raise FileNotFoundError('Hook directory "{}" not found.'.format(hook_dir))
 
             # For each hook script in this directory...
             hook_filenames = glob.glob(os.path.join(hook_dir, 'hook-*.py'))
             for hook_filename in hook_filenames:
                 # Fully-qualified name of this hook's corresponding module, constructed by removing the "hook-" prefix
```

### Comparing `pyinstaller-6.6.0/PyInstaller/depend/imphookapi.py` & `pyinstaller-6.7.0/PyInstaller/depend/imphookapi.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/depend/utils.py` & `pyinstaller-6.7.0/PyInstaller/depend/utils.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/exceptions.py` & `pyinstaller-6.7.0/PyInstaller/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/fake-modules/_pyi_rth_utils/__init__.py` & `pyinstaller-6.7.0/PyInstaller/fake-modules/_pyi_rth_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/fake-modules/_pyi_rth_utils/_win32.py` & `pyinstaller-6.7.0/PyInstaller/fake-modules/_pyi_rth_utils/_win32.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/fake-modules/_pyi_rth_utils/qt.py` & `pyinstaller-6.7.0/PyInstaller/fake-modules/_pyi_rth_utils/qt.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/fake-modules/_pyi_rth_utils/tempfile.py` & `pyinstaller-6.7.0/PyInstaller/fake-modules/_pyi_rth_utils/tempfile.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/fake-modules/pyi_splash.py` & `pyinstaller-6.7.0/PyInstaller/fake-modules/pyi_splash.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PIL.Image.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PIL.Image.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PIL.ImageFilter.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PIL.ImageFilter.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PIL.SpiderImagePlugin.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PIL.SpiderImagePlugin.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PIL.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PIL.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.QAxContainer.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.QAxContainer.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.Qsci.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.Qsci.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.Qt.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.Qt.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.Qt3DAnimation.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.Qt3DAnimation.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.Qt3DCore.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.Qt3DCore.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.Qt3DExtras.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.Qt3DExtras.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.Qt3DInput.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.Qt3DInput.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.Qt3DLogic.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.Qt3DLogic.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.Qt3DRender.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.Qt3DRender.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.QtBluetooth.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.QtBluetooth.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.QtChart.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.QtChart.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.QtCore.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.QtCore.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.QtDBus.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.QtDBus.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.QtDataVisualization.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.QtDataVisualization.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.QtDesigner.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.QtDesigner.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.QtGui.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.QtGui.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.QtHelp.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.QtHelp.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.QtLocation.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.QtLocation.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.QtMacExtras.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.QtMacExtras.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.QtMultimedia.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.QtMultimedia.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.QtMultimediaWidgets.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.QtMultimediaWidgets.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.QtNetwork.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.QtNetwork.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.QtNetworkAuth.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.QtNetworkAuth.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.QtNfc.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.QtNfc.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.QtOpenGL.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.QtOpenGL.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.QtPositioning.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.QtPositioning.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.QtPrintSupport.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.QtPrintSupport.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.QtPurchasing.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.QtPurchasing.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.QtQml.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.QtQml.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.QtQuick.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.QtQuick.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.QtQuick3D.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.QtQuick3D.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.QtQuickWidgets.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.QtQuickWidgets.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.QtRemoteObjects.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.QtRemoteObjects.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.QtScript.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.QtScript.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.QtSensors.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.QtSensors.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.QtSerialPort.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.QtSerialPort.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.QtSql.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.QtSql.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.QtSvg.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.QtSvg.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.QtTest.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.QtTest.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.QtTextToSpeech.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.QtTextToSpeech.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.QtWebChannel.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.QtWebChannel.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.QtWebEngine.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.QtWebEngine.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.QtWebEngineCore.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.QtWebEngineCore.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.QtWebEngineWidgets.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.QtWebEngineWidgets.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.QtWebKit.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.QtWebKit.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.QtWebKitWidgets.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.QtWebKitWidgets.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.QtWebSockets.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.QtWebSockets.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.QtWidgets.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.QtWidgets.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.QtWinExtras.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.QtWinExtras.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.QtX11Extras.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.QtX11Extras.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.QtXml.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.QtXml.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.QtXmlPatterns.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.QtXmlPatterns.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt5.uic.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt5.uic.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.QAxContainer.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.QAxContainer.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.Qsci.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.Qsci.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.Qt3DAnimation.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.Qt3DAnimation.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.Qt3DCore.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.Qt3DCore.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.Qt3DExtras.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.Qt3DExtras.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.Qt3DInput.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.Qt3DInput.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.Qt3DLogic.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.Qt3DLogic.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.Qt3DRender.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.Qt3DRender.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.QtBluetooth.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.QtBluetooth.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.QtCharts.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.QtCharts.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.QtCore.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.QtCore.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.QtDBus.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.QtDBus.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.QtDataVisualization.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.QtDataVisualization.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.QtDesigner.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.QtDesigner.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.QtGui.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.QtGui.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.QtHelp.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.QtHelp.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.QtMultimedia.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.QtMultimedia.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.QtMultimediaWidgets.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.QtMultimediaWidgets.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.QtNetwork.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.QtNetwork.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.QtNetworkAuth.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.QtNetworkAuth.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.QtNfc.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.QtNfc.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.QtOpenGL.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.QtOpenGL.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.QtOpenGLWidgets.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.QtOpenGLWidgets.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.QtPdf.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.QtPdf.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.QtPdfWidgets.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.QtPdfWidgets.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.QtPositioning.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.QtPositioning.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.QtPrintSupport.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.QtPrintSupport.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.QtQml.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.QtQml.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.QtQuick.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.QtQuick.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.QtQuick3D.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.QtQuick3D.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.QtQuickWidgets.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.QtQuickWidgets.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.QtRemoteObjects.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.QtRemoteObjects.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.QtSensors.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.QtSensors.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.QtSerialPort.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.QtSerialPort.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.QtSpatialAudio.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.QtSpatialAudio.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.QtSql.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.QtSql.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.QtSvg.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.QtSvg.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.QtSvgWidgets.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.QtSvgWidgets.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.QtTest.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.QtTest.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.QtTextToSpeech.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.QtTextToSpeech.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.QtWebChannel.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.QtWebChannel.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.QtWebEngineCore.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.QtWebEngineCore.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.QtWebEngineQuick.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.QtWebEngineQuick.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.QtWebEngineWidgets.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.QtWebEngineWidgets.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.QtWebSockets.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.QtWebSockets.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.QtWidgets.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.QtWidgets.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.QtXml.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.QtXml.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PyQt6.uic.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PyQt6.uic.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.Qt3DAnimation.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.Qt3DAnimation.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.Qt3DCore.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.Qt3DCore.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.Qt3DExtras.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.Qt3DExtras.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.Qt3DInput.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.Qt3DInput.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.Qt3DLogic.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.Qt3DLogic.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.Qt3DRender.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.Qt3DRender.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.QtAxContainer.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.QtAxContainer.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.QtCharts.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.QtCharts.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.QtConcurrent.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.QtConcurrent.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.QtCore.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.QtCore.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.QtDataVisualization.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.QtDataVisualization.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.QtGui.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.QtGui.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.QtHelp.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.QtHelp.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.QtLocation.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.QtLocation.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.QtMacExtras.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.QtMacExtras.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.QtMultimedia.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.QtMultimedia.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.QtMultimediaWidgets.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.QtMultimediaWidgets.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.QtNetwork.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.QtNetwork.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.QtOpenGL.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.QtOpenGL.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.QtOpenGLFunctions.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.QtOpenGLFunctions.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.QtPositioning.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.QtPositioning.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.QtPrintSupport.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.QtPrintSupport.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.QtQml.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.QtQml.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.QtQuick.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.QtQuick.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.QtQuickControls2.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.QtQuickControls2.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.QtQuickWidgets.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.QtQuickWidgets.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.QtRemoteObjects.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.QtRemoteObjects.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.QtScript.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.QtScript.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.QtScriptTools.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.QtScriptTools.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.QtScxml.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.QtScxml.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.QtSensors.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.QtSensors.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.QtSerialPort.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.QtSerialPort.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.QtSql.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.QtSql.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.QtSvg.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.QtSvg.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.QtTest.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.QtTest.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.QtTextToSpeech.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.QtTextToSpeech.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.QtUiTools.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.QtUiTools.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.QtWebChannel.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.QtWebChannel.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.QtWebEngine.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.QtWebEngine.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.QtWebEngineCore.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.QtWebEngineCore.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.QtWebEngineWidgets.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.QtWebEngineWidgets.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.QtWebKit.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.QtWebKit.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.QtWebKitWidgets.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.QtWebKitWidgets.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.QtWebSockets.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.QtWebSockets.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.QtWidgets.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.QtWidgets.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.QtWinExtras.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.QtWinExtras.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.QtX11Extras.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.QtX11Extras.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.QtXml.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.QtXml.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.QtXmlPatterns.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.QtXmlPatterns.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.Qwt5.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.Qwt5.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide2.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide2.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.Qt3DAnimation.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.Qt3DAnimation.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.Qt3DCore.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.Qt3DCore.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.Qt3DExtras.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.Qt3DExtras.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.Qt3DInput.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.Qt3DInput.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.Qt3DLogic.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.Qt3DLogic.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.Qt3DRender.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.Qt3DRender.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtAxContainer.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtAxContainer.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtBluetooth.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtBluetooth.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtCharts.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtCharts.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtConcurrent.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtConcurrent.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtCore.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtCore.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtDBus.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtDBus.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtDataVisualization.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtDataVisualization.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtDesigner.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtDesigner.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtGraphs.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtGraphs.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtGui.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtGui.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtHelp.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtHelp.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtHttpServer.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtHttpServer.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtLocation.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtLocation.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtMultimedia.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtMultimedia.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtMultimediaWidgets.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtMultimediaWidgets.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtNetwork.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtNetwork.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtNetworkAuth.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtNetworkAuth.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtNfc.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtNfc.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtOpenGL.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtOpenGL.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtOpenGLWidgets.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtOpenGLWidgets.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtPdf.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtPdf.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtPdfWidgets.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtPdfWidgets.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtPositioning.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtPositioning.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtPrintSupport.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtPrintSupport.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtQml.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtQml.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtQuick.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtQuick.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtQuick3D.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtQuick3D.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtQuickControls2.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtQuickControls2.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtQuickWidgets.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtQuickWidgets.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtRemoteObjects.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtRemoteObjects.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtScxml.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtScxml.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtSensors.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtSensors.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtSerialBus.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtSerialBus.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtSerialPort.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtSerialPort.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtSpatialAudio.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtSpatialAudio.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtSql.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtSql.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtStateMachine.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtStateMachine.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtSvg.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtSvg.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtSvgWidgets.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtSvgWidgets.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtTest.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtTest.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtTextToSpeech.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtTextToSpeech.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtUiTools.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtUiTools.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtWebChannel.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtWebChannel.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtWebEngineCore.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtWebEngineCore.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtWebEngineQuick.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtWebEngineQuick.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtWebEngineWidgets.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtWebEngineWidgets.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtWebSockets.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtWebSockets.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtWidgets.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtWidgets.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.QtXml.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.QtXml.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-PySide6.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-PySide6.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-_pyi_rth_utils.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-_pyi_rth_utils.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-_tkinter.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-_tkinter.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-babel.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-babel.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-difflib.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-difflib.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-distutils.command.check.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-distutils.command.check.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-distutils.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-distutils.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-distutils.util.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-distutils.util.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-django.contrib.sessions.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-django.contrib.sessions.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-django.core.cache.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-django.core.cache.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-django.core.mail.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-django.core.mail.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-django.core.management.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-django.core.management.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-django.db.backends.mysql.base.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-django.db.backends.mysql.base.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-django.db.backends.oracle.base.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-django.db.backends.oracle.base.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-django.db.backends.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-django.db.backends.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-django.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-django.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-django.template.loaders.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-django.template.loaders.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-encodings.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-encodings.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-gevent.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-gevent.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.Adw.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.Adw.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.AppIndicator3.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.AppIndicator3.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.Atk.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.Atk.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.AyatanaAppIndicator3.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.AyatanaAppIndicator3.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.Champlain.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.Champlain.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.Clutter.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.Clutter.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.DBus.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.DBus.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.GIRepository.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.GIRepository.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.GLib.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.GLib.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.GModule.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.GModule.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.GObject.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.GObject.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.Gdk.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.Gdk.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.GdkPixbuf.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.GdkPixbuf.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.Gio.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.Gio.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.Graphene.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.Graphene.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.Gsk.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.Gsk.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.Gst.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.Gst.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.GstAllocators.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.GstAllocators.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.GstApp.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.GstApp.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.GstAudio.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.GstAudio.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.GstBadAudio.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.GstBadAudio.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.GstBase.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.GstBase.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.GstCheck.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.GstCheck.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.GstCodecs.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.GstCodecs.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.GstController.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.GstController.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.GstGL.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.GstGL.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.GstGLEGL.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.GstGLEGL.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.GstGLWayland.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.GstGLWayland.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.GstGLX11.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.GstGLX11.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.GstInsertBin.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.GstInsertBin.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.GstMpegts.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.GstMpegts.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.GstNet.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.GstNet.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.GstPbutils.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.GstPbutils.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.GstPlay.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.GstPlay.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.GstPlayer.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.GstPlayer.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.GstRtp.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.GstRtp.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.GstRtsp.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.GstRtsp.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.GstRtspServer.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.GstRtspServer.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.GstSdp.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.GstSdp.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.GstTag.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.GstTag.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.GstTranscoder.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.GstTranscoder.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.GstVideo.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.GstVideo.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.GstVulkan.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.GstVulkan.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.GstVulkanWayland.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.GstVulkanWayland.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.GstVulkanXCB.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.GstVulkanXCB.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.GstWebRTC.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.GstWebRTC.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.Gtk.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.Gtk.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.GtkChamplain.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.GtkChamplain.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.GtkClutter.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.GtkClutter.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.GtkSource.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.GtkSource.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.GtkosxApplication.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.GtkosxApplication.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.HarfBuzz.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.HarfBuzz.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.Pango.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.Pango.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.PangoCairo.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.PangoCairo.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.cairo.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.cairo.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.freetype2.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.freetype2.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-gi.repository.xlib.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-gi.repository.xlib.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-heapq.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-heapq.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-idlelib.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-idlelib.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-importlib_metadata.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-importlib_metadata.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-importlib_resources.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-importlib_resources.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-keyring.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-keyring.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-kivy.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-kivy.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-lib2to3.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-lib2to3.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-matplotlib.backends.backend_qtagg.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-matplotlib.backends.backend_qtagg.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-matplotlib.backends.backend_qtcairo.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-matplotlib.backends.backend_qtcairo.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-matplotlib.backends.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-matplotlib.backends.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-matplotlib.backends.qt_compat.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-matplotlib.backends.qt_compat.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-matplotlib.numerix.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-matplotlib.numerix.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-matplotlib.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-matplotlib.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-multiprocessing.util.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-multiprocessing.util.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-numpy.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-numpy.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-packaging.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-packaging.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-pandas.io.clipboard.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-pandas.io.clipboard.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-pandas.io.formats.style.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-pandas.io.formats.style.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-pandas.plotting.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-pandas.plotting.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-pandas.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-pandas.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-pickle.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-pickle.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-pkg_resources.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-pkg_resources.py`

 * *Files 7% similar despite different names*

```diff
@@ -51,7 +51,13 @@
 # accommodate it with couple of hidden imports.
 elif check_requirement("setuptools >= 60.7.1"):
     hiddenimports += [
         'pkg_resources._vendor.jaraco.functools',
         'pkg_resources._vendor.jaraco.context',
         'pkg_resources._vendor.jaraco.text',
     ]
+
+# As of setuptools 70.0.0, we need pkg_resources.extern added to hidden imports.
+if check_requirement("setuptools >= 70.0.0"):
+    hiddenimports += [
+        'pkg_resources.extern',
+    ]
```

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-platform.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-platform.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-pygments.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-pygments.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-pytz.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-pytz.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-pytzdata.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-pytzdata.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-qtawesome.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-qtawesome.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-qtpy.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-qtpy.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-scapy.layers.all.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-scapy.layers.all.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-scipy.io.matlab.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-scipy.io.matlab.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-scipy.linalg.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-scipy.linalg.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-scipy.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-scipy.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-scipy.sparse.csgraph.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-scipy.sparse.csgraph.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-scipy.spatial.transform.rotation.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-scipy.spatial.transform.rotation.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-scipy.special._ellip_harm_2.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-scipy.special._ellip_harm_2.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-scipy.special._ufuncs.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-scipy.special._ufuncs.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-scipy.stats._stats.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-scipy.stats._stats.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-scrapy.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-scrapy.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-setuptools._distutils.command.check.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-setuptools._distutils.command.check.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-setuptools.msvc.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-setuptools.msvc.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-setuptools.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-setuptools.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-shelve.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-shelve.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-shiboken6.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-shiboken6.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-sphinx.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-sphinx.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-sqlalchemy.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-sqlalchemy.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,15 +10,17 @@
 #-----------------------------------------------------------------------------
 
 import re
 import importlib.util
 
 from PyInstaller import isolated
 from PyInstaller.lib.modulegraph.modulegraph import SourceModule
-from PyInstaller.utils.hooks import check_requirement, logger
+from PyInstaller.utils.hooks import check_requirement, collect_entry_point, logger
+
+datas = []
 
 # 'sqlalchemy.testing' causes bundling a lot of unnecessary modules.
 excludedimports = ['sqlalchemy.testing']
 
 # Include most common database bindings some database bindings are detected and include some are not. We should
 # explicitly include database backends.
 hiddenimports = ['pysqlite2', 'MySQLdb', 'psycopg2', 'sqlalchemy.ext.baked']
@@ -37,14 +39,21 @@
 # In SQLAlchemy >= 0.6, the "sqlalchemy.dialects" package provides dialects.
 # In SQLAlchemy <= 0.5, the "sqlalchemy.databases" package provides dialects.
 if check_requirement('sqlalchemy >= 0.6'):
     hiddenimports += _get_dialect_modules("sqlalchemy.dialects")
 else:
     hiddenimports += _get_dialect_modules("sqlalchemy.databases")
 
+# Collect additional dialects and plugins that are registered via entry-points, under assumption that they are available
+# in the build environment for a reason (i.e., they are used).
+for entry_point_name in ('sqlalchemy.dialects', 'sqlalchemy.plugins'):
+    ep_datas, ep_hiddenimports = collect_entry_point(entry_point_name)
+    datas += ep_datas
+    hiddenimports += ep_hiddenimports
+
 
 def hook(hook_api):
     """
     SQLAlchemy 0.9 introduced the decorator 'util.dependencies'.  This decorator does imports. E.g.:
 
             @util.dependencies("sqlalchemy.sql.schema")
```

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-sqlite3.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-sqlite3.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-sysconfig.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-sysconfig.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-wcwidth.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-wcwidth.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-win32ctypes.core.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-win32ctypes.core.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,13 +9,14 @@
 # SPDX-License-Identifier: (GPL-2.0-or-later WITH Bootloader-exception)
 #-----------------------------------------------------------------------------
 
 # TODO: remove this hook during PyInstaller 4.5 release cycle!
 
 from PyInstaller.utils.hooks import can_import_module, collect_submodules
 
-# We need to collect submodules from win32ctypes.core.cffi or win32ctypes.core.ctypes for win32ctypes.core to work. The
-# use of the backend is determined by availability of cffi.
+# We need to collect submodules from win32ctypes.core.cffi or win32ctypes.core.ctypes for win32ctypes.core to work.
+# Always collect the `ctypes` backend, and add the `cffi` one if `cffi` is available. Having the `ctypes` backend always
+# available helps in situations when `cffi` is available in the build environment, but is disabled at run-time or not
+# collected (e.g., due to `--exclude cffi`).
+hiddenimports = collect_submodules('win32ctypes.core.ctypes')
 if can_import_module('cffi'):
-    hiddenimports = collect_submodules('win32ctypes.core.cffi')
-else:
-    hiddenimports = collect_submodules('win32ctypes.core.ctypes')
+    hiddenimports += collect_submodules('win32ctypes.core.cffi')
```

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-xml.dom.domreg.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-xml.dom.domreg.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-xml.etree.cElementTree.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-xml.etree.cElementTree.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-xml.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-xml.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/hook-zope.interface.py` & `pyinstaller-6.7.0/PyInstaller/hooks/hook-zope.interface.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/pre_find_module_path/hook-PyQt5.uic.port_v2.py` & `pyinstaller-6.7.0/PyInstaller/hooks/pre_find_module_path/hook-PyQt5.uic.port_v2.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/pre_find_module_path/hook-_pyi_rth_utils.py` & `pyinstaller-6.7.0/PyInstaller/hooks/pre_find_module_path/hook-_pyi_rth_utils.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/pre_find_module_path/hook-distutils.py` & `pyinstaller-6.7.0/PyInstaller/hooks/pre_find_module_path/hook-distutils.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/pre_find_module_path/hook-pyi_splash.py` & `pyinstaller-6.7.0/PyInstaller/hooks/pre_find_module_path/hook-pyi_splash.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-distutils.py` & `pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-distutils.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.py` & `pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.Adw.py` & `pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.Adw.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.AppIndicator3.py` & `pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.AppIndicator3.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.Atk.py` & `pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.Atk.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.AyatanaAppIndicator3.py` & `pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.AyatanaAppIndicator3.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.Champlain.py` & `pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.Champlain.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.Clutter.py` & `pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.Clutter.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.DBus.py` & `pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.DBus.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GIRepository.py` & `pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GIRepository.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GLib.py` & `pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GLib.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GModule.py` & `pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GModule.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GObject.py` & `pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GObject.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.Gdk.py` & `pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.Gdk.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GdkPixbuf.py` & `pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GdkPixbuf.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.Gio.py` & `pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.Gio.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.Graphene.py` & `pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.Graphene.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.Gsk.py` & `pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.Gsk.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.Gst.py` & `pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.Gst.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstAllocators.py` & `pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstAllocators.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstApp.py` & `pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstApp.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstAudio.py` & `pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstAudio.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstBadAudio.py` & `pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstBadAudio.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstBase.py` & `pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstBase.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstCheck.py` & `pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstCheck.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstCodecs.py` & `pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstCodecs.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstController.py` & `pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstController.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstGL.py` & `pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstGL.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstGLEGL.py` & `pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstGLEGL.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstGLWayland.py` & `pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstGLWayland.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstGLX11.py` & `pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstGLX11.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstInsertBin.py` & `pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstInsertBin.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstMpegts.py` & `pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstMpegts.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstNet.py` & `pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstNet.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstPbutils.py` & `pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstPbutils.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstPlay.py` & `pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstPlay.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstPlayer.py` & `pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstPlayer.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstRtp.py` & `pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstRtp.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstRtsp.py` & `pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstRtsp.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstRtspServer.py` & `pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstRtspServer.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstSdp.py` & `pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstSdp.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstTag.py` & `pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstTag.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstTranscoder.py` & `pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstTranscoder.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstVideo.py` & `pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstVideo.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstVulkan.py` & `pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstVulkan.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstVulkanWayland.py` & `pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstVulkanWayland.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstVulkanXCB.py` & `pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstVulkanXCB.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstWebRTC.py` & `pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GstWebRTC.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.Gtk.py` & `pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.Gtk.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GtkChamplain.py` & `pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GtkChamplain.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GtkClutter.py` & `pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GtkClutter.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GtkSource.py` & `pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GtkSource.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GtkosxApplication.py` & `pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.GtkosxApplication.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.HarfBuzz.py` & `pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.HarfBuzz.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.Pango.py` & `pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.Pango.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.PangoCairo.py` & `pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.PangoCairo.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.cairo.py` & `pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.cairo.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.freetype2.py` & `pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.freetype2.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.xlib.py` & `pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-gi.repository.xlib.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-setuptools.extern.six.moves.py` & `pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-setuptools.extern.six.moves.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-six.moves.py` & `pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-six.moves.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/pre_safe_import_module/hook-urllib3.packages.six.moves.py` & `pyinstaller-6.7.0/PyInstaller/hooks/pre_safe_import_module/hook-urllib3.packages.six.moves.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/rthooks/pyi_rth__tkinter.py` & `pyinstaller-6.7.0/PyInstaller/hooks/rthooks/pyi_rth__tkinter.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/rthooks/pyi_rth_django.py` & `pyinstaller-6.7.0/PyInstaller/hooks/rthooks/pyi_rth_django.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/rthooks/pyi_rth_gdkpixbuf.py` & `pyinstaller-6.7.0/PyInstaller/hooks/rthooks/pyi_rth_gdkpixbuf.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/rthooks/pyi_rth_gi.py` & `pyinstaller-6.7.0/PyInstaller/hooks/rthooks/pyi_rth_gi.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/rthooks/pyi_rth_gio.py` & `pyinstaller-6.7.0/PyInstaller/hooks/rthooks/pyi_rth_gio.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/rthooks/pyi_rth_glib.py` & `pyinstaller-6.7.0/PyInstaller/hooks/rthooks/pyi_rth_glib.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/rthooks/pyi_rth_gstreamer.py` & `pyinstaller-6.7.0/PyInstaller/hooks/rthooks/pyi_rth_gstreamer.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/rthooks/pyi_rth_gtk.py` & `pyinstaller-6.7.0/PyInstaller/hooks/rthooks/pyi_rth_gtk.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/rthooks/pyi_rth_inspect.py` & `pyinstaller-6.7.0/PyInstaller/hooks/rthooks/pyi_rth_inspect.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/rthooks/pyi_rth_kivy.py` & `pyinstaller-6.7.0/PyInstaller/hooks/rthooks/pyi_rth_kivy.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/rthooks/pyi_rth_mplconfig.py` & `pyinstaller-6.7.0/PyInstaller/hooks/rthooks/pyi_rth_mplconfig.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/rthooks/pyi_rth_multiprocessing.py` & `pyinstaller-6.7.0/PyInstaller/hooks/rthooks/pyi_rth_multiprocessing.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/rthooks/pyi_rth_pkgres.py` & `pyinstaller-6.7.0/PyInstaller/hooks/rthooks/pyi_rth_pkgres.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/rthooks/pyi_rth_pkgutil.py` & `pyinstaller-6.7.0/PyInstaller/hooks/rthooks/pyi_rth_pkgutil.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/rthooks/pyi_rth_pyqt5.py` & `pyinstaller-6.7.0/PyInstaller/hooks/rthooks/pyi_rth_pyqt5.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/rthooks/pyi_rth_pyqt6.py` & `pyinstaller-6.7.0/PyInstaller/hooks/rthooks/pyi_rth_pyqt6.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/rthooks/pyi_rth_pyside2.py` & `pyinstaller-6.7.0/PyInstaller/hooks/rthooks/pyi_rth_pyside2.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/rthooks/pyi_rth_pyside6.py` & `pyinstaller-6.7.0/PyInstaller/hooks/rthooks/pyi_rth_pyside6.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/rthooks/pyi_rth_setuptools.py` & `pyinstaller-6.7.0/PyInstaller/hooks/rthooks/pyi_rth_setuptools.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/hooks/rthooks.dat` & `pyinstaller-6.7.0/PyInstaller/hooks/rthooks.dat`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/isolated/__init__.py` & `pyinstaller-6.7.0/PyInstaller/isolated/__init__.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/isolated/_child.py` & `pyinstaller-6.7.0/PyInstaller/isolated/_child.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/isolated/_parent.py` & `pyinstaller-6.7.0/PyInstaller/isolated/_parent.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/lib/README.rst` & `pyinstaller-6.7.0/PyInstaller/lib/README.rst`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/lib/modulegraph/__main__.py` & `pyinstaller-6.7.0/PyInstaller/lib/modulegraph/__main__.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/lib/modulegraph/find_modules.py` & `pyinstaller-6.7.0/PyInstaller/lib/modulegraph/find_modules.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/lib/modulegraph/modulegraph.py` & `pyinstaller-6.7.0/PyInstaller/lib/modulegraph/modulegraph.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/lib/modulegraph/util.py` & `pyinstaller-6.7.0/PyInstaller/lib/modulegraph/util.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/loader/pyiboot01_bootstrap.py` & `pyinstaller-6.7.0/PyInstaller/loader/pyiboot01_bootstrap.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/loader/pyimod01_archive.py` & `pyinstaller-6.7.0/PyInstaller/loader/pyimod01_archive.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/loader/pyimod02_importers.py` & `pyinstaller-6.7.0/PyInstaller/loader/pyimod02_importers.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/loader/pyimod03_ctypes.py` & `pyinstaller-6.7.0/PyInstaller/loader/pyimod03_ctypes.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/loader/pyimod04_pywin32.py` & `pyinstaller-6.7.0/PyInstaller/loader/pyimod04_pywin32.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/log.py` & `pyinstaller-6.7.0/PyInstaller/log.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/utils/cliutils/archive_viewer.py` & `pyinstaller-6.7.0/PyInstaller/utils/cliutils/archive_viewer.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/utils/cliutils/bindepend.py` & `pyinstaller-6.7.0/PyInstaller/utils/cliutils/bindepend.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/utils/cliutils/grab_version.py` & `pyinstaller-6.7.0/PyInstaller/utils/cliutils/grab_version.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/utils/cliutils/makespec.py` & `pyinstaller-6.7.0/PyInstaller/utils/cliutils/makespec.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/utils/cliutils/set_version.py` & `pyinstaller-6.7.0/PyInstaller/utils/cliutils/set_version.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/utils/conftest.py` & `pyinstaller-6.7.0/PyInstaller/utils/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -331,14 +331,20 @@
         prog_env = copy.deepcopy(os.environ)
         prog_env['PATH'] = ''
         del prog_env['PATH']
         # For Windows we need to keep minimal PATH for successful running of some tests.
         if is_win:
             # Minimum Windows PATH is in most cases:   C:\Windows\system32;C:\Windows
             prog_env['PATH'] = os.pathsep.join(winutils.get_system_path())
+        # On macOS, we similarly set up minimal PATH with system directories, in case utilities from there are used by
+        # tested python code (for example, matplotlib >= 3.9.0 uses `system_profiler` that is found in /usr/sbin).
+        if is_darwin:
+            # The following paths are registered when application is launched via Finder, and are a subset of what is
+            # typically available in the shell.
+            prog_env['PATH'] = os.pathsep.join(['/usr/bin', '/bin', '/usr/sbin', '/sbin'])
 
         exe_path = prog
         if run_from_path:
             # Run executable in the temp directory. Add the directory containing the executable to $PATH. Basically,
             # pretend we are a shell executing the program from $PATH.
             prog_cwd = str(self._tmpdir)
             prog_name = os.path.basename(prog)
```

### Comparing `pyinstaller-6.6.0/PyInstaller/utils/git.py` & `pyinstaller-6.7.0/PyInstaller/utils/git.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/utils/hooks/__init__.py` & `pyinstaller-6.7.0/PyInstaller/utils/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/utils/hooks/conda.py` & `pyinstaller-6.7.0/PyInstaller/utils/hooks/conda.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/utils/hooks/django.py` & `pyinstaller-6.7.0/PyInstaller/utils/hooks/django.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/utils/hooks/gi.py` & `pyinstaller-6.7.0/PyInstaller/utils/hooks/gi.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/utils/hooks/qt/__init__.py` & `pyinstaller-6.7.0/PyInstaller/utils/hooks/qt/__init__.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/utils/hooks/qt/_modules_info.py` & `pyinstaller-6.7.0/PyInstaller/utils/hooks/qt/_modules_info.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/utils/hooks/tcl_tk.py` & `pyinstaller-6.7.0/PyInstaller/utils/hooks/tcl_tk.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/utils/misc.py` & `pyinstaller-6.7.0/PyInstaller/utils/misc.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/utils/osx.py` & `pyinstaller-6.7.0/PyInstaller/utils/osx.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/utils/run_tests.py` & `pyinstaller-6.7.0/PyInstaller/utils/run_tests.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/utils/tests.py` & `pyinstaller-6.7.0/PyInstaller/utils/tests.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/utils/win32/icon.py` & `pyinstaller-6.7.0/PyInstaller/utils/win32/icon.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/utils/win32/versioninfo.py` & `pyinstaller-6.7.0/PyInstaller/utils/win32/versioninfo.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/utils/win32/winmanifest.py` & `pyinstaller-6.7.0/PyInstaller/utils/win32/winmanifest.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/utils/win32/winresource.py` & `pyinstaller-6.7.0/PyInstaller/utils/win32/winresource.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/PyInstaller/utils/win32/winutils.py` & `pyinstaller-6.7.0/PyInstaller/utils/win32/winutils.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/README.rst` & `pyinstaller-6.7.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -130,21 +130,21 @@
 pyinstaller`` provided that you have an appropriate C compiler (typically
 either ``gcc`` or ``clang``) and zlib's development headers already installed.
 
 
 Support
 -------
 
-- Official debugging guide: https://pyinstaller.org/en/v6.6.0/when-things-go-wrong.html
+- Official debugging guide: https://pyinstaller.org/en/v6.7.0/when-things-go-wrong.html
 - Assorted user contributed help topics: https://github.com/pyinstaller/pyinstaller/wiki
 - Web based Q&A forums: https://github.com/pyinstaller/pyinstaller/discussions
 - Email based Q&A forums: https://groups.google.com/g/pyinstaller
 
 
 Changes in this Release
 -----------------------
 
 You can find a detailed list of changes in this release
 in the `Changelog`_ section of the manual.
 
-.. _`manual`: https://pyinstaller.org/en/v6.6.0/
-.. _`Changelog`: https://pyinstaller.org/en/v6.6.0/CHANGES.html
+.. _`manual`: https://pyinstaller.org/en/v6.7.0/
+.. _`Changelog`: https://pyinstaller.org/en/v6.7.0/CHANGES.html
```

### Comparing `pyinstaller-6.6.0/alpine.dockerfile` & `pyinstaller-6.7.0/alpine.dockerfile`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/Dockerfile` & `pyinstaller-6.7.0/bootloader/Dockerfile`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/Dockerfile.osxcross` & `pyinstaller-6.7.0/bootloader/Dockerfile.osxcross`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/README.txt` & `pyinstaller-6.7.0/bootloader/README.txt`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/Vagrantfile` & `pyinstaller-6.7.0/bootloader/Vagrantfile`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/build.sh` & `pyinstaller-6.7.0/bootloader/build.sh`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/src/main.c` & `pyinstaller-6.7.0/bootloader/src/main.c`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/src/mkdtemp.h` & `pyinstaller-6.7.0/bootloader/src/mkdtemp.h`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/src/pyi_apple_events.c` & `pyinstaller-6.7.0/bootloader/src/pyi_apple_events.c`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/src/pyi_apple_events.h` & `pyinstaller-6.7.0/bootloader/src/pyi_apple_events.h`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/src/pyi_archive.c` & `pyinstaller-6.7.0/bootloader/src/pyi_archive.c`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/src/pyi_archive.h` & `pyinstaller-6.7.0/bootloader/src/pyi_archive.h`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/src/pyi_exception_dialog.c` & `pyinstaller-6.7.0/bootloader/src/pyi_exception_dialog.c`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/src/pyi_exception_dialog.h` & `pyinstaller-6.7.0/bootloader/src/pyi_exception_dialog.h`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/src/pyi_global.c` & `pyinstaller-6.7.0/bootloader/src/pyi_global.c`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/src/pyi_global.h` & `pyinstaller-6.7.0/bootloader/src/pyi_global.h`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/src/pyi_launch.c` & `pyinstaller-6.7.0/bootloader/src/pyi_launch.c`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/src/pyi_launch.h` & `pyinstaller-6.7.0/bootloader/src/pyi_launch.h`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/src/pyi_main.c` & `pyinstaller-6.7.0/bootloader/src/pyi_main.c`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/src/pyi_main.h` & `pyinstaller-6.7.0/bootloader/src/pyi_main.h`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/src/pyi_path.c` & `pyinstaller-6.7.0/bootloader/src/pyi_path.c`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/src/pyi_path.h` & `pyinstaller-6.7.0/bootloader/src/pyi_path.h`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/src/pyi_pyconfig.c` & `pyinstaller-6.7.0/bootloader/src/pyi_pyconfig.c`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/src/pyi_pyconfig.h` & `pyinstaller-6.7.0/bootloader/src/pyi_pyconfig.h`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/src/pyi_pyconfig_v310.h` & `pyinstaller-6.7.0/bootloader/src/pyi_pyconfig_v310.h`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/src/pyi_pyconfig_v311.h` & `pyinstaller-6.7.0/bootloader/src/pyi_pyconfig_v311.h`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/src/pyi_pyconfig_v312.h` & `pyinstaller-6.7.0/bootloader/src/pyi_pyconfig_v312.h`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/src/pyi_pyconfig_v38.h` & `pyinstaller-6.7.0/bootloader/src/pyi_pyconfig_v38.h`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/src/pyi_pyconfig_v39.h` & `pyinstaller-6.7.0/bootloader/src/pyi_pyconfig_v39.h`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/src/pyi_python.c` & `pyinstaller-6.7.0/bootloader/src/pyi_python.c`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/src/pyi_python.h` & `pyinstaller-6.7.0/bootloader/src/pyi_python.h`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/src/pyi_pythonlib.c` & `pyinstaller-6.7.0/bootloader/src/pyi_pythonlib.c`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/src/pyi_pythonlib.h` & `pyinstaller-6.7.0/bootloader/src/pyi_pythonlib.h`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/src/pyi_splash.c` & `pyinstaller-6.7.0/bootloader/src/pyi_splash.c`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/src/pyi_splash.h` & `pyinstaller-6.7.0/bootloader/src/pyi_splash.h`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/src/pyi_splashlib.c` & `pyinstaller-6.7.0/bootloader/src/pyi_splashlib.c`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/src/pyi_splashlib.h` & `pyinstaller-6.7.0/bootloader/src/pyi_splashlib.h`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/src/pyi_utils.c` & `pyinstaller-6.7.0/bootloader/src/pyi_utils.c`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/src/pyi_utils.h` & `pyinstaller-6.7.0/bootloader/src/pyi_utils.h`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/src/pyi_win32_utils.c` & `pyinstaller-6.7.0/bootloader/src/pyi_win32_utils.c`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/src/pyi_win32_utils.h` & `pyinstaller-6.7.0/bootloader/src/pyi_win32_utils.h`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/tests/test_launch.c` & `pyinstaller-6.7.0/bootloader/tests/test_launch.c`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/tests/test_path.c` & `pyinstaller-6.7.0/bootloader/tests/test_path.c`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/tests/wscript` & `pyinstaller-6.7.0/bootloader/tests/wscript`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/tools/strip.py` & `pyinstaller-6.7.0/bootloader/tools/strip.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/uncrustify.cfg` & `pyinstaller-6.7.0/bootloader/uncrustify.cfg`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/update-waf.sh` & `pyinstaller-6.7.0/bootloader/update-waf.sh`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/waf` & `pyinstaller-6.7.0/bootloader/waf`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/waflib/Build.py` & `pyinstaller-6.7.0/bootloader/waflib/Build.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/waflib/ConfigSet.py` & `pyinstaller-6.7.0/bootloader/waflib/ConfigSet.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/waflib/Configure.py` & `pyinstaller-6.7.0/bootloader/waflib/Configure.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/waflib/Context.py` & `pyinstaller-6.7.0/bootloader/waflib/Context.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/waflib/Errors.py` & `pyinstaller-6.7.0/bootloader/waflib/Errors.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/waflib/Logs.py` & `pyinstaller-6.7.0/bootloader/waflib/Logs.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/waflib/Node.py` & `pyinstaller-6.7.0/bootloader/waflib/Node.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/waflib/Options.py` & `pyinstaller-6.7.0/bootloader/waflib/Options.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/waflib/Runner.py` & `pyinstaller-6.7.0/bootloader/waflib/Runner.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/waflib/Scripting.py` & `pyinstaller-6.7.0/bootloader/waflib/Scripting.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/waflib/Task.py` & `pyinstaller-6.7.0/bootloader/waflib/Task.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/waflib/TaskGen.py` & `pyinstaller-6.7.0/bootloader/waflib/TaskGen.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/waflib/Tools/asm.py` & `pyinstaller-6.7.0/bootloader/waflib/Tools/asm.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/waflib/Tools/bison.py` & `pyinstaller-6.7.0/bootloader/waflib/Tools/bison.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/waflib/Tools/c.py` & `pyinstaller-6.7.0/bootloader/waflib/Tools/c.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/waflib/Tools/c_aliases.py` & `pyinstaller-6.7.0/bootloader/waflib/Tools/c_aliases.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/waflib/Tools/c_config.py` & `pyinstaller-6.7.0/bootloader/waflib/Tools/c_config.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/waflib/Tools/c_osx.py` & `pyinstaller-6.7.0/bootloader/waflib/Tools/c_osx.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/waflib/Tools/c_preproc.py` & `pyinstaller-6.7.0/bootloader/waflib/Tools/c_preproc.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/waflib/Tools/c_tests.py` & `pyinstaller-6.7.0/bootloader/waflib/Tools/c_tests.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/waflib/Tools/ccroot.py` & `pyinstaller-6.7.0/bootloader/waflib/Tools/ccroot.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/waflib/Tools/clang.py` & `pyinstaller-6.7.0/bootloader/waflib/Tools/clang.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/waflib/Tools/clangxx.py` & `pyinstaller-6.7.0/bootloader/waflib/Tools/clangxx.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/waflib/Tools/compiler_c.py` & `pyinstaller-6.7.0/bootloader/waflib/Tools/compiler_c.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/waflib/Tools/compiler_cxx.py` & `pyinstaller-6.7.0/bootloader/waflib/Tools/compiler_cxx.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/waflib/Tools/compiler_d.py` & `pyinstaller-6.7.0/bootloader/waflib/Tools/compiler_d.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/waflib/Tools/compiler_fc.py` & `pyinstaller-6.7.0/bootloader/waflib/Tools/compiler_fc.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/waflib/Tools/cs.py` & `pyinstaller-6.7.0/bootloader/waflib/Tools/cs.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/waflib/Tools/cxx.py` & `pyinstaller-6.7.0/bootloader/waflib/Tools/cxx.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/waflib/Tools/d.py` & `pyinstaller-6.7.0/bootloader/waflib/Tools/d.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/waflib/Tools/d_config.py` & `pyinstaller-6.7.0/bootloader/waflib/Tools/d_config.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/waflib/Tools/d_scan.py` & `pyinstaller-6.7.0/bootloader/waflib/Tools/d_scan.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/waflib/Tools/dbus.py` & `pyinstaller-6.7.0/bootloader/waflib/Tools/dbus.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/waflib/Tools/dmd.py` & `pyinstaller-6.7.0/bootloader/waflib/Tools/dmd.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/waflib/Tools/errcheck.py` & `pyinstaller-6.7.0/bootloader/waflib/Tools/errcheck.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/waflib/Tools/fc.py` & `pyinstaller-6.7.0/bootloader/waflib/Tools/fc.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/waflib/Tools/fc_config.py` & `pyinstaller-6.7.0/bootloader/waflib/Tools/fc_config.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/waflib/Tools/fc_scan.py` & `pyinstaller-6.7.0/bootloader/waflib/Tools/fc_scan.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/waflib/Tools/flex.py` & `pyinstaller-6.7.0/bootloader/waflib/Tools/flex.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/waflib/Tools/g95.py` & `pyinstaller-6.7.0/bootloader/waflib/Tools/g95.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/waflib/Tools/gcc.py` & `pyinstaller-6.7.0/bootloader/waflib/Tools/gcc.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/waflib/Tools/gdc.py` & `pyinstaller-6.7.0/bootloader/waflib/Tools/gdc.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/waflib/Tools/gfortran.py` & `pyinstaller-6.7.0/bootloader/waflib/Tools/gfortran.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/waflib/Tools/glib2.py` & `pyinstaller-6.7.0/bootloader/waflib/Tools/glib2.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/waflib/Tools/gnu_dirs.py` & `pyinstaller-6.7.0/bootloader/waflib/Tools/gnu_dirs.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/waflib/Tools/gxx.py` & `pyinstaller-6.7.0/bootloader/waflib/Tools/gxx.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/waflib/Tools/icc.py` & `pyinstaller-6.7.0/bootloader/waflib/Tools/icc.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/waflib/Tools/icpc.py` & `pyinstaller-6.7.0/bootloader/waflib/Tools/icpc.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/waflib/Tools/ifort.py` & `pyinstaller-6.7.0/bootloader/waflib/Tools/ifort.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/waflib/Tools/intltool.py` & `pyinstaller-6.7.0/bootloader/waflib/Tools/intltool.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/waflib/Tools/irixcc.py` & `pyinstaller-6.7.0/bootloader/waflib/Tools/irixcc.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/waflib/Tools/javaw.py` & `pyinstaller-6.7.0/bootloader/waflib/Tools/javaw.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/waflib/Tools/ldc2.py` & `pyinstaller-6.7.0/bootloader/waflib/Tools/ldc2.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/waflib/Tools/lua.py` & `pyinstaller-6.7.0/bootloader/waflib/Tools/lua.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/waflib/Tools/md5_tstamp.py` & `pyinstaller-6.7.0/bootloader/waflib/Tools/md5_tstamp.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/waflib/Tools/msvc.py` & `pyinstaller-6.7.0/bootloader/waflib/Tools/msvc.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/waflib/Tools/nasm.py` & `pyinstaller-6.7.0/bootloader/waflib/Tools/nasm.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/waflib/Tools/perl.py` & `pyinstaller-6.7.0/bootloader/waflib/Tools/perl.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/waflib/Tools/python.py` & `pyinstaller-6.7.0/bootloader/waflib/Tools/python.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/waflib/Tools/qt5.py` & `pyinstaller-6.7.0/bootloader/waflib/Tools/qt5.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/waflib/Tools/ruby.py` & `pyinstaller-6.7.0/bootloader/waflib/Tools/ruby.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/waflib/Tools/suncc.py` & `pyinstaller-6.7.0/bootloader/waflib/Tools/suncc.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/waflib/Tools/suncxx.py` & `pyinstaller-6.7.0/bootloader/waflib/Tools/suncxx.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/waflib/Tools/tex.py` & `pyinstaller-6.7.0/bootloader/waflib/Tools/tex.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/waflib/Tools/vala.py` & `pyinstaller-6.7.0/bootloader/waflib/Tools/vala.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/waflib/Tools/waf_unit_test.py` & `pyinstaller-6.7.0/bootloader/waflib/Tools/waf_unit_test.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/waflib/Tools/winres.py` & `pyinstaller-6.7.0/bootloader/waflib/Tools/winres.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/waflib/Tools/xlc.py` & `pyinstaller-6.7.0/bootloader/waflib/Tools/xlc.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/waflib/Tools/xlcxx.py` & `pyinstaller-6.7.0/bootloader/waflib/Tools/xlcxx.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/waflib/Utils.py` & `pyinstaller-6.7.0/bootloader/waflib/Utils.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/waflib/ansiterm.py` & `pyinstaller-6.7.0/bootloader/waflib/ansiterm.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/waflib/fixpy2.py` & `pyinstaller-6.7.0/bootloader/waflib/fixpy2.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/waflib/processor.py` & `pyinstaller-6.7.0/bootloader/waflib/processor.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/wscript` & `pyinstaller-6.7.0/bootloader/wscript`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/zlib/adler32.c` & `pyinstaller-6.7.0/bootloader/zlib/adler32.c`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/zlib/crc32.c` & `pyinstaller-6.7.0/bootloader/zlib/crc32.c`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/zlib/crc32.h` & `pyinstaller-6.7.0/bootloader/zlib/crc32.h`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/zlib/gzguts.h` & `pyinstaller-6.7.0/bootloader/zlib/gzguts.h`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/zlib/inffast.c` & `pyinstaller-6.7.0/bootloader/zlib/inffast.c`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/zlib/inffixed.h` & `pyinstaller-6.7.0/bootloader/zlib/inffixed.h`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/zlib/inflate.c` & `pyinstaller-6.7.0/bootloader/zlib/inflate.c`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/zlib/inflate.h` & `pyinstaller-6.7.0/bootloader/zlib/inflate.h`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/zlib/inftrees.c` & `pyinstaller-6.7.0/bootloader/zlib/inftrees.c`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/zlib/inftrees.h` & `pyinstaller-6.7.0/bootloader/zlib/inftrees.h`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/zlib/zconf.h` & `pyinstaller-6.7.0/bootloader/zlib/zconf.h`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/zlib/zlib.h` & `pyinstaller-6.7.0/bootloader/zlib/zlib.h`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/zlib/zutil.c` & `pyinstaller-6.7.0/bootloader/zlib/zutil.c`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/bootloader/zlib/zutil.h` & `pyinstaller-6.7.0/bootloader/zlib/zutil.h`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/doc/CHANGES-1.rst` & `pyinstaller-6.7.0/doc/CHANGES-1.rst`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/doc/CHANGES-2.rst` & `pyinstaller-6.7.0/doc/CHANGES-2.rst`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/doc/CHANGES-3.rst` & `pyinstaller-6.7.0/doc/CHANGES-3.rst`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/doc/CHANGES.rst` & `pyinstaller-6.7.0/doc/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,66 @@
    https://pyinstaller.readthedocs.io/en/latest/development/changelog-entries.html
 
 .. Preview unreleased news fragments.
 .. towncrier-draft-entries:: The Next Release
 
 .. towncrier release notes start
 
+6.7.0 (2024-05-21)
+------------------
+
+Bugfix
+~~~~~~
+
+* (POSIX) Fix ``PyInstaller.depend.bindepend.resolve_library_path`` for
+  cases when ``ldconfig`` cache is not available (e.g., ``musl libc`` on
+  Alpine Linux). In such cases, the search code now distinguishes between
+  the case when fully suffixed library name is given (i.e., search for
+  exact match) and the case when library name has no suffix (i.e., search
+  for library with matching basename). (:issue:`8422`)
+* (Windows) Fix mangling of path to the entry-point script when the script
+  is in the current working directory, and the path to this directory
+  contains two or more consecutive ``$`` or ``%`` characters. (:issue:`8434`)
+
+
+Incompatible Changes
+~~~~~~~~~~~~~~~~~~~~
+
+* PyInstaller does not attempt to expand environment variables in paths
+  given via :option:`--workpath`, :option:`--distpath`, :option:`--specpath`,
+  and :option:`--additional-hooks-dir` anymore (note that other paths were
+  never subject to environment variable expansion in the first place).
+  Expansion of the starting tilde (``~``) into user's home directory is
+  still performed, as a work-around for tilde not being expanded by the
+  shell when passing arguments as ``--workpath=~/path/abc`` instead of
+  ``--workpath ~/path/abc``. (:issue:`8441`)
+
+
+Hooks
+~~~~~
+
+* Have ``sqlalchemy`` hook collect all dialects and plugins that are
+  registered via ``sqlalchemy.dialects`` and ``sqlalchemy.plugins``
+  entry-points. This ensures collection of 3rd party dialects and plugins
+  that may be available in the build environment (e.g., ``ibm-db-sa``).
+  (:issue:`8465`)
+* The ``pywin32-ctypes`` hook now always collects the
+  ``win32ctypes.core.ctypes``
+  modules, so that the ``ctypes`` backend is always available (i.e., even
+  if we also collect the ``cffi`` backend due to availability of ``cffi``
+  in the build environment). This fixes issues when ``cffi`` ends up
+  unavailable at run-time in spite of being available in the build environment
+  at build time (for example, due to explicit exclusion via
+  :option:`--exclude-module`
+  option). (:issue:`8544`)
+* Update ``pkg_resources`` hook for compatibility with ``setuptools`` v70.0.0
+  and later (fix ``ModuleNotFoundError: No module named
+  'pkg_resources.extern'``). (:issue:`8554`)
+
+
 6.6.0 (2024-04-13)
 ------------------
 
 Features
 ~~~~~~~~
 
 * (Windows) Implement support for resolving executable's true location
```

### Comparing `pyinstaller-6.6.0/doc/CREDITS.rst` & `pyinstaller-6.7.0/doc/CREDITS.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 Credits
 =======
 
 Thanks goes to all the kind PyInstaller contributors who have contributed
 new code, bug reports, fixes, comments and ideas. A brief list follows,
 please let us know if your name is omitted by accident:
 
+Contributions to PyInstaller 6.7.0
+----------------------------------
+
+* Rok Mandeljc
+* Brénainn Woodsend
+* Dan Yeaw
+
 Contributions to PyInstaller 6.6.0
 ----------------------------------
 
 * Rok Mandeljc
 * Brénainn Woodsend
 * Olliver Aikenhead
 * RoboSchmied
```

### Comparing `pyinstaller-6.6.0/doc/Makefile` & `pyinstaller-6.7.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/doc/_common_definitions.txt` & `pyinstaller-6.7.0/doc/_common_definitions.txt`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/doc/_static/CArchive.png` & `pyinstaller-6.7.0/doc/_static/CArchive.png`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/doc/_static/SE_exe.png` & `pyinstaller-6.7.0/doc/_static/SE_exe.png`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/doc/_static/ZlibArchive.png` & `pyinstaller-6.7.0/doc/_static/ZlibArchive.png`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/doc/_static/css/pyinstaller.css` & `pyinstaller-6.7.0/doc/_static/css/pyinstaller.css`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/doc/_static/pyinstaller-draft1a-100_trans.png` & `pyinstaller-6.7.0/doc/_static/pyinstaller-draft1a-100_trans.png`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/doc/_static/pyinstaller-draft1a.ico` & `pyinstaller-6.7.0/doc/_static/pyinstaller-draft1a.ico`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/doc/advanced-topics.rst` & `pyinstaller-6.7.0/doc/advanced-topics.rst`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/doc/bootloader-building.rst` & `pyinstaller-6.7.0/doc/bootloader-building.rst`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/doc/common-issues-and-pitfalls.rst` & `pyinstaller-6.7.0/doc/common-issues-and-pitfalls.rst`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/doc/conf.py` & `pyinstaller-6.7.0/doc/conf.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/doc/contributing.rst` & `pyinstaller-6.7.0/doc/contributing.rst`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/doc/development/branch-model.rst` & `pyinstaller-6.7.0/doc/development/branch-model.rst`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/doc/development/changelog-entries.rst` & `pyinstaller-6.7.0/doc/development/changelog-entries.rst`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/doc/development/coding-conventions.rst` & `pyinstaller-6.7.0/doc/development/coding-conventions.rst`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/doc/development/commit-messages.rst` & `pyinstaller-6.7.0/doc/development/commit-messages.rst`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/doc/development/documentation.rst` & `pyinstaller-6.7.0/doc/development/documentation.rst`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/doc/development/git.rst` & `pyinstaller-6.7.0/doc/development/git.rst`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/doc/development/pull-requests.rst` & `pyinstaller-6.7.0/doc/development/pull-requests.rst`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/doc/development/quickstart.rst` & `pyinstaller-6.7.0/doc/development/quickstart.rst`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/doc/development/testing.rst` & `pyinstaller-6.7.0/doc/development/testing.rst`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/doc/development/venv.rst` & `pyinstaller-6.7.0/doc/development/venv.rst`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/doc/feature-notes.rst` & `pyinstaller-6.7.0/doc/feature-notes.rst`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/doc/help2rst.py` & `pyinstaller-6.7.0/doc/help2rst.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/doc/hooks-config.rst` & `pyinstaller-6.7.0/doc/hooks-config.rst`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/doc/hooks.rst` & `pyinstaller-6.7.0/doc/hooks.rst`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/doc/index.rst` & `pyinstaller-6.7.0/doc/index.rst`

 * *Files 10% similar despite different names*

```diff
@@ -38,14 +38,19 @@
 
 .. code-block:: bash
 
     pyinstaller your_program.py
 
 Your bundled application should now be available in the `dist` folder.
 
+.. note::
+
+    See :ref:`pyinstaller_not_in_path` if you get some kind of *pyinstaller
+    command not found* error.
+
 
 Contents:
 _________
 
 .. toctree::
    :maxdepth: 2
```

### Comparing `pyinstaller-6.6.0/doc/installation.rst` & `pyinstaller-6.7.0/doc/installation.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,25 @@
 How to Install PyInstaller
 ===============================
 
 PyInstaller is available as a regular Python package.
-The source archives for released versions are available from PyPi_,
+The source archives for released versions are available from PyPI_,
 but it is easier to install the latest version using pip_::
 
     pip install pyinstaller
 
+.. note::
+
+    PyInstaller is split into two packages ``pyinstaller`` and
+    ``pyinstaller-hooks-contrib``. These should be kept approximately (roughly
+    within a year of each other) in sync. To that end, if you choose to pin your
+    ``pyinstaller`` version, please also pin ``pyinstaller-hooks-contrib``. If
+    you upgrade ``pyinstaller``, you will also need to upgrade
+    ``pyinstaller-hooks-contrib``.
+
 To upgrade existing PyInstaller installation to the latest version, use::
 
     pip install --upgrade pyinstaller
 
 To install the current development version, use::
 
     pip install https://github.com/pyinstaller/pyinstaller/tarball/develop
@@ -58,38 +67,41 @@
 
 For platforms other than Windows, GNU/Linux and macOS, you must first
 build the bootloader for your platform: see :ref:`Building the Bootloader`.
 After the bootloader has been built, use the ``pip install .`` command
 to complete the installation.
 
 
-Verifying the installation
-~~~~~~~~~~~~~~~~~~~~~~~~~~
+.. _`pyinstaller_not_in_path`:
+
+Troubleshooting missing PyInstaller command
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-On all platforms, the command ``pyinstaller`` should now exist on the
-execution path. To verify this, enter the command::
+In a properly setup Python environment, the command ``pyinstaller`` should now
+exist on the execution path and the command below should display PyInstaller's
+version. ::
 
     pyinstaller --version
 
-The result should resemble ``4.n`` for a released version,
-and ``4.n.dev0-xxxxxx`` for a development branch.
+If the command is not found, make sure that the ``PATH`` (the executable search
+path) environment variable includes the directory that the ``pyinstaller``
+executable was installed into.
+
+* On Windows, this location is either of the paths returned by::
+
+    import sysconfig; print(sysconfig.get_path("scripts"))
+    import site; print(site.USER_BASE + "\\Scripts")
 
-If the command is not found, make sure the execution path includes
-the proper directory:
+* On UNIX, this location is either of the paths returned by::
 
-* Windows: ``C:\PythonXY\Scripts`` where *XY* stands for the
-  major and minor Python version number,
-  for example ``C:\Python38\Scripts`` for Python 3.8)
-* GNU/Linux: ``/usr/bin/``
-* macOS (using the default Apple-supplied Python) ``/usr/bin``
-* macOS (using Python installed by homebrew) ``/usr/local/bin``
-* macOS (using Python installed by macports) ``/opt/local/bin``
+    import sysconfig; print(sysconfig.get_path("scripts"))
+    import site; print(site.USER_BASE + "/bin")
 
-To display the current path in Windows the command is ``echo %path%``
-and in other systems, ``echo $PATH``.
+To display the current path in Windows the command is ``echo %PATH%`` and on
+other systems, ``echo $PATH``.
 
 .. Note::
     If you cannot use the ``pyinstaller`` command due to the scripts
     directory not being in ``PATH``, you can instead invoke the
     ``PyInstaller`` module, by running ``python -m PyInstaller``
     (pay attention to the module name, which is case sensitive).
     This form of invocation is also useful when you have PyInstaller
```

### Comparing `pyinstaller-6.6.0/doc/license.rst` & `pyinstaller-6.7.0/doc/license.rst`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/doc/make.bat` & `pyinstaller-6.7.0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/doc/man/pyi-makespec.rst` & `pyinstaller-6.7.0/doc/man/pyi-makespec.rst`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/doc/man/pyinstaller.rst` & `pyinstaller-6.7.0/doc/man/pyinstaller.rst`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/doc/operating-mode.rst` & `pyinstaller-6.7.0/doc/operating-mode.rst`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/doc/pyi-makespec.1` & `pyinstaller-6.7.0/doc/pyi-makespec.1`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" Man page generated from reStructuredText.
 .
-.TH "PYI-MAKESPEC" "1" "2024-04-13" "6.6.0" "PyInstaller"
+.TH "PYI-MAKESPEC" "1" "2024-05-21" "6.7.0" "PyInstaller"
 .SH NAME
 pyi-makespec \- Create a spec file for your PyInstaller project
 .
 .nr rst2man-indent-level 0
 .
 .de1 rstReportMargin
 \\$1 \\n[an-margin]
@@ -231,15 +231,15 @@
 .B \-w\fP,\fB  \-\-windowed\fP,\fB  \-\-noconsole
 Windows and Mac OS X: do not provide a console window for standard i/o. On
 Mac OS this also triggers building a Mac OS .app bundle. On Windows this
 option is automatically set if the first script is a \(aq.pyw\(aq file. This
 option is ignored on *NIX systems.
 .UNINDENT
 .sp
-\-\-hide\-console {minimize\-late,minimize\-early,hide\-late,hide\-early}
+\-\-hide\-console {hide\-late,minimize\-late,minimize\-early,hide\-early}
 .INDENT 0.0
 .INDENT 3.5
 Windows only: in console\-enabled executable, have bootloader automatically
 hide or minimize the console window if the program owns the console window
 (i.e., was not launched from an existing console window).
 .UNINDENT
 .UNINDENT
```

### Comparing `pyinstaller-6.6.0/doc/pyinstaller.1` & `pyinstaller-6.7.0/doc/pyinstaller.1`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 .\" Man page generated from reStructuredText.
 .
-.TH "PYINSTALLER" "1" "2024-04-13" "6.6.0" "PyInstaller"
+.TH "PYINSTALLER" "1" "2024-05-21" "6.7.0" "PyInstaller"
 .SH NAME
 pyinstaller \- Configure and build a PyInstaller project in one run
 .
 .nr rst2man-indent-level 0
 .
 .de1 rstReportMargin
 \\$1 \\n[an-margin]
@@ -251,15 +251,15 @@
 .B \-w\fP,\fB  \-\-windowed\fP,\fB  \-\-noconsole
 Windows and Mac OS X: do not provide a console window for standard i/o. On
 Mac OS this also triggers building a Mac OS .app bundle. On Windows this
 option is automatically set if the first script is a \(aq.pyw\(aq file. This
 option is ignored on *NIX systems.
 .UNINDENT
 .sp
-\-\-hide\-console {minimize\-late,minimize\-early,hide\-late,hide\-early}
+\-\-hide\-console {hide\-late,minimize\-late,minimize\-early,hide\-early}
 .INDENT 0.0
 .INDENT 3.5
 Windows only: in console\-enabled executable, have bootloader automatically
 hide or minimize the console window if the program owns the console window
 (i.e., was not launched from an existing console window).
 .UNINDENT
 .UNINDENT
```

### Comparing `pyinstaller-6.6.0/doc/requirements.rst` & `pyinstaller-6.7.0/doc/requirements.rst`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/doc/requirements.txt` & `pyinstaller-6.7.0/doc/requirements.txt`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/doc/runtime-information.rst` & `pyinstaller-6.7.0/doc/runtime-information.rst`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/doc/spec-files.rst` & `pyinstaller-6.7.0/doc/spec-files.rst`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/doc/usage.rst` & `pyinstaller-6.7.0/doc/usage.rst`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/doc/when-things-go-wrong.rst` & `pyinstaller-6.7.0/doc/when-things-go-wrong.rst`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/icons/github_logo.png` & `pyinstaller-6.7.0/icons/github_logo.png`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/icons/icon-console.svg` & `pyinstaller-6.7.0/icons/icon-console.svg`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/icons/icon-windowed.svg` & `pyinstaller-6.7.0/icons/icon-windowed.svg`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/news/README.txt` & `pyinstaller-6.7.0/news/README.txt`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/news/_template.rst` & `pyinstaller-6.7.0/news/_template.rst`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/pyinstaller.egg-info/PKG-INFO` & `pyinstaller-6.7.0/pyinstaller.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyinstaller
-Version: 6.6.0
+Version: 6.7.0
 Summary: PyInstaller bundles a Python application and all its dependencies into a single package.
 Home-page: https://www.pyinstaller.org/
 Author: Hartmut Goebel, Giovanni Bajo, David Vierra, David Cortesi, Martin Zibricky
 License: GPLv2-or-later with a special exception which allows to use PyInstaller to build and distribute non-free programs (including commercial ones)
 Project-URL: Source, https://github.com/pyinstaller/pyinstaller
 Keywords: packaging, app, apps, bundle, convert, standalone, executable,pyinstaller, cxfreeze, freeze, py2exe, py2app, bbfreeze
 Classifier: Development Status :: 6 - Mature
@@ -42,15 +42,15 @@
 Description-Content-Type: text/x-rst
 License-File: COPYING.txt
 Requires-Dist: setuptools>=42.0.0
 Requires-Dist: altgraph
 Requires-Dist: pefile>=2022.5.30; sys_platform == "win32"
 Requires-Dist: pywin32-ctypes>=0.2.1; sys_platform == "win32"
 Requires-Dist: macholib>=1.8; sys_platform == "darwin"
-Requires-Dist: pyinstaller-hooks-contrib>=2024.3
+Requires-Dist: pyinstaller-hooks-contrib>=2024.6
 Requires-Dist: importlib_metadata>=4.6; python_version < "3.10"
 Requires-Dist: packaging>=22.0
 Provides-Extra: hook-testing
 Requires-Dist: pytest>=2.7.3; extra == "hook-testing"
 Requires-Dist: execnet>=1.5.0; extra == "hook-testing"
 Requires-Dist: psutil; extra == "hook-testing"
 Provides-Extra: completion
@@ -188,21 +188,21 @@
 pyinstaller`` provided that you have an appropriate C compiler (typically
 either ``gcc`` or ``clang``) and zlib's development headers already installed.
 
 
 Support
 -------
 
-- Official debugging guide: https://pyinstaller.org/en/v6.6.0/when-things-go-wrong.html
+- Official debugging guide: https://pyinstaller.org/en/v6.7.0/when-things-go-wrong.html
 - Assorted user contributed help topics: https://github.com/pyinstaller/pyinstaller/wiki
 - Web based Q&A forums: https://github.com/pyinstaller/pyinstaller/discussions
 - Email based Q&A forums: https://groups.google.com/g/pyinstaller
 
 
 Changes in this Release
 -----------------------
 
 You can find a detailed list of changes in this release
 in the `Changelog`_ section of the manual.
 
-.. _`manual`: https://pyinstaller.org/en/v6.6.0/
-.. _`Changelog`: https://pyinstaller.org/en/v6.6.0/CHANGES.html
+.. _`manual`: https://pyinstaller.org/en/v6.7.0/
+.. _`Changelog`: https://pyinstaller.org/en/v6.7.0/CHANGES.html
```

### Comparing `pyinstaller-6.6.0/pyinstaller.egg-info/SOURCES.txt` & `pyinstaller-6.7.0/pyinstaller.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 .github/ISSUE_TEMPLATE/config.yml
 .github/ISSUE_TEMPLATE/feature_request.md
 .github/workflows/cancel.yml
 .github/workflows/ci.yml
 .github/workflows/lint.yml
 .github/workflows/lock-threads.yml
 .github/workflows/validate-new-news.yml
+.github/workflows/viruscheck.yml
 .github/workflows/wheel-builder.yml
 PyInstaller/__init__.py
 PyInstaller/__main__.py
 PyInstaller/_recursion_too_deep_message.py
 PyInstaller/_shared_with_waf.py
 PyInstaller/compat.py
 PyInstaller/config.py
```

### Comparing `pyinstaller-6.6.0/pyproject.toml` & `pyinstaller-6.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/release/README.rst` & `pyinstaller-6.7.0/release/README.rst`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/scripts/find-empty-hooks.py` & `pyinstaller-6.7.0/scripts/find-empty-hooks.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/scripts/update-copyright` & `pyinstaller-6.7.0/scripts/update-copyright`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/scripts/verify-news-fragments.py` & `pyinstaller-6.7.0/scripts/verify-news-fragments.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/setup.cfg` & `pyinstaller-6.7.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 python_requires = >=3.8, <3.13
 install_requires = 
 	setuptools >= 42.0.0
 	altgraph
 	pefile >= 2022.5.30 ; sys_platform == 'win32'
 	pywin32-ctypes >= 0.2.1 ; sys_platform == 'win32'
 	macholib >= 1.8 ; sys_platform == 'darwin'
-	pyinstaller-hooks-contrib >= 2024.3
+	pyinstaller-hooks-contrib >= 2024.6
 	importlib_metadata >= 4.6 ; python_version < "3.10"
 	packaging >= 22.0
 
 [options.packages.find]
 include = 
 	PyInstaller
 	PyInstaller.*
```

### Comparing `pyinstaller-6.6.0/setup.py` & `pyinstaller-6.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/README.md` & `pyinstaller-6.7.0/tests/README.md`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/data/PIL_images/tinysample.tiff` & `pyinstaller-6.7.0/tests/functional/data/PIL_images/tinysample.tiff`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/data/Qt_Ui_file/gui.ui` & `pyinstaller-6.7.0/tests/functional/data/Qt_Ui_file/gui.ui`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/data/app_with_plugin/static_plugin.py` & `pyinstaller-6.7.0/tests/functional/data/app_with_plugin/static_plugin.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/data/appimage/AppIcon.svg` & `pyinstaller-6.7.0/tests/functional/data/appimage/AppIcon.svg`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/data/appimage/DirIcon.png` & `pyinstaller-6.7.0/tests/functional/data/appimage/DirIcon.png`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/data/appimage/create.sh` & `pyinstaller-6.7.0/tests/functional/data/appimage/create.sh`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/data/appimage/org.pyinstaller.appimage.test.appdata.xml` & `pyinstaller-6.7.0/tests/functional/data/appimage/org.pyinstaller.appimage.test.appdata.xml`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/data/ctypes_dylib/ctypes_dylib.c` & `pyinstaller-6.7.0/tests/functional/data/ctypes_dylib/ctypes_dylib.c`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/data/django/db.sqlite3` & `pyinstaller-6.7.0/tests/functional/data/django/db.sqlite3`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/data/django/django_site/settings.py` & `pyinstaller-6.7.0/tests/functional/data/django/django_site/settings.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/data/django/django_site/urls.py` & `pyinstaller-6.7.0/tests/functional/data/django/django_site/urls.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/data/django/manage.py` & `pyinstaller-6.7.0/tests/functional/data/django/manage.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/data/invalid_icon/pyi_icon.png` & `pyinstaller-6.7.0/tests/functional/data/invalid_icon/pyi_icon.png`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/data/requests/server.pem` & `pyinstaller-6.7.0/tests/functional/data/requests/server.pem`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/data/set_icon/pyi_icon.icns` & `pyinstaller-6.7.0/tests/functional/data/set_icon/pyi_icon.icns`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/data/set_icon/pyi_icon.ico` & `pyinstaller-6.7.0/tests/functional/data/set_icon/pyi_icon.ico`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/data/sphinx/conf.py` & `pyinstaller-6.7.0/tests/functional/data/sphinx/conf.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/data/splash/image.png` & `pyinstaller-6.7.0/tests/functional/data/splash/image.png`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/modules/error_during_import2.py` & `pyinstaller-6.7.0/tests/functional/modules/error_during_import2.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/modules/module_with_coding_utf8.py` & `pyinstaller-6.7.0/tests/functional/modules/module_with_coding_utf8.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/modules/module_with_utf8_emoji.py` & `pyinstaller-6.7.0/tests/functional/modules/module_with_utf8_emoji.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/modules/nspkg1-pkg/nspkg1_bbb.egg` & `pyinstaller-6.7.0/tests/functional/modules/nspkg1-pkg/nspkg1_bbb.egg`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/modules/nspkg1-pkg/nspkg1_empty.egg` & `pyinstaller-6.7.0/tests/functional/modules/nspkg1-pkg/nspkg1_empty.egg`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/modules/nspkg2-pkg/nspkg2_bbb-nspkg.pth` & `pyinstaller-6.7.0/tests/functional/modules/nspkg2-pkg/nspkg2_bbb-nspkg.pth`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/modules/nspkg3-pkg/nspkg3_bbb.egg` & `pyinstaller-6.7.0/tests/functional/modules/nspkg3-pkg/nspkg3_bbb.egg`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/modules/nspkg3-pkg/nspkg3_empty.egg` & `pyinstaller-6.7.0/tests/functional/modules/nspkg3-pkg/nspkg3_empty.egg`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/modules/pyi_collect_submodules_mod.py` & `pyinstaller-6.7.0/tests/functional/modules/pyi_collect_submodules_mod.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/modules/pyi_egg_zipped.egg` & `pyinstaller-6.7.0/tests/functional/modules/pyi_egg_zipped.egg`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/modules/pyi_excluded_relative_imports/mypackage/__init__.py` & `pyinstaller-6.7.0/tests/functional/modules/pyi_excluded_relative_imports/mypackage/__init__.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/modules/pyi_excluded_relative_imports/mypackage/subpkg1/__init__.py` & `pyinstaller-6.7.0/tests/functional/modules/pyi_excluded_relative_imports/mypackage/subpkg1/__init__.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/modules/pyi_excluded_relative_imports/mypackage/subpkg1/subpkg2/__init__.py` & `pyinstaller-6.7.0/tests/functional/modules/pyi_excluded_relative_imports/mypackage/subpkg1/subpkg2/__init__.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/modules/pyi_get_datadir.py` & `pyinstaller-6.7.0/tests/functional/modules/pyi_get_datadir.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/modules/pyi_module_exclusion/modules/mymodule_main/__init__.py` & `pyinstaller-6.7.0/tests/functional/modules/pyi_module_exclusion/modules/mymodule_main/__init__.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/modules/pyi_module_with_invalid_encoding/mymodule1.py` & `pyinstaller-6.7.0/tests/functional/modules/pyi_module_with_invalid_encoding/mymodule1.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/modules/pyi_module_with_invalid_encoding/mymodule2.py` & `pyinstaller-6.7.0/tests/functional/modules/pyi_module_with_invalid_encoding/mymodule2.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/modules/pyi_optimization/mypackage/__init__.py` & `pyinstaller-6.7.0/tests/functional/modules/pyi_optimization/mypackage/__init__.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/modules/pyi_pkg_resources_provider/hooks/hook-pyi_pkgres_testpkg.py` & `pyinstaller-6.7.0/tests/functional/modules/pyi_pkg_resources_provider/hooks/hook-pyi_pkgres_testpkg.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/modules/pyi_pkg_resources_provider/package/setup.py` & `pyinstaller-6.7.0/tests/functional/modules/pyi_pkg_resources_provider/package/setup.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/modules/pyi_pkgutil_itermodules/hooks/hook-mypackage.py` & `pyinstaller-6.7.0/tests/functional/modules/pyi_pkgutil_itermodules/hooks/hook-mypackage.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/modules/pyi_test_egg/pyi_egg_unzipped.egg/unzipped_egg/__init__.py` & `pyinstaller-6.7.0/tests/functional/modules/pyi_test_egg/pyi_egg_unzipped.egg/unzipped_egg/__init__.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_dynamic.py` & `pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_dynamic.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_gettemp.py` & `pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_gettemp.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_metapath1/__init__.py` & `pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_metapath1/__init__.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_metapath1/_vendor/aaa.py` & `pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_metapath1/_vendor/aaa.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_metapath1/_vendor/bbb.py` & `pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_metapath1/_vendor/bbb.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_metapath1/_vendor/ccc/ddd.py` & `pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_metapath1/_vendor/ccc/ddd.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_metapath1/_vendor/ccc/eee/fff.py` & `pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_metapath1/_vendor/ccc/eee/fff.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_metapath1/extern/__init__.py` & `pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_metapath1/extern/__init__.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_path/__init__.py` & `pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_path/__init__.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_path/b.py` & `pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_path/b.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_relimp/B/C.py` & `pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_relimp/B/C.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_relimp/B/D.py` & `pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_relimp/B/D.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_relimp/B/__init__.py` & `pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_relimp/B/__init__.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_relimp/E.py` & `pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_relimp/E.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_relimp/F/G.py` & `pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_relimp/F/G.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_relimp/F/__init__.py` & `pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_relimp/F/__init__.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_relimp/__init__.py` & `pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_relimp/__init__.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_relimp/pyi_testmod_relimp/__init__.py` & `pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_relimp/pyi_testmod_relimp/__init__.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_relimp/pyi_testmod_relimp/relimp2.py` & `pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_relimp/pyi_testmod_relimp/relimp2.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_relimp/pyi_testmod_relimp/relimp3.py` & `pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_relimp/pyi_testmod_relimp/relimp3.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_relimp/relimp1.py` & `pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_relimp/relimp1.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_relimp/relimp2.py` & `pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_relimp/relimp2.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_relimp2/bar/__init__.py` & `pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_relimp2/bar/__init__.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_relimp2/bar/bar2/__init__.py` & `pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_relimp2/bar/bar2/__init__.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_relimp2/bar/baz.py` & `pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_relimp2/bar/baz.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_relimp3a/aa/a1.py` & `pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_relimp3a/aa/a1.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_relimp3a/aa/pyi_testmod_relimp3c.py` & `pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_relimp3a/aa/pyi_testmod_relimp3c.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_relimp3a/pyi_testmod_relimp3b/b1.py` & `pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_relimp3a/pyi_testmod_relimp3b/b1.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_relimp3a/pyi_testmod_relimp3c.py` & `pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_relimp3a/pyi_testmod_relimp3c.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_relimp3b/b1.py` & `pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_relimp3b/b1.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_relimp3c/__init__.py` & `pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_relimp3c/__init__.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_submodule_global_shadowed/__init__.py` & `pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_submodule_global_shadowed/__init__.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_submodule_global_shadowed/submodule.py` & `pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_submodule_global_shadowed/submodule.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_submodule_global_unshadowed/__init__.py` & `pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_submodule_global_unshadowed/__init__.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_submodule_global_unshadowed/submodule.py` & `pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_submodule_global_unshadowed/submodule.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/modules/pyi_testmod_threading.py` & `pyinstaller-6.7.0/tests/functional/modules/pyi_testmod_threading.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/modules/resources_testmod.py` & `pyinstaller-6.7.0/tests/functional/modules/resources_testmod.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/scripts/list_pytest11_entry_point.py` & `pyinstaller-6.7.0/tests/functional/scripts/list_pytest11_entry_point.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/scripts/pkg_resource_res_string.py` & `pyinstaller-6.7.0/tests/functional/scripts/pkg_resource_res_string.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/scripts/pkgutil_get_data.py` & `pyinstaller-6.7.0/tests/functional/scripts/pkgutil_get_data.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/scripts/pkgutil_get_data__main__.py` & `pyinstaller-6.7.0/tests/functional/scripts/pkgutil_get_data__main__.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/scripts/pyi_absolute_ld_library_path.py` & `pyinstaller-6.7.0/tests/functional/scripts/pyi_absolute_ld_library_path.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/scripts/pyi_absolute_python_path.py` & `pyinstaller-6.7.0/tests/functional/scripts/pyi_absolute_python_path.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/scripts/pyi_app_with_plugin.py` & `pyinstaller-6.7.0/tests/functional/scripts/pyi_app_with_plugin.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/scripts/pyi_c_extension.py` & `pyinstaller-6.7.0/tests/functional/scripts/pyi_c_extension.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/scripts/pyi_codecs.py` & `pyinstaller-6.7.0/tests/functional/scripts/pyi_codecs.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/scripts/pyi_filename.py` & `pyinstaller-6.7.0/tests/functional/scripts/pyi_filename.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/scripts/pyi_frozen_stdlib_modules.py` & `pyinstaller-6.7.0/tests/functional/scripts/pyi_frozen_stdlib_modules.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/scripts/pyi_future.py` & `pyinstaller-6.7.0/tests/functional/scripts/pyi_future.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/scripts/pyi_get_meipass_value.py` & `pyinstaller-6.7.0/tests/functional/scripts/pyi_get_meipass_value.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/scripts/pyi_getfilesystemencoding.py` & `pyinstaller-6.7.0/tests/functional/scripts/pyi_getfilesystemencoding.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/scripts/pyi_helloworld.py` & `pyinstaller-6.7.0/tests/functional/scripts/pyi_helloworld.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/scripts/pyi_hooks/hook-pyi_collect_submodules_mod.py` & `pyinstaller-6.7.0/tests/functional/scripts/pyi_hooks/hook-pyi_collect_submodules_mod.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/scripts/pyi_hooks/hook-pyi_testmod_metapath1.py` & `pyinstaller-6.7.0/tests/functional/scripts/pyi_hooks/hook-pyi_testmod_metapath1.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/scripts/pyi_hooks/hook-pyi_testmod_path.py` & `pyinstaller-6.7.0/tests/functional/scripts/pyi_hooks/hook-pyi_testmod_path.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/scripts/pyi_hooks/pre_safe_import_module/hook-alias_name.py` & `pyinstaller-6.7.0/tests/functional/scripts/pyi_hooks/pre_safe_import_module/hook-alias_name.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/scripts/pyi_import_pyqt5_uic_port.py` & `pyinstaller-6.7.0/tests/functional/scripts/pyi_import_pyqt5_uic_port.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/scripts/pyi_importlib_resources.py` & `pyinstaller-6.7.0/tests/functional/scripts/pyi_importlib_resources.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/scripts/pyi_interact_pyi_splash.py` & `pyinstaller-6.7.0/tests/functional/scripts/pyi_interact_pyi_splash.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/scripts/pyi_issue_4141.py` & `pyinstaller-6.7.0/tests/functional/scripts/pyi_issue_4141.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/scripts/pyi_lazy_import.py` & `pyinstaller-6.7.0/tests/functional/scripts/pyi_lazy_import.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/scripts/pyi_lib_PIL_img_conversion.py` & `pyinstaller-6.7.0/tests/functional/scripts/pyi_lib_PIL_img_conversion.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/scripts/pyi_lib_PyQt5-uic.py` & `pyinstaller-6.7.0/tests/functional/scripts/pyi_lib_PyQt5-uic.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/scripts/pyi_lib_requests.py` & `pyinstaller-6.7.0/tests/functional/scripts/pyi_lib_requests.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/scripts/pyi_lib_sphinx.py` & `pyinstaller-6.7.0/tests/functional/scripts/pyi_lib_sphinx.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/scripts/pyi_lib_tkinter.py` & `pyinstaller-6.7.0/tests/functional/scripts/pyi_lib_tkinter.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/scripts/pyi_load_dll_using_ctypes.py` & `pyinstaller-6.7.0/tests/functional/scripts/pyi_load_dll_using_ctypes.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/scripts/pyi_module__file__attribute.py` & `pyinstaller-6.7.0/tests/functional/scripts/pyi_module__file__attribute.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/scripts/pyi_module_attributes.py` & `pyinstaller-6.7.0/tests/functional/scripts/pyi_module_attributes.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/scripts/pyi_module_reload.py` & `pyinstaller-6.7.0/tests/functional/scripts/pyi_module_reload.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/scripts/pyi_multiprocessing_main_module_code_in_process.py` & `pyinstaller-6.7.0/tests/functional/scripts/pyi_multiprocessing_main_module_code_in_process.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/scripts/pyi_multiprocessing_nested_process.py` & `pyinstaller-6.7.0/tests/functional/scripts/pyi_multiprocessing_nested_process.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/scripts/pyi_multiprocessing_pool.py` & `pyinstaller-6.7.0/tests/functional/scripts/pyi_multiprocessing_pool.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/scripts/pyi_multiprocessing_process.py` & `pyinstaller-6.7.0/tests/functional/scripts/pyi_multiprocessing_process.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/scripts/pyi_multiprocessing_process_start_in_threads.py` & `pyinstaller-6.7.0/tests/functional/scripts/pyi_multiprocessing_process_start_in_threads.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/scripts/pyi_multiprocessing_queue.py` & `pyinstaller-6.7.0/tests/functional/scripts/pyi_multiprocessing_queue.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/scripts/pyi_multiprocessing_semaphore.py` & `pyinstaller-6.7.0/tests/functional/scripts/pyi_multiprocessing_semaphore.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/scripts/pyi_optimization.py` & `pyinstaller-6.7.0/tests/functional/scripts/pyi_optimization.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/scripts/pyi_osx_aevent_logger_carbon.py` & `pyinstaller-6.7.0/tests/functional/scripts/pyi_osx_aevent_logger_carbon.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/scripts/pyi_path_encoding.py` & `pyinstaller-6.7.0/tests/functional/scripts/pyi_path_encoding.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/scripts/pyi_pkg_resources_provider.py` & `pyinstaller-6.7.0/tests/functional/scripts/pyi_pkg_resources_provider.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/scripts/pyi_pkgutil_iter_modules.py` & `pyinstaller-6.7.0/tests/functional/scripts/pyi_pkgutil_iter_modules.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/scripts/pyi_python_home.py` & `pyinstaller-6.7.0/tests/functional/scripts/pyi_python_home.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/scripts/pyi_site_module_disabled.py` & `pyinstaller-6.7.0/tests/functional/scripts/pyi_site_module_disabled.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/scripts/pyi_stderr_encoding.py` & `pyinstaller-6.7.0/tests/functional/scripts/pyi_stderr_encoding.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/scripts/pyi_stdout_encoding.py` & `pyinstaller-6.7.0/tests/functional/scripts/pyi_stdout_encoding.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/scripts/pyi_symlink_basename_is_kept.py` & `pyinstaller-6.7.0/tests/functional/scripts/pyi_symlink_basename_is_kept.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/scripts/pyi_symlinks_test.py` & `pyinstaller-6.7.0/tests/functional/scripts/pyi_symlinks_test.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/scripts/pyi_threading_module2.py` & `pyinstaller-6.7.0/tests/functional/scripts/pyi_threading_module2.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/scripts/pyi_unbuffered_output.py` & `pyinstaller-6.7.0/tests/functional/scripts/pyi_unbuffered_output.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/scripts/pyi_win_py3_no_shortpathname.py` & `pyinstaller-6.7.0/tests/functional/scripts/pyi_win_py3_no_shortpathname.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/specs/list_pytest11_entry_point.spec` & `pyinstaller-6.7.0/tests/functional/specs/list_pytest11_entry_point.spec`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/specs/multipackage-scripts/extra-hooks/hook-multipackage_test_pkg.py` & `pyinstaller-6.7.0/tests/functional/specs/multipackage-scripts/extra-hooks/hook-multipackage_test_pkg.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/specs/multipackage-scripts/multipackage1_B.py` & `pyinstaller-6.7.0/tests/functional/specs/multipackage-scripts/multipackage1_B.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/specs/multipackage-scripts/multipackage2_B.py` & `pyinstaller-6.7.0/tests/functional/specs/multipackage-scripts/multipackage2_B.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/specs/multipackage-scripts/multipackage3_B.py` & `pyinstaller-6.7.0/tests/functional/specs/multipackage-scripts/multipackage3_B.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/specs/multipackage-scripts/multipackage4_B.py` & `pyinstaller-6.7.0/tests/functional/specs/multipackage-scripts/multipackage4_B.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/specs/multipackage-scripts/multipackage5_B.py` & `pyinstaller-6.7.0/tests/functional/specs/multipackage-scripts/multipackage5_B.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/specs/multipackage-scripts/multipackage5_C.py` & `pyinstaller-6.7.0/tests/functional/specs/multipackage-scripts/multipackage5_C.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/specs/multipackage-scripts/multipackage_test_pkg/__init__.py` & `pyinstaller-6.7.0/tests/functional/specs/multipackage-scripts/multipackage_test_pkg/__init__.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/specs/multipackage-scripts/test_multipackage1.py` & `pyinstaller-6.7.0/tests/functional/specs/multipackage-scripts/test_multipackage1.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/specs/multipackage-scripts/test_multipackage2.py` & `pyinstaller-6.7.0/tests/functional/specs/multipackage-scripts/test_multipackage2.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/specs/multipackage-scripts/test_multipackage3.py` & `pyinstaller-6.7.0/tests/functional/specs/multipackage-scripts/test_multipackage3.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/specs/multipackage-scripts/test_multipackage4.py` & `pyinstaller-6.7.0/tests/functional/specs/multipackage-scripts/test_multipackage4.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/specs/multipackage-scripts/test_multipackage5.py` & `pyinstaller-6.7.0/tests/functional/specs/multipackage-scripts/test_multipackage5.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/specs/pyi_osx_aevent_handling_carbon.spec` & `pyinstaller-6.7.0/tests/functional/specs/pyi_osx_aevent_handling_carbon.spec`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/specs/pyi_osx_override_info_plist.spec` & `pyinstaller-6.7.0/tests/functional/specs/pyi_osx_override_info_plist.spec`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/specs/pyi_spec_options.spec` & `pyinstaller-6.7.0/tests/functional/specs/pyi_spec_options.spec`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/specs/pyi_unbuffered_output.spec` & `pyinstaller-6.7.0/tests/functional/specs/pyi_unbuffered_output.spec`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/specs/several-scripts1.spec` & `pyinstaller-6.7.0/tests/functional/specs/several-scripts1.spec`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/specs/several-scripts2.spec` & `pyinstaller-6.7.0/tests/functional/specs/several-scripts2.spec`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/specs/spec-with-utf8.spec` & `pyinstaller-6.7.0/tests/functional/specs/spec-with-utf8.spec`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/specs/spec_with_splash.spec` & `pyinstaller-6.7.0/tests/functional/specs/spec_with_splash.spec`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/specs/symlink_basename_is_kept.spec` & `pyinstaller-6.7.0/tests/functional/specs/symlink_basename_is_kept.spec`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/specs/test_multipackage1.spec` & `pyinstaller-6.7.0/tests/functional/specs/test_multipackage1.spec`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/specs/test_multipackage2.spec` & `pyinstaller-6.7.0/tests/functional/specs/test_multipackage2.spec`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/specs/test_multipackage3.spec` & `pyinstaller-6.7.0/tests/functional/specs/test_multipackage3.spec`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/specs/test_multipackage4.spec` & `pyinstaller-6.7.0/tests/functional/specs/test_multipackage4.spec`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/specs/test_multipackage5.spec` & `pyinstaller-6.7.0/tests/functional/specs/test_multipackage5.spec`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/test_apple_events.py` & `pyinstaller-6.7.0/tests/functional/test_apple_events.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/test_basic.py` & `pyinstaller-6.7.0/tests/functional/test_basic.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/test_binary_vs_data_reclassification.py` & `pyinstaller-6.7.0/tests/functional/test_binary_vs_data_reclassification.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/test_cliutils.py` & `pyinstaller-6.7.0/tests/functional/test_cliutils.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/test_django.py` & `pyinstaller-6.7.0/tests/functional/test_django.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/test_hook_utilities.py` & `pyinstaller-6.7.0/tests/functional/test_hook_utilities.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/test_hooks/test_gi.py` & `pyinstaller-6.7.0/tests/functional/test_hooks/test_gi.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/test_hooks/test_matplotlib.py` & `pyinstaller-6.7.0/tests/functional/test_hooks/test_matplotlib.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/test_hooks/test_pil.py` & `pyinstaller-6.7.0/tests/functional/test_hooks/test_pil.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/test_hooks/test_pkg_resources.py` & `pyinstaller-6.7.0/tests/functional/test_hooks/test_pkg_resources.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/test_hooks/test_scipy.py` & `pyinstaller-6.7.0/tests/functional/test_hooks/test_scipy.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/test_hooks/test_six.py` & `pyinstaller-6.7.0/tests/functional/test_hooks/test_six.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/test_import.py` & `pyinstaller-6.7.0/tests/functional/test_import.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/test_import_lazy_loader.py` & `pyinstaller-6.7.0/tests/functional/test_import_lazy_loader.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/test_import_pep302.py` & `pyinstaller-6.7.0/tests/functional/test_import_pep302.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/test_importlib_resources.py` & `pyinstaller-6.7.0/tests/functional/test_importlib_resources.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/test_interactive.py` & `pyinstaller-6.7.0/tests/functional/test_interactive.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/test_libraries.py` & `pyinstaller-6.7.0/tests/functional/test_libraries.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/test_linux_appimage.py` & `pyinstaller-6.7.0/tests/functional/test_linux_appimage.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/test_macos_bundle_structure.py` & `pyinstaller-6.7.0/tests/functional/test_macos_bundle_structure.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/test_misc.py` & `pyinstaller-6.7.0/tests/functional/test_misc.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/test_module_exclusion.py` & `pyinstaller-6.7.0/tests/functional/test_module_exclusion.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/test_multipackage.py` & `pyinstaller-6.7.0/tests/functional/test_multipackage.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/test_multiprocessing.py` & `pyinstaller-6.7.0/tests/functional/test_multiprocessing.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/test_path_encodings.py` & `pyinstaller-6.7.0/tests/functional/test_path_encodings.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/test_pkg_resources_provider.py` & `pyinstaller-6.7.0/tests/functional/test_pkg_resources_provider.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/test_pkgutil.py` & `pyinstaller-6.7.0/tests/functional/test_pkgutil.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/test_pywin32.py` & `pyinstaller-6.7.0/tests/functional/test_pywin32.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/test_qt.py` & `pyinstaller-6.7.0/tests/functional/test_qt.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,20 +16,14 @@
 
 from PyInstaller import isolated
 from PyInstaller.compat import is_win, is_darwin, is_linux
 from PyInstaller.utils.hooks import check_requirement, can_import_module
 from PyInstaller.utils.hooks.qt import get_qt_library_info
 from PyInstaller.utils.tests import importorskip, requires, skipif
 
-PYQT5_NEED_OPENGL = pytest.mark.skipif(
-    check_requirement('PyQt5 <= 5.10.1'),
-    reason='PyQt5 v5.10.1 and older does not package ``opengl32sw.dll``, '
-    'the OpenGL software renderer, which this test requires.'
-)
-
 
 def qt_param(qt_flavor, *args, **kwargs):
     """
     A Qt flavour to be used in @pytest.mark.parametrize(). Implicitly skips the test if said flavor is not installed.
     """
     p = pytest.param(qt_flavor, *args, **kwargs)
     return pytest.param(*p.values, marks=(requires(qt_flavor),) + p.marks, id=p.id)
@@ -91,17 +85,27 @@
         else:
             res = app.exec_()
         sys.exit(res)
         """.format(QtPyLib), **USE_WINDOWED_KWARG
     )
 
 
-@PYQT5_NEED_OPENGL
 @QtPyLibs
 def test_Qt_QtQml(pyi_builder, QtPyLib):
+    # Qt6 6.6.3 split Qt Quick Controls 2 styles into separate shared libraries, and both PySide6 6.6.3 and PyQt6 6.6.3
+    # PyPI wheels failed to account for that. Skip this test if running with affected version.
+    if QtPyLib == 'PyQt6':
+        # With PyQt6, the shared libraries are missing on Windows and Linux, but not on macOS.
+        if not is_darwin and check_requirement('PyQt6-Qt6 == 6.6.3'):
+            pytest.skip('PyQt6-Qt6 6.6.3 is missing shared libraries required by Qt Quick Controls 2.')
+    if QtPyLib == 'PySide6':
+        # With PySide6, all OSes seem to be affected.
+        if check_requirement('PySide6-Essentials == 6.6.3'):
+            pytest.skip('PySide6-Essentials 6.6.3 is missing shared libraries required by Qt Quick Controls 2.')
+
     pyi_builder.test_source(
         """
         import sys
 
         from {0}.QtGui import QGuiApplication
         from {0}.QtQml import QQmlApplicationEngine
         from {0}.QtCore import QTimer, QUrl
@@ -239,15 +243,14 @@
         else:
             print('Qt locale %s not found!' % locale.name())
             assert False
         """.format(QtPyLib)
     )
 
 
-@PYQT5_NEED_OPENGL
 @QtPyLibs
 def test_Qt_Ui_file(tmpdir, pyi_builder, data_dir, QtPyLib):
     # Note that including the data_dir fixture copies files needed by this test.
     pyi_builder.test_source(
         """
         import os
         import sys
@@ -537,17 +540,21 @@
 def test_Qt_QtWebEngineWidgets_PyQt6(pyi_builder):
     _test_Qt_QtWebEngineWidgets(pyi_builder, 'PyQt6')
 
 
 @requires('PyQt6 >= 6.2.2')
 @requires('PyQt6-WebEngine')  # NOTE: base Qt6 must be 6.2.2 or newer, QtWebEngine can be older
 @pytest.mark.skipif(
-    check_requirement('PyQt6 == 6.6.0'),
+    check_requirement('PyQt6-Qt6 == 6.6.0'),
     reason='PyQt6 6.6.0 PyPI wheels are missing Qt6WebChannelQuick shared library.'
 )
+@pytest.mark.skipif(
+    check_requirement('PyQt6-Qt6 == 6.6.3') and is_win,
+    reason='PyQt6 6.6.3 PyPI wheels for Windows are missing Qt6WebChannelQuick shared library.'
+)
 def test_Qt_QtWebEngineQuick_PyQt6(pyi_builder):
     _test_Qt_QtWebEngineQuick(pyi_builder, 'PyQt6')
 
 
 @requires('PySide6 >= 6.2.2')
 @pytest.mark.skipif(
     check_requirement('PySide6 == 6.5.0') and is_win,
```

### Comparing `pyinstaller-6.6.0/tests/functional/test_regression.py` & `pyinstaller-6.7.0/tests/functional/test_regression.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/test_runtime.py` & `pyinstaller-6.7.0/tests/functional/test_runtime.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/test_signals.py` & `pyinstaller-6.7.0/tests/functional/test_signals.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/test_symlinks.py` & `pyinstaller-6.7.0/tests/functional/test_symlinks.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/functional/test_unbuffered_stdio.py` & `pyinstaller-6.7.0/tests/functional/test_unbuffered_stdio.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,18 +16,14 @@
 import asyncio
 
 import pytest
 
 from PyInstaller.compat import is_win
 
 
-@pytest.mark.skipif(
-    os.environ.get('CI', 'false').lower() == 'true',
-    reason="The test does not support CI (pytest-xdist sometimes runs it in secondary thread)."
-)
 @pytest.mark.parametrize('stream_mode', ['binary', 'text'])
 @pytest.mark.parametrize('output_stream', ['stdout', 'stderr'])
 def test_unbuffered_stdio(tmp_path, output_stream, stream_mode, pyi_builder_spec):
     # Freeze the test program; test_spec() builds the app and runs it, so explicitly set the number of
     # stars to 0 for this run.
     pyi_builder_spec.test_spec('pyi_unbuffered_output.spec', app_args=['--num-stars', '0'])
```

### Comparing `pyinstaller-6.6.0/tests/requirements-base.txt` & `pyinstaller-6.7.0/tests/requirements-base.txt`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/requirements-developer.txt` & `pyinstaller-6.7.0/tests/requirements-developer.txt`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/requirements-libraries.txt` & `pyinstaller-6.7.0/tests/requirements-libraries.txt`

 * *Files 22% similar despite different names*

```diff
@@ -11,26 +11,26 @@
 # Backport of importlib.resources for python 3.8 and earlier.
 importlib_resources==6.4.0; python_version < '3.9'
 
 
 # Working
 # -------
 # These packages work with no (known) issues.
-babel==2.14.0
-Django==5.0.4; python_version >= '3.10'
+babel==2.15.0
+Django==5.0.6; python_version >= '3.10'
 future==1.0.0
 gevent==24.2.1
-ipython==8.23.0; python_version >= '3.10'
+ipython==8.24.0; python_version >= '3.10'
 # keyring >= 23.1 requires python >= 3.8.7 on macOS 11 and later (with dyld shared cache support)
 keyring==23.0.1; sys_platform == 'darwin' and python_version < '3.8.7'  # pyup: ignore
-keyring==25.1.0; sys_platform != 'darwin' or python_version >= '3.8.7'
-matplotlib==3.8.4; python_version >= '3.9'
+keyring==25.2.1; sys_platform != 'darwin' or python_version >= '3.8.7'
+matplotlib==3.9.0; python_version >= '3.9'
 numpy==1.26.4; python_version >= '3.9'
-pandas==2.2.1; python_version >= '3.9'
-pygments==2.17.2
+pandas==2.2.2; python_version >= '3.9'
+pygments==2.18.0
 PyGObject==3.48.2; sys_platform == 'linux'
 # Official PySide2 wheels do not support python 3.11 or newer
 PySide2==5.15.2.1; python_version < '3.11'
 # PySide6 is a metapackage that depends on PySide6-Essentials and PySide6-Addons. Their versions are
 # usually kept in sync.
 PySide6==6.7.0; python_version >= '3.9'
 PySide6-Addons==6.7.0; python_version >= '3.9'
@@ -48,37 +48,42 @@
 QScintilla==2.14.1
 PyQtWebEngine==5.15.6
 # PyQt6 and add-on packages
 # The *-Qt6 packages contain Qt shared libraries; their version is therefore the version of Qt release,
 # but in contrast to Qt5 and PyQt5 bindings, the versions here must usually be kept in sync with the
 # version of corresponding PyQt bindings packages. That is because Qt6 is under active development, and
 # thus the ABI is still changing.
-PyQt6==6.6.1
-PyQt6-Qt6==6.6.2
-PyQt6-3D==6.6.0
-PyQt6-3D-Qt6==6.6.2
-PyQt6-Charts==6.6.0
-PyQt6-Charts-Qt6==6.6.2
-PyQt6-DataVisualization==6.6.0
-PyQt6-DataVisualization-Qt6==6.6.2
-PyQt6-NetworkAuth==6.6.0
-PyQt6-NetworkAuth-Qt6==6.6.2
+PyQt6==6.7.0
+PyQt6-Qt6==6.7.0
+PyQt6-3D==6.7.0
+PyQt6-3D-Qt6==6.7.0
+PyQt6-Charts==6.7.0
+PyQt6-Charts-Qt6==6.7.0
+PyQt6-DataVisualization==6.7.0
+PyQt6-DataVisualization-Qt6==6.7.0
+PyQt6-NetworkAuth==6.7.0
+PyQt6-NetworkAuth-Qt6==6.7.0
 PyQt6-QScintilla==2.14.1  # Does not have a corresponding -Qt6 package
-PyQt6-WebEngine==6.6.0
-PyQt6-WebEngine-Qt6==6.6.2
+# At the time of writing, x86_64 macOS wheel for PyQt6-WebEngine-Qt6 6.7.0 is missing due to its size
+# exceeding the size limit on PyPI. Work around this by using 6.6.x series for macOS x86_64.
+# TODO: remove this split once the wheel situation is sorted out on PyPI.
+PyQt6-WebEngine==6.7.0; sys_platform != 'darwin' or platform_machine != 'x86_64'
+PyQt6-WebEngine-Qt6==6.7.0; sys_platform != 'darwin' or platform_machine != 'x86_64'
+PyQt6-WebEngine==6.6.0; sys_platform == 'darwin' and platform_machine == 'x86_64'  # pyup: ignore
+PyQt6-WebEngine-Qt6==6.6.3; sys_platform == 'darwin' and platform_machine == 'x86_64'  # pyup: ignore
 python-dateutil==2.9.0.post0
 pytz==2024.1
 requests==2.31.0
 scipy==1.13.0; python_version >= '3.9'
 # simplejson is used for text_c_extension
 simplejson==3.19.2
-sphinx==7.2.6; python_version >= '3.9'
+sphinx==7.3.7; python_version >= '3.9'
 # Required for test_namespace_package
-sqlalchemy==2.0.29
-zope.interface==6.2
+sqlalchemy==2.0.30
+zope.interface==6.4
 Pillow==10.3.0
 
 
 # Python versions not supported / supported for older package versions
 # -------------------------------------------------------
 
 numpy==1.24.3; python_version == '3.8'  # pyup: ignore
```

### Comparing `pyinstaller-6.6.0/tests/requirements-tools.txt` & `pyinstaller-6.7.0/tests/requirements-tools.txt`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/scripts/Dockerfile` & `pyinstaller-6.7.0/tests/scripts/Dockerfile`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/scripts/check-pefile-arch.py` & `pyinstaller-6.7.0/tests/scripts/check-pefile-arch.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/scripts/eggs4testing/build-nspkg-tests.py` & `pyinstaller-6.7.0/tests/scripts/eggs4testing/build-nspkg-tests.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/scripts/eggs4testing/make.sh` & `pyinstaller-6.7.0/tests/scripts/eggs4testing/make.sh`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/scripts/eggs4testing/setup-unzipped.py` & `pyinstaller-6.7.0/tests/scripts/eggs4testing/setup-unzipped.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/scripts/eggs4testing/setup-zipped.py` & `pyinstaller-6.7.0/tests/scripts/eggs4testing/setup-zipped.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/scripts/eggs4testing/unzipped_egg/__init__.py` & `pyinstaller-6.7.0/tests/scripts/eggs4testing/unzipped_egg/__init__.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/scripts/eggs4testing/zipped_egg/__init__.py` & `pyinstaller-6.7.0/tests/scripts/eggs4testing/zipped_egg/__init__.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/scripts/test-cliutils.sh` & `pyinstaller-6.7.0/tests/scripts/test-cliutils.sh`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/scripts/test-docker.sh` & `pyinstaller-6.7.0/tests/scripts/test-docker.sh`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/speed/speed_pefile.py` & `pyinstaller-6.7.0/tests/speed/speed_pefile.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/unit/conftest.py` & `pyinstaller-6.7.0/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/unit/hookutils_files/setup.py` & `pyinstaller-6.7.0/tests/unit/hookutils_files/setup.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/unit/test_TOC.py` & `pyinstaller-6.7.0/tests/unit/test_TOC.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/unit/test_Tree.py` & `pyinstaller-6.7.0/tests/unit/test_Tree.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/unit/test_additionalfilescache.py` & `pyinstaller-6.7.0/tests/unit/test_additionalfilescache.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/unit/test_bindepend.py` & `pyinstaller-6.7.0/tests/unit/test_bindepend.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/unit/test_building_utils.py` & `pyinstaller-6.7.0/tests/unit/test_building_utils.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/unit/test_bytecode.py` & `pyinstaller-6.7.0/tests/unit/test_bytecode.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/unit/test_compat.py` & `pyinstaller-6.7.0/tests/unit/test_compat.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/unit/test_depend_utils.py` & `pyinstaller-6.7.0/tests/unit/test_depend_utils.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/unit/test_hook_order.py` & `pyinstaller-6.7.0/tests/unit/test_hook_order.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/unit/test_hookutils.py` & `pyinstaller-6.7.0/tests/unit/test_hookutils.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/unit/test_hookutils_gi.py` & `pyinstaller-6.7.0/tests/unit/test_hookutils_gi.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/unit/test_isolation.py` & `pyinstaller-6.7.0/tests/unit/test_isolation.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/unit/test_makespec.py` & `pyinstaller-6.7.0/tests/unit/test_makespec.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/unit/test_miscutils.py` & `pyinstaller-6.7.0/tests/unit/test_miscutils.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/unit/test_modulegraph/test_basic.py` & `pyinstaller-6.7.0/tests/unit/test_modulegraph/test_basic.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/unit/test_modulegraph/test_compiled_modules.py` & `pyinstaller-6.7.0/tests/unit/test_modulegraph/test_compiled_modules.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/unit/test_modulegraph/test_edge_data.py` & `pyinstaller-6.7.0/tests/unit/test_modulegraph/test_edge_data.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/unit/test_modulegraph/test_implies.py` & `pyinstaller-6.7.0/tests/unit/test_modulegraph/test_implies.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/unit/test_modulegraph/test_import_from_init.py` & `pyinstaller-6.7.0/tests/unit/test_modulegraph/test_import_from_init.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/unit/test_modulegraph/test_imports.py` & `pyinstaller-6.7.0/tests/unit/test_modulegraph/test_imports.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/unit/test_modulegraph/test_modulegraph.py` & `pyinstaller-6.7.0/tests/unit/test_modulegraph/test_modulegraph.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/unit/test_modulegraph/test_pep420_nspkg.py` & `pyinstaller-6.7.0/tests/unit/test_modulegraph/test_pep420_nspkg.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/unit/test_modulegraph/test_pycompat_pkg.py` & `pyinstaller-6.7.0/tests/unit/test_modulegraph/test_pycompat_pkg.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/unit/test_modulegraph/test_relimport2.py` & `pyinstaller-6.7.0/tests/unit/test_modulegraph/test_relimport2.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/unit/test_modulegraph/test_setuptools_nspkg.py` & `pyinstaller-6.7.0/tests/unit/test_modulegraph/test_setuptools_nspkg.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/unit/test_modulegraph/test_swig.py` & `pyinstaller-6.7.0/tests/unit/test_modulegraph/test_swig.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/unit/test_modulegraph/testdata/syspath.egg` & `pyinstaller-6.7.0/tests/unit/test_modulegraph/testdata/syspath.egg`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/unit/test_modulegraph/testdata/syspath.zip` & `pyinstaller-6.7.0/tests/unit/test_modulegraph/testdata/syspath.zip`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/unit/test_modulegraph/testdata/test.egg` & `pyinstaller-6.7.0/tests/unit/test_modulegraph/testdata/test.egg`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-edgedata/script.py` & `pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-edgedata/script.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-edgedata/script_from_import.py` & `pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-edgedata/script_from_import.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/unit/test_modulegraph/testpkg-swig/pkg/sample.py` & `pyinstaller-6.7.0/tests/unit/test_modulegraph/testpkg-swig/pkg/sample.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/unit/test_modulegraph_more.py` & `pyinstaller-6.7.0/tests/unit/test_modulegraph_more.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/unit/test_normalize_icon_type.py` & `pyinstaller-6.7.0/tests/unit/test_normalize_icon_type.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/unit/test_pyimodulegraph.py` & `pyinstaller-6.7.0/tests/unit/test_pyimodulegraph.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/unit/test_recursion_limit.py` & `pyinstaller-6.7.0/tests/unit/test_recursion_limit.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/unit/test_systemexit.py` & `pyinstaller-6.7.0/tests/unit/test_systemexit.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/unit/test_toc_normalization.py` & `pyinstaller-6.7.0/tests/unit/test_toc_normalization.py`

 * *Files identical despite different names*

### Comparing `pyinstaller-6.6.0/tests/unit/test_winmanifest.py` & `pyinstaller-6.7.0/tests/unit/test_winmanifest.py`

 * *Files identical despite different names*

