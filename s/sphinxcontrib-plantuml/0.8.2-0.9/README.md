# Comparing `tmp/sphinxcontrib-plantuml-0.8.2.tar.gz` & `tmp/sphinxcontrib-plantuml-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sphinxcontrib-plantuml-0.8.2.tar", last modified: Fri Nov  3 03:16:32 2017, max compression
+gzip compressed data, was "dist/sphinxcontrib-plantuml-0.9.tar", last modified: Sat Jan 13 14:45:55 2018, max compression
```

## Comparing `sphinxcontrib-plantuml-0.8.2.tar` & `sphinxcontrib-plantuml-0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 yuya      (1000) yuya      (1000)        0 2017-11-03 03:16:32.000000 sphinxcontrib-plantuml-0.8.2/
-drwxr-xr-x   0 yuya      (1000) yuya      (1000)        0 2017-11-03 03:16:32.000000 sphinxcontrib-plantuml-0.8.2/sphinxcontrib_plantuml.egg-info/
--rw-r--r--   0 yuya      (1000) yuya      (1000)     3203 2017-11-03 03:16:32.000000 sphinxcontrib-plantuml-0.8.2/sphinxcontrib_plantuml.egg-info/PKG-INFO
--rw-r--r--   0 yuya      (1000) yuya      (1000)        1 2017-11-03 03:16:32.000000 sphinxcontrib-plantuml-0.8.2/sphinxcontrib_plantuml.egg-info/dependency_links.txt
--rw-r--r--   0 yuya      (1000) yuya      (1000)      422 2017-11-03 03:16:32.000000 sphinxcontrib-plantuml-0.8.2/sphinxcontrib_plantuml.egg-info/SOURCES.txt
--rw-r--r--   0 yuya      (1000) yuya      (1000)       12 2017-11-03 03:16:32.000000 sphinxcontrib-plantuml-0.8.2/sphinxcontrib_plantuml.egg-info/requires.txt
--rw-r--r--   0 yuya      (1000) yuya      (1000)        1 2017-11-03 03:16:32.000000 sphinxcontrib-plantuml-0.8.2/sphinxcontrib_plantuml.egg-info/not-zip-safe
--rw-r--r--   0 yuya      (1000) yuya      (1000)       14 2017-11-03 03:16:32.000000 sphinxcontrib-plantuml-0.8.2/sphinxcontrib_plantuml.egg-info/namespace_packages.txt
--rw-r--r--   0 yuya      (1000) yuya      (1000)       14 2017-11-03 03:16:32.000000 sphinxcontrib-plantuml-0.8.2/sphinxcontrib_plantuml.egg-info/top_level.txt
--rw-r--r--   0 yuya      (1000) yuya      (1000)     3203 2017-11-03 03:16:32.000000 sphinxcontrib-plantuml-0.8.2/PKG-INFO
--rw-r--r--   0 yuya      (1000) yuya      (1000)       49 2017-10-21 09:59:59.000000 sphinxcontrib-plantuml-0.8.2/MANIFEST.in
--rw-r--r--   0 yuya      (1000) yuya      (1000)     1841 2017-11-03 03:04:58.000000 sphinxcontrib-plantuml-0.8.2/README.rst
--rw-r--r--   0 yuya      (1000) yuya      (1000)     1053 2017-11-03 03:05:54.000000 sphinxcontrib-plantuml-0.8.2/setup.py
-drwxr-xr-x   0 yuya      (1000) yuya      (1000)        0 2017-11-03 03:16:32.000000 sphinxcontrib-plantuml-0.8.2/sphinxcontrib/
--rw-r--r--   0 yuya      (1000) yuya      (1000)    12438 2017-11-03 03:00:48.000000 sphinxcontrib-plantuml-0.8.2/sphinxcontrib/plantuml.py
--rw-r--r--   0 yuya      (1000) yuya      (1000)      366 2017-10-21 09:59:59.000000 sphinxcontrib-plantuml-0.8.2/sphinxcontrib/__init__.py
--rw-r--r--   0 yuya      (1000) yuya      (1000)       76 2017-11-03 03:16:32.000000 sphinxcontrib-plantuml-0.8.2/setup.cfg
+drwxr-xr-x   0 yuya      (1000) yuya      (1000)        0 2018-01-13 14:45:55.000000 sphinxcontrib-plantuml-0.9/
+drwxr-xr-x   0 yuya      (1000) yuya      (1000)        0 2018-01-13 14:45:55.000000 sphinxcontrib-plantuml-0.9/sphinxcontrib_plantuml.egg-info/
+-rw-r--r--   0 yuya      (1000) yuya      (1000)     3201 2018-01-13 14:45:55.000000 sphinxcontrib-plantuml-0.9/sphinxcontrib_plantuml.egg-info/PKG-INFO
+-rw-r--r--   0 yuya      (1000) yuya      (1000)        1 2018-01-13 14:45:55.000000 sphinxcontrib-plantuml-0.9/sphinxcontrib_plantuml.egg-info/dependency_links.txt
+-rw-r--r--   0 yuya      (1000) yuya      (1000)      422 2018-01-13 14:45:55.000000 sphinxcontrib-plantuml-0.9/sphinxcontrib_plantuml.egg-info/SOURCES.txt
+-rw-r--r--   0 yuya      (1000) yuya      (1000)       12 2018-01-13 14:45:55.000000 sphinxcontrib-plantuml-0.9/sphinxcontrib_plantuml.egg-info/requires.txt
+-rw-r--r--   0 yuya      (1000) yuya      (1000)        1 2018-01-13 14:45:41.000000 sphinxcontrib-plantuml-0.9/sphinxcontrib_plantuml.egg-info/not-zip-safe
+-rw-r--r--   0 yuya      (1000) yuya      (1000)       14 2018-01-13 14:45:55.000000 sphinxcontrib-plantuml-0.9/sphinxcontrib_plantuml.egg-info/namespace_packages.txt
+-rw-r--r--   0 yuya      (1000) yuya      (1000)       14 2018-01-13 14:45:55.000000 sphinxcontrib-plantuml-0.9/sphinxcontrib_plantuml.egg-info/top_level.txt
+-rw-r--r--   0 yuya      (1000) yuya      (1000)     3201 2018-01-13 14:45:55.000000 sphinxcontrib-plantuml-0.9/PKG-INFO
+-rw-r--r--   0 yuya      (1000) yuya      (1000)       49 2017-10-21 09:59:59.000000 sphinxcontrib-plantuml-0.9/MANIFEST.in
+-rw-r--r--   0 yuya      (1000) yuya      (1000)     1841 2017-11-03 03:04:58.000000 sphinxcontrib-plantuml-0.9/README.rst
+-rw-r--r--   0 yuya      (1000) yuya      (1000)     1051 2018-01-13 14:44:49.000000 sphinxcontrib-plantuml-0.9/setup.py
+drwxr-xr-x   0 yuya      (1000) yuya      (1000)        0 2018-01-13 14:45:55.000000 sphinxcontrib-plantuml-0.9/sphinxcontrib/
+-rw-r--r--   0 yuya      (1000) yuya      (1000)    12247 2017-12-23 04:08:02.000000 sphinxcontrib-plantuml-0.9/sphinxcontrib/plantuml.py
+-rw-r--r--   0 yuya      (1000) yuya      (1000)      366 2017-10-21 09:59:59.000000 sphinxcontrib-plantuml-0.9/sphinxcontrib/__init__.py
+-rw-r--r--   0 yuya      (1000) yuya      (1000)       76 2018-01-13 14:45:55.000000 sphinxcontrib-plantuml-0.9/setup.cfg
```

### Comparing `sphinxcontrib-plantuml-0.8.2/sphinxcontrib_plantuml.egg-info/PKG-INFO` & `sphinxcontrib-plantuml-0.9/sphinxcontrib_plantuml.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: sphinxcontrib-plantuml
-Version: 0.8.2
+Version: 0.9
 Summary: Sphinx "plantuml" extension
 Home-page: https://github.com/sphinx-contrib/plantuml/
 Author: Yuya Nishihara
 Author-email: yuya@tcha.org
 License: BSD
 Download-URL: https://pypi.python.org/pypi/sphinxcontrib-plantuml
 Description-Content-Type: UNKNOWN
```

### Comparing `sphinxcontrib-plantuml-0.8.2/PKG-INFO` & `sphinxcontrib-plantuml-0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: sphinxcontrib-plantuml
-Version: 0.8.2
+Version: 0.9
 Summary: Sphinx "plantuml" extension
 Home-page: https://github.com/sphinx-contrib/plantuml/
 Author: Yuya Nishihara
 Author-email: yuya@tcha.org
 License: BSD
 Download-URL: https://pypi.python.org/pypi/sphinxcontrib-plantuml
 Description-Content-Type: UNKNOWN
```

### Comparing `sphinxcontrib-plantuml-0.8.2/README.rst` & `sphinxcontrib-plantuml-0.9/README.rst`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-plantuml-0.8.2/setup.py` & `sphinxcontrib-plantuml-0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 long_desc = open('README.rst').read()
 
 requires = ['Sphinx>=1.1']
 
 setup(
     name='sphinxcontrib-plantuml',
-    version='0.8.2',
+    version='0.9',
     url='https://github.com/sphinx-contrib/plantuml/',
     download_url='https://pypi.python.org/pypi/sphinxcontrib-plantuml',
     license='BSD',
     author='Yuya Nishihara',
     author_email='yuya@tcha.org',
     description='Sphinx "plantuml" extension',
     long_description=long_desc,
```

### Comparing `sphinxcontrib-plantuml-0.8.2/sphinxcontrib/plantuml.py` & `sphinxcontrib-plantuml-0.9/sphinxcontrib/plantuml.py`

 * *Files 4% similar despite different names*

```diff
@@ -87,14 +87,15 @@
         else:
             relfn = env.doc2path(env.docname, base=None)
             umlcode = '\n'.join(self.content)
 
         node = plantuml(self.block_text, **self.options)
         node['uml'] = umlcode
         node['incdir'] = os.path.dirname(relfn)
+        node['filename'] = os.path.split(relfn)[1]
 
         # XXX maybe this should be moved to _visit_plantuml functions. it
         # seems wrong to insert "figure" node by "plantuml" directive.
         if 'caption' in self.options or 'align' in self.options:
             node = nodes.figure('', node)
             if 'align' in self.options:
                 node['align'] = self.options['align']
@@ -133,33 +134,34 @@
 
 _ARGS_BY_FILEFORMAT = {
     'eps': '-teps'.split(),
     'png': (),
     'svg': '-tsvg'.split(),
     }
 
-def generate_plantuml_args(self, fileformat):
+def generate_plantuml_args(self, node, fileformat):
     if isinstance(self.builder.config.plantuml, (tuple, list)):
         args = list(self.builder.config.plantuml)
     else:
         args = shlex.split(self.builder.config.plantuml)
     args.extend('-pipe -charset utf-8'.split())
+    args.extend(['-filename', node['filename']])
     args.extend(_ARGS_BY_FILEFORMAT[fileformat])
     return args
 
 def render_plantuml(self, node, fileformat):
     refname, outfname = generate_name(self, node, fileformat)
     if os.path.exists(outfname):
         return refname, outfname  # don't regenerate
     absincdir = os.path.join(self.builder.srcdir, node['incdir'])
     ensuredir(os.path.dirname(outfname))
     f = open(outfname, 'wb')
     try:
         try:
-            p = subprocess.Popen(generate_plantuml_args(self, fileformat),
+            p = subprocess.Popen(generate_plantuml_args(self, node, fileformat),
                                  stdout=f, stdin=subprocess.PIPE,
                                  stderr=subprocess.PIPE,
                                  cwd=absincdir)
         except OSError as err:
             if err.errno != ENOENT:
                 raise
             raise PlantUmlError('plantuml command %r cannot be run'
@@ -168,71 +170,53 @@
         if p.returncode != 0:
             raise PlantUmlError('error while running plantuml\n\n%s' % serr)
         return refname, outfname
     finally:
         f.close()
 
 def _get_png_tag(self, fnames, node):
-    refname, _outfname = fnames['png']
+    refname, outfname = fnames['png']
     alt = node.get('alt', node['uml'])
 
     # mimic StandaloneHTMLBuilder.post_process_images(). maybe we should
     # process images prior to html_vist.
     scale_keys = ('scale', 'width', 'height')
     if all(key not in node for key in scale_keys) or Image is None:
         return ('<img src="%s" alt="%s" />\n'
                 % (self.encode(refname), self.encode(alt)))
 
-    # Get sizes from the rendered image (defaults)
-    im = Image.open(_outfname)
-    im.load()
-    (fw, fh) = im.size
+    scale = node.get('scale', 100)
+    styles = []
 
-    # Regex to get value and units
+    # Width/Height
     vu = re.compile(r"(?P<value>\d+)\s*(?P<units>[a-zA-Z%]+)?")
-
-    # Width
-    if 'width' in node:
-        m = vu.match(node['width'])
+    for a in ['width', 'height']:
+        if a not in node:
+            continue
+        m = vu.match(node[a])
         if not m:
-            raise PlantUmlError('Invalid width')
-        else:
-            m = m.groupdict()
+            raise PlantUmlError('Invalid %s' % a)
+        m = m.groupdict()
         w = int(m['value'])
         wu = m['units'] if m['units'] else 'px'
-    else:
-        w = fw
-        wu = 'px'
-
-    # Height
-    if 'height' in node:
-        m = vu.match(node['height'])
-        if not m:
-            raise PlantUmlError('Invalid height')
-        else:
-            m = m.groupdict()
-        h = int(m['value'])
-        hu = m['units'] if m['units'] else 'px'
-    else:
-        h = fh
-        hu = 'px'
+        styles.append('%s: %s%s' % (a, w * scale / 100, wu))
 
-    # Scale
-    if 'scale' not in node:
-        node['scale'] = 100
+    # Add physical size to assist rendering (defaults)
+    if not styles:
+        im = Image.open(outfname)
+        im.load()
+        styles.extend('%s: %s%s' % (a, w * scale / 100, 'px')
+                      for a, w in zip(['width', 'height'], im.size))
 
-    return ('<a href="%s"><img src="%s" alt="%s" width="%s%s" height="%s%s"/>'
+    return ('<a href="%s"><img src="%s" alt="%s" style="%s"/>'
             '</a>\n'
             % (self.encode(refname),
                self.encode(refname),
                self.encode(alt),
-               self.encode(w * node['scale'] / 100),
-               self.encode(wu),
-               self.encode(h * node['scale'] / 100),
-               self.encode(hu)))
+               self.encode('; '.join(styles))))
 
 def _get_svg_style(fname):
     f = open(fname)
     try:
         for l in f:
             m = re.search(r'<svg\b([^<>]+)', l)
             if m:
```

