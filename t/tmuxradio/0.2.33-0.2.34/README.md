# Comparing `tmp/tmuxradio-0.2.33.tar.gz` & `tmp/tmuxradio-0.2.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tmuxradio-0.2.33.tar", last modified: Sun May 19 22:17:40 2024, max compression
+gzip compressed data, was "tmuxradio-0.2.34.tar", last modified: Wed May 22 16:20:21 2024, max compression
```

## Comparing `tmuxradio-0.2.33.tar` & `tmuxradio-0.2.34.tar`

### file list

```diff
@@ -1,1531 +1,1531 @@
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:40.352113 tmuxradio-0.2.33/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      226 2024-05-19 22:07:59.000000 tmuxradio-0.2.33/CHANGELOG.txt
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1056 2024-05-10 11:47:04.000000 tmuxradio-0.2.33/LICENSE.txt
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)       26 2024-05-10 11:47:21.000000 tmuxradio-0.2.33/MANIFEST.in
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1082 2024-05-19 22:17:40.352113 tmuxradio-0.2.33/PKG-INFO
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      555 2024-05-10 16:17:36.000000 tmuxradio-0.2.33/README.txt
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      622 2024-05-19 22:02:33.000000 tmuxradio-0.2.33/main.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      190 2024-05-14 13:02:18.000000 tmuxradio-0.2.33/requirements.txt
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)       38 2024-05-19 22:17:40.352113 tmuxradio-0.2.33/setup.cfg
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      822 2024-05-19 22:12:03.000000 tmuxradio-0.2.33/setup.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.444121 tmuxradio-0.2.33/src/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)       69 2024-05-10 13:57:49.000000 tmuxradio-0.2.33/src/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)       56 2024-05-10 14:18:00.000000 tmuxradio-0.2.33/src/__main__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      242 2024-05-11 18:56:08.000000 tmuxradio-0.2.33/src/args.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1357 2024-05-19 22:10:23.000000 tmuxradio-0.2.33/src/fplay.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      903 2024-05-14 12:31:26.000000 tmuxradio-0.2.33/src/fprobe.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      622 2024-05-19 22:02:19.000000 tmuxradio-0.2.33/src/main.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1563 2024-05-14 12:32:34.000000 tmuxradio-0.2.33/src/utilities.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.460121 tmuxradio-0.2.33/tmuxradio.egg-info/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1082 2024-05-19 22:17:39.000000 tmuxradio-0.2.33/tmuxradio.egg-info/PKG-INFO
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    88905 2024-05-19 22:17:39.000000 tmuxradio-0.2.33/tmuxradio.egg-info/SOURCES.txt
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)        1 2024-05-19 22:17:39.000000 tmuxradio-0.2.33/tmuxradio.egg-info/dependency_links.txt
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)       66 2024-05-19 22:17:39.000000 tmuxradio-0.2.33/tmuxradio.egg-info/entry_points.txt
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)        1 2024-05-10 12:54:26.000000 tmuxradio-0.2.33/tmuxradio.egg-info/not-zip-safe
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      190 2024-05-19 22:17:39.000000 tmuxradio-0.2.33/tmuxradio.egg-info/requires.txt
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)        4 2024-05-19 22:17:39.000000 tmuxradio-0.2.33/tmuxradio.egg-info/top_level.txt
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.360122 tmuxradio-0.2.33/venv/
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.460121 tmuxradio-0.2.33/venv/bin/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1337 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/bin/activate_this.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.360122 tmuxradio-0.2.33/venv/lib/
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.360122 tmuxradio-0.2.33/venv/lib/python3.11/
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.472121 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.484121 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/_distutils_hack/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6299 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/_distutils_hack/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)       44 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/_distutils_hack/override.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4329 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/_virtualenv.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.492121 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/anyio/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4344 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/anyio/__init__.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.500121 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/anyio/_backends/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)        0 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/anyio/_backends/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    81968 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/anyio/_backends/_asyncio.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    35642 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/anyio/_backends/_trio.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.504121 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/anyio/_core/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)        0 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/anyio/_core/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4408 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/anyio/_core/_eventloop.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2078 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/anyio/_core/_exceptions.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    19512 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/anyio/_core/_fileio.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      435 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/anyio/_core/_resources.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      878 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/anyio/_core/_signals.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    24048 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/anyio/_core/_sockets.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1811 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/anyio/_core/_streams.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5272 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/anyio/_core/_subprocesses.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    18444 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/anyio/_core/_synchronization.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4764 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/anyio/_core/_tasks.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1964 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/anyio/_core/_testing.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2499 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/anyio/_core/_typedattr.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.508121 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/anyio/abc/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2681 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/anyio/abc/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    10097 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/anyio/abc/_eventloop.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      763 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/anyio/abc/_resources.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6269 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/anyio/abc/_sockets.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6598 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/anyio/abc/_streams.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2067 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/anyio/abc/_subprocesses.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2747 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/anyio/abc/_tasks.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1829 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/anyio/abc/_testing.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    15749 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/anyio/from_thread.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4185 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/anyio/lowlevel.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5386 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/anyio/pytest_plugin.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.508121 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/anyio/streams/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)        0 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/anyio/streams/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4500 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/anyio/streams/buffered.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4383 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/anyio/streams/file.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     9296 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/anyio/streams/memory.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4302 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/anyio/streams/stapled.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5094 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/anyio/streams/text.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    12752 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/anyio/streams/tls.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     9535 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/anyio/to_process.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2396 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/anyio/to_thread.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.496121 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/anyio-4.3.0.dist-info/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)       39 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/anyio-4.3.0.dist-info/entry_points.txt
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)        6 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/anyio-4.3.0.dist-info/top_level.txt
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.516121 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/certifi/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)       94 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/certifi/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      243 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/certifi/__main__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4426 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/certifi/core.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.516121 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/certifi-2024.2.2.dist-info/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)        8 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/certifi-2024.2.2.dist-info/top_level.txt
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.520121 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/h11/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1507 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/h11/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4815 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/h11/_abnf.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    26539 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/h11/_connection.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    11816 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/h11/_events.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    10230 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/h11/_headers.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8383 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/h11/_readers.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5252 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/h11/_receivebuffer.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    13300 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/h11/_state.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4888 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/h11/_util.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      686 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/h11/_version.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5081 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/h11/_writers.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.524121 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/h11/tests/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)        0 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/h11/tests/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3355 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/h11/tests/helpers.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3995 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/h11/tests/test_against_stdlib_http.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    38720 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/h11/tests/test_connection.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4657 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/h11/tests/test_events.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5612 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/h11/tests/test_headers.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      794 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/h11/tests/test_helpers.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    16386 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/h11/tests/test_io.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3454 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/h11/tests/test_receivebuffer.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8928 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/h11/tests/test_state.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2970 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/h11/tests/test_util.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.520121 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/h11-0.14.0.dist-info/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1124 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/h11-0.14.0.dist-info/LICENSE.txt
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)        4 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/h11-0.14.0.dist-info/top_level.txt
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.528121 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpcore/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3337 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpcore/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3167 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpcore/_api.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.528121 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpcore/_async/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1221 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpcore/_async/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8484 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpcore/_async/connection.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    15609 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpcore/_async/connection_pool.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    13978 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpcore/_async/http11.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    23881 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpcore/_async/http2.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    14851 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpcore/_async/http_proxy.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4486 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpcore/_async/interfaces.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    13934 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpcore/_async/socks_proxy.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.528121 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpcore/_backends/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)        0 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpcore/_backends/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5295 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpcore/_backends/anyio.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1683 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpcore/_backends/auto.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3218 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpcore/_backends/base.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4179 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpcore/_backends/mock.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8086 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpcore/_backends/sync.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6078 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpcore/_backends/trio.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1185 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpcore/_exceptions.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    16614 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpcore/_models.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      187 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpcore/_ssl.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.532121 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpcore/_sync/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1141 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpcore/_sync/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8273 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpcore/_sync/connection.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    15277 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpcore/_sync/connection_pool.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    13564 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpcore/_sync/http11.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    23345 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpcore/_sync/http2.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    14613 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpcore/_sync/http_proxy.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4365 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpcore/_sync/interfaces.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    13707 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpcore/_sync/socks_proxy.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     9464 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpcore/_synchronization.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3954 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpcore/_trace.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1525 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpcore/_utils.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.548121 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpx/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3210 2024-05-09 12:01:15.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpx/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      108 2024-05-09 12:01:15.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpx/__version__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    12928 2024-05-09 12:01:15.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpx/_api.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    11830 2024-05-09 12:01:15.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpx/_auth.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    67490 2024-05-09 12:01:15.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpx/_client.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1563 2024-05-09 12:01:15.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpx/_compat.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    12204 2024-05-09 12:01:15.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpx/_config.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8047 2024-05-09 12:01:15.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpx/_content.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     9904 2024-05-09 12:01:15.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpx/_decoders.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     7922 2024-05-09 12:01:15.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpx/_exceptions.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    15635 2024-05-09 12:01:15.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpx/_main.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    42303 2024-05-09 12:01:15.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpx/_models.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8885 2024-05-09 12:01:15.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpx/_multipart.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5618 2024-05-09 12:01:15.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpx/_status_codes.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.548121 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpx/_transports/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)        0 2024-05-09 12:01:15.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpx/_transports/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5490 2024-05-09 12:01:15.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpx/_transports/asgi.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2472 2024-05-09 12:01:15.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpx/_transports/base.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    13290 2024-05-09 12:01:15.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpx/_transports/default.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1202 2024-05-09 12:01:15.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpx/_transports/mock.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4795 2024-05-09 12:01:15.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpx/_transports/wsgi.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3391 2024-05-09 12:01:15.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpx/_types.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    17720 2024-05-09 12:01:15.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpx/_urlparse.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    21783 2024-05-09 12:01:15.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpx/_urls.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    13858 2024-05-09 12:01:15.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpx/_utils.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.548121 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpx-0.27.0.dist-info/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)       37 2024-05-09 12:01:15.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpx-0.27.0.dist-info/entry_points.txt
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.560120 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/idna/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      849 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/idna/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3426 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/idna/codec.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      321 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/idna/compat.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    12663 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/idna/core.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    78320 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/idna/idnadata.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1881 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/idna/intranges.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)       21 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/idna/package_data.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)   206503 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/idna/uts46data.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.584120 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      113 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      246 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/_compat.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2364 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/_punycode.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.584120 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/cli/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)        0 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/cli/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2901 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/cli/parse.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.588120 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/common/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)        0 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/common/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      156 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/common/entities.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      932 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/common/html_blocks.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      929 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/common/html_re.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2568 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/common/normalize_url.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    10728 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/common/utils.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.588120 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/helpers/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      253 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/helpers/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1977 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/helpers/parse_link_destination.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1036 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/helpers/parse_link_label.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1425 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/helpers/parse_link_title.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    12772 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/main.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3911 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/parser_block.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1010 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/parser_core.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4997 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/parser_inline.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.588120 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/presets/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      970 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/presets/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2868 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/presets/commonmark.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1810 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/presets/default.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2112 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/presets/zero.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     9970 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/renderer.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     9199 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/ruler.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.592120 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/rules_block/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      553 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/rules_block/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8887 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/rules_block/blockquote.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      859 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/rules_block/code.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2537 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/rules_block/fence.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1746 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/rules_block/heading.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1226 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/rules_block/hr.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2721 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/rules_block/html_block.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2625 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/rules_block/lheading.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     9668 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/rules_block/list.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1818 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/rules_block/paragraph.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6168 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/rules_block/reference.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8422 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/rules_block/state_block.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6987 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/rules_block/table.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.592120 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/rules_core/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      394 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/rules_core/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      372 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/rules_core/block.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      325 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/rules_core/inline.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5141 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/rules_core/linkify.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      402 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/rules_core/normalize.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3470 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/rules_core/replacements.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     7443 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/rules_core/smartquotes.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      570 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/rules_core/state_core.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1172 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/rules_core/text_join.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.596120 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/rules_inline/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      696 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/rules_inline/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2079 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/rules_inline/autolink.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2037 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/rules_inline/backticks.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4851 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/rules_inline/balance_pairs.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3123 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/rules_inline/emphasis.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1651 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/rules_inline/entity.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1658 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/rules_inline/escape.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1493 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/rules_inline/fragments_join.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1130 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/rules_inline/html_inline.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4135 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/rules_inline/image.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4318 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/rules_inline/link.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1704 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/rules_inline/linkify.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1296 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/rules_inline/newline.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5101 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/rules_inline/state_inline.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3214 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/rules_inline/strikethrough.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      901 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/rules_inline/text.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6439 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/token.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    11421 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/tree.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5365 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/utils.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.596120 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it_py-3.0.0.dist-info/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)       58 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it_py-3.0.0.dist-info/entry_points.txt
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.596120 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/mdurl/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      547 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/mdurl/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3004 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/mdurl/_decode.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2602 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/mdurl/_encode.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      626 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/mdurl/_format.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    11374 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/mdurl/_parse.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      284 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/mdurl/_url.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.596120 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      355 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      854 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/__main__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1444 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/__pip-runner__.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.608120 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      573 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    10243 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/build_env.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    10429 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/cache.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.624120 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/cli/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      132 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/cli/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6676 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/cli/autocompletion.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8726 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/cli/base_command.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    30029 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/cli/cmdoptions.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      774 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/cli/command_context.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2816 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/cli/main.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4338 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/cli/main_parser.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    10817 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/cli/parser.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1968 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/cli/progress_bars.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    18328 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/cli/req_command.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5118 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/cli/spinners.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      116 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/cli/status_codes.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.636120 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/commands/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3882 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/commands/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     7581 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/commands/cache.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1782 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/commands/check.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3986 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/commands/completion.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     9815 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/commands/configuration.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6591 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/commands/debug.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5335 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/commands/download.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3243 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/commands/freeze.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1703 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/commands/hash.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1132 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/commands/help.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4793 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/commands/index.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3188 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/commands/inspect.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    28934 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/commands/install.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    12554 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/commands/list.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5697 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/commands/search.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6419 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/commands/show.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3886 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/commands/uninstall.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6476 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/commands/wheel.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    13839 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/configuration.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.644120 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/distributions/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      858 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/distributions/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1221 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/distributions/base.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      729 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/distributions/installed.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6494 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/distributions/sdist.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1164 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/distributions/wheel.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    23737 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/exceptions.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.644120 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/index/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)       30 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/index/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    16504 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/index/collector.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    37873 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/index/package_finder.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6556 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/index/sources.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.652119 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/locations/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    15365 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/locations/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6100 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/locations/_distutils.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     7680 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/locations/_sysconfig.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2556 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/locations/base.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      340 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/main.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.652119 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/metadata/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4280 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/metadata/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2595 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/metadata/_json.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    25277 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/metadata/base.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.656119 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/metadata/importlib/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      107 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/metadata/importlib/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1882 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/metadata/importlib/_compat.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8181 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/metadata/importlib/_dists.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     7435 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/metadata/importlib/_envs.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     9773 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/metadata/pkg_resources.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.664120 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/models/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)       63 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/models/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      990 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/models/candidate.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6931 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/models/direct_url.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2520 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/models/format_control.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1030 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/models/index.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2609 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/models/installation_report.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    20819 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/models/link.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      738 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/models/scheme.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4643 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/models/search_scope.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1907 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/models/selection_prefs.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3858 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/models/target_python.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3600 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/models/wheel.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.664120 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/network/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)       50 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/network/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    20541 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/network/auth.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2145 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/network/cache.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6096 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/network/download.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     7638 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/network/lazy_wheel.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    18442 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/network/session.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4073 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/network/utils.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1791 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/network/xmlrpc.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.664120 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/operations/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)        0 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/operations/__init__.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.676119 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/operations/build/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)        0 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/operations/build/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4133 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/operations/build/build_tracker.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1422 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/operations/build/metadata.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1474 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/operations/build/metadata_editable.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2198 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/operations/build/metadata_legacy.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1075 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/operations/build/wheel.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1417 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/operations/build/wheel_editable.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3064 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/operations/build/wheel_legacy.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6806 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/operations/check.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     9816 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/operations/freeze.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.676119 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/operations/install/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)       51 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/operations/install/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1282 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/operations/install/editable_legacy.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    27475 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/operations/install/wheel.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    28571 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/operations/prepare.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     7161 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/pyproject.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.676119 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/req/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2738 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/req/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    16610 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/req/constructors.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    17872 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/req/req_file.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    33084 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/req/req_install.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4704 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/req/req_set.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    24678 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/req/req_uninstall.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.680119 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/resolution/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)        0 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/resolution/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      583 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/resolution/base.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.680119 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/resolution/legacy/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)        0 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/resolution/legacy/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    24128 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/resolution/legacy/resolver.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.680119 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)        0 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5220 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/base.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    18969 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/candidates.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    27845 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/factory.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5705 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     9824 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/provider.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3100 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/reporter.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5454 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/requirements.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    11642 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/resolver.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8167 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/self_outdated_check.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.704119 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/utils/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)        0 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/utils/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3351 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/utils/_jaraco_text.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1015 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/utils/_log.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1665 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/utils/appdirs.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1884 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/utils/compat.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5377 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/utils/compatibility_tags.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      242 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/utils/datetime.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3627 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/utils/deprecation.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3206 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/utils/direct_url_helpers.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2118 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/utils/egg_link.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1169 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/utils/encoding.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3064 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/utils/entrypoints.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5122 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/utils/filesystem.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      716 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/utils/filetypes.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3113 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/utils/glibc.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5118 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/utils/hashes.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      795 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/utils/inject_securetransport.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    11632 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/utils/logging.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    23344 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/utils/misc.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1193 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/utils/models.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2108 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/utils/packaging.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4435 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/utils/setuptools_build.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     9200 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/utils/subprocess.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     7702 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/utils/temp_dir.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8821 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/utils/unpacking.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1759 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/utils/urls.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3456 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/utils/virtualenv.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4549 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/utils/wheel.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.704119 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/vcs/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      596 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/vcs/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3519 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/vcs/bazaar.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    18116 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/vcs/git.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5244 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/vcs/mercurial.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    11729 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/vcs/subversion.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    22811 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/vcs/versioncontrol.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    11842 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/wheel_builder.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.716119 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4966 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/__init__.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.728119 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      465 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1379 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/_cmd.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5033 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/adapter.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1535 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/cache.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.728119 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/caches/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      242 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/caches/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5271 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1033 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      778 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/compat.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    16416 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/controller.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3946 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/filewrapper.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4154 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/heuristics.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     7105 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/serialize.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      774 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/wrapper.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.732119 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/certifi/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)       94 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/certifi/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      255 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/certifi/__main__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4531 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/certifi/core.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.776118 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4797 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    31274 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/big5freq.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1763 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/big5prober.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    10032 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/chardistribution.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3915 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/charsetgroupprober.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5420 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/charsetprober.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.776118 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/cli/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)        0 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/cli/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3242 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/cli/chardetect.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3732 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/codingstatemachine.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      542 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/codingstatemachinedict.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1860 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/cp949prober.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1683 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/enums.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4006 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/escprober.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    12176 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/escsm.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3934 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/eucjpprober.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    13566 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/euckrfreq.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1753 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/euckrprober.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    36913 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/euctwfreq.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1753 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/euctwprober.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    20735 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/gb2312freq.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1759 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/gb2312prober.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    14537 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/hebrewprober.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    25796 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/jisfreq.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    42498 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/johabfreq.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1752 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/johabprober.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    27055 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/jpcntx.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)   104562 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/langbulgarianmodel.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    98484 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/langgreekmodel.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    98196 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/langhebrewmodel.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)   101363 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/langhungarianmodel.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)   128035 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/langrussianmodel.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)   102774 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/langthaimodel.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    95372 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/langturkishmodel.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5380 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/latin1prober.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6077 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/macromanprober.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3715 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/mbcharsetprober.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2131 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/mbcsgroupprober.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    30391 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/mbcssm.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.780118 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/metadata/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)        0 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/metadata/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    13560 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/metadata/languages.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      402 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/resultdict.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6400 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/sbcharsetprober.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4137 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/sbcsgroupprober.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4007 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/sjisprober.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    14848 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/universaldetector.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8505 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/utf1632prober.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2812 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/utf8prober.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      244 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/version.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.788118 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/colorama/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      266 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/colorama/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2522 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/colorama/ansi.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    11128 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/colorama/ansitowin32.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3325 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/colorama/initialise.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.788118 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)       75 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2839 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/ansi_test.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    10678 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6741 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/initialise_test.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1866 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/isatty_test.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1079 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/utils.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3709 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/winterm_test.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6181 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/colorama/win32.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     7134 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/colorama/winterm.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.800118 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/distlib/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      581 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/distlib/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    41259 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/distlib/compat.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    51697 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/distlib/database.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    20834 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/distlib/index.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    51991 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/distlib/locators.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    14811 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/distlib/manifest.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5058 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/distlib/markers.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    39801 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/distlib/metadata.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    10820 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/distlib/resources.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    18102 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/distlib/scripts.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    66262 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/distlib/util.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    23513 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/distlib/version.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    43898 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/distlib/wheel.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.812118 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/distro/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      981 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/distro/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)       64 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/distro/__main__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    49330 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/distro/distro.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.820118 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/idna/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      849 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/idna/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3374 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/idna/codec.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      321 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/idna/compat.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    12950 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/idna/core.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    44375 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/idna/idnadata.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1881 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/idna/intranges.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)       21 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/idna/package_data.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)   206539 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/idna/uts46data.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.820118 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/msgpack/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1132 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/msgpack/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1081 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/msgpack/exceptions.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6079 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/msgpack/ext.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    34544 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/msgpack/fallback.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.824118 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/packaging/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      661 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/packaging/__about__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      497 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/packaging/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    11488 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/packaging/_manylinux.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4378 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/packaging/_musllinux.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1431 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/packaging/_structures.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8487 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/packaging/markers.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4676 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/packaging/requirements.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    30110 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/packaging/specifiers.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    15699 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/packaging/tags.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4200 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/packaging/utils.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    14665 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/packaging/version.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.824118 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pkg_resources/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)   109364 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pkg_resources/__init__.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.824118 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    20155 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1476 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/__main__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     7211 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/android.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     7132 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/api.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3678 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/macos.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8809 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/unix.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      160 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/version.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     9573 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/windows.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.832118 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pygments/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2983 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pygments/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      353 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pygments/__main__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    23685 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pygments/cmdline.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1697 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pygments/console.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1938 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pygments/filter.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.832118 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pygments/filters/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    40386 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pygments/filters/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4178 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatter.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.836118 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5424 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4176 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/_mapping.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3314 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/bbcode.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5094 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/groff.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    35610 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/html.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    21938 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/img.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4981 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/irc.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    19351 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/latex.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5073 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/other.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2212 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5014 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/rtf.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     7335 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/svg.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4674 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/terminal.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    11753 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/terminal256.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    34618 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pygments/lexer.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.848118 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    12130 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    72281 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/_mapping.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    53424 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/python.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      986 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pygments/modeline.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2591 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pygments/plugin.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3072 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pygments/regexopt.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3092 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pygments/scanner.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6882 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pygments/sphinxext.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6257 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pygments/style.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.848118 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pygments/styles/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3700 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pygments/styles/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6184 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pygments/token.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    63223 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pygments/unistring.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    10230 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pygments/util.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.864117 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     9116 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6567 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/actions.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    13387 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/common.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)   224445 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/core.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.864117 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/diagram/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    24215 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/diagram/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     9523 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/exceptions.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    38646 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/helpers.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    26692 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/results.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    13488 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/testing.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    10646 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/unicode.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8670 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/util.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.864117 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      491 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      138 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_compat.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    11920 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_impl.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.864117 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_in_process/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      546 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    10927 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.872117 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/requests/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5169 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/requests/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      435 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/requests/__version__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1495 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/requests/_internal_utils.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    19697 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/requests/adapters.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6449 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/requests/api.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    10187 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/requests/auth.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      575 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/requests/certs.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1286 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/requests/compat.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    18560 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/requests/cookies.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3823 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/requests/exceptions.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3879 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/requests/help.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      733 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/requests/hooks.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    35288 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/requests/models.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      695 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/requests/packages.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    30373 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/requests/sessions.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4235 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/requests/status_codes.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2912 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/requests/structures.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    33460 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/requests/utils.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.872117 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      537 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/__init__.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.872117 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/compat/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)        0 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/compat/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      156 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/compat/collections_abc.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5871 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/providers.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1601 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/reporters.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    20511 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/resolvers.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4963 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/structs.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.916117 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6090 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8478 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/__main__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    10096 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/_cell_widths.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)   140235 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/_emoji_codes.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1064 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/_emoji_replace.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2100 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/_export_format.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      265 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/_extension.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      799 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/_fileno.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     9695 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/_inspect.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3225 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/_log_render.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1236 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/_loop.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1387 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/_null_file.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     7063 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/_palettes.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      423 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/_pick.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5472 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/_ratio.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    19919 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/_spinners.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      351 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/_stack.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      417 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/_timer.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    22820 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/_win32_console.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1926 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/_windows.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2783 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/_windows_renderer.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1840 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/_wrap.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      890 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/abc.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    10368 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/align.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6906 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/ansi.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3264 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/bar.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     9842 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/box.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4509 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/cells.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    18224 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/color.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1054 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/color_triplet.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     7131 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/columns.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    99218 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/console.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1288 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/constrain.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5497 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/containers.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6630 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/control.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8082 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/default_styles.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      972 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/diagnose.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2501 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/emoji.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      642 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/errors.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1683 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/file_proxy.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2508 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/filesize.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     9584 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/highlighter.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5032 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/json.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3252 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/jupyter.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    14007 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/layout.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    14273 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/live.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3667 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/live_render.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    11903 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/logging.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8198 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/markup.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5305 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/measure.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4970 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/padding.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      828 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/pager.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3396 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/palette.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    10574 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/panel.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    35852 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/pretty.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    59706 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/progress.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8165 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/progress_bar.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    11303 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/prompt.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1391 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/protocol.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      166 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/region.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4431 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/repr.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4602 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/rule.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2843 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/scope.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1591 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/screen.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    24247 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/segment.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4339 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/spinner.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4425 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/status.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    27073 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/style.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1258 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/styled.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    35173 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/syntax.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    39684 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/table.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3370 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/terminal_theme.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    45525 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/text.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3777 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/theme.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      102 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/themes.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    29604 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/traceback.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     9169 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/tree.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    34549 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/six.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.916117 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/tenacity/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    20493 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/tenacity/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3551 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/tenacity/_asyncio.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2179 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/tenacity/_utils.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1682 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/tenacity/after.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1562 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/tenacity/before.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2372 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/tenacity/before_sleep.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1383 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/tenacity/nap.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8746 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/tenacity/retry.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3086 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/tenacity/stop.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2142 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/tenacity/tornadoweb.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8024 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/tenacity/wait.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.916117 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/tomli/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      396 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/tomli/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    22633 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/tomli/_parser.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2943 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/tomli/_re.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      254 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/tomli/_types.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)   111130 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/typing_extensions.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.928117 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3333 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    11372 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/_collections.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)       64 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/_version.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    20300 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/connection.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    40285 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/connectionpool.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.932117 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)        0 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      957 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.932117 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_securetransport/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)        0 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    17632 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    13922 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    11036 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/appengine.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4528 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    17081 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    34448 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/securetransport.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     7097 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/socks.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8217 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/exceptions.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8579 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/fields.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2440 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/filepost.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.932117 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)        0 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/__init__.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.936117 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/backports/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)        0 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/backports/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1417 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5343 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/backports/weakref_finalize.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    34665 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/six.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    19990 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/poolmanager.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5985 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/request.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    30641 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/response.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.936117 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1155 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4901 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/connection.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1605 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/proxy.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      498 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/queue.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3997 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/request.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3510 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/response.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    22013 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/retry.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    17177 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/ssl_.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5758 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6895 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/ssltransport.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    10168 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/timeout.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    14296 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/url.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5403 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/wait.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      475 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/vendor.txt
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.940117 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/webencodings/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    10579 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/webencodings/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8979 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/webencodings/labels.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1305 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/webencodings/mklabels.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6563 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/webencodings/tests.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4307 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/webencodings/x_user_defined.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.600120 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip-23.2.dist-info/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    10065 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip-23.2.dist-info/AUTHORS.txt
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1093 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip-23.2.dist-info/LICENSE.txt
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      125 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip-23.2.dist-info/entry_points.txt
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)        4 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip-23.2.dist-info/top_level.txt
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.940117 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pkg_resources/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)   109429 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pkg_resources/__init__.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.952117 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pkg_resources/_vendor/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)        0 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pkg_resources/_vendor/__init__.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.956117 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      506 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4504 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_adapters.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5457 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_common.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2925 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_compat.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      884 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_itertools.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3481 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_legacy.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5140 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/abc.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3581 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/readers.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2576 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/simple.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.956117 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)        0 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     7460 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/context.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    15056 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/functools.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.956117 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/text/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    15526 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/text/__init__.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.956117 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      148 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)   134976 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/more.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    25416 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/recipes.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.960117 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      501 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3266 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_elffile.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8926 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_manylinux.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2524 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_musllinux.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    10194 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_parser.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1431 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_structures.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5292 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_tokenizer.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8208 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/markers.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    16397 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/metadata.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3287 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/requirements.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    39206 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/specifiers.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    18106 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/tags.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4355 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/utils.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    16326 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/version.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.960117 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    12806 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1164 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/__main__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4068 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/android.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4910 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/api.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2655 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/macos.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6911 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/unix.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      160 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/version.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6596 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/windows.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    80078 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pkg_resources/_vendor/typing_extensions.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8425 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pkg_resources/_vendor/zipp.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.960117 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pkg_resources/extern/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2442 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pkg_resources/extern/__init__.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.972117 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2959 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      348 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/__main__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    23536 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/cmdline.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1718 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/console.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1910 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/filter.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.980116 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/filters/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    40344 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/filters/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4366 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/formatter.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.984116 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/formatters/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5349 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/formatters/__init__.py
--rwxrwxr-x   0 sifaw     (1000) sifaw     (1000)     4176 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/formatters/_mapping.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3296 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/formatters/bbcode.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5082 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/formatters/groff.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    35633 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/formatters/html.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    23263 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/formatters/img.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4945 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/formatters/irc.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    19258 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/formatters/latex.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4986 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/formatters/other.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2206 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/formatters/pangomarkup.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    11921 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/formatters/rtf.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     7138 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/formatters/svg.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4626 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/formatters/terminal.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    11717 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/formatters/terminal256.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    35109 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexer.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:40.116115 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    12067 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1543 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/_ada_builtins.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    27287 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/_asy_builtins.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    13994 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/_cl_builtins.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)   105173 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/_cocoa_builtins.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    18414 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/_csound_builtins.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    12446 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/_css_builtins.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    11883 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/_julia_builtins.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)   134510 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/_lasso_builtins.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)   108094 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/_lilypond_builtins.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8108 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/_lua_builtins.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      955 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/_luau_builtins.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    69089 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/_mapping.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    24713 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/_mql_builtins.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    25838 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/_mysql_builtins.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    49398 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/_openedge_builtins.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)   107922 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/_php_builtins.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    13343 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/_postgres_builtins.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    12595 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/_qlik_builtins.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    32564 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/_scheme_builtins.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    52411 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/_scilab_builtins.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    26777 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/_sourcemod_builtins.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    13445 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/_stan_builtins.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    27227 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/_stata_builtins.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    15460 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/_tsql_builtins.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1658 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/_usd_builtins.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4225 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/_vbscript_builtins.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    57066 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/_vim_builtins.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    11727 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/actionscript.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5353 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/ada.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      896 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/agile.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     9912 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/algebra.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2605 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/ambient.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1723 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/amdgpu.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4176 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/ampl.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    30800 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/apdlexer.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3404 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/apl.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    11538 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/archetype.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3564 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/arrow.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    11414 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/arturo.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1693 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/asc.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    41934 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/asm.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4262 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/asn1.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    19831 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/automation.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3020 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/bare.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    27989 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/basic.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1641 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/bdd.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3209 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/berry.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4811 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/bibtex.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6188 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/blueprint.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3921 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/boa.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3337 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/bqn.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    28345 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/business.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    18059 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/c_cpp.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    32021 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/c_like.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2174 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/capnproto.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3211 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/carbon.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5076 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/cddl.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5156 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/chapel.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6418 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/clean.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3179 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/comal.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1426 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/compiled.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    50534 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/configs.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4180 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/console.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1389 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/cplint.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    15754 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/crystal.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    16998 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/csound.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    25366 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/css.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     9920 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/d.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4606 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/dalvik.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    27026 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/data.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8098 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/dax.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4019 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/devicetree.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5382 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/diff.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3891 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/dns.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    37958 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/dotnet.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    36746 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/dsls.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    10391 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/dylan.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6371 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/ecl.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2690 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/eiffel.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3152 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/elm.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6535 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/elpi.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4804 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/email.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    19147 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/erlang.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    10500 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/esoteric.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3272 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/ezhil.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    19530 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/factor.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    10231 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/fantom.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     9655 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/felix.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1644 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/fift.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2667 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/floscript.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     7193 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/forth.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    10382 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/fortran.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    26295 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/foxpro.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    26913 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/freefem.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3700 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/func.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      693 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/functional.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3743 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/futhark.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      874 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/gcodelexer.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     7566 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/gdscript.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3783 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/go.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8043 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/grammar_notation.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4108 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/graph.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    39145 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/graphics.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5601 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/graphql.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1934 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/graphviz.py
--rwxrwxr-x   0 sifaw     (1000) sifaw     (1000)     3990 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/gsql.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    33239 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/haskell.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    30974 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/haxe.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    22738 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/hdl.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3653 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/hexdump.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    20574 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/html.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    15449 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/idl.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    31626 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/igor.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3135 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/inferno.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    13297 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/installers.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    56544 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/int_fiction.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1905 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/iolang.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4853 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/j.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    63101 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/javascript.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2082 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/jmespath.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3700 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/jslt.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5636 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/jsonnet.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2233 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/jsx.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    11679 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/julia.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    72666 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/jvm.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    11405 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/kuin.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3477 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/kusto.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6551 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/ldap.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8570 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/lean.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     9752 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/lilypond.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)   157668 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/lisp.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    32844 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/macaulay2.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     7831 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/make.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    65088 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/markup.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      695 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/math.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)   132962 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/matlab.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2715 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/maxima.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4336 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/meson.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     7582 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/mime.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    13696 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/minecraft.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4656 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/mips.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    35390 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/ml.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    13683 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/modeling.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    53072 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/modula2.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    24181 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/mojo.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6289 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/monte.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     9297 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/mosel.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    63999 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/ncl.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6413 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/nimrod.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2725 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/nit.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4421 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/nix.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4210 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/oberon.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    23240 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/objective.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2981 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/ooc.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3700 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/openscad.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1763 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/other.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2719 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/parasail.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    26596 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/parsers.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    30989 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/pascal.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8253 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/pawn.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    39192 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/perl.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    23249 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/phix.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    13061 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/php.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1974 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/pointless.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3279 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/pony.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    12676 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/praat.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1155 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/procfile.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    12866 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/prolog.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4738 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/promql.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8747 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/prql.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4501 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/ptx.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    53639 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/python.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6936 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/q.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3693 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/qlik.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6103 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/qvt.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6342 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/r.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    16042 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/rdf.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    18259 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/rebol.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2927 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/resource.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5035 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/ride.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1127 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/rita.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1972 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/rnc.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2074 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/roboconf.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    18448 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/robotframework.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    22753 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/ruby.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8260 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/rust.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     9456 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/sas.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4878 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/savi.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2524 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/scdoc.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    81062 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/scripting.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1985 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/sgf.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    36234 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/shell.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2514 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/sieve.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8484 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/slash.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     7204 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/smalltalk.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2659 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/smithy.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2805 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/smv.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2778 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/snobol.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3163 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/solidity.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2339 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/soong.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3376 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/sophia.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3554 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/special.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2790 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/spice.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    42594 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/sql.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1746 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/srcinfo.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6415 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/stata.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3697 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/supercollider.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    10809 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/tact.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2904 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/tal.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5512 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/tcl.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3522 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/teal.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    75719 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/templates.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     9718 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/teraterm.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    10810 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/testing.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1048 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/text.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     7760 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/textedit.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    15524 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/textfmts.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    17855 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/theorem.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6017 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/thingsdb.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1450 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/tlb.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1540 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/tls.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    10456 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/tnt.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1506 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/trafficscript.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8332 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/typoscript.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4337 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/typst.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    10499 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/ul4.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    18625 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/unicon.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6082 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/urbi.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3304 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/usd.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     7473 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/varnish.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3934 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/verification.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2661 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/verifpal.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5711 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/vip.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5590 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/vyper.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      913 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/web.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5698 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/webassembly.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    10516 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/webidl.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    40564 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/webmisc.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    11880 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/wgsl.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4017 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/whiley.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4076 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/wowtoc.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3229 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/wren.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1943 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/x10.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      925 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/xorg.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4499 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/yang.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2427 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/yara.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3976 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/zig.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1005 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/modeline.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1891 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/plugin.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3072 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/regexopt.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3092 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/scanner.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     7898 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/sphinxext.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6408 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/style.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:40.128115 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2006 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3312 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/_mapping.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      749 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/abap.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2262 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/algol.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2283 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/algol_nu.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4557 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/arduino.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2195 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/autumn.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1611 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/borland.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1406 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/bw.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2308 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/coffee.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2832 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/colorful.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2588 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/default.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2182 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/dracula.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2535 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/emacs.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2604 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/friendly.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2828 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/friendly_grayscale.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1324 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/fruity.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3590 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/gh_dark.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3387 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/gruvbox.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      737 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/igor.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2404 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/inkpot.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3172 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/lightbulb.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2066 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/lilypond.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3178 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/lovelace.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2443 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/manni.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4201 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/material.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5184 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/monokai.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2805 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/murphy.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2043 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/native.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5391 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/nord.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1719 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/onedark.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5662 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/paraiso_dark.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5668 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/paraiso_light.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2525 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/pastie.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2230 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/perldoc.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2390 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/rainbow_dash.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      964 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/rrt.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1440 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/sas.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4247 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/solarized.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      831 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/staroffice.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1257 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/stata_dark.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1289 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/stata_light.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     7137 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/tango.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1981 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/trac.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2019 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/vim.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1130 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/vs.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1504 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/xcode.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2203 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/zenburn.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6226 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/token.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    63208 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/unistring.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    10031 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/util.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:39.972117 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments-2.18.0.dist-info/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)       53 2024-05-09 11:44:04.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments-2.18.0.dist-info/entry_points.txt
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:40.132115 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pyradios/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      316 2024-05-09 12:01:15.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pyradios/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1679 2024-05-09 12:01:15.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pyradios/base_url.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2468 2024-05-09 12:01:15.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pyradios/facets.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    14102 2024-05-09 12:01:15.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pyradios/radios.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2927 2024-05-09 12:01:15.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pyradios/utils.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:40.132115 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pyradios-2.1.0.dist-info/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)        9 2024-05-09 12:01:15.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pyradios-2.1.0.dist-info/top_level.txt
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:40.184115 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6066 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8333 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/__main__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    10209 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/_cell_widths.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)   140235 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/_emoji_codes.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1064 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/_emoji_replace.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2128 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/_export_format.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      241 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/_extension.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      799 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/_fileno.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     9695 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/_inspect.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3213 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/_log_render.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1236 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/_loop.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1387 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/_null_file.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     7063 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/_palettes.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      423 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/_pick.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5459 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/_ratio.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    19919 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/_spinners.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      351 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/_stack.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      417 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/_timer.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    22784 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/_win32_console.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1901 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/_windows.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2759 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/_windows_renderer.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3404 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/_wrap.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      878 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/abc.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    10320 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/align.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6906 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/ansi.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3263 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/bar.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    10783 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/box.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4780 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/cells.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    18223 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/color.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1054 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/color_triplet.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     7131 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/columns.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    99101 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/console.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1288 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/constrain.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5502 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/containers.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6606 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/control.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8046 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/default_styles.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      924 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/diagnose.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2465 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/emoji.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      642 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/errors.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1683 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/file_proxy.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2508 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/filesize.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     9585 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/highlighter.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5019 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/json.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3228 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/jupyter.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    13944 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/layout.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    14271 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/live.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3654 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/live_render.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    11891 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/logging.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    26167 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/markdown.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8427 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/markup.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5305 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/measure.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4958 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/padding.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      828 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/pager.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3288 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/palette.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    10705 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/panel.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    35812 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/pretty.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    59703 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/progress.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8164 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/progress_bar.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    11292 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/prompt.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1367 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/protocol.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      166 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/region.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4419 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/repr.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4590 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/rule.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2831 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/scope.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1579 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/screen.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    24210 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/segment.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4339 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/spinner.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4424 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/status.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    27073 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/style.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1234 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/styled.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    35367 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/syntax.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    39644 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/table.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3370 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/terminal_theme.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    47300 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/text.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3777 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/theme.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      102 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/themes.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    29529 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/traceback.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     9107 2024-05-09 11:44:05.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/tree.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:40.208114 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     9258 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/__init__.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:40.272114 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      359 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5300 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/_collections.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      411 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/_functools.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)       43 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/_log.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      239 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/_macos_compat.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    19616 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/_msvccompiler.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8572 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/archive_util.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    14721 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/bcppcompiler.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    48643 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/ccompiler.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    17861 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/cmd.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:40.276114 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/command/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      430 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/command/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1614 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/command/_framework_compat.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5408 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/command/bdist.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4665 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/command/bdist_dumb.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    22013 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/command/bdist_rpm.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5584 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/command/build.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     7684 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/command/build_clib.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    31503 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/command/build_ext.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    16537 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/command/build_py.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5604 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/command/build_scripts.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4872 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/command/check.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2594 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/command/clean.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    13077 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/command/config.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    30153 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/command/install.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2762 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/command/install_data.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2788 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/command/install_egg_info.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1180 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/command/install_headers.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8409 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/command/install_lib.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1932 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/command/install_scripts.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      672 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/command/py37compat.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    11817 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/command/register.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    19232 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/command/sdist.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     7491 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/command/upload.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4911 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/config.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     9397 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/core.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    11924 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/cygwinccompiler.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      139 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/debug.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3414 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/dep_util.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8072 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/dir_util.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    50174 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/dist.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3589 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/errors.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    10270 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/extension.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    17899 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/fancy_getopt.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8212 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/file_util.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    13715 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/filelist.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1201 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/log.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    30188 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/msvc9compiler.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    23577 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/msvccompiler.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      217 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/py38compat.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      639 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/py39compat.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3495 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/spawn.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    18928 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/sysconfig.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    12085 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/text_file.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    15601 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/unixccompiler.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    18099 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/util.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    12951 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/version.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5205 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/versionpredicate.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2235 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_entry_points.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2433 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_imp.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1468 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_importlib.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      675 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_itertools.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3706 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_normalization.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1056 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_path.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      882 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_reqs.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:40.280114 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)        0 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/__init__.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:40.284114 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    26498 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2454 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_adapters.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      743 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_collections.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1859 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_compat.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2895 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_functools.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2068 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_itertools.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1165 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_meta.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1098 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_py39compat.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2166 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_text.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:40.284114 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      506 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4504 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_adapters.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5457 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_common.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2925 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_compat.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      884 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_itertools.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3481 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_legacy.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5140 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/abc.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3581 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/readers.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2576 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/simple.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:40.284114 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/jaraco/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)        0 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/jaraco/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     7460 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/jaraco/context.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    15053 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/jaraco/functools.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:40.288113 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/jaraco/text/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    15517 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/jaraco/text/__init__.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:40.288113 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)       82 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)   117959 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/more.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    16256 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/recipes.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    15130 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/ordered_set.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:40.300113 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      501 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3266 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/_elffile.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8926 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/_manylinux.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2524 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/_musllinux.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    10194 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/_parser.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1431 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/_structures.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5292 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/_tokenizer.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8208 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/markers.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    16397 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/metadata.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3287 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/requirements.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    39206 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/specifiers.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    18106 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/tags.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4355 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/utils.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    16326 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/version.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:40.300113 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/tomli/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      396 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/tomli/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    22633 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/tomli/_parser.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2943 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/tomli/_re.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      254 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/tomli/_types.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    87149 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/typing_extensions.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8425 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/zipp.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     7331 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/archive_util.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    20091 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/build_meta.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:40.324113 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/command/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      396 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/command/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2383 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/command/alias.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    16559 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/command/bdist_egg.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1309 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/command/bdist_rpm.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6784 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/command/build.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4398 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/command/build_clib.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    17504 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/command/build_ext.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    14997 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/command/build_py.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6722 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/command/develop.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4242 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/command/dist_info.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    88844 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/command/easy_install.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    33238 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/command/editable_wheel.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    27134 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/command/egg_info.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5627 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/command/install.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3044 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/command/install_egg_info.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5031 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/command/install_lib.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2359 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/command/install_scripts.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      468 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/command/register.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2097 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/command/rotate.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      657 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/command/saveopts.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     7098 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/command/sdist.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4927 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/command/setopt.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8101 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/command/test.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      462 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/command/upload.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     7773 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/command/upload_docs.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:40.328113 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/config/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1498 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/config/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    14195 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/config/_apply_pyprojecttoml.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:40.344113 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1038 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    11266 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/error_reporting.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1153 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/extra_validations.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1612 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_exceptions.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)   274908 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_validations.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     9160 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/formats.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    16401 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/config/expand.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    17490 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/config/pyprojecttoml.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    26184 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/config/setupcfg.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      936 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/dep_util.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5528 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/depends.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    21147 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/discovery.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    46833 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/dist.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2464 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/errors.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5591 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/extension.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:40.344113 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/extern/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2539 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/extern/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4868 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/glob.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4989 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/installer.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      812 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/launch.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1239 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/logging.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4686 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/monkey.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    47495 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/msvc.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3044 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/namespaces.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    38350 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/package_index.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      330 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/py312compat.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    14349 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/sandbox.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      941 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/unicode_utils.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      161 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/version.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3697 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/warnings.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8628 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/wheel.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      719 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/windows_support.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:40.220114 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools-68.1.2.dist-info/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2676 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools-68.1.2.dist-info/entry_points.txt
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)       41 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools-68.1.2.dist-info/top_level.txt
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:40.344113 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/sniffio/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      335 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/sniffio/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2843 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/sniffio/_impl.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:40.344113 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/sniffio/_tests/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)        0 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/sniffio/_tests/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2058 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/sniffio/_tests/test_sniffio.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)       89 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/sniffio/_version.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:40.344113 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/sniffio-1.3.1.dist-info/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)        8 2024-05-09 12:01:14.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/sniffio-1.3.1.dist-info/top_level.txt
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:40.344113 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/wheel/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)       59 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/wheel/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      455 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/wheel/__main__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      746 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/wheel/_setuptools_logging.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    20127 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/wheel/bdist_wheel.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:40.348113 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/wheel/cli/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4250 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/wheel/cli/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     9431 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/wheel/cli/convert.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4338 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/wheel/cli/pack.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5096 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/wheel/cli/tags.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1021 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/wheel/cli/unpack.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    16143 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/wheel/macosx_libfile.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5889 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/wheel/metadata.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      621 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/wheel/util.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:40.348113 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/wheel/vendored/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)        0 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/wheel/vendored/__init__.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:40.352113 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/wheel/vendored/packaging/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)        0 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/wheel/vendored/packaging/__init__.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3266 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/wheel/vendored/packaging/_elffile.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8813 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/wheel/vendored/packaging/_manylinux.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2524 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/wheel/vendored/packaging/_musllinux.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     9399 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/wheel/vendored/packaging/_parser.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1431 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/wheel/vendored/packaging/_structures.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5148 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/wheel/vendored/packaging/_tokenizer.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8161 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/wheel/vendored/packaging/markers.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3264 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/wheel/vendored/packaging/requirements.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    39047 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/wheel/vendored/packaging/specifiers.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    18065 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/wheel/vendored/packaging/tags.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4355 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/wheel/vendored/packaging/utils.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    16295 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/wheel/vendored/packaging/version.py
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)       16 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/wheel/vendored/vendor.txt
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     7748 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/wheel/wheelfile.py
-drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-19 22:17:40.344113 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/wheel-0.41.0.dist-info/
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1107 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/wheel-0.41.0.dist-info/LICENSE.txt
--rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      104 2024-05-09 11:43:18.000000 tmuxradio-0.2.33/venv/lib/python3.11/site-packages/wheel-0.41.0.dist-info/entry_points.txt
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:21.119453 tmuxradio-0.2.34/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      226 2024-05-22 16:19:49.000000 tmuxradio-0.2.34/CHANGELOG.txt
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1056 2024-05-10 11:47:04.000000 tmuxradio-0.2.34/LICENSE.txt
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)       26 2024-05-10 11:47:21.000000 tmuxradio-0.2.34/MANIFEST.in
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1082 2024-05-22 16:20:21.119453 tmuxradio-0.2.34/PKG-INFO
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      555 2024-05-10 16:17:36.000000 tmuxradio-0.2.34/README.txt
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      622 2024-05-19 22:02:33.000000 tmuxradio-0.2.34/main.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      190 2024-05-14 13:02:18.000000 tmuxradio-0.2.34/requirements.txt
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)       38 2024-05-22 16:20:21.119453 tmuxradio-0.2.34/setup.cfg
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      822 2024-05-22 16:19:39.000000 tmuxradio-0.2.34/setup.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.226332 tmuxradio-0.2.34/src/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)       69 2024-05-10 13:57:49.000000 tmuxradio-0.2.34/src/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)       56 2024-05-10 14:18:00.000000 tmuxradio-0.2.34/src/__main__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      242 2024-05-11 18:56:08.000000 tmuxradio-0.2.34/src/args.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1367 2024-05-22 16:17:31.000000 tmuxradio-0.2.34/src/fplay.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      903 2024-05-14 12:31:26.000000 tmuxradio-0.2.34/src/fprobe.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      622 2024-05-19 22:02:19.000000 tmuxradio-0.2.34/src/main.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1563 2024-05-19 23:09:15.000000 tmuxradio-0.2.34/src/utilities.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.230337 tmuxradio-0.2.34/tmuxradio.egg-info/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1082 2024-05-22 16:20:19.000000 tmuxradio-0.2.34/tmuxradio.egg-info/PKG-INFO
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    88905 2024-05-22 16:20:20.000000 tmuxradio-0.2.34/tmuxradio.egg-info/SOURCES.txt
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)        1 2024-05-22 16:20:19.000000 tmuxradio-0.2.34/tmuxradio.egg-info/dependency_links.txt
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)       66 2024-05-22 16:20:19.000000 tmuxradio-0.2.34/tmuxradio.egg-info/entry_points.txt
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)        1 2024-05-10 12:54:26.000000 tmuxradio-0.2.34/tmuxradio.egg-info/not-zip-safe
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      190 2024-05-22 16:20:19.000000 tmuxradio-0.2.34/tmuxradio.egg-info/requires.txt
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)        4 2024-05-22 16:20:19.000000 tmuxradio-0.2.34/tmuxradio.egg-info/top_level.txt
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.202302 tmuxradio-0.2.34/venv/
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.230337 tmuxradio-0.2.34/venv/bin/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1337 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/bin/activate_this.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.202302 tmuxradio-0.2.34/venv/lib/
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.202302 tmuxradio-0.2.34/venv/lib/python3.11/
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.238347 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.246358 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/_distutils_hack/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6299 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/_distutils_hack/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)       44 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/_distutils_hack/override.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4329 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/_virtualenv.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.254368 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/anyio/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4344 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/anyio/__init__.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.262378 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/anyio/_backends/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)        0 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/anyio/_backends/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    81968 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/anyio/_backends/_asyncio.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    35642 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/anyio/_backends/_trio.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.266383 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/anyio/_core/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)        0 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/anyio/_core/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4408 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/anyio/_core/_eventloop.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2078 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/anyio/_core/_exceptions.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    19512 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/anyio/_core/_fileio.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      435 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/anyio/_core/_resources.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      878 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/anyio/_core/_signals.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    24048 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/anyio/_core/_sockets.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1811 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/anyio/_core/_streams.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5272 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/anyio/_core/_subprocesses.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    18444 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/anyio/_core/_synchronization.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4764 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/anyio/_core/_tasks.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1964 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/anyio/_core/_testing.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2499 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/anyio/_core/_typedattr.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.266383 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/anyio/abc/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2681 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/anyio/abc/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    10097 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/anyio/abc/_eventloop.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      763 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/anyio/abc/_resources.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6269 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/anyio/abc/_sockets.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6598 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/anyio/abc/_streams.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2067 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/anyio/abc/_subprocesses.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2747 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/anyio/abc/_tasks.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1829 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/anyio/abc/_testing.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    15749 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/anyio/from_thread.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4185 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/anyio/lowlevel.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5386 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/anyio/pytest_plugin.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.270388 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/anyio/streams/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)        0 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/anyio/streams/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4500 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/anyio/streams/buffered.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4383 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/anyio/streams/file.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     9296 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/anyio/streams/memory.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4302 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/anyio/streams/stapled.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5094 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/anyio/streams/text.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    12752 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/anyio/streams/tls.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     9535 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/anyio/to_process.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2396 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/anyio/to_thread.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.254368 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/anyio-4.3.0.dist-info/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)       39 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/anyio-4.3.0.dist-info/entry_points.txt
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)        6 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/anyio-4.3.0.dist-info/top_level.txt
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.278398 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/certifi/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)       94 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/certifi/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      243 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/certifi/__main__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4426 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/certifi/core.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.278398 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/certifi-2024.2.2.dist-info/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)        8 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/certifi-2024.2.2.dist-info/top_level.txt
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.282403 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/h11/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1507 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/h11/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4815 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/h11/_abnf.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    26539 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/h11/_connection.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    11816 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/h11/_events.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    10230 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/h11/_headers.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8383 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/h11/_readers.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5252 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/h11/_receivebuffer.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    13300 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/h11/_state.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4888 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/h11/_util.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      686 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/h11/_version.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5081 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/h11/_writers.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.282403 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/h11/tests/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)        0 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/h11/tests/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3355 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/h11/tests/helpers.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3995 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/h11/tests/test_against_stdlib_http.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    38720 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/h11/tests/test_connection.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4657 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/h11/tests/test_events.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5612 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/h11/tests/test_headers.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      794 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/h11/tests/test_helpers.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    16386 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/h11/tests/test_io.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3454 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/h11/tests/test_receivebuffer.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8928 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/h11/tests/test_state.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2970 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/h11/tests/test_util.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.282403 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/h11-0.14.0.dist-info/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1124 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/h11-0.14.0.dist-info/LICENSE.txt
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)        4 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/h11-0.14.0.dist-info/top_level.txt
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.286408 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpcore/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3337 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpcore/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3167 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpcore/_api.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.286408 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpcore/_async/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1221 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpcore/_async/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8484 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpcore/_async/connection.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    15609 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpcore/_async/connection_pool.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    13978 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpcore/_async/http11.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    23881 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpcore/_async/http2.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    14851 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpcore/_async/http_proxy.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4486 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpcore/_async/interfaces.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    13934 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpcore/_async/socks_proxy.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.290413 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpcore/_backends/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)        0 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpcore/_backends/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5295 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpcore/_backends/anyio.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1683 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpcore/_backends/auto.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3218 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpcore/_backends/base.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4179 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpcore/_backends/mock.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8086 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpcore/_backends/sync.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6078 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpcore/_backends/trio.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1185 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpcore/_exceptions.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    16614 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpcore/_models.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      187 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpcore/_ssl.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.290413 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpcore/_sync/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1141 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpcore/_sync/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8273 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpcore/_sync/connection.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    15277 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpcore/_sync/connection_pool.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    13564 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpcore/_sync/http11.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    23345 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpcore/_sync/http2.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    14613 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpcore/_sync/http_proxy.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4365 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpcore/_sync/interfaces.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    13707 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpcore/_sync/socks_proxy.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     9464 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpcore/_synchronization.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3954 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpcore/_trace.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1525 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpcore/_utils.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.306433 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpx/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3210 2024-05-09 12:01:15.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpx/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      108 2024-05-09 12:01:15.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpx/__version__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    12928 2024-05-09 12:01:15.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpx/_api.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    11830 2024-05-09 12:01:15.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpx/_auth.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    67490 2024-05-09 12:01:15.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpx/_client.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1563 2024-05-09 12:01:15.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpx/_compat.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    12204 2024-05-09 12:01:15.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpx/_config.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8047 2024-05-09 12:01:15.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpx/_content.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     9904 2024-05-09 12:01:15.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpx/_decoders.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     7922 2024-05-09 12:01:15.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpx/_exceptions.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    15635 2024-05-09 12:01:15.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpx/_main.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    42303 2024-05-09 12:01:15.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpx/_models.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8885 2024-05-09 12:01:15.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpx/_multipart.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5618 2024-05-09 12:01:15.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpx/_status_codes.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.306433 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpx/_transports/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)        0 2024-05-09 12:01:15.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpx/_transports/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5490 2024-05-09 12:01:15.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpx/_transports/asgi.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2472 2024-05-09 12:01:15.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpx/_transports/base.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    13290 2024-05-09 12:01:15.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpx/_transports/default.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1202 2024-05-09 12:01:15.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpx/_transports/mock.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4795 2024-05-09 12:01:15.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpx/_transports/wsgi.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3391 2024-05-09 12:01:15.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpx/_types.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    17720 2024-05-09 12:01:15.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpx/_urlparse.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    21783 2024-05-09 12:01:15.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpx/_urls.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    13858 2024-05-09 12:01:15.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpx/_utils.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.306433 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpx-0.27.0.dist-info/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)       37 2024-05-09 12:01:15.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpx-0.27.0.dist-info/entry_points.txt
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.318448 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/idna/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      849 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/idna/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3426 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/idna/codec.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      321 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/idna/compat.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    12663 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/idna/core.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    78320 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/idna/idnadata.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1881 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/idna/intranges.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)       21 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/idna/package_data.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)   206503 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/idna/uts46data.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.342478 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      113 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      246 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/_compat.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2364 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/_punycode.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.346484 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/cli/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)        0 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/cli/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2901 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/cli/parse.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.346484 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/common/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)        0 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/common/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      156 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/common/entities.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      932 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/common/html_blocks.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      929 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/common/html_re.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2568 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/common/normalize_url.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    10728 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/common/utils.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.346484 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/helpers/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      253 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/helpers/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1977 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/helpers/parse_link_destination.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1036 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/helpers/parse_link_label.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1425 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/helpers/parse_link_title.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    12772 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/main.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3911 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/parser_block.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1010 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/parser_core.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4997 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/parser_inline.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.346484 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/presets/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      970 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/presets/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2868 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/presets/commonmark.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1810 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/presets/default.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2112 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/presets/zero.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     9970 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/renderer.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     9199 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/ruler.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.350489 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/rules_block/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      553 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/rules_block/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8887 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/rules_block/blockquote.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      859 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/rules_block/code.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2537 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/rules_block/fence.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1746 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/rules_block/heading.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1226 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/rules_block/hr.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2721 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/rules_block/html_block.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2625 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/rules_block/lheading.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     9668 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/rules_block/list.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1818 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/rules_block/paragraph.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6168 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/rules_block/reference.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8422 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/rules_block/state_block.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6987 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/rules_block/table.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.350489 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/rules_core/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      394 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/rules_core/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      372 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/rules_core/block.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      325 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/rules_core/inline.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5141 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/rules_core/linkify.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      402 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/rules_core/normalize.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3470 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/rules_core/replacements.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     7443 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/rules_core/smartquotes.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      570 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/rules_core/state_core.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1172 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/rules_core/text_join.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.354493 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/rules_inline/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      696 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/rules_inline/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2079 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/rules_inline/autolink.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2037 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/rules_inline/backticks.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4851 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/rules_inline/balance_pairs.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3123 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/rules_inline/emphasis.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1651 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/rules_inline/entity.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1658 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/rules_inline/escape.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1493 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/rules_inline/fragments_join.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1130 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/rules_inline/html_inline.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4135 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/rules_inline/image.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4318 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/rules_inline/link.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1704 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/rules_inline/linkify.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1296 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/rules_inline/newline.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5101 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/rules_inline/state_inline.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3214 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/rules_inline/strikethrough.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      901 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/rules_inline/text.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6439 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/token.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    11421 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/tree.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5365 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/utils.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.354493 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it_py-3.0.0.dist-info/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)       58 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it_py-3.0.0.dist-info/entry_points.txt
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.354493 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/mdurl/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      547 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/mdurl/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3004 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/mdurl/_decode.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2602 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/mdurl/_encode.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      626 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/mdurl/_format.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    11374 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/mdurl/_parse.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      284 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/mdurl/_url.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.358499 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      355 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      854 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/__main__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1444 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/__pip-runner__.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.370514 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      573 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    10243 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/build_env.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    10429 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/cache.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.382529 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/cli/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      132 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/cli/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6676 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/cli/autocompletion.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8726 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/cli/base_command.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    30029 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/cli/cmdoptions.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      774 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/cli/command_context.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2816 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/cli/main.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4338 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/cli/main_parser.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    10817 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/cli/parser.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1968 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/cli/progress_bars.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    18328 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/cli/req_command.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5118 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/cli/spinners.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      116 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/cli/status_codes.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.398549 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/commands/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3882 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/commands/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     7581 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/commands/cache.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1782 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/commands/check.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3986 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/commands/completion.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     9815 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/commands/configuration.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6591 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/commands/debug.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5335 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/commands/download.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3243 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/commands/freeze.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1703 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/commands/hash.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1132 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/commands/help.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4793 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/commands/index.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3188 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/commands/inspect.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    28934 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/commands/install.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    12554 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/commands/list.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5697 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/commands/search.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6419 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/commands/show.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3886 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/commands/uninstall.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6476 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/commands/wheel.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    13839 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/configuration.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.402554 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/distributions/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      858 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/distributions/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1221 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/distributions/base.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      729 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/distributions/installed.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6494 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/distributions/sdist.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1164 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/distributions/wheel.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    23737 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/exceptions.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.406559 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/index/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)       30 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/index/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    16504 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/index/collector.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    37873 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/index/package_finder.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6556 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/index/sources.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.410564 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/locations/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    15365 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/locations/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6100 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/locations/_distutils.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     7680 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/locations/_sysconfig.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2556 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/locations/base.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      340 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/main.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.414569 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/metadata/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4280 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/metadata/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2595 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/metadata/_json.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    25277 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/metadata/base.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.414569 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/metadata/importlib/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      107 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/metadata/importlib/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1882 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/metadata/importlib/_compat.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8181 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/metadata/importlib/_dists.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     7435 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/metadata/importlib/_envs.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     9773 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/metadata/pkg_resources.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.430589 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/models/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)       63 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/models/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      990 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/models/candidate.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6931 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/models/direct_url.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2520 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/models/format_control.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1030 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/models/index.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2609 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/models/installation_report.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    20819 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/models/link.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      738 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/models/scheme.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4643 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/models/search_scope.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1907 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/models/selection_prefs.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3858 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/models/target_python.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3600 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/models/wheel.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.434594 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/network/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)       50 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/network/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    20541 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/network/auth.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2145 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/network/cache.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6096 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/network/download.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     7638 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/network/lazy_wheel.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    18442 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/network/session.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4073 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/network/utils.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1791 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/network/xmlrpc.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.434594 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/operations/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)        0 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/operations/__init__.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.442604 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/operations/build/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)        0 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/operations/build/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4133 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/operations/build/build_tracker.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1422 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/operations/build/metadata.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1474 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/operations/build/metadata_editable.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2198 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/operations/build/metadata_legacy.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1075 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/operations/build/wheel.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1417 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/operations/build/wheel_editable.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3064 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/operations/build/wheel_legacy.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6806 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/operations/check.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     9816 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/operations/freeze.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.442604 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/operations/install/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)       51 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/operations/install/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1282 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/operations/install/editable_legacy.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    27475 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/operations/install/wheel.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    28571 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/operations/prepare.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     7161 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/pyproject.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.446610 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/req/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2738 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/req/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    16610 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/req/constructors.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    17872 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/req/req_file.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    33084 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/req/req_install.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4704 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/req/req_set.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    24678 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/req/req_uninstall.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.446610 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/resolution/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)        0 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/resolution/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      583 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/resolution/base.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.446610 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/resolution/legacy/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)        0 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/resolution/legacy/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    24128 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/resolution/legacy/resolver.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.450615 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)        0 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5220 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/base.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    18969 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/candidates.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    27845 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/factory.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5705 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     9824 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/provider.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3100 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/reporter.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5454 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/requirements.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    11642 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/resolver.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8167 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/self_outdated_check.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.474645 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/utils/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)        0 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/utils/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3351 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/utils/_jaraco_text.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1015 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/utils/_log.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1665 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/utils/appdirs.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1884 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/utils/compat.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5377 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/utils/compatibility_tags.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      242 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/utils/datetime.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3627 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/utils/deprecation.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3206 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/utils/direct_url_helpers.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2118 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/utils/egg_link.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1169 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/utils/encoding.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3064 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/utils/entrypoints.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5122 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/utils/filesystem.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      716 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/utils/filetypes.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3113 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/utils/glibc.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5118 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/utils/hashes.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      795 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/utils/inject_securetransport.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    11632 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/utils/logging.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    23344 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/utils/misc.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1193 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/utils/models.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2108 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/utils/packaging.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4435 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/utils/setuptools_build.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     9200 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/utils/subprocess.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     7702 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/utils/temp_dir.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8821 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/utils/unpacking.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1759 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/utils/urls.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3456 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/utils/virtualenv.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4549 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/utils/wheel.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.474645 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/vcs/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      596 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/vcs/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3519 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/vcs/bazaar.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    18116 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/vcs/git.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5244 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/vcs/mercurial.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    11729 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/vcs/subversion.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    22811 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/vcs/versioncontrol.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    11842 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/wheel_builder.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.486660 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4966 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/__init__.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.498675 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      465 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1379 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/_cmd.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5033 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/adapter.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1535 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/cache.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.498675 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/caches/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      242 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/caches/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5271 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1033 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      778 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/compat.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    16416 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/controller.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3946 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/filewrapper.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4154 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/heuristics.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     7105 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/serialize.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      774 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/wrapper.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.502680 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/certifi/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)       94 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/certifi/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      255 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/certifi/__main__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4531 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/certifi/core.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.562756 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4797 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    31274 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/big5freq.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1763 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/big5prober.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    10032 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/chardistribution.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3915 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/charsetgroupprober.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5420 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/charsetprober.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.562756 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/cli/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)        0 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/cli/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3242 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/cli/chardetect.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3732 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/codingstatemachine.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      542 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/codingstatemachinedict.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1860 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/cp949prober.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1683 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/enums.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4006 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/escprober.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    12176 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/escsm.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3934 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/eucjpprober.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    13566 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/euckrfreq.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1753 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/euckrprober.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    36913 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/euctwfreq.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1753 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/euctwprober.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    20735 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/gb2312freq.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1759 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/gb2312prober.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    14537 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/hebrewprober.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    25796 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/jisfreq.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    42498 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/johabfreq.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1752 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/johabprober.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    27055 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/jpcntx.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)   104562 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/langbulgarianmodel.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    98484 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/langgreekmodel.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    98196 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/langhebrewmodel.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)   101363 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/langhungarianmodel.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)   128035 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/langrussianmodel.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)   102774 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/langthaimodel.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    95372 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/langturkishmodel.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5380 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/latin1prober.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6077 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/macromanprober.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3715 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/mbcharsetprober.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2131 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/mbcsgroupprober.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    30391 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/mbcssm.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.562756 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/metadata/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)        0 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/metadata/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    13560 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/metadata/languages.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      402 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/resultdict.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6400 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/sbcharsetprober.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4137 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/sbcsgroupprober.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4007 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/sjisprober.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    14848 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/universaldetector.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8505 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/utf1632prober.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2812 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/utf8prober.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      244 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/version.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.574771 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/colorama/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      266 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/colorama/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2522 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/colorama/ansi.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    11128 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/colorama/ansitowin32.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3325 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/colorama/initialise.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.574771 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)       75 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2839 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/ansi_test.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    10678 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6741 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/initialise_test.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1866 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/isatty_test.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1079 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/utils.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3709 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/winterm_test.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6181 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/colorama/win32.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     7134 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/colorama/winterm.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.586786 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/distlib/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      581 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/distlib/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    41259 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/distlib/compat.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    51697 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/distlib/database.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    20834 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/distlib/index.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    51991 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/distlib/locators.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    14811 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/distlib/manifest.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5058 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/distlib/markers.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    39801 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/distlib/metadata.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    10820 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/distlib/resources.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    18102 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/distlib/scripts.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    66262 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/distlib/util.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    23513 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/distlib/version.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    43898 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/distlib/wheel.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.594796 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/distro/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      981 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/distro/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)       64 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/distro/__main__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    49330 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/distro/distro.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.606811 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/idna/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      849 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/idna/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3374 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/idna/codec.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      321 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/idna/compat.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    12950 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/idna/core.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    44375 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/idna/idnadata.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1881 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/idna/intranges.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)       21 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/idna/package_data.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)   206539 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/idna/uts46data.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.606811 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/msgpack/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1132 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/msgpack/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1081 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/msgpack/exceptions.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6079 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/msgpack/ext.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    34544 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/msgpack/fallback.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.618826 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/packaging/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      661 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/packaging/__about__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      497 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/packaging/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    11488 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/packaging/_manylinux.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4378 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/packaging/_musllinux.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1431 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/packaging/_structures.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8487 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/packaging/markers.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4676 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/packaging/requirements.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    30110 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/packaging/specifiers.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    15699 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/packaging/tags.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4200 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/packaging/utils.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    14665 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/packaging/version.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.618826 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pkg_resources/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)   109364 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pkg_resources/__init__.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.630841 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    20155 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1476 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/__main__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     7211 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/android.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     7132 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/api.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3678 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/macos.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8809 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/unix.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      160 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/version.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     9573 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/windows.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.642856 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pygments/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2983 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pygments/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      353 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pygments/__main__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    23685 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pygments/cmdline.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1697 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pygments/console.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1938 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pygments/filter.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.642856 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pygments/filters/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    40386 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pygments/filters/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4178 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatter.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.646862 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5424 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4176 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/_mapping.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3314 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/bbcode.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5094 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/groff.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    35610 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/html.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    21938 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/img.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4981 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/irc.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    19351 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/latex.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5073 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/other.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2212 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5014 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/rtf.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     7335 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/svg.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4674 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/terminal.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    11753 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/terminal256.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    34618 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pygments/lexer.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.658877 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    12130 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    72281 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/_mapping.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    53424 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/python.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      986 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pygments/modeline.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2591 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pygments/plugin.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3072 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pygments/regexopt.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3092 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pygments/scanner.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6882 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pygments/sphinxext.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6257 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pygments/style.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.658877 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pygments/styles/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3700 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pygments/styles/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6184 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pygments/token.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    63223 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pygments/unistring.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    10230 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pygments/util.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.674897 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     9116 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6567 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/actions.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    13387 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/common.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)   224445 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/core.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.674897 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/diagram/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    24215 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/diagram/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     9523 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/exceptions.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    38646 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/helpers.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    26692 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/results.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    13488 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/testing.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    10646 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/unicode.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8670 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/util.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.674897 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      491 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      138 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_compat.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    11920 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_impl.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.678902 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_in_process/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      546 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    10927 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.682907 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/requests/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5169 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/requests/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      435 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/requests/__version__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1495 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/requests/_internal_utils.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    19697 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/requests/adapters.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6449 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/requests/api.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    10187 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/requests/auth.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      575 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/requests/certs.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1286 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/requests/compat.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    18560 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/requests/cookies.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3823 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/requests/exceptions.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3879 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/requests/help.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      733 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/requests/hooks.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    35288 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/requests/models.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      695 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/requests/packages.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    30373 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/requests/sessions.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4235 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/requests/status_codes.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2912 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/requests/structures.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    33460 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/requests/utils.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.682907 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      537 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/__init__.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.682907 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/compat/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)        0 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/compat/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      156 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/compat/collections_abc.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5871 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/providers.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1601 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/reporters.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    20511 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/resolvers.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4963 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/structs.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.738978 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6090 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8478 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/__main__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    10096 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/_cell_widths.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)   140235 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/_emoji_codes.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1064 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/_emoji_replace.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2100 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/_export_format.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      265 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/_extension.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      799 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/_fileno.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     9695 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/_inspect.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3225 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/_log_render.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1236 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/_loop.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1387 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/_null_file.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     7063 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/_palettes.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      423 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/_pick.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5472 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/_ratio.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    19919 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/_spinners.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      351 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/_stack.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      417 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/_timer.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    22820 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/_win32_console.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1926 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/_windows.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2783 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/_windows_renderer.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1840 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/_wrap.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      890 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/abc.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    10368 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/align.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6906 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/ansi.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3264 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/bar.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     9842 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/box.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4509 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/cells.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    18224 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/color.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1054 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/color_triplet.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     7131 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/columns.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    99218 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/console.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1288 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/constrain.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5497 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/containers.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6630 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/control.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8082 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/default_styles.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      972 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/diagnose.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2501 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/emoji.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      642 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/errors.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1683 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/file_proxy.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2508 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/filesize.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     9584 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/highlighter.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5032 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/json.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3252 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/jupyter.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    14007 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/layout.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    14273 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/live.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3667 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/live_render.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    11903 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/logging.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8198 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/markup.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5305 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/measure.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4970 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/padding.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      828 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/pager.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3396 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/palette.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    10574 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/panel.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    35852 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/pretty.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    59706 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/progress.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8165 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/progress_bar.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    11303 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/prompt.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1391 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/protocol.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      166 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/region.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4431 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/repr.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4602 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/rule.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2843 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/scope.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1591 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/screen.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    24247 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/segment.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4339 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/spinner.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4425 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/status.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    27073 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/style.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1258 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/styled.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    35173 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/syntax.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    39684 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/table.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3370 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/terminal_theme.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    45525 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/text.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3777 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/theme.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      102 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/themes.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    29604 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/traceback.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     9169 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/tree.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    34549 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/six.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.742982 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/tenacity/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    20493 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/tenacity/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3551 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/tenacity/_asyncio.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2179 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/tenacity/_utils.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1682 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/tenacity/after.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1562 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/tenacity/before.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2372 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/tenacity/before_sleep.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1383 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/tenacity/nap.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8746 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/tenacity/retry.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3086 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/tenacity/stop.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2142 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/tenacity/tornadoweb.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8024 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/tenacity/wait.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.742982 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/tomli/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      396 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/tomli/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    22633 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/tomli/_parser.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2943 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/tomli/_re.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      254 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/tomli/_types.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)   111130 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/typing_extensions.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.746988 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3333 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    11372 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/_collections.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)       64 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/_version.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    20300 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/connection.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    40285 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/connectionpool.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.750993 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)        0 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      957 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.750993 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_securetransport/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)        0 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    17632 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    13922 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    11036 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/appengine.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4528 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    17081 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    34448 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/securetransport.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     7097 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/socks.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8217 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/exceptions.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8579 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/fields.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2440 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/filepost.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.754998 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)        0 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/__init__.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.759003 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/backports/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)        0 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/backports/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1417 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5343 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/backports/weakref_finalize.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    34665 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/six.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    19990 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/poolmanager.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5985 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/request.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    30641 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/response.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.767013 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1155 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4901 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/connection.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1605 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/proxy.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      498 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/queue.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3997 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/request.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3510 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/response.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    22013 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/retry.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    17177 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/ssl_.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5758 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6895 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/ssltransport.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    10168 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/timeout.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    14296 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/url.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5403 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/wait.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      475 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/vendor.txt
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.771018 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/webencodings/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    10579 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/webencodings/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8979 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/webencodings/labels.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1305 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/webencodings/mklabels.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6563 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/webencodings/tests.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4307 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/webencodings/x_user_defined.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.358499 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip-23.2.dist-info/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    10065 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip-23.2.dist-info/AUTHORS.txt
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1093 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip-23.2.dist-info/LICENSE.txt
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      125 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip-23.2.dist-info/entry_points.txt
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)        4 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip-23.2.dist-info/top_level.txt
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.771018 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pkg_resources/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)   109429 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pkg_resources/__init__.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.779028 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pkg_resources/_vendor/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)        0 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pkg_resources/_vendor/__init__.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.783033 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      506 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4504 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_adapters.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5457 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_common.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2925 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_compat.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      884 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_itertools.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3481 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_legacy.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5140 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/abc.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3581 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/readers.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2576 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/simple.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.783033 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)        0 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     7460 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/context.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    15056 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/functools.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.783033 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/text/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    15526 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/text/__init__.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.787038 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      148 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)   134976 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/more.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    25416 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/recipes.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.791043 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      501 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3266 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_elffile.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8926 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_manylinux.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2524 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_musllinux.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    10194 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_parser.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1431 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_structures.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5292 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_tokenizer.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8208 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/markers.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    16397 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/metadata.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3287 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/requirements.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    39206 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/specifiers.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    18106 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/tags.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4355 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/utils.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    16326 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/version.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.791043 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    12806 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1164 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/__main__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4068 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/android.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4910 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/api.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2655 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/macos.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6911 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/unix.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      160 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/version.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6596 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/windows.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    80078 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pkg_resources/_vendor/typing_extensions.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8425 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pkg_resources/_vendor/zipp.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.791043 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pkg_resources/extern/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2442 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pkg_resources/extern/__init__.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.799053 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2959 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      348 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/__main__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    23536 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/cmdline.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1718 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/console.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1910 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/filter.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.799053 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/filters/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    40344 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/filters/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4366 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/formatter.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.803058 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/formatters/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5349 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/formatters/__init__.py
+-rwxrwxr-x   0 sifaw     (1000) sifaw     (1000)     4176 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/formatters/_mapping.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3296 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/formatters/bbcode.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5082 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/formatters/groff.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    35633 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/formatters/html.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    23263 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/formatters/img.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4945 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/formatters/irc.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    19258 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/formatters/latex.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4986 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/formatters/other.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2206 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/formatters/pangomarkup.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    11921 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/formatters/rtf.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     7138 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/formatters/svg.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4626 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/formatters/terminal.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    11717 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/formatters/terminal256.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    35109 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexer.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.895174 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    12067 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1543 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/_ada_builtins.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    27287 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/_asy_builtins.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    13994 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/_cl_builtins.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)   105173 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/_cocoa_builtins.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    18414 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/_csound_builtins.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    12446 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/_css_builtins.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    11883 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/_julia_builtins.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)   134510 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/_lasso_builtins.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)   108094 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/_lilypond_builtins.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8108 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/_lua_builtins.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      955 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/_luau_builtins.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    69089 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/_mapping.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    24713 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/_mql_builtins.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    25838 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/_mysql_builtins.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    49398 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/_openedge_builtins.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)   107922 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/_php_builtins.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    13343 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/_postgres_builtins.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    12595 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/_qlik_builtins.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    32564 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/_scheme_builtins.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    52411 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/_scilab_builtins.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    26777 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/_sourcemod_builtins.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    13445 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/_stan_builtins.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    27227 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/_stata_builtins.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    15460 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/_tsql_builtins.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1658 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/_usd_builtins.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4225 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/_vbscript_builtins.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    57066 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/_vim_builtins.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    11727 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/actionscript.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5353 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/ada.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      896 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/agile.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     9912 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/algebra.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2605 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/ambient.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1723 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/amdgpu.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4176 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/ampl.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    30800 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/apdlexer.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3404 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/apl.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    11538 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/archetype.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3564 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/arrow.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    11414 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/arturo.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1693 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/asc.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    41934 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/asm.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4262 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/asn1.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    19831 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/automation.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3020 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/bare.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    27989 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/basic.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1641 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/bdd.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3209 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/berry.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4811 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/bibtex.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6188 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/blueprint.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3921 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/boa.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3337 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/bqn.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    28345 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/business.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    18059 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/c_cpp.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    32021 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/c_like.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2174 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/capnproto.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3211 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/carbon.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5076 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/cddl.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5156 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/chapel.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6418 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/clean.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3179 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/comal.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1426 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/compiled.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    50534 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/configs.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4180 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/console.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1389 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/cplint.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    15754 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/crystal.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    16998 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/csound.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    25366 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/css.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     9920 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/d.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4606 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/dalvik.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    27026 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/data.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8098 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/dax.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4019 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/devicetree.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5382 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/diff.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3891 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/dns.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    37958 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/dotnet.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    36746 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/dsls.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    10391 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/dylan.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6371 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/ecl.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2690 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/eiffel.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3152 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/elm.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6535 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/elpi.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4804 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/email.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    19147 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/erlang.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    10500 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/esoteric.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3272 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/ezhil.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    19530 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/factor.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    10231 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/fantom.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     9655 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/felix.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1644 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/fift.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2667 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/floscript.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     7193 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/forth.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    10382 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/fortran.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    26295 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/foxpro.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    26913 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/freefem.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3700 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/func.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      693 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/functional.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3743 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/futhark.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      874 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/gcodelexer.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     7566 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/gdscript.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3783 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/go.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8043 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/grammar_notation.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4108 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/graph.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    39145 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/graphics.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5601 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/graphql.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1934 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/graphviz.py
+-rwxrwxr-x   0 sifaw     (1000) sifaw     (1000)     3990 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/gsql.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    33239 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/haskell.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    30974 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/haxe.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    22738 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/hdl.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3653 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/hexdump.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    20574 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/html.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    15449 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/idl.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    31626 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/igor.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3135 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/inferno.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    13297 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/installers.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    56544 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/int_fiction.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1905 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/iolang.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4853 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/j.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    63101 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/javascript.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2082 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/jmespath.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3700 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/jslt.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5636 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/jsonnet.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2233 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/jsx.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    11679 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/julia.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    72666 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/jvm.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    11405 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/kuin.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3477 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/kusto.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6551 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/ldap.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8570 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/lean.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     9752 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/lilypond.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)   157668 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/lisp.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    32844 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/macaulay2.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     7831 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/make.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    65088 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/markup.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      695 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/math.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)   132962 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/matlab.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2715 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/maxima.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4336 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/meson.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     7582 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/mime.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    13696 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/minecraft.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4656 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/mips.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    35390 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/ml.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    13683 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/modeling.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    53072 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/modula2.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    24181 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/mojo.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6289 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/monte.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     9297 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/mosel.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    63999 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/ncl.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6413 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/nimrod.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2725 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/nit.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4421 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/nix.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4210 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/oberon.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    23240 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/objective.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2981 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/ooc.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3700 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/openscad.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1763 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/other.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2719 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/parasail.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    26596 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/parsers.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    30989 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/pascal.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8253 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/pawn.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    39192 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/perl.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    23249 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/phix.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    13061 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/php.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1974 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/pointless.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3279 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/pony.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    12676 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/praat.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1155 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/procfile.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    12866 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/prolog.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4738 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/promql.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8747 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/prql.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4501 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/ptx.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    53639 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/python.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6936 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/q.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3693 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/qlik.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6103 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/qvt.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6342 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/r.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    16042 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/rdf.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    18259 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/rebol.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2927 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/resource.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5035 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/ride.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1127 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/rita.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1972 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/rnc.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2074 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/roboconf.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    18448 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/robotframework.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    22753 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/ruby.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8260 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/rust.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     9456 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/sas.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4878 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/savi.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2524 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/scdoc.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    81062 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/scripting.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1985 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/sgf.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    36234 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/shell.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2514 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/sieve.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8484 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/slash.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     7204 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/smalltalk.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2659 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/smithy.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2805 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/smv.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2778 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/snobol.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3163 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/solidity.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2339 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/soong.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3376 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/sophia.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3554 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/special.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2790 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/spice.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    42594 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/sql.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1746 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/srcinfo.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6415 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/stata.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3697 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/supercollider.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    10809 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/tact.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2904 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/tal.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5512 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/tcl.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3522 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/teal.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    75719 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/templates.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     9718 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/teraterm.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    10810 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/testing.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1048 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/text.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     7760 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/textedit.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    15524 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/textfmts.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    17855 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/theorem.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6017 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/thingsdb.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1450 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/tlb.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1540 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/tls.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    10456 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/tnt.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1506 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/trafficscript.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8332 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/typoscript.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4337 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/typst.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    10499 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/ul4.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    18625 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/unicon.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6082 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/urbi.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3304 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/usd.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     7473 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/varnish.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3934 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/verification.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2661 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/verifpal.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5711 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/vip.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5590 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/vyper.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      913 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/web.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5698 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/webassembly.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    10516 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/webidl.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    40564 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/webmisc.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    11880 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/wgsl.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4017 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/whiley.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4076 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/wowtoc.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3229 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/wren.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1943 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/x10.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      925 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/xorg.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4499 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/yang.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2427 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/yara.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3976 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/zig.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1005 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/modeline.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1891 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/plugin.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3072 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/regexopt.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3092 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/scanner.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     7898 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/sphinxext.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6408 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/style.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.907189 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2006 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3312 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/_mapping.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      749 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/abap.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2262 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/algol.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2283 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/algol_nu.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4557 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/arduino.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2195 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/autumn.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1611 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/borland.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1406 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/bw.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2308 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/coffee.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2832 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/colorful.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2588 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/default.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2182 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/dracula.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2535 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/emacs.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2604 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/friendly.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2828 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/friendly_grayscale.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1324 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/fruity.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3590 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/gh_dark.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3387 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/gruvbox.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      737 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/igor.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2404 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/inkpot.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3172 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/lightbulb.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2066 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/lilypond.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3178 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/lovelace.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2443 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/manni.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4201 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/material.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5184 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/monokai.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2805 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/murphy.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2043 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/native.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5391 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/nord.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1719 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/onedark.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5662 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/paraiso_dark.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5668 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/paraiso_light.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2525 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/pastie.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2230 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/perldoc.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2390 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/rainbow_dash.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      964 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/rrt.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1440 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/sas.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4247 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/solarized.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      831 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/staroffice.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1257 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/stata_dark.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1289 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/stata_light.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     7137 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/tango.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1981 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/trac.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2019 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/vim.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1130 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/vs.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1504 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/xcode.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2203 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/zenburn.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6226 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/token.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    63208 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/unistring.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    10031 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/util.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.799053 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments-2.18.0.dist-info/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)       53 2024-05-09 11:44:04.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments-2.18.0.dist-info/entry_points.txt
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.919204 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pyradios/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      316 2024-05-09 12:01:15.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pyradios/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1679 2024-05-09 12:01:15.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pyradios/base_url.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2468 2024-05-09 12:01:15.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pyradios/facets.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    14102 2024-05-09 12:01:15.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pyradios/radios.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2927 2024-05-09 12:01:15.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pyradios/utils.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.919204 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pyradios-2.1.0.dist-info/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)        9 2024-05-09 12:01:15.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pyradios-2.1.0.dist-info/top_level.txt
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.971270 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6066 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8333 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/__main__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    10209 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/_cell_widths.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)   140235 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/_emoji_codes.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1064 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/_emoji_replace.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2128 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/_export_format.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      241 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/_extension.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      799 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/_fileno.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     9695 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/_inspect.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3213 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/_log_render.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1236 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/_loop.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1387 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/_null_file.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     7063 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/_palettes.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      423 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/_pick.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5459 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/_ratio.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    19919 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/_spinners.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      351 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/_stack.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      417 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/_timer.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    22784 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/_win32_console.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1901 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/_windows.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2759 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/_windows_renderer.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3404 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/_wrap.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      878 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/abc.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    10320 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/align.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6906 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/ansi.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3263 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/bar.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    10783 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/box.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4780 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/cells.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    18223 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/color.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1054 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/color_triplet.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     7131 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/columns.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    99101 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/console.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1288 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/constrain.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5502 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/containers.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6606 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/control.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8046 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/default_styles.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      924 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/diagnose.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2465 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/emoji.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      642 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/errors.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1683 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/file_proxy.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2508 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/filesize.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     9585 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/highlighter.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5019 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/json.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3228 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/jupyter.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    13944 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/layout.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    14271 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/live.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3654 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/live_render.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    11891 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/logging.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    26167 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/markdown.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8427 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/markup.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5305 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/measure.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4958 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/padding.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      828 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/pager.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3288 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/palette.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    10705 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/panel.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    35812 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/pretty.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    59703 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/progress.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8164 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/progress_bar.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    11292 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/prompt.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1367 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/protocol.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      166 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/region.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4419 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/repr.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4590 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/rule.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2831 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/scope.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1579 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/screen.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    24210 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/segment.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4339 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/spinner.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4424 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/status.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    27073 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/style.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1234 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/styled.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    35367 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/syntax.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    39644 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/table.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3370 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/terminal_theme.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    47300 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/text.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3777 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/theme.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      102 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/themes.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    29529 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/traceback.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     9107 2024-05-09 11:44:05.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/tree.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.995300 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     9258 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/__init__.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:21.039354 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      359 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5300 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/_collections.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      411 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/_functools.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)       43 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/_log.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      239 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/_macos_compat.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    19616 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/_msvccompiler.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8572 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/archive_util.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    14721 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/bcppcompiler.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    48643 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/ccompiler.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    17861 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/cmd.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:21.047364 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/command/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      430 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/command/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1614 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/command/_framework_compat.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5408 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/command/bdist.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4665 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/command/bdist_dumb.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    22013 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/command/bdist_rpm.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5584 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/command/build.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     7684 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/command/build_clib.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    31503 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/command/build_ext.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    16537 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/command/build_py.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5604 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/command/build_scripts.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4872 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/command/check.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2594 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/command/clean.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    13077 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/command/config.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    30153 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/command/install.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2762 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/command/install_data.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2788 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/command/install_egg_info.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1180 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/command/install_headers.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8409 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/command/install_lib.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1932 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/command/install_scripts.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      672 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/command/py37compat.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    11817 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/command/register.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    19232 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/command/sdist.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     7491 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/command/upload.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4911 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/config.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     9397 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/core.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    11924 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/cygwinccompiler.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      139 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/debug.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3414 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/dep_util.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8072 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/dir_util.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    50174 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/dist.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3589 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/errors.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    10270 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/extension.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    17899 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/fancy_getopt.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8212 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/file_util.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    13715 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/filelist.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1201 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/log.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    30188 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/msvc9compiler.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    23577 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/msvccompiler.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      217 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/py38compat.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      639 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/py39compat.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3495 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/spawn.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    18928 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/sysconfig.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    12085 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/text_file.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    15601 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/unixccompiler.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    18099 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/util.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    12951 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/version.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5205 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/versionpredicate.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2235 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_entry_points.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2433 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_imp.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1468 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_importlib.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      675 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_itertools.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3706 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_normalization.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1056 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_path.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      882 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_reqs.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:21.051369 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)        0 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/__init__.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:21.063384 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    26498 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2454 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_adapters.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      743 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_collections.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1859 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_compat.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2895 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_functools.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2068 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_itertools.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1165 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_meta.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1098 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_py39compat.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2166 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_text.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:21.067389 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      506 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4504 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_adapters.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5457 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_common.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2925 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_compat.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      884 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_itertools.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3481 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_legacy.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5140 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/abc.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3581 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/readers.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2576 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/simple.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:21.071394 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/jaraco/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)        0 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/jaraco/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     7460 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/jaraco/context.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    15053 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/jaraco/functools.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:21.071394 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/jaraco/text/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    15517 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/jaraco/text/__init__.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:21.071394 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)       82 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)   117959 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/more.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    16256 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/recipes.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    15130 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/ordered_set.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:21.083408 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      501 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3266 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/_elffile.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8926 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/_manylinux.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2524 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/_musllinux.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    10194 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/_parser.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1431 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/_structures.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5292 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/_tokenizer.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8208 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/markers.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    16397 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/metadata.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3287 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/requirements.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    39206 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/specifiers.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    18106 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/tags.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4355 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/utils.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    16326 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/version.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:21.083408 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/tomli/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      396 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/tomli/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    22633 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/tomli/_parser.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2943 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/tomli/_re.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      254 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/tomli/_types.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    87149 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/typing_extensions.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8425 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/zipp.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     7331 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/archive_util.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    20091 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/build_meta.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:21.103433 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/command/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      396 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/command/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2383 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/command/alias.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    16559 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/command/bdist_egg.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1309 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/command/bdist_rpm.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6784 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/command/build.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4398 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/command/build_clib.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    17504 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/command/build_ext.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    14997 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/command/build_py.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     6722 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/command/develop.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4242 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/command/dist_info.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    88844 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/command/easy_install.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    33238 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/command/editable_wheel.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    27134 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/command/egg_info.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5627 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/command/install.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3044 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/command/install_egg_info.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5031 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/command/install_lib.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2359 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/command/install_scripts.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      468 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/command/register.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2097 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/command/rotate.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      657 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/command/saveopts.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     7098 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/command/sdist.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4927 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/command/setopt.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8101 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/command/test.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      462 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/command/upload.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     7773 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/command/upload_docs.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:21.103433 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/config/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1498 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/config/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    14195 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/config/_apply_pyprojecttoml.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:21.111443 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1038 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    11266 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/error_reporting.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1153 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/extra_validations.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1612 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_exceptions.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)   274908 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_validations.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     9160 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/formats.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    16401 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/config/expand.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    17490 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/config/pyprojecttoml.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    26184 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/config/setupcfg.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      936 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/dep_util.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5528 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/depends.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    21147 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/discovery.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    46833 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/dist.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2464 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/errors.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5591 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/extension.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:21.111443 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/extern/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2539 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/extern/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4868 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/glob.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4989 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/installer.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      812 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/launch.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1239 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/logging.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4686 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/monkey.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    47495 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/msvc.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3044 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/namespaces.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    38350 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/package_index.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      330 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/py312compat.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    14349 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/sandbox.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      941 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/unicode_utils.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      161 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/version.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3697 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/warnings.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8628 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/wheel.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      719 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/windows_support.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:20.999305 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools-68.1.2.dist-info/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2676 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools-68.1.2.dist-info/entry_points.txt
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)       41 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools-68.1.2.dist-info/top_level.txt
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:21.111443 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/sniffio/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      335 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/sniffio/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2843 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/sniffio/_impl.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:21.115448 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/sniffio/_tests/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)        0 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/sniffio/_tests/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2058 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/sniffio/_tests/test_sniffio.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)       89 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/sniffio/_version.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:21.115448 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/sniffio-1.3.1.dist-info/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)        8 2024-05-09 12:01:14.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/sniffio-1.3.1.dist-info/top_level.txt
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:21.115448 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/wheel/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)       59 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/wheel/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      455 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/wheel/__main__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      746 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/wheel/_setuptools_logging.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    20127 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/wheel/bdist_wheel.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:21.115448 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/wheel/cli/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4250 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/wheel/cli/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     9431 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/wheel/cli/convert.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4338 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/wheel/cli/pack.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5096 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/wheel/cli/tags.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1021 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/wheel/cli/unpack.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    16143 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/wheel/macosx_libfile.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5889 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/wheel/metadata.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      621 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/wheel/util.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:21.115448 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/wheel/vendored/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)        0 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/wheel/vendored/__init__.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:21.119453 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/wheel/vendored/packaging/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)        0 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/wheel/vendored/packaging/__init__.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3266 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/wheel/vendored/packaging/_elffile.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8813 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/wheel/vendored/packaging/_manylinux.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     2524 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/wheel/vendored/packaging/_musllinux.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     9399 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/wheel/vendored/packaging/_parser.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1431 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/wheel/vendored/packaging/_structures.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     5148 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/wheel/vendored/packaging/_tokenizer.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     8161 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/wheel/vendored/packaging/markers.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     3264 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/wheel/vendored/packaging/requirements.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    39047 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/wheel/vendored/packaging/specifiers.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    18065 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/wheel/vendored/packaging/tags.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     4355 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/wheel/vendored/packaging/utils.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)    16295 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/wheel/vendored/packaging/version.py
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)       16 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/wheel/vendored/vendor.txt
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     7748 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/wheel/wheelfile.py
+drwxrwxr-x   0 sifaw     (1000) sifaw     (1000)        0 2024-05-22 16:20:21.115448 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/wheel-0.41.0.dist-info/
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)     1107 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/wheel-0.41.0.dist-info/LICENSE.txt
+-rw-rw-r--   0 sifaw     (1000) sifaw     (1000)      104 2024-05-09 11:43:18.000000 tmuxradio-0.2.34/venv/lib/python3.11/site-packages/wheel-0.41.0.dist-info/entry_points.txt
```

### Comparing `tmuxradio-0.2.33/LICENSE.txt` & `tmuxradio-0.2.34/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/PKG-INFO` & `tmuxradio-0.2.34/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tmuxradio
-Version: 0.2.33
+Version: 0.2.34
 Summary: Playing globe radio station from terminal
 Home-page: http://github.com/sifaw99/terminal_radio
 Author: Lahcen Ouchary
 Author-email: lahcen.ouchary@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
@@ -36,15 +36,15 @@
 Search a station with `radio -s [STATION_NAME]`.
 
 
 
 Change Log
 ============
 
-0.2.33 (May 19, 2024) 
+0.2.34 (May 22, 2024) 
 — — — — — — — — — -- 
 Fixe Bugs and Make Improvements 
 Display Fetched IcyMetadata  
 
 0.1 (May 10, 2024) 
 — — — — — — — — — -- 
 First Release
```

### Comparing `tmuxradio-0.2.33/README.txt` & `tmuxradio-0.2.34/README.txt`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/main.py` & `tmuxradio-0.2.34/main.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/setup.py` & `tmuxradio-0.2.34/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 import io
 
 def required(sfx=""):
     with io.open(f"requirements{sfx}.txt", encoding="utf-8") as f:
         return f.read().splitlines()
 setup(name='tmuxradio',
-      version='0.2.33',
+      version='0.2.34',
       description='Playing globe radio station from terminal',
       long_description=open('README.txt').read() + "\n\n" + open('CHANGELOG.txt').read(),
       long_description_content_type='text/markdown', 
       url='http://github.com/sifaw99/terminal_radio',
       author='Lahcen Ouchary',
       author_email='lahcen.ouchary@gmail.com',
       license='MIT',
```

### Comparing `tmuxradio-0.2.33/src/fplay.py` & `tmuxradio-0.2.34/src/fplay.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,38 +13,32 @@
 	def __init__(self,url,name):
 		self.url = url
 		self.name = name
 
 	def handlePlaying(self):
 		cmd = ["ffplay", "-nodisp", "-i", "-loglevel", "quiet", "-vn", self.url]
 		cmd1 = ["ffprobe", "-v", "quiet", "-print_format", "json", "-show_format", "-show_entries", "format=icy", "-pretty", self.url]
-		
 		try:
 			console = Console()
 			panel = Panel(Text(f"{self.name}",justify="center"), title= ":play_button:[bold yellow] Playing Now", subtitle= "[blink]:radio:", title_align="center", width=83)
 			console.print(panel)
 			playingProc = subprocess.Popen(cmd, shell=False)
 			try:
 				while True:
-					streamTitle = ''
-					dataProc = subprocess.check_output(cmd1)
-					streamInfos = json.loads(dataProc)
-					streamTitle = streamInfos['format']['tags']['StreamTitle']
 					userResponse = console.input("[bold red] Want playing song infos[/] (y/n) ")
 					if(userResponse == 'y'):
-						if(streamTitle):
+						dataProc = subprocess.check_output(cmd1)
+						streamInfos = json.loads(dataProc)
+						streamTitle = streamInfos.get("format", {}).get("tags", {}).get("StreamTitle", "")
+						if streamTitle != "" or streamTitle != null:
                            				print(f" Track title 🎶: [bold]{streamTitle}")
 						else:
 							print(' Unknow Song')
-
 					else:
-						print(' You can try again')
-					time.sleep(5)
+						print(' You can try again')		
 			except:
 				dataProc.kill()
-
-
 		except:
 			print("Exit Playing Radio")
 			playingProc.kill()
```

### Comparing `tmuxradio-0.2.33/src/fprobe.py` & `tmuxradio-0.2.34/src/fprobe.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/src/main.py` & `tmuxradio-0.2.34/src/main.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/src/utilities.py` & `tmuxradio-0.2.34/src/utilities.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/tmuxradio.egg-info/PKG-INFO` & `tmuxradio-0.2.34/tmuxradio.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tmuxradio
-Version: 0.2.33
+Version: 0.2.34
 Summary: Playing globe radio station from terminal
 Home-page: http://github.com/sifaw99/terminal_radio
 Author: Lahcen Ouchary
 Author-email: lahcen.ouchary@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
@@ -36,15 +36,15 @@
 Search a station with `radio -s [STATION_NAME]`.
 
 
 
 Change Log
 ============
 
-0.2.33 (May 19, 2024) 
+0.2.34 (May 22, 2024) 
 — — — — — — — — — -- 
 Fixe Bugs and Make Improvements 
 Display Fetched IcyMetadata  
 
 0.1 (May 10, 2024) 
 — — — — — — — — — -- 
 First Release
```

### Comparing `tmuxradio-0.2.33/tmuxradio.egg-info/SOURCES.txt` & `tmuxradio-0.2.34/tmuxradio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/bin/activate_this.py` & `tmuxradio-0.2.34/venv/bin/activate_this.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/_distutils_hack/__init__.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/_distutils_hack/__init__.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/_virtualenv.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/_virtualenv.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/anyio/__init__.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/anyio/__init__.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/anyio/_backends/_asyncio.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/anyio/_backends/_asyncio.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/anyio/_backends/_trio.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/anyio/_backends/_trio.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/anyio/_core/_eventloop.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/anyio/_core/_eventloop.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/anyio/_core/_exceptions.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/anyio/_core/_exceptions.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/anyio/_core/_fileio.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/anyio/_core/_fileio.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/anyio/_core/_signals.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/anyio/_core/_signals.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/anyio/_core/_sockets.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/anyio/_core/_sockets.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/anyio/_core/_streams.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/anyio/_core/_streams.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/anyio/_core/_subprocesses.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/anyio/_core/_subprocesses.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/anyio/_core/_synchronization.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/anyio/_core/_synchronization.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/anyio/_core/_tasks.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/anyio/_core/_tasks.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/anyio/_core/_testing.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/anyio/_core/_testing.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/anyio/_core/_typedattr.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/anyio/_core/_typedattr.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/anyio/abc/__init__.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/anyio/abc/__init__.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/anyio/abc/_eventloop.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/anyio/abc/_eventloop.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/anyio/abc/_resources.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/anyio/abc/_resources.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/anyio/abc/_sockets.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/anyio/abc/_sockets.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/anyio/abc/_streams.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/anyio/abc/_streams.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/anyio/abc/_subprocesses.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/anyio/abc/_subprocesses.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/anyio/abc/_tasks.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/anyio/abc/_tasks.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/anyio/abc/_testing.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/anyio/abc/_testing.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/anyio/from_thread.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/anyio/from_thread.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/anyio/lowlevel.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/anyio/lowlevel.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/anyio/pytest_plugin.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/anyio/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/anyio/streams/buffered.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/anyio/streams/buffered.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/anyio/streams/file.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/anyio/streams/file.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/anyio/streams/memory.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/anyio/streams/memory.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/anyio/streams/stapled.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/anyio/streams/stapled.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/anyio/streams/text.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/anyio/streams/text.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/anyio/streams/tls.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/anyio/streams/tls.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/anyio/to_process.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/anyio/to_process.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/anyio/to_thread.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/anyio/to_thread.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/certifi/core.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/certifi/core.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/h11/__init__.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/h11/__init__.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/h11/_abnf.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/h11/_abnf.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/h11/_connection.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/h11/_connection.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/h11/_events.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/h11/_events.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/h11/_headers.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/h11/_headers.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/h11/_readers.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/h11/_readers.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/h11/_receivebuffer.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/h11/_receivebuffer.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/h11/_state.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/h11/_state.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/h11/_util.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/h11/_util.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/h11/_version.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/h11/_version.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/h11/_writers.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/h11/_writers.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/h11/tests/helpers.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/h11/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/h11/tests/test_against_stdlib_http.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/h11/tests/test_against_stdlib_http.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/h11/tests/test_connection.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/h11/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/h11/tests/test_events.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/h11/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/h11/tests/test_headers.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/h11/tests/test_headers.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/h11/tests/test_helpers.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/h11/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/h11/tests/test_io.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/h11/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/h11/tests/test_receivebuffer.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/h11/tests/test_receivebuffer.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/h11/tests/test_state.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/h11/tests/test_state.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/h11/tests/test_util.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/h11/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/h11-0.14.0.dist-info/LICENSE.txt` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/h11-0.14.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpcore/__init__.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpcore/__init__.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpcore/_api.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpcore/_api.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpcore/_async/__init__.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpcore/_async/__init__.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpcore/_async/connection.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpcore/_async/connection.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpcore/_async/connection_pool.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpcore/_async/connection_pool.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpcore/_async/http11.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpcore/_async/http11.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpcore/_async/http2.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpcore/_async/http2.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpcore/_async/http_proxy.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpcore/_async/http_proxy.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpcore/_async/interfaces.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpcore/_async/interfaces.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpcore/_async/socks_proxy.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpcore/_async/socks_proxy.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpcore/_backends/anyio.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpcore/_backends/anyio.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpcore/_backends/auto.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpcore/_backends/auto.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpcore/_backends/base.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpcore/_backends/base.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpcore/_backends/mock.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpcore/_backends/mock.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpcore/_backends/sync.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpcore/_backends/sync.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpcore/_backends/trio.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpcore/_backends/trio.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpcore/_exceptions.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpcore/_exceptions.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpcore/_models.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpcore/_models.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpcore/_sync/__init__.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpcore/_sync/__init__.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpcore/_sync/connection.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpcore/_sync/connection.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpcore/_sync/connection_pool.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpcore/_sync/connection_pool.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpcore/_sync/http11.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpcore/_sync/http11.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpcore/_sync/http2.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpcore/_sync/http2.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpcore/_sync/http_proxy.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpcore/_sync/http_proxy.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpcore/_sync/interfaces.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpcore/_sync/interfaces.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpcore/_sync/socks_proxy.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpcore/_sync/socks_proxy.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpcore/_synchronization.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpcore/_synchronization.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpcore/_trace.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpcore/_trace.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpcore/_utils.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpcore/_utils.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpx/__init__.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpx/__init__.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpx/_api.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpx/_api.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpx/_auth.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpx/_auth.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpx/_client.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpx/_client.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpx/_compat.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpx/_compat.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpx/_config.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpx/_config.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpx/_content.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpx/_content.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpx/_decoders.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpx/_decoders.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpx/_exceptions.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpx/_exceptions.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpx/_main.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpx/_main.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpx/_models.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpx/_models.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpx/_multipart.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpx/_multipart.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpx/_status_codes.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpx/_status_codes.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpx/_transports/asgi.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpx/_transports/asgi.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpx/_transports/base.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpx/_transports/base.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpx/_transports/default.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpx/_transports/default.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpx/_transports/mock.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpx/_transports/mock.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpx/_transports/wsgi.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpx/_transports/wsgi.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpx/_types.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpx/_types.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpx/_urlparse.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpx/_urlparse.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpx/_urls.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpx/_urls.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/httpx/_utils.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/httpx/_utils.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/idna/__init__.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/idna/__init__.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/idna/codec.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/idna/codec.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/idna/core.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/idna/core.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/idna/idnadata.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/idna/idnadata.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/idna/intranges.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/idna/intranges.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/idna/uts46data.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/idna/uts46data.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/_punycode.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/_punycode.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/cli/parse.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/cli/parse.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/common/html_blocks.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/common/html_blocks.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/common/html_re.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/common/html_re.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/common/normalize_url.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/common/normalize_url.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/common/utils.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/common/utils.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/helpers/parse_link_destination.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/helpers/parse_link_destination.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/helpers/parse_link_label.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/helpers/parse_link_label.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/helpers/parse_link_title.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/helpers/parse_link_title.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/main.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/main.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/parser_block.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/parser_block.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/parser_core.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/parser_core.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/parser_inline.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/parser_inline.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/presets/__init__.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/presets/__init__.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/presets/commonmark.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/presets/commonmark.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/presets/default.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/presets/default.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/presets/zero.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/presets/zero.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/renderer.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/renderer.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/ruler.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/ruler.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/rules_block/__init__.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/rules_block/__init__.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/rules_block/blockquote.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/rules_block/blockquote.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/rules_block/code.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/rules_block/code.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/rules_block/fence.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/rules_block/fence.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/rules_block/heading.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/rules_block/heading.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/rules_block/hr.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/rules_block/hr.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/rules_block/html_block.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/rules_block/html_block.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/rules_block/lheading.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/rules_block/lheading.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/rules_block/list.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/rules_block/list.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/rules_block/paragraph.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/rules_block/paragraph.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/rules_block/reference.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/rules_block/reference.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/rules_block/state_block.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/rules_block/state_block.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/rules_block/table.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/rules_block/table.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/rules_core/linkify.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/rules_core/linkify.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/rules_core/replacements.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/rules_core/replacements.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/rules_core/smartquotes.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/rules_core/smartquotes.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/rules_core/state_core.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/rules_core/state_core.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/rules_core/text_join.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/rules_core/text_join.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/rules_inline/__init__.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/rules_inline/__init__.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/rules_inline/autolink.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/rules_inline/autolink.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/rules_inline/backticks.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/rules_inline/backticks.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/rules_inline/balance_pairs.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/rules_inline/balance_pairs.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/rules_inline/emphasis.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/rules_inline/emphasis.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/rules_inline/entity.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/rules_inline/entity.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/rules_inline/escape.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/rules_inline/escape.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/rules_inline/fragments_join.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/rules_inline/fragments_join.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/rules_inline/html_inline.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/rules_inline/html_inline.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/rules_inline/image.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/rules_inline/image.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/rules_inline/link.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/rules_inline/link.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/rules_inline/linkify.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/rules_inline/linkify.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/rules_inline/newline.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/rules_inline/newline.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/rules_inline/state_inline.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/rules_inline/state_inline.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/rules_inline/strikethrough.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/rules_inline/strikethrough.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/rules_inline/text.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/rules_inline/text.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/token.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/token.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/tree.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/tree.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/markdown_it/utils.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/markdown_it/utils.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/mdurl/__init__.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/mdurl/__init__.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/mdurl/_decode.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/mdurl/_decode.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/mdurl/_encode.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/mdurl/_encode.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/mdurl/_format.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/mdurl/_format.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/mdurl/_parse.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/mdurl/_parse.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/__main__.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/__main__.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/__pip-runner__.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/__pip-runner__.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/__init__.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/__init__.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/build_env.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/build_env.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/cache.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/cache.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/cli/autocompletion.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/cli/autocompletion.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/cli/base_command.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/cli/base_command.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/cli/cmdoptions.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/cli/cmdoptions.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/cli/command_context.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/cli/command_context.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/cli/main.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/cli/main.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/cli/main_parser.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/cli/main_parser.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/cli/parser.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/cli/parser.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/cli/progress_bars.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/cli/progress_bars.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/cli/req_command.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/cli/req_command.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/cli/spinners.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/cli/spinners.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/commands/__init__.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/commands/cache.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/commands/cache.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/commands/check.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/commands/check.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/commands/completion.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/commands/completion.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/commands/configuration.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/commands/configuration.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/commands/debug.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/commands/debug.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/commands/download.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/commands/download.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/commands/freeze.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/commands/freeze.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/commands/hash.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/commands/hash.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/commands/help.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/commands/help.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/commands/index.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/commands/index.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/commands/inspect.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/commands/inspect.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/commands/install.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/commands/install.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/commands/list.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/commands/list.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/commands/search.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/commands/search.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/commands/show.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/commands/show.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/commands/uninstall.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/commands/uninstall.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/commands/wheel.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/commands/wheel.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/configuration.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/configuration.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/distributions/__init__.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/distributions/__init__.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/distributions/base.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/distributions/base.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/distributions/installed.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/distributions/installed.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/distributions/sdist.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/distributions/sdist.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/distributions/wheel.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/distributions/wheel.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/exceptions.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/exceptions.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/index/collector.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/index/collector.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/index/package_finder.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/index/package_finder.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/index/sources.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/index/sources.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/locations/__init__.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/locations/__init__.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/locations/_distutils.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/locations/_distutils.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/locations/_sysconfig.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/locations/_sysconfig.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/locations/base.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/locations/base.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/metadata/__init__.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/metadata/_json.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/metadata/_json.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/metadata/base.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/metadata/base.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/metadata/importlib/_compat.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/metadata/importlib/_compat.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/metadata/importlib/_dists.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/metadata/importlib/_dists.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/metadata/importlib/_envs.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/metadata/importlib/_envs.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/metadata/pkg_resources.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/metadata/pkg_resources.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/models/candidate.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/models/candidate.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/models/direct_url.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/models/direct_url.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/models/format_control.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/models/format_control.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/models/index.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/models/index.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/models/installation_report.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/models/installation_report.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/models/link.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/models/link.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/models/scheme.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/models/scheme.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/models/search_scope.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/models/search_scope.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/models/selection_prefs.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/models/selection_prefs.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/models/target_python.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/models/target_python.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/models/wheel.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/models/wheel.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/network/auth.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/network/auth.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/network/cache.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/network/cache.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/network/download.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/network/download.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/network/lazy_wheel.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/network/lazy_wheel.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/network/session.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/network/session.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/network/utils.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/network/utils.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/network/xmlrpc.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/network/xmlrpc.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/operations/build/build_tracker.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/operations/build/build_tracker.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/operations/build/metadata.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/operations/build/metadata.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/operations/build/metadata_editable.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/operations/build/metadata_editable.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/operations/build/metadata_legacy.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/operations/build/metadata_legacy.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/operations/build/wheel.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/operations/build/wheel.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/operations/build/wheel_editable.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/operations/build/wheel_editable.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/operations/build/wheel_legacy.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/operations/build/wheel_legacy.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/operations/check.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/operations/check.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/operations/freeze.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/operations/freeze.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/operations/install/editable_legacy.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/operations/install/editable_legacy.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/operations/install/wheel.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/operations/install/wheel.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/operations/prepare.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/operations/prepare.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/pyproject.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/pyproject.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/req/__init__.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/req/__init__.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/req/constructors.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/req/constructors.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/req/req_file.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/req/req_file.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/req/req_install.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/req/req_install.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/req/req_set.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/req/req_set.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/req/req_uninstall.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/req/req_uninstall.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/resolution/base.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/resolution/base.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/resolution/legacy/resolver.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/resolution/legacy/resolver.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/base.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/base.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/candidates.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/candidates.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/factory.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/factory.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/provider.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/provider.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/reporter.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/reporter.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/requirements.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/requirements.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/resolver.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/resolution/resolvelib/resolver.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/self_outdated_check.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/self_outdated_check.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/utils/_jaraco_text.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/utils/_jaraco_text.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/utils/_log.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/utils/_log.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/utils/appdirs.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/utils/appdirs.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/utils/compat.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/utils/compat.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/utils/compatibility_tags.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/utils/compatibility_tags.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/utils/deprecation.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/utils/direct_url_helpers.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/utils/direct_url_helpers.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/utils/egg_link.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/utils/egg_link.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/utils/encoding.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/utils/entrypoints.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/utils/entrypoints.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/utils/filesystem.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/utils/filetypes.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/utils/filetypes.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/utils/glibc.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/utils/glibc.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/utils/hashes.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/utils/hashes.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/utils/inject_securetransport.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/utils/inject_securetransport.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/utils/logging.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/utils/logging.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/utils/misc.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/utils/misc.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/utils/models.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/utils/models.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/utils/packaging.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/utils/packaging.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/utils/setuptools_build.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/utils/setuptools_build.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/utils/subprocess.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/utils/subprocess.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/utils/temp_dir.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/utils/temp_dir.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/utils/unpacking.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/utils/unpacking.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/utils/urls.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/utils/urls.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/utils/virtualenv.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/utils/virtualenv.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/utils/wheel.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/utils/wheel.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/vcs/__init__.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/vcs/__init__.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/vcs/bazaar.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/vcs/bazaar.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/vcs/git.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/vcs/git.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/vcs/mercurial.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/vcs/mercurial.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/vcs/subversion.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/vcs/subversion.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/vcs/versioncontrol.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/vcs/versioncontrol.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_internal/wheel_builder.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_internal/wheel_builder.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/__init__.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/__init__.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/_cmd.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/_cmd.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/adapter.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/adapter.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/cache.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/cache.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/compat.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/compat.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/controller.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/controller.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/filewrapper.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/filewrapper.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/heuristics.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/heuristics.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/serialize.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/serialize.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/wrapper.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/cachecontrol/wrapper.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/certifi/core.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/certifi/core.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/__init__.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/__init__.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/big5freq.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/big5freq.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/big5prober.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/big5prober.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/chardistribution.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/chardistribution.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/charsetgroupprober.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/charsetgroupprober.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/charsetprober.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/charsetprober.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/cli/chardetect.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/cli/chardetect.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/codingstatemachine.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/codingstatemachine.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/codingstatemachinedict.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/codingstatemachinedict.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/cp949prober.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/cp949prober.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/enums.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/enums.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/escprober.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/escprober.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/escsm.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/escsm.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/eucjpprober.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/eucjpprober.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/euckrfreq.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/euckrfreq.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/euckrprober.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/euckrprober.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/euctwfreq.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/euctwfreq.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/euctwprober.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/euctwprober.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/gb2312freq.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/gb2312freq.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/gb2312prober.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/gb2312prober.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/hebrewprober.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/hebrewprober.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/jisfreq.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/jisfreq.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/johabfreq.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/johabfreq.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/johabprober.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/johabprober.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/jpcntx.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/jpcntx.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/langbulgarianmodel.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/langbulgarianmodel.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/langgreekmodel.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/langgreekmodel.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/langhebrewmodel.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/langhebrewmodel.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/langhungarianmodel.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/langhungarianmodel.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/langrussianmodel.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/langrussianmodel.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/langthaimodel.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/langthaimodel.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/langturkishmodel.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/langturkishmodel.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/latin1prober.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/latin1prober.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/macromanprober.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/macromanprober.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/mbcharsetprober.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/mbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/mbcsgroupprober.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/mbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/mbcssm.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/mbcssm.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/metadata/languages.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/metadata/languages.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/sbcharsetprober.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/sbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/sbcsgroupprober.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/sbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/sjisprober.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/sjisprober.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/universaldetector.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/universaldetector.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/utf1632prober.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/utf1632prober.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/chardet/utf8prober.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/chardet/utf8prober.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/colorama/ansi.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/colorama/ansi.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/colorama/ansitowin32.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/colorama/ansitowin32.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/colorama/initialise.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/colorama/initialise.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/ansi_test.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/ansi_test.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/initialise_test.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/initialise_test.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/isatty_test.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/isatty_test.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/utils.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/utils.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/winterm_test.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/colorama/tests/winterm_test.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/colorama/win32.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/colorama/win32.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/colorama/winterm.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/colorama/winterm.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/distlib/__init__.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/distlib/__init__.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/distlib/compat.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/distlib/compat.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/distlib/database.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/distlib/database.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/distlib/index.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/distlib/index.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/distlib/locators.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/distlib/locators.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/distlib/manifest.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/distlib/manifest.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/distlib/markers.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/distlib/markers.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/distlib/metadata.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/distlib/metadata.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/distlib/resources.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/distlib/resources.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/distlib/scripts.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/distlib/scripts.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/distlib/util.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/distlib/util.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/distlib/version.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/distlib/version.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/distlib/wheel.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/distlib/wheel.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/distro/__init__.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/distro/__init__.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/distro/distro.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/distro/distro.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/idna/__init__.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/idna/__init__.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/idna/codec.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/idna/codec.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/idna/core.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/idna/core.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/idna/idnadata.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/idna/idnadata.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/idna/intranges.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/idna/intranges.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/idna/uts46data.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/idna/uts46data.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/msgpack/__init__.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/msgpack/__init__.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/msgpack/exceptions.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/msgpack/exceptions.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/msgpack/ext.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/msgpack/ext.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/msgpack/fallback.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/msgpack/fallback.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/packaging/__about__.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/packaging/__about__.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/packaging/_manylinux.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/packaging/_musllinux.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/packaging/_structures.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/packaging/markers.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/packaging/requirements.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/packaging/specifiers.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/packaging/tags.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/packaging/utils.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/packaging/version.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pkg_resources/__init__.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pkg_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/__init__.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/__init__.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/__main__.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/__main__.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/android.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/android.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/api.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/api.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/macos.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/macos.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/unix.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/unix.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/windows.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/platformdirs/windows.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pygments/__init__.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pygments/__init__.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pygments/cmdline.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pygments/cmdline.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pygments/console.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pygments/console.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pygments/filter.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pygments/filter.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pygments/filters/__init__.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pygments/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatter.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatter.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/__init__.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/__init__.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/_mapping.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/_mapping.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/bbcode.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/bbcode.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/groff.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/groff.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/html.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/html.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/img.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/img.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/irc.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/irc.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/latex.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/latex.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/other.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/other.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/rtf.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/rtf.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/svg.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/svg.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/terminal.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/terminal.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/terminal256.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pygments/formatters/terminal256.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pygments/lexer.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pygments/lexer.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/__init__.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/__init__.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/_mapping.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/_mapping.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/python.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pygments/lexers/python.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pygments/modeline.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pygments/modeline.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pygments/plugin.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pygments/plugin.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pygments/regexopt.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pygments/regexopt.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pygments/scanner.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pygments/scanner.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pygments/sphinxext.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pygments/sphinxext.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pygments/style.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pygments/style.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pygments/styles/__init__.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pygments/styles/__init__.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pygments/token.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pygments/token.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pygments/unistring.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pygments/unistring.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pygments/util.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pygments/util.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/__init__.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/__init__.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/actions.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/actions.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/common.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/common.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/core.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/core.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/diagram/__init__.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/diagram/__init__.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/exceptions.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/exceptions.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/helpers.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/helpers.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/results.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/results.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/testing.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/testing.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/unicode.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/unicode.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/util.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pyparsing/util.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_impl.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_impl.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/requests/__init__.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/requests/_internal_utils.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/requests/_internal_utils.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/requests/adapters.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/requests/adapters.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/requests/api.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/requests/api.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/requests/auth.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/requests/auth.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/requests/certs.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/requests/certs.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/requests/compat.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/requests/compat.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/requests/cookies.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/requests/cookies.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/requests/exceptions.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/requests/exceptions.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/requests/help.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/requests/help.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/requests/hooks.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/requests/hooks.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/requests/models.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/requests/models.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/requests/packages.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/requests/packages.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/requests/sessions.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/requests/sessions.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/requests/status_codes.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/requests/status_codes.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/requests/structures.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/requests/structures.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/requests/utils.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/requests/utils.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/__init__.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/__init__.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/providers.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/providers.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/reporters.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/reporters.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/resolvers.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/resolvers.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/structs.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/resolvelib/structs.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/__init__.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/__init__.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/__main__.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/__main__.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/_cell_widths.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/_cell_widths.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/_emoji_codes.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/_emoji_codes.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/_emoji_replace.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/_emoji_replace.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/_export_format.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/_export_format.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/_fileno.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/_fileno.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/_inspect.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/_inspect.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/_log_render.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/_log_render.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/_loop.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/_loop.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/_null_file.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/_null_file.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/_palettes.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/_palettes.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/_ratio.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/_ratio.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/_spinners.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/_spinners.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/_win32_console.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/_win32_console.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/_windows.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/_windows.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/_windows_renderer.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/_windows_renderer.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/_wrap.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/_wrap.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/abc.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/abc.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/align.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/align.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/ansi.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/ansi.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/bar.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/bar.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/box.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/box.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/cells.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/cells.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/color.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/color.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/color_triplet.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/color_triplet.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/columns.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/columns.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/console.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/console.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/constrain.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/constrain.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/containers.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/containers.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/control.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/control.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/default_styles.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/default_styles.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/diagnose.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/diagnose.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/emoji.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/emoji.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/errors.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/errors.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/file_proxy.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/file_proxy.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/filesize.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/filesize.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/highlighter.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/highlighter.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/json.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/json.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/jupyter.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/jupyter.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/layout.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/layout.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/live.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/live.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/live_render.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/live_render.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/logging.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/logging.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/markup.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/markup.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/measure.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/measure.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/padding.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/padding.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/pager.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/pager.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/palette.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/palette.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/panel.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/panel.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/pretty.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/pretty.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/progress.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/progress.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/progress_bar.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/progress_bar.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/prompt.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/prompt.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/protocol.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/protocol.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/repr.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/repr.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/rule.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/rule.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/scope.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/scope.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/screen.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/screen.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/segment.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/segment.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/spinner.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/spinner.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/status.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/status.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/style.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/style.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/styled.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/styled.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/syntax.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/syntax.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/table.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/table.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/terminal_theme.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/terminal_theme.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/text.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/text.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/theme.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/theme.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/traceback.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/traceback.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/rich/tree.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/rich/tree.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/six.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/six.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/tenacity/__init__.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/tenacity/__init__.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/tenacity/_asyncio.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/tenacity/_asyncio.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/tenacity/_utils.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/tenacity/_utils.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/tenacity/after.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/tenacity/after.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/tenacity/before.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/tenacity/before.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/tenacity/before_sleep.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/tenacity/before_sleep.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/tenacity/nap.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/tenacity/nap.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/tenacity/retry.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/tenacity/retry.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/tenacity/stop.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/tenacity/stop.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/tenacity/tornadoweb.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/tenacity/tornadoweb.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/tenacity/wait.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/tenacity/wait.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/tomli/_parser.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/tomli/_parser.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/tomli/_re.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/tomli/_re.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/typing_extensions.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/typing_extensions.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/__init__.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/__init__.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/_collections.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/_collections.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/connection.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/connection.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/connectionpool.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/connectionpool.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/appengine.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/appengine.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/securetransport.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/securetransport.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/socks.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/contrib/socks.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/exceptions.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/exceptions.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/fields.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/fields.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/filepost.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/filepost.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/backports/weakref_finalize.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/backports/weakref_finalize.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/six.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/packages/six.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/poolmanager.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/poolmanager.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/request.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/request.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/response.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/response.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/__init__.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/__init__.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/connection.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/connection.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/proxy.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/proxy.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/request.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/request.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/response.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/response.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/retry.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/retry.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/ssl_.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/ssl_.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/ssltransport.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/ssltransport.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/timeout.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/timeout.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/url.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/url.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/wait.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/urllib3/util/wait.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/webencodings/__init__.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/webencodings/__init__.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/webencodings/labels.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/webencodings/labels.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/webencodings/mklabels.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/webencodings/mklabels.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/webencodings/tests.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/webencodings/tests.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip/_vendor/webencodings/x_user_defined.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip/_vendor/webencodings/x_user_defined.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip-23.2.dist-info/AUTHORS.txt` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip-23.2.dist-info/AUTHORS.txt`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pip-23.2.dist-info/LICENSE.txt` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pip-23.2.dist-info/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pkg_resources/__init__.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pkg_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_adapters.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_adapters.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_common.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_common.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_compat.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_compat.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_itertools.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_itertools.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_legacy.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/_legacy.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/abc.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/abc.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/readers.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/readers.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/simple.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pkg_resources/_vendor/importlib_resources/simple.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/context.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/context.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/functools.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/functools.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/text/__init__.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pkg_resources/_vendor/jaraco/text/__init__.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/more.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/more.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/recipes.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pkg_resources/_vendor/more_itertools/recipes.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_elffile.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_elffile.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_manylinux.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_musllinux.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_parser.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_parser.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_structures.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_tokenizer.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/_tokenizer.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/markers.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/metadata.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/metadata.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/requirements.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/specifiers.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/tags.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/utils.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/version.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pkg_resources/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/__init__.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/__init__.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/__main__.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/__main__.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/android.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/android.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/api.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/api.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/macos.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/macos.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/unix.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/unix.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/windows.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pkg_resources/_vendor/platformdirs/windows.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pkg_resources/_vendor/typing_extensions.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pkg_resources/_vendor/typing_extensions.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pkg_resources/_vendor/zipp.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pkg_resources/_vendor/zipp.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pkg_resources/extern/__init__.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pkg_resources/extern/__init__.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/__init__.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/__init__.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/cmdline.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/cmdline.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/console.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/console.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/filter.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/filter.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/filters/__init__.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/formatter.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/formatter.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/formatters/__init__.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/formatters/__init__.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/formatters/_mapping.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/formatters/_mapping.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/formatters/bbcode.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/formatters/bbcode.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/formatters/groff.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/formatters/groff.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/formatters/html.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/formatters/html.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/formatters/img.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/formatters/img.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/formatters/irc.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/formatters/irc.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/formatters/latex.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/formatters/latex.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/formatters/other.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/formatters/other.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/formatters/pangomarkup.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/formatters/pangomarkup.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/formatters/rtf.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/formatters/rtf.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/formatters/svg.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/formatters/svg.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/formatters/terminal.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/formatters/terminal.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/formatters/terminal256.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/formatters/terminal256.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexer.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexer.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/__init__.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/__init__.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/_ada_builtins.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/_ada_builtins.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/_asy_builtins.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/_asy_builtins.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/_cl_builtins.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/_cl_builtins.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/_cocoa_builtins.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/_cocoa_builtins.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/_csound_builtins.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/_csound_builtins.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/_css_builtins.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/_css_builtins.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/_julia_builtins.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/_julia_builtins.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/_lasso_builtins.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/_lasso_builtins.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/_lilypond_builtins.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/_lilypond_builtins.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/_lua_builtins.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/_lua_builtins.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/_luau_builtins.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/_luau_builtins.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/_mapping.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/_mapping.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/_mql_builtins.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/_mql_builtins.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/_mysql_builtins.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/_mysql_builtins.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/_openedge_builtins.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/_openedge_builtins.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/_php_builtins.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/_php_builtins.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/_postgres_builtins.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/_postgres_builtins.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/_qlik_builtins.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/_qlik_builtins.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/_scheme_builtins.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/_scheme_builtins.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/_scilab_builtins.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/_scilab_builtins.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/_sourcemod_builtins.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/_sourcemod_builtins.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/_stan_builtins.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/_stan_builtins.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/_stata_builtins.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/_stata_builtins.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/_tsql_builtins.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/_tsql_builtins.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/_usd_builtins.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/_usd_builtins.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/_vbscript_builtins.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/_vbscript_builtins.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/_vim_builtins.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/_vim_builtins.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/actionscript.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/actionscript.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/ada.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/ada.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/agile.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/agile.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/algebra.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/algebra.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/ambient.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/ambient.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/amdgpu.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/amdgpu.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/ampl.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/ampl.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/apdlexer.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/apdlexer.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/apl.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/apl.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/archetype.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/archetype.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/arrow.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/arrow.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/arturo.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/arturo.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/asc.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/asc.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/asm.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/asm.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/asn1.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/asn1.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/automation.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/automation.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/bare.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/bare.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/basic.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/basic.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/bdd.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/bdd.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/berry.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/berry.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/bibtex.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/bibtex.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/blueprint.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/blueprint.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/boa.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/boa.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/bqn.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/bqn.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/business.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/business.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/c_cpp.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/c_cpp.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/c_like.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/c_like.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/capnproto.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/capnproto.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/carbon.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/carbon.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/cddl.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/cddl.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/chapel.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/chapel.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/clean.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/clean.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/comal.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/comal.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/compiled.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/compiled.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/configs.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/configs.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/console.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/console.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/cplint.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/cplint.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/crystal.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/crystal.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/csound.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/csound.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/css.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/css.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/d.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/d.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/dalvik.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/dalvik.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/data.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/data.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/dax.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/dax.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/devicetree.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/devicetree.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/diff.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/diff.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/dns.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/dns.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/dotnet.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/dotnet.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/dsls.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/dsls.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/dylan.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/dylan.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/ecl.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/ecl.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/eiffel.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/eiffel.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/elm.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/elm.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/elpi.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/elpi.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/email.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/email.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/erlang.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/erlang.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/esoteric.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/esoteric.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/ezhil.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/ezhil.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/factor.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/factor.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/fantom.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/fantom.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/felix.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/felix.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/fift.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/fift.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/floscript.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/floscript.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/forth.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/forth.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/fortran.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/fortran.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/foxpro.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/foxpro.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/freefem.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/freefem.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/func.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/func.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/functional.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/functional.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/futhark.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/futhark.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/gcodelexer.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/gcodelexer.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/gdscript.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/gdscript.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/go.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/go.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/grammar_notation.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/grammar_notation.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/graph.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/graph.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/graphics.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/graphics.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/graphql.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/graphql.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/graphviz.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/graphviz.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/gsql.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/gsql.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/haskell.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/haskell.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/haxe.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/haxe.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/hdl.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/hdl.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/hexdump.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/hexdump.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/html.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/html.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/idl.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/idl.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/igor.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/igor.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/inferno.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/inferno.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/installers.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/installers.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/int_fiction.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/int_fiction.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/iolang.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/iolang.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/j.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/j.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/javascript.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/javascript.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/jmespath.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/jmespath.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/jslt.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/jslt.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/jsonnet.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/jsonnet.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/jsx.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/jsx.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/julia.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/julia.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/jvm.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/jvm.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/kuin.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/kuin.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/kusto.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/kusto.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/ldap.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/ldap.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/lean.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/lean.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/lilypond.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/lilypond.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/lisp.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/lisp.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/macaulay2.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/macaulay2.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/make.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/make.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/markup.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/markup.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/math.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/math.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/matlab.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/matlab.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/maxima.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/maxima.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/meson.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/meson.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/mime.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/mime.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/minecraft.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/minecraft.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/mips.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/mips.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/ml.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/ml.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/modeling.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/modeling.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/modula2.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/modula2.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/mojo.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/mojo.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/monte.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/monte.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/mosel.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/mosel.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/ncl.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/ncl.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/nimrod.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/nimrod.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/nit.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/nit.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/nix.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/nix.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/oberon.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/oberon.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/objective.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/objective.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/ooc.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/ooc.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/openscad.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/openscad.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/other.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/other.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/parasail.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/parasail.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/parsers.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/parsers.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/pascal.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/pascal.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/pawn.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/pawn.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/perl.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/perl.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/phix.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/phix.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/php.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/php.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/pointless.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/pointless.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/pony.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/pony.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/praat.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/praat.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/procfile.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/procfile.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/prolog.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/prolog.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/promql.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/promql.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/prql.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/prql.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/ptx.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/ptx.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/python.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/python.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/q.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/q.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/qlik.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/qlik.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/qvt.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/qvt.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/r.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/r.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/rdf.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/rdf.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/rebol.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/rebol.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/resource.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/resource.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/ride.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/ride.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/rita.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/rita.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/rnc.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/rnc.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/roboconf.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/roboconf.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/robotframework.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/robotframework.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/ruby.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/ruby.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/rust.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/rust.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/sas.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/sas.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/savi.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/savi.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/scdoc.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/scdoc.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/scripting.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/scripting.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/sgf.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/sgf.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/shell.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/shell.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/sieve.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/sieve.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/slash.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/slash.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/smalltalk.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/smalltalk.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/smithy.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/smithy.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/smv.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/smv.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/snobol.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/snobol.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/solidity.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/solidity.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/soong.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/soong.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/sophia.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/sophia.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/special.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/special.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/spice.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/spice.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/sql.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/sql.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/srcinfo.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/srcinfo.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/stata.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/stata.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/supercollider.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/supercollider.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/tact.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/tact.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/tal.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/tal.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/tcl.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/tcl.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/teal.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/teal.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/templates.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/templates.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/teraterm.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/teraterm.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/testing.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/testing.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/text.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/text.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/textedit.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/textedit.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/textfmts.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/textfmts.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/theorem.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/theorem.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/thingsdb.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/thingsdb.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/tlb.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/tlb.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/tls.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/tls.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/tnt.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/tnt.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/trafficscript.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/trafficscript.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/typoscript.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/typoscript.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/typst.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/typst.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/ul4.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/ul4.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/unicon.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/unicon.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/urbi.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/urbi.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/usd.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/usd.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/varnish.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/varnish.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/verification.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/verification.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/verifpal.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/verifpal.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/vip.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/vip.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/vyper.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/vyper.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/web.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/web.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/webassembly.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/webassembly.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/webidl.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/webidl.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/webmisc.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/webmisc.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/wgsl.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/wgsl.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/whiley.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/whiley.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/wowtoc.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/wowtoc.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/wren.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/wren.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/x10.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/x10.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/xorg.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/xorg.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/yang.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/yang.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/yara.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/yara.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/lexers/zig.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/lexers/zig.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/modeline.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/modeline.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/plugin.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/plugin.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/regexopt.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/regexopt.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/scanner.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/scanner.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/sphinxext.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/sphinxext.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/style.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/style.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/__init__.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/__init__.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/_mapping.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/_mapping.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/abap.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/abap.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/algol.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/algol.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/algol_nu.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/algol_nu.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/arduino.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/arduino.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/autumn.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/autumn.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/borland.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/borland.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/bw.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/bw.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/coffee.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/coffee.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/colorful.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/colorful.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/default.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/default.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/dracula.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/dracula.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/emacs.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/emacs.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/friendly.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/friendly.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/friendly_grayscale.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/friendly_grayscale.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/fruity.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/fruity.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/gh_dark.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/gh_dark.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/gruvbox.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/gruvbox.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/igor.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/igor.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/inkpot.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/inkpot.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/lightbulb.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/lightbulb.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/lilypond.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/lilypond.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/lovelace.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/lovelace.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/manni.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/manni.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/material.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/material.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/monokai.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/monokai.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/murphy.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/murphy.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/native.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/native.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/nord.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/nord.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/onedark.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/onedark.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/paraiso_dark.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/paraiso_dark.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/paraiso_light.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/paraiso_light.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/pastie.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/pastie.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/perldoc.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/perldoc.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/rainbow_dash.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/rainbow_dash.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/rrt.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/rrt.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/sas.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/sas.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/solarized.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/solarized.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/staroffice.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/staroffice.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/stata_dark.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/stata_dark.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/stata_light.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/stata_light.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/tango.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/tango.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/trac.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/trac.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/vim.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/vim.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/vs.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/vs.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/xcode.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/xcode.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/styles/zenburn.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/styles/zenburn.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/token.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/token.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/unistring.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/unistring.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pygments/util.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pygments/util.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pyradios/base_url.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pyradios/base_url.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pyradios/facets.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pyradios/facets.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pyradios/radios.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pyradios/radios.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/pyradios/utils.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/pyradios/utils.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/__init__.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/__init__.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/__main__.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/__main__.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/_cell_widths.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/_cell_widths.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/_emoji_codes.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/_emoji_codes.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/_emoji_replace.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/_emoji_replace.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/_export_format.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/_export_format.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/_fileno.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/_fileno.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/_inspect.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/_inspect.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/_log_render.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/_log_render.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/_loop.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/_loop.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/_null_file.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/_null_file.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/_palettes.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/_palettes.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/_ratio.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/_ratio.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/_spinners.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/_spinners.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/_win32_console.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/_win32_console.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/_windows.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/_windows.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/_windows_renderer.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/_windows_renderer.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/_wrap.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/_wrap.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/abc.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/abc.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/align.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/align.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/ansi.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/ansi.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/bar.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/bar.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/box.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/box.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/cells.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/cells.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/color.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/color.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/color_triplet.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/color_triplet.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/columns.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/columns.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/console.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/console.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/constrain.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/constrain.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/containers.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/containers.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/control.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/control.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/default_styles.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/default_styles.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/diagnose.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/diagnose.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/emoji.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/emoji.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/errors.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/errors.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/file_proxy.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/file_proxy.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/filesize.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/filesize.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/highlighter.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/highlighter.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/json.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/json.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/jupyter.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/jupyter.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/layout.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/layout.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/live.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/live.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/live_render.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/live_render.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/logging.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/logging.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/markdown.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/markdown.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/markup.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/markup.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/measure.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/measure.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/padding.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/padding.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/pager.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/pager.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/palette.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/palette.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/panel.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/panel.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/pretty.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/pretty.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/progress.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/progress.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/progress_bar.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/progress_bar.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/prompt.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/prompt.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/protocol.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/protocol.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/repr.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/repr.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/rule.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/rule.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/scope.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/scope.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/screen.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/screen.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/segment.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/segment.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/spinner.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/spinner.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/status.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/status.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/style.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/style.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/styled.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/styled.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/syntax.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/syntax.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/table.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/table.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/terminal_theme.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/terminal_theme.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/text.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/text.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/theme.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/theme.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/traceback.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/traceback.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/rich/tree.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/rich/tree.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/__init__.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/__init__.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/_collections.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/_collections.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/_msvccompiler.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/_msvccompiler.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/archive_util.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/archive_util.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/bcppcompiler.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/bcppcompiler.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/ccompiler.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/ccompiler.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/cmd.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/cmd.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/command/_framework_compat.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/command/_framework_compat.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/command/bdist.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/command/bdist.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/command/bdist_dumb.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/command/bdist_dumb.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/command/bdist_rpm.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/command/bdist_rpm.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/command/build.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/command/build.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/command/build_clib.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/command/build_clib.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/command/build_ext.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/command/build_ext.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/command/build_py.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/command/build_py.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/command/build_scripts.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/command/build_scripts.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/command/check.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/command/check.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/command/clean.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/command/clean.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/command/config.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/command/config.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/command/install.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/command/install.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/command/install_data.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/command/install_data.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/command/install_egg_info.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/command/install_egg_info.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/command/install_headers.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/command/install_headers.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/command/install_lib.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/command/install_lib.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/command/install_scripts.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/command/install_scripts.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/command/py37compat.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/command/py37compat.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/command/register.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/command/register.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/command/sdist.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/command/sdist.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/command/upload.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/command/upload.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/config.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/config.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/core.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/core.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/cygwinccompiler.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/cygwinccompiler.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/dep_util.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/dep_util.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/dir_util.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/dir_util.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/dist.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/dist.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/errors.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/errors.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/extension.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/extension.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/fancy_getopt.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/fancy_getopt.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/file_util.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/file_util.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/filelist.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/filelist.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/log.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/log.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/msvc9compiler.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/msvc9compiler.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/msvccompiler.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/msvccompiler.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/py39compat.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/py39compat.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/spawn.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/spawn.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/sysconfig.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/sysconfig.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/text_file.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/text_file.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/unixccompiler.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/unixccompiler.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/util.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/util.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/version.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/version.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_distutils/versionpredicate.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_distutils/versionpredicate.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_entry_points.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_entry_points.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_imp.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_imp.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_importlib.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_importlib.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_itertools.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_itertools.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_normalization.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_normalization.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_path.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_path.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_reqs.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_reqs.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/__init__.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_adapters.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_adapters.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_collections.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_collections.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_compat.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_compat.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_functools.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_functools.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_itertools.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_itertools.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_meta.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_meta.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_py39compat.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_py39compat.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_text.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_metadata/_text.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_adapters.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_adapters.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_common.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_common.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_compat.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_compat.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_itertools.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_itertools.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_legacy.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/_legacy.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/abc.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/abc.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/readers.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/readers.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/simple.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/importlib_resources/simple.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/jaraco/context.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/jaraco/context.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/jaraco/functools.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/jaraco/functools.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/jaraco/text/__init__.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/jaraco/text/__init__.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/more.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/more.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/recipes.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/more_itertools/recipes.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/ordered_set.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/ordered_set.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/_elffile.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/_elffile.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/_manylinux.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/_musllinux.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/_parser.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/_parser.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/_structures.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/_tokenizer.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/_tokenizer.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/markers.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/metadata.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/metadata.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/requirements.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/specifiers.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/tags.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/utils.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/version.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/tomli/_parser.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/tomli/_parser.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/tomli/_re.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/tomli/_re.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/typing_extensions.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/typing_extensions.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/_vendor/zipp.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/_vendor/zipp.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/archive_util.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/archive_util.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/build_meta.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/build_meta.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/command/alias.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/command/alias.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/command/bdist_egg.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/command/bdist_egg.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/command/bdist_rpm.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/command/bdist_rpm.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/command/build.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/command/build.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/command/build_clib.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/command/build_clib.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/command/build_ext.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/command/build_ext.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/command/build_py.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/command/build_py.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/command/develop.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/command/develop.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/command/dist_info.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/command/dist_info.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/command/easy_install.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/command/easy_install.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/command/editable_wheel.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/command/editable_wheel.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/command/egg_info.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/command/egg_info.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/command/install.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/command/install.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/command/install_egg_info.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/command/install_egg_info.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/command/install_lib.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/command/install_lib.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/command/install_scripts.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/command/install_scripts.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/command/rotate.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/command/rotate.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/command/saveopts.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/command/saveopts.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/command/sdist.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/command/sdist.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/command/setopt.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/command/setopt.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/command/test.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/command/test.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/command/upload_docs.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/command/upload_docs.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/config/__init__.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/config/__init__.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/config/_apply_pyprojecttoml.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/config/_apply_pyprojecttoml.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/__init__.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/__init__.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/error_reporting.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/error_reporting.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/extra_validations.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/extra_validations.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_exceptions.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_exceptions.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_validations.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_validations.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/formats.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/config/_validate_pyproject/formats.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/config/expand.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/config/expand.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/config/pyprojecttoml.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/config/pyprojecttoml.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/config/setupcfg.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/config/setupcfg.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/dep_util.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/dep_util.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/depends.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/depends.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/discovery.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/discovery.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/dist.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/dist.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/errors.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/errors.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/extension.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/extension.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/extern/__init__.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/extern/__init__.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/glob.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/glob.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/installer.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/installer.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/launch.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/launch.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/logging.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/logging.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/monkey.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/monkey.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/msvc.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/msvc.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/namespaces.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/namespaces.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/package_index.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/package_index.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/sandbox.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/sandbox.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/unicode_utils.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/unicode_utils.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/warnings.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/warnings.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/wheel.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/wheel.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools/windows_support.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools/windows_support.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/setuptools-68.1.2.dist-info/entry_points.txt` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/setuptools-68.1.2.dist-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/sniffio/_impl.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/sniffio/_impl.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/sniffio/_tests/test_sniffio.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/sniffio/_tests/test_sniffio.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/wheel/_setuptools_logging.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/wheel/_setuptools_logging.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/wheel/bdist_wheel.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/wheel/bdist_wheel.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/wheel/cli/__init__.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/wheel/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/wheel/cli/convert.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/wheel/cli/convert.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/wheel/cli/pack.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/wheel/cli/pack.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/wheel/cli/tags.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/wheel/cli/tags.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/wheel/cli/unpack.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/wheel/cli/unpack.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/wheel/macosx_libfile.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/wheel/macosx_libfile.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/wheel/metadata.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/wheel/metadata.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/wheel/util.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/wheel/util.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/wheel/vendored/packaging/_elffile.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/wheel/vendored/packaging/_elffile.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/wheel/vendored/packaging/_manylinux.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/wheel/vendored/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/wheel/vendored/packaging/_musllinux.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/wheel/vendored/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/wheel/vendored/packaging/_parser.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/wheel/vendored/packaging/_parser.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/wheel/vendored/packaging/_structures.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/wheel/vendored/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/wheel/vendored/packaging/_tokenizer.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/wheel/vendored/packaging/_tokenizer.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/wheel/vendored/packaging/markers.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/wheel/vendored/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/wheel/vendored/packaging/requirements.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/wheel/vendored/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/wheel/vendored/packaging/specifiers.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/wheel/vendored/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/wheel/vendored/packaging/tags.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/wheel/vendored/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/wheel/vendored/packaging/utils.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/wheel/vendored/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/wheel/vendored/packaging/version.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/wheel/vendored/packaging/version.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/wheel/wheelfile.py` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/wheel/wheelfile.py`

 * *Files identical despite different names*

### Comparing `tmuxradio-0.2.33/venv/lib/python3.11/site-packages/wheel-0.41.0.dist-info/LICENSE.txt` & `tmuxradio-0.2.34/venv/lib/python3.11/site-packages/wheel-0.41.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

