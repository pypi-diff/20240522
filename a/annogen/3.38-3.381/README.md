# Comparing `tmp/annogen-3.38.tar.gz` & `tmp/annogen-3.381.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "annogen-3.38.tar", last modified: Thu May 16 17:38:20 2024, max compression
+gzip compressed data, was "annogen-3.381.tar", last modified: Wed May 22 07:24:54 2024, max compression
```

## Comparing `annogen-3.38.tar` & `annogen-3.381.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 silbrown   (501) staff       (20)        0 2024-05-16 17:38:20.884886 annogen-3.38/
--rw-r--r--   0 silbrown   (501) staff       (20)    11357 2021-08-21 08:25:30.000000 annogen-3.38/LICENSE
--rw-r--r--   0 silbrown   (501) staff       (20)    36827 2024-05-16 17:38:20.884291 annogen-3.38/PKG-INFO
-drwxr-xr-x   0 silbrown   (501) staff       (20)        0 2024-05-16 17:38:20.880530 annogen-3.38/annogen/
--rw-r--r--   0 silbrown   (501) staff       (20)      128 2024-05-16 17:38:20.000000 annogen-3.38/annogen/__init__.py
--rwxr-xr-x   0 silbrown   (501) staff       (20)   375882 2024-05-16 17:38:20.000000 annogen-3.38/annogen/__main__.py
-drwxr-xr-x   0 silbrown   (501) staff       (20)        0 2024-05-16 17:38:20.883430 annogen-3.38/annogen.egg-info/
--rw-r--r--   0 silbrown   (501) staff       (20)    36827 2024-05-16 17:38:20.000000 annogen-3.38/annogen.egg-info/PKG-INFO
--rw-r--r--   0 silbrown   (501) staff       (20)      214 2024-05-16 17:38:20.000000 annogen-3.38/annogen.egg-info/SOURCES.txt
--rw-r--r--   0 silbrown   (501) staff       (20)        1 2024-05-16 17:38:20.000000 annogen-3.38/annogen.egg-info/dependency_links.txt
--rw-r--r--   0 silbrown   (501) staff       (20)       54 2024-05-16 17:38:20.000000 annogen-3.38/annogen.egg-info/entry_points.txt
--rw-r--r--   0 silbrown   (501) staff       (20)        8 2024-05-16 17:38:20.000000 annogen-3.38/annogen.egg-info/top_level.txt
--rw-r--r--   0 silbrown   (501) staff       (20)       38 2024-05-16 17:38:20.885629 annogen-3.38/setup.cfg
--rw-r--r--   0 silbrown   (501) staff       (20)    36939 2024-05-16 17:38:20.000000 annogen-3.38/setup.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-22 07:24:54.044417 annogen-3.381/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)    11357 2024-05-22 07:17:51.000000 annogen-3.381/LICENSE
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)    36830 2024-05-22 07:24:54.044417 annogen-3.381/PKG-INFO
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-22 07:24:54.044417 annogen-3.381/annogen/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      128 2024-05-22 07:24:53.000000 annogen-3.381/annogen/__init__.py
+-rwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)   375727 2024-05-22 07:24:53.000000 annogen-3.381/annogen/__main__.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2024-05-22 07:24:54.044417 annogen-3.381/annogen.egg-info/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)    36830 2024-05-22 07:24:54.000000 annogen-3.381/annogen.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      214 2024-05-22 07:24:54.000000 annogen-3.381/annogen.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2024-05-22 07:24:54.000000 annogen-3.381/annogen.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       54 2024-05-22 07:24:54.000000 annogen-3.381/annogen.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        8 2024-05-22 07:24:54.000000 annogen-3.381/annogen.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       38 2024-05-22 07:24:54.044417 annogen-3.381/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)    36942 2024-05-22 07:24:53.000000 annogen-3.381/setup.py
```

### Comparing `annogen-3.38/LICENSE` & `annogen-3.381/LICENSE`

 * *Files identical despite different names*

### Comparing `annogen-3.38/PKG-INFO` & `annogen-3.381/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: annogen
-Version: 3.38
+Version: 3.381
 Summary: Annotator Generator, an examples-driven generator of fast text annotators for language learning aids etc
 Home-page: http://ssb22.user.srcf.net/adjuster/annogen.html
 Author: Silas S. Brown
 Author-email: ssb22@cam.ac.uk
 License: Apache 2
-Platform: all
+Platform: any
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=2.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -54,16 +54,16 @@
 Citation
 --------
 
 If you need to cite a peer-reviewed paper:
 
 Silas S. Brown.  Web Annotation with Modified-Yarowsky and Other Algorithms.  Overload 112 (December 2012) pp.4-7.
 
-Options for Annotator Generator v3.37
-=====================================
+Options for Annotator Generator v3.381
+======================================
 
 `-h`, `--help`
  : show this help message and exit
 
 `--infile=`
  : Filename of a text file (or a compressed .gz, .bz2 or .xz file or URL) to read the input examples from. If this is not specified, standard input is used.
```

### Comparing `annogen-3.38/annogen/__main__.py` & `annogen-3.381/annogen/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # (compatible with both Python 2.7 and Python 3)
 
-"Annotator Generator v3.38 (c) 2012-24 Silas S. Brown"
+"Annotator Generator v3.381 (c) 2012-24 Silas S. Brown"
 
 # See http://ssb22.user.srcf.net/adjuster/annogen.html
 
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 
@@ -369,46 +369,42 @@
 
 parser.add_option("-p","--status-prefix",help="Label to add at the start of the status line, for use if you batch-run annogen in multiple configurations and want to know which one is currently running")
 
 if '--html-options' in sys.argv or '--markdown-options' in sys.argv:
   if '--html-options' in sys.argv:
     print ("</dl>")
   sys.exit()
-main = (__name__ == "__main__")
 term = os.environ.get("TERM","")
 is_xterm = "xterm" in term
 ansi_escapes = is_xterm or term in ["screen","linux"]
 def isatty(f): return hasattr(f,"isatty") and f.isatty()
 if ansi_escapes and isatty(sys.stderr): clear_eol,reverse_on,reverse_off,bold_on,bold_off="\x1b[K","\x1b[7m","\x1b[0m","\x1b[1m","\x1b[0m"
 else: clear_eol,reverse_on,reverse_off,bold_on,bold_off="  "," **","** ","",""
-if main: sys.stderr.write(bold_on+__doc__+bold_off+"\n") # not sys.stdout: may or may not be showing --help (and anyway might want to process the help text for website etc)
-# else (if not main), STILL parse options (if we're being imported for parallel processing)
+sys.stderr.write(bold_on+__doc__+bold_off+"\n") # not sys.stdout: may or may not be showing --help (and anyway might want to process the help text for website etc)
 options, args = parser.parse_args()
 globals().update(options.__dict__)
 
 try: import thread
 except: import _thread as thread # Python 3
 import gc ; gc.disable() # should be OK if we don't create cycles (TODO: run gc.collect() manually after init, just in case?)
 
 def warn(msg):
-  if main: sys.stderr.write("Warning: "+msg+"\n")
-  # else it should have already been written
+  sys.stderr.write("Warning: "+msg+"\n")
 if "PyPy" in sys.version: warn("with annogen, PyPy is likely to run 60% slower than python") # (not to mention concurrent.futures being less likely to be available)
 
 if ybytes: ybytes=int(ybytes)
 if ybytes_max: ybytes_max=int(ybytes_max)
 else: ybytes_max = ybytes
 if yarowsky_debug: yarowsky_debug=int(yarowsky_debug)
 else: yarowsky_debug = 0
 if normalise_debug: normalise_debug=int(normalise_debug)
 else: normalise_debug = 0
 ybytes_step = int(ybytes_step)
 ymax_threshold = int(ymax_threshold)
 def errExit(msg):
-  assert main # bad news if this happens in non-main module
   try:
     if not outfile==getBuf(sys.stdout):
       outfile.close() ; rm_f(c_filename)
   except: pass # works only if got past outfile opening
   sys.stderr.write(msg+"\n") ; sys.exit(1)
 if args: errExit("Unknown argument "+repr(args[0]))
 if sharp_multi and not annotation_names and (browser_extension or existing_ruby_lang_regex): errExit("--sharp-multi requires --annotation-names to be set if --browser-extension or --existing-ruby-lang-regex")
@@ -507,20 +503,20 @@
     if library: cOnly("--library")
     if not outcode=="utf-8": cOnly("Non utf-8 outcode")
     if compress: cOnly("--compress")
     if sum(1 for x in [java,javascript,python,dart] if x) > 1:
       errExit("Outputting more than one programming language on the same run is not yet implemented")
     if java:
       if android and not "/src//" in java: errExit("When using --android, the last thing before the // in --java must be 'src' e.g. --java=/workspace/MyProject/src//org/example/package")
-      if main and not compile_only: # (delete previous files, only if we're not a subprocess)
+      if not compile_only: # (delete previous files, only if we're not a subprocess)
        os.system("mkdir -p "+shell_escape(java))
        for f in os.listdir(java):
         if f.endswith(".java") and f.startswith("z"): os.remove(java+os.sep+f)
       c_filename = java+os.sep+"Annotator.java"
-      if main and android:
+      if android:
         os.system("rm -rf "+shell_escape(jSrc+"/../bin")) # needed to get rid of old *.class files that might be no longer used
         for d in ["assets","bin","gen","res/layout","res/menu","res/values","res/xml"]: os.system("mkdir -p "+shell_escape(jSrc+"/../"+d))
     elif c_filename.endswith(".c"):
       if javascript: c_filename = c_filename[:-2]+".js"
       elif dart: c_filename = c_filename[:-2]+".dart"
       else: c_filename = c_filename[:-2]+".py"
 elif windows_clipboard:
@@ -595,15 +591,14 @@
 if single_words: max_words = 1
 if read_rules and diagnose_manual: errExit("--diagnose-manual is not compatible with --read-rules")
 suffix_minlen=int(suffix_minlen)
 
 if compress:
   squashStrings = set() ; squashReplacements = []
   def squashFinish():
-    assert main, "squashFinish sets globals"
     global squashStrings # so can set it to "done" at end
     tokens = set()
     for s in squashStrings: tokens.update(list(S(s)))
     totSaved = 0
     tokens = [chr(t) for t in range(1,256) if not chr(t) in tokens] ; orig_tokens = set(tokens)
     pairs = [chr(0)] * 512
     while tokens and squashStrings:
@@ -4089,15 +4084,14 @@
     global corpus_unistr,allWords,cu_lower_nospaces
     if normalise_cache:
       try:
         corpus_unistr = openfile(normalise_cache).read().decode('utf-8')
         sys.stderr.write("Normalised copy loaded\n")
         return True # loaded from cache
       except: pass
-    assert main, "normalise called in non-main module"
     if (capitalisation and annot_whitespace) or priority_list: return # TODO: might want to normalise at least the word breaks if priority_list (but it loads it anyway if cached)
     sys.stderr.write("Normalising...");sys.stderr.flush()
     old_caps = capitalisation
     if priority_list: capitalisation = True # no point keeping it at False
     allWords = getAllWords()
     if removeSpace:
      corpus_unistr = re.sub(re.escape(markupEnd)+r'\s+'+re.escape(markupStart),(markupEnd+markupStart).replace('\\',r'\\'),corpus_unistr,flags=re.UNICODE) # so getOkStarts works consistently if corpus has some space-separated and some not
@@ -4791,15 +4785,14 @@
     diagnose_limit -= 1
     if not diagnose_limit:
       diagnose = False
       diagnose_write("limit reached, suppressing further diagnostics")
 
 def generate_map():
     global m2c_map, precalc_sets, yPriorityDic
-    assert main, "Only main should generate corpus map"
     sys.stderr.write("Generating corpus map... ")
     m2c_map = {} ; precalc_sets = {}
     muStart = downLenSoFar = 0
     for s in re.finditer(re.escape(markupStart), corpus_unistr):
       s=s.start()
       md = markDown(corpus_unistr[muStart:s])
       if markupStart in md: errExit("examples have nested markup! "+repr(md))
@@ -4825,22 +4818,23 @@
           yPriorityDic[wd] = w
     sys.stderr.write("done\n")
 
 executor = None
 def setup_parallelism(): # returns number of cores
     global executor
     if single_core: return 1
-    elif not hasattr(os,'fork'): return 1 # e.g. Windows, would need to write to filesystem like versions of annogen before 3.183 (and may get muddled up if running from __main__.py under python -m)
+    elif not hasattr(os,'fork'): return 1 # e.g. Windows, would need to write to filesystem like versions of annogen before 3.183 and distinguish main/non-main like versions of annogen before 3.38 (may get muddled up if running from __main__.py under python -m)
     elif executor: executor.shutdown(True) # MUST wait for the shutdown to finish before creating a new instance: some implementations seem to have a race condition
     try:
       import multiprocessing
       params = [multiprocessing.cpu_count()-1]
       if params[0] <= 0: return 1
       if hasattr(multiprocessing,"get_context"): params.append(multiprocessing.get_context('fork')) # Python 3.4+: if this raises ValueError, we can't fork so won't multiprocess
-      import concurrent.futures # sudo pip install futures (2.7 backport of 3.2 standard library)
+      import concurrent.futures # Python 3.  On Python 2, you can try the backport via 'pip install futures' but deadlock is possible.  And seems to occur when annogen __name__ is not "__main__" after first normBatch returns, not sure why:
+      if not (type("")==type(u"") or __name__=="__main__"): raise Exception("Python 2 as submodule is known to deadlock unless multicore disabled")
       executor = concurrent.futures.ProcessPoolExecutor(*params)
       # Do not reduce Python 2's sys.setcheckinterval() (or Python 3's setswitchinterval) if using ProcessPoolExecutor, or job starts can be delayed.
       cores = multiprocessing.cpu_count()
       if cores_command: os.system("%s %d" % (cores_command,cores))
       return cores
     except: return 1 # can't fork for some reason
 
@@ -5318,15 +5312,15 @@
   open(dirToUse+"/content.js","wb").write(jsAnnot(False,True))
   open(dirToUse+"/config.html","wb").write(extension_config)
   open(dirToUse+"/config.js","wb").write(extension_confjs)
   open(dirToUse+"/ruby.css","wb").write(extension_rubycss)
   global c_filename
   c_filename = dirToUse+"/annotate-dat.txt"
 
-if isatty(sys.stdout) and not java and main and not priority_list and not browser_extension and not write_rules: sys.stderr.write("Will write to "+c_filename+"\n") # will open it later (avoid having a 0-length file sitting around during the analyse() run so you don't rm it by mistake)
+if isatty(sys.stdout) and not java and not priority_list and not browser_extension and not write_rules: sys.stderr.write("Will write to "+c_filename+"\n") # will open it later (avoid having a 0-length file sitting around during the analyse() run so you don't rm it by mistake)
 
 def openfile(fname,mode='r'):
     lzma = bz2 = None
     mode += 'b' # Python 2+3 compatibility: always binary
     if fname.endswith(".xz"): import lzma # 'pip install lzma' or 'apt-get install python2.7-lzma' may be required for .xz files
     elif fname.endswith(".bz2"): import bz2
     if re.match("https?://",fname) or fname.startswith("ftp://"):
@@ -5364,24 +5358,22 @@
   if not isatty(sys.stderr): return
   if t: atexit.register(set_title,"")
   is_screen = (term=="screen" and os.environ.get("STY",""))
   is_tmux = (term=="screen" and os.environ.get("TMUX",""))
   if is_xterm or is_tmux: sys.stderr.write("\033]0;%s\007" % (t,)) # ("0;" sets both title and minimised title, "1;" sets minimised title, "2;" sets title.  Tmux takes its pane title from title (but doesn't display it in the titlebar))
   elif is_screen: os.system("screen -X title \"%s\"" % (t,))
 def diagnose_write(s,label="Diagnose"):
-  if not main: start="\n"
-  else: start=""
-  getBuf(sys.stderr).write(B(start+bold_on+label+": "+bold_off)+s.encode(terminal_charset,'replace')+B(clear_eol+'\n'))
+  getBuf(sys.stderr).write(B(bold_on+label+": "+bold_off)+s.encode(terminal_charset,'replace')+B(clear_eol+'\n'))
 try: screenWidth = int(os.environ['COLUMNS'])
 except:
   import struct, fcntl, termios
   try: screenWidth = struct.unpack('hh',fcntl.ioctl(sys.stderr,termios.TIOCGWINSZ,'xxxx'))[1]
   except: screenWidth = 45 # conservative
 
-if main and not compile_only:
+if not compile_only:
  set_title("annogen")
  if read_rules: rulesAndConds = loadRules()
  else:
   read_and_normalise()
   if priority_list:
     if os.path.exists(priority_list):
       sys.stderr.write("Reading "+priority_list+"\n")
@@ -5425,22 +5417,21 @@
 def cmd_or_exit(cmd):
   sys.stderr.write(cmd+"\n")
   r = os.system(cmd)
   if not r: return
   if r&0xFF == 0: r >>= 8 # POSIX
   sys.exit(r)
 
-if main and not compile_only:
+if not compile_only:
  if browser_extension: setup_browser_extension()
  if c_filename: outfile = openfile(c_filename,'w')
  else: outfile = getBuf(sys.stdout)
  outputParser(rulesAndConds) ; del rulesAndConds
  outfile.close() ; sys.stderr.write("Output complete\n")
-if main:
- if android:
+if android:
    can_compile_android = all(x in os.environ for x in ["SDK","PLATFORM","BUILD_TOOLS"])
    can_track_android = (can_compile_android and android_upload) or ("GOOGLE_PLAY_TRACK" in os.environ and "SERVICE_ACCOUNT_KEY" in os.environ and not os.environ.get("ANDROID_NO_RETRACK",""))
    if can_compile_android and compile_only and android_upload: update_android_manifest() # AndroidManifest.xml will not have been updated, so we'd better do it now
    if can_compile_android or can_track_android:
      os.chdir(jSrc+"/..")
      dirName0 = S(getoutput("pwd|sed -e s,.*./,,"))
      dirName = shell_escape(dirName0)
@@ -5522,13 +5513,13 @@
 
 On Google Play you may wish to set Release management -
    Pre-launch report - Settings - Enable pre-launch
    reports to OFF, or it'll report issues on the websites
    you link to (and maybe crashes due to Firebase issues),
    which (if you don't want them) is wasting resources.
 """) # TODO: try if("true".equals(android.provider.Settings.System.getString(getContentResolver(),"firebase.test.lab"))) browser.loadUrl("about:blank"); (but turning off unwanted reports is better)
- elif c_filename and c_compiler:
+elif c_filename and c_compiler:
     cmd = c_compiler # should include any -o option
     if zlib: cmd += " -lz" # TODO: is this always correct on all platforms? (although user can always simply redirect the C to a file and compile separately)
     cmd_or_exit(cmd + " " + shell_escape(c_filename))
- elif compile_only: errExit("Don't know what compiler to run for this set of options")
+elif compile_only: errExit("Don't know what compiler to run for this set of options")
 def placebo(): pass # for setuptools entry_points
```

### Comparing `annogen-3.38/annogen.egg-info/PKG-INFO` & `annogen-3.381/annogen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: annogen
-Version: 3.38
+Version: 3.381
 Summary: Annotator Generator, an examples-driven generator of fast text annotators for language learning aids etc
 Home-page: http://ssb22.user.srcf.net/adjuster/annogen.html
 Author: Silas S. Brown
 Author-email: ssb22@cam.ac.uk
 License: Apache 2
-Platform: all
+Platform: any
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=2.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -54,16 +54,16 @@
 Citation
 --------
 
 If you need to cite a peer-reviewed paper:
 
 Silas S. Brown.  Web Annotation with Modified-Yarowsky and Other Algorithms.  Overload 112 (December 2012) pp.4-7.
 
-Options for Annotator Generator v3.37
-=====================================
+Options for Annotator Generator v3.381
+======================================
 
 `-h`, `--help`
  : show this help message and exit
 
 `--infile=`
  : Filename of a text file (or a compressed .gz, .bz2 or .xz file or URL) to read the input examples from. If this is not specified, standard input is used.
```

### Comparing `annogen-3.38/setup.py` & `annogen-3.381/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from setuptools import setup, find_packages;setup(name='annogen',version='3.38',entry_points={'console_scripts':['annogen=annogen.__main__:placebo']},license='Apache 2',platforms='all',url='http://ssb22.user.srcf.net/adjuster/annogen.html',author='Silas S. Brown',author_email='ssb22@cam.ac.uk',description='Annotator Generator, an examples-driven generator of fast text annotators for language learning aids etc',long_description=r'''Annotator Generator
+from setuptools import setup, find_packages;setup(name='annogen',version='3.381',entry_points={'console_scripts':['annogen=annogen.__main__:placebo']},license='Apache 2',platforms='any',url='http://ssb22.user.srcf.net/adjuster/annogen.html',author='Silas S. Brown',author_email='ssb22@cam.ac.uk',description='Annotator Generator, an examples-driven generator of fast text annotators for language learning aids etc',long_description=r'''Annotator Generator
 ===================
 
 Annotator Generator is an examples-driven generator of fast text annotators. “Annotate” in this context means to add pronunciation or other information to each word, and/or to split text into words in a language that does not use spaces.
 
 * You supply a corpus of pre-annotated texts for Annotator Generator to work out the rules and exceptions
 
 * Annotator Generator creates table-driven code in C, Java, Javascript, Dart or Python with 2 and 3 compatibility
@@ -37,16 +37,16 @@
 Citation
 --------
 
 If you need to cite a peer-reviewed paper:
 
 Silas S. Brown.  Web Annotation with Modified-Yarowsky and Other Algorithms.  Overload 112 (December 2012) pp.4-7.
 
-Options for Annotator Generator v3.37
-=====================================
+Options for Annotator Generator v3.381
+======================================
 
 `-h`, `--help`
  : show this help message and exit
 
 `--infile=`
  : Filename of a text file (or a compressed .gz, .bz2 or .xz file or URL) to read the input examples from. If this is not specified, standard input is used.
```

