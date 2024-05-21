# Comparing `tmp/corgea_cli-1.3.1.tar.gz` & `tmp/corgea_cli-1.3.2.tar.gz`

## Comparing `corgea_cli-1.3.1.tar` & `corgea_cli-1.3.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      571 1970-01-01 00:00:00.000000 corgea_cli-1.3.1/Cargo.toml
--rw-r--r--   0     1001      127     3285 2024-05-15 22:36:03.000000 corgea_cli-1.3.1/.github/workflows/release.yml
--rw-r--r--   0     1001      127       39 2024-05-15 22:36:03.000000 corgea_cli-1.3.1/.gitignore
--rw-r--r--   0     1001      127    37633 2024-05-15 22:36:03.000000 corgea_cli-1.3.1/Cargo.lock
--rw-r--r--   0     1001      127    26530 2024-05-15 22:36:03.000000 corgea_cli-1.3.1/LICENSE
--rw-r--r--   0     1001      127      780 2024-05-15 22:36:03.000000 corgea_cli-1.3.1/README.md
--rwxr-xr-x   0     1001      127      844 2024-05-15 22:36:03.000000 corgea_cli-1.3.1/build_release.sh
--rw-r--r--   0     1001      127      698 2024-05-15 22:36:03.000000 corgea_cli-1.3.1/src/cicd.rs
--rw-r--r--   0     1001      127     2102 2024-05-15 22:36:03.000000 corgea_cli-1.3.1/src/config.rs
--rw-r--r--   0     1001      127      123 2024-05-15 22:36:03.000000 corgea_cli-1.3.1/src/log.rs
--rw-r--r--   0     1001      127      687 2024-05-15 22:36:03.000000 corgea_cli-1.3.1/src/login.rs
--rw-r--r--   0     1001      127     3222 2024-05-15 22:36:03.000000 corgea_cli-1.3.1/src/main.rs
--rw-r--r--   0     1001      127    14889 2024-05-15 22:36:03.000000 corgea_cli-1.3.1/src/scan.rs
--rw-r--r--   0     1001      127     1109 2024-05-15 22:36:03.000000 corgea_cli-1.3.1/pyproject.toml
--rw-r--r--   0        0        0     1902 1970-01-01 00:00:00.000000 corgea_cli-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0      571 1970-01-01 00:00:00.000000 corgea_cli-1.3.2/Cargo.toml
+-rw-r--r--   0     1001      127     3285 2024-05-21 23:53:53.000000 corgea_cli-1.3.2/.github/workflows/release.yml
+-rw-r--r--   0     1001      127       39 2024-05-21 23:53:53.000000 corgea_cli-1.3.2/.gitignore
+-rw-r--r--   0     1001      127    37633 2024-05-21 23:53:53.000000 corgea_cli-1.3.2/Cargo.lock
+-rw-r--r--   0     1001      127    26530 2024-05-21 23:53:53.000000 corgea_cli-1.3.2/LICENSE
+-rw-r--r--   0     1001      127      780 2024-05-21 23:53:53.000000 corgea_cli-1.3.2/README.md
+-rwxr-xr-x   0     1001      127      844 2024-05-21 23:53:53.000000 corgea_cli-1.3.2/build_release.sh
+-rw-r--r--   0     1001      127      698 2024-05-21 23:53:53.000000 corgea_cli-1.3.2/src/cicd.rs
+-rw-r--r--   0     1001      127     2102 2024-05-21 23:53:53.000000 corgea_cli-1.3.2/src/config.rs
+-rw-r--r--   0     1001      127      123 2024-05-21 23:53:53.000000 corgea_cli-1.3.2/src/log.rs
+-rw-r--r--   0     1001      127      687 2024-05-21 23:53:53.000000 corgea_cli-1.3.2/src/login.rs
+-rw-r--r--   0     1001      127     3222 2024-05-21 23:53:53.000000 corgea_cli-1.3.2/src/main.rs
+-rw-r--r--   0     1001      127    15810 2024-05-21 23:53:53.000000 corgea_cli-1.3.2/src/scan.rs
+-rw-r--r--   0     1001      127     1109 2024-05-21 23:53:53.000000 corgea_cli-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0     1902 1970-01-01 00:00:00.000000 corgea_cli-1.3.2/PKG-INFO
```

### Comparing `corgea_cli-1.3.1/Cargo.toml` & `corgea_cli-1.3.2/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "corgea"
-version = "1.3.1"
+version = "1.3.2"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [dependencies]
 clap = {  version = "4.4.13", features = ["derive"] }
 dirs = "5.0.1"
```

### Comparing `corgea_cli-1.3.1/.github/workflows/release.yml` & `corgea_cli-1.3.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `corgea_cli-1.3.1/Cargo.lock` & `corgea_cli-1.3.2/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -191,15 +191,15 @@
 name = "core-foundation-sys"
 version = "0.8.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "06ea2b9bc92be3c2baa9334a323ebca2d6f074ff852cd1d7b11064035cd3868f"
 
 [[package]]
 name = "corgea"
-version = "1.3.1"
+version = "1.3.2"
 dependencies = [
  "clap",
  "dirs",
  "reqwest",
  "serde",
  "serde_derive",
  "serde_json",
```

### Comparing `corgea_cli-1.3.1/LICENSE` & `corgea_cli-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `corgea_cli-1.3.1/README.md` & `corgea_cli-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `corgea_cli-1.3.1/build_release.sh` & `corgea_cli-1.3.2/build_release.sh`

 * *Files identical despite different names*

### Comparing `corgea_cli-1.3.1/src/cicd.rs` & `corgea_cli-1.3.2/src/cicd.rs`

 * *Files identical despite different names*

### Comparing `corgea_cli-1.3.1/src/config.rs` & `corgea_cli-1.3.2/src/config.rs`

 * *Files identical despite different names*

### Comparing `corgea_cli-1.3.1/src/login.rs` & `corgea_cli-1.3.2/src/login.rs`

 * *Files identical despite different names*

### Comparing `corgea_cli-1.3.1/src/main.rs` & `corgea_cli-1.3.2/src/main.rs`

 * *Files identical despite different names*

### Comparing `corgea_cli-1.3.1/src/scan.rs` & `corgea_cli-1.3.2/src/scan.rs`

 * *Files 3% similar despite different names*

```diff
@@ -140,15 +140,15 @@
                                     }
                                 }
                             }
                         }
                     }
                 }
             // checkmarx report generated by CLI
-            } else if input.contains("Cx") && data.get("results").is_some() && data.get("scanID").is_some() {
+            } else if data.get("totalCount").is_some() && data.get("results").is_some() && data.get("scanID").is_some() {
                 debug("Detected checkmarx cli schema");
                 scanner = "checkmarx".to_string();
                 if let Some(results) = data.get("results").and_then(|v| v.as_array()) {
                     for result in results {
                         if let Some(data) = result.get("data") {
                             if let Some(nodes) = data.get("nodes").and_then(|v| v.as_array()) {
                                 for node in nodes {
@@ -159,15 +159,15 @@
                                     }
                                 }
                             }
                         }
                     }
                 }
             // for checkmarx report generated by web
-            } else if input.contains("Cx") && data.get("scanResults").is_some() && data.get("reportId").is_some() {
+            } else if data.get("scanResults").is_some() && data.get("reportId").is_some() {
                 debug("Detected checkmarx web schema");
                 scanner = "checkmarx".to_string();
                 if let Some(scan_results) = data.get("scanResults") {
                     if let Some(sast) = scan_results.get("sast") {
                         if let Some(languges) = sast.get("languages").and_then(|v| v.as_array()) {
                             for language in languges {
                                 if let Some(queries) = language.get("queries").and_then(|v| v.as_array()) {
@@ -240,14 +240,16 @@
         .timeout(std::time::Duration::from_secs(5 * 60))
         .build()
         .expect("Failed to build client");
 
     println!("Uploading required files for the scan...");
 
     let mut uploaded_paths = HashSet::new();
+    let mut uploaded_count = 0;
+    let mut upload_error_count = 0;
 
     for path in &paths {
         if !Path::new(&path).exists() {
             eprintln!("Required file {} not found which is required for the scan, exiting.", path);
             std::process::exit(1);
         }
 
@@ -257,40 +259,57 @@
 
         let src_upload_url = format!(
             "{}/api/cli/code-upload?token={}&run_id={}&path={}", base_url, token, run_id, path
         );
         debug(&format!("Uploading file: {}", path));
         let fp = Path::new(&path);
 
-        let form = reqwest::blocking::multipart::Form::new()
-            .file("file", fp)
-            .expect("Failed to read file");
-
-
-        debug(&format!("POST: {}", src_upload_url));
-        let res = client.post(&src_upload_url)
-            .multipart(form)
-            .send();
+        let mut attempts = 0;
+        let mut success = false;
 
-        match res {
-            Ok(response) => {
-                if !response.status().is_success() {
-                    eprintln!("Failed to upload file: {}", response.status());
+        while attempts < 3 && !success {
+            let form = reqwest::blocking::multipart::Form::new()
+                .file("file", fp)
+                .expect("Failed to read file");
+
+            debug(&format!("POST: {}", src_upload_url));
+            let res = client.post(&src_upload_url)
+                .multipart(form)
+                .send();
+
+            match res {
+                Ok(response) => {
+                    if !response.status().is_success() {
+                        eprintln!("Failed to upload file {} {}... retrying", response.status(), path);
+                        std::thread::sleep(std::time::Duration::from_secs(1));
+                        upload_error_count = upload_error_count + 1;
+                        attempts += 1;
+                    } else {
+                        uploaded_count += 1;
+                        success = true;
+                        uploaded_paths.insert(path.clone());
+                    }
+                }
+                Err(e) => {
+                    eprintln!("Failed to send request: {}", e);
                     std::process::exit(1);
-                } else {
-                    uploaded_paths.insert(path.clone());
                 }
             }
-            Err(e) => {
-                eprintln!("Failed to send request: {}", e);
-                std::process::exit(1);
-            }
+        }
+
+        if attempts == 3 && !success {
+            eprintln!("Failed to upload file: {} after 3 attempts. skipping...", path);
         }
     }
 
+    if uploaded_count == 0 {
+        eprintln!("Failed to upload any files for the scan, exiting.");
+        std::process::exit(1);
+    }
+
     println!("Uploading the scan...");
 
     // main scan upload
     debug(&format!("POST: {}", scan_upload_url));
     let res = client.post(scan_upload_url)
         .header(header::CONTENT_TYPE, "application/json")
         .body(input.clone())
@@ -367,9 +386,14 @@
         match std::fs::write(&file_path, input.clone()) {
             Ok(_) => println!("Successfully saved scan to {}", file_path.display()),
             Err(e) => eprintln!("Failed to save scan to {}: {}", file_path.display(), e)
         }
     }
 
     println!("Successfully scanned using {} and uploaded to Corgea.", scanner);
+
+    if upload_error_count > 0 {
+        println!("Failed to upload {} files, you may not see all fixes in Corgea.", upload_error_count);
+    }
+
     println!("Go to {base_url} to see results.");
 }
```

### Comparing `corgea_cli-1.3.1/pyproject.toml` & `corgea_cli-1.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `corgea_cli-1.3.1/PKG-INFO` & `corgea_cli-1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: corgea-cli
-Version: 1.3.1
+Version: 1.3.2
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

