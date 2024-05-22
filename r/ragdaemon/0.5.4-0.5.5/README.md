# Comparing `tmp/ragdaemon-0.5.4.tar.gz` & `tmp/ragdaemon-0.5.5.tar.gz`

## Comparing `ragdaemon-0.5.4.tar` & `ragdaemon-0.5.5.tar`

### file list

```diff
@@ -1,78 +1,78 @@
--rw-r--r--   0        0        0     6985 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/scratch.ipynb
--rw-r--r--   0        0        0    10345 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/tutorial.ipynb
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/.github/workflows/run-tests.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/ragdaemon/__init__.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/ragdaemon/__main__.py
--rw-r--r--   0        0        0     3712 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/ragdaemon/app.py
--rw-r--r--   0        0        0    10876 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/ragdaemon/context.py
--rw-r--r--   0        0        0     8200 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/ragdaemon/daemon.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/ragdaemon/errors.py
--rw-r--r--   0        0        0     6974 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/ragdaemon/get_paths.py
--rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/ragdaemon/graph.py
--rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/ragdaemon/locate.py
--rw-r--r--   0        0        0     5976 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/ragdaemon/utils.py
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/ragdaemon/annotators/__init__.py
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/ragdaemon/annotators/base_annotator.py
--rw-r--r--   0        0        0    10676 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/ragdaemon/annotators/call_graph.py
--rw-r--r--   0        0        0     8370 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/ragdaemon/annotators/chunker.py
--rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/ragdaemon/annotators/chunker_line.py
--rw-r--r--   0        0        0    10250 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/ragdaemon/annotators/chunker_llm.py
--rw-r--r--   0        0        0     6226 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/ragdaemon/annotators/diff.py
--rw-r--r--   0        0        0     4789 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/ragdaemon/annotators/hierarchy.py
--rw-r--r--   0        0        0     3812 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/ragdaemon/annotators/layout_hierarchy.py
--rw-r--r--   0        0        0    12309 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/ragdaemon/annotators/summarizer.py
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/ragdaemon/database/__init__.py
--rw-r--r--   0        0        0     4644 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/ragdaemon/database/chroma_database.py
--rw-r--r--   0        0        0     2249 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/ragdaemon/database/database.py
--rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/ragdaemon/database/lite_database.py
--rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/ragdaemon/prompts/call_graph.toml
--rw-r--r--   0        0        0     2482 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/ragdaemon/prompts/chunker_llm.toml
--rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/ragdaemon/prompts/locate.toml
--rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/ragdaemon/prompts/summarizer/base.txt
--rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/ragdaemon/prompts/summarizer/chunk.txt
--rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/ragdaemon/prompts/summarizer/directory.txt
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/ragdaemon/prompts/summarizer/file.txt
--rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/ragdaemon/prompts/summarizer/root.txt
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/ragdaemon/prompts/summarizer/user.txt
--rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/ragdaemon/static/favicon.ico
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/ragdaemon/static/js/controlPanel.js
--rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/ragdaemon/static/js/main.js
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/ragdaemon/static/js/three/camera.js
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/ragdaemon/static/js/three/controls.js
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/ragdaemon/static/js/three/edge.js
--rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/ragdaemon/static/js/three/node.js
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/ragdaemon/static/js/three/raycaster.js
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/ragdaemon/static/js/three/renderer.js
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/ragdaemon/static/js/three/scene.js
--rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/ragdaemon/templates/index.html
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/ragdaemon/templates/search_results.html
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/tests/conftest.py
--rw-r--r--   0        0        0     4422 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/tests/test_comments.py
--rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/tests/test_context.py
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/tests/test_daemon.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/tests/test_database.py
--rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/tests/test_get_paths.py
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/tests/test_sample.py
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/tests/annotators/test_chunker.py
--rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/tests/annotators/test_chunker_llm.py
--rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/tests/annotators/test_diff.py
--rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/tests/annotators/test_hierarchy.py
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/tests/annotators/test_layout_hierarchy.py
--rw-r--r--   0        0        0     5731 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/tests/annotators/test_summarizer.py
--rw-r--r--   0        0        0     8531 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/tests/data/chunker_graph.json
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/tests/data/context_message.txt
--rw-r--r--   0        0        0    10570 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/tests/data/diff_graph.json
--rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/tests/data/hard_to_chunk.txt
--rw-r--r--   0        0        0     2622 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/tests/data/hierarchy_graph.json
--rw-r--r--   0        0        0     3857 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/tests/data/layout_hierarchy_graph.json
--rw-r--r--   0        0        0    17458 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/tests/data/summarizer_graph.json
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/tests/sample/README.md
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/tests/sample/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/tests/sample/src/__init__.py
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/tests/sample/src/interface.py
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/tests/sample/src/operations.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/.gitignore
--rw-r--r--   0        0        0    11340 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/LICENSE
--rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/README.md
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/pyproject.toml
--rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 ragdaemon-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0     6985 2020-02-02 00:00:00.000000 ragdaemon-0.5.5/scratch.ipynb
+-rw-r--r--   0        0        0    10345 2020-02-02 00:00:00.000000 ragdaemon-0.5.5/tutorial.ipynb
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 ragdaemon-0.5.5/.github/workflows/run-tests.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ragdaemon-0.5.5/ragdaemon/__init__.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ragdaemon-0.5.5/ragdaemon/__main__.py
+-rw-r--r--   0        0        0     3712 2020-02-02 00:00:00.000000 ragdaemon-0.5.5/ragdaemon/app.py
+-rw-r--r--   0        0        0    10876 2020-02-02 00:00:00.000000 ragdaemon-0.5.5/ragdaemon/context.py
+-rw-r--r--   0        0        0     8200 2020-02-02 00:00:00.000000 ragdaemon-0.5.5/ragdaemon/daemon.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ragdaemon-0.5.5/ragdaemon/errors.py
+-rw-r--r--   0        0        0     6974 2020-02-02 00:00:00.000000 ragdaemon-0.5.5/ragdaemon/get_paths.py
+-rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 ragdaemon-0.5.5/ragdaemon/graph.py
+-rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 ragdaemon-0.5.5/ragdaemon/locate.py
+-rw-r--r--   0        0        0     5976 2020-02-02 00:00:00.000000 ragdaemon-0.5.5/ragdaemon/utils.py
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 ragdaemon-0.5.5/ragdaemon/annotators/__init__.py
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 ragdaemon-0.5.5/ragdaemon/annotators/base_annotator.py
+-rw-r--r--   0        0        0    10676 2020-02-02 00:00:00.000000 ragdaemon-0.5.5/ragdaemon/annotators/call_graph.py
+-rw-r--r--   0        0        0     8370 2020-02-02 00:00:00.000000 ragdaemon-0.5.5/ragdaemon/annotators/chunker.py
+-rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 ragdaemon-0.5.5/ragdaemon/annotators/chunker_line.py
+-rw-r--r--   0        0        0    10250 2020-02-02 00:00:00.000000 ragdaemon-0.5.5/ragdaemon/annotators/chunker_llm.py
+-rw-r--r--   0        0        0     6226 2020-02-02 00:00:00.000000 ragdaemon-0.5.5/ragdaemon/annotators/diff.py
+-rw-r--r--   0        0        0     4789 2020-02-02 00:00:00.000000 ragdaemon-0.5.5/ragdaemon/annotators/hierarchy.py
+-rw-r--r--   0        0        0     3812 2020-02-02 00:00:00.000000 ragdaemon-0.5.5/ragdaemon/annotators/layout_hierarchy.py
+-rw-r--r--   0        0        0    12309 2020-02-02 00:00:00.000000 ragdaemon-0.5.5/ragdaemon/annotators/summarizer.py
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 ragdaemon-0.5.5/ragdaemon/database/__init__.py
+-rw-r--r--   0        0        0     4644 2020-02-02 00:00:00.000000 ragdaemon-0.5.5/ragdaemon/database/chroma_database.py
+-rw-r--r--   0        0        0     2728 2020-02-02 00:00:00.000000 ragdaemon-0.5.5/ragdaemon/database/database.py
+-rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 ragdaemon-0.5.5/ragdaemon/database/lite_database.py
+-rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 ragdaemon-0.5.5/ragdaemon/prompts/call_graph.toml
+-rw-r--r--   0        0        0     2482 2020-02-02 00:00:00.000000 ragdaemon-0.5.5/ragdaemon/prompts/chunker_llm.toml
+-rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 ragdaemon-0.5.5/ragdaemon/prompts/locate.toml
+-rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 ragdaemon-0.5.5/ragdaemon/prompts/summarizer/base.txt
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 ragdaemon-0.5.5/ragdaemon/prompts/summarizer/chunk.txt
+-rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 ragdaemon-0.5.5/ragdaemon/prompts/summarizer/directory.txt
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 ragdaemon-0.5.5/ragdaemon/prompts/summarizer/file.txt
+-rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 ragdaemon-0.5.5/ragdaemon/prompts/summarizer/root.txt
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 ragdaemon-0.5.5/ragdaemon/prompts/summarizer/user.txt
+-rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 ragdaemon-0.5.5/ragdaemon/static/favicon.ico
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 ragdaemon-0.5.5/ragdaemon/static/js/controlPanel.js
+-rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 ragdaemon-0.5.5/ragdaemon/static/js/main.js
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 ragdaemon-0.5.5/ragdaemon/static/js/three/camera.js
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 ragdaemon-0.5.5/ragdaemon/static/js/three/controls.js
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ragdaemon-0.5.5/ragdaemon/static/js/three/edge.js
+-rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 ragdaemon-0.5.5/ragdaemon/static/js/three/node.js
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 ragdaemon-0.5.5/ragdaemon/static/js/three/raycaster.js
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ragdaemon-0.5.5/ragdaemon/static/js/three/renderer.js
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ragdaemon-0.5.5/ragdaemon/static/js/three/scene.js
+-rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 ragdaemon-0.5.5/ragdaemon/templates/index.html
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 ragdaemon-0.5.5/ragdaemon/templates/search_results.html
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 ragdaemon-0.5.5/tests/conftest.py
+-rw-r--r--   0        0        0     4422 2020-02-02 00:00:00.000000 ragdaemon-0.5.5/tests/test_comments.py
+-rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 ragdaemon-0.5.5/tests/test_context.py
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 ragdaemon-0.5.5/tests/test_daemon.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 ragdaemon-0.5.5/tests/test_database.py
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 ragdaemon-0.5.5/tests/test_get_paths.py
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 ragdaemon-0.5.5/tests/test_sample.py
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 ragdaemon-0.5.5/tests/annotators/test_chunker.py
+-rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 ragdaemon-0.5.5/tests/annotators/test_chunker_llm.py
+-rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 ragdaemon-0.5.5/tests/annotators/test_diff.py
+-rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 ragdaemon-0.5.5/tests/annotators/test_hierarchy.py
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 ragdaemon-0.5.5/tests/annotators/test_layout_hierarchy.py
+-rw-r--r--   0        0        0     5731 2020-02-02 00:00:00.000000 ragdaemon-0.5.5/tests/annotators/test_summarizer.py
+-rw-r--r--   0        0        0     8531 2020-02-02 00:00:00.000000 ragdaemon-0.5.5/tests/data/chunker_graph.json
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 ragdaemon-0.5.5/tests/data/context_message.txt
+-rw-r--r--   0        0        0    10570 2020-02-02 00:00:00.000000 ragdaemon-0.5.5/tests/data/diff_graph.json
+-rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 ragdaemon-0.5.5/tests/data/hard_to_chunk.txt
+-rw-r--r--   0        0        0     2622 2020-02-02 00:00:00.000000 ragdaemon-0.5.5/tests/data/hierarchy_graph.json
+-rw-r--r--   0        0        0     3857 2020-02-02 00:00:00.000000 ragdaemon-0.5.5/tests/data/layout_hierarchy_graph.json
+-rw-r--r--   0        0        0    17458 2020-02-02 00:00:00.000000 ragdaemon-0.5.5/tests/data/summarizer_graph.json
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 ragdaemon-0.5.5/tests/sample/README.md
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 ragdaemon-0.5.5/tests/sample/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ragdaemon-0.5.5/tests/sample/src/__init__.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 ragdaemon-0.5.5/tests/sample/src/interface.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 ragdaemon-0.5.5/tests/sample/src/operations.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 ragdaemon-0.5.5/.gitignore
+-rw-r--r--   0        0        0    11340 2020-02-02 00:00:00.000000 ragdaemon-0.5.5/LICENSE
+-rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 ragdaemon-0.5.5/README.md
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 ragdaemon-0.5.5/pyproject.toml
+-rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 ragdaemon-0.5.5/PKG-INFO
```

### Comparing `ragdaemon-0.5.4/scratch.ipynb` & `ragdaemon-0.5.5/scratch.ipynb`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.4/tutorial.ipynb` & `ragdaemon-0.5.5/tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.4/.github/workflows/run-tests.yml` & `ragdaemon-0.5.5/.github/workflows/run-tests.yml`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.4/ragdaemon/app.py` & `ragdaemon-0.5.5/ragdaemon/app.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.4/ragdaemon/context.py` & `ragdaemon-0.5.5/ragdaemon/context.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.4/ragdaemon/daemon.py` & `ragdaemon-0.5.5/ragdaemon/daemon.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.4/ragdaemon/get_paths.py` & `ragdaemon-0.5.5/ragdaemon/get_paths.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.4/ragdaemon/graph.py` & `ragdaemon-0.5.5/ragdaemon/graph.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.4/ragdaemon/locate.py` & `ragdaemon-0.5.5/ragdaemon/locate.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.4/ragdaemon/utils.py` & `ragdaemon-0.5.5/ragdaemon/utils.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.4/ragdaemon/annotators/__init__.py` & `ragdaemon-0.5.5/ragdaemon/annotators/__init__.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.4/ragdaemon/annotators/base_annotator.py` & `ragdaemon-0.5.5/ragdaemon/annotators/base_annotator.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.4/ragdaemon/annotators/call_graph.py` & `ragdaemon-0.5.5/ragdaemon/annotators/call_graph.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.4/ragdaemon/annotators/chunker.py` & `ragdaemon-0.5.5/ragdaemon/annotators/chunker.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.4/ragdaemon/annotators/chunker_line.py` & `ragdaemon-0.5.5/ragdaemon/annotators/chunker_line.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.4/ragdaemon/annotators/chunker_llm.py` & `ragdaemon-0.5.5/ragdaemon/annotators/chunker_llm.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.4/ragdaemon/annotators/diff.py` & `ragdaemon-0.5.5/ragdaemon/annotators/diff.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.4/ragdaemon/annotators/hierarchy.py` & `ragdaemon-0.5.5/ragdaemon/annotators/hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.4/ragdaemon/annotators/layout_hierarchy.py` & `ragdaemon-0.5.5/ragdaemon/annotators/layout_hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.4/ragdaemon/annotators/summarizer.py` & `ragdaemon-0.5.5/ragdaemon/annotators/summarizer.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.4/ragdaemon/database/__init__.py` & `ragdaemon-0.5.5/ragdaemon/database/__init__.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.4/ragdaemon/database/chroma_database.py` & `ragdaemon-0.5.5/ragdaemon/database/chroma_database.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.4/ragdaemon/database/database.py` & `ragdaemon-0.5.5/ragdaemon/database/database.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,14 +22,26 @@
         self,
         query: str,
         graph: KnowledgeGraph,
         n: Optional[int] = None,
         node_types: Iterable[str] = ("file", "chunk", "diff"),
     ) -> list[dict]:
         """Return documents, metadatas and distances, sorted, for nodes in the graph."""
+        # If query is empty, searching DB will raise "RuntimeError('Cannot return the
+        # results in a contigious 2D array. Probably ef or M is too small')"
+        if not query:
+            results = [
+                {**data, "distance": 1}
+                for _, data in graph.nodes(data=True)
+                if data and "checksum" in data and data["type"] in node_types
+            ]
+            if n:
+                results = results[:n]
+            return results
+
         checksum_index = {
             data["checksum"]: node
             for node, data in graph.nodes(data=True)
             if data and "checksum" in data and data["type"] in node_types
         }
         response = self.query(query, list(checksum_index.keys()))
```

### Comparing `ragdaemon-0.5.4/ragdaemon/database/lite_database.py` & `ragdaemon-0.5.5/ragdaemon/database/lite_database.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.4/ragdaemon/prompts/call_graph.toml` & `ragdaemon-0.5.5/ragdaemon/prompts/call_graph.toml`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.4/ragdaemon/prompts/chunker_llm.toml` & `ragdaemon-0.5.5/ragdaemon/prompts/chunker_llm.toml`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.4/ragdaemon/prompts/locate.toml` & `ragdaemon-0.5.5/ragdaemon/prompts/locate.toml`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.4/ragdaemon/prompts/summarizer/base.txt` & `ragdaemon-0.5.5/ragdaemon/prompts/summarizer/base.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.4/ragdaemon/prompts/summarizer/chunk.txt` & `ragdaemon-0.5.5/ragdaemon/prompts/summarizer/chunk.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.4/ragdaemon/prompts/summarizer/directory.txt` & `ragdaemon-0.5.5/ragdaemon/prompts/summarizer/directory.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.4/ragdaemon/prompts/summarizer/file.txt` & `ragdaemon-0.5.5/ragdaemon/prompts/summarizer/file.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.4/ragdaemon/prompts/summarizer/root.txt` & `ragdaemon-0.5.5/ragdaemon/prompts/summarizer/root.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.4/ragdaemon/static/favicon.ico` & `ragdaemon-0.5.5/ragdaemon/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.4/ragdaemon/static/js/controlPanel.js` & `ragdaemon-0.5.5/ragdaemon/static/js/controlPanel.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.4/ragdaemon/static/js/main.js` & `ragdaemon-0.5.5/ragdaemon/static/js/main.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.4/ragdaemon/static/js/three/edge.js` & `ragdaemon-0.5.5/ragdaemon/static/js/three/edge.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.4/ragdaemon/static/js/three/node.js` & `ragdaemon-0.5.5/ragdaemon/static/js/three/node.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.4/ragdaemon/static/js/three/raycaster.js` & `ragdaemon-0.5.5/ragdaemon/static/js/three/raycaster.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.4/ragdaemon/templates/index.html` & `ragdaemon-0.5.5/ragdaemon/templates/index.html`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.4/tests/conftest.py` & `ragdaemon-0.5.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.4/tests/test_comments.py` & `ragdaemon-0.5.5/tests/test_comments.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.4/tests/test_context.py` & `ragdaemon-0.5.5/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.4/tests/test_daemon.py` & `ragdaemon-0.5.5/tests/test_daemon.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.4/tests/test_get_paths.py` & `ragdaemon-0.5.5/tests/test_get_paths.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.4/tests/test_sample.py` & `ragdaemon-0.5.5/tests/test_sample.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.4/tests/annotators/test_chunker.py` & `ragdaemon-0.5.5/tests/annotators/test_chunker.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.4/tests/annotators/test_chunker_llm.py` & `ragdaemon-0.5.5/tests/annotators/test_chunker_llm.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.4/tests/annotators/test_diff.py` & `ragdaemon-0.5.5/tests/annotators/test_diff.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.4/tests/annotators/test_hierarchy.py` & `ragdaemon-0.5.5/tests/annotators/test_hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.4/tests/annotators/test_layout_hierarchy.py` & `ragdaemon-0.5.5/tests/annotators/test_layout_hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.4/tests/annotators/test_summarizer.py` & `ragdaemon-0.5.5/tests/annotators/test_summarizer.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.4/tests/data/chunker_graph.json` & `ragdaemon-0.5.5/tests/data/chunker_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.4/tests/data/context_message.txt` & `ragdaemon-0.5.5/tests/data/context_message.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.4/tests/data/diff_graph.json` & `ragdaemon-0.5.5/tests/data/diff_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.4/tests/data/hard_to_chunk.txt` & `ragdaemon-0.5.5/tests/data/hard_to_chunk.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.4/tests/data/hierarchy_graph.json` & `ragdaemon-0.5.5/tests/data/hierarchy_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.4/tests/data/layout_hierarchy_graph.json` & `ragdaemon-0.5.5/tests/data/layout_hierarchy_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.4/tests/data/summarizer_graph.json` & `ragdaemon-0.5.5/tests/data/summarizer_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.4/tests/sample/src/interface.py` & `ragdaemon-0.5.5/tests/sample/src/interface.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.4/LICENSE` & `ragdaemon-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.4/README.md` & `ragdaemon-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.5.4/pyproject.toml` & `ragdaemon-0.5.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages=["ragdaemon"]
 
 [project]
 name = "ragdaemon"
-version = "0.5.4"
+version = "0.5.5"
 description = "Generate and render a call graph for a Python project."
 readme = "README.md"
 dependencies = [
     "chromadb==0.4.24",
     "dict2xml==1.7.5",
     "fastapi==0.109.2",
     "Jinja2==3.1.3",
```

### Comparing `ragdaemon-0.5.4/PKG-INFO` & `ragdaemon-0.5.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ragdaemon
-Version: 0.5.4
+Version: 0.5.5
 Summary: Generate and render a call graph for a Python project.
 Project-URL: Homepage, https://github.com/AbanteAI/ragdaemon
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
```

