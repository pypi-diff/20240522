# Comparing `tmp/genimtools-0.0.8.tar.gz` & `tmp/genimtools-0.0.9.tar.gz`

## Comparing `genimtools-0.0.8.tar` & `genimtools-0.0.9.tar`

### file list

```diff
@@ -1,59 +1,68 @@
--rw-r--r--   0     1001      127      561 2024-01-17 19:17:43.000000 genimtools-0.0.8/genimtools/Cargo.toml
--rw-r--r--   0     1001      127     1382 2024-01-17 19:17:43.000000 genimtools-0.0.8/genimtools/docs/changelog.md
--rw-r--r--   0     1001      127    64540 2024-01-17 19:17:43.000000 genimtools-0.0.8/genimtools/docs/logo.svg
--rw-r--r--   0     1001      127     4823 2024-01-17 19:17:43.000000 genimtools-0.0.8/genimtools/src/ailist/mod.rs
--rw-r--r--   0     1001      127      371 2024-01-17 19:17:43.000000 genimtools-0.0.8/genimtools/src/common/consts.rs
--rw-r--r--   0     1001      127       47 2024-01-17 19:17:43.000000 genimtools-0.0.8/genimtools/src/common/mod.rs
--rw-r--r--   0     1001      127      310 2024-01-17 19:17:43.000000 genimtools-0.0.8/genimtools/src/common/models/bed_set.rs
--rw-r--r--   0     1001      127      396 2024-01-17 19:17:43.000000 genimtools-0.0.8/genimtools/src/common/models/mod.rs
--rw-r--r--   0     1001      127      305 2024-01-17 19:17:43.000000 genimtools-0.0.8/genimtools/src/common/models/region.rs
--rw-r--r--   0     1001      127     2812 2024-01-17 19:17:43.000000 genimtools-0.0.8/genimtools/src/common/models/region_set.rs
--rw-r--r--   0     1001      127      107 2024-01-17 19:17:43.000000 genimtools-0.0.8/genimtools/src/common/models/tokenized_region.rs
--rw-r--r--   0     1001      127     3221 2024-01-17 19:17:43.000000 genimtools-0.0.8/genimtools/src/common/models/tokenized_regionset.rs
--rw-r--r--   0     1001      127     5315 2024-01-17 19:17:43.000000 genimtools-0.0.8/genimtools/src/common/models/universe.rs
--rw-r--r--   0     1001      127     1840 2024-01-17 19:17:43.000000 genimtools-0.0.8/genimtools/src/common/utils.rs
--rw-r--r--   0     1001      127      578 2024-01-17 19:17:43.000000 genimtools-0.0.8/genimtools/src/lib.rs
--rw-r--r--   0     1001      127     1284 2024-01-17 19:17:43.000000 genimtools-0.0.8/genimtools/src/main.rs
--rw-r--r--   0     1001      127     1961 2024-01-17 19:17:43.000000 genimtools-0.0.8/genimtools/src/tokenizers/cli.rs
--rw-r--r--   0     1001      127      497 2024-01-17 19:17:43.000000 genimtools-0.0.8/genimtools/src/tokenizers/mod.rs
--rw-r--r--   0     1001      127     2094 2024-01-17 19:17:43.000000 genimtools-0.0.8/genimtools/src/tokenizers/traits.rs
--rw-r--r--   0     1001      127     4798 2024-01-17 19:17:43.000000 genimtools-0.0.8/genimtools/src/tokenizers/tree_tokenizer.rs
--rw-r--r--   0     1001      127       52 2024-01-17 19:17:43.000000 genimtools-0.0.8/genimtools/src/uniwig/mod.rs
--rw-r--r--   0     1001      127     1752 2024-01-17 19:17:43.000000 genimtools-0.0.8/genimtools/src/vocab/cli.rs
--rw-r--r--   0     1001      127     2873 2024-01-17 19:17:43.000000 genimtools-0.0.8/genimtools/src/vocab/mod.rs
--rwxr-xr-x   0     1001      127      591 2024-01-17 19:17:43.000000 genimtools-0.0.8/genimtools/tests/data/peaks.bed
--rw-r--r--   0     1001      127       71 2024-01-17 19:17:43.000000 genimtools-0.0.8/genimtools/tests/data/to_tokenize.bed
--rw-r--r--   0     1001      127     2417 2024-01-17 19:17:43.000000 genimtools-0.0.8/genimtools/tests/test.rs
--rw-r--r--   0        0        0      288 1970-01-01 00:00:00.000000 genimtools-0.0.8/bindings/Cargo.toml
--rw-r--r--   0     1001      127      686 2024-01-17 19:17:43.000000 genimtools-0.0.8/bindings/.gitignore
--rw-r--r--   0     1001      127      521 2024-01-17 19:17:43.000000 genimtools-0.0.8/bindings/README.md
--rw-r--r--   0     1001      127       25 2024-01-17 19:17:43.000000 genimtools-0.0.8/bindings/genimtools/__init__.py
--rw-r--r--   0     1001      127       95 2024-01-17 19:17:43.000000 genimtools-0.0.8/bindings/genimtools/__init__.pyi
--rw-r--r--   0     1001      127       32 2024-01-17 19:17:43.000000 genimtools-0.0.8/bindings/genimtools/ailist/__init__.py
--rw-r--r--   0     1001      127      732 2024-01-17 19:17:43.000000 genimtools-0.0.8/bindings/genimtools/ailist/__init__.pyi
--rw-r--r--   0     1001      127       37 2024-01-17 19:17:43.000000 genimtools-0.0.8/bindings/genimtools/tokenizers/__init__.py
--rw-r--r--   0     1001      127     1087 2024-01-17 19:17:43.000000 genimtools-0.0.8/bindings/genimtools/tokenizers/__init__.pyi
--rw-r--r--   0     1001      127       31 2024-01-17 19:17:43.000000 genimtools-0.0.8/bindings/genimtools/vocab/__init__.py
--rw-r--r--   0     1001      127      707 2024-01-17 19:17:43.000000 genimtools-0.0.8/bindings/genimtools/vocab/__init__.pyi
--rw-r--r--   0     1001      127     1310 2024-01-17 19:17:43.000000 genimtools-0.0.8/bindings/src/ailist/mod.rs
--rw-r--r--   0     1001      127       39 2024-01-17 19:17:43.000000 genimtools-0.0.8/bindings/src/consts.rs
--rw-r--r--   0     1001      127     1240 2024-01-17 19:17:43.000000 genimtools-0.0.8/bindings/src/lib.rs
--rw-r--r--   0     1001      127      402 2024-01-17 19:17:43.000000 genimtools-0.0.8/bindings/src/models/interval.rs
--rw-r--r--   0     1001      127      230 2024-01-17 19:17:43.000000 genimtools-0.0.8/bindings/src/models/mod.rs
--rw-r--r--   0     1001      127     2434 2024-01-17 19:17:43.000000 genimtools-0.0.8/bindings/src/models/region.rs
--rw-r--r--   0     1001      127     2837 2024-01-17 19:17:43.000000 genimtools-0.0.8/bindings/src/models/region_set.rs
--rw-r--r--   0     1001      127     1144 2024-01-17 19:17:43.000000 genimtools-0.0.8/bindings/src/models/universe.rs
--rw-r--r--   0     1001      127      458 2024-01-17 19:17:43.000000 genimtools-0.0.8/bindings/src/tokenizers/mod.rs
--rw-r--r--   0     1001      127     4357 2024-01-17 19:17:43.000000 genimtools-0.0.8/bindings/src/tokenizers/tree_tokenizer.rs
--rw-r--r--   0     1001      127     1006 2024-01-17 19:17:43.000000 genimtools-0.0.8/bindings/src/vocab/mod.rs
--rw-r--r--   0     1001      127    43837 2024-01-17 19:17:52.000000 genimtools-0.0.8/bindings/Cargo.lock
--rw-r--r--   0        0        0      520 1970-01-01 00:00:00.000000 genimtools-0.0.8/pyproject.toml
--rw-r--r--   0     1001      127      707 2024-01-17 19:17:43.000000 genimtools-0.0.8/genimtools/vocab/__init__.pyi
--rw-r--r--   0     1001      127       31 2024-01-17 19:17:43.000000 genimtools-0.0.8/genimtools/vocab/__init__.py
--rw-r--r--   0     1001      127       95 2024-01-17 19:17:43.000000 genimtools-0.0.8/genimtools/__init__.pyi
--rw-r--r--   0     1001      127     1087 2024-01-17 19:17:43.000000 genimtools-0.0.8/genimtools/tokenizers/__init__.pyi
--rw-r--r--   0     1001      127       37 2024-01-17 19:17:43.000000 genimtools-0.0.8/genimtools/tokenizers/__init__.py
--rw-r--r--   0     1001      127      732 2024-01-17 19:17:43.000000 genimtools-0.0.8/genimtools/ailist/__init__.pyi
--rw-r--r--   0     1001      127       32 2024-01-17 19:17:43.000000 genimtools-0.0.8/genimtools/ailist/__init__.py
--rw-r--r--   0     1001      127       25 2024-01-17 19:17:43.000000 genimtools-0.0.8/genimtools/__init__.py
--rw-r--r--   0        0        0      850 1970-01-01 00:00:00.000000 genimtools-0.0.8/PKG-INFO
+-rw-r--r--   0     1001      127      597 2024-01-22 16:35:17.000000 genimtools-0.0.9/genimtools/Cargo.toml
+-rw-r--r--   0     1001      127     1529 2024-01-22 16:35:17.000000 genimtools-0.0.9/genimtools/docs/changelog.md
+-rw-r--r--   0     1001      127    64540 2024-01-22 16:35:17.000000 genimtools-0.0.9/genimtools/docs/logo.svg
+-rw-r--r--   0     1001      127     4804 2024-01-22 16:35:17.000000 genimtools-0.0.9/genimtools/src/ailist/mod.rs
+-rw-r--r--   0     1001      127      371 2024-01-22 16:35:17.000000 genimtools-0.0.9/genimtools/src/common/consts.rs
+-rw-r--r--   0     1001      127       47 2024-01-22 16:35:17.000000 genimtools-0.0.9/genimtools/src/common/mod.rs
+-rw-r--r--   0     1001      127      310 2024-01-22 16:35:17.000000 genimtools-0.0.9/genimtools/src/common/models/bed_set.rs
+-rw-r--r--   0     1001      127      396 2024-01-22 16:35:17.000000 genimtools-0.0.9/genimtools/src/common/models/mod.rs
+-rw-r--r--   0     1001      127      305 2024-01-22 16:35:17.000000 genimtools-0.0.9/genimtools/src/common/models/region.rs
+-rw-r--r--   0     1001      127     2812 2024-01-22 16:35:17.000000 genimtools-0.0.9/genimtools/src/common/models/region_set.rs
+-rw-r--r--   0     1001      127      107 2024-01-22 16:35:17.000000 genimtools-0.0.9/genimtools/src/common/models/tokenized_region.rs
+-rw-r--r--   0     1001      127     3568 2024-01-22 16:35:17.000000 genimtools-0.0.9/genimtools/src/common/models/tokenized_regionset.rs
+-rw-r--r--   0     1001      127     5315 2024-01-22 16:35:17.000000 genimtools-0.0.9/genimtools/src/common/models/universe.rs
+-rw-r--r--   0     1001      127     2921 2024-01-22 16:35:17.000000 genimtools-0.0.9/genimtools/src/common/utils.rs
+-rw-r--r--   0     1001      127     1039 2024-01-22 16:35:17.000000 genimtools-0.0.9/genimtools/src/io/mod.rs
+-rw-r--r--   0     1001      127      604 2024-01-22 16:35:17.000000 genimtools-0.0.9/genimtools/src/lib.rs
+-rw-r--r--   0     1001      127     1480 2024-01-22 16:35:17.000000 genimtools-0.0.9/genimtools/src/main.rs
+-rw-r--r--   0     1001      127     1961 2024-01-22 16:35:17.000000 genimtools-0.0.9/genimtools/src/tokenizers/cli.rs
+-rw-r--r--   0     1001      127      497 2024-01-22 16:35:17.000000 genimtools-0.0.9/genimtools/src/tokenizers/mod.rs
+-rw-r--r--   0     1001      127     2094 2024-01-22 16:35:17.000000 genimtools-0.0.9/genimtools/src/tokenizers/traits.rs
+-rw-r--r--   0     1001      127     5277 2024-01-22 16:35:17.000000 genimtools-0.0.9/genimtools/src/tokenizers/tree_tokenizer.rs
+-rw-r--r--   0     1001      127     3646 2024-01-22 16:35:17.000000 genimtools-0.0.9/genimtools/src/tools/cli.rs
+-rw-r--r--   0     1001      127     2143 2024-01-22 16:35:17.000000 genimtools-0.0.9/genimtools/src/tools/mod.rs
+-rw-r--r--   0     1001      127       52 2024-01-22 16:35:17.000000 genimtools-0.0.9/genimtools/src/uniwig/mod.rs
+-rw-r--r--   0     1001      127     1752 2024-01-22 16:35:17.000000 genimtools-0.0.9/genimtools/src/vocab/cli.rs
+-rw-r--r--   0     1001      127     2873 2024-01-22 16:35:17.000000 genimtools-0.0.9/genimtools/src/vocab/mod.rs
+-rwxr-xr-x   0     1001      127      591 2024-01-22 16:35:17.000000 genimtools-0.0.9/genimtools/tests/data/peaks.bed
+-rwxr-xr-x   0     1001      127      266 2024-01-22 16:35:17.000000 genimtools-0.0.9/genimtools/tests/data/peaks.bed.gz
+-rw-r--r--   0     1001      127       71 2024-01-22 16:35:17.000000 genimtools-0.0.9/genimtools/tests/data/to_tokenize.bed
+-rw-r--r--   0     1001      127     3306 2024-01-22 16:35:17.000000 genimtools-0.0.9/genimtools/tests/test.rs
+-rw-r--r--   0        0        0      288 1970-01-01 00:00:00.000000 genimtools-0.0.9/bindings/Cargo.toml
+-rw-r--r--   0     1001      127      686 2024-01-22 16:35:17.000000 genimtools-0.0.9/bindings/.gitignore
+-rw-r--r--   0     1001      127      521 2024-01-22 16:35:17.000000 genimtools-0.0.9/bindings/README.md
+-rw-r--r--   0     1001      127       25 2024-01-22 16:35:17.000000 genimtools-0.0.9/bindings/genimtools/__init__.py
+-rw-r--r--   0     1001      127       95 2024-01-22 16:35:17.000000 genimtools-0.0.9/bindings/genimtools/__init__.pyi
+-rw-r--r--   0     1001      127       32 2024-01-22 16:35:17.000000 genimtools-0.0.9/bindings/genimtools/ailist/__init__.py
+-rw-r--r--   0     1001      127      732 2024-01-22 16:35:17.000000 genimtools-0.0.9/bindings/genimtools/ailist/__init__.pyi
+-rw-r--r--   0     1001      127       37 2024-01-22 16:35:17.000000 genimtools-0.0.9/bindings/genimtools/tokenizers/__init__.py
+-rw-r--r--   0     1001      127     1386 2024-01-22 16:35:17.000000 genimtools-0.0.9/bindings/genimtools/tokenizers/__init__.pyi
+-rw-r--r--   0     1001      127       31 2024-01-22 16:35:17.000000 genimtools-0.0.9/bindings/genimtools/utils/__init__.py
+-rw-r--r--   0     1001      127      267 2024-01-22 16:35:17.000000 genimtools-0.0.9/bindings/genimtools/utils/__init__.pyi
+-rw-r--r--   0     1001      127       31 2024-01-22 16:35:17.000000 genimtools-0.0.9/bindings/genimtools/vocab/__init__.py
+-rw-r--r--   0     1001      127      707 2024-01-22 16:35:17.000000 genimtools-0.0.9/bindings/genimtools/vocab/__init__.pyi
+-rw-r--r--   0     1001      127     1296 2024-01-22 16:35:17.000000 genimtools-0.0.9/bindings/src/ailist/mod.rs
+-rw-r--r--   0     1001      127       39 2024-01-22 16:35:17.000000 genimtools-0.0.9/bindings/src/consts.rs
+-rw-r--r--   0     1001      127     1413 2024-01-22 16:35:17.000000 genimtools-0.0.9/bindings/src/lib.rs
+-rw-r--r--   0     1001      127      402 2024-01-22 16:35:17.000000 genimtools-0.0.9/bindings/src/models/interval.rs
+-rw-r--r--   0     1001      127      230 2024-01-22 16:35:17.000000 genimtools-0.0.9/bindings/src/models/mod.rs
+-rw-r--r--   0     1001      127     2434 2024-01-22 16:35:17.000000 genimtools-0.0.9/bindings/src/models/region.rs
+-rw-r--r--   0     1001      127     2838 2024-01-22 16:35:17.000000 genimtools-0.0.9/bindings/src/models/region_set.rs
+-rw-r--r--   0     1001      127     1144 2024-01-22 16:35:17.000000 genimtools-0.0.9/bindings/src/models/universe.rs
+-rw-r--r--   0     1001      127      458 2024-01-22 16:35:17.000000 genimtools-0.0.9/bindings/src/tokenizers/mod.rs
+-rw-r--r--   0     1001      127     5177 2024-01-22 16:35:17.000000 genimtools-0.0.9/bindings/src/tokenizers/tree_tokenizer.rs
+-rw-r--r--   0     1001      127      566 2024-01-22 16:35:17.000000 genimtools-0.0.9/bindings/src/utils/mod.rs
+-rw-r--r--   0     1001      127     1006 2024-01-22 16:35:17.000000 genimtools-0.0.9/bindings/src/vocab/mod.rs
+-rw-r--r--   0     1001      127    45430 2024-01-22 16:35:26.000000 genimtools-0.0.9/bindings/Cargo.lock
+-rw-r--r--   0        0        0      520 1970-01-01 00:00:00.000000 genimtools-0.0.9/pyproject.toml
+-rw-r--r--   0     1001      127      707 2024-01-22 16:35:17.000000 genimtools-0.0.9/genimtools/vocab/__init__.pyi
+-rw-r--r--   0     1001      127       31 2024-01-22 16:35:17.000000 genimtools-0.0.9/genimtools/vocab/__init__.py
+-rw-r--r--   0     1001      127       95 2024-01-22 16:35:17.000000 genimtools-0.0.9/genimtools/__init__.pyi
+-rw-r--r--   0     1001      127     1386 2024-01-22 16:35:17.000000 genimtools-0.0.9/genimtools/tokenizers/__init__.pyi
+-rw-r--r--   0     1001      127       37 2024-01-22 16:35:17.000000 genimtools-0.0.9/genimtools/tokenizers/__init__.py
+-rw-r--r--   0     1001      127      732 2024-01-22 16:35:17.000000 genimtools-0.0.9/genimtools/ailist/__init__.pyi
+-rw-r--r--   0     1001      127       32 2024-01-22 16:35:17.000000 genimtools-0.0.9/genimtools/ailist/__init__.py
+-rw-r--r--   0     1001      127      267 2024-01-22 16:35:17.000000 genimtools-0.0.9/genimtools/utils/__init__.pyi
+-rw-r--r--   0     1001      127       31 2024-01-22 16:35:17.000000 genimtools-0.0.9/genimtools/utils/__init__.py
+-rw-r--r--   0     1001      127       25 2024-01-22 16:35:17.000000 genimtools-0.0.9/genimtools/__init__.py
+-rw-r--r--   0        0        0      850 1970-01-01 00:00:00.000000 genimtools-0.0.9/PKG-INFO
```

### Comparing `genimtools-0.0.8/genimtools/Cargo.toml` & `genimtools-0.0.9/genimtools/Cargo.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 [package]
 name = "genimtools"
-version = "0.0.8"
+version = "0.0.9"
 edition = "2021"
 description = "Performance-critical tools to manipulate, analyze, and process genomic interval data. Primarily focused on building tools for geniml - our genomic machine learning python package."
 license = "MIT"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [dependencies]
 clap = { version = "4.4.7", features = ["derive"] }
+flate2 = "1.0.28"
 indicatif = "0.17.7"
 polars = "0.35.4"
 rust-lapper = "1.1.0"
+walkdir = "2.4.0"
 
 [dev-dependencies]
 rstest = "0.18.2"
 tempfile = "3.8.1"
```

### Comparing `genimtools-0.0.8/genimtools/docs/changelog.md` & `genimtools-0.0.9/genimtools/docs/changelog.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [0.0.9]
+- start working on the concept of a `.gtok` file-format to store tokenized regions
+- - added basic readers and writers for this format
+
 ## [0.0.8]
 - add a new `ids_as_strs` getter to the `TokenizedRegionSet` struct so that we can get the ids as strings quickly, this is meant mostly for interface with geniml.
 
 ## [0.0.7]
 - move things around based on rust club feedback
 
 ## [0.0.6]
```

### Comparing `genimtools-0.0.8/genimtools/docs/logo.svg` & `genimtools-0.0.9/genimtools/docs/logo.svg`

 * *Files identical despite different names*

### Comparing `genimtools-0.0.8/genimtools/src/ailist/mod.rs` & `genimtools-0.0.9/genimtools/src/ailist/mod.rs`

 * *Files 5% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
             starts.append(&mut results.0);
             ends.append(&mut results.1);
             max_ends.append(&mut results.2);
 
             *intervals = results.3;
 
-            if intervals.len() == 0 {
+            if intervals.is_empty() {
                 break;
             } else {
                 header_list.push(starts.len());
             }
         }
 
         AIList {
@@ -49,15 +49,15 @@
             ends,
             max_ends,
             header_list,
         }
     }
 
     fn decompose(
-        intervals: &mut Vec<Interval>,
+        intervals: &mut [Interval],
         minimum_coverage_length: usize,
     ) -> (Vec<u32>, Vec<u32>, Vec<u32>, Vec<Interval>) {
         // look at the next minL*2 intervals
         let mut starts: Vec<u32> = Vec::new();
         let mut ends: Vec<u32> = Vec::new();
         let mut max_ends: Vec<u32> = Vec::new();
         let mut l2: Vec<Interval> = Vec::new();
@@ -115,15 +115,15 @@
             } else {
                 results_list.push(Interval {
                     start: starts[i],
                     end: ends[i],
                 })
             }
         }
-        return results_list;
+        results_list
     }
 
     pub fn query(&self, interval: &Interval) -> Vec<Interval> {
         let mut results_list: Vec<Interval> = Vec::new();
 
         for i in 0..(self.header_list.len() - 1) {
             results_list.append(&mut Self::query_slice(
@@ -138,15 +138,15 @@
         results_list.extend(Self::query_slice(
             interval,
             &self.starts[self.header_list[i]..],
             &self.ends[self.header_list[i]..],
             &self.max_ends[self.header_list[i]..],
         ));
 
-        return results_list;
+        results_list
     }
 
     pub fn print(&self) {
         println!("");
         for element in self.starts.iter() {
             print!("{}, ", element);
         }
```

### Comparing `genimtools-0.0.8/genimtools/src/common/models/region_set.rs` & `genimtools-0.0.9/genimtools/src/common/models/region_set.rs`

 * *Files identical despite different names*

### Comparing `genimtools-0.0.8/genimtools/src/common/models/tokenized_regionset.rs` & `genimtools-0.0.9/genimtools/src/common/models/tokenized_regionset.rs`

 * *Files 12% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 use std::io::Write;
 use std::path::PathBuf;
 
 use crate::common::consts::{PAD_CHR, PAD_END, PAD_START};
 use crate::common::models::region::Region;
 use crate::common::models::tokenized_region::TokenizedRegion;
 use crate::common::models::universe::Universe;
+use crate::io::write_tokens_to_gtok;
 
 pub struct TokenizedRegionSet<'a> {
     pub regions: Vec<Region>,
     pub universe: &'a Universe,
 }
 
 impl<'a> IntoIterator for &'a TokenizedRegionSet<'_> {
@@ -65,14 +66,24 @@
             );
             file.write_all(line.as_bytes())?;
         }
         Ok(())
     }
 
     ///
+    /// Write a TokenizedRegionSet to a .gtok file
+    /// * `path` - A PathBuf to write the .gtok file to
+    /// 
+    pub fn to_gtok_file(&self, path: &str) -> Result<(), Box<dyn Error>> {
+        let tokens = self.to_region_ids();
+        write_tokens_to_gtok(path, &tokens)?;
+        Ok(())
+    }
+
+    ///
     /// Convert a TokenizedRegionSet to a vector of region IDs
     ///
     pub fn to_region_ids(&self) -> Vec<u32> {
         let mut region_ids = Vec::new();
         for region in &self.regions {
             region_ids.push(self.universe.convert_chr_start_end_to_id(
                 &region.chr,
```

### Comparing `genimtools-0.0.8/genimtools/src/common/models/universe.rs` & `genimtools-0.0.9/genimtools/src/common/models/universe.rs`

 * *Files identical despite different names*

### Comparing `genimtools-0.0.8/genimtools/src/common/utils.rs` & `genimtools-0.0.9/genimtools/src/common/utils.rs`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 use std::collections::HashMap;
 use std::error::Error;
 use std::fs::File;
 use std::io::{BufRead, BufReader};
 use std::path::Path;
 
+use clap::builder::OsStr;
+use flate2::read::GzDecoder;
 use polars::datatypes::DataType;
 use polars::prelude::*;
 
 use crate::common::consts::{CHR_COL_NAME, DELIMITER, END_COL_NAME, START_COL_NAME};
 use crate::common::models::region::Region;
 
 pub fn bed_file_to_df(path: &Path) -> Result<DataFrame, Box<dyn std::error::Error>> {
@@ -38,31 +40,59 @@
         });
     }
 
     region_to_id
 }
 
 pub fn extract_regions_from_bed_file(path: &Path) -> Result<Vec<Region>, Box<dyn Error>> {
-    let file = File::open(path)?;
-    let reader = BufReader::new(file);
-
+    let file = File::open(path)?; 
     let mut regions = Vec::new();
 
-    for line in reader.lines() {
-        let line = line?;
-        let fields: Vec<&str> = line.split('\t').collect();
-
-        let chr = fields[0];
-        let start = fields[1].parse::<u32>()?;
-        let end = fields[2].parse::<u32>()?;
-
-        let region = Region {
-            chr: chr.to_string(),
-            start,
-            end,
-        };
-
-        regions.push(region);
+    // determine if the file is gzipped; default to extension is bed
+    // because we dont truly care what the extension is
+    // we just want to know if it is gzipped or not, and we dont want to
+    // fail if the extension is not present (e.g. a user passes in a file without an extension)
+    let is_gzipped = path.extension().unwrap_or(&OsStr::from("bed")) == "gz";
+
+    if is_gzipped {
+        let decoder = GzDecoder::new(file);
+        let reader = BufReader::new(decoder);
+
+        for line in reader.lines() {
+            let line = line?;
+            let fields: Vec<&str> = line.split('\t').collect();
+    
+            let chr = fields[0];
+            let start = fields[1].parse::<u32>()?;
+            let end = fields[2].parse::<u32>()?;
+    
+            let region = Region {
+                chr: chr.to_string(),
+                start,
+                end,
+            };
+    
+            regions.push(region);
+        }
+    } else {
+        let reader = BufReader::new(file);
+
+        for line in reader.lines() {
+            let line = line?;
+            let fields: Vec<&str> = line.split('\t').collect();
+    
+            let chr = fields[0];
+            let start = fields[1].parse::<u32>()?;
+            let end = fields[2].parse::<u32>()?;
+    
+            let region = Region {
+                chr: chr.to_string(),
+                start,
+                end,
+            };
+    
+            regions.push(region);
+        }
     }
 
     Ok(regions)
 }
```

### Comparing `genimtools-0.0.8/genimtools/src/lib.rs` & `genimtools-0.0.9/genimtools/src/lib.rs`

 * *Files 26% similar despite different names*

```diff
@@ -5,7 +5,9 @@
 //! However, it can be used as a standalone library for working with genomic intervals as well.
 //!
 pub mod ailist;
 pub mod common;
 pub mod tokenizers;
 pub mod uniwig;
 pub mod vocab;
+pub mod tools;
+pub mod io;
```

### Comparing `genimtools-0.0.8/genimtools/src/main.rs` & `genimtools-0.0.9/genimtools/src/main.rs`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 use clap::Command;
 
 // go through the library crate to get the interfaces
 use genimtools::tokenizers;
 use genimtools::vocab;
+use genimtools::tools;
 // use genimtools::uniwig;
 
 pub mod consts {
     pub const VERSION: &str = env!("CARGO_PKG_VERSION");
     pub const PKG_NAME: &str = env!("CARGO_PKG_NAME");
     pub const BIN_NAME: &str = env!("CARGO_PKG_NAME");
     pub const UNIWIG_CMD: &str = "uniwig";
@@ -17,24 +18,28 @@
         .bin_name(consts::BIN_NAME)
         .version(consts::VERSION)
         .author("Databio")
         .about("Performance critical tools for working with genomic interval data with an emphasis on preprocessing for machine learning pipelines.")
         .subcommand_required(true)
         .subcommand(vocab::cli::make_prune_cli())
         .subcommand(tokenizers::cli::make_tokenization_cli())
+        .subcommand(tools::cli::make_tools_cli())
 }
 
 fn main() {
     let app = build_parser();
     let matches = app.get_matches();
 
     match matches.subcommand() {
         Some((vocab::consts::PRUNE_CMD, matches)) => {
             vocab::cli::handlers::prune_universe(matches);
         }
         Some((tokenizers::consts::TOKENIZE_CMD, matches)) => {
             tokenizers::cli::handlers::tokenize_bed_file(matches);
         }
+        Some((tools::consts::TOOLS_CMD, matches)) => {
+            tools::cli::handlers::tools_handler(matches);
+        }
 
         _ => unreachable!("Subcommand not found"),
     };
 }
```

### Comparing `genimtools-0.0.8/genimtools/src/tokenizers/cli.rs` & `genimtools-0.0.9/genimtools/src/tokenizers/cli.rs`

 * *Files identical despite different names*

### Comparing `genimtools-0.0.8/genimtools/src/tokenizers/traits.rs` & `genimtools-0.0.9/genimtools/src/tokenizers/traits.rs`

 * *Files identical despite different names*

### Comparing `genimtools-0.0.8/genimtools/src/tokenizers/tree_tokenizer.rs` & `genimtools-0.0.9/genimtools/src/tokenizers/tree_tokenizer.rs`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 use std::path::Path;
 
 use polars::prelude::*;
 use rust_lapper::{Interval, Lapper};
 
 use crate::common::consts::{UNKNOWN_CHR, UNKNOWN_END, UNKNOWN_START};
 use crate::common::models::{Region, RegionSet, TokenizedRegionSet, Universe};
+use crate::common::utils::extract_regions_from_bed_file;
 use crate::tokenizers::traits::Tokenizer;
 
 pub struct TreeTokenizer {
     pub universe: Universe,
     pub tree: HashMap<String, Lapper<u32, ()>>,
 }
 
@@ -146,7 +147,21 @@
 
         Some(TokenizedRegionSet {
             regions: tokenized_regions,
             universe: &self.universe,
         })
     }
 }
+
+impl TreeTokenizer {
+    pub fn tokenize_bed_file(&self, bed_file: &Path) -> Option<TokenizedRegionSet> {
+        let regions = extract_regions_from_bed_file(bed_file);
+        match regions {
+            Ok(regions) => {
+                let rs = RegionSet::from(regions);
+                self.tokenize_region_set(&rs)
+            },
+            Err(e) => panic!("Error reading bedfile: {}", e)
+        }
+        
+    }
+}
```

### Comparing `genimtools-0.0.8/genimtools/src/vocab/cli.rs` & `genimtools-0.0.9/genimtools/src/vocab/cli.rs`

 * *Files identical despite different names*

### Comparing `genimtools-0.0.8/genimtools/src/vocab/mod.rs` & `genimtools-0.0.9/genimtools/src/vocab/mod.rs`

 * *Files identical despite different names*

### Comparing `genimtools-0.0.8/genimtools/tests/data/peaks.bed` & `genimtools-0.0.9/genimtools/tests/data/peaks.bed`

 * *Files identical despite different names*

### Comparing `genimtools-0.0.8/genimtools/tests/test.rs` & `genimtools-0.0.9/genimtools/tests/test.rs`

 * *Files 21% similar despite different names*

```diff
@@ -8,19 +8,26 @@
 
 #[fixture]
 fn path_to_bed_file() -> &'static str {
     "tests/data/peaks.bed"
 }
 
 #[fixture]
+fn path_to_bed_file_gzipped() -> &'static str {
+    "tests/data/peaks.bed.gz"
+}
+
+#[fixture]
 fn path_to_tokenize_bed_file() -> &'static str {
     "tests/data/to_tokenize.bed"
 }
 
 mod tests {
+    use genimtools::common::utils::extract_regions_from_bed_file;
+
     use super::*;
 
     #[rstest]
     fn test_region() {
         let region = Region {
             chr: "chr1".to_string(),
             start: 100,
@@ -29,14 +36,32 @@
 
         assert_eq!(region.chr, "chr1");
         assert_eq!(region.start, 100);
         assert_eq!(region.end, 200);
     }
 
     #[rstest]
+    fn test_extract_regions_from_bed_file(path_to_bed_file: &str) {
+        let path = Path::new(path_to_bed_file);
+        let regions = extract_regions_from_bed_file(path);
+        assert!(regions.is_ok(), "Failed to extract regions from BED file");
+        let regions = regions.unwrap();
+        assert!(regions.len() == 25);
+    }
+    
+    #[rstest]
+    fn test_extract_regions_from_bed_file_gzipped(path_to_bed_file_gzipped: &str) {
+        let path = Path::new(path_to_bed_file_gzipped);
+        let regions = extract_regions_from_bed_file(path);
+        assert!(regions.is_ok(), "Failed to extract regions from BED file");
+        let regions = regions.unwrap();
+        assert!(regions.len() == 25);
+    }
+
+    #[rstest]
     fn test_region_set_from_bed(path_to_bed_file: &str) {
         let path = Path::new(path_to_bed_file);
         let rs = RegionSet::try_from(path).unwrap();
 
         assert!(rs.regions.height() == 25);
     }
```

### Comparing `genimtools-0.0.8/bindings/.gitignore` & `genimtools-0.0.9/bindings/.gitignore`

 * *Files identical despite different names*

### Comparing `genimtools-0.0.8/bindings/README.md` & `genimtools-0.0.9/bindings/README.md`

 * *Files identical despite different names*

### Comparing `genimtools-0.0.8/bindings/genimtools/ailist/__init__.pyi` & `genimtools-0.0.9/bindings/genimtools/ailist/__init__.pyi`

 * *Files identical despite different names*

### Comparing `genimtools-0.0.8/bindings/genimtools/tokenizers/__init__.pyi` & `genimtools-0.0.9/bindings/genimtools/tokenizers/__init__.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -38,8 +38,17 @@
         :param universe: The universe of characters to use for tokenization.
         """
         pass
     
     def tokenize(self, regions: List[Region]) -> TokenizedRegionSet:
         """
         Tokenize a list of regions.
+        """
+    
+    def tokenize_bed_file(self, bed_file: str) -> TokenizedRegionSet:
+        """
+        Tokenize a bed file directly.
+
+        This was added to create a more performant tokenization strategy
+        that could tokenize directly from disk in rust instead of using
+        pandas.
         """
```

### Comparing `genimtools-0.0.8/bindings/genimtools/vocab/__init__.pyi` & `genimtools-0.0.9/bindings/genimtools/vocab/__init__.pyi`

 * *Files identical despite different names*

### Comparing `genimtools-0.0.8/bindings/src/ailist/mod.rs` & `genimtools-0.0.9/bindings/src/ailist/mod.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 use genimtools::ailist::{AIList, Interval};
-use pyo3::{prelude::*, pyclass, PyNativeType};
+use pyo3::{prelude::*, pyclass};
 
 use crate::models::PyInterval;
 
 #[pyclass(name = "AIList")]
 struct PyAIList {
     ailist: AIList,
 }
```

### Comparing `genimtools-0.0.8/bindings/src/lib.rs` & `genimtools-0.0.9/bindings/src/lib.rs`

 * *Files 11% similar despite different names*

```diff
@@ -2,33 +2,38 @@
 use pyo3::types::PyDict;
 
 mod ailist;
 mod consts;
 mod models;
 mod tokenizers;
 mod vocab;
+mod utils;
 
 pub const VERSION: &str = env!("CARGO_PKG_VERSION");
 
 #[pymodule]
 fn genimtools(py: Python, m: &PyModule) -> PyResult<()> {
     let vocab_module = pyo3::wrap_pymodule!(vocab::vocab);
     let tokenize_module = pyo3::wrap_pymodule!(tokenizers::tokenizers);
     let ailist_module = pyo3::wrap_pymodule!(ailist::ailist);
+    let utils_module = pyo3::wrap_pymodule!(utils::utils);
+
     m.add_wrapped(vocab_module)?;
     m.add_wrapped(tokenize_module)?;
     m.add_wrapped(ailist_module)?;
+    m.add_wrapped(utils_module)?;
 
     let sys = PyModule::import(py, "sys")?;
     let sys_modules: &PyDict = sys.getattr("modules")?.downcast()?;
 
     // set names of submodules
     sys_modules.set_item("genimtools.vocab", m.getattr("vocab")?)?;
     sys_modules.set_item("genimtools.tokenizers", m.getattr("tokenizers")?)?;
     sys_modules.set_item("genimtools.ailist", m.getattr("ailist")?)?;
+    sys_modules.set_item("genimtools.utils", m.getattr("utils")?)?;
 
     // add constants
     m.add("PAD_CHR", consts::PAD_CHR)?;
     m.add("PAD_START", consts::PAD_START)?;
     m.add("PAD_END", consts::PAD_END)?;
     m.add("UNKNOWN_CHR", consts::UNKNOWN_CHR)?;
     m.add("UNKNOWN_START", consts::UNKNOWN_START)?;
```

### Comparing `genimtools-0.0.8/bindings/src/models/region.rs` & `genimtools-0.0.9/bindings/src/models/region.rs`

 * *Files identical despite different names*

### Comparing `genimtools-0.0.8/bindings/src/models/region_set.rs` & `genimtools-0.0.9/bindings/src/models/region_set.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 use pyo3::exceptions::PyIndexError;
 use pyo3::prelude::*;
 
 use genimtools::common::consts::{PAD_CHR, PAD_END, PAD_START};
 
 use crate::models::{PyRegion, PyTokenizedRegion};
 
+
 #[pyclass(name = "TokenizedRegionSet")]
 #[derive(Clone, Debug)]
 pub struct PyTokenizedRegionSet {
     pub regions: Vec<PyRegion>,
     pub ids: Vec<u32>,
     curr: usize,
 }
```

### Comparing `genimtools-0.0.8/bindings/src/models/universe.rs` & `genimtools-0.0.9/bindings/src/models/universe.rs`

 * *Files identical despite different names*

### Comparing `genimtools-0.0.8/bindings/src/tokenizers/tree_tokenizer.rs` & `genimtools-0.0.9/bindings/src/tokenizers/tree_tokenizer.rs`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+use pyo3::exceptions::PyRuntimeError;
 use pyo3::prelude::*;
 use pyo3::types::PyList;
 
 use std::collections::HashMap;
 use std::path::Path;
 
 use genimtools::common::consts::{
@@ -144,8 +145,31 @@
             }
             // return error if tokenized_regions is None
             None => Err(pyo3::exceptions::PyValueError::new_err(
                 "Failed to tokenize regions",
             )),
         }
     }
+
+    pub fn tokenize_bed_file(&self, path: String) -> PyResult<PyTokenizedRegionSet> {
+        let bed_file = Path::new(&path);
+        let tokens = self.tokenizer.tokenize_bed_file(bed_file);
+
+        match tokens {
+            Some(tokens) => {
+                let regions = tokens
+                    .into_iter()
+                    .map(|x| PyRegion {
+                        chr: x.chr,
+                        start: x.start,
+                        end: x.end,
+                    })
+                    .collect::<Vec<_>>();
+
+                let ids = tokens.to_region_ids();
+
+                Ok(PyTokenizedRegionSet::new(regions, ids))
+            },
+            None => Err(PyErr::new::<PyRuntimeError, _>(format!("Error parsing the bedfile: {}", path)))
+        }
+    }
 }
```

### Comparing `genimtools-0.0.8/bindings/src/vocab/mod.rs` & `genimtools-0.0.9/bindings/src/vocab/mod.rs`

 * *Files identical despite different names*

### Comparing `genimtools-0.0.8/bindings/Cargo.lock` & `genimtools-0.0.9/bindings/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
+name = "adler"
+version = "1.0.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f26201604c87b1e01bd3d98f8d5d9a8fcbb815e8cedb41ffccbeb4bf593a35fe"
+
+[[package]]
 name = "ahash"
 version = "0.8.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "77c3a9648d43b9cd48db467b3f87fdd6e146bcc88ab0180006cef2179fe11d01"
 dependencies = [
  "cfg-if",
  "getrandom",
@@ -43,17 +49,17 @@
 checksum = "819e7219dbd41043ac279b19830f2efc897156490d7fd6ea916720117ee66311"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "anstream"
-version = "0.6.8"
+version = "0.6.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "628a8f9bd1e24b4e0db2b4bc2d000b001e7dd032d54afa60a68836aeec5aa54a"
+checksum = "6e2e1ebcb11de5c03c67de28a7df593d32191b44939c482e97702baaaa6ab6a5"
 dependencies = [
  "anstyle",
  "anstyle-parse",
  "anstyle-query",
  "anstyle-wincon",
  "colorchoice",
  "utf8parse",
@@ -285,14 +291,23 @@
 [[package]]
 name = "core-foundation-sys"
 version = "0.8.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "06ea2b9bc92be3c2baa9334a323ebca2d6f074ff852cd1d7b11064035cd3868f"
 
 [[package]]
+name = "crc32fast"
+version = "1.3.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b540bd8bc810d3885c6ea91e2018302f68baba2129ab3e88f32389ee9370880d"
+dependencies = [
+ "cfg-if",
+]
+
+[[package]]
 name = "crossbeam-channel"
 version = "0.5.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "176dc175b78f56c0f321911d9c8eb2b77a78a4860b9c19db83835fea1a46649b"
 dependencies = [
  "crossbeam-utils",
 ]
@@ -398,32 +413,44 @@
 [[package]]
 name = "fast-float"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "95765f67b4b18863968b4a1bd5bb576f732b29a4a28c7cd84c09fa3e2875f33c"
 
 [[package]]
+name = "flate2"
+version = "1.0.28"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "46303f565772937ffe1d394a4fac6f411c6013172fadde9dcdb1e147a086940e"
+dependencies = [
+ "crc32fast",
+ "miniz_oxide",
+]
+
+[[package]]
 name = "foreign_vec"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ee1b05cbd864bcaecbd3455d6d967862d446e4ebfc3c2e5e5b9841e53cba6673"
 
 [[package]]
 name = "genimtools"
-version = "0.0.8"
+version = "0.0.9"
 dependencies = [
  "clap",
+ "flate2",
  "indicatif",
  "polars",
  "rust-lapper",
+ "walkdir",
 ]
 
 [[package]]
 name = "genimtools-py"
-version = "0.0.8"
+version = "0.0.9"
 dependencies = [
  "genimtools",
  "pyo3",
 ]
 
 [[package]]
 name = "getrandom"
@@ -630,14 +657,23 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
+name = "miniz_oxide"
+version = "0.7.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e7810e0be55b428ada41041c41f32c9f1a42817901b4ccf45fa3d4b6561e74c7"
+dependencies = [
+ "adler",
+]
+
+[[package]]
 name = "multiversion"
 version = "0.7.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b2c7b9d7fe61760ce5ea19532ead98541f6b4c495d87247aff9826445cf6872a"
 dependencies = [
  "multiversion-macros",
  "target-features",
@@ -1028,17 +1064,17 @@
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.76"
+version = "1.0.78"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "95fc56cda0b5c3325f5fbbd7ff9fda9e02bb00bb3dac51252d2f1bfa1cb8cc8c"
+checksum = "e2422ad645d89c99f8f3e6b88a9fdeca7fabeac836b1002371c4367c8f984aae"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
 version = "0.20.2"
@@ -1176,29 +1212,29 @@
 checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
 dependencies = [
  "bitflags 1.3.2",
 ]
 
 [[package]]
 name = "regex"
-version = "1.10.2"
+version = "1.10.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "380b951a9c5e80ddfd6136919eef32310721aa4aacd4889a8d39124b026ab343"
+checksum = "b62dbe01f0b06f9d8dc7d49e05a0785f153b00b2c227856282f671e0318c9b15"
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-automata",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-automata"
-version = "0.4.3"
+version = "0.4.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5f804c7828047e88b2d32e2d7fe5a105da8ee3264f01902f796c8e067dc2483f"
+checksum = "3b7fa1134405e2ec9353fd416b17f8dacd46c473d7d3fd1cf202706a14eb792a"
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-syntax",
 ]
 
 [[package]]
@@ -1234,14 +1270,23 @@
 [[package]]
 name = "ryu"
 version = "1.0.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f98d2aa92eebf49b69786be48e4477826b256916e84a57ff2a4f21923b48eb4c"
 
 [[package]]
+name = "same-file"
+version = "1.0.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "93fc1dc3aaa9bfed95e02e6eadabb4baf7e3078b0bd1b4d7b6b0b68378900502"
+dependencies = [
+ "winapi-util",
+]
+
+[[package]]
 name = "scopeguard"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
 name = "semver"
@@ -1284,17 +1329,17 @@
 name = "simdutf8"
 version = "0.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f27f6278552951f1f2b8cf9da965d10969b2efdea95a6ec47987ab46edfe263a"
 
 [[package]]
 name = "smallvec"
-version = "1.12.0"
+version = "1.13.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2593d31f82ead8df961d8bd23a64c2ccf2eb5dd34b0a34bfb4dd54011c72009e"
+checksum = "e6ecd384b10a64542d77071bd64bd7b231f4ed5940fba55e98c3de13824cf3d7"
 
 [[package]]
 name = "smartstring"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3fb72c633efbaa2dd666986505016c32c3044395ceaf881518399d2f4127ee29"
 dependencies = [
@@ -1450,14 +1495,24 @@
 [[package]]
 name = "version_check"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
 
 [[package]]
+name = "walkdir"
+version = "2.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d71d857dc86794ca4c280d616f7da00d2dbfd8cd788846559a6813e6aa4b54ee"
+dependencies = [
+ "same-file",
+ "winapi-util",
+]
+
+[[package]]
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
 name = "wasm-bindgen"
@@ -1526,14 +1581,23 @@
 [[package]]
 name = "winapi-i686-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ac3b87c63620426dd9b991e5ce0329eff545bccbbb34f3be09ff6fb6ab51b7b6"
 
 [[package]]
+name = "winapi-util"
+version = "0.1.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f29e6f9198ba0d26b4c9f07dbe6f9ed633e1f3d5b8b414090084349e46a52596"
+dependencies = [
+ "winapi",
+]
+
+[[package]]
 name = "winapi-x86_64-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
 
 [[package]]
 name = "windows-core"
```

### Comparing `genimtools-0.0.8/pyproject.toml` & `genimtools-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `genimtools-0.0.8/genimtools/vocab/__init__.pyi` & `genimtools-0.0.9/genimtools/vocab/__init__.pyi`

 * *Files identical despite different names*

### Comparing `genimtools-0.0.8/genimtools/tokenizers/__init__.pyi` & `genimtools-0.0.9/genimtools/tokenizers/__init__.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -38,8 +38,17 @@
         :param universe: The universe of characters to use for tokenization.
         """
         pass
     
     def tokenize(self, regions: List[Region]) -> TokenizedRegionSet:
         """
         Tokenize a list of regions.
+        """
+    
+    def tokenize_bed_file(self, bed_file: str) -> TokenizedRegionSet:
+        """
+        Tokenize a bed file directly.
+
+        This was added to create a more performant tokenization strategy
+        that could tokenize directly from disk in rust instead of using
+        pandas.
         """
```

### Comparing `genimtools-0.0.8/genimtools/ailist/__init__.pyi` & `genimtools-0.0.9/genimtools/ailist/__init__.pyi`

 * *Files identical despite different names*

### Comparing `genimtools-0.0.8/PKG-INFO` & `genimtools-0.0.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genimtools
-Version: 0.0.8
+Version: 0.0.9
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 # genimtools
```

