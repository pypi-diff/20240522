# Comparing `tmp/static-stig-0.1.8.tar.gz` & `tmp/static-stig-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "static-stig-0.1.8.tar", last modified: Thu Feb 15 21:16:44 2024, max compression
+gzip compressed data, was "static-stig-0.1.9.tar", last modified: Tue Mar 19 20:29:25 2024, max compression
```

## Comparing `static-stig-0.1.8.tar` & `static-stig-0.1.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 21:16:44.395272 static-stig-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-02-15 21:16:44.395272 static-stig-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-02-15 21:16:35.000000 static-stig-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-15 21:16:44.395272 static-stig-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-02-15 21:16:35.000000 static-stig-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 21:16:44.391271 static-stig-0.1.8/static_stig/
--rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-02-15 21:16:35.000000 static-stig-0.1.8/static_stig/stig_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 21:16:44.395272 static-stig-0.1.8/static_stig.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-02-15 21:16:44.000000 static-stig-0.1.8/static_stig.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-02-15 21:16:44.000000 static-stig-0.1.8/static_stig.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-15 21:16:44.000000 static-stig-0.1.8/static_stig.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-02-15 21:16:44.000000 static-stig-0.1.8/static_stig.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-15 21:16:44.000000 static-stig-0.1.8/static_stig.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:29:25.901344 static-stig-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-03-19 20:29:25.901344 static-stig-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-03-19 20:29:12.000000 static-stig-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-19 20:29:25.901344 static-stig-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-03-19 20:29:12.000000 static-stig-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:29:25.901344 static-stig-0.1.9/static_stig/
+-rw-r--r--   0 runner    (1001) docker     (127)     3585 2024-03-19 20:29:12.000000 static-stig-0.1.9/static_stig/stig_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 20:29:25.901344 static-stig-0.1.9/static_stig.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-03-19 20:29:25.000000 static-stig-0.1.9/static_stig.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-03-19 20:29:25.000000 static-stig-0.1.9/static_stig.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 20:29:25.000000 static-stig-0.1.9/static_stig.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-19 20:29:25.000000 static-stig-0.1.9/static_stig.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-19 20:29:25.000000 static-stig-0.1.9/static_stig.egg-info/top_level.txt
```

### Comparing `static-stig-0.1.8/PKG-INFO` & `static-stig-0.1.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: static-stig
-Version: 0.1.8
+Version: 0.1.9
 Description-Content-Type: text/markdown
 
 # Static STIG
 
 ## Overview
 
 This tool allows users to run OSCAP STIGs against a static image instead of waiting to do so at runtime. It will pull the image and determine its base distro and run a standard STIG profile against the image before outputting the results to a file on your local machine.
 
 ## Requirements
 
 Static STIG requires docker to run. Ensure that Docker is installed and your user is a part of the Docker group so the use of sudo isn't required to run docker commands. Additionally, ensure that your user owns the directory you are running Static STIG in.
 
 ## How to Run
 
-Run `pip install -U .` in the cli directory.
+Run `pip install -U static-stig`
 
 To run Static STIG, simply run package and give it the desired target image: `static-stig -i registry_url/repo/image:tag`
 
 For exammple, to run a stig against the latest ubuntu image run `static-stig -i docker.io/library/ubuntu:latest`
 
 To run a STIG against an image in a private repository, run the same command with the credential flags: `static-stig -i registry_url/repo/image:tag -u username -p password -r registry_url`
```

### Comparing `static-stig-0.1.8/README.md` & `static-stig-0.1.9/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 ## Requirements
 
 Static STIG requires docker to run. Ensure that Docker is installed and your user is a part of the Docker group so the use of sudo isn't required to run docker commands. Additionally, ensure that your user owns the directory you are running Static STIG in.
 
 ## How to Run
 
-Run `pip install -U .` in the cli directory.
+Run `pip install -U static-stig`
 
 To run Static STIG, simply run package and give it the desired target image: `static-stig -i registry_url/repo/image:tag`
 
 For exammple, to run a stig against the latest ubuntu image run `static-stig -i docker.io/library/ubuntu:latest`
 
 To run a STIG against an image in a private repository, run the same command with the credential flags: `static-stig -i registry_url/repo/image:tag -u username -p password -r registry_url`
```

### Comparing `static-stig-0.1.8/static_stig/stig_runner.py` & `static-stig-0.1.9/static_stig/stig_runner.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,34 +38,34 @@
 
     signal.signal(signal.SIGINT, cleanup_volume)
 
     if args.local:
         print("Detected local image. Running in local mode.")
         subprocess.run(["docker", "save", args.image, "-o", "./local-image.tar.gz"])
         subprocess.run(["docker", "run", "-t", "--rm", "--privileged",
-                        "-e", f"SCAN_IMAGE=localhost/{args.image}",
+                        "-e", f"SCAN_IMAGE={args.image}",
                         "-e", f"INSECURE_REG={args.insecure}",
                         "--name", "stig-runner",
                         "-v", f"{os.getcwd()}/local-image.tar.gz:/etc/local-image.tar.gz:ro",
                         "-v", f"{os.getcwd()}/stig-results/{dir_name}:/tmp",
-                        "anchore/static-stig:0.1.8"])
+                        "anchore/static-stig:0.1.9"])
         os.remove("local-image.tar.gz")
     elif not args.username:
         subprocess.run(["docker", "run", "-t", "--rm", "--privileged",
                         "-e", f"SCAN_IMAGE={args.image}",
                         "-e", f"INSECURE_REG={args.insecure}",
                         "--name", "stig-runner",
                         "-v", f"{os.getcwd()}/stig-results/{dir_name}:/tmp",
-                        "anchore/static-stig:0.1.8"])
+                        "anchore/static-stig:0.1.9"])
     else:
         subprocess.run(["docker", "run", "-t", "--rm", "--privileged",
                         "-e", f"SCAN_IMAGE={args.image}",
                         "-e", f"INSECURE_REG={args.insecure}",
                         "-e", f"REGISTRY_USERNAME={args.username}",
                         "-e", f"REGISTRY_PASSWORD={args.password}",
                         "-e", f"REGISTRY_URL={args.url}",
                         "--name", "stig-runner",
                         "-v", f"{os.getcwd()}/stig-results/{dir_name}:/tmp",
-                        "anchore/static-stig:0.1.8"])
+                        "anchore/static-stig:0.1.9"])
 
 if __name__ == "__main__":
     main()
```

### Comparing `static-stig-0.1.8/static_stig.egg-info/PKG-INFO` & `static-stig-0.1.9/static_stig.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: static-stig
-Version: 0.1.8
+Version: 0.1.9
 Description-Content-Type: text/markdown
 
 # Static STIG
 
 ## Overview
 
 This tool allows users to run OSCAP STIGs against a static image instead of waiting to do so at runtime. It will pull the image and determine its base distro and run a standard STIG profile against the image before outputting the results to a file on your local machine.
 
 ## Requirements
 
 Static STIG requires docker to run. Ensure that Docker is installed and your user is a part of the Docker group so the use of sudo isn't required to run docker commands. Additionally, ensure that your user owns the directory you are running Static STIG in.
 
 ## How to Run
 
-Run `pip install -U .` in the cli directory.
+Run `pip install -U static-stig`
 
 To run Static STIG, simply run package and give it the desired target image: `static-stig -i registry_url/repo/image:tag`
 
 For exammple, to run a stig against the latest ubuntu image run `static-stig -i docker.io/library/ubuntu:latest`
 
 To run a STIG against an image in a private repository, run the same command with the credential flags: `static-stig -i registry_url/repo/image:tag -u username -p password -r registry_url`
```

