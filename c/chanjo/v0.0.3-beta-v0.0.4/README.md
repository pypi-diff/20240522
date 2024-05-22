# Comparing `tmp/chanjo-v0.0.3-beta.tar.gz` & `tmp/chanjo-v0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/chanjo-v0.0.3-beta.tar", last modified: Tue Sep  3 09:17:38 2013, max compression
+gzip compressed data, was "dist/chanjo-v0.0.4.tar", last modified: Mon Sep 16 11:22:26 2013, max compression
```

## Comparing `chanjo-v0.0.3-beta.tar` & `chanjo-v0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 robinandeer   (501) staff       (20)        0 2013-09-03 09:17:38.000000 chanjo-v0.0.3-beta/
-drwxr-xr-x   0 robinandeer   (501) staff       (20)        0 2013-09-03 09:17:38.000000 chanjo-v0.0.3-beta/chanjo/
--rw-r--r--   0 robinandeer   (501) staff       (20)      217 2013-09-03 09:15:38.000000 chanjo-v0.0.3-beta/chanjo/__init__.py
--rw-r--r--   0 robinandeer   (501) staff       (20)     1948 2013-09-03 09:13:47.000000 chanjo-v0.0.3-beta/chanjo/bam.py
--rw-r--r--   0 robinandeer   (501) staff       (20)     5531 2013-09-03 09:13:47.000000 chanjo-v0.0.3-beta/chanjo/ccds2sql.py
--rw-r--r--   0 robinandeer   (501) staff       (20)     4798 2013-09-03 09:13:47.000000 chanjo-v0.0.3-beta/chanjo/core.py
--rw-r--r--   0 robinandeer   (501) staff       (20)    15569 2013-09-03 09:13:47.000000 chanjo-v0.0.3-beta/chanjo/sql.py
--rw-r--r--   0 robinandeer   (501) staff       (20)     2864 2013-09-03 09:13:47.000000 chanjo-v0.0.3-beta/chanjo/utils.py
-drwxr-xr-x   0 robinandeer   (501) staff       (20)        0 2013-09-03 09:17:38.000000 chanjo-v0.0.3-beta/chanjo.egg-info/
--rw-r--r--   0 robinandeer   (501) staff       (20)        1 2013-09-03 09:17:38.000000 chanjo-v0.0.3-beta/chanjo.egg-info/dependency_links.txt
--rw-r--r--   0 robinandeer   (501) staff       (20)      326 2013-09-03 09:17:38.000000 chanjo-v0.0.3-beta/chanjo.egg-info/PKG-INFO
--rw-r--r--   0 robinandeer   (501) staff       (20)       53 2013-09-03 09:17:38.000000 chanjo-v0.0.3-beta/chanjo.egg-info/requires.txt
--rw-r--r--   0 robinandeer   (501) staff       (20)      282 2013-09-03 09:17:38.000000 chanjo-v0.0.3-beta/chanjo.egg-info/SOURCES.txt
--rw-r--r--   0 robinandeer   (501) staff       (20)        7 2013-09-03 09:17:38.000000 chanjo-v0.0.3-beta/chanjo.egg-info/top_level.txt
--rw-r--r--   0 robinandeer   (501) staff       (20)      326 2013-09-03 09:17:38.000000 chanjo-v0.0.3-beta/PKG-INFO
-drwxr-xr-x   0 robinandeer   (501) staff       (20)        0 2013-09-03 09:17:38.000000 chanjo-v0.0.3-beta/scripts/
--rw-r--r--   0 robinandeer   (501) staff       (20)     2893 2013-09-03 09:13:47.000000 chanjo-v0.0.3-beta/scripts/chanjo-autopilot.py
--rw-r--r--   0 robinandeer   (501) staff       (20)       59 2013-09-03 09:17:38.000000 chanjo-v0.0.3-beta/setup.cfg
--rw-r--r--   0 robinandeer   (501) staff       (20)      713 2013-09-03 09:13:47.000000 chanjo-v0.0.3-beta/setup.py
+drwxr-xr-x   0 robinandeer   (501) staff       (20)        0 2013-09-16 11:22:26.000000 chanjo-v0.0.4/
+drwxr-xr-x   0 robinandeer   (501) staff       (20)        0 2013-09-16 11:22:26.000000 chanjo-v0.0.4/chanjo/
+-rw-r--r--   0 robinandeer   (501) staff       (20)      212 2013-09-16 11:20:40.000000 chanjo-v0.0.4/chanjo/__init__.py
+-rw-r--r--   0 robinandeer   (501) staff       (20)     1948 2013-09-03 13:27:25.000000 chanjo-v0.0.4/chanjo/bam.py
+-rw-r--r--   0 robinandeer   (501) staff       (20)     5531 2013-09-03 13:27:25.000000 chanjo-v0.0.4/chanjo/ccds2sql.py
+-rw-r--r--   0 robinandeer   (501) staff       (20)     4826 2013-09-16 11:20:40.000000 chanjo-v0.0.4/chanjo/core.py
+-rw-r--r--   0 robinandeer   (501) staff       (20)    16057 2013-09-16 11:20:40.000000 chanjo-v0.0.4/chanjo/sql.py
+-rw-r--r--   0 robinandeer   (501) staff       (20)     1523 2013-09-16 11:20:40.000000 chanjo-v0.0.4/chanjo/utils.py
+drwxr-xr-x   0 robinandeer   (501) staff       (20)        0 2013-09-16 11:22:26.000000 chanjo-v0.0.4/chanjo.egg-info/
+-rw-r--r--   0 robinandeer   (501) staff       (20)        1 2013-09-16 11:22:26.000000 chanjo-v0.0.4/chanjo.egg-info/dependency_links.txt
+-rw-r--r--   0 robinandeer   (501) staff       (20)      321 2013-09-16 11:22:26.000000 chanjo-v0.0.4/chanjo.egg-info/PKG-INFO
+-rw-r--r--   0 robinandeer   (501) staff       (20)       43 2013-09-16 11:22:26.000000 chanjo-v0.0.4/chanjo.egg-info/requires.txt
+-rw-r--r--   0 robinandeer   (501) staff       (20)      282 2013-09-16 11:22:26.000000 chanjo-v0.0.4/chanjo.egg-info/SOURCES.txt
+-rw-r--r--   0 robinandeer   (501) staff       (20)        7 2013-09-16 11:22:26.000000 chanjo-v0.0.4/chanjo.egg-info/top_level.txt
+-rw-r--r--   0 robinandeer   (501) staff       (20)      321 2013-09-16 11:22:26.000000 chanjo-v0.0.4/PKG-INFO
+drwxr-xr-x   0 robinandeer   (501) staff       (20)        0 2013-09-16 11:22:26.000000 chanjo-v0.0.4/scripts/
+-rw-r--r--   0 robinandeer   (501) staff       (20)     2862 2013-09-16 11:20:40.000000 chanjo-v0.0.4/scripts/chanjo-autopilot.py
+-rw-r--r--   0 robinandeer   (501) staff       (20)       59 2013-09-16 11:22:26.000000 chanjo-v0.0.4/setup.cfg
+-rw-r--r--   0 robinandeer   (501) staff       (20)      692 2013-09-16 11:20:40.000000 chanjo-v0.0.4/setup.py
```

### Comparing `chanjo-v0.0.3-beta/chanjo/bam.py` & `chanjo-v0.0.4/chanjo/bam.py`

 * *Files identical despite different names*

### Comparing `chanjo-v0.0.3-beta/chanjo/ccds2sql.py` & `chanjo-v0.0.4/chanjo/ccds2sql.py`

 * *Files identical despite different names*

### Comparing `chanjo-v0.0.3-beta/chanjo/core.py` & `chanjo-v0.0.4/chanjo/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
   the only part of the package you directly interact with.
 
   :copyright: (c) 2013 by Robin Andeer
   :license: MIT, see LICENSE for more details
 """
 
 import zlib
+import itertools
 
 
 class Hub(object):
   """
   The :class:`Hub` is the core component of Chanjo. When you plug in the
   adapters, it will create handy shortcuts to easily reach common methods.
 
@@ -141,11 +142,11 @@
     Because of how compression works I believe this will be sort of the same
     as generating BEDGraph intervals to compress the information.
 
     :param list depths: Array of read depth (float or int)
     :returns: Compressed string of read depths
     """
     # Turn floats to ints, then to strings, then concat with "|"-separator
-    str_depths = "|".join(map(str, map(int, depths)))
+    str_depths = "|".join(itertools.imap(str, map(int, depths)))
 
     # Compress and return compressed string
     return zlib.compress(str_depths)
```

### Comparing `chanjo-v0.0.3-beta/chanjo/sql.py` & `chanjo-v0.0.4/chanjo/sql.py`

 * *Files 3% similar despite different names*

```diff
@@ -269,14 +269,28 @@
     # Fetch the element class ORM object
     klass = self._getClass(elemClass)
 
     # Filter by "WHERE ``attr`` IS NOT NULL".
     return self.session.query(klass).filter(getattr(klass, attr) != None)\
                                     .count()
 
+  def inadequateBaseEstimate(self, elemClass="Exon"):
+    """
+    Calculates an estimate number of bases with inadequate coverage baesd on
+    the completeness score and the cutoff used. Not perfectly accurate since
+    there is overlap between all elements.
+    """
+    rawSQL = """
+    SELECT sum(completeness * (end-start))/sum(end-start)
+    FROM {elem}
+    """.format(elem=elemClass.capitalize())
+
+    return self.session.execute(rawSQL).fetchall()
+
+
 # =============================================================================
 #   Association tables
 # -----------------------------------------------------------------------------
 Exon_Gene = sql.Table('Exon_Gene', Base.metadata,
     sql.Column('exon_id', sql.String, sql.ForeignKey('Exon.id')),
     sql.Column('gene_id', sql.String, sql.ForeignKey('Gene.id'))
 )
@@ -449,14 +463,15 @@
 
   id = sql.Column(sql.String, primary_key=True)
   chrom = sql.Column(sql.String)
   start = sql.Column(sql.Integer)
   end = sql.Column(sql.Integer)
   strand = sql.Column(sql.String)
 
+  levels = sql.Column(sql.BLOB)
   coverage = sql.Column(sql.Float)
   completeness = sql.Column(sql.Float)
   cutoff = sql.Column(sql.Integer)
 
   transcripts = relationship("Transcript", secondary=Exon_Transcript,
                              backref=backref("exons", order_by=start))
```

### Comparing `chanjo-v0.0.3-beta/scripts/chanjo-autopilot.py` & `chanjo-v0.0.4/scripts/chanjo-autopilot.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 # coding: utf-8
 """
 Chanjo.
 Process all or a subset of exons, get coverage from a BAM alignment and
 commit changes to a SQLite database.
 
 Usage:
-  chanjo.py <sql_path> <bam_path> [--ccds=<ccds_path>] [--cutoff=<int>] [--read=<path> | --pipe] [-p | --print]
-  chanjo.py -h | --help
-  chanjo.py --version
+  chanjo-autopilot.py <sql_path> <bam_path> [--ccds=<ccds_path>] [--cutoff=<int>] [--read=<path> | --pipe] [-p | --print]
+  chanjo-autopilot.py -h | --help
+  chanjo-autopilot.py --version
 
 Arguments:
   <sql_path>  path to the SQLite database file
   <bam_path>  path to the BAM alignment file
 
 Options:
   -h --help       Show this screen.
@@ -23,15 +23,14 @@
   --pipe          Read piped list of HGNC symbols.
   -p --print      Just print the input variables to the console
 """
 from __future__ import print_function
 from docopt import docopt
 import time
 import sys
-sys.path.append("/Users/robinandeer/SciLife/modules/chanjo")
 
 import chanjo
 from chanjo import core, sql, bam, ccds2sql
 
 def main(args):
   # Start a timer to be able to print out the runtime
   start = time.time()
```

### Comparing `chanjo-v0.0.3-beta/setup.py` & `chanjo-v0.0.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,13 +19,12 @@
     long_description="",
     install_requires=[
         "nose",
         "pysam",
         "numpy",
         "sqlalchemy",
         "interval",
-        "bx-python",
         "docopt"
     ],
     packages=["chanjo"],
     scripts=["scripts/chanjo-autopilot.py"]
 )
```

