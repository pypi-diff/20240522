# Comparing `tmp/sideko_py-0.4.1.tar.gz` & `tmp/sideko_py-0.5.0.tar.gz`

## Comparing `sideko_py-0.4.1.tar` & `sideko_py-0.5.0.tar`

### file list

```diff
@@ -1,31 +1,32 @@
--rw-r--r--   0      501       20      835 2024-04-22 13:43:15.000000 sideko_py-0.4.1/core/Cargo.toml
--rw-r--r--   0      501       20     6012 2024-04-22 13:43:15.000000 sideko_py-0.4.1/core/src/cli.rs
--rw-r--r--   0      501       20     4653 2024-04-22 13:43:15.000000 sideko_py-0.4.1/core/src/cmds/generate.rs
--rw-r--r--   0      501       20     3492 2024-04-22 13:43:15.000000 sideko_py-0.4.1/core/src/cmds/login.rs
--rw-r--r--   0      501       20       33 2024-04-22 13:43:15.000000 sideko_py-0.4.1/core/src/cmds/mod.rs
--rw-r--r--   0      501       20     2011 2024-04-22 13:43:15.000000 sideko_py-0.4.1/core/src/config.rs
--rw-r--r--   0      501       20     1264 2024-04-22 13:43:15.000000 sideko_py-0.4.1/core/src/html/failure.html
--rw-r--r--   0      501       20     1216 2024-04-22 13:43:15.000000 sideko_py-0.4.1/core/src/html/success.html
--rw-r--r--   0      501       20       90 2024-04-22 13:43:15.000000 sideko_py-0.4.1/core/src/lib.rs
--rw-r--r--   0      501       20      203 2024-04-22 13:43:15.000000 sideko_py-0.4.1/core/src/main.rs
--rw-r--r--   0      501       20     1850 2024-04-22 13:43:15.000000 sideko_py-0.4.1/core/src/result.rs
--rw-r--r--   0      501       20     1060 2024-04-22 13:43:15.000000 sideko_py-0.4.1/core/src/styles.rs
--rw-r--r--   0      501       20     3176 2024-04-22 13:43:15.000000 sideko_py-0.4.1/core/src/utils.rs
--rw-r--r--   0      501       20      484 2024-04-22 13:43:15.000000 sideko_py-0.4.1/sideko-api/Cargo.toml
--rw-r--r--   0      501       20     2195 2024-04-22 13:43:15.000000 sideko_py-0.4.1/sideko-api/README.md
--rw-r--r--   0      501       20     3169 2024-04-22 13:43:15.000000 sideko_py-0.4.1/sideko-api/src/auth.rs
--rw-r--r--   0      501       20     8275 2024-04-22 13:43:15.000000 sideko_py-0.4.1/sideko-api/src/blocking.rs
--rw-r--r--   0      501       20      580 2024-04-22 13:43:15.000000 sideko_py-0.4.1/sideko-api/src/error_enums.rs
--rw-r--r--   0      501       20     8915 2024-04-22 13:43:15.000000 sideko_py-0.4.1/sideko-api/src/lib.rs
--rw-r--r--   0      501       20      445 2024-04-22 13:43:15.000000 sideko_py-0.4.1/sideko-api/src/request_types.rs
--rw-r--r--   0      501       20     1522 2024-04-22 13:43:15.000000 sideko_py-0.4.1/sideko-api/src/result.rs
--rw-r--r--   0      501       20     3579 2024-04-22 13:43:15.000000 sideko_py-0.4.1/sideko-api/src/schemas.rs
--rw-r--r--   0        0        0      481 1970-01-01 00:00:00.000000 sideko_py-0.4.1/sideko-py/Cargo.toml
--rw-r--r--   0      501       20     3860 2024-04-22 13:43:15.000000 sideko_py-0.4.1/sideko-py/LICENSE
--rw-r--r--   0      501       20     1640 2024-04-22 13:43:15.000000 sideko_py-0.4.1/sideko-py/README.md
--rw-r--r--   0      501       20     2334 2024-04-22 13:43:15.000000 sideko_py-0.4.1/sideko-py/src/lib.rs
--rw-r--r--   0      501       20    62967 2024-04-22 13:43:15.000000 sideko_py-0.4.1/Cargo.lock
--rw-r--r--   0        0        0      297 1970-01-01 00:00:00.000000 sideko_py-0.4.1/Cargo.toml
--rw-r--r--   0        0        0      615 1970-01-01 00:00:00.000000 sideko_py-0.4.1/pyproject.toml
--rw-r--r--   0      501       20     3860 2024-04-22 13:43:15.000000 sideko_py-0.4.1/LICENSE
--rw-r--r--   0        0        0     2271 1970-01-01 00:00:00.000000 sideko_py-0.4.1/PKG-INFO
+-rw-r--r--   0      501       20      484 2024-05-21 21:55:30.000000 sideko_py-0.5.0/sideko-api/Cargo.toml
+-rw-r--r--   0      501       20     3778 2024-05-21 21:55:30.000000 sideko_py-0.5.0/sideko-api/README.md
+-rw-r--r--   0      501       20     3169 2024-05-21 21:55:30.000000 sideko_py-0.5.0/sideko-api/src/auth.rs
+-rw-r--r--   0      501       20    12846 2024-05-21 21:55:30.000000 sideko_py-0.5.0/sideko-api/src/blocking.rs
+-rw-r--r--   0      501       20     1492 2024-05-21 21:55:30.000000 sideko_py-0.5.0/sideko-api/src/error_enums.rs
+-rw-r--r--   0      501       20    13555 2024-05-21 21:55:30.000000 sideko_py-0.5.0/sideko-api/src/lib.rs
+-rw-r--r--   0      501       20      888 2024-05-21 21:55:30.000000 sideko_py-0.5.0/sideko-api/src/request_types.rs
+-rw-r--r--   0      501       20      996 2024-05-21 21:55:30.000000 sideko_py-0.5.0/sideko-api/src/result.rs
+-rw-r--r--   0      501       20     4220 2024-05-21 21:55:30.000000 sideko_py-0.5.0/sideko-api/src/schemas.rs
+-rw-r--r--   0      501       20      850 2024-05-21 21:55:30.000000 sideko_py-0.5.0/core/Cargo.toml
+-rw-r--r--   0      501       20     8114 2024-05-21 21:55:30.000000 sideko_py-0.5.0/core/src/cli.rs
+-rw-r--r--   0      501       20     3995 2024-05-21 21:55:30.000000 sideko_py-0.5.0/core/src/cmds/apis.rs
+-rw-r--r--   0      501       20     4657 2024-05-21 21:55:30.000000 sideko_py-0.5.0/core/src/cmds/generate.rs
+-rw-r--r--   0      501       20     3492 2024-05-21 21:55:30.000000 sideko_py-0.5.0/core/src/cmds/login.rs
+-rw-r--r--   0      501       20       47 2024-05-21 21:55:30.000000 sideko_py-0.5.0/core/src/cmds/mod.rs
+-rw-r--r--   0      501       20     2011 2024-05-21 21:55:30.000000 sideko_py-0.5.0/core/src/config.rs
+-rw-r--r--   0      501       20     1264 2024-05-21 21:55:30.000000 sideko_py-0.5.0/core/src/html/failure.html
+-rw-r--r--   0      501       20     1216 2024-05-21 21:55:30.000000 sideko_py-0.5.0/core/src/html/success.html
+-rw-r--r--   0      501       20       90 2024-05-21 21:55:30.000000 sideko_py-0.5.0/core/src/lib.rs
+-rw-r--r--   0      501       20      203 2024-05-21 21:55:30.000000 sideko_py-0.5.0/core/src/main.rs
+-rw-r--r--   0      501       20     1850 2024-05-21 21:55:30.000000 sideko_py-0.5.0/core/src/result.rs
+-rw-r--r--   0      501       20     1060 2024-05-21 21:55:30.000000 sideko_py-0.5.0/core/src/styles.rs
+-rw-r--r--   0      501       20     3176 2024-05-21 21:55:30.000000 sideko_py-0.5.0/core/src/utils.rs
+-rw-r--r--   0        0        0      481 1970-01-01 00:00:00.000000 sideko_py-0.5.0/sideko-py/Cargo.toml
+-rw-r--r--   0      501       20     3860 2024-05-21 21:55:30.000000 sideko_py-0.5.0/sideko-py/LICENSE
+-rw-r--r--   0      501       20     1640 2024-05-21 21:55:30.000000 sideko_py-0.5.0/sideko-py/README.md
+-rw-r--r--   0      501       20     2334 2024-05-21 21:55:30.000000 sideko_py-0.5.0/sideko-py/src/lib.rs
+-rw-r--r--   0      501       20    63164 2024-05-21 21:55:30.000000 sideko_py-0.5.0/Cargo.lock
+-rw-r--r--   0        0        0      297 1970-01-01 00:00:00.000000 sideko_py-0.5.0/Cargo.toml
+-rw-r--r--   0        0        0      615 1970-01-01 00:00:00.000000 sideko_py-0.5.0/pyproject.toml
+-rw-r--r--   0      501       20     3860 2024-05-21 21:55:30.000000 sideko_py-0.5.0/LICENSE
+-rw-r--r--   0        0        0     2271 1970-01-01 00:00:00.000000 sideko_py-0.5.0/PKG-INFO
```

### Comparing `sideko_py-0.4.1/core/Cargo.toml` & `sideko_py-0.5.0/core/Cargo.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "sideko"
-version = "0.4.1"
+version = "0.5.0"
 edition = "2021"
 authors = [
     "Elias Posen <elias@sideko.dev>",
     "Patrick Kelly <patrick@sideko.dev>",
 ]
 
 [target.x86_64-unknown-linux-musl.dependencies]
@@ -33,7 +33,8 @@
 rocket = "0.5.0"
 serde = "1.0.196"
 serde_json = "1.0.113"
 serde_yaml = "0.9.31"
 tar = "0.4.40"
 tokio = { version = "1.35.1", features = ["time"] }
 url = "2.4.1"
+uuid = "1.8.0"
```

### Comparing `sideko_py-0.4.1/core/src/cli.rs` & `sideko_py-0.5.0/core/src/cli.rs`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 use crate::{
-    cmds::{self, generate::OpenApiSource},
+    cmds::{
+        self,
+        generate::{load_openapi, OpenApiSource},
+    },
     config, result, styles, utils,
 };
 use clap::{Parser, Subcommand, ValueEnum};
-use sideko_api::schemas as sideko_schemas;
+use sideko_api::schemas::{self as sideko_schemas, NewApiVersion};
+
 use std::{path::PathBuf, str::FromStr};
 
 #[derive(Debug, Clone)]
 pub struct GenerationLanguageClap {
     inner: sideko_schemas::GenerationLanguageEnum,
 }
 impl ValueEnum for GenerationLanguageClap {
@@ -80,15 +84,24 @@
 enum Commands {
     /// Log into Sideko interactively to obtain API key for generations
     Login {
         #[arg(long, short)]
         /// Path to file to store API key, default: $HOME/.sideko
         output: Option<PathBuf>,
     },
-    /// Generate a SDK client
+    /// Generate and configure SDK clients
+    #[command(subcommand)]
+    Sdk(SdkCommands),
+    /// Manage API specifications in the Sideko Portal
+    #[command(subcommand)]
+    Api(ApiCommands),
+}
+
+#[derive(Debug, Subcommand)]
+enum SdkCommands {
     Generate {
         /// Path or URL of OpenAPI spec
         openapi_source: String,
         /// Programming language to generate
         language: GenerationLanguageClap,
         #[arg(long, short)]
         /// Output path of generated source files, default: ./
@@ -98,14 +111,29 @@
         base_url: Option<String>,
         #[arg(long, short)]
         /// Name of SDK package to generate
         package_name: Option<String>,
     },
 }
 
+#[derive(Debug, Subcommand)]
+enum ApiCommands {
+    List {},
+    Create {
+        openapi_source: String,
+        semver: String,
+        title: Option<String>,
+    },
+    NewVersion {
+        api_id: uuid::Uuid,
+        openapi_source: String,
+        semver: String,
+    },
+}
+
 pub async fn cli(args: Vec<String>) -> result::Result<()> {
     let cli = Cli::parse_from(args);
 
     // set up logger
     let level = if cli.quiet {
         log::Level::Error
     } else if cli.verbose {
@@ -113,48 +141,52 @@
     } else {
         log::Level::Info
     };
     utils::init_logger(level);
     config::load_config(config::config_bufs(vec![cli.config]));
 
     let cmd_res = match &cli.command {
-        Commands::Generate {
-            openapi_source,
-            language,
-            output,
-            base_url,
-            package_name,
-        } => {
-            // Set defaults
-            let destination = if let Some(o) = output {
-                o.clone()
-            } else {
-                std::env::current_dir().map_err(|e| {
-                    log::debug!("CWD failure: {e}");
-                    result::Error::general("Failed determining cwd for --output default")
-                })?
-            };
-
-            // Construct cmd input params
-            let params = cmds::generate::GenerateSdkParams {
-                source: cmds::generate::OpenApiSource::from(openapi_source),
-                destination,
-                language: language.inner.clone(),
-                base_url: base_url.clone(),
-                package_name: package_name.clone(),
-            };
+        Commands::Sdk(sdk_command) => {
+            match sdk_command {
+                SdkCommands::Generate {
+                    openapi_source,
+                    language,
+                    output,
+                    base_url,
+                    package_name,
+                } => {
+                    // Set defaults
+                    let destination = if let Some(o) = output {
+                        o.clone()
+                    } else {
+                        std::env::current_dir().map_err(|e| {
+                            log::debug!("CWD failure: {e}");
+                            result::Error::general("Failed determining cwd for --output default")
+                        })?
+                    };
+
+                    // Construct cmd input params
+                    let params = cmds::generate::GenerateSdkParams {
+                        source: cmds::generate::OpenApiSource::from(openapi_source),
+                        destination,
+                        language: language.inner.clone(),
+                        base_url: base_url.clone(),
+                        package_name: package_name.clone(),
+                    };
+
+                    if let OpenApiSource::Raw(_) = params.source {
+                        log::error!("Unable to parse OpenAPI as a URL or Path");
+                        return Err(result::Error::general(
+                            "Unable to parse OpenAPI as a URL or Path",
+                        ));
+                    };
 
-            if let OpenApiSource::Raw(_) = params.source {
-                log::error!("Unable to parse OpenAPI as a URL or Path");
-                return Err(result::Error::general(
-                    "Unable to parse OpenAPI as a URL or Path",
-                ));
-            };
-
-            cmds::generate::handle_generate(&params).await
+                    cmds::generate::handle_generate(&params).await
+                }
+            }
         }
         Commands::Login { output } => {
             // Set defaults
             let output_path = if let Some(o) = output {
                 o.clone()
             } else {
                 let home = std::env::var("HOME")
@@ -163,14 +195,47 @@
                     .map_err(|_| result::Error::general("Unable to build default --output path"))?;
                 utf_buf.push(".sideko");
                 utf_buf
             };
 
             cmds::login::handle_login(output_path).await
         }
+        Commands::Api(api_command) => match api_command {
+            ApiCommands::List {} => cmds::apis::handle_list_apis().await,
+            ApiCommands::Create {
+                openapi_source,
+                semver,
+                title,
+            } => {
+                cmds::apis::create_new_api_project(
+                    &NewApiVersion {
+                        semver: semver.clone(),
+                        openapi: load_openapi(&cmds::generate::OpenApiSource::from(openapi_source))
+                            .await?,
+                    },
+                    title.clone(),
+                )
+                .await
+            }
+            ApiCommands::NewVersion {
+                api_id,
+                openapi_source,
+                semver,
+            } => {
+                cmds::apis::create_new_api_project_version(
+                    *api_id,
+                    &NewApiVersion {
+                        openapi: load_openapi(&cmds::generate::OpenApiSource::from(openapi_source))
+                            .await?,
+                        semver: semver.clone(),
+                    },
+                )
+                .await
+            }
+        },
     };
 
     if let Err(e) = &cmd_res {
         if let Some(debug_msg) = e.debug_msg() {
             log::debug!("{debug_msg}");
         }
         log::error!("{}", e.error_msg());
```

### Comparing `sideko_py-0.4.1/core/src/cmds/generate.rs` & `sideko_py-0.5.0/core/src/cmds/generate.rs`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
 #[derive(Serialize, Deserialize)]
 struct SidekoApiErr {
     message: String,
     data: Option<serde_json::Value>,
 }
 
-async fn load_openapi(source: &OpenApiSource) -> Result<String> {
+pub async fn load_openapi(source: &OpenApiSource) -> Result<String> {
     match source {
         OpenApiSource::Url(url) => {
             debug!("Loading OpenAPI spec from url: {url}");
             let response = reqwest::get(url.to_string()).await.map_err(|e| {
                 Error::arg_with_debug(
                     &format!("Failed loading OpenAPI spec from {url}"),
                     &format!("Send err: {e}"),
```

### Comparing `sideko_py-0.4.1/core/src/cmds/login.rs` & `sideko_py-0.5.0/core/src/cmds/login.rs`

 * *Files identical despite different names*

### Comparing `sideko_py-0.4.1/core/src/config.rs` & `sideko_py-0.5.0/core/src/config.rs`

 * *Files identical despite different names*

### Comparing `sideko_py-0.4.1/core/src/html/failure.html` & `sideko_py-0.5.0/core/src/html/failure.html`

 * *Files identical despite different names*

### Comparing `sideko_py-0.4.1/core/src/html/success.html` & `sideko_py-0.5.0/core/src/html/success.html`

 * *Files identical despite different names*

### Comparing `sideko_py-0.4.1/core/src/result.rs` & `sideko_py-0.5.0/core/src/result.rs`

 * *Files identical despite different names*

### Comparing `sideko_py-0.4.1/core/src/styles.rs` & `sideko_py-0.5.0/core/src/styles.rs`

 * *Files identical despite different names*

### Comparing `sideko_py-0.4.1/core/src/utils.rs` & `sideko_py-0.5.0/core/src/utils.rs`

 * *Files identical despite different names*

### Comparing `sideko_py-0.4.1/sideko-api/src/auth.rs` & `sideko_py-0.5.0/sideko-api/src/auth.rs`

 * *Files identical despite different names*

### Comparing `sideko_py-0.4.1/sideko-api/src/result.rs` & `sideko_py-0.5.0/sideko-api/src/result.rs`

 * *Files 23% similar despite different names*

```diff
@@ -1,42 +1,27 @@
 ///Generated by Sideko (sideko.dev)
 #[derive(Debug, thiserror::Error)]
 pub enum Error<T> {
     #[error("Failed serializing json: {0} ")]
     Serialize(serde_json::Error),
     #[error("Failed sending http request: {0}")]
     Dispatch(reqwest::Error),
-    #[error("Failed deserializing json into {expected_signature:?}: {serde_err:?} ")]
-    UnexpectedResponseBody {
-        status_code: u16,
-        method: String,
-        url: String,
-        response_text: String,
-        expected_signature: String,
-        serde_err: serde_json::Error,
-    },
-    #[error(
-        "Unexpected status {status_code:?}, handlers set up for {expected_status_codes:?}"
-    )]
-    BlockingUnexpectedStatus {
+    #[error("Api Error status:{status_code:?}")]
+    BlockingApiError {
         status_code: u16,
         method: String,
         url: String,
         response: reqwest::blocking::Response,
-        expected_status_codes: Vec<String>,
     },
-    #[error(
-        "Unexpected status {status_code:?}, handlers set up for {expected_status_codes:?}"
-    )]
-    UnexpectedStatus {
+    #[error("Api Error status:{status_code:?}")]
+    ApiError {
         status_code: u16,
         method: String,
         url: String,
         response: reqwest::Response,
-        expected_status_codes: Vec<String>,
     },
     #[error("Response returned unsuccessful status code: {status_code:?}")]
     Response { status_code: u16, method: String, url: String, data: T },
     #[error("Failed extracting bytes from response: {0}")]
     ResponseBytes(reqwest::Error),
     #[error("Failed reading file: {0}")]
     File(std::io::Error),
```

### Comparing `sideko_py-0.4.1/sideko-api/src/schemas.rs` & `sideko_py-0.5.0/sideko-api/src/schemas.rs`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,89 @@
 pub struct BinaryResponse {
     pub content: bytes::Bytes,
 }
 #[derive(serde::Serialize, serde::Deserialize, Debug, Default, Clone)]
+pub struct ApiProject {
+    pub created_at: String,
+    pub id: String,
+    pub title: String,
+}
+#[derive(serde::Serialize, serde::Deserialize, Debug, Default, Clone)]
+pub struct Error {
+    pub description: String,
+    pub error: ErrorCodeEnum,
+}
+#[derive(serde::Serialize, serde::Deserialize, Debug, Default, Clone)]
+pub struct ApiVersion {
+    pub api_project_id: String,
+    pub created_at: String,
+    pub id: String,
+    pub semver: String,
+}
+#[derive(serde::Serialize, serde::Deserialize, Debug, Default, Clone)]
 pub struct ApiKey {
     pub api_key: String,
 }
 #[derive(serde::Serialize, serde::Deserialize, Debug, Default, Clone)]
 pub struct CliUpdate {
     pub message: String,
     pub severity: CliUpdateSeverityEnum,
 }
 #[derive(serde::Serialize, serde::Deserialize, Debug, Default, Clone)]
+pub struct NewApiProject {
+    pub title: String,
+}
+#[derive(serde::Serialize, serde::Deserialize, Debug, Default, Clone)]
+pub struct NewApiVersion {
+    pub openapi: String,
+    pub semver: String,
+}
+#[derive(serde::Serialize, serde::Deserialize, Debug, Default, Clone)]
 pub struct StatelessGenerateSdk {
     #[serde(skip_serializing_if = "Option::is_none")]
     pub base_url: Option<String>,
     pub language: GenerationLanguageEnum,
     pub openapi: String,
     #[serde(skip_serializing_if = "Option::is_none")]
     pub package_name: Option<String>,
 }
 #[derive(serde::Serialize, serde::Deserialize, Debug, Default, Clone)]
-pub struct Error {
-    pub description: String,
-    pub error: ErrorCodeEnum,
+pub enum ErrorCodeEnum {
+    #[default]
+    #[serde(rename = "forbidden")]
+    Forbidden,
+    #[serde(rename = "unauthorized")]
+    Unauthorized,
+    #[serde(rename = "not_found")]
+    NotFound,
+    #[serde(rename = "internal_server_error")]
+    InternalServerError,
+    #[serde(rename = "Bad Request")]
+    BadRequest,
+    #[serde(rename = "unavailable_subdomain")]
+    UnavailableSubdomain,
+    #[serde(rename = "invalid_openapi")]
+    InvalidOpenapi,
+    #[serde(rename = "invalid_url")]
+    InvalidUrl,
+}
+impl std::fmt::Display for ErrorCodeEnum {
+    fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
+        let str_val = match self {
+            ErrorCodeEnum::Forbidden => "forbidden",
+            ErrorCodeEnum::Unauthorized => "unauthorized",
+            ErrorCodeEnum::NotFound => "not_found",
+            ErrorCodeEnum::InternalServerError => "internal_server_error",
+            ErrorCodeEnum::BadRequest => "Bad Request",
+            ErrorCodeEnum::UnavailableSubdomain => "unavailable_subdomain",
+            ErrorCodeEnum::InvalidOpenapi => "invalid_openapi",
+            ErrorCodeEnum::InvalidUrl => "invalid_url",
+        };
+        write!(f, "{}", str_val)
+    }
 }
 #[derive(serde::Serialize, serde::Deserialize, Debug, Default, Clone)]
 pub enum CliUpdateSeverityEnum {
     #[default]
     #[serde(rename = "info")]
     Info,
     #[serde(rename = "suggested")]
@@ -66,42 +123,7 @@
             GenerationLanguageEnum::Rust => "rust",
             GenerationLanguageEnum::Ruby => "ruby",
             GenerationLanguageEnum::Typescript => "typescript",
         };
         write!(f, "{}", str_val)
     }
 }
-#[derive(serde::Serialize, serde::Deserialize, Debug, Default, Clone)]
-pub enum ErrorCodeEnum {
-    #[default]
-    #[serde(rename = "forbidden")]
-    Forbidden,
-    #[serde(rename = "unauthorized")]
-    Unauthorized,
-    #[serde(rename = "not_found")]
-    NotFound,
-    #[serde(rename = "internal_server_error")]
-    InternalServerError,
-    #[serde(rename = "Bad Request")]
-    BadRequest,
-    #[serde(rename = "unavailable_subdomain")]
-    UnavailableSubdomain,
-    #[serde(rename = "invalid_openapi")]
-    InvalidOpenapi,
-    #[serde(rename = "invalid_url")]
-    InvalidUrl,
-}
-impl std::fmt::Display for ErrorCodeEnum {
-    fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
-        let str_val = match self {
-            ErrorCodeEnum::Forbidden => "forbidden",
-            ErrorCodeEnum::Unauthorized => "unauthorized",
-            ErrorCodeEnum::NotFound => "not_found",
-            ErrorCodeEnum::InternalServerError => "internal_server_error",
-            ErrorCodeEnum::BadRequest => "Bad Request",
-            ErrorCodeEnum::UnavailableSubdomain => "unavailable_subdomain",
-            ErrorCodeEnum::InvalidOpenapi => "invalid_openapi",
-            ErrorCodeEnum::InvalidUrl => "invalid_url",
-        };
-        write!(f, "{}", str_val)
-    }
-}
```

### Comparing `sideko_py-0.4.1/sideko-py/LICENSE` & `sideko_py-0.5.0/sideko-py/LICENSE`

 * *Files identical despite different names*

### Comparing `sideko_py-0.4.1/sideko-py/README.md` & `sideko_py-0.5.0/sideko-py/README.md`

 * *Files identical despite different names*

### Comparing `sideko_py-0.4.1/sideko-py/src/lib.rs` & `sideko_py-0.5.0/sideko-py/src/lib.rs`

 * *Files identical despite different names*

### Comparing `sideko_py-0.4.1/Cargo.lock` & `sideko_py-0.5.0/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1659,15 +1659,15 @@
 checksum = "f40ca3c46823713e0d4209592e8d6e826aa57e928f09752619fc696c499637f6"
 dependencies = [
  "lazy_static",
 ]
 
 [[package]]
 name = "sideko"
-version = "0.4.1"
+version = "0.5.0"
 dependencies = [
  "anstyle",
  "bytes",
  "camino",
  "clap",
  "dotenv",
  "env_logger",
@@ -1681,19 +1681,20 @@
  "serde",
  "serde_json",
  "serde_yaml",
  "sideko_api",
  "tar",
  "tokio",
  "url",
+ "uuid",
 ]
 
 [[package]]
 name = "sideko-py"
-version = "0.4.1"
+version = "0.5.0"
 dependencies = [
  "log",
  "pyo3",
  "sideko",
  "sideko_api",
  "tokio",
 ]
@@ -2187,14 +2188,20 @@
 [[package]]
 name = "utf8parse"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "711b9620af191e0cdc7468a8d14e709c3dcdb115b36f838e601583af800a370a"
 
 [[package]]
+name = "uuid"
+version = "1.8.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a183cf7feeba97b4dd1c0d46788634f6221d87fa961b305bed08c851829efcc0"
+
+[[package]]
 name = "valuable"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "830b7e5d4d90034032940e4ace0d9a9a057e7a45cd94e6c007832e39edb82f6d"
 
 [[package]]
 name = "vcpkg"
```

### Comparing `sideko_py-0.4.1/pyproject.toml` & `sideko_py-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sideko_py-0.4.1/LICENSE` & `sideko_py-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sideko_py-0.4.1/PKG-INFO` & `sideko_py-0.5.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: sideko-py
-Version: 0.4.1
+Version: 0.5.0
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Framework :: FastAPI
 Classifier: Framework :: Flask
 License-File: LICENSE
```

