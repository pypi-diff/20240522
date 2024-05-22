# Comparing `tmp/pulumi_eks-2.4.0a1715798612.tar.gz` & `tmp/pulumi_eks-2.5.0a1716314787.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_eks-2.4.0a1715798612.tar", last modified: Wed May 15 18:48:46 2024, max compression
+gzip compressed data, was "pulumi_eks-2.5.0a1716314787.tar", last modified: Tue May 21 18:10:51 2024, max compression
```

## Comparing `pulumi_eks-2.4.0a1715798612.tar` & `pulumi_eks-2.5.0a1716314787.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:48:46.622979 pulumi_eks-2.4.0a1715798612/
--rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-05-15 18:48:46.622979 pulumi_eks-2.4.0a1715798612/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-15 18:48:36.000000 pulumi_eks-2.4.0a1715798612/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:48:46.618980 pulumi_eks-2.4.0a1715798612/pulumi_eks/
--rw-------   0 runner    (1001) docker     (127)     1150 2024-05-15 18:48:36.000000 pulumi_eks-2.4.0a1715798612/pulumi_eks/__init__.py
--rw-------   0 runner    (1001) docker     (127)    89785 2024-05-15 18:48:36.000000 pulumi_eks-2.4.0a1715798612/pulumi_eks/_inputs.py
--rw-------   0 runner    (1001) docker     (127)     9222 2024-05-15 18:48:36.000000 pulumi_eks-2.4.0a1715798612/pulumi_eks/_utilities.py
--rw-------   0 runner    (1001) docker     (127)    95529 2024-05-15 18:48:36.000000 pulumi_eks-2.4.0a1715798612/pulumi_eks/cluster.py
--rw-------   0 runner    (1001) docker     (127)     4860 2024-05-15 18:48:36.000000 pulumi_eks-2.4.0a1715798612/pulumi_eks/cluster_creation_role_provider.py
--rw-------   0 runner    (1001) docker     (127)    30218 2024-05-15 18:48:36.000000 pulumi_eks-2.4.0a1715798612/pulumi_eks/managed_node_group.py
--rw-------   0 runner    (1001) docker     (127)    48913 2024-05-15 18:48:36.000000 pulumi_eks-2.4.0a1715798612/pulumi_eks/node_group.py
--rw-------   0 runner    (1001) docker     (127)     8405 2024-05-15 18:48:36.000000 pulumi_eks-2.4.0a1715798612/pulumi_eks/node_group_security_group.py
--rw-------   0 runner    (1001) docker     (127)    51825 2024-05-15 18:48:36.000000 pulumi_eks-2.4.0a1715798612/pulumi_eks/node_group_v2.py
--rw-------   0 runner    (1001) docker     (127)    42512 2024-05-15 18:48:36.000000 pulumi_eks-2.4.0a1715798612/pulumi_eks/outputs.py
--rw-------   0 runner    (1001) docker     (127)     2715 2024-05-15 18:48:36.000000 pulumi_eks-2.4.0a1715798612/pulumi_eks/provider.py
--rw-------   0 runner    (1001) docker     (127)       40 2024-05-15 18:48:36.000000 pulumi_eks-2.4.0a1715798612/pulumi_eks/pulumi-plugin.json
--rw-------   0 runner    (1001) docker     (127)        0 2024-05-15 18:48:36.000000 pulumi_eks-2.4.0a1715798612/pulumi_eks/py.typed
--rw-------   0 runner    (1001) docker     (127)    39043 2024-05-15 18:48:36.000000 pulumi_eks-2.4.0a1715798612/pulumi_eks/vpc_cni.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:48:46.622979 pulumi_eks-2.4.0a1715798612/pulumi_eks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-05-15 18:48:46.000000 pulumi_eks-2.4.0a1715798612/pulumi_eks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-15 18:48:46.000000 pulumi_eks-2.4.0a1715798612/pulumi_eks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 18:48:46.000000 pulumi_eks-2.4.0a1715798612/pulumi_eks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-15 18:48:46.000000 pulumi_eks-2.4.0a1715798612/pulumi_eks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-15 18:48:46.000000 pulumi_eks-2.4.0a1715798612/pulumi_eks.egg-info/top_level.txt
--rw-------   0 runner    (1001) docker     (127)      720 2024-05-15 18:48:36.000000 pulumi_eks-2.4.0a1715798612/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 18:48:46.622979 pulumi_eks-2.4.0a1715798612/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:10:50.995811 pulumi_eks-2.5.0a1716314787/
+-rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-05-21 18:10:50.995811 pulumi_eks-2.5.0a1716314787/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-21 18:10:44.000000 pulumi_eks-2.5.0a1716314787/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:10:50.995811 pulumi_eks-2.5.0a1716314787/pulumi_eks/
+-rw-------   0 runner    (1001) docker     (127)     1150 2024-05-21 18:10:44.000000 pulumi_eks-2.5.0a1716314787/pulumi_eks/__init__.py
+-rw-------   0 runner    (1001) docker     (127)    89785 2024-05-21 18:10:44.000000 pulumi_eks-2.5.0a1716314787/pulumi_eks/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)     9222 2024-05-21 18:10:44.000000 pulumi_eks-2.5.0a1716314787/pulumi_eks/_utilities.py
+-rw-------   0 runner    (1001) docker     (127)    95529 2024-05-21 18:10:44.000000 pulumi_eks-2.5.0a1716314787/pulumi_eks/cluster.py
+-rw-------   0 runner    (1001) docker     (127)     4860 2024-05-21 18:10:44.000000 pulumi_eks-2.5.0a1716314787/pulumi_eks/cluster_creation_role_provider.py
+-rw-------   0 runner    (1001) docker     (127)    36848 2024-05-21 18:10:44.000000 pulumi_eks-2.5.0a1716314787/pulumi_eks/managed_node_group.py
+-rw-------   0 runner    (1001) docker     (127)    48913 2024-05-21 18:10:44.000000 pulumi_eks-2.5.0a1716314787/pulumi_eks/node_group.py
+-rw-------   0 runner    (1001) docker     (127)     8405 2024-05-21 18:10:44.000000 pulumi_eks-2.5.0a1716314787/pulumi_eks/node_group_security_group.py
+-rw-------   0 runner    (1001) docker     (127)    51825 2024-05-21 18:10:44.000000 pulumi_eks-2.5.0a1716314787/pulumi_eks/node_group_v2.py
+-rw-------   0 runner    (1001) docker     (127)    42512 2024-05-21 18:10:44.000000 pulumi_eks-2.5.0a1716314787/pulumi_eks/outputs.py
+-rw-------   0 runner    (1001) docker     (127)     2715 2024-05-21 18:10:44.000000 pulumi_eks-2.5.0a1716314787/pulumi_eks/provider.py
+-rw-------   0 runner    (1001) docker     (127)       40 2024-05-21 18:10:44.000000 pulumi_eks-2.5.0a1716314787/pulumi_eks/pulumi-plugin.json
+-rw-------   0 runner    (1001) docker     (127)        0 2024-05-21 18:10:44.000000 pulumi_eks-2.5.0a1716314787/pulumi_eks/py.typed
+-rw-------   0 runner    (1001) docker     (127)    39043 2024-05-21 18:10:44.000000 pulumi_eks-2.5.0a1716314787/pulumi_eks/vpc_cni.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:10:50.995811 pulumi_eks-2.5.0a1716314787/pulumi_eks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-05-21 18:10:50.000000 pulumi_eks-2.5.0a1716314787/pulumi_eks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-21 18:10:50.000000 pulumi_eks-2.5.0a1716314787/pulumi_eks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 18:10:50.000000 pulumi_eks-2.5.0a1716314787/pulumi_eks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-21 18:10:50.000000 pulumi_eks-2.5.0a1716314787/pulumi_eks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-21 18:10:50.000000 pulumi_eks-2.5.0a1716314787/pulumi_eks.egg-info/top_level.txt
+-rw-------   0 runner    (1001) docker     (127)      720 2024-05-21 18:10:44.000000 pulumi_eks-2.5.0a1716314787/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 18:10:50.995811 pulumi_eks-2.5.0a1716314787/setup.cfg
```

### Comparing `pulumi_eks-2.4.0a1715798612/PKG-INFO` & `pulumi_eks-2.5.0a1716314787/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_eks
-Version: 2.4.0a1715798612
+Version: 2.5.0a1716314787
 Summary: Pulumi Amazon Web Services (AWS) EKS Components.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.com
 Project-URL: Repository, https://github.com/pulumi/pulumi-eks
 Keywords: pulumi,aws,eks
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pulumi_eks Version: 2.4.0a1715798612 Summary:
+Metadata-Version: 2.1 Name: pulumi_eks Version: 2.5.0a1716314787 Summary:
 Pulumi Amazon Web Services (AWS) EKS Components. License: Apache-2.0 Project-
 URL: Homepage, https://pulumi.com Project-URL: Repository, https://github.com/
 pulumi/pulumi-eks Keywords: pulumi,aws,eks Requires-Python: >=3.8 Description-
 Content-Type: text/markdown Requires-Dist: parver>=0.2.1 Requires-Dist:
 pulumi<4.0.0,>=3.0.0 Requires-Dist: pulumi-aws<7.0.0,>=6.0.0 Requires-Dist:
 pulumi-kubernetes<5.0.0,>=4.0.0 Requires-Dist: semver>=2.8.1 [![Build Status]
 (https://github.com/pulumi/pulumi-eks/actions/workflows/master.yml/badge.svg)]
```

### Comparing `pulumi_eks-2.4.0a1715798612/README.md` & `pulumi_eks-2.5.0a1716314787/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_eks-2.4.0a1715798612/pulumi_eks/__init__.py` & `pulumi_eks-2.5.0a1716314787/pulumi_eks/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_eks-2.4.0a1715798612/pulumi_eks/_inputs.py` & `pulumi_eks-2.5.0a1716314787/pulumi_eks/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_eks-2.4.0a1715798612/pulumi_eks/_utilities.py` & `pulumi_eks-2.5.0a1716314787/pulumi_eks/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_eks-2.4.0a1715798612/pulumi_eks/cluster.py` & `pulumi_eks-2.5.0a1716314787/pulumi_eks/cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_eks-2.4.0a1715798612/pulumi_eks/cluster_creation_role_provider.py` & `pulumi_eks-2.5.0a1716314787/pulumi_eks/cluster_creation_role_provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_eks-2.4.0a1715798612/pulumi_eks/managed_node_group.py` & `pulumi_eks-2.5.0a1716314787/pulumi_eks/managed_node_group.py`

 * *Files 19% similar despite different names*

```diff
@@ -17,19 +17,22 @@
 __all__ = ['ManagedNodeGroupArgs', 'ManagedNodeGroup']
 
 @pulumi.input_type
 class ManagedNodeGroupArgs:
     def __init__(__self__, *,
                  cluster: pulumi.Input[Union['Cluster', 'CoreDataArgs']],
                  ami_type: Optional[pulumi.Input[str]] = None,
+                 bootstrap_extra_args: Optional[str] = None,
                  capacity_type: Optional[pulumi.Input[str]] = None,
                  cluster_name: Optional[pulumi.Input[str]] = None,
                  disk_size: Optional[pulumi.Input[int]] = None,
+                 enable_imd_sv2: Optional[bool] = None,
                  force_update_version: Optional[pulumi.Input[bool]] = None,
                  instance_types: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 kubelet_extra_args: Optional[str] = None,
                  labels: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  launch_template: Optional[pulumi.Input['pulumi_aws.eks.NodeGroupLaunchTemplateArgs']] = None,
                  node_group_name: Optional[pulumi.Input[str]] = None,
                  node_group_name_prefix: Optional[pulumi.Input[str]] = None,
                  node_role: Optional[pulumi.Input['pulumi_aws.iam.Role']] = None,
                  node_role_arn: Optional[pulumi.Input[str]] = None,
                  release_version: Optional[pulumi.Input[str]] = None,
@@ -39,21 +42,32 @@
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  taints: Optional[pulumi.Input[Sequence[pulumi.Input['pulumi_aws.eks.NodeGroupTaintArgs']]]] = None,
                  version: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a ManagedNodeGroup resource.
         :param pulumi.Input[Union['Cluster', 'CoreDataArgs']] cluster: The target EKS cluster.
         :param pulumi.Input[str] ami_type: Type of Amazon Machine Image (AMI) associated with the EKS Node Group. Defaults to `AL2_x86_64`. See the AWS documentation (https://docs.aws.amazon.com/eks/latest/APIReference/API_Nodegroup.html#AmazonEKS-Type-Nodegroup-amiType) for valid AMI Types. This provider will only perform drift detection if a configuration value is provided.
+        :param str bootstrap_extra_args: Additional args to pass directly to `/etc/eks/bootstrap.sh`. For details on available options, see: https://github.com/awslabs/amazon-eks-ami/blob/master/files/bootstrap.sh. Note that the `--apiserver-endpoint`, `--b64-cluster-ca` and `--kubelet-extra-args` flags are included automatically based on other configuration parameters.
+               
+               Note that this field conflicts with `launchTemplate`.
         :param pulumi.Input[str] capacity_type: Type of capacity associated with the EKS Node Group. Valid values: `ON_DEMAND`, `SPOT`. This provider will only perform drift detection if a configuration value is provided.
         :param pulumi.Input[str] cluster_name: Name of the EKS Cluster.
         :param pulumi.Input[int] disk_size: Disk size in GiB for worker nodes. Defaults to `20`. This provider will only perform drift detection if a configuration value is provided.
+        :param bool enable_imd_sv2: Enables the ability to use EC2 Instance Metadata Service v2, which provides a more secure way to access instance metadata. For more information, see: https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/configuring-instance-metadata-service.html.
+               Defaults to `false`.
+               
+               Note that this field conflicts with `launchTemplate`. If you are providing a custom `launchTemplate`, you should enable this feature within the `launchTemplateMetadataOptions` of the supplied `launchTemplate`.
         :param pulumi.Input[bool] force_update_version: Force version update if existing pods are unable to be drained due to a pod disruption budget issue.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] instance_types: Set of instance types associated with the EKS Node Group. Defaults to `["t3.medium"]`. This provider will only perform drift detection if a configuration value is provided. Currently, the EKS API only accepts a single value in the set.
+        :param str kubelet_extra_args: Extra args to pass to the Kubelet. Corresponds to the options passed in the `--kubeletExtraArgs` flag to `/etc/eks/bootstrap.sh`. For example, '--port=10251 --address=0.0.0.0'. To escape characters in the extra argsvalue, wrap the value in quotes. For example, `kubeletExtraArgs = '--allowed-unsafe-sysctls "net.core.somaxconn"'`.
+               Note that this field conflicts with `launchTemplate`.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: Key-value map of Kubernetes labels. Only labels that are applied with the EKS API are managed by this argument. Other Kubernetes labels applied to the EKS Node Group will not be managed.
         :param pulumi.Input['pulumi_aws.eks.NodeGroupLaunchTemplateArgs'] launch_template: Launch Template settings.
+               
+               Note: This field is mutually exclusive with `kubeletExtraArgs` and `bootstrapExtraArgs`.
         :param pulumi.Input[str] node_group_name: Name of the EKS Node Group. If omitted, this provider will assign a random, unique name. Conflicts with `nodeGroupNamePrefix`.
         :param pulumi.Input[str] node_group_name_prefix: Creates a unique name beginning with the specified prefix. Conflicts with `nodeGroupName`.
         :param pulumi.Input['pulumi_aws.iam.Role'] node_role: The IAM Role that provides permissions for the EKS Node Group.
                
                Note, `nodeRole` and `nodeRoleArn` are mutually exclusive, and a single option must be used.
         :param pulumi.Input[str] node_role_arn: Amazon Resource Name (ARN) of the IAM Role that provides permissions for the EKS Node Group.
                
@@ -76,24 +90,30 @@
                This default logic is based on the existing subnet IDs logic of this package: https://git.io/JeM11
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Key-value mapping of resource tags.
         :param pulumi.Input[Sequence[pulumi.Input['pulumi_aws.eks.NodeGroupTaintArgs']]] taints: The Kubernetes taints to be applied to the nodes in the node group. Maximum of 50 taints per node group.
         """
         pulumi.set(__self__, "cluster", cluster)
         if ami_type is not None:
             pulumi.set(__self__, "ami_type", ami_type)
+        if bootstrap_extra_args is not None:
+            pulumi.set(__self__, "bootstrap_extra_args", bootstrap_extra_args)
         if capacity_type is not None:
             pulumi.set(__self__, "capacity_type", capacity_type)
         if cluster_name is not None:
             pulumi.set(__self__, "cluster_name", cluster_name)
         if disk_size is not None:
             pulumi.set(__self__, "disk_size", disk_size)
+        if enable_imd_sv2 is not None:
+            pulumi.set(__self__, "enable_imd_sv2", enable_imd_sv2)
         if force_update_version is not None:
             pulumi.set(__self__, "force_update_version", force_update_version)
         if instance_types is not None:
             pulumi.set(__self__, "instance_types", instance_types)
+        if kubelet_extra_args is not None:
+            pulumi.set(__self__, "kubelet_extra_args", kubelet_extra_args)
         if labels is not None:
             pulumi.set(__self__, "labels", labels)
         if launch_template is not None:
             pulumi.set(__self__, "launch_template", launch_template)
         if node_group_name is not None:
             pulumi.set(__self__, "node_group_name", node_group_name)
         if node_group_name_prefix is not None:
@@ -138,14 +158,28 @@
         return pulumi.get(self, "ami_type")
 
     @ami_type.setter
     def ami_type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "ami_type", value)
 
     @property
+    @pulumi.getter(name="bootstrapExtraArgs")
+    def bootstrap_extra_args(self) -> Optional[str]:
+        """
+        Additional args to pass directly to `/etc/eks/bootstrap.sh`. For details on available options, see: https://github.com/awslabs/amazon-eks-ami/blob/master/files/bootstrap.sh. Note that the `--apiserver-endpoint`, `--b64-cluster-ca` and `--kubelet-extra-args` flags are included automatically based on other configuration parameters.
+
+        Note that this field conflicts with `launchTemplate`.
+        """
+        return pulumi.get(self, "bootstrap_extra_args")
+
+    @bootstrap_extra_args.setter
+    def bootstrap_extra_args(self, value: Optional[str]):
+        pulumi.set(self, "bootstrap_extra_args", value)
+
+    @property
     @pulumi.getter(name="capacityType")
     def capacity_type(self) -> Optional[pulumi.Input[str]]:
         """
         Type of capacity associated with the EKS Node Group. Valid values: `ON_DEMAND`, `SPOT`. This provider will only perform drift detection if a configuration value is provided.
         """
         return pulumi.get(self, "capacity_type")
 
@@ -174,14 +208,29 @@
         return pulumi.get(self, "disk_size")
 
     @disk_size.setter
     def disk_size(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "disk_size", value)
 
     @property
+    @pulumi.getter(name="enableIMDSv2")
+    def enable_imd_sv2(self) -> Optional[bool]:
+        """
+        Enables the ability to use EC2 Instance Metadata Service v2, which provides a more secure way to access instance metadata. For more information, see: https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/configuring-instance-metadata-service.html.
+        Defaults to `false`.
+
+        Note that this field conflicts with `launchTemplate`. If you are providing a custom `launchTemplate`, you should enable this feature within the `launchTemplateMetadataOptions` of the supplied `launchTemplate`.
+        """
+        return pulumi.get(self, "enable_imd_sv2")
+
+    @enable_imd_sv2.setter
+    def enable_imd_sv2(self, value: Optional[bool]):
+        pulumi.set(self, "enable_imd_sv2", value)
+
+    @property
     @pulumi.getter(name="forceUpdateVersion")
     def force_update_version(self) -> Optional[pulumi.Input[bool]]:
         """
         Force version update if existing pods are unable to be drained due to a pod disruption budget issue.
         """
         return pulumi.get(self, "force_update_version")
 
@@ -198,14 +247,27 @@
         return pulumi.get(self, "instance_types")
 
     @instance_types.setter
     def instance_types(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "instance_types", value)
 
     @property
+    @pulumi.getter(name="kubeletExtraArgs")
+    def kubelet_extra_args(self) -> Optional[str]:
+        """
+        Extra args to pass to the Kubelet. Corresponds to the options passed in the `--kubeletExtraArgs` flag to `/etc/eks/bootstrap.sh`. For example, '--port=10251 --address=0.0.0.0'. To escape characters in the extra argsvalue, wrap the value in quotes. For example, `kubeletExtraArgs = '--allowed-unsafe-sysctls "net.core.somaxconn"'`.
+        Note that this field conflicts with `launchTemplate`.
+        """
+        return pulumi.get(self, "kubelet_extra_args")
+
+    @kubelet_extra_args.setter
+    def kubelet_extra_args(self, value: Optional[str]):
+        pulumi.set(self, "kubelet_extra_args", value)
+
+    @property
     @pulumi.getter
     def labels(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Key-value map of Kubernetes labels. Only labels that are applied with the EKS API are managed by this argument. Other Kubernetes labels applied to the EKS Node Group will not be managed.
         """
         return pulumi.get(self, "labels")
 
@@ -214,14 +276,16 @@
         pulumi.set(self, "labels", value)
 
     @property
     @pulumi.getter(name="launchTemplate")
     def launch_template(self) -> Optional[pulumi.Input['pulumi_aws.eks.NodeGroupLaunchTemplateArgs']]:
         """
         Launch Template settings.
+
+        Note: This field is mutually exclusive with `kubeletExtraArgs` and `bootstrapExtraArgs`.
         """
         return pulumi.get(self, "launch_template")
 
     @launch_template.setter
     def launch_template(self, value: Optional[pulumi.Input['pulumi_aws.eks.NodeGroupLaunchTemplateArgs']]):
         pulumi.set(self, "launch_template", value)
 
@@ -373,20 +437,23 @@
 
 class ManagedNodeGroup(pulumi.ComponentResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  ami_type: Optional[pulumi.Input[str]] = None,
+                 bootstrap_extra_args: Optional[str] = None,
                  capacity_type: Optional[pulumi.Input[str]] = None,
                  cluster: Optional[pulumi.Input[Union['Cluster', pulumi.InputType['CoreDataArgs']]]] = None,
                  cluster_name: Optional[pulumi.Input[str]] = None,
                  disk_size: Optional[pulumi.Input[int]] = None,
+                 enable_imd_sv2: Optional[bool] = None,
                  force_update_version: Optional[pulumi.Input[bool]] = None,
                  instance_types: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 kubelet_extra_args: Optional[str] = None,
                  labels: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  launch_template: Optional[pulumi.Input[pulumi.InputType['pulumi_aws.eks.NodeGroupLaunchTemplateArgs']]] = None,
                  node_group_name: Optional[pulumi.Input[str]] = None,
                  node_group_name_prefix: Optional[pulumi.Input[str]] = None,
                  node_role: Optional[pulumi.Input['pulumi_aws.iam.Role']] = None,
                  node_role_arn: Optional[pulumi.Input[str]] = None,
                  release_version: Optional[pulumi.Input[str]] = None,
@@ -402,22 +469,33 @@
 
         See for more details:
         https://docs.aws.amazon.com/eks/latest/userguide/managed-node-groups.html
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] ami_type: Type of Amazon Machine Image (AMI) associated with the EKS Node Group. Defaults to `AL2_x86_64`. See the AWS documentation (https://docs.aws.amazon.com/eks/latest/APIReference/API_Nodegroup.html#AmazonEKS-Type-Nodegroup-amiType) for valid AMI Types. This provider will only perform drift detection if a configuration value is provided.
+        :param str bootstrap_extra_args: Additional args to pass directly to `/etc/eks/bootstrap.sh`. For details on available options, see: https://github.com/awslabs/amazon-eks-ami/blob/master/files/bootstrap.sh. Note that the `--apiserver-endpoint`, `--b64-cluster-ca` and `--kubelet-extra-args` flags are included automatically based on other configuration parameters.
+               
+               Note that this field conflicts with `launchTemplate`.
         :param pulumi.Input[str] capacity_type: Type of capacity associated with the EKS Node Group. Valid values: `ON_DEMAND`, `SPOT`. This provider will only perform drift detection if a configuration value is provided.
         :param pulumi.Input[Union['Cluster', pulumi.InputType['CoreDataArgs']]] cluster: The target EKS cluster.
         :param pulumi.Input[str] cluster_name: Name of the EKS Cluster.
         :param pulumi.Input[int] disk_size: Disk size in GiB for worker nodes. Defaults to `20`. This provider will only perform drift detection if a configuration value is provided.
+        :param bool enable_imd_sv2: Enables the ability to use EC2 Instance Metadata Service v2, which provides a more secure way to access instance metadata. For more information, see: https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/configuring-instance-metadata-service.html.
+               Defaults to `false`.
+               
+               Note that this field conflicts with `launchTemplate`. If you are providing a custom `launchTemplate`, you should enable this feature within the `launchTemplateMetadataOptions` of the supplied `launchTemplate`.
         :param pulumi.Input[bool] force_update_version: Force version update if existing pods are unable to be drained due to a pod disruption budget issue.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] instance_types: Set of instance types associated with the EKS Node Group. Defaults to `["t3.medium"]`. This provider will only perform drift detection if a configuration value is provided. Currently, the EKS API only accepts a single value in the set.
+        :param str kubelet_extra_args: Extra args to pass to the Kubelet. Corresponds to the options passed in the `--kubeletExtraArgs` flag to `/etc/eks/bootstrap.sh`. For example, '--port=10251 --address=0.0.0.0'. To escape characters in the extra argsvalue, wrap the value in quotes. For example, `kubeletExtraArgs = '--allowed-unsafe-sysctls "net.core.somaxconn"'`.
+               Note that this field conflicts with `launchTemplate`.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: Key-value map of Kubernetes labels. Only labels that are applied with the EKS API are managed by this argument. Other Kubernetes labels applied to the EKS Node Group will not be managed.
         :param pulumi.Input[pulumi.InputType['pulumi_aws.eks.NodeGroupLaunchTemplateArgs']] launch_template: Launch Template settings.
+               
+               Note: This field is mutually exclusive with `kubeletExtraArgs` and `bootstrapExtraArgs`.
         :param pulumi.Input[str] node_group_name: Name of the EKS Node Group. If omitted, this provider will assign a random, unique name. Conflicts with `nodeGroupNamePrefix`.
         :param pulumi.Input[str] node_group_name_prefix: Creates a unique name beginning with the specified prefix. Conflicts with `nodeGroupName`.
         :param pulumi.Input['pulumi_aws.iam.Role'] node_role: The IAM Role that provides permissions for the EKS Node Group.
                
                Note, `nodeRole` and `nodeRoleArn` are mutually exclusive, and a single option must be used.
         :param pulumi.Input[str] node_role_arn: Amazon Resource Name (ARN) of the IAM Role that provides permissions for the EKS Node Group.
                
@@ -465,20 +543,23 @@
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  ami_type: Optional[pulumi.Input[str]] = None,
+                 bootstrap_extra_args: Optional[str] = None,
                  capacity_type: Optional[pulumi.Input[str]] = None,
                  cluster: Optional[pulumi.Input[Union['Cluster', pulumi.InputType['CoreDataArgs']]]] = None,
                  cluster_name: Optional[pulumi.Input[str]] = None,
                  disk_size: Optional[pulumi.Input[int]] = None,
+                 enable_imd_sv2: Optional[bool] = None,
                  force_update_version: Optional[pulumi.Input[bool]] = None,
                  instance_types: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 kubelet_extra_args: Optional[str] = None,
                  labels: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  launch_template: Optional[pulumi.Input[pulumi.InputType['pulumi_aws.eks.NodeGroupLaunchTemplateArgs']]] = None,
                  node_group_name: Optional[pulumi.Input[str]] = None,
                  node_group_name_prefix: Optional[pulumi.Input[str]] = None,
                  node_role: Optional[pulumi.Input['pulumi_aws.iam.Role']] = None,
                  node_role_arn: Optional[pulumi.Input[str]] = None,
                  release_version: Optional[pulumi.Input[str]] = None,
@@ -496,22 +577,25 @@
             raise ValueError('ComponentResource classes do not support opts.id')
         else:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ManagedNodeGroupArgs.__new__(ManagedNodeGroupArgs)
 
             __props__.__dict__["ami_type"] = ami_type
+            __props__.__dict__["bootstrap_extra_args"] = bootstrap_extra_args
             __props__.__dict__["capacity_type"] = capacity_type
             if cluster is None and not opts.urn:
                 raise TypeError("Missing required property 'cluster'")
             __props__.__dict__["cluster"] = cluster
             __props__.__dict__["cluster_name"] = cluster_name
             __props__.__dict__["disk_size"] = disk_size
+            __props__.__dict__["enable_imd_sv2"] = enable_imd_sv2
             __props__.__dict__["force_update_version"] = force_update_version
             __props__.__dict__["instance_types"] = instance_types
+            __props__.__dict__["kubelet_extra_args"] = kubelet_extra_args
             __props__.__dict__["labels"] = labels
             __props__.__dict__["launch_template"] = launch_template
             __props__.__dict__["node_group_name"] = node_group_name
             __props__.__dict__["node_group_name_prefix"] = node_group_name_prefix
             __props__.__dict__["node_role"] = node_role
             __props__.__dict__["node_role_arn"] = node_role_arn
             __props__.__dict__["release_version"] = release_version
```

### Comparing `pulumi_eks-2.4.0a1715798612/pulumi_eks/node_group.py` & `pulumi_eks-2.5.0a1716314787/pulumi_eks/node_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_eks-2.4.0a1715798612/pulumi_eks/node_group_security_group.py` & `pulumi_eks-2.5.0a1716314787/pulumi_eks/node_group_security_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_eks-2.4.0a1715798612/pulumi_eks/node_group_v2.py` & `pulumi_eks-2.5.0a1716314787/pulumi_eks/node_group_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_eks-2.4.0a1715798612/pulumi_eks/outputs.py` & `pulumi_eks-2.5.0a1716314787/pulumi_eks/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_eks-2.4.0a1715798612/pulumi_eks/provider.py` & `pulumi_eks-2.5.0a1716314787/pulumi_eks/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_eks-2.4.0a1715798612/pulumi_eks/vpc_cni.py` & `pulumi_eks-2.5.0a1716314787/pulumi_eks/vpc_cni.py`

 * *Files identical despite different names*

### Comparing `pulumi_eks-2.4.0a1715798612/pulumi_eks.egg-info/PKG-INFO` & `pulumi_eks-2.5.0a1716314787/pulumi_eks.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_eks
-Version: 2.4.0a1715798612
+Version: 2.5.0a1716314787
 Summary: Pulumi Amazon Web Services (AWS) EKS Components.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.com
 Project-URL: Repository, https://github.com/pulumi/pulumi-eks
 Keywords: pulumi,aws,eks
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pulumi_eks Version: 2.4.0a1715798612 Summary:
+Metadata-Version: 2.1 Name: pulumi_eks Version: 2.5.0a1716314787 Summary:
 Pulumi Amazon Web Services (AWS) EKS Components. License: Apache-2.0 Project-
 URL: Homepage, https://pulumi.com Project-URL: Repository, https://github.com/
 pulumi/pulumi-eks Keywords: pulumi,aws,eks Requires-Python: >=3.8 Description-
 Content-Type: text/markdown Requires-Dist: parver>=0.2.1 Requires-Dist:
 pulumi<4.0.0,>=3.0.0 Requires-Dist: pulumi-aws<7.0.0,>=6.0.0 Requires-Dist:
 pulumi-kubernetes<5.0.0,>=4.0.0 Requires-Dist: semver>=2.8.1 [![Build Status]
 (https://github.com/pulumi/pulumi-eks/actions/workflows/master.yml/badge.svg)]
```

### Comparing `pulumi_eks-2.4.0a1715798612/pulumi_eks.egg-info/SOURCES.txt` & `pulumi_eks-2.5.0a1716314787/pulumi_eks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_eks-2.4.0a1715798612/pyproject.toml` & `pulumi_eks-2.5.0a1716314787/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_eks"
   description = "Pulumi Amazon Web Services (AWS) EKS Components."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "pulumi-aws>=6.0.0,<7.0.0", "pulumi-kubernetes>=4.0.0,<5.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "aws", "eks"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "2.4.0a1715798612"
+  version = "2.5.0a1716314787"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.com"
     Repository = "https://github.com/pulumi/pulumi-eks"
 
 [build-system]
```

