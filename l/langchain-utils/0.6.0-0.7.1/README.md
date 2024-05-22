# Comparing `tmp/langchain_utils-0.6.0.tar.gz` & `tmp/langchain_utils-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_utils-0.6.0.tar", max compression
+gzip compressed data, was "langchain_utils-0.7.1.tar", max compression
```

## Comparing `langchain_utils-0.6.0.tar` & `langchain_utils-0.7.1.tar`

### file list

```diff
@@ -1,23 +1,24 @@
--rw-r--r--   0        0        0    13854 2024-02-02 17:00:12.841402 langchain_utils-0.6.0/README.md
--rw-r--r--   0        0        0       22 2024-02-02 17:00:23.849092 langchain_utils-0.6.0/langchain_utils/__init__.py
--rw-r--r--   0        0        0     2343 2024-02-02 16:57:51.311557 langchain_utils-0.6.0/langchain_utils/config.py
--rw-r--r--   0        0        0     4805 2023-12-09 18:01:26.353794 langchain_utils-0.6.0/langchain_utils/document_loaders.py
--rwxr-xr-x   0        0        0      697 2023-10-11 18:33:52.181978 langchain_utils-0.6.0/langchain_utils/get_clipboard_prompt.py
--rwxr-xr-x   0        0        0     2991 2023-06-04 03:25:10.362046 langchain_utils-0.6.0/langchain_utils/get_html_prompt.py
--rwxr-xr-x   0        0        0     5155 2023-12-09 18:06:26.800981 langchain_utils-0.6.0/langchain_utils/get_pdf_prompt.py
--rwxr-xr-x   0        0        0     3582 2023-06-04 03:25:10.341545 langchain_utils-0.6.0/langchain_utils/get_text_prompt.py
--rwxr-xr-x   0        0        0     4477 2024-02-02 16:59:51.343702 langchain_utils-0.6.0/langchain_utils/get_url_prompt.py
--rwxr-xr-x   0        0        0     3508 2023-06-04 03:25:10.360593 langchain_utils-0.6.0/langchain_utils/get_word_prompt.py
--rwxr-xr-x   0        0        0     3170 2023-12-19 23:11:51.751594 langchain_utils-0.6.0/langchain_utils/get_youtube_transcript_prompt.py
--rw-r--r--   0        0        0      989 2023-10-11 03:19:45.479046 langchain_utils-0.6.0/langchain_utils/job_search/config.py
--rwxr-xr-x   0        0        0     3146 2023-10-11 03:22:14.646653 langchain_utils-0.6.0/langchain_utils/job_search/lcu_referral_statement.py
--rw-r--r--   0        0        0      487 2023-10-11 03:19:32.550425 langchain_utils-0.6.0/langchain_utils/job_search/prompts.py
--rw-r--r--   0        0        0        0 2023-10-11 02:53:55.645010 langchain_utils-0.6.0/langchain_utils/job_search/utils.py
--rw-r--r--   0        0        0     3571 2023-12-09 18:03:24.059589 langchain_utils-0.6.0/langchain_utils/loaders.py
--rw-r--r--   0        0        0      594 2023-10-23 23:15:37.815190 langchain_utils-0.6.0/langchain_utils/prompts.py
--rw-r--r--   0        0        0    12207 2024-02-02 16:58:33.680196 langchain_utils-0.6.0/langchain_utils/utils.py
--rw-r--r--   0        0        0     2296 2023-06-04 03:25:12.243614 langchain_utils-0.6.0/langchain_utils/utils_argparse.py
--rw-r--r--   0        0        0     3310 2023-05-31 04:08:37.439910 langchain_utils-0.6.0/langchain_utils/utils_doc_loaders.py
--rw-r--r--   0        0        0      578 2023-06-05 03:45:28.871265 langchain_utils-0.6.0/langchain_utils/utils_notify.py
--rw-r--r--   0        0        0     2295 2024-02-02 17:00:23.846236 langchain_utils-0.6.0/pyproject.toml
--rw-r--r--   0        0        0    15114 1970-01-01 00:00:00.000000 langchain_utils-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0    17936 2024-05-22 02:05:09.867645 langchain_utils-0.7.1/README.md
+-rw-r--r--   0        0        0       22 2024-05-22 02:08:43.844531 langchain_utils-0.7.1/langchain_utils/__init__.py
+-rw-r--r--   0        0        0     2414 2024-05-22 02:02:24.897354 langchain_utils-0.7.1/langchain_utils/config.py
+-rw-r--r--   0        0        0     4805 2024-05-22 01:49:05.530433 langchain_utils-0.7.1/langchain_utils/document_loaders.py
+-rwxr-xr-x   0        0        0      697 2023-10-11 18:33:52.181978 langchain_utils-0.7.1/langchain_utils/get_clipboard_prompt.py
+-rwxr-xr-x   0        0        0     2833 2024-05-22 01:59:16.516353 langchain_utils-0.7.1/langchain_utils/get_html_prompt.py
+-rwxr-xr-x   0        0        0     4504 2024-05-22 02:05:05.136301 langchain_utils-0.7.1/langchain_utils/get_pandoc_prompt.py
+-rwxr-xr-x   0        0        0     5177 2024-05-22 01:33:31.002074 langchain_utils-0.7.1/langchain_utils/get_pdf_prompt.py
+-rwxr-xr-x   0        0        0     3446 2024-05-22 01:58:59.721498 langchain_utils-0.7.1/langchain_utils/get_text_prompt.py
+-rwxr-xr-x   0        0        0     4499 2024-05-22 01:33:48.779170 langchain_utils-0.7.1/langchain_utils/get_url_prompt.py
+-rwxr-xr-x   0        0        0     3571 2024-05-22 01:33:54.331130 langchain_utils-0.7.1/langchain_utils/get_word_prompt.py
+-rwxr-xr-x   0        0        0     3192 2024-05-22 01:34:01.980687 langchain_utils-0.7.1/langchain_utils/get_youtube_transcript_prompt.py
+-rw-r--r--   0        0        0      989 2023-10-11 03:19:45.479046 langchain_utils-0.7.1/langchain_utils/job_search/config.py
+-rwxr-xr-x   0        0        0     3146 2023-10-11 03:22:14.646653 langchain_utils-0.7.1/langchain_utils/job_search/lcu_referral_statement.py
+-rw-r--r--   0        0        0      487 2023-10-11 03:19:32.550425 langchain_utils-0.7.1/langchain_utils/job_search/prompts.py
+-rw-r--r--   0        0        0        0 2023-10-11 02:53:55.645010 langchain_utils-0.7.1/langchain_utils/job_search/utils.py
+-rw-r--r--   0        0        0     4043 2024-05-22 01:42:32.490068 langchain_utils-0.7.1/langchain_utils/loaders.py
+-rw-r--r--   0        0        0      594 2023-10-23 23:15:37.815190 langchain_utils-0.7.1/langchain_utils/prompts.py
+-rw-r--r--   0        0        0    12401 2024-05-22 01:33:06.020474 langchain_utils-0.7.1/langchain_utils/utils.py
+-rw-r--r--   0        0        0     2965 2024-05-22 01:57:57.431228 langchain_utils-0.7.1/langchain_utils/utils_argparse.py
+-rw-r--r--   0        0        0     3310 2023-05-31 04:08:37.439910 langchain_utils-0.7.1/langchain_utils/utils_doc_loaders.py
+-rw-r--r--   0        0        0      578 2023-06-05 03:45:28.871265 langchain_utils-0.7.1/langchain_utils/utils_notify.py
+-rw-r--r--   0        0        0     2450 2024-05-22 02:08:43.842802 langchain_utils-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0    19242 1970-01-01 00:00:00.000000 langchain_utils-0.7.1/PKG-INFO
```

### Comparing `langchain_utils-0.6.0/README.md` & `langchain_utils-0.7.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # langchain-utils
 
 LangChain Utilities
 
 - [langchain-utils](#langchain-utils)
   - [Prompt generation using LangChain document loaders](#prompt-generation-using-langchain-document-loaders)
     - [Demos](#demos)
+    - [`pandocprompt`](#pandocprompt)
     - [`urlprompt`](#urlprompt)
     - [`pdfprompt`](#pdfprompt)
     - [`ytprompt`](#ytprompt)
     - [`textprompt`](#textprompt)
     - [`htmlprompt`](#htmlprompt)
   - [Installation](#installation)
     - [pipx](#pipx)
@@ -49,38 +50,103 @@
 
 - Load 3 pages of a pdf file, open each part for inspection before copying, and optionally merge 3 pages into 2 prompts that wouldn't go over the `gpt-3.5-turbo`'s context length limit with langchain's `TokenTextSplitter`.
 
 <!-- for https://user-images.githubusercontent.com/45612704/231731553-63cf3cef-a210-4761-8ca3-dd47bedc3393.mp4 -->
 
 <video src="https://user-images.githubusercontent.com/45612704/231731553-63cf3cef-a210-4761-8ca3-dd47bedc3393.mp4" controls width="100%"></video>
 
+### `pandocprompt`
+
+```
+$ pandocprompt --help
+
+usage: pandocprompt [-h] [-V] [-c] [-e] [-m model] [-S] [-s chunk_size]
+                    [-P PARTS [PARTS ...]] [-r] [-R]
+                    [--print-percentage-non-ascii] [-n] [--out OUT] [-C]
+                    [-w WHAT] [-M] [--from PANDOC_FROM_FORMAT]
+                    [--to PANDOC_TO_FORMAT]
+                    [PATH ...]
+
+Get a prompt from arbitrary files. You need to have `pandoc` installed and in
+$PATH, it will be used to convert source files to desired (hopefully textual)
+format. Common use cases: Getting prompts from EPub books or several TeX
+files.
+
+positional arguments:
+  PATH                  Paths to the text files, or stdin if not provided
+                        (default: None)
+
+options:
+  -h, --help            show this help message and exit
+  -V, --version         show program's version number and exit
+  -c, --copy            Copy the prompt to clipboard (default: False)
+  -e, --edit            Edit the prompt and copy manually (default: False)
+  -m model, --model model
+                        Model to use. This only affects the chunk size. Use -S
+                        to disable splitting (infinite chunk size). (default:
+                        gpt-4-32k)
+  -S, --no-split        Do not split the prompt into multiple parts (use this
+                        if the model has a really large context size)
+                        (default: False)
+  -s chunk_size, --chunk-size chunk_size
+                        Chunk size when splitting transcript, also used to
+                        determine whether to split, defaults to 1/2 of the
+                        context length limit of the model (default: None)
+  -P PARTS [PARTS ...], --parts PARTS [PARTS ...]
+                        Parts to select in the processes list of Documents
+                        (default: None)
+  -r, --raw             Wraps the content in triple quotes with no extra text
+                        (default: False)
+  -R, --raw-no-quotes   Output the content only (default: False)
+  --print-percentage-non-ascii
+                        Print percentage of non-ascii characters (default:
+                        False)
+  -n, --dry-run         Dry run (default: False)
+  --out OUT             Output file (default: None)
+  -C, --from-clipboard  Load text from clipboard (default: False)
+  -w WHAT, --what WHAT  Initial knowledge you want to insert before the PDF
+                        content in the prompt (default: the content of a
+                        document)
+  -M, --merge           Merge contents of all pages before processing
+                        (default: False)
+  --from PANDOC_FROM_FORMAT
+                        The format that is passed to -f in pandoc (default:
+                        None)
+  --to PANDOC_TO_FORMAT
+                        The format that is passed to -t in pandoc. gfm-
+                        raw_html means GitHub Flavored Markdown with raw HTML
+                        stripped. (default: gfm-raw_html)
+
+```
 ### `urlprompt`
 
 ```
 $ urlprompt --help
 
 usage: urlprompt [-h] [-V] [-c] [-e] [-m model] [-S] [-s chunk_size]
                  [-P PARTS [PARTS ...]] [-r] [-R]
-                 [--print-percentage-non-ascii] [-n] [-w WHAT] [-M] [-j] [-g]
-                 [--github-path GITHUB_PATH]
+                 [--print-percentage-non-ascii] [-n] [--out OUT] [-w WHAT]
+                 [-M] [-j] [-g] [--github-path GITHUB_PATH]
                  [--github-revision GITHUB_REVISION] [--substack]
                  URL
 
 Get a prompt consisting the text content of a webpage
 
 positional arguments:
   URL                   URL to the webpage
 
 options:
   -h, --help            show this help message and exit
   -V, --version         show program's version number and exit
   -c, --copy            Copy the prompt to clipboard (default: False)
   -e, --edit            Edit the prompt and copy manually (default: False)
   -m model, --model model
-                        Model to use (default: gpt-3.5-turbo)
+                        Model to use. This only affects the chunk size. Use -S
+                        to disable splitting (infinite chunk size). (default:
+                        gpt-4-32k)
   -S, --no-split        Do not split the prompt into multiple parts (use this
                         if the model has a really large context size)
                         (default: False)
   -s chunk_size, --chunk-size chunk_size
                         Chunk size when splitting transcript, also used to
                         determine whether to split, defaults to 1/2 of the
                         context length limit of the model (default: None)
@@ -90,14 +156,15 @@
   -r, --raw             Wraps the content in triple quotes with no extra text
                         (default: False)
   -R, --raw-no-quotes   Output the content only (default: False)
   --print-percentage-non-ascii
                         Print percentage of non-ascii characters (default:
                         False)
   -n, --dry-run         Dry run (default: False)
+  --out OUT             Output file (default: None)
   -w WHAT, --what WHAT  Initial knowledge you want to insert before the PDF
                         content in the prompt (default: the content of a
                         webpage)
   -M, --merge           Merge contents of all pages before processing
                         (default: False)
   -j, --javascript      Use JavaScript to render the page (default: False)
   -g, --github          Load the raw file from a GitHub URL (default: False)
@@ -112,30 +179,33 @@
 ### `pdfprompt`
 
 ```
 $ pdfprompt --help
 
 usage: pdfprompt [-h] [-V] [-c] [-e] [-m model] [-S] [-s chunk_size]
                  [-P PARTS [PARTS ...]] [-r] [-R]
-                 [--print-percentage-non-ascii] [-n] [-p PAGES [PAGES ...]]
-                 [-l PAGE_SLICE] [-M] [-w WHAT] [-o] [-O] [-L OCR_LANGUAGE]
+                 [--print-percentage-non-ascii] [-n] [--out OUT]
+                 [-p PAGES [PAGES ...]] [-l PAGE_SLICE] [-M] [-w WHAT] [-o]
+                 [-O] [-L OCR_LANGUAGE]
                  PDF Path
 
 Get a prompt consisting the text content of a PDF file
 
 positional arguments:
   PDF Path              Path to the PDF file
 
 options:
   -h, --help            show this help message and exit
   -V, --version         show program's version number and exit
   -c, --copy            Copy the prompt to clipboard (default: False)
   -e, --edit            Edit the prompt and copy manually (default: False)
   -m model, --model model
-                        Model to use (default: gpt-3.5-turbo)
+                        Model to use. This only affects the chunk size. Use -S
+                        to disable splitting (infinite chunk size). (default:
+                        gpt-4-32k)
   -S, --no-split        Do not split the prompt into multiple parts (use this
                         if the model has a really large context size)
                         (default: False)
   -s chunk_size, --chunk-size chunk_size
                         Chunk size when splitting transcript, also used to
                         determine whether to split, defaults to 1/2 of the
                         context length limit of the model (default: None)
@@ -145,14 +215,15 @@
   -r, --raw             Wraps the content in triple quotes with no extra text
                         (default: False)
   -R, --raw-no-quotes   Output the content only (default: False)
   --print-percentage-non-ascii
                         Print percentage of non-ascii characters (default:
                         False)
   -n, --dry-run         Dry run (default: False)
+  --out OUT             Output file (default: None)
   -p PAGES [PAGES ...], --pages PAGES [PAGES ...]
                         Only include specified page numbers (default: None)
   -l PAGE_SLICE, --page-slice PAGE_SLICE
                         Use Python slice syntax to select page numbers (e.g.
                         1:3, 1:10:2, etc.) (default: None)
   -M, --merge           Merge contents of all pages before processing
                         (default: False)
@@ -171,29 +242,31 @@
 ### `ytprompt`
 
 ```
 $ ytprompt --help
 
 usage: ytprompt [-h] [-V] [-c] [-e] [-m model] [-S] [-s chunk_size]
                 [-P PARTS [PARTS ...]] [-r] [-R]
-                [--print-percentage-non-ascii] [-n]
+                [--print-percentage-non-ascii] [-n] [--out OUT]
                 YouTube URL
 
 Get a prompt consisting Title and Transcript of a YouTube Video
 
 positional arguments:
   YouTube URL           YouTube URL
 
 options:
   -h, --help            show this help message and exit
   -V, --version         show program's version number and exit
   -c, --copy            Copy the prompt to clipboard (default: False)
   -e, --edit            Edit the prompt and copy manually (default: False)
   -m model, --model model
-                        Model to use (default: gpt-3.5-turbo)
+                        Model to use. This only affects the chunk size. Use -S
+                        to disable splitting (infinite chunk size). (default:
+                        gpt-4-32k)
   -S, --no-split        Do not split the prompt into multiple parts (use this
                         if the model has a really large context size)
                         (default: False)
   -s chunk_size, --chunk-size chunk_size
                         Chunk size when splitting transcript, also used to
                         determine whether to split, defaults to 1/2 of the
                         context length limit of the model (default: None)
@@ -203,39 +276,43 @@
   -r, --raw             Wraps the content in triple quotes with no extra text
                         (default: False)
   -R, --raw-no-quotes   Output the content only (default: False)
   --print-percentage-non-ascii
                         Print percentage of non-ascii characters (default:
                         False)
   -n, --dry-run         Dry run (default: False)
+  --out OUT             Output file (default: None)
 
 ```
 ### `textprompt`
 
 ```
 $ textprompt --help
 
 usage: textprompt [-h] [-V] [-c] [-e] [-m model] [-S] [-s chunk_size]
                   [-P PARTS [PARTS ...]] [-r] [-R]
-                  [--print-percentage-non-ascii] [-n] [-C] [-w WHAT] [-M]
+                  [--print-percentage-non-ascii] [-n] [--out OUT] [-C]
+                  [-w WHAT] [-M]
                   [PATH ...]
 
 Get a prompt from text files
 
 positional arguments:
   PATH                  Paths to the text files, or stdin if not provided
                         (default: None)
 
 options:
   -h, --help            show this help message and exit
   -V, --version         show program's version number and exit
   -c, --copy            Copy the prompt to clipboard (default: False)
   -e, --edit            Edit the prompt and copy manually (default: False)
   -m model, --model model
-                        Model to use (default: gpt-3.5-turbo)
+                        Model to use. This only affects the chunk size. Use -S
+                        to disable splitting (infinite chunk size). (default:
+                        gpt-4-32k)
   -S, --no-split        Do not split the prompt into multiple parts (use this
                         if the model has a really large context size)
                         (default: False)
   -s chunk_size, --chunk-size chunk_size
                         Chunk size when splitting transcript, also used to
                         determine whether to split, defaults to 1/2 of the
                         context length limit of the model (default: None)
@@ -245,14 +322,15 @@
   -r, --raw             Wraps the content in triple quotes with no extra text
                         (default: False)
   -R, --raw-no-quotes   Output the content only (default: False)
   --print-percentage-non-ascii
                         Print percentage of non-ascii characters (default:
                         False)
   -n, --dry-run         Dry run (default: False)
+  --out OUT             Output file (default: None)
   -C, --from-clipboard  Load text from clipboard (default: False)
   -w WHAT, --what WHAT  Initial knowledge you want to insert before the PDF
                         content in the prompt (default: the content of a
                         document)
   -M, --merge           Merge contents of all pages before processing
                         (default: False)
 
@@ -260,30 +338,33 @@
 ### `htmlprompt`
 
 ```
 $ htmlprompt --help
 
 usage: htmlprompt [-h] [-V] [-c] [-e] [-m model] [-S] [-s chunk_size]
                   [-P PARTS [PARTS ...]] [-r] [-R]
-                  [--print-percentage-non-ascii] [-n] [-C] [-w WHAT] [-M]
+                  [--print-percentage-non-ascii] [-n] [--out OUT] [-C]
+                  [-w WHAT] [-M]
                   [PATH ...]
 
 Get a prompt from html files
 
 positional arguments:
   PATH                  Paths to the html files, or stdin if not provided
                         (default: None)
 
 options:
   -h, --help            show this help message and exit
   -V, --version         show program's version number and exit
   -c, --copy            Copy the prompt to clipboard (default: False)
   -e, --edit            Edit the prompt and copy manually (default: False)
   -m model, --model model
-                        Model to use (default: gpt-3.5-turbo)
+                        Model to use. This only affects the chunk size. Use -S
+                        to disable splitting (infinite chunk size). (default:
+                        gpt-4-32k)
   -S, --no-split        Do not split the prompt into multiple parts (use this
                         if the model has a really large context size)
                         (default: False)
   -s chunk_size, --chunk-size chunk_size
                         Chunk size when splitting transcript, also used to
                         determine whether to split, defaults to 1/2 of the
                         context length limit of the model (default: None)
@@ -293,14 +374,15 @@
   -r, --raw             Wraps the content in triple quotes with no extra text
                         (default: False)
   -R, --raw-no-quotes   Output the content only (default: False)
   --print-percentage-non-ascii
                         Print percentage of non-ascii characters (default:
                         False)
   -n, --dry-run         Dry run (default: False)
+  --out OUT             Output file (default: None)
   -C, --from-clipboard  Load text from clipboard (default: False)
   -w WHAT, --what WHAT  Initial knowledge you want to insert before the PDF
                         content in the prompt (default: the text content of a
                         html file)
   -M, --merge           Merge contents of all pages before processing
                         (default: False)
```

### Comparing `langchain_utils-0.6.0/langchain_utils/config.py` & `langchain_utils-0.7.1/langchain_utils/config.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,21 +11,29 @@
     "gpt-3.5-turbo": 4096,
     "text-davinci-003": 4096,
     "gpt-4": 8192,
     "gpt-4-32k": 32768,
 }
 
 DEFAULT_MODEL = "gpt-3.5-turbo"
+DEFAULT_MODEL = "gpt-4-32k"
 
 
 _REPO_ROOT_DIR = Path(__file__).parent.parent
 TEMPLATE_DIR = _REPO_ROOT_DIR / "templates"
 
 _README_PATH = _REPO_ROOT_DIR / "README.md"
-_README_COMMANDS = ["urlprompt", "pdfprompt", "ytprompt", "textprompt", "htmlprompt"]
+_README_COMMANDS = [
+    "pandocprompt",
+    "urlprompt",
+    "pdfprompt",
+    "ytprompt",
+    "textprompt",
+    "htmlprompt",
+]
 _README_TEMPLATE = TEMPLATE_DIR / "README.jinja.md"
 _COMMAND_USAGE_TEMPLATE = TEMPLATE_DIR / "readme-command-usage.jinja.md"
 
 LOW_QUALITY_PAGE_CONTENT_PUNC_WHITESPACE_PCT_THRESHOLD = 0.15
 
 # TESSERACT_OCR_DEFAULT_LANG = 'chi_sim'
 TESSERACT_OCR_DEFAULT_LANG = "eng"
```

### Comparing `langchain_utils-0.6.0/langchain_utils/document_loaders.py` & `langchain_utils-0.7.1/langchain_utils/document_loaders.py`

 * *Files identical despite different names*

### Comparing `langchain_utils-0.6.0/langchain_utils/get_clipboard_prompt.py` & `langchain_utils-0.7.1/langchain_utils/get_clipboard_prompt.py`

 * *Files identical despite different names*

### Comparing `langchain_utils-0.6.0/langchain_utils/get_html_prompt.py` & `langchain_utils-0.7.1/langchain_utils/get_html_prompt.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,70 +14,68 @@
     html_source_info,
     save_stdin_to_tempfile,
     save_clipboard_to_tempfile,
     get_default_chunk_size,
 )
 from langchain_utils.loaders import load_html
 from langchain_utils.config import DEFAULT_HTML_WHAT
-from langchain_utils.utils_argparse import get_get_prompt_base_arg_parser
+from langchain_utils.utils_argparse import (
+    get_get_prompt_base_arg_parser,
+    postprocess_args,
+)
 
 
 def get_args():
     """Get command-line arguments"""
 
-    parser = get_get_prompt_base_arg_parser(description='Get a prompt from html files')
+    parser = get_get_prompt_base_arg_parser(description="Get a prompt from html files")
 
     parser.add_argument(
-        'path',
-        help='Paths to the html files, or stdin if not provided',
-        metavar='PATH',
+        "path",
+        help="Paths to the html files, or stdin if not provided",
+        metavar="PATH",
         type=str,
         default=None,
-        nargs='*',
+        nargs="*",
     )
 
     parser.add_argument(
-        '-C', '--from-clipboard', help='Load text from clipboard', action='store_true'
+        "-C", "--from-clipboard", help="Load text from clipboard", action="store_true"
     )
 
     parser.add_argument(
-        '-w',
-        '--what',
-        help='Initial knowledge you want to insert before the PDF content in the prompt',
+        "-w",
+        "--what",
+        help="Initial knowledge you want to insert before the PDF content in the prompt",
         type=str,
         default=DEFAULT_HTML_WHAT,
     )
     parser.add_argument(
-        '-M',
-        '--merge',
-        help='Merge contents of all pages before processing',
-        action='store_true',
+        "-M",
+        "--merge",
+        help="Merge contents of all pages before processing",
+        action="store_true",
     )
 
     args = parser.parse_args()
-    if args.from_clipboard:
-        args.path = [save_clipboard_to_tempfile()]
-    elif not args.path:
-        args.path = [save_stdin_to_tempfile()]
-    args.chunk_size = get_default_chunk_size(args.model)
-    return args
+    return postprocess_args(args)
 
 
 def main():
     """Make a jazz noise here"""
 
     args = get_args()
 
-    print(f'Loading html file(s) from {args.path} ...', file=sys.stderr)
+    print(f"Loading html file(s) from {args.path} ...", file=sys.stderr)
     docs = [load_html(p)[0] for p in args.path]
     texts = [doc.page_content for doc in docs]
-    all_text = '\n'.join(texts)
+    all_text = "\n".join(texts)
     word_count = get_word_count((all_text))
     print(
-        f'Loaded {len(docs)} pages. Word count: {word_count} Char count: {len(all_text)}',
+        f"Loaded {len(docs)} pages. Word count: {word_count} Char count: {len(all_text)}",
         file=sys.stderr,
     )
     if args.merge:
         from langchain.docstore.document import Document
 
         merged = Document(
             page_content=all_text,
@@ -102,9 +100,9 @@
         dry_run=args.dry_run,
         raw_triple_quotes=args.raw,
         raw=args.raw_no_quotes,
         parts=args.parts,
     )
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

### Comparing `langchain_utils-0.6.0/langchain_utils/get_pdf_prompt.py` & `langchain_utils-0.7.1/langchain_utils/get_pdf_prompt.py`

 * *Files 2% similar despite different names*

```diff
@@ -155,12 +155,13 @@
         edit=args.edit,
         chunk_size=args.chunk_size,
         extra_chunk_info_fn=pymupdf_doc_page_info,
         dry_run=args.dry_run,
         raw_triple_quotes=args.raw,
         raw=args.raw_no_quotes,
         parts=args.parts,
+        out=args.out,
     )
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `langchain_utils-0.6.0/langchain_utils/get_text_prompt.py` & `langchain_utils-0.7.1/langchain_utils/get_text_prompt.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,82 +16,80 @@
     save_clipboard_to_tempfile,
     get_token_count,
     get_percentage_non_ascii,
     get_default_chunk_size,
 )
 from langchain_utils.loaders import load_text
 from langchain_utils.config import DEFAULT_GENERAL_WHAT
-from langchain_utils.utils_argparse import get_get_prompt_base_arg_parser
+from langchain_utils.utils_argparse import (
+    get_get_prompt_base_arg_parser,
+    postprocess_args,
+)
 
 
 def get_args():
     """Get command-line arguments"""
 
-    parser = get_get_prompt_base_arg_parser(description='Get a prompt from text files')
+    parser = get_get_prompt_base_arg_parser(description="Get a prompt from text files")
 
     parser.add_argument(
-        'path',
-        help='Paths to the text files, or stdin if not provided',
-        metavar='PATH',
+        "path",
+        help="Paths to the text files, or stdin if not provided",
+        metavar="PATH",
         type=str,
         default=None,
-        nargs='*',
+        nargs="*",
     )
 
     parser.add_argument(
-        '-C', '--from-clipboard', help='Load text from clipboard', action='store_true'
+        "-C", "--from-clipboard", help="Load text from clipboard", action="store_true"
     )
 
     parser.add_argument(
-        '-w',
-        '--what',
-        help='Initial knowledge you want to insert before the PDF content in the prompt',
+        "-w",
+        "--what",
+        help="Initial knowledge you want to insert before the PDF content in the prompt",
         type=str,
         default=DEFAULT_GENERAL_WHAT,
     )
     parser.add_argument(
-        '-M',
-        '--merge',
-        help='Merge contents of all pages before processing',
-        action='store_true',
+        "-M",
+        "--merge",
+        help="Merge contents of all pages before processing",
+        action="store_true",
     )
 
     args = parser.parse_args()
-    if args.from_clipboard:
-        args.path = [save_clipboard_to_tempfile()]
-    elif not args.path:
-        args.path = [save_stdin_to_tempfile()]
-    args.chunk_size = get_default_chunk_size(args.model)
-    return args
+    return postprocess_args(args)
 
 
 def main():
     """Make a jazz noise here"""
 
     args = get_args()
 
-    print(f'Loading text file(s) from {args.path} ...', file=sys.stderr)
+    print(f"Loading text file(s) from {args.path} ...", file=sys.stderr)
     docs = [load_text(p)[0] for p in args.path]
     texts = [doc.page_content for doc in docs]
-    all_text = '\n'.join(texts)
+    all_text = "\n".join(texts)
     word_count = get_word_count((all_text))
     char_count = len(all_text)
     print(
-        f'Loaded {len(docs)} pages. Word count: {word_count} Char count: {len(all_text)}',
+        f"Loaded {len(docs)} pages. Word count: {word_count} Char count: {len(all_text)}",
         file=sys.stderr,
     )
     if args.print_percentage_non_ascii:
         print(
-            f'Percentage of non-ascii characters: {get_percentage_non_ascii(all_text) * 100:.2f}%',
+            f"Percentage of non-ascii characters: {get_percentage_non_ascii(all_text) * 100:.2f}%",
             file=sys.stderr,
         )
         token_count = get_token_count(all_text)
-        print(f'Token count: {token_count}', file=sys.stderr)
-        print(f'Token / Word: {token_count / word_count:.2f}', file=sys.stderr)
-        print(f'Token / Char: {token_count / char_count:.2f}', file=sys.stderr)
+        print(f"Token count: {token_count}", file=sys.stderr)
+        print(f"Token / Word: {token_count / word_count:.2f}", file=sys.stderr)
+        print(f"Token / Char: {token_count / char_count:.2f}", file=sys.stderr)
         return
     if args.merge:
         from langchain.docstore.document import Document
 
         merged = Document(
             page_content=all_text,
         )
@@ -112,12 +110,13 @@
         should_be_only_one_doc=True if num_docs == 1 else False,
         chunk_size=args.chunk_size,
         extra_chunk_info_fn=general_document_source_info,
         dry_run=args.dry_run,
         raw_triple_quotes=args.raw,
         raw=args.raw_no_quotes,
         parts=args.parts,
+        out=args.out,
     )
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

### Comparing `langchain_utils-0.6.0/langchain_utils/get_url_prompt.py` & `langchain_utils-0.7.1/langchain_utils/get_url_prompt.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,12 +138,13 @@
         should_be_only_one_doc=True,
         chunk_size=args.chunk_size,
         extra_chunk_info_fn=general_document_source_info,
         dry_run=args.dry_run,
         raw_triple_quotes=args.raw,
         raw=args.raw_no_quotes,
         parts=args.parts,
+        out=args.out,
     )
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `langchain_utils-0.6.0/langchain_utils/get_word_prompt.py` & `langchain_utils-0.7.1/langchain_utils/get_word_prompt.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,76 +20,81 @@
 from langchain_utils.config import DEFAULT_GENERAL_WHAT
 from langchain_utils.utils_argparse import get_get_prompt_base_arg_parser
 
 
 def get_args():
     """Get command-line arguments"""
 
-    parser = get_get_prompt_base_arg_parser(description='Get a prompt from text files')
+    parser = get_get_prompt_base_arg_parser(description="Get a prompt from text files")
 
     parser.add_argument(
-        'word_path',
-        help='Path to the Word document',
-        metavar='Word Document Path',
+        "word_path",
+        help="Path to the Word document",
+        metavar="Word Document Path",
         type=str,
     )
     parser.add_argument(
-        '-u', '--unstructured-loading-mode', type=str, choices=UnstructuredLoadingMode.__args__, default='single', help='Unstructured loading mode'  # type: ignore
+        "-u",
+        "--unstructured-loading-mode",
+        type=str,
+        choices=UnstructuredLoadingMode.__args__,
+        default="single",
+        help="Unstructured loading mode",  # type: ignore
     )
 
     parser.add_argument(
-        '-w',
-        '--what',
-        help='Initial knowledge you want to insert before the PDF content in the prompt',
+        "-w",
+        "--what",
+        help="Initial knowledge you want to insert before the PDF content in the prompt",
         type=str,
         default=DEFAULT_GENERAL_WHAT,
     )
     parser.add_argument(
-        '-M',
-        '--merge',
-        help='Merge contents of all pages before processing',
-        action='store_true',
+        "-M",
+        "--merge",
+        help="Merge contents of all pages before processing",
+        action="store_true",
     )
 
     args = parser.parse_args()
     args.chunk_size = get_default_chunk_size(args.model)
     return args
 
 
 def main():
     """Make a jazz noise here"""
 
     args = get_args()
 
-    print(f'Loading Word document from {args.word_path} ...', file=sys.stderr)
+    print(f"Loading Word document from {args.word_path} ...", file=sys.stderr)
     docs = load_word(args.word_path)
     texts = [doc.page_content for doc in docs]
-    all_text = '\n'.join(texts)
+    all_text = "\n".join(texts)
     word_count = get_word_count((all_text))
     char_count = len(all_text)
     print(
-        f'Loaded {len(docs)} Documents. Word count: {word_count} Char count: {char_count}',
+        f"Loaded {len(docs)} Documents. Word count: {word_count} Char count: {char_count}",
         file=sys.stderr,
     )
     if args.print_percentage_non_ascii:
         print(
-            f'Percentage of non-ascii characters: {get_percentage_non_ascii(all_text) * 100:.2f}%',
+            f"Percentage of non-ascii characters: {get_percentage_non_ascii(all_text) * 100:.2f}%",
             file=sys.stderr,
         )
         token_count = get_token_count(all_text)
-        print(f'Token count: {token_count}', file=sys.stderr)
-        print(f'Token / Word: {token_count / word_count:.2f}', file=sys.stderr)
-        print(f'Token / Char: {token_count / char_count:.2f}', file=sys.stderr)
+        print(f"Token count: {token_count}", file=sys.stderr)
+        print(f"Token / Word: {token_count / word_count:.2f}", file=sys.stderr)
+        print(f"Token / Char: {token_count / char_count:.2f}", file=sys.stderr)
         return
     if args.merge:
         from langchain.docstore.document import Document
 
         merged = Document(
             page_content=all_text,
-            metadata={k: v for k, v in docs[0].metadata.items() if k in {'source'}},
+            metadata={k: v for k, v in docs[0].metadata.items() if k in {"source"}},
         )
     documents = [merged] if args.merge else docs  # type: ignore
     num_docs = len(documents)
     if args.no_split:
         needs_splitting = False
     elif word_count > args.chunk_size * 0.75:
         needs_splitting = True
@@ -104,12 +109,13 @@
         should_be_only_one_doc=True if num_docs == 1 else False,
         chunk_size=args.chunk_size,
         extra_chunk_info_fn=general_document_source_info,
         dry_run=args.dry_run,
         raw_triple_quotes=args.raw,
         raw=args.raw_no_quotes,
         parts=args.parts,
+        out=args.out,
     )
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

### Comparing `langchain_utils-0.6.0/langchain_utils/get_youtube_transcript_prompt.py` & `langchain_utils-0.7.1/langchain_utils/get_youtube_transcript_prompt.py`

 * *Files 4% similar despite different names*

```diff
@@ -90,12 +90,13 @@
         copy=args.copy,
         edit=args.edit,
         chunk_size=args.chunk_size,
         dry_run=args.dry_run,
         raw_triple_quotes=args.raw,
         raw=args.raw_no_quotes,
         parts=args.parts,
+        out=args.out,
     )
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `langchain_utils-0.6.0/langchain_utils/job_search/config.py` & `langchain_utils-0.7.1/langchain_utils/job_search/config.py`

 * *Files identical despite different names*

### Comparing `langchain_utils-0.6.0/langchain_utils/job_search/lcu_referral_statement.py` & `langchain_utils-0.7.1/langchain_utils/job_search/lcu_referral_statement.py`

 * *Files identical despite different names*

### Comparing `langchain_utils-0.6.0/langchain_utils/loaders.py` & `langchain_utils-0.7.1/langchain_utils/loaders.py`

 * *Files 13% similar despite different names*

```diff
@@ -107,7 +107,23 @@
         raise ValueError(f"Invalid GitHub URL: {github_url}")
     github_info |= {"revision": github_revision, "file_path": github_path}
     url = get_github_file_raw_url(**github_info)
     text = TextRequestsWrapper().get(url)
 
     docs = [Document(page_content=text, metadata={"url": url})]
     return docs
+
+
+def load_pandoc(
+    input_file: str, output_format: str = "gfm", input_format: str | None = None
+) -> list["Document"]:
+    import subprocess
+    from langchain.docstore.document import Document
+
+    command = ["pandoc", input_file, "-t", output_format]
+    if input_format:
+        command.extend(["-f", input_format])
+
+    result = subprocess.run(command, capture_output=True, text=True, check=True)
+
+    docs = [Document(page_content=result.stdout)]
+    return docs
```

### Comparing `langchain_utils-0.6.0/langchain_utils/prompts.py` & `langchain_utils-0.7.1/langchain_utils/prompts.py`

 * *Files identical despite different names*

### Comparing `langchain_utils-0.6.0/langchain_utils/utils.py` & `langchain_utils-0.7.1/langchain_utils/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,14 +133,15 @@
     edit: bool = False,
     chunk_size: int = 2000,
     extra_chunk_info_fn: Callable[["Document"], str] = lambda doc: "",
     dry_run: bool = False,
     parts: list[int] | None = None,
     raw_triple_quotes: bool = False,
     raw: bool = False,
+    out: str | None = None,
 ):
     from langchain.prompts import PromptTemplate
 
     def deliver_single_doc(document: "Document"):
         if raw:
             template = RAW_TEMPLATE
         elif raw_triple_quotes:
@@ -174,14 +175,18 @@
                 file=sys.stderr,
             )
             if not dry_run:
                 import pyperclip
 
                 pyperclip.copy(formatted_prompt)
                 print("Prompt copied to clipboard.", file=sys.stderr)
+        elif out:
+            with open(out, "w") as f:
+                f.write(formatted_prompt)
+                print(f"Prompt written to {out}.", file=sys.stderr)
         else:
             print(formatted_prompt)
 
     def deliver_multiple_docs(documents: list["Document"]):
         if len(documents) == 1:
             deliver_single_doc(documents[0])
             return
```

### Comparing `langchain_utils-0.6.0/langchain_utils/utils_doc_loaders.py` & `langchain_utils-0.7.1/langchain_utils/utils_doc_loaders.py`

 * *Files identical despite different names*

### Comparing `langchain_utils-0.6.0/langchain_utils/utils_notify.py` & `langchain_utils-0.7.1/langchain_utils/utils_notify.py`

 * *Files identical despite different names*

### Comparing `langchain_utils-0.6.0/pyproject.toml` & `langchain_utils-0.7.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langchain-utils"
-version = "0.6.0"
+version = "0.7.1"
 description = "Utilities built upon the langchain library"
 authors = ["Teddy Xinyuan Chen <45612704+tddschn@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{ include = "langchain_utils" }]
 license = "MIT"
 homepage = "https://github.com/tddschn/langchain-utils"
 repository = "https://github.com/tddschn/langchain-utils"
@@ -22,35 +22,38 @@
 clipboardprompt = "langchain_utils.get_clipboard_prompt:main"
 get-word-prompt = "langchain_utils.get_word_prompt:main"
 wordprompt = "langchain_utils.get_word_prompt:main"
 get-html-prompt = "langchain_utils.get_html_prompt:main"
 htmlprompt = "langchain_utils.get_html_prompt:main"
 get-pdf-prompt = "langchain_utils.get_pdf_prompt:main"
 pdfprompt = "langchain_utils.get_pdf_prompt:main"
+get-pandoc-prompt = "langchain_utils.get_pandoc_prompt:main"
+pandocprompt = "langchain_utils.get_pandoc_prompt:main"
 referral-statement-prompt = "langchain_utils.job_search.lcu_referral_statement:main"
 refstmtprompt = "langchain_utils.job_search.lcu_referral_statement:main"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/tddschn/langchain-utils/issues"
 
 [tool.poetry.dependencies]
-python = "^3.11"
+python = ">=3.11, <4.0"
 langchain = "^0.0.351"
 youtube-transcript-api = "^0.5.0"
 pytube = "^15.0.0"
 pyperclip = "^1.8.2"
 tiktoken = "^0.3.3"
 pymupdf = "^1.21.1"
 # must use this version of unstructured, or it won't be able to parse certain htmls
 unstructured = "0.5.2"
 selenium = "^4.8.3"
 bs4 = "^0.0.1"
 tqdm = "^4.65.0"
 pync = { version = "^2.0.3", extras = ["notify"] }
 markdownify = "^0.11.6"
+typing-extensions = "3.10.0.2"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 better-exceptions = "^0.3.3"
 ipython = "^8.12.0"
 ipykernel = "^6.22.0"
```

### Comparing `langchain_utils-0.6.0/PKG-INFO` & `langchain_utils-0.7.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-utils
-Version: 0.6.0
+Version: 0.7.1
 Summary: Utilities built upon the langchain library
 Home-page: https://github.com/tddschn/langchain-utils
 License: MIT
 Keywords: langchain,utils,LLM,prompts,CLI
 Author: Teddy Xinyuan Chen
 Author-email: 45612704+tddschn@users.noreply.github.com
 Requires-Python: >=3.11,<4.0
@@ -19,27 +19,29 @@
 Requires-Dist: pymupdf (>=1.21.1,<2.0.0)
 Requires-Dist: pync[notify] (>=2.0.3,<3.0.0)
 Requires-Dist: pyperclip (>=1.8.2,<2.0.0)
 Requires-Dist: pytube (>=15.0.0,<16.0.0)
 Requires-Dist: selenium (>=4.8.3,<5.0.0)
 Requires-Dist: tiktoken (>=0.3.3,<0.4.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
+Requires-Dist: typing-extensions (==3.10.0.2)
 Requires-Dist: unstructured (==0.5.2)
 Requires-Dist: youtube-transcript-api (>=0.5.0,<0.6.0)
 Project-URL: Bug Tracker, https://github.com/tddschn/langchain-utils/issues
 Project-URL: Repository, https://github.com/tddschn/langchain-utils
 Description-Content-Type: text/markdown
 
 # langchain-utils
 
 LangChain Utilities
 
 - [langchain-utils](#langchain-utils)
   - [Prompt generation using LangChain document loaders](#prompt-generation-using-langchain-document-loaders)
     - [Demos](#demos)
+    - [`pandocprompt`](#pandocprompt)
     - [`urlprompt`](#urlprompt)
     - [`pdfprompt`](#pdfprompt)
     - [`ytprompt`](#ytprompt)
     - [`textprompt`](#textprompt)
     - [`htmlprompt`](#htmlprompt)
   - [Installation](#installation)
     - [pipx](#pipx)
@@ -80,38 +82,103 @@
 
 - Load 3 pages of a pdf file, open each part for inspection before copying, and optionally merge 3 pages into 2 prompts that wouldn't go over the `gpt-3.5-turbo`'s context length limit with langchain's `TokenTextSplitter`.
 
 <!-- for https://user-images.githubusercontent.com/45612704/231731553-63cf3cef-a210-4761-8ca3-dd47bedc3393.mp4 -->
 
 <video src="https://user-images.githubusercontent.com/45612704/231731553-63cf3cef-a210-4761-8ca3-dd47bedc3393.mp4" controls width="100%"></video>
 
+### `pandocprompt`
+
+```
+$ pandocprompt --help
+
+usage: pandocprompt [-h] [-V] [-c] [-e] [-m model] [-S] [-s chunk_size]
+                    [-P PARTS [PARTS ...]] [-r] [-R]
+                    [--print-percentage-non-ascii] [-n] [--out OUT] [-C]
+                    [-w WHAT] [-M] [--from PANDOC_FROM_FORMAT]
+                    [--to PANDOC_TO_FORMAT]
+                    [PATH ...]
+
+Get a prompt from arbitrary files. You need to have `pandoc` installed and in
+$PATH, it will be used to convert source files to desired (hopefully textual)
+format. Common use cases: Getting prompts from EPub books or several TeX
+files.
+
+positional arguments:
+  PATH                  Paths to the text files, or stdin if not provided
+                        (default: None)
+
+options:
+  -h, --help            show this help message and exit
+  -V, --version         show program's version number and exit
+  -c, --copy            Copy the prompt to clipboard (default: False)
+  -e, --edit            Edit the prompt and copy manually (default: False)
+  -m model, --model model
+                        Model to use. This only affects the chunk size. Use -S
+                        to disable splitting (infinite chunk size). (default:
+                        gpt-4-32k)
+  -S, --no-split        Do not split the prompt into multiple parts (use this
+                        if the model has a really large context size)
+                        (default: False)
+  -s chunk_size, --chunk-size chunk_size
+                        Chunk size when splitting transcript, also used to
+                        determine whether to split, defaults to 1/2 of the
+                        context length limit of the model (default: None)
+  -P PARTS [PARTS ...], --parts PARTS [PARTS ...]
+                        Parts to select in the processes list of Documents
+                        (default: None)
+  -r, --raw             Wraps the content in triple quotes with no extra text
+                        (default: False)
+  -R, --raw-no-quotes   Output the content only (default: False)
+  --print-percentage-non-ascii
+                        Print percentage of non-ascii characters (default:
+                        False)
+  -n, --dry-run         Dry run (default: False)
+  --out OUT             Output file (default: None)
+  -C, --from-clipboard  Load text from clipboard (default: False)
+  -w WHAT, --what WHAT  Initial knowledge you want to insert before the PDF
+                        content in the prompt (default: the content of a
+                        document)
+  -M, --merge           Merge contents of all pages before processing
+                        (default: False)
+  --from PANDOC_FROM_FORMAT
+                        The format that is passed to -f in pandoc (default:
+                        None)
+  --to PANDOC_TO_FORMAT
+                        The format that is passed to -t in pandoc. gfm-
+                        raw_html means GitHub Flavored Markdown with raw HTML
+                        stripped. (default: gfm-raw_html)
+
+```
 ### `urlprompt`
 
 ```
 $ urlprompt --help
 
 usage: urlprompt [-h] [-V] [-c] [-e] [-m model] [-S] [-s chunk_size]
                  [-P PARTS [PARTS ...]] [-r] [-R]
-                 [--print-percentage-non-ascii] [-n] [-w WHAT] [-M] [-j] [-g]
-                 [--github-path GITHUB_PATH]
+                 [--print-percentage-non-ascii] [-n] [--out OUT] [-w WHAT]
+                 [-M] [-j] [-g] [--github-path GITHUB_PATH]
                  [--github-revision GITHUB_REVISION] [--substack]
                  URL
 
 Get a prompt consisting the text content of a webpage
 
 positional arguments:
   URL                   URL to the webpage
 
 options:
   -h, --help            show this help message and exit
   -V, --version         show program's version number and exit
   -c, --copy            Copy the prompt to clipboard (default: False)
   -e, --edit            Edit the prompt and copy manually (default: False)
   -m model, --model model
-                        Model to use (default: gpt-3.5-turbo)
+                        Model to use. This only affects the chunk size. Use -S
+                        to disable splitting (infinite chunk size). (default:
+                        gpt-4-32k)
   -S, --no-split        Do not split the prompt into multiple parts (use this
                         if the model has a really large context size)
                         (default: False)
   -s chunk_size, --chunk-size chunk_size
                         Chunk size when splitting transcript, also used to
                         determine whether to split, defaults to 1/2 of the
                         context length limit of the model (default: None)
@@ -121,14 +188,15 @@
   -r, --raw             Wraps the content in triple quotes with no extra text
                         (default: False)
   -R, --raw-no-quotes   Output the content only (default: False)
   --print-percentage-non-ascii
                         Print percentage of non-ascii characters (default:
                         False)
   -n, --dry-run         Dry run (default: False)
+  --out OUT             Output file (default: None)
   -w WHAT, --what WHAT  Initial knowledge you want to insert before the PDF
                         content in the prompt (default: the content of a
                         webpage)
   -M, --merge           Merge contents of all pages before processing
                         (default: False)
   -j, --javascript      Use JavaScript to render the page (default: False)
   -g, --github          Load the raw file from a GitHub URL (default: False)
@@ -143,30 +211,33 @@
 ### `pdfprompt`
 
 ```
 $ pdfprompt --help
 
 usage: pdfprompt [-h] [-V] [-c] [-e] [-m model] [-S] [-s chunk_size]
                  [-P PARTS [PARTS ...]] [-r] [-R]
-                 [--print-percentage-non-ascii] [-n] [-p PAGES [PAGES ...]]
-                 [-l PAGE_SLICE] [-M] [-w WHAT] [-o] [-O] [-L OCR_LANGUAGE]
+                 [--print-percentage-non-ascii] [-n] [--out OUT]
+                 [-p PAGES [PAGES ...]] [-l PAGE_SLICE] [-M] [-w WHAT] [-o]
+                 [-O] [-L OCR_LANGUAGE]
                  PDF Path
 
 Get a prompt consisting the text content of a PDF file
 
 positional arguments:
   PDF Path              Path to the PDF file
 
 options:
   -h, --help            show this help message and exit
   -V, --version         show program's version number and exit
   -c, --copy            Copy the prompt to clipboard (default: False)
   -e, --edit            Edit the prompt and copy manually (default: False)
   -m model, --model model
-                        Model to use (default: gpt-3.5-turbo)
+                        Model to use. This only affects the chunk size. Use -S
+                        to disable splitting (infinite chunk size). (default:
+                        gpt-4-32k)
   -S, --no-split        Do not split the prompt into multiple parts (use this
                         if the model has a really large context size)
                         (default: False)
   -s chunk_size, --chunk-size chunk_size
                         Chunk size when splitting transcript, also used to
                         determine whether to split, defaults to 1/2 of the
                         context length limit of the model (default: None)
@@ -176,14 +247,15 @@
   -r, --raw             Wraps the content in triple quotes with no extra text
                         (default: False)
   -R, --raw-no-quotes   Output the content only (default: False)
   --print-percentage-non-ascii
                         Print percentage of non-ascii characters (default:
                         False)
   -n, --dry-run         Dry run (default: False)
+  --out OUT             Output file (default: None)
   -p PAGES [PAGES ...], --pages PAGES [PAGES ...]
                         Only include specified page numbers (default: None)
   -l PAGE_SLICE, --page-slice PAGE_SLICE
                         Use Python slice syntax to select page numbers (e.g.
                         1:3, 1:10:2, etc.) (default: None)
   -M, --merge           Merge contents of all pages before processing
                         (default: False)
@@ -202,29 +274,31 @@
 ### `ytprompt`
 
 ```
 $ ytprompt --help
 
 usage: ytprompt [-h] [-V] [-c] [-e] [-m model] [-S] [-s chunk_size]
                 [-P PARTS [PARTS ...]] [-r] [-R]
-                [--print-percentage-non-ascii] [-n]
+                [--print-percentage-non-ascii] [-n] [--out OUT]
                 YouTube URL
 
 Get a prompt consisting Title and Transcript of a YouTube Video
 
 positional arguments:
   YouTube URL           YouTube URL
 
 options:
   -h, --help            show this help message and exit
   -V, --version         show program's version number and exit
   -c, --copy            Copy the prompt to clipboard (default: False)
   -e, --edit            Edit the prompt and copy manually (default: False)
   -m model, --model model
-                        Model to use (default: gpt-3.5-turbo)
+                        Model to use. This only affects the chunk size. Use -S
+                        to disable splitting (infinite chunk size). (default:
+                        gpt-4-32k)
   -S, --no-split        Do not split the prompt into multiple parts (use this
                         if the model has a really large context size)
                         (default: False)
   -s chunk_size, --chunk-size chunk_size
                         Chunk size when splitting transcript, also used to
                         determine whether to split, defaults to 1/2 of the
                         context length limit of the model (default: None)
@@ -234,39 +308,43 @@
   -r, --raw             Wraps the content in triple quotes with no extra text
                         (default: False)
   -R, --raw-no-quotes   Output the content only (default: False)
   --print-percentage-non-ascii
                         Print percentage of non-ascii characters (default:
                         False)
   -n, --dry-run         Dry run (default: False)
+  --out OUT             Output file (default: None)
 
 ```
 ### `textprompt`
 
 ```
 $ textprompt --help
 
 usage: textprompt [-h] [-V] [-c] [-e] [-m model] [-S] [-s chunk_size]
                   [-P PARTS [PARTS ...]] [-r] [-R]
-                  [--print-percentage-non-ascii] [-n] [-C] [-w WHAT] [-M]
+                  [--print-percentage-non-ascii] [-n] [--out OUT] [-C]
+                  [-w WHAT] [-M]
                   [PATH ...]
 
 Get a prompt from text files
 
 positional arguments:
   PATH                  Paths to the text files, or stdin if not provided
                         (default: None)
 
 options:
   -h, --help            show this help message and exit
   -V, --version         show program's version number and exit
   -c, --copy            Copy the prompt to clipboard (default: False)
   -e, --edit            Edit the prompt and copy manually (default: False)
   -m model, --model model
-                        Model to use (default: gpt-3.5-turbo)
+                        Model to use. This only affects the chunk size. Use -S
+                        to disable splitting (infinite chunk size). (default:
+                        gpt-4-32k)
   -S, --no-split        Do not split the prompt into multiple parts (use this
                         if the model has a really large context size)
                         (default: False)
   -s chunk_size, --chunk-size chunk_size
                         Chunk size when splitting transcript, also used to
                         determine whether to split, defaults to 1/2 of the
                         context length limit of the model (default: None)
@@ -276,14 +354,15 @@
   -r, --raw             Wraps the content in triple quotes with no extra text
                         (default: False)
   -R, --raw-no-quotes   Output the content only (default: False)
   --print-percentage-non-ascii
                         Print percentage of non-ascii characters (default:
                         False)
   -n, --dry-run         Dry run (default: False)
+  --out OUT             Output file (default: None)
   -C, --from-clipboard  Load text from clipboard (default: False)
   -w WHAT, --what WHAT  Initial knowledge you want to insert before the PDF
                         content in the prompt (default: the content of a
                         document)
   -M, --merge           Merge contents of all pages before processing
                         (default: False)
 
@@ -291,30 +370,33 @@
 ### `htmlprompt`
 
 ```
 $ htmlprompt --help
 
 usage: htmlprompt [-h] [-V] [-c] [-e] [-m model] [-S] [-s chunk_size]
                   [-P PARTS [PARTS ...]] [-r] [-R]
-                  [--print-percentage-non-ascii] [-n] [-C] [-w WHAT] [-M]
+                  [--print-percentage-non-ascii] [-n] [--out OUT] [-C]
+                  [-w WHAT] [-M]
                   [PATH ...]
 
 Get a prompt from html files
 
 positional arguments:
   PATH                  Paths to the html files, or stdin if not provided
                         (default: None)
 
 options:
   -h, --help            show this help message and exit
   -V, --version         show program's version number and exit
   -c, --copy            Copy the prompt to clipboard (default: False)
   -e, --edit            Edit the prompt and copy manually (default: False)
   -m model, --model model
-                        Model to use (default: gpt-3.5-turbo)
+                        Model to use. This only affects the chunk size. Use -S
+                        to disable splitting (infinite chunk size). (default:
+                        gpt-4-32k)
   -S, --no-split        Do not split the prompt into multiple parts (use this
                         if the model has a really large context size)
                         (default: False)
   -s chunk_size, --chunk-size chunk_size
                         Chunk size when splitting transcript, also used to
                         determine whether to split, defaults to 1/2 of the
                         context length limit of the model (default: None)
@@ -324,14 +406,15 @@
   -r, --raw             Wraps the content in triple quotes with no extra text
                         (default: False)
   -R, --raw-no-quotes   Output the content only (default: False)
   --print-percentage-non-ascii
                         Print percentage of non-ascii characters (default:
                         False)
   -n, --dry-run         Dry run (default: False)
+  --out OUT             Output file (default: None)
   -C, --from-clipboard  Load text from clipboard (default: False)
   -w WHAT, --what WHAT  Initial knowledge you want to insert before the PDF
                         content in the prompt (default: the text content of a
                         html file)
   -M, --merge           Merge contents of all pages before processing
                         (default: False)
```

