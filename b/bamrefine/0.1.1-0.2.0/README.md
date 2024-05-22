# Comparing `tmp/bamrefine-0.1.1.tar.gz` & `tmp/bamrefine-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bamrefine-0.1.1.tar", last modified: Mon Nov 13 18:13:10 2023, max compression
+gzip compressed data, was "bamrefine-0.2.0.tar", last modified: Wed May 22 11:40:58 2024, max compression
```

## Comparing `bamrefine-0.1.1.tar` & `bamrefine-0.2.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 etka       (501) staff       (20)        0 2023-11-13 18:13:10.532441 bamrefine-0.1.1/
--rw-r--r--   0 etka       (501) staff       (20)     1518 2023-11-13 17:30:46.000000 bamrefine-0.1.1/LICENSE
--rw-r--r--   0 etka       (501) staff       (20)     7595 2023-11-13 18:13:10.532244 bamrefine-0.1.1/PKG-INFO
--rw-r--r--   0 etka       (501) staff       (20)     7020 2023-11-13 18:05:43.000000 bamrefine-0.1.1/README.md
--rw-r--r--   0 etka       (501) staff       (20)      899 2023-11-13 17:41:40.000000 bamrefine-0.1.1/pyproject.toml
--rw-r--r--   0 etka       (501) staff       (20)       38 2023-11-13 18:13:10.532482 bamrefine-0.1.1/setup.cfg
-drwxr-xr-x   0 etka       (501) staff       (20)        0 2023-11-13 18:13:10.529488 bamrefine-0.1.1/src/
-drwxr-xr-x   0 etka       (501) staff       (20)        0 2023-11-13 18:13:10.530419 bamrefine-0.1.1/src/bamRefine/
--rw-r--r--   0 etka       (501) staff       (20)        0 2023-11-13 17:30:46.000000 bamrefine-0.1.1/src/bamRefine/__init__.py
--rwxr-xr-x   0 etka       (501) staff       (20)     8695 2023-11-13 17:30:46.000000 bamrefine-0.1.1/src/bamRefine/__main__.py
--rw-r--r--   0 etka       (501) staff       (20)     7232 2023-11-13 17:30:46.000000 bamrefine-0.1.1/src/bamRefine/functions.py
-drwxr-xr-x   0 etka       (501) staff       (20)        0 2023-11-13 18:13:10.529356 bamrefine-0.1.1/src/bamRefine/man/
-drwxr-xr-x   0 etka       (501) staff       (20)        0 2023-11-13 18:13:10.530657 bamrefine-0.1.1/src/bamRefine/man/man1/
--rw-r--r--   0 etka       (501) staff       (20)     2649 2023-11-13 17:30:46.000000 bamrefine-0.1.1/src/bamRefine/man/man1/bamrefine.1
-drwxr-xr-x   0 etka       (501) staff       (20)        0 2023-11-13 18:13:10.531138 bamrefine-0.1.1/src/bamRefine/sample_data/
--rw-r--r--   0 etka       (501) staff       (20)      780 2023-11-13 17:30:46.000000 bamrefine-0.1.1/src/bamRefine/sample_data/omitColumn_sampleSNPs.bed
--rw-r--r--   0 etka       (501) staff       (20)     1236 2023-11-13 17:30:46.000000 bamrefine-0.1.1/src/bamRefine/sample_data/sampleSNPs.bed
--rw-r--r--   0 etka       (501) staff       (20)     1790 2023-11-13 17:30:46.000000 bamrefine-0.1.1/src/bamRefine/sample_data/sampleSNPs.snp
-drwxr-xr-x   0 etka       (501) staff       (20)        0 2023-11-13 18:13:10.531866 bamrefine-0.1.1/src/bamrefine.egg-info/
--rw-r--r--   0 etka       (501) staff       (20)     7595 2023-11-13 18:13:10.000000 bamrefine-0.1.1/src/bamrefine.egg-info/PKG-INFO
--rw-r--r--   0 etka       (501) staff       (20)      528 2023-11-13 18:13:10.000000 bamrefine-0.1.1/src/bamrefine.egg-info/SOURCES.txt
--rw-r--r--   0 etka       (501) staff       (20)        1 2023-11-13 18:13:10.000000 bamrefine-0.1.1/src/bamrefine.egg-info/dependency_links.txt
--rw-r--r--   0 etka       (501) staff       (20)      135 2023-11-13 18:13:10.000000 bamrefine-0.1.1/src/bamrefine.egg-info/entry_points.txt
--rw-r--r--   0 etka       (501) staff       (20)       14 2023-11-13 18:13:10.000000 bamrefine-0.1.1/src/bamrefine.egg-info/requires.txt
--rw-r--r--   0 etka       (501) staff       (20)       10 2023-11-13 18:13:10.000000 bamrefine-0.1.1/src/bamrefine.egg-info/top_level.txt
-drwxr-xr-x   0 etka       (501) staff       (20)        0 2023-11-13 18:13:10.532009 bamrefine-0.1.1/tests/
--rw-r--r--   0 etka       (501) staff       (20)     1361 2023-11-13 17:30:46.000000 bamrefine-0.1.1/tests/test_flagReads.py
+drwxrwxr-x   0 etka      (1001) etka      (1001)        0 2024-05-22 11:40:58.241428 bamrefine-0.2.0/
+-rw-r--r--   0 etka      (1001) etka      (1001)     1518 2024-03-17 17:38:21.000000 bamrefine-0.2.0/LICENSE
+-rw-r--r--   0 etka      (1001) etka      (1001)     7928 2024-05-22 11:40:58.241428 bamrefine-0.2.0/PKG-INFO
+-rw-rw-r--   0 etka      (1001) etka      (1001)     7353 2024-05-22 11:30:23.000000 bamrefine-0.2.0/README.md
+-rw-rw-r--   0 etka      (1001) etka      (1001)      899 2024-05-22 11:30:23.000000 bamrefine-0.2.0/pyproject.toml
+-rw-rw-r--   0 etka      (1001) etka      (1001)       38 2024-05-22 11:40:58.241428 bamrefine-0.2.0/setup.cfg
+drwxrwxr-x   0 etka      (1001) etka      (1001)        0 2024-05-22 11:40:58.237428 bamrefine-0.2.0/src/
+drwxrwxr-x   0 etka      (1001) etka      (1001)        0 2024-05-22 11:40:58.237428 bamrefine-0.2.0/src/bamRefine/
+-rw-r--r--   0 etka      (1001) etka      (1001)        0 2024-03-17 17:38:25.000000 bamrefine-0.2.0/src/bamRefine/__init__.py
+-rwxrwxr-x   0 etka      (1001) etka      (1001)     8874 2024-05-16 20:48:36.000000 bamrefine-0.2.0/src/bamRefine/__main__.py
+-rw-rw-r--   0 etka      (1001) etka      (1001)    10542 2024-05-16 20:48:36.000000 bamrefine-0.2.0/src/bamRefine/functions.py
+drwxrwxr-x   0 etka      (1001) etka      (1001)        0 2024-05-22 11:40:58.237428 bamrefine-0.2.0/src/bamRefine/man/
+drwxrwxr-x   0 etka      (1001) etka      (1001)        0 2024-05-22 11:40:58.237428 bamrefine-0.2.0/src/bamRefine/man/man1/
+-rw-rw-r--   0 etka      (1001) etka      (1001)     3450 2024-05-16 20:48:36.000000 bamrefine-0.2.0/src/bamRefine/man/man1/bamrefine.1
+drwxrwxr-x   0 etka      (1001) etka      (1001)        0 2024-05-22 11:40:58.241428 bamrefine-0.2.0/src/bamRefine/sample_data/
+-rw-r--r--   0 etka      (1001) etka      (1001)      780 2024-03-17 17:38:25.000000 bamrefine-0.2.0/src/bamRefine/sample_data/omitColumn_sampleSNPs.bed
+-rw-r--r--   0 etka      (1001) etka      (1001)     1236 2024-03-17 17:38:25.000000 bamrefine-0.2.0/src/bamRefine/sample_data/sampleSNPs.bed
+-rw-r--r--   0 etka      (1001) etka      (1001)     1790 2024-03-17 17:38:25.000000 bamrefine-0.2.0/src/bamRefine/sample_data/sampleSNPs.snp
+drwxrwxr-x   0 etka      (1001) etka      (1001)        0 2024-05-22 11:40:58.241428 bamrefine-0.2.0/src/bamrefine.egg-info/
+-rw-r--r--   0 etka      (1001) etka      (1001)     7928 2024-05-22 11:40:58.000000 bamrefine-0.2.0/src/bamrefine.egg-info/PKG-INFO
+-rw-r--r--   0 etka      (1001) etka      (1001)      528 2024-05-22 11:40:58.000000 bamrefine-0.2.0/src/bamrefine.egg-info/SOURCES.txt
+-rw-r--r--   0 etka      (1001) etka      (1001)        1 2024-05-22 11:40:58.000000 bamrefine-0.2.0/src/bamrefine.egg-info/dependency_links.txt
+-rw-r--r--   0 etka      (1001) etka      (1001)      135 2024-05-22 11:40:58.000000 bamrefine-0.2.0/src/bamrefine.egg-info/entry_points.txt
+-rw-r--r--   0 etka      (1001) etka      (1001)       14 2024-05-22 11:40:58.000000 bamrefine-0.2.0/src/bamrefine.egg-info/requires.txt
+-rw-r--r--   0 etka      (1001) etka      (1001)       10 2024-05-22 11:40:58.000000 bamrefine-0.2.0/src/bamrefine.egg-info/top_level.txt
+drwxrwxr-x   0 etka      (1001) etka      (1001)        0 2024-05-22 11:40:58.241428 bamrefine-0.2.0/tests/
+-rw-rw-r--   0 etka      (1001) etka      (1001)     2427 2024-05-16 20:48:36.000000 bamrefine-0.2.0/tests/test_flagReads.py
```

### Comparing `bamrefine-0.1.1/LICENSE` & `bamrefine-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bamrefine-0.1.1/PKG-INFO` & `bamrefine-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bamrefine
-Version: 0.1.1
+Version: 0.2.0
 Summary: A small program to mask positions that could result in a PMD artifact from a BAM file using a predefined SNP catalog
 Author-email: Etka Yapar <etka.yapar@gmail.com>
 Project-URL: Homepage, https://github.com/etkayapar/bamRefine
 Project-URL: Bug Tracker, https://github.com/etkayapar/bamRefine/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Requires-Python: >=3.6
@@ -147,14 +147,18 @@
   risk of seeing a PMD artifact) regarding your libraries before you run this program on the BAM files 
   because the `--pmd-length-threshold` parameter requires an user specified value for the program to run, 
   there is no default value. This can be achieved by using [PMDtools](https://github.com/pontussk/PMDtools)
 
 
 ### Flags:
 
+  * `-S, --single-stranded`: Run the program in single-stranded mode. This flag should be 
+    turned on for BAM files that are generated from single-stranded libraries. When turned 
+    on, C/* variants are considered for overlapping read positions at both 5' and 3' ends.
+    (Instead of using C/* for 5' ends and G/* for 3' ends)
   * `-v, --verbose`: verbose output of progress.
   * `-t, --add-tags`: Add tags to reads in output BAM file related to masking statistics 
     using optional SAM fields in alignment records. e.g. `ZC:Z:2,1`  and `ZP:Z:0,5;-3` 
     would mean that the program masked n=2 5' and n=1 3' positions and they were at index 
     0,5 and -3 in the read sequence. 3' masking positions are represented with negative 
 	indices that start counting from the 3' end of the read and is compatible with python 
 	list indices.
```

### Comparing `bamrefine-0.1.1/README.md` & `bamrefine-0.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -133,14 +133,18 @@
   risk of seeing a PMD artifact) regarding your libraries before you run this program on the BAM files 
   because the `--pmd-length-threshold` parameter requires an user specified value for the program to run, 
   there is no default value. This can be achieved by using [PMDtools](https://github.com/pontussk/PMDtools)
 
 
 ### Flags:
 
+  * `-S, --single-stranded`: Run the program in single-stranded mode. This flag should be 
+    turned on for BAM files that are generated from single-stranded libraries. When turned 
+    on, C/* variants are considered for overlapping read positions at both 5' and 3' ends.
+    (Instead of using C/* for 5' ends and G/* for 3' ends)
   * `-v, --verbose`: verbose output of progress.
   * `-t, --add-tags`: Add tags to reads in output BAM file related to masking statistics 
     using optional SAM fields in alignment records. e.g. `ZC:Z:2,1`  and `ZP:Z:0,5;-3` 
     would mean that the program masked n=2 5' and n=1 3' positions and they were at index 
     0,5 and -3 in the read sequence. 3' masking positions are represented with negative 
 	indices that start counting from the 3' end of the read and is compatible with python 
 	list indices.
```

### Comparing `bamrefine-0.1.1/pyproject.toml` & `bamrefine-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bamrefine"
-version = "0.1.1"
+version = "0.2.0"
 authors = [
 	{name="Etka Yapar", email="etka.yapar@gmail.com"},
 ]
 description = "A small program to mask positions that could result in a PMD artifact from a BAM file using a predefined SNP catalog"
 readme = "README.md"
 requires-python = ">=3.6"
 dependencies = [
```

### Comparing `bamrefine-0.1.1/src/bamRefine/__main__.py` & `bamrefine-0.2.0/src/bamRefine/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 Usage: bamrefine [options] <in.bam> <out.bam>
 
 OPTIONS:
         -s, --snps                    <FILE> BED  or SNP formatted file for snps
         -p, --threads                 <INT> # of threads to use
         -l, --pmd-length-threshold    <INT|INT,INT> pmd length threshold
 FLAGS:
+        -S, --single-stranded         run the program in single-stranded mode
         -t, --add-tags                add maskings stats as optional SAM fields to the alignments
         -v, --verbose                 verbose output of progress
         -k, --keep-tmp                don't remove the temporary directory (.YYYY-MM-DD_HH-MM-SS_<out.bam>_tmp_bamrefine)
         -h, --help                    display this message end exit
 
 
     '''
@@ -34,43 +35,43 @@
     helpmsg = '''
 Consider reading the man page. You can do so by running the command: bamrefine_man
 '''
 
     if help:
         msg = helpmsg + msg
 
-    print(msg)
+    print(msg, file=sys.stderr)
     sys.exit()
 
 
 def waitJobs(runningJobs):
     while len([i for i in runningJobs if i.poll() != None]) < len(runningJobs):
         continue
 
 
 def man(args=None):
     data_path = os.path.join(os.path.dirname(__file__), 'man', 'man1','bamrefine.1')
     os.system(f"man {data_path}")
-    
+
 
 def main(args=None):
-    def parallelParse(jobL, n, lookup):
+    def parallelParse(jobL, n, lookup, env):
         activeJobs = []
         jobN = []
 
         for i in range(n):
             try:
                 c = jobL.pop()
             except IndexError:
                 waitJobs(activeJobs)
                 return None
 
-            cmdList = ["bamrefine_proc", inName,c, lookup, snpF, str(int(addTags))]
+            cmdList = ["bamrefine_proc", inName,c, lookup, snpF, str(int(addTags)), str(int(singleStranded))]
             cmd = " ".join(cmdList)
-            p = Popen([cmd], shell = True)
+            p = Popen([cmd], shell = True, env=env)
             activeJobs.append(p)
             jobN.append(c)
             if verbose:
                 print('Started job for chr%s' % c)
 
         while True:
             time.sleep(3)
@@ -82,51 +83,53 @@
             if n_f > 0:
                 for i in finished:
                     if verbose:
                         print("Finished job for chr%s" % jobN[i])
                     if len(jobL) == 0:
                         continue
                     c = jobL.pop()
-                    cmdList = ["bamrefine_proc", inName,c, lookup, snpF,str(int(addTags))]
+                    cmdList = ["bamrefine_proc", inName,c, lookup, snpF,str(int(addTags)), str(int(singleStranded))]
                     cmd = " ".join(cmdList)
-                    p = Popen([cmd], shell = True)
+                    p = Popen([cmd], shell = True, env=env)
                     if verbose:
                         print("Started job for chr%s" % c)
                     activeJobs[i] = p
                     jobN[i] = c
 
         waitJobs(activeJobs)
-    
+
     dirN = os.path.dirname(os.path.realpath(__file__))#dirname of the script
     # Processing command-line options for the program ------------------
 
     ## default args
     chrmFname = None
     genomeF = None
     thread = None
     inName = None
     ouName = None
     lookup = None
+    singleStranded = False
     verbose = False
     snpF = None
     addTags = False
     keeptmp = False
 
     nOptions=0
 
     try:
         options, remainder = getopt.gnu_getopt(sys.argv[1:],
-                                            's:p:l:tvhk',
-                                            ['snps=',
-                                            'threads=',
+                                            's:p:l:Stvhk',
+                                               ['snps=',
+                                                'threads=',
                                                 'pmd-length-threshold=',
+                                                'single-stranded',
                                                 'add-tags',
-                                            'verbose',
+                                                'verbose',
                                                 'help',
-                                            'keep-tmp'])
+                                                'keep-tmp'])
     except getopt.GetoptError as err:
         print(str(err))
         usage()
 
 
     for opt, arg in options:
         if opt in ('-p', '--threads'):
@@ -134,14 +137,16 @@
             nOptions += 1
         elif opt in ('-s', '--snps'):
             snpF = arg
             nOptions += 1
         elif opt in ('-l', '--pmd-length-threshold'):
             lookup = arg
             nOptions += 1
+        elif opt in ('-S', '--single-stranded'):
+            singleStranded = True
         elif opt in ('-t', '--add-tags'):
             addTags = True
         elif opt in ('-v', '--verbose'):
             verbose = True
         elif opt in ('-k', '--keep-tmp'):
             keeptmp = True
         elif opt in ('-h', '--help'):
@@ -150,28 +155,21 @@
             usage()
 
 
     if nOptions != 3:
         print("All options need arguments")
         usage()
 
-    if remainder[0].startswith('/'):
-        inName = remainder[0]
-    else:
-        inName = './'+remainder[0]
-
-    if remainder[1].startswith('/'):
-        ouName = remainder[1]
-    else:
-        ouName = './'+remainder[1]
+    if len(remainder) < 2:
+        msg = "At least two positional arguments are needed: <in.bam> <out.bam>"
+        print(msg, file=sys.stderr)
+        usage()
 
-    if snpF.startswith('/'):
-        pass
-    else:
-        snpF = './'+snpF
+    inName = remainder[0]
+    ouName = remainder[1]
 
     inName  = os.path.abspath(inName)
     ouName  = os.path.abspath(ouName)
     snpF    = os.path.abspath(snpF)
     ouDir   = os.path.dirname(ouName)
 
     lookup = lookup.split(",")
@@ -222,18 +220,21 @@
         shutil.rmtree(tmpname)
         os.mkdir(tmpname)
 
 
     print('\nStarted bam filtering\n')
     os.chdir(tmpname)
 
-    jobs, bypass = bamRefine.createBypassBED(inName, chrms, snpF)
+    jobs, bypass = bamRefine.createBypassBED(inName, chrms, snpF, singleStranded)
     jobs_c = jobs.copy()
 
-    parallelParse(jobs, thread, lookup)
+    env = os.environ.copy()
+    env["BAMREFINE_CMDLINE"] = " ".join(sys.argv)
+
+    parallelParse(jobs, thread, lookup, env)
 
     print("Finished BAM filtering\n\nMerging BAM files...")
 
 
 
     ## samtools merge commands -------------
     with open('toMerge_bamlist.txt', 'w') as f:
@@ -246,20 +247,14 @@
     ### ----------------------
 
     if bypass:
         pysam.view("-@", str(thread), "--no-PG", "-L", "bypass.bed", "-b", "-o" "bypassed.bam", inName, catch_stdout=False) ##pysam bug
 
     pysam.merge("--no-PG", "-c", "-p", "-b" , toMergeF, "-O", "BAM", "-@", str(thread), ouName)
 
-    # pysam.view("-H", "-o", "header.sam", inName, catch_stdout=False)
-    # pysam.reheader("-P",  "-i", "header.sam", ouName)
-
-    # while reheading.poll() == None:
-    #     continue
-
     print("Finished merging.")
 
     ### -----------------------------------
 
     ## Wrapping up stats -----------------
     stats = []
     for statFile in glob.glob('./*_stats.txt'):
```

### Comparing `bamrefine-0.1.1/src/bamRefine/man/man1/bamrefine.1` & `bamrefine-0.2.0/src/bamRefine/man/man1/bamrefine.1`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 .TH bamrefine 1 "January  7, 2023"
 .SH NAME
 bamrefine \- Mask SNPs from a BAM file
 .SH SYNOPSIS
-\fB bamrefine \fP [OPTIONS][-vtkh] <in.bam> <out.bam>
+\fB bamrefine \fP [OPTIONS][-Svtkh] <in.bam> <out.bam>
 .SH DESCRIPTION
 \fBbamrefine\fP processes a BAM file to mask the positions from an
 alignment if that read carries a variant position that could be affected
 by post-mortem damage (PMD). e.g. If a read carries a C/* position at its
 5' end or it carries a G/* position at its 3' end. The regions treated as 5'
-or 3' "end" is not pre-defined and should be provided to the program with its
-argument (see \fB-l\fP)
+or 3' "ends" are not pre-defined and should be provided to the program with the
+corresponding option (see \fB-l\fP)
 .SS OPTIONS
 .TP
 \fB-s, --snps\fP
 Path to BED or SNP formatted file for SNP positions and minor and
 major alleles. This can be either 4/5 column BED (genomic position
 [with or without the `start` position column] + Minor and Major allele)
 or SNP (that is used by EIGENSTRAT) formatted files. Format distinction is done by
@@ -25,26 +25,37 @@
 \fBpip3 show bamrefine\fP
 
 or
 
 \fBpip show bamrefine\fP
 .TP
 \fB-p, --threads\fP
-Number of threads to run the program in parallel.
+Number of threads to run the program in parallel. Parallelization is done by multiprocessing
+over the available contigs in the input BAM file, therefore the total number of threads that
+can be used effectively by the program has an upper limit. There is probably no real advantage
+in passing absurdly high numbers for this option for a single run, over simultaneously running
+the program with multiple different input files (e.g. independent invocations with xargs or
+similar) by using 4/8 threads per input file.
 .TP
 .TP
 \fB-l, --pmd-length-threshold\fP
 PMD length threshold. Either a single integer (e.g \fB-l 10\fP) or two integers separated
 by a comma (e.g \fB-l 2,0\fP) representing different length values corresponding 5' and 3'
 ends, respectively. Positions that are up to and including this far in any read
 will be evaluated and masked. There is no one-for-all default value that can be set,
 so it is highly recommended that you have a prior information about the PMD profiles
 of your libraries before you run \fBbamrefine\fP
 .SS FLAGS
 .TP
+\fB-S, --single-stranded\fP
+Run the program in single-stranded mode. This flag should be turned on for BAM files that
+are generated from single-stranded libraries. When turned on, C/* variants are considered
+for overlapping read positions at both 5' and 3' ends. (Instead of using C/* for 5' ends
+and G/* for 3' ends)
+.TP
 \fB-v, --verbose\fP
 Verbose output of progress
 .TP
 \fB-t, --add-tags\fP
 Add tags to output BAM file related to masking statistics using optional fields in alignment
 records. e.g. ZC:Z:2,1 ZP:Z:0,5;-3 would mean that the program masked n=2 5' and n=1 3' positions
 and they were at index 0,5 and -3 in the sequence. 3' masking positions are represented with
```

### Comparing `bamrefine-0.1.1/src/bamRefine/sample_data/omitColumn_sampleSNPs.bed` & `bamrefine-0.2.0/src/bamRefine/sample_data/omitColumn_sampleSNPs.bed`

 * *Files identical despite different names*

### Comparing `bamrefine-0.1.1/src/bamRefine/sample_data/sampleSNPs.bed` & `bamrefine-0.2.0/src/bamRefine/sample_data/sampleSNPs.bed`

 * *Files identical despite different names*

### Comparing `bamrefine-0.1.1/src/bamRefine/sample_data/sampleSNPs.snp` & `bamrefine-0.2.0/src/bamRefine/sample_data/sampleSNPs.snp`

 * *Files identical despite different names*

### Comparing `bamrefine-0.1.1/src/bamrefine.egg-info/PKG-INFO` & `bamrefine-0.2.0/src/bamrefine.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bamrefine
-Version: 0.1.1
+Version: 0.2.0
 Summary: A small program to mask positions that could result in a PMD artifact from a BAM file using a predefined SNP catalog
 Author-email: Etka Yapar <etka.yapar@gmail.com>
 Project-URL: Homepage, https://github.com/etkayapar/bamRefine
 Project-URL: Bug Tracker, https://github.com/etkayapar/bamRefine/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Requires-Python: >=3.6
@@ -147,14 +147,18 @@
   risk of seeing a PMD artifact) regarding your libraries before you run this program on the BAM files 
   because the `--pmd-length-threshold` parameter requires an user specified value for the program to run, 
   there is no default value. This can be achieved by using [PMDtools](https://github.com/pontussk/PMDtools)
 
 
 ### Flags:
 
+  * `-S, --single-stranded`: Run the program in single-stranded mode. This flag should be 
+    turned on for BAM files that are generated from single-stranded libraries. When turned 
+    on, C/* variants are considered for overlapping read positions at both 5' and 3' ends.
+    (Instead of using C/* for 5' ends and G/* for 3' ends)
   * `-v, --verbose`: verbose output of progress.
   * `-t, --add-tags`: Add tags to reads in output BAM file related to masking statistics 
     using optional SAM fields in alignment records. e.g. `ZC:Z:2,1`  and `ZP:Z:0,5;-3` 
     would mean that the program masked n=2 5' and n=1 3' positions and they were at index 
     0,5 and -3 in the read sequence. 3' masking positions are represented with negative 
 	indices that start counting from the 3' end of the read and is compatible with python 
 	list indices.
```

### Comparing `bamrefine-0.1.1/src/bamrefine.egg-info/SOURCES.txt` & `bamrefine-0.2.0/src/bamrefine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bamrefine-0.1.1/tests/test_flagReads.py` & `bamrefine-0.2.0/tests/test_flagReads.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,54 +1,84 @@
 from bamRefine.functions import *
-#import os
+import os
 
 dirN = os.path.dirname(os.path.realpath(__file__))
 os.chdir(dirN)
 
 
 
-snps = "random_reads.snp"
-snps = handleSNPs(snps)
 lookup_l = 10
 lookup_r = 10
 
+### Double-stranded mode (default) -------------------------
+snps_ds = "random_reads.snp"
+snps_ds = parseSNPs(snps_ds, False)
 def test_flagReads_complex():
     inName = "complex_read.sam"
     inBAM = pysam.AlignmentFile(inName, 'rb')
     for read in inBAM.fetch():
         bamL = read.to_dict()
-        mask, m_pos, m_side = flagReads(snps, bamL, lookup_l, lookup_r, read)
+        mask, m_pos, m_side = flagReads(snps_ds, bamL, lookup_l, lookup_r, read)
 
         assert mask == "mask" 
         assert m_pos == [1,5,8,-9]
         assert m_side == [0,0,0,1]
     inBAM.close()
 
 def test_flagReads_complex_asymmetric():
     inName = "complex_read.sam"
     inBAM = pysam.AlignmentFile(inName, 'rb')
     for read in inBAM.fetch():
         bamL = read.to_dict()
-        mask, m_pos, m_side = flagReads(snps, bamL, 10, 8, read)
+        mask, m_pos, m_side = flagReads(snps_ds, bamL, 10, 8, read)
 
         assert mask == "mask" 
         assert m_pos == [1,5,8]
         assert m_side == [0,0,0]
     inBAM.close()
 
 def test_flagReads_short():
     inName = "short_read.sam"
     inBAM = pysam.AlignmentFile(inName, 'rb')
     for read in inBAM.fetch():
         bamL = read.to_dict()
-        mask, m_pos, m_side = flagReads(snps, bamL, lookup_l, lookup_r, read)
+        mask, m_pos, m_side = flagReads(snps_ds, bamL, lookup_l, lookup_r, read)
         print(m_pos)
         print(m_side)
-        print(snps)
+        print(snps_ds)
 
         assert mask == "mask" 
         assert m_pos == [0,1,5,-2,-5]
         assert m_side == [0,0,0,1,1]
     inBAM.close()
+## ---------------------------------------------------
 
+## single-stranded mode
+snps_ss = "random_reads_ss.snp"
+snps_ss = parseSNPs(snps_ss, singleStranded=True)
 
-    
+def test_flagReads_complex_single():
+    inName = "complex_read.sam"
+    inBAM = pysam.AlignmentFile(inName, 'rb')
+    for read in inBAM.fetch():
+        bamL = read.to_dict()
+        mask, m_pos, m_side = flagReads(snps_ss, bamL, lookup_l, lookup_r, read)
+
+        assert mask == "mask" 
+        assert m_pos == [1,5,8]
+        assert m_side == [0,0,0]
+    inBAM.close()
+
+def test_flagReads_short_single():
+    inName = "short_read.sam"
+    inBAM = pysam.AlignmentFile(inName, 'rb')
+    for read in inBAM.fetch():
+        bamL = read.to_dict()
+        mask, m_pos, m_side = flagReads(snps_ss, bamL, lookup_l, lookup_r, read)
+        print(m_pos)
+        print(m_side)
+        print(snps_ds)
+
+        assert mask == "mask" 
+        assert m_pos == [0,1,5,-5,-9,-10]
+        assert m_side == [0,0,0,1,1,1]
+    inBAM.close()
```

