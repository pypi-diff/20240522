# Comparing `tmp/littlejo_cilium-0.0.6.tar.gz` & `tmp/littlejo_cilium-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "littlejo_cilium-0.0.6.tar", last modified: Fri Jan 19 14:39:04 2024, max compression
+gzip compressed data, was "littlejo_cilium-0.0.7.tar", last modified: Wed May 22 16:14:02 2024, max compression
```

## Comparing `littlejo_cilium-0.0.6.tar` & `littlejo_cilium-0.0.7.tar`

### file list

```diff
@@ -1,28 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 14:39:04.959764 littlejo_cilium-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-01-19 14:39:04.955764 littlejo_cilium-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-01-19 14:39:04.000000 littlejo_cilium-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 14:39:04.955764 littlejo_cilium-0.0.6/littlejo_cilium/
--rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-01-19 14:39:04.000000 littlejo_cilium-0.0.6/littlejo_cilium/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9293 2024-01-19 14:39:04.000000 littlejo_cilium-0.0.6/littlejo_cilium/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    16776 2024-01-19 14:39:04.000000 littlejo_cilium-0.0.6/littlejo_cilium/clustermesh.py
--rw-r--r--   0 runner    (1001) docker     (127)     8877 2024-01-19 14:39:04.000000 littlejo_cilium-0.0.6/littlejo_cilium/clustermesh_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 14:39:04.955764 littlejo_cilium-0.0.6/littlejo_cilium/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-01-19 14:39:04.000000 littlejo_cilium-0.0.6/littlejo_cilium/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-01-19 14:39:04.000000 littlejo_cilium-0.0.6/littlejo_cilium/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    10967 2024-01-19 14:39:04.000000 littlejo_cilium-0.0.6/littlejo_cilium/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4433 2024-01-19 14:39:04.000000 littlejo_cilium-0.0.6/littlejo_cilium/get_helm_values.py
--rw-r--r--   0 runner    (1001) docker     (127)     9286 2024-01-19 14:39:04.000000 littlejo_cilium-0.0.6/littlejo_cilium/hubble.py
--rw-r--r--   0 runner    (1001) docker     (127)    24816 2024-01-19 14:39:04.000000 littlejo_cilium-0.0.6/littlejo_cilium/install.py
--rw-r--r--   0 runner    (1001) docker     (127)     7624 2024-01-19 14:39:04.000000 littlejo_cilium-0.0.6/littlejo_cilium/kubeproxy_free.py
--rw-r--r--   0 runner    (1001) docker     (127)     6797 2024-01-19 14:39:04.000000 littlejo_cilium-0.0.6/littlejo_cilium/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-01-19 14:39:04.000000 littlejo_cilium-0.0.6/littlejo_cilium/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-19 14:39:04.000000 littlejo_cilium-0.0.6/littlejo_cilium/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 14:39:04.955764 littlejo_cilium-0.0.6/littlejo_cilium.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-01-19 14:39:04.000000 littlejo_cilium-0.0.6/littlejo_cilium.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-01-19 14:39:04.000000 littlejo_cilium-0.0.6/littlejo_cilium.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-19 14:39:04.000000 littlejo_cilium-0.0.6/littlejo_cilium.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-19 14:39:04.000000 littlejo_cilium-0.0.6/littlejo_cilium.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-01-19 14:39:04.000000 littlejo_cilium-0.0.6/littlejo_cilium.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-01-19 14:39:04.000000 littlejo_cilium-0.0.6/littlejo_cilium.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-19 14:39:04.959764 littlejo_cilium-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-01-19 14:39:04.000000 littlejo_cilium-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:14:02.287436 littlejo_cilium-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-22 16:14:02.287436 littlejo_cilium-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-22 16:14:02.000000 littlejo_cilium-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:14:02.283436 littlejo_cilium-0.0.7/littlejo_cilium/
+-rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-05-22 16:14:02.000000 littlejo_cilium-0.0.7/littlejo_cilium/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-22 16:14:02.000000 littlejo_cilium-0.0.7/littlejo_cilium/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9292 2024-05-22 16:14:02.000000 littlejo_cilium-0.0.7/littlejo_cilium/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13575 2024-05-22 16:14:02.000000 littlejo_cilium-0.0.7/littlejo_cilium/clustermesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6316 2024-05-22 16:14:02.000000 littlejo_cilium-0.0.7/littlejo_cilium/clustermesh_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:14:02.287436 littlejo_cilium-0.0.7/littlejo_cilium/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-22 16:14:02.000000 littlejo_cilium-0.0.7/littlejo_cilium/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-22 16:14:02.000000 littlejo_cilium-0.0.7/littlejo_cilium/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9044 2024-05-22 16:14:02.000000 littlejo_cilium-0.0.7/littlejo_cilium/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22148 2024-05-22 16:14:02.000000 littlejo_cilium-0.0.7/littlejo_cilium/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-05-22 16:14:02.000000 littlejo_cilium-0.0.7/littlejo_cilium/get_helm_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7363 2024-05-22 16:14:02.000000 littlejo_cilium-0.0.7/littlejo_cilium/hubble.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23601 2024-05-22 16:14:02.000000 littlejo_cilium-0.0.7/littlejo_cilium/install.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7624 2024-05-22 16:14:02.000000 littlejo_cilium-0.0.7/littlejo_cilium/kubeproxy_free.py
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-22 16:14:02.000000 littlejo_cilium-0.0.7/littlejo_cilium/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9199 2024-05-22 16:14:02.000000 littlejo_cilium-0.0.7/littlejo_cilium/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-22 16:14:02.000000 littlejo_cilium-0.0.7/littlejo_cilium/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 16:14:02.000000 littlejo_cilium-0.0.7/littlejo_cilium/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:14:02.287436 littlejo_cilium-0.0.7/littlejo_cilium.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-22 16:14:02.000000 littlejo_cilium-0.0.7/littlejo_cilium.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-22 16:14:02.000000 littlejo_cilium-0.0.7/littlejo_cilium.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 16:14:02.000000 littlejo_cilium-0.0.7/littlejo_cilium.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 16:14:02.000000 littlejo_cilium-0.0.7/littlejo_cilium.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-22 16:14:02.000000 littlejo_cilium-0.0.7/littlejo_cilium.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-22 16:14:02.000000 littlejo_cilium-0.0.7/littlejo_cilium.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 16:14:02.287436 littlejo_cilium-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-05-22 16:14:02.000000 littlejo_cilium-0.0.7/setup.py
```

### Comparing `littlejo_cilium-0.0.6/PKG-INFO` & `littlejo_cilium-0.0.7/littlejo_cilium.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
-Name: littlejo_cilium
-Version: 0.0.6
+Name: littlejo-cilium
+Version: 0.0.7
 Summary: A Pulumi package for creating and managing Cilium resources
 Home-page: https://github.com/littlejo/pulumi-cilium
 License: Apache-2.0
 Project-URL: Repository, https://github.com/littlejo/pulumi-cilium
 Keywords: pulumi cilium category/network
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # Cilium Resource Provider
 
 The Cilium Resource Provider lets you manage [cilium](https://www.pulumi.com/registry/packages/cilium/) resources.
 
 ## Installing
```

### Comparing `littlejo_cilium-0.0.6/README.md` & `littlejo_cilium-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `littlejo_cilium-0.0.6/littlejo_cilium/__init__.py` & `littlejo_cilium-0.0.7/littlejo_cilium/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,19 +4,22 @@
 
 from . import _utilities
 import typing
 # Export this package's modules as members:
 from .clustermesh import *
 from .clustermesh_connection import *
 from .config import *
+from .deploy import *
 from .get_helm_values import *
 from .hubble import *
 from .install import *
 from .kubeproxy_free import *
 from .provider import *
+from ._inputs import *
+from . import outputs
 
 # Make subpackages available:
 if typing.TYPE_CHECKING:
     import littlejo_cilium.config as __config
     config = __config
 else:
     config = _utilities.lazy_import('littlejo_cilium.config')
@@ -46,14 +49,22 @@
   "fqn": "littlejo_cilium",
   "classes": {
    "cilium:index/config:Config": "Config"
   }
  },
  {
   "pkg": "cilium",
+  "mod": "index/deploy",
+  "fqn": "littlejo_cilium",
+  "classes": {
+   "cilium:index/deploy:Deploy": "Deploy"
+  }
+ },
+ {
+  "pkg": "cilium",
   "mod": "index/hubble",
   "fqn": "littlejo_cilium",
   "classes": {
    "cilium:index/hubble:Hubble": "Hubble"
   }
  },
  {
```

### Comparing `littlejo_cilium-0.0.6/littlejo_cilium/_utilities.py` & `littlejo_cilium-0.0.7/littlejo_cilium/_utilities.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 
 import asyncio
+import importlib.metadata
 import importlib.util
 import inspect
 import json
 import os
-import pkg_resources
 import sys
 import typing
 
 import pulumi
 import pulumi.runtime
 from pulumi.runtime.sync_await import _sync_await
 
@@ -68,15 +68,15 @@
     # pkg_resources uses setuptools to inspect the set of installed packages. We use it here to ask
     # for the currently installed version of the root package (i.e. us) and get its version.
 
     # Unfortunately, PEP440 and semver differ slightly in incompatible ways. The Pulumi engine expects
     # to receive a valid semver string when receiving requests from the language host, so it's our
     # responsibility as the library to convert our own PEP440 version into a valid semver string.
 
-    pep440_version_string = pkg_resources.require(root_package)[0].version
+    pep440_version_string = importlib.metadata.version(root_package)
     pep440_version = PEP440Version.parse(pep440_version_string)
     (major, minor, patch) = pep440_version.release
     prerelease = None
     if pep440_version.pre_tag == 'a':
         prerelease = f"alpha.{pep440_version.pre}"
     elif pep440_version.pre_tag == 'b':
         prerelease = f"beta.{pep440_version.pre}"
```

### Comparing `littlejo_cilium-0.0.6/littlejo_cilium/clustermesh.py` & `littlejo_cilium-0.0.7/littlejo_cilium/clustermesh.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,31 +12,27 @@
 __all__ = ['ClustermeshArgs', 'Clustermesh']
 
 @pulumi.input_type
 class ClustermeshArgs:
     def __init__(__self__, *,
                  enable_external_workloads: Optional[pulumi.Input[bool]] = None,
                  enable_kv_store_mesh: Optional[pulumi.Input[bool]] = None,
-                 namespace: Optional[pulumi.Input[str]] = None,
                  service_type: Optional[pulumi.Input[str]] = None,
                  wait: Optional[pulumi.Input[bool]] = None):
         """
         The set of arguments for constructing a Clustermesh resource.
         :param pulumi.Input[bool] enable_external_workloads: Enable support for external workloads, such as VMs (Default: `false`).
         :param pulumi.Input[bool] enable_kv_store_mesh: Enable kvstoremesh, an extension which caches remote cluster information in the local kvstore (Cilium >=1.14 only) (Default: `false`).
-        :param pulumi.Input[str] namespace: Namespace in which to install (Default: `kube-system`).
         :param pulumi.Input[str] service_type: Type of Kubernetes service to expose control plane { LoadBalancer | NodePort | ClusterIP } (Default: `autodetected`).
         :param pulumi.Input[bool] wait: Wait Cluster Mesh status is ok (Default: `true`).
         """
         if enable_external_workloads is not None:
             pulumi.set(__self__, "enable_external_workloads", enable_external_workloads)
         if enable_kv_store_mesh is not None:
             pulumi.set(__self__, "enable_kv_store_mesh", enable_kv_store_mesh)
-        if namespace is not None:
-            pulumi.set(__self__, "namespace", namespace)
         if service_type is not None:
             pulumi.set(__self__, "service_type", service_type)
         if wait is not None:
             pulumi.set(__self__, "wait", wait)
 
     @property
     @pulumi.getter(name="enableExternalWorkloads")
@@ -59,26 +55,14 @@
         return pulumi.get(self, "enable_kv_store_mesh")
 
     @enable_kv_store_mesh.setter
     def enable_kv_store_mesh(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "enable_kv_store_mesh", value)
 
     @property
-    @pulumi.getter
-    def namespace(self) -> Optional[pulumi.Input[str]]:
-        """
-        Namespace in which to install (Default: `kube-system`).
-        """
-        return pulumi.get(self, "namespace")
-
-    @namespace.setter
-    def namespace(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "namespace", value)
-
-    @property
     @pulumi.getter(name="serviceType")
     def service_type(self) -> Optional[pulumi.Input[str]]:
         """
         Type of Kubernetes service to expose control plane { LoadBalancer | NodePort | ClusterIP } (Default: `autodetected`).
         """
         return pulumi.get(self, "service_type")
 
@@ -100,31 +84,27 @@
 
 
 @pulumi.input_type
 class _ClustermeshState:
     def __init__(__self__, *,
                  enable_external_workloads: Optional[pulumi.Input[bool]] = None,
                  enable_kv_store_mesh: Optional[pulumi.Input[bool]] = None,
-                 namespace: Optional[pulumi.Input[str]] = None,
                  service_type: Optional[pulumi.Input[str]] = None,
                  wait: Optional[pulumi.Input[bool]] = None):
         """
         Input properties used for looking up and filtering Clustermesh resources.
         :param pulumi.Input[bool] enable_external_workloads: Enable support for external workloads, such as VMs (Default: `false`).
         :param pulumi.Input[bool] enable_kv_store_mesh: Enable kvstoremesh, an extension which caches remote cluster information in the local kvstore (Cilium >=1.14 only) (Default: `false`).
-        :param pulumi.Input[str] namespace: Namespace in which to install (Default: `kube-system`).
         :param pulumi.Input[str] service_type: Type of Kubernetes service to expose control plane { LoadBalancer | NodePort | ClusterIP } (Default: `autodetected`).
         :param pulumi.Input[bool] wait: Wait Cluster Mesh status is ok (Default: `true`).
         """
         if enable_external_workloads is not None:
             pulumi.set(__self__, "enable_external_workloads", enable_external_workloads)
         if enable_kv_store_mesh is not None:
             pulumi.set(__self__, "enable_kv_store_mesh", enable_kv_store_mesh)
-        if namespace is not None:
-            pulumi.set(__self__, "namespace", namespace)
         if service_type is not None:
             pulumi.set(__self__, "service_type", service_type)
         if wait is not None:
             pulumi.set(__self__, "wait", wait)
 
     @property
     @pulumi.getter(name="enableExternalWorkloads")
@@ -147,26 +127,14 @@
         return pulumi.get(self, "enable_kv_store_mesh")
 
     @enable_kv_store_mesh.setter
     def enable_kv_store_mesh(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "enable_kv_store_mesh", value)
 
     @property
-    @pulumi.getter
-    def namespace(self) -> Optional[pulumi.Input[str]]:
-        """
-        Namespace in which to install (Default: `kube-system`).
-        """
-        return pulumi.get(self, "namespace")
-
-    @namespace.setter
-    def namespace(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "namespace", value)
-
-    @property
     @pulumi.getter(name="serviceType")
     def service_type(self) -> Optional[pulumi.Input[str]]:
         """
         Type of Kubernetes service to expose control plane { LoadBalancer | NodePort | ClusterIP } (Default: `autodetected`).
         """
         return pulumi.get(self, "service_type")
 
@@ -190,72 +158,34 @@
 class Clustermesh(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  enable_external_workloads: Optional[pulumi.Input[bool]] = None,
                  enable_kv_store_mesh: Optional[pulumi.Input[bool]] = None,
-                 namespace: Optional[pulumi.Input[str]] = None,
                  service_type: Optional[pulumi.Input[str]] = None,
                  wait: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
         """
-        Cluster Mesh resource. This is equivalent to cilium cli: `cilium clustermesh enable` and `cilium clustermesh disable`: It manages the activation of Cluster Mesh on one Kubernetes cluster.
-
-        ## Example Usage
-
-        ```python
-        import pulumi
-        import littlejo_cilium as cilium
-
-        example_install = cilium.Install("exampleInstall",
-            sets=[
-                "cluster.name=clustermesh1",
-                "cluster.id=1",
-                "ipam.mode=kubernetes",
-            ],
-            version="1.14.5")
-        example_clustermesh = cilium.Clustermesh("exampleClustermesh", service_type="LoadBalancer",
-        opts=pulumi.ResourceOptions(depends_on=[example_install]))
-        ```
-
+        Create a Clustermesh resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] enable_external_workloads: Enable support for external workloads, such as VMs (Default: `false`).
         :param pulumi.Input[bool] enable_kv_store_mesh: Enable kvstoremesh, an extension which caches remote cluster information in the local kvstore (Cilium >=1.14 only) (Default: `false`).
-        :param pulumi.Input[str] namespace: Namespace in which to install (Default: `kube-system`).
         :param pulumi.Input[str] service_type: Type of Kubernetes service to expose control plane { LoadBalancer | NodePort | ClusterIP } (Default: `autodetected`).
         :param pulumi.Input[bool] wait: Wait Cluster Mesh status is ok (Default: `true`).
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: Optional[ClustermeshArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Cluster Mesh resource. This is equivalent to cilium cli: `cilium clustermesh enable` and `cilium clustermesh disable`: It manages the activation of Cluster Mesh on one Kubernetes cluster.
-
-        ## Example Usage
-
-        ```python
-        import pulumi
-        import littlejo_cilium as cilium
-
-        example_install = cilium.Install("exampleInstall",
-            sets=[
-                "cluster.name=clustermesh1",
-                "cluster.id=1",
-                "ipam.mode=kubernetes",
-            ],
-            version="1.14.5")
-        example_clustermesh = cilium.Clustermesh("exampleClustermesh", service_type="LoadBalancer",
-        opts=pulumi.ResourceOptions(depends_on=[example_install]))
-        ```
-
+        Create a Clustermesh resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
         :param ClustermeshArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
         resource_args, opts = _utilities.get_resource_args_opts(ClustermeshArgs, pulumi.ResourceOptions, *args, **kwargs)
@@ -265,66 +195,61 @@
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  enable_external_workloads: Optional[pulumi.Input[bool]] = None,
                  enable_kv_store_mesh: Optional[pulumi.Input[bool]] = None,
-                 namespace: Optional[pulumi.Input[str]] = None,
                  service_type: Optional[pulumi.Input[str]] = None,
                  wait: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ClustermeshArgs.__new__(ClustermeshArgs)
 
             __props__.__dict__["enable_external_workloads"] = enable_external_workloads
             __props__.__dict__["enable_kv_store_mesh"] = enable_kv_store_mesh
-            __props__.__dict__["namespace"] = namespace
             __props__.__dict__["service_type"] = service_type
             __props__.__dict__["wait"] = wait
         super(Clustermesh, __self__).__init__(
             'cilium:index/clustermesh:Clustermesh',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             enable_external_workloads: Optional[pulumi.Input[bool]] = None,
             enable_kv_store_mesh: Optional[pulumi.Input[bool]] = None,
-            namespace: Optional[pulumi.Input[str]] = None,
             service_type: Optional[pulumi.Input[str]] = None,
             wait: Optional[pulumi.Input[bool]] = None) -> 'Clustermesh':
         """
         Get an existing Clustermesh resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] enable_external_workloads: Enable support for external workloads, such as VMs (Default: `false`).
         :param pulumi.Input[bool] enable_kv_store_mesh: Enable kvstoremesh, an extension which caches remote cluster information in the local kvstore (Cilium >=1.14 only) (Default: `false`).
-        :param pulumi.Input[str] namespace: Namespace in which to install (Default: `kube-system`).
         :param pulumi.Input[str] service_type: Type of Kubernetes service to expose control plane { LoadBalancer | NodePort | ClusterIP } (Default: `autodetected`).
         :param pulumi.Input[bool] wait: Wait Cluster Mesh status is ok (Default: `true`).
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _ClustermeshState.__new__(_ClustermeshState)
 
         __props__.__dict__["enable_external_workloads"] = enable_external_workloads
         __props__.__dict__["enable_kv_store_mesh"] = enable_kv_store_mesh
-        __props__.__dict__["namespace"] = namespace
         __props__.__dict__["service_type"] = service_type
         __props__.__dict__["wait"] = wait
         return Clustermesh(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="enableExternalWorkloads")
     def enable_external_workloads(self) -> pulumi.Output[bool]:
@@ -338,22 +263,14 @@
     def enable_kv_store_mesh(self) -> pulumi.Output[bool]:
         """
         Enable kvstoremesh, an extension which caches remote cluster information in the local kvstore (Cilium >=1.14 only) (Default: `false`).
         """
         return pulumi.get(self, "enable_kv_store_mesh")
 
     @property
-    @pulumi.getter
-    def namespace(self) -> pulumi.Output[str]:
-        """
-        Namespace in which to install (Default: `kube-system`).
-        """
-        return pulumi.get(self, "namespace")
-
-    @property
     @pulumi.getter(name="serviceType")
     def service_type(self) -> pulumi.Output[str]:
         """
         Type of Kubernetes service to expose control plane { LoadBalancer | NodePort | ClusterIP } (Default: `autodetected`).
         """
         return pulumi.get(self, "service_type")
```

### Comparing `littlejo_cilium-0.0.6/littlejo_cilium/clustermesh_connection.py` & `littlejo_cilium-0.0.7/littlejo_cilium/clustermesh_connection.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,134 +10,80 @@
 from . import _utilities
 
 __all__ = ['ClustermeshConnectionArgs', 'ClustermeshConnection']
 
 @pulumi.input_type
 class ClustermeshConnectionArgs:
     def __init__(__self__, *,
-                 destination_context: Optional[pulumi.Input[str]] = None,
-                 namespace: Optional[pulumi.Input[str]] = None):
+                 destination_context: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a ClustermeshConnection resource.
         :param pulumi.Input[str] destination_context: Kubernetes configuration context of destination cluster
-        :param pulumi.Input[str] namespace: Namespace in which to install (Default: `kube-system`).
         """
         if destination_context is not None:
             pulumi.set(__self__, "destination_context", destination_context)
-        if namespace is not None:
-            pulumi.set(__self__, "namespace", namespace)
 
     @property
     @pulumi.getter(name="destinationContext")
     def destination_context(self) -> Optional[pulumi.Input[str]]:
         """
         Kubernetes configuration context of destination cluster
         """
         return pulumi.get(self, "destination_context")
 
     @destination_context.setter
     def destination_context(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "destination_context", value)
 
-    @property
-    @pulumi.getter
-    def namespace(self) -> Optional[pulumi.Input[str]]:
-        """
-        Namespace in which to install (Default: `kube-system`).
-        """
-        return pulumi.get(self, "namespace")
-
-    @namespace.setter
-    def namespace(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "namespace", value)
-
 
 @pulumi.input_type
 class _ClustermeshConnectionState:
     def __init__(__self__, *,
-                 destination_context: Optional[pulumi.Input[str]] = None,
-                 namespace: Optional[pulumi.Input[str]] = None):
+                 destination_context: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering ClustermeshConnection resources.
         :param pulumi.Input[str] destination_context: Kubernetes configuration context of destination cluster
-        :param pulumi.Input[str] namespace: Namespace in which to install (Default: `kube-system`).
         """
         if destination_context is not None:
             pulumi.set(__self__, "destination_context", destination_context)
-        if namespace is not None:
-            pulumi.set(__self__, "namespace", namespace)
 
     @property
     @pulumi.getter(name="destinationContext")
     def destination_context(self) -> Optional[pulumi.Input[str]]:
         """
         Kubernetes configuration context of destination cluster
         """
         return pulumi.get(self, "destination_context")
 
     @destination_context.setter
     def destination_context(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "destination_context", value)
 
-    @property
-    @pulumi.getter
-    def namespace(self) -> Optional[pulumi.Input[str]]:
-        """
-        Namespace in which to install (Default: `kube-system`).
-        """
-        return pulumi.get(self, "namespace")
-
-    @namespace.setter
-    def namespace(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "namespace", value)
-
 
 class ClustermeshConnection(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  destination_context: Optional[pulumi.Input[str]] = None,
-                 namespace: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        Cluster Mesh connection resource. This is equivalent to cilium cli: `cilium clustermesh connect` and `cilium clustermesh disconnect`: It manages the connections between two Kubernetes clusters.
-
-        ## Example Usage
-
-        ```python
-        import pulumi
-        import littlejo_cilium as cilium
-
-        example = cilium.ClustermeshConnection("example", destination_context="context-2")
-        ```
-
+        Create a ClustermeshConnection resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] destination_context: Kubernetes configuration context of destination cluster
-        :param pulumi.Input[str] namespace: Namespace in which to install (Default: `kube-system`).
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: Optional[ClustermeshConnectionArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Cluster Mesh connection resource. This is equivalent to cilium cli: `cilium clustermesh connect` and `cilium clustermesh disconnect`: It manages the connections between two Kubernetes clusters.
-
-        ## Example Usage
-
-        ```python
-        import pulumi
-        import littlejo_cilium as cilium
-
-        example = cilium.ClustermeshConnection("example", destination_context="context-2")
-        ```
-
+        Create a ClustermeshConnection resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
         :param ClustermeshConnectionArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
         resource_args, opts = _utilities.get_resource_args_opts(ClustermeshConnectionArgs, pulumi.ResourceOptions, *args, **kwargs)
@@ -146,65 +92,52 @@
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  destination_context: Optional[pulumi.Input[str]] = None,
-                 namespace: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ClustermeshConnectionArgs.__new__(ClustermeshConnectionArgs)
 
             __props__.__dict__["destination_context"] = destination_context
-            __props__.__dict__["namespace"] = namespace
         super(ClustermeshConnection, __self__).__init__(
             'cilium:index/clustermeshConnection:ClustermeshConnection',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
-            destination_context: Optional[pulumi.Input[str]] = None,
-            namespace: Optional[pulumi.Input[str]] = None) -> 'ClustermeshConnection':
+            destination_context: Optional[pulumi.Input[str]] = None) -> 'ClustermeshConnection':
         """
         Get an existing ClustermeshConnection resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] destination_context: Kubernetes configuration context of destination cluster
-        :param pulumi.Input[str] namespace: Namespace in which to install (Default: `kube-system`).
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _ClustermeshConnectionState.__new__(_ClustermeshConnectionState)
 
         __props__.__dict__["destination_context"] = destination_context
-        __props__.__dict__["namespace"] = namespace
         return ClustermeshConnection(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="destinationContext")
     def destination_context(self) -> pulumi.Output[str]:
         """
         Kubernetes configuration context of destination cluster
         """
         return pulumi.get(self, "destination_context")
 
-    @property
-    @pulumi.getter
-    def namespace(self) -> pulumi.Output[str]:
-        """
-        Namespace in which to install (Default: `kube-system`).
-        """
-        return pulumi.get(self, "namespace")
-
```

### Comparing `littlejo_cilium-0.0.6/littlejo_cilium/config/vars.py` & `littlejo_cilium-0.0.7/littlejo_cilium/config/vars.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,27 +12,41 @@
 import types
 
 __config__ = pulumi.Config('cilium')
 
 
 class _ExportableConfig(types.ModuleType):
     @property
+    def config_content(self) -> Optional[str]:
+        """
+        The content of kube config file (Default: ``).
+        """
+        return __config__.get('configContent')
+
+    @property
     def config_path(self) -> Optional[str]:
         """
         A path to a kube config file (Default: `~/.kube/config`).
         """
         return __config__.get('configPath')
 
     @property
     def context(self) -> Optional[str]:
         """
         Context of kubeconfig file (Default: `default context`).
         """
         return __config__.get('context')
 
     @property
+    def helm_release(self) -> Optional[str]:
+        """
+        Helm Release to install cilium (Default: `Install`).
+        """
+        return __config__.get('helmRelease')
+
+    @property
     def namespace(self) -> Optional[str]:
         """
         Namespace to install cilium (Default: `kube-system`).
         """
         return __config__.get('namespace')
```

### Comparing `littlejo_cilium-0.0.6/littlejo_cilium/config.py` & `littlejo_cilium-0.0.7/littlejo_cilium/config.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,27 +12,23 @@
 __all__ = ['ConfigArgs', 'Config']
 
 @pulumi.input_type
 class ConfigArgs:
     def __init__(__self__, *,
                  key: pulumi.Input[str],
                  value: pulumi.Input[str],
-                 namespace: Optional[pulumi.Input[str]] = None,
                  restart: Optional[pulumi.Input[bool]] = None):
         """
         The set of arguments for constructing a Config resource.
         :param pulumi.Input[str] key: Key of the config
         :param pulumi.Input[str] value: Value of the key
-        :param pulumi.Input[str] namespace: Namespace in which to install (Default: `kube-system`).
         :param pulumi.Input[bool] restart: Restart Cilium pods (Default: `true`).
         """
         pulumi.set(__self__, "key", key)
         pulumi.set(__self__, "value", value)
-        if namespace is not None:
-            pulumi.set(__self__, "namespace", namespace)
         if restart is not None:
             pulumi.set(__self__, "restart", restart)
 
     @property
     @pulumi.getter
     def key(self) -> pulumi.Input[str]:
         """
@@ -54,26 +50,14 @@
 
     @value.setter
     def value(self, value: pulumi.Input[str]):
         pulumi.set(self, "value", value)
 
     @property
     @pulumi.getter
-    def namespace(self) -> Optional[pulumi.Input[str]]:
-        """
-        Namespace in which to install (Default: `kube-system`).
-        """
-        return pulumi.get(self, "namespace")
-
-    @namespace.setter
-    def namespace(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "namespace", value)
-
-    @property
-    @pulumi.getter
     def restart(self) -> Optional[pulumi.Input[bool]]:
         """
         Restart Cilium pods (Default: `true`).
         """
         return pulumi.get(self, "restart")
 
     @restart.setter
@@ -81,28 +65,24 @@
         pulumi.set(self, "restart", value)
 
 
 @pulumi.input_type
 class _ConfigState:
     def __init__(__self__, *,
                  key: Optional[pulumi.Input[str]] = None,
-                 namespace: Optional[pulumi.Input[str]] = None,
                  restart: Optional[pulumi.Input[bool]] = None,
                  value: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering Config resources.
         :param pulumi.Input[str] key: Key of the config
-        :param pulumi.Input[str] namespace: Namespace in which to install (Default: `kube-system`).
         :param pulumi.Input[bool] restart: Restart Cilium pods (Default: `true`).
         :param pulumi.Input[str] value: Value of the key
         """
         if key is not None:
             pulumi.set(__self__, "key", key)
-        if namespace is not None:
-            pulumi.set(__self__, "namespace", namespace)
         if restart is not None:
             pulumi.set(__self__, "restart", restart)
         if value is not None:
             pulumi.set(__self__, "value", value)
 
     @property
     @pulumi.getter
@@ -114,26 +94,14 @@
 
     @key.setter
     def key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "key", value)
 
     @property
     @pulumi.getter
-    def namespace(self) -> Optional[pulumi.Input[str]]:
-        """
-        Namespace in which to install (Default: `kube-system`).
-        """
-        return pulumi.get(self, "namespace")
-
-    @namespace.setter
-    def namespace(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "namespace", value)
-
-    @property
-    @pulumi.getter
     def restart(self) -> Optional[pulumi.Input[bool]]:
         """
         Restart Cilium pods (Default: `true`).
         """
         return pulumi.get(self, "restart")
 
     @restart.setter
@@ -155,15 +123,14 @@
 
 class Config(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  key: Optional[pulumi.Input[str]] = None,
-                 namespace: Optional[pulumi.Input[str]] = None,
                  restart: Optional[pulumi.Input[bool]] = None,
                  value: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Config resource for Cilium. This is equivalent to cilium cli: `cilium config`: It manages the cilium Kubernetes ConfigMap resource
 
         ## Example Usage
@@ -176,15 +143,14 @@
             key="debug",
             value="true")
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] key: Key of the config
-        :param pulumi.Input[str] namespace: Namespace in which to install (Default: `kube-system`).
         :param pulumi.Input[bool] restart: Restart Cilium pods (Default: `true`).
         :param pulumi.Input[str] value: Value of the key
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
@@ -216,30 +182,28 @@
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  key: Optional[pulumi.Input[str]] = None,
-                 namespace: Optional[pulumi.Input[str]] = None,
                  restart: Optional[pulumi.Input[bool]] = None,
                  value: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ConfigArgs.__new__(ConfigArgs)
 
             if key is None and not opts.urn:
                 raise TypeError("Missing required property 'key'")
             __props__.__dict__["key"] = key
-            __props__.__dict__["namespace"] = namespace
             __props__.__dict__["restart"] = restart
             if value is None and not opts.urn:
                 raise TypeError("Missing required property 'value'")
             __props__.__dict__["value"] = value
         super(Config, __self__).__init__(
             'cilium:index/config:Config',
             resource_name,
@@ -247,57 +211,46 @@
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             key: Optional[pulumi.Input[str]] = None,
-            namespace: Optional[pulumi.Input[str]] = None,
             restart: Optional[pulumi.Input[bool]] = None,
             value: Optional[pulumi.Input[str]] = None) -> 'Config':
         """
         Get an existing Config resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] key: Key of the config
-        :param pulumi.Input[str] namespace: Namespace in which to install (Default: `kube-system`).
         :param pulumi.Input[bool] restart: Restart Cilium pods (Default: `true`).
         :param pulumi.Input[str] value: Value of the key
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _ConfigState.__new__(_ConfigState)
 
         __props__.__dict__["key"] = key
-        __props__.__dict__["namespace"] = namespace
         __props__.__dict__["restart"] = restart
         __props__.__dict__["value"] = value
         return Config(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
     def key(self) -> pulumi.Output[str]:
         """
         Key of the config
         """
         return pulumi.get(self, "key")
 
     @property
     @pulumi.getter
-    def namespace(self) -> pulumi.Output[str]:
-        """
-        Namespace in which to install (Default: `kube-system`).
-        """
-        return pulumi.get(self, "namespace")
-
-    @property
-    @pulumi.getter
     def restart(self) -> pulumi.Output[bool]:
         """
         Restart Cilium pods (Default: `true`).
         """
         return pulumi.get(self, "restart")
 
     @property
```

### Comparing `littlejo_cilium-0.0.6/littlejo_cilium/hubble.py` & `littlejo_cilium-0.0.7/littlejo_cilium/hubble.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,44 +10,28 @@
 from . import _utilities
 
 __all__ = ['HubbleArgs', 'Hubble']
 
 @pulumi.input_type
 class HubbleArgs:
     def __init__(__self__, *,
-                 namespace: Optional[pulumi.Input[str]] = None,
                  relay: Optional[pulumi.Input[bool]] = None,
                  ui: Optional[pulumi.Input[bool]] = None):
         """
         The set of arguments for constructing a Hubble resource.
-        :param pulumi.Input[str] namespace: Namespace in which to install (Default: `kube-system`).
         :param pulumi.Input[bool] relay: Deploy Hubble Relay (Default: `true`).
         :param pulumi.Input[bool] ui: Enable Hubble UI (Default: `false`).
         """
-        if namespace is not None:
-            pulumi.set(__self__, "namespace", namespace)
         if relay is not None:
             pulumi.set(__self__, "relay", relay)
         if ui is not None:
             pulumi.set(__self__, "ui", ui)
 
     @property
     @pulumi.getter
-    def namespace(self) -> Optional[pulumi.Input[str]]:
-        """
-        Namespace in which to install (Default: `kube-system`).
-        """
-        return pulumi.get(self, "namespace")
-
-    @namespace.setter
-    def namespace(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "namespace", value)
-
-    @property
-    @pulumi.getter
     def relay(self) -> Optional[pulumi.Input[bool]]:
         """
         Deploy Hubble Relay (Default: `true`).
         """
         return pulumi.get(self, "relay")
 
     @relay.setter
@@ -66,44 +50,28 @@
     def ui(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "ui", value)
 
 
 @pulumi.input_type
 class _HubbleState:
     def __init__(__self__, *,
-                 namespace: Optional[pulumi.Input[str]] = None,
                  relay: Optional[pulumi.Input[bool]] = None,
                  ui: Optional[pulumi.Input[bool]] = None):
         """
         Input properties used for looking up and filtering Hubble resources.
-        :param pulumi.Input[str] namespace: Namespace in which to install (Default: `kube-system`).
         :param pulumi.Input[bool] relay: Deploy Hubble Relay (Default: `true`).
         :param pulumi.Input[bool] ui: Enable Hubble UI (Default: `false`).
         """
-        if namespace is not None:
-            pulumi.set(__self__, "namespace", namespace)
         if relay is not None:
             pulumi.set(__self__, "relay", relay)
         if ui is not None:
             pulumi.set(__self__, "ui", ui)
 
     @property
     @pulumi.getter
-    def namespace(self) -> Optional[pulumi.Input[str]]:
-        """
-        Namespace in which to install (Default: `kube-system`).
-        """
-        return pulumi.get(self, "namespace")
-
-    @namespace.setter
-    def namespace(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "namespace", value)
-
-    @property
-    @pulumi.getter
     def relay(self) -> Optional[pulumi.Input[bool]]:
         """
         Deploy Hubble Relay (Default: `true`).
         """
         return pulumi.get(self, "relay")
 
     @relay.setter
@@ -124,15 +92,14 @@
 
 
 class Hubble(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 namespace: Optional[pulumi.Input[str]] = None,
                  relay: Optional[pulumi.Input[bool]] = None,
                  ui: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
         """
         Hubble resource for Cilium. This is equivalent to cilium cli: `cilium hubble`: It manages cilium hubble
 
         ## Example Usage
@@ -142,15 +109,14 @@
         import littlejo_cilium as cilium
 
         example = cilium.Hubble("example", ui=True)
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] namespace: Namespace in which to install (Default: `kube-system`).
         :param pulumi.Input[bool] relay: Deploy Hubble Relay (Default: `true`).
         :param pulumi.Input[bool] ui: Enable Hubble UI (Default: `false`).
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
@@ -179,72 +145,59 @@
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 namespace: Optional[pulumi.Input[str]] = None,
                  relay: Optional[pulumi.Input[bool]] = None,
                  ui: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = HubbleArgs.__new__(HubbleArgs)
 
-            __props__.__dict__["namespace"] = namespace
             __props__.__dict__["relay"] = relay
             __props__.__dict__["ui"] = ui
         super(Hubble, __self__).__init__(
             'cilium:index/hubble:Hubble',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
-            namespace: Optional[pulumi.Input[str]] = None,
             relay: Optional[pulumi.Input[bool]] = None,
             ui: Optional[pulumi.Input[bool]] = None) -> 'Hubble':
         """
         Get an existing Hubble resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] namespace: Namespace in which to install (Default: `kube-system`).
         :param pulumi.Input[bool] relay: Deploy Hubble Relay (Default: `true`).
         :param pulumi.Input[bool] ui: Enable Hubble UI (Default: `false`).
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _HubbleState.__new__(_HubbleState)
 
-        __props__.__dict__["namespace"] = namespace
         __props__.__dict__["relay"] = relay
         __props__.__dict__["ui"] = ui
         return Hubble(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
-    def namespace(self) -> pulumi.Output[str]:
-        """
-        Namespace in which to install (Default: `kube-system`).
-        """
-        return pulumi.get(self, "namespace")
-
-    @property
-    @pulumi.getter
     def relay(self) -> pulumi.Output[bool]:
         """
         Deploy Hubble Relay (Default: `true`).
         """
         return pulumi.get(self, "relay")
 
     @property
```

### Comparing `littlejo_cilium-0.0.6/littlejo_cilium/install.py` & `littlejo_cilium-0.0.7/littlejo_cilium/install.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,45 +4,43 @@
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
+from . import outputs
+from ._inputs import *
 
 __all__ = ['InstallArgs', 'Install']
 
 @pulumi.input_type
 class InstallArgs:
     def __init__(__self__, *,
                  data_path: Optional[pulumi.Input[str]] = None,
-                 namespace: Optional[pulumi.Input[str]] = None,
                  repository: Optional[pulumi.Input[str]] = None,
                  reset: Optional[pulumi.Input[bool]] = None,
                  reuse: Optional[pulumi.Input[bool]] = None,
                  sets: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  values: Optional[pulumi.Input[str]] = None,
                  version: Optional[pulumi.Input[str]] = None,
                  wait: Optional[pulumi.Input[bool]] = None):
         """
         The set of arguments for constructing a Install resource.
         :param pulumi.Input[str] data_path: Datapath mode to use { tunnel | native | aws-eni | gke | azure | aks-byocni } (Default: `autodetected`).
-        :param pulumi.Input[str] namespace: Namespace in which to install (Default: `kube-system`).
         :param pulumi.Input[str] repository: Helm chart repository to download Cilium charts from (Default: `https://helm.cilium.io`).
         :param pulumi.Input[bool] reset: When upgrading, reset the helm values to the ones built into the chart (Default: `false`).
         :param pulumi.Input[bool] reuse: When upgrading, reuse the helm values from the latest release unless any overrides from are set from other flags. This option takes precedence over HelmResetValues (Default: `true`).
         :param pulumi.Input[Sequence[pulumi.Input[str]]] sets: Set helm values on the command line (can specify multiple or separate values with commas: key1=val1,key2=val2 (Default: `[]`).
         :param pulumi.Input[str] values: values in raw yaml to pass to helm. (Default: `empty`).
         :param pulumi.Input[str] version: Version of Cilium (Default: `v1.14.5`).
         :param pulumi.Input[bool] wait: Wait for Cilium status is ok (Default: `true`).
         """
         if data_path is not None:
             pulumi.set(__self__, "data_path", data_path)
-        if namespace is not None:
-            pulumi.set(__self__, "namespace", namespace)
         if repository is not None:
             pulumi.set(__self__, "repository", repository)
         if reset is not None:
             pulumi.set(__self__, "reset", reset)
         if reuse is not None:
             pulumi.set(__self__, "reuse", reuse)
         if sets is not None:
@@ -64,26 +62,14 @@
 
     @data_path.setter
     def data_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "data_path", value)
 
     @property
     @pulumi.getter
-    def namespace(self) -> Optional[pulumi.Input[str]]:
-        """
-        Namespace in which to install (Default: `kube-system`).
-        """
-        return pulumi.get(self, "namespace")
-
-    @namespace.setter
-    def namespace(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "namespace", value)
-
-    @property
-    @pulumi.getter
     def repository(self) -> Optional[pulumi.Input[str]]:
         """
         Helm chart repository to download Cilium charts from (Default: `https://helm.cilium.io`).
         """
         return pulumi.get(self, "repository")
 
     @repository.setter
@@ -162,39 +148,43 @@
     def wait(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "wait", value)
 
 
 @pulumi.input_type
 class _InstallState:
     def __init__(__self__, *,
+                 ca: Optional[pulumi.Input['InstallCaArgs']] = None,
                  data_path: Optional[pulumi.Input[str]] = None,
-                 namespace: Optional[pulumi.Input[str]] = None,
+                 helm_values: Optional[pulumi.Input[str]] = None,
                  repository: Optional[pulumi.Input[str]] = None,
                  reset: Optional[pulumi.Input[bool]] = None,
                  reuse: Optional[pulumi.Input[bool]] = None,
                  sets: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  values: Optional[pulumi.Input[str]] = None,
                  version: Optional[pulumi.Input[str]] = None,
                  wait: Optional[pulumi.Input[bool]] = None):
         """
         Input properties used for looking up and filtering Install resources.
+        :param pulumi.Input['InstallCaArgs'] ca: Cilium certificates value, Format: `{crt: "b64...", key: "b64.."}` (Equivalent to `kubectl get secret cilium-ca -n kube-system -o yaml`)
         :param pulumi.Input[str] data_path: Datapath mode to use { tunnel | native | aws-eni | gke | azure | aks-byocni } (Default: `autodetected`).
-        :param pulumi.Input[str] namespace: Namespace in which to install (Default: `kube-system`).
+        :param pulumi.Input[str] helm_values: Helm values (`helm get values -n kube-system cilium`)
         :param pulumi.Input[str] repository: Helm chart repository to download Cilium charts from (Default: `https://helm.cilium.io`).
         :param pulumi.Input[bool] reset: When upgrading, reset the helm values to the ones built into the chart (Default: `false`).
         :param pulumi.Input[bool] reuse: When upgrading, reuse the helm values from the latest release unless any overrides from are set from other flags. This option takes precedence over HelmResetValues (Default: `true`).
         :param pulumi.Input[Sequence[pulumi.Input[str]]] sets: Set helm values on the command line (can specify multiple or separate values with commas: key1=val1,key2=val2 (Default: `[]`).
         :param pulumi.Input[str] values: values in raw yaml to pass to helm. (Default: `empty`).
         :param pulumi.Input[str] version: Version of Cilium (Default: `v1.14.5`).
         :param pulumi.Input[bool] wait: Wait for Cilium status is ok (Default: `true`).
         """
+        if ca is not None:
+            pulumi.set(__self__, "ca", ca)
         if data_path is not None:
             pulumi.set(__self__, "data_path", data_path)
-        if namespace is not None:
-            pulumi.set(__self__, "namespace", namespace)
+        if helm_values is not None:
+            pulumi.set(__self__, "helm_values", helm_values)
         if repository is not None:
             pulumi.set(__self__, "repository", repository)
         if reset is not None:
             pulumi.set(__self__, "reset", reset)
         if reuse is not None:
             pulumi.set(__self__, "reuse", reuse)
         if sets is not None:
@@ -203,36 +193,48 @@
             pulumi.set(__self__, "values", values)
         if version is not None:
             pulumi.set(__self__, "version", version)
         if wait is not None:
             pulumi.set(__self__, "wait", wait)
 
     @property
+    @pulumi.getter
+    def ca(self) -> Optional[pulumi.Input['InstallCaArgs']]:
+        """
+        Cilium certificates value, Format: `{crt: "b64...", key: "b64.."}` (Equivalent to `kubectl get secret cilium-ca -n kube-system -o yaml`)
+        """
+        return pulumi.get(self, "ca")
+
+    @ca.setter
+    def ca(self, value: Optional[pulumi.Input['InstallCaArgs']]):
+        pulumi.set(self, "ca", value)
+
+    @property
     @pulumi.getter(name="dataPath")
     def data_path(self) -> Optional[pulumi.Input[str]]:
         """
         Datapath mode to use { tunnel | native | aws-eni | gke | azure | aks-byocni } (Default: `autodetected`).
         """
         return pulumi.get(self, "data_path")
 
     @data_path.setter
     def data_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "data_path", value)
 
     @property
-    @pulumi.getter
-    def namespace(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="helmValues")
+    def helm_values(self) -> Optional[pulumi.Input[str]]:
         """
-        Namespace in which to install (Default: `kube-system`).
+        Helm values (`helm get values -n kube-system cilium`)
         """
-        return pulumi.get(self, "namespace")
+        return pulumi.get(self, "helm_values")
 
-    @namespace.setter
-    def namespace(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "namespace", value)
+    @helm_values.setter
+    def helm_values(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "helm_values", value)
 
     @property
     @pulumi.getter
     def repository(self) -> Optional[pulumi.Input[str]]:
         """
         Helm chart repository to download Cilium charts from (Default: `https://helm.cilium.io`).
         """
@@ -317,63 +319,27 @@
 
 class Install(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  data_path: Optional[pulumi.Input[str]] = None,
-                 namespace: Optional[pulumi.Input[str]] = None,
                  repository: Optional[pulumi.Input[str]] = None,
                  reset: Optional[pulumi.Input[bool]] = None,
                  reuse: Optional[pulumi.Input[bool]] = None,
                  sets: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  values: Optional[pulumi.Input[str]] = None,
                  version: Optional[pulumi.Input[str]] = None,
                  wait: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
         """
-        Install resource for Cilium. This is equivalent to cilium cli: `cilium install`, `cilium upgrade` and `cilium uninstall`: It manages cilium helm chart
-
-        ## Example Usage
-
-        ```python
-        import pulumi
-        import littlejo_cilium as cilium
-        import pulumi_kind as kind
-
-        examplekind_cluster = kind.index.Kind_cluster("examplekind_cluster",
-            name=test-cluster,
-            kind_config=[{
-                kind: Cluster,
-                apiVersion: kind.x-k8s.io/v1alpha4,
-                node: [
-                    {
-                        role: control-plane,
-                    },
-                    {
-                        role: worker,
-                    },
-                ],
-                networking: [{
-                    disableDefaultCni: True,
-                }],
-            }])
-        example_install = cilium.Install("exampleInstall",
-            sets=[
-                "ipam.mode=kubernetes",
-                "ipam.operator.replicas=1",
-                "tunnel=vxlan",
-            ],
-            version="1.14.5")
-        ```
-
+        Create a Install resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] data_path: Datapath mode to use { tunnel | native | aws-eni | gke | azure | aks-byocni } (Default: `autodetected`).
-        :param pulumi.Input[str] namespace: Namespace in which to install (Default: `kube-system`).
         :param pulumi.Input[str] repository: Helm chart repository to download Cilium charts from (Default: `https://helm.cilium.io`).
         :param pulumi.Input[bool] reset: When upgrading, reset the helm values to the ones built into the chart (Default: `false`).
         :param pulumi.Input[bool] reuse: When upgrading, reuse the helm values from the latest release unless any overrides from are set from other flags. This option takes precedence over HelmResetValues (Default: `true`).
         :param pulumi.Input[Sequence[pulumi.Input[str]]] sets: Set helm values on the command line (can specify multiple or separate values with commas: key1=val1,key2=val2 (Default: `[]`).
         :param pulumi.Input[str] values: values in raw yaml to pass to helm. (Default: `empty`).
         :param pulumi.Input[str] version: Version of Cilium (Default: `v1.14.5`).
         :param pulumi.Input[bool] wait: Wait for Cilium status is ok (Default: `true`).
@@ -381,49 +347,15 @@
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: Optional[InstallArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Install resource for Cilium. This is equivalent to cilium cli: `cilium install`, `cilium upgrade` and `cilium uninstall`: It manages cilium helm chart
-
-        ## Example Usage
-
-        ```python
-        import pulumi
-        import littlejo_cilium as cilium
-        import pulumi_kind as kind
-
-        examplekind_cluster = kind.index.Kind_cluster("examplekind_cluster",
-            name=test-cluster,
-            kind_config=[{
-                kind: Cluster,
-                apiVersion: kind.x-k8s.io/v1alpha4,
-                node: [
-                    {
-                        role: control-plane,
-                    },
-                    {
-                        role: worker,
-                    },
-                ],
-                networking: [{
-                    disableDefaultCni: True,
-                }],
-            }])
-        example_install = cilium.Install("exampleInstall",
-            sets=[
-                "ipam.mode=kubernetes",
-                "ipam.operator.replicas=1",
-                "tunnel=vxlan",
-            ],
-            version="1.14.5")
-        ```
-
+        Create a Install resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
         :param InstallArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
         resource_args, opts = _utilities.get_resource_args_opts(InstallArgs, pulumi.ResourceOptions, *args, **kwargs)
@@ -432,15 +364,14 @@
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  data_path: Optional[pulumi.Input[str]] = None,
-                 namespace: Optional[pulumi.Input[str]] = None,
                  repository: Optional[pulumi.Input[str]] = None,
                  reset: Optional[pulumi.Input[bool]] = None,
                  reuse: Optional[pulumi.Input[bool]] = None,
                  sets: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  values: Optional[pulumi.Input[str]] = None,
                  version: Optional[pulumi.Input[str]] = None,
                  wait: Optional[pulumi.Input[bool]] = None,
@@ -450,88 +381,102 @@
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = InstallArgs.__new__(InstallArgs)
 
             __props__.__dict__["data_path"] = data_path
-            __props__.__dict__["namespace"] = namespace
             __props__.__dict__["repository"] = repository
             __props__.__dict__["reset"] = reset
             __props__.__dict__["reuse"] = reuse
             __props__.__dict__["sets"] = sets
             __props__.__dict__["values"] = values
             __props__.__dict__["version"] = version
             __props__.__dict__["wait"] = wait
+            __props__.__dict__["ca"] = None
+            __props__.__dict__["helm_values"] = None
+        secret_opts = pulumi.ResourceOptions(additional_secret_outputs=["ca"])
+        opts = pulumi.ResourceOptions.merge(opts, secret_opts)
         super(Install, __self__).__init__(
             'cilium:index/install:Install',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
+            ca: Optional[pulumi.Input[pulumi.InputType['InstallCaArgs']]] = None,
             data_path: Optional[pulumi.Input[str]] = None,
-            namespace: Optional[pulumi.Input[str]] = None,
+            helm_values: Optional[pulumi.Input[str]] = None,
             repository: Optional[pulumi.Input[str]] = None,
             reset: Optional[pulumi.Input[bool]] = None,
             reuse: Optional[pulumi.Input[bool]] = None,
             sets: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             values: Optional[pulumi.Input[str]] = None,
             version: Optional[pulumi.Input[str]] = None,
             wait: Optional[pulumi.Input[bool]] = None) -> 'Install':
         """
         Get an existing Install resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
+        :param pulumi.Input[pulumi.InputType['InstallCaArgs']] ca: Cilium certificates value, Format: `{crt: "b64...", key: "b64.."}` (Equivalent to `kubectl get secret cilium-ca -n kube-system -o yaml`)
         :param pulumi.Input[str] data_path: Datapath mode to use { tunnel | native | aws-eni | gke | azure | aks-byocni } (Default: `autodetected`).
-        :param pulumi.Input[str] namespace: Namespace in which to install (Default: `kube-system`).
+        :param pulumi.Input[str] helm_values: Helm values (`helm get values -n kube-system cilium`)
         :param pulumi.Input[str] repository: Helm chart repository to download Cilium charts from (Default: `https://helm.cilium.io`).
         :param pulumi.Input[bool] reset: When upgrading, reset the helm values to the ones built into the chart (Default: `false`).
         :param pulumi.Input[bool] reuse: When upgrading, reuse the helm values from the latest release unless any overrides from are set from other flags. This option takes precedence over HelmResetValues (Default: `true`).
         :param pulumi.Input[Sequence[pulumi.Input[str]]] sets: Set helm values on the command line (can specify multiple or separate values with commas: key1=val1,key2=val2 (Default: `[]`).
         :param pulumi.Input[str] values: values in raw yaml to pass to helm. (Default: `empty`).
         :param pulumi.Input[str] version: Version of Cilium (Default: `v1.14.5`).
         :param pulumi.Input[bool] wait: Wait for Cilium status is ok (Default: `true`).
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _InstallState.__new__(_InstallState)
 
+        __props__.__dict__["ca"] = ca
         __props__.__dict__["data_path"] = data_path
-        __props__.__dict__["namespace"] = namespace
+        __props__.__dict__["helm_values"] = helm_values
         __props__.__dict__["repository"] = repository
         __props__.__dict__["reset"] = reset
         __props__.__dict__["reuse"] = reuse
         __props__.__dict__["sets"] = sets
         __props__.__dict__["values"] = values
         __props__.__dict__["version"] = version
         __props__.__dict__["wait"] = wait
         return Install(resource_name, opts=opts, __props__=__props__)
 
     @property
+    @pulumi.getter
+    def ca(self) -> pulumi.Output['outputs.InstallCa']:
+        """
+        Cilium certificates value, Format: `{crt: "b64...", key: "b64.."}` (Equivalent to `kubectl get secret cilium-ca -n kube-system -o yaml`)
+        """
+        return pulumi.get(self, "ca")
+
+    @property
     @pulumi.getter(name="dataPath")
     def data_path(self) -> pulumi.Output[str]:
         """
         Datapath mode to use { tunnel | native | aws-eni | gke | azure | aks-byocni } (Default: `autodetected`).
         """
         return pulumi.get(self, "data_path")
 
     @property
-    @pulumi.getter
-    def namespace(self) -> pulumi.Output[str]:
+    @pulumi.getter(name="helmValues")
+    def helm_values(self) -> pulumi.Output[str]:
         """
-        Namespace in which to install (Default: `kube-system`).
+        Helm values (`helm get values -n kube-system cilium`)
         """
-        return pulumi.get(self, "namespace")
+        return pulumi.get(self, "helm_values")
 
     @property
     @pulumi.getter
     def repository(self) -> pulumi.Output[str]:
         """
         Helm chart repository to download Cilium charts from (Default: `https://helm.cilium.io`).
         """
```

### Comparing `littlejo_cilium-0.0.6/littlejo_cilium/kubeproxy_free.py` & `littlejo_cilium-0.0.7/littlejo_cilium/kubeproxy_free.py`

 * *Files identical despite different names*

### Comparing `littlejo_cilium-0.0.6/littlejo_cilium/provider.py` & `littlejo_cilium-0.0.7/littlejo_cilium/provider.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,31 +10,51 @@
 from . import _utilities
 
 __all__ = ['ProviderArgs', 'Provider']
 
 @pulumi.input_type
 class ProviderArgs:
     def __init__(__self__, *,
+                 config_content: Optional[pulumi.Input[str]] = None,
                  config_path: Optional[pulumi.Input[str]] = None,
                  context: Optional[pulumi.Input[str]] = None,
+                 helm_release: Optional[pulumi.Input[str]] = None,
                  namespace: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a Provider resource.
+        :param pulumi.Input[str] config_content: The content of kube config file (Default: ``).
         :param pulumi.Input[str] config_path: A path to a kube config file (Default: `~/.kube/config`).
         :param pulumi.Input[str] context: Context of kubeconfig file (Default: `default context`).
+        :param pulumi.Input[str] helm_release: Helm Release to install cilium (Default: `Install`).
         :param pulumi.Input[str] namespace: Namespace to install cilium (Default: `kube-system`).
         """
+        if config_content is not None:
+            pulumi.set(__self__, "config_content", config_content)
         if config_path is not None:
             pulumi.set(__self__, "config_path", config_path)
         if context is not None:
             pulumi.set(__self__, "context", context)
+        if helm_release is not None:
+            pulumi.set(__self__, "helm_release", helm_release)
         if namespace is not None:
             pulumi.set(__self__, "namespace", namespace)
 
     @property
+    @pulumi.getter(name="configContent")
+    def config_content(self) -> Optional[pulumi.Input[str]]:
+        """
+        The content of kube config file (Default: ``).
+        """
+        return pulumi.get(self, "config_content")
+
+    @config_content.setter
+    def config_content(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "config_content", value)
+
+    @property
     @pulumi.getter(name="configPath")
     def config_path(self) -> Optional[pulumi.Input[str]]:
         """
         A path to a kube config file (Default: `~/.kube/config`).
         """
         return pulumi.get(self, "config_path")
 
@@ -51,14 +71,26 @@
         return pulumi.get(self, "context")
 
     @context.setter
     def context(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "context", value)
 
     @property
+    @pulumi.getter(name="helmRelease")
+    def helm_release(self) -> Optional[pulumi.Input[str]]:
+        """
+        Helm Release to install cilium (Default: `Install`).
+        """
+        return pulumi.get(self, "helm_release")
+
+    @helm_release.setter
+    def helm_release(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "helm_release", value)
+
+    @property
     @pulumi.getter
     def namespace(self) -> Optional[pulumi.Input[str]]:
         """
         Namespace to install cilium (Default: `kube-system`).
         """
         return pulumi.get(self, "namespace")
 
@@ -68,28 +100,32 @@
 
 
 class Provider(pulumi.ProviderResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
+                 config_content: Optional[pulumi.Input[str]] = None,
                  config_path: Optional[pulumi.Input[str]] = None,
                  context: Optional[pulumi.Input[str]] = None,
+                 helm_release: Optional[pulumi.Input[str]] = None,
                  namespace: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         The provider type for the cilium package. By default, resources use package-wide configuration
         settings, however an explicit `Provider` instance may be created and passed during resource
         construction to achieve fine-grained programmatic control over provider settings. See the
         [documentation](https://www.pulumi.com/docs/reference/programming-model/#providers) for more information.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
+        :param pulumi.Input[str] config_content: The content of kube config file (Default: ``).
         :param pulumi.Input[str] config_path: A path to a kube config file (Default: `~/.kube/config`).
         :param pulumi.Input[str] context: Context of kubeconfig file (Default: `default context`).
+        :param pulumi.Input[str] helm_release: Helm Release to install cilium (Default: `Install`).
         :param pulumi.Input[str] namespace: Namespace to install cilium (Default: `kube-system`).
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: Optional[ProviderArgs] = None,
@@ -111,36 +147,48 @@
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
+                 config_content: Optional[pulumi.Input[str]] = None,
                  config_path: Optional[pulumi.Input[str]] = None,
                  context: Optional[pulumi.Input[str]] = None,
+                 helm_release: Optional[pulumi.Input[str]] = None,
                  namespace: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ProviderArgs.__new__(ProviderArgs)
 
+            __props__.__dict__["config_content"] = config_content
             __props__.__dict__["config_path"] = config_path
             __props__.__dict__["context"] = context
+            __props__.__dict__["helm_release"] = helm_release
             __props__.__dict__["namespace"] = namespace
         super(Provider, __self__).__init__(
             'cilium',
             resource_name,
             __props__,
             opts)
 
     @property
+    @pulumi.getter(name="configContent")
+    def config_content(self) -> pulumi.Output[Optional[str]]:
+        """
+        The content of kube config file (Default: ``).
+        """
+        return pulumi.get(self, "config_content")
+
+    @property
     @pulumi.getter(name="configPath")
     def config_path(self) -> pulumi.Output[Optional[str]]:
         """
         A path to a kube config file (Default: `~/.kube/config`).
         """
         return pulumi.get(self, "config_path")
 
@@ -149,14 +197,22 @@
     def context(self) -> pulumi.Output[Optional[str]]:
         """
         Context of kubeconfig file (Default: `default context`).
         """
         return pulumi.get(self, "context")
 
     @property
+    @pulumi.getter(name="helmRelease")
+    def helm_release(self) -> pulumi.Output[Optional[str]]:
+        """
+        Helm Release to install cilium (Default: `Install`).
+        """
+        return pulumi.get(self, "helm_release")
+
+    @property
     @pulumi.getter
     def namespace(self) -> pulumi.Output[Optional[str]]:
         """
         Namespace to install cilium (Default: `kube-system`).
         """
         return pulumi.get(self, "namespace")
```

### Comparing `littlejo_cilium-0.0.6/littlejo_cilium.egg-info/PKG-INFO` & `littlejo_cilium-0.0.7/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
-Name: littlejo-cilium
-Version: 0.0.6
+Name: littlejo_cilium
+Version: 0.0.7
 Summary: A Pulumi package for creating and managing Cilium resources
 Home-page: https://github.com/littlejo/pulumi-cilium
 License: Apache-2.0
 Project-URL: Repository, https://github.com/littlejo/pulumi-cilium
 Keywords: pulumi cilium category/network
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # Cilium Resource Provider
 
 The Cilium Resource Provider lets you manage [cilium](https://www.pulumi.com/registry/packages/cilium/) resources.
 
 ## Installing
```

### Comparing `littlejo_cilium-0.0.6/littlejo_cilium.egg-info/SOURCES.txt` & `littlejo_cilium-0.0.7/littlejo_cilium.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 README.md
 setup.py
 littlejo_cilium/__init__.py
+littlejo_cilium/_inputs.py
 littlejo_cilium/_utilities.py
 littlejo_cilium/clustermesh.py
 littlejo_cilium/clustermesh_connection.py
 littlejo_cilium/config.py
+littlejo_cilium/deploy.py
 littlejo_cilium/get_helm_values.py
 littlejo_cilium/hubble.py
 littlejo_cilium/install.py
 littlejo_cilium/kubeproxy_free.py
+littlejo_cilium/outputs.py
 littlejo_cilium/provider.py
 littlejo_cilium/pulumi-plugin.json
 littlejo_cilium/py.typed
 littlejo_cilium.egg-info/PKG-INFO
 littlejo_cilium.egg-info/SOURCES.txt
 littlejo_cilium.egg-info/dependency_links.txt
 littlejo_cilium.egg-info/not-zip-safe
```

### Comparing `littlejo_cilium-0.0.6/setup.py` & `littlejo_cilium-0.0.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.0.6"
+VERSION = "0.0.7"
 def readme():
     try:
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "cilium Pulumi Package - Development Version"
 
 
 setup(name='littlejo_cilium',
-      python_requires='>=3.7',
+      python_requires='>=3.8',
       version=VERSION,
       description="A Pulumi package for creating and managing Cilium resources",
       long_description=readme(),
       long_description_content_type='text/markdown',
       keywords='pulumi cilium category/network',
       url='https://github.com/littlejo/pulumi-cilium',
       project_urls={
```

