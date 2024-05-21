# Comparing `tmp/pulumi_pulumiservice-0.9.0.tar.gz` & `tmp/pulumi_pulumiservice-0.9.1a1689804796.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_pulumiservice-0.9.0.tar", last modified: Tue Jun  6 22:38:10 2023, max compression
+gzip compressed data, was "dist/pulumi_pulumiservice-0.9.1a1689804796.tar", last modified: Wed Jul 19 22:16:47 2023, max compression
```

## Comparing `pulumi_pulumiservice-0.9.0.tar` & `pulumi_pulumiservice-0.9.1a1689804796.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 22:38:10.457866 pulumi_pulumiservice-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)     5118 2023-06-06 22:38:10.457866 pulumi_pulumiservice-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-06-06 22:38:10.000000 pulumi_pulumiservice-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 22:38:10.457866 pulumi_pulumiservice-0.9.0/pulumi_pulumiservice/
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-06 22:38:10.000000 pulumi_pulumiservice-0.9.0/pulumi_pulumiservice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-06-06 22:38:10.000000 pulumi_pulumiservice-0.9.0/pulumi_pulumiservice/_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    29328 2023-06-06 22:38:10.000000 pulumi_pulumiservice-0.9.0/pulumi_pulumiservice/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8050 2023-06-06 22:38:10.000000 pulumi_pulumiservice-0.9.0/pulumi_pulumiservice/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-06-06 22:38:10.000000 pulumi_pulumiservice-0.9.0/pulumi_pulumiservice/access_token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 22:38:10.457866 pulumi_pulumiservice-0.9.0/pulumi_pulumiservice/config/
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-06 22:38:10.000000 pulumi_pulumiservice-0.9.0/pulumi_pulumiservice/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-06-06 22:38:10.000000 pulumi_pulumiservice-0.9.0/pulumi_pulumiservice/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    12337 2023-06-06 22:38:10.000000 pulumi_pulumiservice-0.9.0/pulumi_pulumiservice/deployment_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     7511 2023-06-06 22:38:10.000000 pulumi_pulumiservice-0.9.0/pulumi_pulumiservice/org_access_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-06-06 22:38:10.000000 pulumi_pulumiservice-0.9.0/pulumi_pulumiservice/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-06 22:38:10.000000 pulumi_pulumiservice-0.9.0/pulumi_pulumiservice/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 22:38:10.000000 pulumi_pulumiservice-0.9.0/pulumi_pulumiservice/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8636 2023-06-06 22:38:10.000000 pulumi_pulumiservice-0.9.0/pulumi_pulumiservice/stack_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)    10473 2023-06-06 22:38:10.000000 pulumi_pulumiservice-0.9.0/pulumi_pulumiservice/team.py
--rw-r--r--   0 runner    (1001) docker     (123)     8903 2023-06-06 22:38:10.000000 pulumi_pulumiservice-0.9.0/pulumi_pulumiservice/team_access_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-06-06 22:38:10.000000 pulumi_pulumiservice-0.9.0/pulumi_pulumiservice/team_stack_permission.py
--rw-r--r--   0 runner    (1001) docker     (123)    17280 2023-06-06 22:38:10.000000 pulumi_pulumiservice-0.9.0/pulumi_pulumiservice/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 22:38:10.457866 pulumi_pulumiservice-0.9.0/pulumi_pulumiservice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5118 2023-06-06 22:38:10.000000 pulumi_pulumiservice-0.9.0/pulumi_pulumiservice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-06-06 22:38:10.000000 pulumi_pulumiservice-0.9.0/pulumi_pulumiservice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 22:38:10.000000 pulumi_pulumiservice-0.9.0/pulumi_pulumiservice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 22:38:10.000000 pulumi_pulumiservice-0.9.0/pulumi_pulumiservice.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-06 22:38:10.000000 pulumi_pulumiservice-0.9.0/pulumi_pulumiservice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-06 22:38:10.000000 pulumi_pulumiservice-0.9.0/pulumi_pulumiservice.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 22:38:10.457866 pulumi_pulumiservice-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-06-06 22:38:10.000000 pulumi_pulumiservice-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 22:16:47.000000 pulumi_pulumiservice-0.9.1a1689804796/
+-rw-r--r--   0 runner    (1001) docker     (123)     5916 2023-07-19 22:16:47.000000 pulumi_pulumiservice-0.9.1a1689804796/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-07-19 22:16:46.000000 pulumi_pulumiservice-0.9.1a1689804796/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 22:16:47.000000 pulumi_pulumiservice-0.9.1a1689804796/pulumi_pulumiservice/
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-07-19 22:16:46.000000 pulumi_pulumiservice-0.9.1a1689804796/pulumi_pulumiservice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-07-19 22:16:46.000000 pulumi_pulumiservice-0.9.1a1689804796/pulumi_pulumiservice/_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29328 2023-07-19 22:16:46.000000 pulumi_pulumiservice-0.9.1a1689804796/pulumi_pulumiservice/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8050 2023-07-19 22:16:46.000000 pulumi_pulumiservice-0.9.1a1689804796/pulumi_pulumiservice/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-07-19 22:16:46.000000 pulumi_pulumiservice-0.9.1a1689804796/pulumi_pulumiservice/access_token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 22:16:47.000000 pulumi_pulumiservice-0.9.1a1689804796/pulumi_pulumiservice/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-19 22:16:46.000000 pulumi_pulumiservice-0.9.1a1689804796/pulumi_pulumiservice/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-19 22:16:46.000000 pulumi_pulumiservice-0.9.1a1689804796/pulumi_pulumiservice/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12337 2023-07-19 22:16:46.000000 pulumi_pulumiservice-0.9.1a1689804796/pulumi_pulumiservice/deployment_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7511 2023-07-19 22:16:46.000000 pulumi_pulumiservice-0.9.1a1689804796/pulumi_pulumiservice/org_access_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-07-19 22:16:46.000000 pulumi_pulumiservice-0.9.1a1689804796/pulumi_pulumiservice/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-19 22:16:46.000000 pulumi_pulumiservice-0.9.1a1689804796/pulumi_pulumiservice/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 22:16:46.000000 pulumi_pulumiservice-0.9.1a1689804796/pulumi_pulumiservice/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8636 2023-07-19 22:16:46.000000 pulumi_pulumiservice-0.9.1a1689804796/pulumi_pulumiservice/stack_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12327 2023-07-19 22:16:46.000000 pulumi_pulumiservice-0.9.1a1689804796/pulumi_pulumiservice/team.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8903 2023-07-19 22:16:46.000000 pulumi_pulumiservice-0.9.1a1689804796/pulumi_pulumiservice/team_access_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-07-19 22:16:46.000000 pulumi_pulumiservice-0.9.1a1689804796/pulumi_pulumiservice/team_stack_permission.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17280 2023-07-19 22:16:46.000000 pulumi_pulumiservice-0.9.1a1689804796/pulumi_pulumiservice/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 22:16:47.000000 pulumi_pulumiservice-0.9.1a1689804796/pulumi_pulumiservice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5916 2023-07-19 22:16:47.000000 pulumi_pulumiservice-0.9.1a1689804796/pulumi_pulumiservice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-07-19 22:16:47.000000 pulumi_pulumiservice-0.9.1a1689804796/pulumi_pulumiservice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 22:16:47.000000 pulumi_pulumiservice-0.9.1a1689804796/pulumi_pulumiservice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 22:16:47.000000 pulumi_pulumiservice-0.9.1a1689804796/pulumi_pulumiservice.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-19 22:16:47.000000 pulumi_pulumiservice-0.9.1a1689804796/pulumi_pulumiservice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-19 22:16:47.000000 pulumi_pulumiservice-0.9.1a1689804796/pulumi_pulumiservice.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 22:16:47.000000 pulumi_pulumiservice-0.9.1a1689804796/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-07-19 22:16:46.000000 pulumi_pulumiservice-0.9.1a1689804796/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `pulumi_pulumiservice-0.9.0/PKG-INFO` & `pulumi_pulumiservice-0.9.1a1689804796/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: pulumi_pulumiservice
-Version: 0.9.0
-Summary: A native Pulumi package for creating and managing Pulumi Cloud constructs
-Home-page: https://pulumi.com
-License: Apache-2.0
-Project-URL: Repository, https://github.com/pulumi/pulumi-pulumiservice
-Keywords: pulumi kind/native category/infrastructure
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-
 # Pulumi Service Provider
 
 [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
 [![NPM version](https://badge.fury.io/js/%40pulumi%2Fpulumiservice.svg)](https://www.npmjs.com/package/@pulumi/pulumiservice)
 [![Python version](https://badge.fury.io/py/pulumi-pulumiservice.svg)](https://pypi.org/project/pulumi-pulumiservice)
 [![NuGet version](https://badge.fury.io/nu/pulumi.pulumiservice.svg)](https://badge.fury.io/nu/pulumi.pulumiservice)
 [![PkgGoDev](https://pkg.go.dev/badge/github.com/pulumi/pulumi-pulumiservice/sdk/go/pulumiservice)](https://pkg.go.dev/github.com/pulumi/pulumi-pulumiservice/sdk/go)
@@ -102,9 +91,7 @@
     ],
 });
 
 export const members = team.members;
 ```
 
 Check out the [examples/](examples/) directory for more examples.
-
-
```

### Comparing `pulumi_pulumiservice-0.9.0/README.md` & `pulumi_pulumiservice-0.9.1a1689804796/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,97 +1,108 @@
-# Pulumi Service Provider
-
-[![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
-[![NPM version](https://badge.fury.io/js/%40pulumi%2Fpulumiservice.svg)](https://www.npmjs.com/package/@pulumi/pulumiservice)
-[![Python version](https://badge.fury.io/py/pulumi-pulumiservice.svg)](https://pypi.org/project/pulumi-pulumiservice)
-[![NuGet version](https://badge.fury.io/nu/pulumi.pulumiservice.svg)](https://badge.fury.io/nu/pulumi.pulumiservice)
-[![PkgGoDev](https://pkg.go.dev/badge/github.com/pulumi/pulumi-pulumiservice/sdk/go/pulumiservice)](https://pkg.go.dev/github.com/pulumi/pulumi-pulumiservice/sdk/go)
-[![License](https://img.shields.io/npm/l/%40pulumi%2Fpulumiservice.svg)](https://github.com/pulumi/pulumi-pulumiservice/blob/main/LICENSE)
-
-A Pulumi Resource Provider for The Pulumi Service.
-
-The Pulumi Service Provider is built on top of the [Pulumi Service REST API](https://pulumi.com/docs/reference/service-rest-api) which is another feature available to our customers to programmatically configuring the Pulumi Service. The Pulumi Service REST API includes functionality to interact with and manipulate any kind of metadata managed by Pulumi. That includes Projects and Stacks, Previews and Updates, Organizations and Audit Logs. We have already seen Cloud Engineering teams using the Pulumi REST API to build all sorts of custom functionality. These new capabilities are especially powerful when used in combination with the [Automation API](https://pulumi.com/automation).
-
-#### Supported Resources
-
-- [Webhooks](https://pulumi.com/docs/intro/pulumi-service/webhooks)
-- [Teams](https://pulumi.com/docs/intro/pulumi-service/teams)
-  - You can grant a team access to stacks via the `TeamStackPermission` resource
-- [StackTags](https://pulumi.com/docs/reference/cli/pulumi_stack_tag)
-- [AccessTokens](https://pulumi.com/docs/intro/pulumi-service/accounts)
-
-For reference documentation, visit the [Pulumi Service API Documentation](https://www.pulumi.com/registry/packages/pulumiservice/api-docs/) on the [Pulumi Registry](https://www.pulumi.com/registry/packages/pulumiservice/)
-
-## Installing
-
-This package is available in many languages in the standard packaging formats.
-
-### Node.js (Java/TypeScript)
-
-To use from JavaScript or TypeScript in Node.js, install using either `npm`:
-
-    $ npm install @pulumi/pulumiservice
-
-or `yarn`:
-
-    $ yarn add @pulumi/pulumiservice
-
-### Python
-
-To use from Python, install using `pip`:
-
-    $ pip install pulumi_pulumiservice
-
-### Go
-
-To use from Go, use `go get` to grab the latest version of the library
-
-    $ go get github.com/pulumi/pulumi-pulumiservice/sdk/go
-
-### .NET
-
-To use from .NET, install using `dotnet add package`:
-
-    $ dotnet add package Pulumi.PulumiService
-
-## Setup
-
-Ensure that you have ran `pulumi login`. Run `pulumi whoami` to verify that you are logged in.
-
-### Configuration Options
-
-Use `pulumi config set pulumiservice:<option>` or pass options to the [constructor of `new pulumiservice.Provider`](https://pulumi.com/registry/packages/pulumiservice/api-docs/provider).
-
-| Option        | Environment Variable Name | Required/Optional | Description                                                                                                                                                                              |
-| ------------- | ------------------------- | ----------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-| `accessToken` | `PULUMI_ACCESS_TOKEN`     | Optional          | Overrides [Pulumi Service Access Tokens](https://www.pulumi.com/docs/intro/pulumi-service/accounts/#access-tokens)                                                                       |
-| `apiUrl`      | `PULUMI_BACKEND_URL`      | Optional          | Allows overriding default [Pulumi Service API URL](https://www.pulumi.com/docs/reference/service-rest-api) for [self hosted customers](https://www.pulumi.com/docs/guides/self-hosted/). |
-
-## Examples
-
-```typescript
-import * as aws from "@pulumi/awsx"
-import * as pulumi from "@pulumi/pulumi";
-import * as service from "@pulumi/pulumiservice";
-
-const team = new service.Team("team", {
-    name: "pulumi-service-team",
-    displayName: "Pulumi Service",
-    description: "The Pulumi Service Team",
-    organizationName: "pulumi",
-    teamType: "pulumi",
-    members: [
-        "piers",
-        "bryce",
-        "casey"
-        "evan",
-        "devon",
-        "meagan"
-        "myles",
-        "steve"
-    ],
-});
-
-export const members = team.members;
-```
-
-Check out the [examples/](examples/) directory for more examples.
+Metadata-Version: 2.1
+Name: pulumi_pulumiservice
+Version: 0.9.1a1689804796
+Summary: A native Pulumi package for creating and managing Pulumi Cloud constructs
+Home-page: https://pulumi.com
+License: Apache-2.0
+Project-URL: Repository, https://github.com/pulumi/pulumi-pulumiservice
+Description: # Pulumi Service Provider
+        
+        [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
+        [![NPM version](https://badge.fury.io/js/%40pulumi%2Fpulumiservice.svg)](https://www.npmjs.com/package/@pulumi/pulumiservice)
+        [![Python version](https://badge.fury.io/py/pulumi-pulumiservice.svg)](https://pypi.org/project/pulumi-pulumiservice)
+        [![NuGet version](https://badge.fury.io/nu/pulumi.pulumiservice.svg)](https://badge.fury.io/nu/pulumi.pulumiservice)
+        [![PkgGoDev](https://pkg.go.dev/badge/github.com/pulumi/pulumi-pulumiservice/sdk/go/pulumiservice)](https://pkg.go.dev/github.com/pulumi/pulumi-pulumiservice/sdk/go)
+        [![License](https://img.shields.io/npm/l/%40pulumi%2Fpulumiservice.svg)](https://github.com/pulumi/pulumi-pulumiservice/blob/main/LICENSE)
+        
+        A Pulumi Resource Provider for The Pulumi Service.
+        
+        The Pulumi Service Provider is built on top of the [Pulumi Service REST API](https://pulumi.com/docs/reference/service-rest-api) which is another feature available to our customers to programmatically configuring the Pulumi Service. The Pulumi Service REST API includes functionality to interact with and manipulate any kind of metadata managed by Pulumi. That includes Projects and Stacks, Previews and Updates, Organizations and Audit Logs. We have already seen Cloud Engineering teams using the Pulumi REST API to build all sorts of custom functionality. These new capabilities are especially powerful when used in combination with the [Automation API](https://pulumi.com/automation).
+        
+        #### Supported Resources
+        
+        - [Webhooks](https://pulumi.com/docs/intro/pulumi-service/webhooks)
+        - [Teams](https://pulumi.com/docs/intro/pulumi-service/teams)
+          - You can grant a team access to stacks via the `TeamStackPermission` resource
+        - [StackTags](https://pulumi.com/docs/reference/cli/pulumi_stack_tag)
+        - [AccessTokens](https://pulumi.com/docs/intro/pulumi-service/accounts)
+        
+        For reference documentation, visit the [Pulumi Service API Documentation](https://www.pulumi.com/registry/packages/pulumiservice/api-docs/) on the [Pulumi Registry](https://www.pulumi.com/registry/packages/pulumiservice/)
+        
+        ## Installing
+        
+        This package is available in many languages in the standard packaging formats.
+        
+        ### Node.js (Java/TypeScript)
+        
+        To use from JavaScript or TypeScript in Node.js, install using either `npm`:
+        
+            $ npm install @pulumi/pulumiservice
+        
+        or `yarn`:
+        
+            $ yarn add @pulumi/pulumiservice
+        
+        ### Python
+        
+        To use from Python, install using `pip`:
+        
+            $ pip install pulumi_pulumiservice
+        
+        ### Go
+        
+        To use from Go, use `go get` to grab the latest version of the library
+        
+            $ go get github.com/pulumi/pulumi-pulumiservice/sdk/go
+        
+        ### .NET
+        
+        To use from .NET, install using `dotnet add package`:
+        
+            $ dotnet add package Pulumi.PulumiService
+        
+        ## Setup
+        
+        Ensure that you have ran `pulumi login`. Run `pulumi whoami` to verify that you are logged in.
+        
+        ### Configuration Options
+        
+        Use `pulumi config set pulumiservice:<option>` or pass options to the [constructor of `new pulumiservice.Provider`](https://pulumi.com/registry/packages/pulumiservice/api-docs/provider).
+        
+        | Option        | Environment Variable Name | Required/Optional | Description                                                                                                                                                                              |
+        | ------------- | ------------------------- | ----------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+        | `accessToken` | `PULUMI_ACCESS_TOKEN`     | Optional          | Overrides [Pulumi Service Access Tokens](https://www.pulumi.com/docs/intro/pulumi-service/accounts/#access-tokens)                                                                       |
+        | `apiUrl`      | `PULUMI_BACKEND_URL`      | Optional          | Allows overriding default [Pulumi Service API URL](https://www.pulumi.com/docs/reference/service-rest-api) for [self hosted customers](https://www.pulumi.com/docs/guides/self-hosted/). |
+        
+        ## Examples
+        
+        ```typescript
+        import * as aws from "@pulumi/awsx"
+        import * as pulumi from "@pulumi/pulumi";
+        import * as service from "@pulumi/pulumiservice";
+        
+        const team = new service.Team("team", {
+            name: "pulumi-service-team",
+            displayName: "Pulumi Service",
+            description: "The Pulumi Service Team",
+            organizationName: "pulumi",
+            teamType: "pulumi",
+            members: [
+                "piers",
+                "bryce",
+                "casey"
+                "evan",
+                "devon",
+                "meagan"
+                "myles",
+                "steve"
+            ],
+        });
+        
+        export const members = team.members;
+        ```
+        
+        Check out the [examples/](examples/) directory for more examples.
+        
+Keywords: pulumi kind/native category/infrastructure
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
```

### Comparing `pulumi_pulumiservice-0.9.0/pulumi_pulumiservice/__init__.py` & `pulumi_pulumiservice-0.9.1a1689804796/pulumi_pulumiservice/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_pulumiservice-0.9.0/pulumi_pulumiservice/_enums.py` & `pulumi_pulumiservice-0.9.1a1689804796/pulumi_pulumiservice/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_pulumiservice-0.9.0/pulumi_pulumiservice/_inputs.py` & `pulumi_pulumiservice-0.9.1a1689804796/pulumi_pulumiservice/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_pulumiservice-0.9.0/pulumi_pulumiservice/_utilities.py` & `pulumi_pulumiservice-0.9.1a1689804796/pulumi_pulumiservice/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_pulumiservice-0.9.0/pulumi_pulumiservice/access_token.py` & `pulumi_pulumiservice-0.9.1a1689804796/pulumi_pulumiservice/access_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_pulumiservice-0.9.0/pulumi_pulumiservice/config/vars.py` & `pulumi_pulumiservice-0.9.1a1689804796/pulumi_pulumiservice/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_pulumiservice-0.9.0/pulumi_pulumiservice/deployment_settings.py` & `pulumi_pulumiservice-0.9.1a1689804796/pulumi_pulumiservice/deployment_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_pulumiservice-0.9.0/pulumi_pulumiservice/org_access_token.py` & `pulumi_pulumiservice-0.9.1a1689804796/pulumi_pulumiservice/org_access_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_pulumiservice-0.9.0/pulumi_pulumiservice/provider.py` & `pulumi_pulumiservice-0.9.1a1689804796/pulumi_pulumiservice/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_pulumiservice-0.9.0/pulumi_pulumiservice/stack_tag.py` & `pulumi_pulumiservice-0.9.1a1689804796/pulumi_pulumiservice/stack_tag.py`

 * *Files identical despite different names*

### Comparing `pulumi_pulumiservice-0.9.0/pulumi_pulumiservice/team.py` & `pulumi_pulumiservice-0.9.1a1689804796/pulumi_pulumiservice/team.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,56 +10,49 @@
 from . import _utilities
 
 __all__ = ['TeamArgs', 'Team']
 
 @pulumi.input_type
 class TeamArgs:
     def __init__(__self__, *,
-                 name: pulumi.Input[str],
                  organization_name: pulumi.Input[str],
                  team_type: pulumi.Input[str],
                  description: Optional[pulumi.Input[str]] = None,
                  display_name: Optional[pulumi.Input[str]] = None,
-                 members: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
+                 github_team_id: Optional[pulumi.Input[float]] = None,
+                 members: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 name: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a Team resource.
-        :param pulumi.Input[str] name: The team name.
-        :param pulumi.Input[str] organization_name: The organization's name.
+        :param pulumi.Input[str] organization_name: The name of the Pulumi organization the team belongs to.
         :param pulumi.Input[str] team_type: The type of team. Must be either `pulumi` or `github`.
         :param pulumi.Input[str] description: Optional. Team description.
         :param pulumi.Input[str] display_name: Optional. Team display name.
+        :param pulumi.Input[float] github_team_id: The GitHub ID of the team to mirror. Must be in the same GitHub organization that the Pulumi org is backed by. Required for "github" teams.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] members: List of team members.
+        :param pulumi.Input[str] name: The team's name. Required for "pulumi" teams.
         """
-        pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "organization_name", organization_name)
         pulumi.set(__self__, "team_type", team_type)
         if description is not None:
             pulumi.set(__self__, "description", description)
         if display_name is not None:
             pulumi.set(__self__, "display_name", display_name)
+        if github_team_id is not None:
+            pulumi.set(__self__, "github_team_id", github_team_id)
         if members is not None:
             pulumi.set(__self__, "members", members)
-
-    @property
-    @pulumi.getter
-    def name(self) -> pulumi.Input[str]:
-        """
-        The team name.
-        """
-        return pulumi.get(self, "name")
-
-    @name.setter
-    def name(self, value: pulumi.Input[str]):
-        pulumi.set(self, "name", value)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
 
     @property
     @pulumi.getter(name="organizationName")
     def organization_name(self) -> pulumi.Input[str]:
         """
-        The organization's name.
+        The name of the Pulumi organization the team belongs to.
         """
         return pulumi.get(self, "organization_name")
 
     @organization_name.setter
     def organization_name(self, value: pulumi.Input[str]):
         pulumi.set(self, "organization_name", value)
 
@@ -96,48 +89,74 @@
         return pulumi.get(self, "display_name")
 
     @display_name.setter
     def display_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "display_name", value)
 
     @property
+    @pulumi.getter(name="githubTeamId")
+    def github_team_id(self) -> Optional[pulumi.Input[float]]:
+        """
+        The GitHub ID of the team to mirror. Must be in the same GitHub organization that the Pulumi org is backed by. Required for "github" teams.
+        """
+        return pulumi.get(self, "github_team_id")
+
+    @github_team_id.setter
+    def github_team_id(self, value: Optional[pulumi.Input[float]]):
+        pulumi.set(self, "github_team_id", value)
+
+    @property
     @pulumi.getter
     def members(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
         List of team members.
         """
         return pulumi.get(self, "members")
 
     @members.setter
     def members(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "members", value)
 
+    @property
+    @pulumi.getter
+    def name(self) -> Optional[pulumi.Input[str]]:
+        """
+        The team's name. Required for "pulumi" teams.
+        """
+        return pulumi.get(self, "name")
+
+    @name.setter
+    def name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "name", value)
+
 
 class Team(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  display_name: Optional[pulumi.Input[str]] = None,
+                 github_team_id: Optional[pulumi.Input[float]] = None,
                  members: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  organization_name: Optional[pulumi.Input[str]] = None,
                  team_type: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         The Pulumi Cloud offers role-based access control (RBAC) using teams. Teams allow organization admins to assign a set of stack permissions to a group of users.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] description: Optional. Team description.
         :param pulumi.Input[str] display_name: Optional. Team display name.
+        :param pulumi.Input[float] github_team_id: The GitHub ID of the team to mirror. Must be in the same GitHub organization that the Pulumi org is backed by. Required for "github" teams.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] members: List of team members.
-        :param pulumi.Input[str] name: The team name.
-        :param pulumi.Input[str] organization_name: The organization's name.
+        :param pulumi.Input[str] name: The team's name. Required for "pulumi" teams.
+        :param pulumi.Input[str] organization_name: The name of the Pulumi organization the team belongs to.
         :param pulumi.Input[str] team_type: The type of team. Must be either `pulumi` or `github`.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: TeamArgs,
@@ -158,14 +177,15 @@
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  display_name: Optional[pulumi.Input[str]] = None,
+                 github_team_id: Optional[pulumi.Input[float]] = None,
                  members: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  organization_name: Optional[pulumi.Input[str]] = None,
                  team_type: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
@@ -173,17 +193,16 @@
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = TeamArgs.__new__(TeamArgs)
 
             __props__.__dict__["description"] = description
             __props__.__dict__["display_name"] = display_name
+            __props__.__dict__["github_team_id"] = github_team_id
             __props__.__dict__["members"] = members
-            if name is None and not opts.urn:
-                raise TypeError("Missing required property 'name'")
             __props__.__dict__["name"] = name
             if organization_name is None and not opts.urn:
                 raise TypeError("Missing required property 'organization_name'")
             __props__.__dict__["organization_name"] = organization_name
             if team_type is None and not opts.urn:
                 raise TypeError("Missing required property 'team_type'")
             __props__.__dict__["team_type"] = team_type
@@ -207,14 +226,15 @@
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = TeamArgs.__new__(TeamArgs)
 
         __props__.__dict__["description"] = None
         __props__.__dict__["display_name"] = None
+        __props__.__dict__["github_team_id"] = None
         __props__.__dict__["members"] = None
         __props__.__dict__["name"] = None
         __props__.__dict__["organization_name"] = None
         __props__.__dict__["team_type"] = None
         return Team(resource_name, opts=opts, __props__=__props__)
 
     @property
@@ -230,34 +250,42 @@
     def display_name(self) -> pulumi.Output[Optional[str]]:
         """
         Optional. Team display name.
         """
         return pulumi.get(self, "display_name")
 
     @property
+    @pulumi.getter(name="githubTeamId")
+    def github_team_id(self) -> pulumi.Output[Optional[float]]:
+        """
+        The GitHub ID of the team to mirror. Must be in the same GitHub organization that the Pulumi org is backed by. Required for "github" teams.
+        """
+        return pulumi.get(self, "github_team_id")
+
+    @property
     @pulumi.getter
     def members(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
         List of team members.
         """
         return pulumi.get(self, "members")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[Optional[str]]:
         """
-        The team name.
+        The team's name. Required for "pulumi" teams.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="organizationName")
     def organization_name(self) -> pulumi.Output[Optional[str]]:
         """
-        The organization's name.
+        The name of the Pulumi organization the team belongs to.
         """
         return pulumi.get(self, "organization_name")
 
     @property
     @pulumi.getter(name="teamType")
     def team_type(self) -> pulumi.Output[Optional[str]]:
         """
```

### Comparing `pulumi_pulumiservice-0.9.0/pulumi_pulumiservice/team_access_token.py` & `pulumi_pulumiservice-0.9.1a1689804796/pulumi_pulumiservice/team_access_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_pulumiservice-0.9.0/pulumi_pulumiservice/team_stack_permission.py` & `pulumi_pulumiservice-0.9.1a1689804796/pulumi_pulumiservice/team_stack_permission.py`

 * *Files identical despite different names*

### Comparing `pulumi_pulumiservice-0.9.0/pulumi_pulumiservice/webhook.py` & `pulumi_pulumiservice-0.9.1a1689804796/pulumi_pulumiservice/webhook.py`

 * *Files identical despite different names*

### Comparing `pulumi_pulumiservice-0.9.0/pulumi_pulumiservice.egg-info/PKG-INFO` & `pulumi_pulumiservice-0.9.1a1689804796/pulumi_pulumiservice.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,110 +1,108 @@
 Metadata-Version: 2.1
 Name: pulumi-pulumiservice
-Version: 0.9.0
+Version: 0.9.1a1689804796
 Summary: A native Pulumi package for creating and managing Pulumi Cloud constructs
 Home-page: https://pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-pulumiservice
+Description: # Pulumi Service Provider
+        
+        [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
+        [![NPM version](https://badge.fury.io/js/%40pulumi%2Fpulumiservice.svg)](https://www.npmjs.com/package/@pulumi/pulumiservice)
+        [![Python version](https://badge.fury.io/py/pulumi-pulumiservice.svg)](https://pypi.org/project/pulumi-pulumiservice)
+        [![NuGet version](https://badge.fury.io/nu/pulumi.pulumiservice.svg)](https://badge.fury.io/nu/pulumi.pulumiservice)
+        [![PkgGoDev](https://pkg.go.dev/badge/github.com/pulumi/pulumi-pulumiservice/sdk/go/pulumiservice)](https://pkg.go.dev/github.com/pulumi/pulumi-pulumiservice/sdk/go)
+        [![License](https://img.shields.io/npm/l/%40pulumi%2Fpulumiservice.svg)](https://github.com/pulumi/pulumi-pulumiservice/blob/main/LICENSE)
+        
+        A Pulumi Resource Provider for The Pulumi Service.
+        
+        The Pulumi Service Provider is built on top of the [Pulumi Service REST API](https://pulumi.com/docs/reference/service-rest-api) which is another feature available to our customers to programmatically configuring the Pulumi Service. The Pulumi Service REST API includes functionality to interact with and manipulate any kind of metadata managed by Pulumi. That includes Projects and Stacks, Previews and Updates, Organizations and Audit Logs. We have already seen Cloud Engineering teams using the Pulumi REST API to build all sorts of custom functionality. These new capabilities are especially powerful when used in combination with the [Automation API](https://pulumi.com/automation).
+        
+        #### Supported Resources
+        
+        - [Webhooks](https://pulumi.com/docs/intro/pulumi-service/webhooks)
+        - [Teams](https://pulumi.com/docs/intro/pulumi-service/teams)
+          - You can grant a team access to stacks via the `TeamStackPermission` resource
+        - [StackTags](https://pulumi.com/docs/reference/cli/pulumi_stack_tag)
+        - [AccessTokens](https://pulumi.com/docs/intro/pulumi-service/accounts)
+        
+        For reference documentation, visit the [Pulumi Service API Documentation](https://www.pulumi.com/registry/packages/pulumiservice/api-docs/) on the [Pulumi Registry](https://www.pulumi.com/registry/packages/pulumiservice/)
+        
+        ## Installing
+        
+        This package is available in many languages in the standard packaging formats.
+        
+        ### Node.js (Java/TypeScript)
+        
+        To use from JavaScript or TypeScript in Node.js, install using either `npm`:
+        
+            $ npm install @pulumi/pulumiservice
+        
+        or `yarn`:
+        
+            $ yarn add @pulumi/pulumiservice
+        
+        ### Python
+        
+        To use from Python, install using `pip`:
+        
+            $ pip install pulumi_pulumiservice
+        
+        ### Go
+        
+        To use from Go, use `go get` to grab the latest version of the library
+        
+            $ go get github.com/pulumi/pulumi-pulumiservice/sdk/go
+        
+        ### .NET
+        
+        To use from .NET, install using `dotnet add package`:
+        
+            $ dotnet add package Pulumi.PulumiService
+        
+        ## Setup
+        
+        Ensure that you have ran `pulumi login`. Run `pulumi whoami` to verify that you are logged in.
+        
+        ### Configuration Options
+        
+        Use `pulumi config set pulumiservice:<option>` or pass options to the [constructor of `new pulumiservice.Provider`](https://pulumi.com/registry/packages/pulumiservice/api-docs/provider).
+        
+        | Option        | Environment Variable Name | Required/Optional | Description                                                                                                                                                                              |
+        | ------------- | ------------------------- | ----------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+        | `accessToken` | `PULUMI_ACCESS_TOKEN`     | Optional          | Overrides [Pulumi Service Access Tokens](https://www.pulumi.com/docs/intro/pulumi-service/accounts/#access-tokens)                                                                       |
+        | `apiUrl`      | `PULUMI_BACKEND_URL`      | Optional          | Allows overriding default [Pulumi Service API URL](https://www.pulumi.com/docs/reference/service-rest-api) for [self hosted customers](https://www.pulumi.com/docs/guides/self-hosted/). |
+        
+        ## Examples
+        
+        ```typescript
+        import * as aws from "@pulumi/awsx"
+        import * as pulumi from "@pulumi/pulumi";
+        import * as service from "@pulumi/pulumiservice";
+        
+        const team = new service.Team("team", {
+            name: "pulumi-service-team",
+            displayName: "Pulumi Service",
+            description: "The Pulumi Service Team",
+            organizationName: "pulumi",
+            teamType: "pulumi",
+            members: [
+                "piers",
+                "bryce",
+                "casey"
+                "evan",
+                "devon",
+                "meagan"
+                "myles",
+                "steve"
+            ],
+        });
+        
+        export const members = team.members;
+        ```
+        
+        Check out the [examples/](examples/) directory for more examples.
+        
 Keywords: pulumi kind/native category/infrastructure
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
-
-# Pulumi Service Provider
-
-[![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
-[![NPM version](https://badge.fury.io/js/%40pulumi%2Fpulumiservice.svg)](https://www.npmjs.com/package/@pulumi/pulumiservice)
-[![Python version](https://badge.fury.io/py/pulumi-pulumiservice.svg)](https://pypi.org/project/pulumi-pulumiservice)
-[![NuGet version](https://badge.fury.io/nu/pulumi.pulumiservice.svg)](https://badge.fury.io/nu/pulumi.pulumiservice)
-[![PkgGoDev](https://pkg.go.dev/badge/github.com/pulumi/pulumi-pulumiservice/sdk/go/pulumiservice)](https://pkg.go.dev/github.com/pulumi/pulumi-pulumiservice/sdk/go)
-[![License](https://img.shields.io/npm/l/%40pulumi%2Fpulumiservice.svg)](https://github.com/pulumi/pulumi-pulumiservice/blob/main/LICENSE)
-
-A Pulumi Resource Provider for The Pulumi Service.
-
-The Pulumi Service Provider is built on top of the [Pulumi Service REST API](https://pulumi.com/docs/reference/service-rest-api) which is another feature available to our customers to programmatically configuring the Pulumi Service. The Pulumi Service REST API includes functionality to interact with and manipulate any kind of metadata managed by Pulumi. That includes Projects and Stacks, Previews and Updates, Organizations and Audit Logs. We have already seen Cloud Engineering teams using the Pulumi REST API to build all sorts of custom functionality. These new capabilities are especially powerful when used in combination with the [Automation API](https://pulumi.com/automation).
-
-#### Supported Resources
-
-- [Webhooks](https://pulumi.com/docs/intro/pulumi-service/webhooks)
-- [Teams](https://pulumi.com/docs/intro/pulumi-service/teams)
-  - You can grant a team access to stacks via the `TeamStackPermission` resource
-- [StackTags](https://pulumi.com/docs/reference/cli/pulumi_stack_tag)
-- [AccessTokens](https://pulumi.com/docs/intro/pulumi-service/accounts)
-
-For reference documentation, visit the [Pulumi Service API Documentation](https://www.pulumi.com/registry/packages/pulumiservice/api-docs/) on the [Pulumi Registry](https://www.pulumi.com/registry/packages/pulumiservice/)
-
-## Installing
-
-This package is available in many languages in the standard packaging formats.
-
-### Node.js (Java/TypeScript)
-
-To use from JavaScript or TypeScript in Node.js, install using either `npm`:
-
-    $ npm install @pulumi/pulumiservice
-
-or `yarn`:
-
-    $ yarn add @pulumi/pulumiservice
-
-### Python
-
-To use from Python, install using `pip`:
-
-    $ pip install pulumi_pulumiservice
-
-### Go
-
-To use from Go, use `go get` to grab the latest version of the library
-
-    $ go get github.com/pulumi/pulumi-pulumiservice/sdk/go
-
-### .NET
-
-To use from .NET, install using `dotnet add package`:
-
-    $ dotnet add package Pulumi.PulumiService
-
-## Setup
-
-Ensure that you have ran `pulumi login`. Run `pulumi whoami` to verify that you are logged in.
-
-### Configuration Options
-
-Use `pulumi config set pulumiservice:<option>` or pass options to the [constructor of `new pulumiservice.Provider`](https://pulumi.com/registry/packages/pulumiservice/api-docs/provider).
-
-| Option        | Environment Variable Name | Required/Optional | Description                                                                                                                                                                              |
-| ------------- | ------------------------- | ----------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-| `accessToken` | `PULUMI_ACCESS_TOKEN`     | Optional          | Overrides [Pulumi Service Access Tokens](https://www.pulumi.com/docs/intro/pulumi-service/accounts/#access-tokens)                                                                       |
-| `apiUrl`      | `PULUMI_BACKEND_URL`      | Optional          | Allows overriding default [Pulumi Service API URL](https://www.pulumi.com/docs/reference/service-rest-api) for [self hosted customers](https://www.pulumi.com/docs/guides/self-hosted/). |
-
-## Examples
-
-```typescript
-import * as aws from "@pulumi/awsx"
-import * as pulumi from "@pulumi/pulumi";
-import * as service from "@pulumi/pulumiservice";
-
-const team = new service.Team("team", {
-    name: "pulumi-service-team",
-    displayName: "Pulumi Service",
-    description: "The Pulumi Service Team",
-    organizationName: "pulumi",
-    teamType: "pulumi",
-    members: [
-        "piers",
-        "bryce",
-        "casey"
-        "evan",
-        "devon",
-        "meagan"
-        "myles",
-        "steve"
-    ],
-});
-
-export const members = team.members;
-```
-
-Check out the [examples/](examples/) directory for more examples.
-
-
```

### Comparing `pulumi_pulumiservice-0.9.0/pulumi_pulumiservice.egg-info/SOURCES.txt` & `pulumi_pulumiservice-0.9.1a1689804796/pulumi_pulumiservice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_pulumiservice-0.9.0/setup.py` & `pulumi_pulumiservice-0.9.1a1689804796/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.9.0"
-PLUGIN_VERSION = "0.9.0"
+VERSION = "0.9.1a1689804796"
+PLUGIN_VERSION = "0.9.1-alpha.1689804796+dd5e1dd7"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'pulumiservice', PLUGIN_VERSION])
         except OSError as error:
```

