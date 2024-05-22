# Comparing `tmp/pulumi_kubernetes_the_hard_way-0.0.26a1716235251.tar.gz` & `tmp/pulumi_kubernetes_the_hard_way-0.0.26a1716346744.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_kubernetes_the_hard_way-0.0.26a1716235251.tar", last modified: Mon May 20 20:03:29 2024, max compression
+gzip compressed data, was "pulumi_kubernetes_the_hard_way-0.0.26a1716346744.tar", last modified: Wed May 22 03:01:32 2024, max compression
```

## Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716235251.tar` & `pulumi_kubernetes_the_hard_way-0.0.26a1716346744.tar`

### file list

```diff
@@ -1,89 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 20:03:29.751444 pulumi_kubernetes_the_hard_way-0.0.26a1716235251/
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-20 20:03:29.751444 pulumi_kubernetes_the_hard_way-0.0.26a1716235251/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-20 20:03:20.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716235251/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 20:03:29.735444 pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/
--rw-------   0 runner    (1001) docker     (127)     4925 2024-05-20 20:03:20.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/__init__.py
--rw-------   0 runner    (1001) docker     (127)     9268 2024-05-20 20:03:20.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 20:03:29.739444 pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/config/
--rw-------   0 runner    (1001) docker     (127)      580 2024-05-20 20:03:20.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/config/__init__.py
--rw-------   0 runner    (1001) docker     (127)      427 2024-05-20 20:03:20.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/config/_enums.py
--rw-------   0 runner    (1001) docker     (127)    21648 2024-05-20 20:03:20.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/config/_inputs.py
--rw-------   0 runner    (1001) docker     (127)     2860 2024-05-20 20:03:20.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/config/get_kube_proxy_configuration.py
--rw-------   0 runner    (1001) docker     (127)     8791 2024-05-20 20:03:20.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/config/get_kube_vip_manifest.py
--rw-------   0 runner    (1001) docker     (127)     3426 2024-05-20 20:03:20.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/config/get_kubeconfig.py
--rw-------   0 runner    (1001) docker     (127)     4826 2024-05-20 20:03:20.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/config/get_kubelet_configuration.py
--rw-------   0 runner    (1001) docker     (127)     5799 2024-05-20 20:03:20.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/config/kube_proxy_configuration.py
--rw-------   0 runner    (1001) docker     (127)    23901 2024-05-20 20:03:20.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/config/kube_vip_manifest.py
--rw-------   0 runner    (1001) docker     (127)    12558 2024-05-20 20:03:20.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/config/kubelet_configuration.py
--rw-------   0 runner    (1001) docker     (127)    41444 2024-05-20 20:03:20.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/config/outputs.py
--rw-------   0 runner    (1001) docker     (127)     2783 2024-05-20 20:03:20.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/provider.py
--rw-------   0 runner    (1001) docker     (127)      116 2024-05-20 20:03:20.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/pulumi-plugin.json
--rw-------   0 runner    (1001) docker     (127)        0 2024-05-20 20:03:20.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 20:03:29.743444 pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/remote/
--rw-------   0 runner    (1001) docker     (127)     1274 2024-05-20 20:03:20.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/remote/__init__.py
--rw-------   0 runner    (1001) docker     (127)     1095 2024-05-20 20:03:20.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/remote/_enums.py
--rw-------   0 runner    (1001) docker     (127)    30736 2024-05-20 20:03:20.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/remote/_inputs.py
--rw-------   0 runner    (1001) docker     (127)    13340 2024-05-20 20:03:20.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/remote/cni_bridge_plugin_configuration.py
--rw-------   0 runner    (1001) docker     (127)     8612 2024-05-20 20:03:20.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/remote/cni_loopback_plugin_configuration.py
--rw-------   0 runner    (1001) docker     (127)     7575 2024-05-20 20:03:20.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/remote/cni_plugin_configuration.py
--rw-------   0 runner    (1001) docker     (127)    19229 2024-05-20 20:03:20.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/remote/cni_plugins_install.py
--rw-------   0 runner    (1001) docker     (127)     6879 2024-05-20 20:03:20.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/remote/containerd_configuration.py
--rw-------   0 runner    (1001) docker     (127)    10255 2024-05-20 20:03:20.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/remote/containerd_install.py
--rw-------   0 runner    (1001) docker     (127)    10159 2024-05-20 20:03:20.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/remote/crictl_install.py
--rw-------   0 runner    (1001) docker     (127)     8328 2024-05-20 20:03:20.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/remote/download.py
--rw-------   0 runner    (1001) docker     (127)    12377 2024-05-20 20:03:20.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/remote/etcd_cluster.py
--rw-------   0 runner    (1001) docker     (127)    14905 2024-05-20 20:03:20.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/remote/etcd_configuration.py
--rw-------   0 runner    (1001) docker     (127)    10651 2024-05-20 20:03:20.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/remote/etcd_install.py
--rw-------   0 runner    (1001) docker     (127)    14696 2024-05-20 20:03:20.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/remote/etcd_service.py
--rw-------   0 runner    (1001) docker     (127)     7339 2024-05-20 20:03:20.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/remote/file.py
--rw-------   0 runner    (1001) docker     (127)     9708 2024-05-20 20:03:20.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/remote/kube_api_server_install.py
--rw-------   0 runner    (1001) docker     (127)     9822 2024-05-20 20:03:20.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/remote/kube_controller_manager_install.py
--rw-------   0 runner    (1001) docker     (127)     9652 2024-05-20 20:03:20.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/remote/kube_proxy_install.py
--rw-------   0 runner    (1001) docker     (127)    13465 2024-05-20 20:03:20.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/remote/kube_proxy_service.py
--rw-------   0 runner    (1001) docker     (127)     9708 2024-05-20 20:03:20.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/remote/kube_scheduler_install.py
--rw-------   0 runner    (1001) docker     (127)     9622 2024-05-20 20:03:20.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/remote/kubectl_install.py
--rw-------   0 runner    (1001) docker     (127)     9622 2024-05-20 20:03:20.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/remote/kubelet_install.py
--rw-------   0 runner    (1001) docker     (127)    15819 2024-05-20 20:03:20.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/remote/kubelet_service.py
--rw-------   0 runner    (1001) docker     (127)    30935 2024-05-20 20:03:20.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/remote/outputs.py
--rw-------   0 runner    (1001) docker     (127)    13390 2024-05-20 20:03:20.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/remote/provision_etcd.py
--rw-------   0 runner    (1001) docker     (127)     9580 2024-05-20 20:03:20.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/remote/runc_install.py
--rw-------   0 runner    (1001) docker     (127)     5199 2024-05-20 20:03:20.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/remote/start_containerd.py
--rw-------   0 runner    (1001) docker     (127)     5115 2024-05-20 20:03:20.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/remote/start_etcd.py
--rw-------   0 runner    (1001) docker     (127)     5187 2024-05-20 20:03:20.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/remote/start_kube_proxy.py
--rw-------   0 runner    (1001) docker     (127)     5157 2024-05-20 20:03:20.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/remote/start_kubelet.py
--rw-------   0 runner    (1001) docker     (127)     7429 2024-05-20 20:03:20.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/remote/static_pod.py
--rw-------   0 runner    (1001) docker     (127)    10944 2024-05-20 20:03:20.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/remote/systemd_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 20:03:29.747444 pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/tls/
--rw-------   0 runner    (1001) docker     (127)      425 2024-05-20 20:03:20.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/tls/__init__.py
--rw-------   0 runner    (1001) docker     (127)     1000 2024-05-20 20:03:20.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/tls/_enums.py
--rw-------   0 runner    (1001) docker     (127)     3019 2024-05-20 20:03:20.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/tls/_inputs.py
--rw-------   0 runner    (1001) docker     (127)    30597 2024-05-20 20:03:20.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/tls/certificate.py
--rw-------   0 runner    (1001) docker     (127)    15919 2024-05-20 20:03:20.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py
--rw-------   0 runner    (1001) docker     (127)     4450 2024-05-20 20:03:20.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/tls/encryption_key.py
--rw-------   0 runner    (1001) docker     (127)     2983 2024-05-20 20:03:20.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/tls/outputs.py
--rw-------   0 runner    (1001) docker     (127)    27130 2024-05-20 20:03:20.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/tls/root_ca.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 20:03:29.751444 pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/tools/
--rw-------   0 runner    (1001) docker     (127)      570 2024-05-20 20:03:20.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/tools/__init__.py
--rw-------   0 runner    (1001) docker     (127)     2920 2024-05-20 20:03:20.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/tools/_enums.py
--rw-------   0 runner    (1001) docker     (127)    61362 2024-05-20 20:03:20.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/tools/_inputs.py
--rw-------   0 runner    (1001) docker     (127)    14957 2024-05-20 20:03:20.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/tools/chmod.py
--rw-------   0 runner    (1001) docker     (127)    15049 2024-05-20 20:03:20.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/tools/etcdctl.py
--rw-------   0 runner    (1001) docker     (127)    15189 2024-05-20 20:03:20.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/tools/hostnamectl.py
--rw-------   0 runner    (1001) docker     (127)    14957 2024-05-20 20:03:20.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/tools/mkdir.py
--rw-------   0 runner    (1001) docker     (127)    14992 2024-05-20 20:03:20.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/tools/mktemp.py
--rw-------   0 runner    (1001) docker     (127)    14852 2024-05-20 20:03:20.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/tools/mv.py
--rw-------   0 runner    (1001) docker     (127)    52391 2024-05-20 20:03:20.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/tools/outputs.py
--rw-------   0 runner    (1001) docker     (127)    14852 2024-05-20 20:03:20.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/tools/rm.py
--rw-------   0 runner    (1001) docker     (127)    14887 2024-05-20 20:03:20.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/tools/sed.py
--rw-------   0 runner    (1001) docker     (127)    15119 2024-05-20 20:03:20.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/tools/systemctl.py
--rw-------   0 runner    (1001) docker     (127)    14887 2024-05-20 20:03:20.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/tools/tar.py
--rw-------   0 runner    (1001) docker     (127)    14907 2024-05-20 20:03:20.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/tools/tee.py
--rw-------   0 runner    (1001) docker     (127)    14922 2024-05-20 20:03:20.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/tools/wget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 20:03:29.751444 pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-20 20:03:29.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4187 2024-05-20 20:03:29.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 20:03:29.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-20 20:03:29.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-20 20:03:29.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way.egg-info/top_level.txt
--rw-------   0 runner    (1001) docker     (127)      899 2024-05-20 20:03:20.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 20:03:29.751444 pulumi_kubernetes_the_hard_way-0.0.26a1716235251/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:01:32.200204 pulumi_kubernetes_the_hard_way-0.0.26a1716346744/
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-22 03:01:32.200204 pulumi_kubernetes_the_hard_way-0.0.26a1716346744/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-22 03:01:23.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716346744/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:01:32.188204 pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/
+-rw-------   0 runner    (1001) docker     (127)     4839 2024-05-22 03:01:23.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     9268 2024-05-22 03:01:23.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:01:32.188204 pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/config/
+-rw-------   0 runner    (1001) docker     (127)      864 2024-05-22 03:01:23.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/config/__init__.py
+-rw-------   0 runner    (1001) docker     (127)      427 2024-05-22 03:01:23.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/config/_enums.py
+-rw-------   0 runner    (1001) docker     (127)    38814 2024-05-22 03:01:23.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/config/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)    10400 2024-05-22 03:01:23.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/config/cni_bridge_plugin_configuration.py
+-rw-------   0 runner    (1001) docker     (127)     6556 2024-05-22 03:01:23.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/config/cni_loopback_plugin_configuration.py
+-rw-------   0 runner    (1001) docker     (127)     4371 2024-05-22 03:01:23.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/config/containerd_configuration.py
+-rw-------   0 runner    (1001) docker     (127)     4880 2024-05-22 03:01:23.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/config/get_cni_bridge_plugin_configuration.py
+-rw-------   0 runner    (1001) docker     (127)     3418 2024-05-22 03:01:23.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/config/get_cni_loopback_plugin_configuration.py
+-rw-------   0 runner    (1001) docker     (127)     2560 2024-05-22 03:01:23.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/config/get_containerd_configuration.py
+-rw-------   0 runner    (1001) docker     (127)     2860 2024-05-22 03:01:23.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/config/get_kube_proxy_configuration.py
+-rw-------   0 runner    (1001) docker     (127)     8791 2024-05-22 03:01:23.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/config/get_kube_vip_manifest.py
+-rw-------   0 runner    (1001) docker     (127)     3426 2024-05-22 03:01:23.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/config/get_kubeconfig.py
+-rw-------   0 runner    (1001) docker     (127)     4826 2024-05-22 03:01:23.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/config/get_kubelet_configuration.py
+-rw-------   0 runner    (1001) docker     (127)     5799 2024-05-22 03:01:23.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/config/kube_proxy_configuration.py
+-rw-------   0 runner    (1001) docker     (127)    23901 2024-05-22 03:01:23.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/config/kube_vip_manifest.py
+-rw-------   0 runner    (1001) docker     (127)    12558 2024-05-22 03:01:23.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/config/kubelet_configuration.py
+-rw-------   0 runner    (1001) docker     (127)    56778 2024-05-22 03:01:23.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/config/outputs.py
+-rw-------   0 runner    (1001) docker     (127)     2783 2024-05-22 03:01:23.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/provider.py
+-rw-------   0 runner    (1001) docker     (127)      116 2024-05-22 03:01:23.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/pulumi-plugin.json
+-rw-------   0 runner    (1001) docker     (127)        0 2024-05-22 03:01:23.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:01:32.196204 pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/remote/
+-rw-------   0 runner    (1001) docker     (127)     1098 2024-05-22 03:01:23.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/remote/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     1095 2024-05-22 03:01:23.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/remote/_enums.py
+-rw-------   0 runner    (1001) docker     (127)    21733 2024-05-22 03:01:23.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/remote/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)    19229 2024-05-22 03:01:23.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/remote/cni_plugins_install.py
+-rw-------   0 runner    (1001) docker     (127)    10255 2024-05-22 03:01:23.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/remote/containerd_install.py
+-rw-------   0 runner    (1001) docker     (127)    10159 2024-05-22 03:01:23.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/remote/crictl_install.py
+-rw-------   0 runner    (1001) docker     (127)     8328 2024-05-22 03:01:23.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/remote/download.py
+-rw-------   0 runner    (1001) docker     (127)    12377 2024-05-22 03:01:23.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/remote/etcd_cluster.py
+-rw-------   0 runner    (1001) docker     (127)    14905 2024-05-22 03:01:23.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/remote/etcd_configuration.py
+-rw-------   0 runner    (1001) docker     (127)    10651 2024-05-22 03:01:23.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/remote/etcd_install.py
+-rw-------   0 runner    (1001) docker     (127)    14696 2024-05-22 03:01:23.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/remote/etcd_service.py
+-rw-------   0 runner    (1001) docker     (127)     7339 2024-05-22 03:01:23.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/remote/file.py
+-rw-------   0 runner    (1001) docker     (127)     9708 2024-05-22 03:01:23.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/remote/kube_api_server_install.py
+-rw-------   0 runner    (1001) docker     (127)     9822 2024-05-22 03:01:23.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/remote/kube_controller_manager_install.py
+-rw-------   0 runner    (1001) docker     (127)     9652 2024-05-22 03:01:23.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/remote/kube_proxy_install.py
+-rw-------   0 runner    (1001) docker     (127)    13465 2024-05-22 03:01:23.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/remote/kube_proxy_service.py
+-rw-------   0 runner    (1001) docker     (127)     9708 2024-05-22 03:01:23.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/remote/kube_scheduler_install.py
+-rw-------   0 runner    (1001) docker     (127)     9622 2024-05-22 03:01:23.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/remote/kubectl_install.py
+-rw-------   0 runner    (1001) docker     (127)     9622 2024-05-22 03:01:23.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/remote/kubelet_install.py
+-rw-------   0 runner    (1001) docker     (127)    15819 2024-05-22 03:01:23.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/remote/kubelet_service.py
+-rw-------   0 runner    (1001) docker     (127)    21302 2024-05-22 03:01:23.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/remote/outputs.py
+-rw-------   0 runner    (1001) docker     (127)    13390 2024-05-22 03:01:23.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/remote/provision_etcd.py
+-rw-------   0 runner    (1001) docker     (127)     9580 2024-05-22 03:01:23.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/remote/runc_install.py
+-rw-------   0 runner    (1001) docker     (127)     5199 2024-05-22 03:01:23.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/remote/start_containerd.py
+-rw-------   0 runner    (1001) docker     (127)     5115 2024-05-22 03:01:23.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/remote/start_etcd.py
+-rw-------   0 runner    (1001) docker     (127)     5187 2024-05-22 03:01:23.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/remote/start_kube_proxy.py
+-rw-------   0 runner    (1001) docker     (127)     5157 2024-05-22 03:01:23.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/remote/start_kubelet.py
+-rw-------   0 runner    (1001) docker     (127)     7429 2024-05-22 03:01:23.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/remote/static_pod.py
+-rw-------   0 runner    (1001) docker     (127)    10944 2024-05-22 03:01:23.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/remote/systemd_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:01:32.196204 pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/tls/
+-rw-------   0 runner    (1001) docker     (127)      425 2024-05-22 03:01:23.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/tls/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     1000 2024-05-22 03:01:23.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/tls/_enums.py
+-rw-------   0 runner    (1001) docker     (127)     3019 2024-05-22 03:01:23.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/tls/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)    30597 2024-05-22 03:01:23.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/tls/certificate.py
+-rw-------   0 runner    (1001) docker     (127)    15919 2024-05-22 03:01:23.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py
+-rw-------   0 runner    (1001) docker     (127)     4450 2024-05-22 03:01:23.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/tls/encryption_key.py
+-rw-------   0 runner    (1001) docker     (127)     2983 2024-05-22 03:01:23.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/tls/outputs.py
+-rw-------   0 runner    (1001) docker     (127)    27130 2024-05-22 03:01:23.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/tls/root_ca.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:01:32.200204 pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/tools/
+-rw-------   0 runner    (1001) docker     (127)      570 2024-05-22 03:01:23.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/tools/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     2920 2024-05-22 03:01:23.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/tools/_enums.py
+-rw-------   0 runner    (1001) docker     (127)    61362 2024-05-22 03:01:23.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/tools/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)    14957 2024-05-22 03:01:23.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/tools/chmod.py
+-rw-------   0 runner    (1001) docker     (127)    15049 2024-05-22 03:01:23.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/tools/etcdctl.py
+-rw-------   0 runner    (1001) docker     (127)    15189 2024-05-22 03:01:23.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/tools/hostnamectl.py
+-rw-------   0 runner    (1001) docker     (127)    14957 2024-05-22 03:01:23.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/tools/mkdir.py
+-rw-------   0 runner    (1001) docker     (127)    14992 2024-05-22 03:01:23.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/tools/mktemp.py
+-rw-------   0 runner    (1001) docker     (127)    14852 2024-05-22 03:01:23.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/tools/mv.py
+-rw-------   0 runner    (1001) docker     (127)    52391 2024-05-22 03:01:23.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/tools/outputs.py
+-rw-------   0 runner    (1001) docker     (127)    14852 2024-05-22 03:01:23.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/tools/rm.py
+-rw-------   0 runner    (1001) docker     (127)    14887 2024-05-22 03:01:23.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/tools/sed.py
+-rw-------   0 runner    (1001) docker     (127)    15119 2024-05-22 03:01:23.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/tools/systemctl.py
+-rw-------   0 runner    (1001) docker     (127)    14887 2024-05-22 03:01:23.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/tools/tar.py
+-rw-------   0 runner    (1001) docker     (127)    14907 2024-05-22 03:01:23.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/tools/tee.py
+-rw-------   0 runner    (1001) docker     (127)    14922 2024-05-22 03:01:23.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/tools/wget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:01:32.200204 pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-22 03:01:32.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4347 2024-05-22 03:01:32.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 03:01:32.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-22 03:01:32.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-22 03:01:32.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way.egg-info/top_level.txt
+-rw-------   0 runner    (1001) docker     (127)      899 2024-05-22 03:01:23.000000 pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 03:01:32.200204 pulumi_kubernetes_the_hard_way-0.0.26a1716346744/setup.cfg
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716235251/PKG-INFO` & `pulumi_kubernetes_the_hard_way-0.0.26a1716346744/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_kubernetes_the_hard_way
-Version: 0.0.26a1716235251
+Version: 0.0.26a1716346744
 Summary: A Pulumi implementation of Kelsey Hightower's Kubernetes the Hard Way
 License: Apache-2.0
 Project-URL: Repository, https://github.com/UnstoppableMango/pulumi-kubernetes-the-hard-way
 Keywords: pulumi,command,tls,kubernetes,category/utility,kind/component
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: parver>=0.2.1
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716235251/README.md` & `pulumi_kubernetes_the_hard_way-0.0.26a1716346744/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/__init__.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,29 +27,28 @@
     resource_modules="""
 [
  {
   "pkg": "kubernetes-the-hard-way",
   "mod": "config",
   "fqn": "pulumi_kubernetes_the_hard_way.config",
   "classes": {
+   "kubernetes-the-hard-way:config:CniBridgePluginConfiguration": "CniBridgePluginConfiguration",
+   "kubernetes-the-hard-way:config:CniLoopbackPluginConfiguration": "CniLoopbackPluginConfiguration",
+   "kubernetes-the-hard-way:config:ContainerdConfiguration": "ContainerdConfiguration",
    "kubernetes-the-hard-way:config:KubeProxyConfiguration": "KubeProxyConfiguration",
    "kubernetes-the-hard-way:config:KubeVipManifest": "KubeVipManifest",
    "kubernetes-the-hard-way:config:KubeletConfiguration": "KubeletConfiguration"
   }
  },
  {
   "pkg": "kubernetes-the-hard-way",
   "mod": "remote",
   "fqn": "pulumi_kubernetes_the_hard_way.remote",
   "classes": {
-   "kubernetes-the-hard-way:remote:CniBridgePluginConfiguration": "CniBridgePluginConfiguration",
-   "kubernetes-the-hard-way:remote:CniLoopbackPluginConfiguration": "CniLoopbackPluginConfiguration",
-   "kubernetes-the-hard-way:remote:CniPluginConfiguration": "CniPluginConfiguration",
    "kubernetes-the-hard-way:remote:CniPluginsInstall": "CniPluginsInstall",
-   "kubernetes-the-hard-way:remote:ContainerdConfiguration": "ContainerdConfiguration",
    "kubernetes-the-hard-way:remote:ContainerdInstall": "ContainerdInstall",
    "kubernetes-the-hard-way:remote:CrictlInstall": "CrictlInstall",
    "kubernetes-the-hard-way:remote:Download": "Download",
    "kubernetes-the-hard-way:remote:EtcdCluster": "EtcdCluster",
    "kubernetes-the-hard-way:remote:EtcdConfiguration": "EtcdConfiguration",
    "kubernetes-the-hard-way:remote:EtcdInstall": "EtcdInstall",
    "kubernetes-the-hard-way:remote:EtcdService": "EtcdService",
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/_utilities.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/config/get_kube_proxy_configuration.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/config/get_kube_proxy_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/config/get_kube_vip_manifest.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/config/get_kube_vip_manifest.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/config/get_kubeconfig.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/config/get_kubeconfig.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/config/get_kubelet_configuration.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/config/get_kubelet_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/config/kube_proxy_configuration.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/config/kube_proxy_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/config/kube_vip_manifest.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/config/kube_vip_manifest.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/config/kubelet_configuration.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/config/kubelet_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/provider.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/remote/__init__.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/remote/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,19 +2,15 @@
 # *** WARNING: this file was generated by pulumi-language-python. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 from .. import _utilities
 import typing
 # Export this package's modules as members:
 from ._enums import *
-from .cni_bridge_plugin_configuration import *
-from .cni_loopback_plugin_configuration import *
-from .cni_plugin_configuration import *
 from .cni_plugins_install import *
-from .containerd_configuration import *
 from .containerd_install import *
 from .crictl_install import *
 from .download import *
 from .etcd_cluster import *
 from .etcd_configuration import *
 from .etcd_install import *
 from .etcd_service import *
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/remote/_enums.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/remote/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/remote/_inputs.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/remote/_inputs.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,283 +8,24 @@
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from ._enums import *
 import pulumi_command
 
 __all__ = [
-    'CniBridgeIpamArgs',
-    'ContainerdCriPluginConfigurationCniArgs',
-    'ContainerdCriPluginConfigurationContainerdRuncOptionsArgs',
-    'ContainerdCriPluginConfigurationContainerdRuncArgs',
-    'ContainerdCriPluginConfigurationContainerdArgs',
-    'ContainerdCriPluginConfigurationArgs',
     'EtcdConfigurationPropsArgs',
     'EtcdNodeArgs',
     'KubeProxyConfigurationPropsArgs',
     'KubeletConfigurationPropsArgs',
     'SystemdInstallSectionArgs',
     'SystemdServiceSectionArgs',
     'SystemdUnitSectionArgs',
 ]
 
 @pulumi.input_type
-class CniBridgeIpamArgs:
-    def __init__(__self__, *,
-                 ranges: Optional[pulumi.Input[Sequence[pulumi.Input[Mapping[str, pulumi.Input[str]]]]]] = None,
-                 routes: Optional[pulumi.Input[Sequence[pulumi.Input[Mapping[str, pulumi.Input[str]]]]]] = None,
-                 type: Optional[pulumi.Input[str]] = None):
-        """
-        The CNI plugins IPAM
-        :param pulumi.Input[Sequence[pulumi.Input[Mapping[str, pulumi.Input[str]]]]] ranges: IPAM ranges.
-        :param pulumi.Input[Sequence[pulumi.Input[Mapping[str, pulumi.Input[str]]]]] routes: IPAM routes.
-        :param pulumi.Input[str] type: CNI bridge IPAM type
-        """
-        if ranges is not None:
-            pulumi.set(__self__, "ranges", ranges)
-        if routes is not None:
-            pulumi.set(__self__, "routes", routes)
-        if type is not None:
-            pulumi.set(__self__, "type", type)
-
-    @property
-    @pulumi.getter
-    def ranges(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[Mapping[str, pulumi.Input[str]]]]]]:
-        """
-        IPAM ranges.
-        """
-        return pulumi.get(self, "ranges")
-
-    @ranges.setter
-    def ranges(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[Mapping[str, pulumi.Input[str]]]]]]):
-        pulumi.set(self, "ranges", value)
-
-    @property
-    @pulumi.getter
-    def routes(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[Mapping[str, pulumi.Input[str]]]]]]:
-        """
-        IPAM routes.
-        """
-        return pulumi.get(self, "routes")
-
-    @routes.setter
-    def routes(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[Mapping[str, pulumi.Input[str]]]]]]):
-        pulumi.set(self, "routes", value)
-
-    @property
-    @pulumi.getter
-    def type(self) -> Optional[pulumi.Input[str]]:
-        """
-        CNI bridge IPAM type
-        """
-        return pulumi.get(self, "type")
-
-    @type.setter
-    def type(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "type", value)
-
-
-@pulumi.input_type
-class ContainerdCriPluginConfigurationCniArgs:
-    def __init__(__self__, *,
-                 bin_dir: Optional[pulumi.Input[str]] = None,
-                 conf_dir: Optional[pulumi.Input[str]] = None):
-        """
-        containerd cri plugin configuration.
-        :param pulumi.Input[str] bin_dir: bin_dir
-        :param pulumi.Input[str] conf_dir: conf_dir
-        """
-        if bin_dir is not None:
-            pulumi.set(__self__, "bin_dir", bin_dir)
-        if conf_dir is not None:
-            pulumi.set(__self__, "conf_dir", conf_dir)
-
-    @property
-    @pulumi.getter(name="binDir")
-    def bin_dir(self) -> Optional[pulumi.Input[str]]:
-        """
-        bin_dir
-        """
-        return pulumi.get(self, "bin_dir")
-
-    @bin_dir.setter
-    def bin_dir(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "bin_dir", value)
-
-    @property
-    @pulumi.getter(name="confDir")
-    def conf_dir(self) -> Optional[pulumi.Input[str]]:
-        """
-        conf_dir
-        """
-        return pulumi.get(self, "conf_dir")
-
-    @conf_dir.setter
-    def conf_dir(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "conf_dir", value)
-
-
-@pulumi.input_type
-class ContainerdCriPluginConfigurationContainerdRuncOptionsArgs:
-    def __init__(__self__, *,
-                 systemd_cgroup: Optional[pulumi.Input[bool]] = None):
-        """
-        containerd cri runc plugin configuration.
-        :param pulumi.Input[bool] systemd_cgroup: SystemdCgroup
-        """
-        if systemd_cgroup is not None:
-            pulumi.set(__self__, "systemd_cgroup", systemd_cgroup)
-
-    @property
-    @pulumi.getter(name="systemdCgroup")
-    def systemd_cgroup(self) -> Optional[pulumi.Input[bool]]:
-        """
-        SystemdCgroup
-        """
-        return pulumi.get(self, "systemd_cgroup")
-
-    @systemd_cgroup.setter
-    def systemd_cgroup(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "systemd_cgroup", value)
-
-
-@pulumi.input_type
-class ContainerdCriPluginConfigurationContainerdRuncArgs:
-    def __init__(__self__, *,
-                 options: 'ContainerdCriPluginConfigurationContainerdRuncOptionsArgs',
-                 runtime_type: Optional[pulumi.Input[str]] = None):
-        """
-        containerd cri runc plugin configuration.
-        :param 'ContainerdCriPluginConfigurationContainerdRuncOptionsArgs' options: runc options.
-        :param pulumi.Input[str] runtime_type: runtime_type
-        """
-        pulumi.set(__self__, "options", options)
-        if runtime_type is not None:
-            pulumi.set(__self__, "runtime_type", runtime_type)
-
-    @property
-    @pulumi.getter
-    def options(self) -> 'ContainerdCriPluginConfigurationContainerdRuncOptionsArgs':
-        """
-        runc options.
-        """
-        return pulumi.get(self, "options")
-
-    @options.setter
-    def options(self, value: 'ContainerdCriPluginConfigurationContainerdRuncOptionsArgs'):
-        pulumi.set(self, "options", value)
-
-    @property
-    @pulumi.getter(name="runtimeType")
-    def runtime_type(self) -> Optional[pulumi.Input[str]]:
-        """
-        runtime_type
-        """
-        return pulumi.get(self, "runtime_type")
-
-    @runtime_type.setter
-    def runtime_type(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "runtime_type", value)
-
-
-@pulumi.input_type
-class ContainerdCriPluginConfigurationContainerdArgs:
-    def __init__(__self__, *,
-                 default_runtime_name: Optional[pulumi.Input[str]] = None,
-                 runtimes: Optional['ContainerdCriPluginConfigurationContainerdRuncArgs'] = None,
-                 snapshotter: Optional[pulumi.Input[str]] = None):
-        """
-        containerd cri plugin configuration.
-        :param pulumi.Input[str] default_runtime_name: default_runtime_name
-        :param 'ContainerdCriPluginConfigurationContainerdRuncArgs' runtimes: The containerd runtime configuration.
-        :param pulumi.Input[str] snapshotter: snapshotter
-        """
-        if default_runtime_name is not None:
-            pulumi.set(__self__, "default_runtime_name", default_runtime_name)
-        if runtimes is not None:
-            pulumi.set(__self__, "runtimes", runtimes)
-        if snapshotter is not None:
-            pulumi.set(__self__, "snapshotter", snapshotter)
-
-    @property
-    @pulumi.getter(name="defaultRuntimeName")
-    def default_runtime_name(self) -> Optional[pulumi.Input[str]]:
-        """
-        default_runtime_name
-        """
-        return pulumi.get(self, "default_runtime_name")
-
-    @default_runtime_name.setter
-    def default_runtime_name(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "default_runtime_name", value)
-
-    @property
-    @pulumi.getter
-    def runtimes(self) -> Optional['ContainerdCriPluginConfigurationContainerdRuncArgs']:
-        """
-        The containerd runtime configuration.
-        """
-        return pulumi.get(self, "runtimes")
-
-    @runtimes.setter
-    def runtimes(self, value: Optional['ContainerdCriPluginConfigurationContainerdRuncArgs']):
-        pulumi.set(self, "runtimes", value)
-
-    @property
-    @pulumi.getter
-    def snapshotter(self) -> Optional[pulumi.Input[str]]:
-        """
-        snapshotter
-        """
-        return pulumi.get(self, "snapshotter")
-
-    @snapshotter.setter
-    def snapshotter(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "snapshotter", value)
-
-
-@pulumi.input_type
-class ContainerdCriPluginConfigurationArgs:
-    def __init__(__self__, *,
-                 cni: 'ContainerdCriPluginConfigurationCniArgs',
-                 containerd: 'ContainerdCriPluginConfigurationContainerdArgs'):
-        """
-        containerd cri plugin configuration.
-        :param 'ContainerdCriPluginConfigurationCniArgs' cni: cni configuration.
-        :param 'ContainerdCriPluginConfigurationContainerdArgs' containerd: containerd configuration.
-        """
-        pulumi.set(__self__, "cni", cni)
-        pulumi.set(__self__, "containerd", containerd)
-
-    @property
-    @pulumi.getter
-    def cni(self) -> 'ContainerdCriPluginConfigurationCniArgs':
-        """
-        cni configuration.
-        """
-        return pulumi.get(self, "cni")
-
-    @cni.setter
-    def cni(self, value: 'ContainerdCriPluginConfigurationCniArgs'):
-        pulumi.set(self, "cni", value)
-
-    @property
-    @pulumi.getter
-    def containerd(self) -> 'ContainerdCriPluginConfigurationContainerdArgs':
-        """
-        containerd configuration.
-        """
-        return pulumi.get(self, "containerd")
-
-    @containerd.setter
-    def containerd(self, value: 'ContainerdCriPluginConfigurationContainerdArgs'):
-        pulumi.set(self, "containerd", value)
-
-
-@pulumi.input_type
 class EtcdConfigurationPropsArgs:
     def __init__(__self__, *,
                  ca_file_path: pulumi.Input[str],
                  cert_file_path: pulumi.Input[str],
                  data_directory: pulumi.Input[str],
                  etcd_path: pulumi.Input[str],
                  internal_ip: pulumi.Input[str],
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/remote/cni_bridge_plugin_configuration.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/remote/etcd_cluster.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,365 +5,314 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
+from .. import tls as _tls
+from ._enums import *
 from ._inputs import *
-from .file import File
+from .etcd_configuration import EtcdConfiguration
+from .etcd_install import EtcdInstall
+from .etcd_service import EtcdService
+from .start_etcd import StartEtcd
 import pulumi_command
 
-__all__ = ['CniBridgePluginConfigurationArgs', 'CniBridgePluginConfiguration']
+__all__ = ['EtcdClusterArgs', 'EtcdCluster']
 
 @pulumi.input_type
-class CniBridgePluginConfigurationArgs:
+class EtcdClusterArgs:
     def __init__(__self__, *,
-                 connection: pulumi.Input['pulumi_command.remote.ConnectionArgs'],
-                 bridge: Optional[pulumi.Input[str]] = None,
-                 cni_version: Optional[pulumi.Input[str]] = None,
-                 ip_masq: Optional[pulumi.Input[bool]] = None,
-                 ipam: Optional[pulumi.Input['CniBridgeIpamArgs']] = None,
-                 is_gateway: Optional[pulumi.Input[bool]] = None,
-                 name: Optional[pulumi.Input[str]] = None,
-                 path: Optional[pulumi.Input[str]] = None,
-                 subnet: Optional[pulumi.Input[str]] = None,
-                 type: Optional[pulumi.Input[str]] = None):
+                 bundle: pulumi.Input['_tls.BundleArgs'],
+                 nodes: Mapping[str, pulumi.Input['EtcdNodeArgs']],
+                 architecture: Optional[pulumi.Input['Architecture']] = None,
+                 binary_directory: Optional[pulumi.Input[str]] = None,
+                 configuration_directory: Optional[pulumi.Input[str]] = None,
+                 data_directory: Optional[pulumi.Input[str]] = None,
+                 version: Optional[pulumi.Input[str]] = None):
         """
-        The set of arguments for constructing a CniBridgePluginConfiguration resource.
-        :param pulumi.Input['pulumi_command.remote.ConnectionArgs'] connection: The parameters with which to connect to the remote host.
-        :param pulumi.Input[str] bridge: Bridge name.
-        :param pulumi.Input[str] cni_version: CNI version.
-        :param pulumi.Input[bool] ip_masq: IP masq.
-        :param pulumi.Input['CniBridgeIpamArgs'] ipam: IPAM
-        :param pulumi.Input[bool] is_gateway: Is gateway.
-        :param pulumi.Input[str] name: CNI plugin name.
-        :param pulumi.Input[str] path: Path to put the configuration file on the remote system
-        :param pulumi.Input[str] subnet: The subnet to use.
-        :param pulumi.Input[str] type: CNI plugin type.
+        The set of arguments for constructing a EtcdCluster resource.
+        :param pulumi.Input['_tls.BundleArgs'] bundle: The TLS bundle.
+        :param Mapping[str, pulumi.Input['EtcdNodeArgs']] nodes: Etcd node configuration. The key should be a name used to identify the node.
+        :param pulumi.Input['Architecture'] architecture: TODO
+        :param pulumi.Input[str] binary_directory: TODO
+        :param pulumi.Input[str] configuration_directory: The directory to use for etcd configuration.
+        :param pulumi.Input[str] data_directory: The directory to use for etcd data.
+        :param pulumi.Input[str] version: The version to install.
         """
-        pulumi.set(__self__, "connection", connection)
-        if bridge is not None:
-            pulumi.set(__self__, "bridge", bridge)
-        if cni_version is not None:
-            pulumi.set(__self__, "cni_version", cni_version)
-        if ip_masq is not None:
-            pulumi.set(__self__, "ip_masq", ip_masq)
-        if ipam is not None:
-            pulumi.set(__self__, "ipam", ipam)
-        if is_gateway is not None:
-            pulumi.set(__self__, "is_gateway", is_gateway)
-        if name is not None:
-            pulumi.set(__self__, "name", name)
-        if path is not None:
-            pulumi.set(__self__, "path", path)
-        if subnet is not None:
-            pulumi.set(__self__, "subnet", subnet)
-        if type is not None:
-            pulumi.set(__self__, "type", type)
+        pulumi.set(__self__, "bundle", bundle)
+        pulumi.set(__self__, "nodes", nodes)
+        if architecture is not None:
+            pulumi.set(__self__, "architecture", architecture)
+        if binary_directory is not None:
+            pulumi.set(__self__, "binary_directory", binary_directory)
+        if configuration_directory is not None:
+            pulumi.set(__self__, "configuration_directory", configuration_directory)
+        if data_directory is not None:
+            pulumi.set(__self__, "data_directory", data_directory)
+        if version is not None:
+            pulumi.set(__self__, "version", version)
 
     @property
     @pulumi.getter
-    def connection(self) -> pulumi.Input['pulumi_command.remote.ConnectionArgs']:
+    def bundle(self) -> pulumi.Input['_tls.BundleArgs']:
         """
-        The parameters with which to connect to the remote host.
+        The TLS bundle.
         """
-        return pulumi.get(self, "connection")
+        return pulumi.get(self, "bundle")
 
-    @connection.setter
-    def connection(self, value: pulumi.Input['pulumi_command.remote.ConnectionArgs']):
-        pulumi.set(self, "connection", value)
+    @bundle.setter
+    def bundle(self, value: pulumi.Input['_tls.BundleArgs']):
+        pulumi.set(self, "bundle", value)
 
     @property
     @pulumi.getter
-    def bridge(self) -> Optional[pulumi.Input[str]]:
+    def nodes(self) -> Mapping[str, pulumi.Input['EtcdNodeArgs']]:
         """
-        Bridge name.
+        Etcd node configuration. The key should be a name used to identify the node.
         """
-        return pulumi.get(self, "bridge")
+        return pulumi.get(self, "nodes")
 
-    @bridge.setter
-    def bridge(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "bridge", value)
-
-    @property
-    @pulumi.getter(name="cniVersion")
-    def cni_version(self) -> Optional[pulumi.Input[str]]:
-        """
-        CNI version.
-        """
-        return pulumi.get(self, "cni_version")
-
-    @cni_version.setter
-    def cni_version(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "cni_version", value)
-
-    @property
-    @pulumi.getter(name="ipMasq")
-    def ip_masq(self) -> Optional[pulumi.Input[bool]]:
-        """
-        IP masq.
-        """
-        return pulumi.get(self, "ip_masq")
-
-    @ip_masq.setter
-    def ip_masq(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "ip_masq", value)
+    @nodes.setter
+    def nodes(self, value: Mapping[str, pulumi.Input['EtcdNodeArgs']]):
+        pulumi.set(self, "nodes", value)
 
     @property
     @pulumi.getter
-    def ipam(self) -> Optional[pulumi.Input['CniBridgeIpamArgs']]:
+    def architecture(self) -> Optional[pulumi.Input['Architecture']]:
         """
-        IPAM
+        TODO
         """
-        return pulumi.get(self, "ipam")
+        return pulumi.get(self, "architecture")
 
-    @ipam.setter
-    def ipam(self, value: Optional[pulumi.Input['CniBridgeIpamArgs']]):
-        pulumi.set(self, "ipam", value)
+    @architecture.setter
+    def architecture(self, value: Optional[pulumi.Input['Architecture']]):
+        pulumi.set(self, "architecture", value)
 
     @property
-    @pulumi.getter(name="isGateway")
-    def is_gateway(self) -> Optional[pulumi.Input[bool]]:
+    @pulumi.getter(name="binaryDirectory")
+    def binary_directory(self) -> Optional[pulumi.Input[str]]:
         """
-        Is gateway.
+        TODO
         """
-        return pulumi.get(self, "is_gateway")
+        return pulumi.get(self, "binary_directory")
 
-    @is_gateway.setter
-    def is_gateway(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "is_gateway", value)
+    @binary_directory.setter
+    def binary_directory(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "binary_directory", value)
 
     @property
-    @pulumi.getter
-    def name(self) -> Optional[pulumi.Input[str]]:
-        """
-        CNI plugin name.
-        """
-        return pulumi.get(self, "name")
-
-    @name.setter
-    def name(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "name", value)
-
-    @property
-    @pulumi.getter
-    def path(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="configurationDirectory")
+    def configuration_directory(self) -> Optional[pulumi.Input[str]]:
         """
-        Path to put the configuration file on the remote system
+        The directory to use for etcd configuration.
         """
-        return pulumi.get(self, "path")
+        return pulumi.get(self, "configuration_directory")
 
-    @path.setter
-    def path(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "path", value)
+    @configuration_directory.setter
+    def configuration_directory(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "configuration_directory", value)
 
     @property
-    @pulumi.getter
-    def subnet(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="dataDirectory")
+    def data_directory(self) -> Optional[pulumi.Input[str]]:
         """
-        The subnet to use.
+        The directory to use for etcd data.
         """
-        return pulumi.get(self, "subnet")
+        return pulumi.get(self, "data_directory")
 
-    @subnet.setter
-    def subnet(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "subnet", value)
+    @data_directory.setter
+    def data_directory(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "data_directory", value)
 
     @property
     @pulumi.getter
-    def type(self) -> Optional[pulumi.Input[str]]:
+    def version(self) -> Optional[pulumi.Input[str]]:
         """
-        CNI plugin type.
+        The version to install.
         """
-        return pulumi.get(self, "type")
+        return pulumi.get(self, "version")
 
-    @type.setter
-    def type(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "type", value)
+    @version.setter
+    def version(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "version", value)
 
 
-class CniBridgePluginConfiguration(pulumi.ComponentResource):
+class EtcdCluster(pulumi.ComponentResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 bridge: Optional[pulumi.Input[str]] = None,
-                 cni_version: Optional[pulumi.Input[str]] = None,
-                 connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
-                 ip_masq: Optional[pulumi.Input[bool]] = None,
-                 ipam: Optional[pulumi.Input[pulumi.InputType['CniBridgeIpamArgs']]] = None,
-                 is_gateway: Optional[pulumi.Input[bool]] = None,
-                 name: Optional[pulumi.Input[str]] = None,
-                 path: Optional[pulumi.Input[str]] = None,
-                 subnet: Optional[pulumi.Input[str]] = None,
-                 type: Optional[pulumi.Input[str]] = None,
+                 architecture: Optional[pulumi.Input['Architecture']] = None,
+                 binary_directory: Optional[pulumi.Input[str]] = None,
+                 bundle: Optional[pulumi.Input[pulumi.InputType['_tls.BundleArgs']]] = None,
+                 configuration_directory: Optional[pulumi.Input[str]] = None,
+                 data_directory: Optional[pulumi.Input[str]] = None,
+                 nodes: Optional[Mapping[str, pulumi.Input[pulumi.InputType['EtcdNodeArgs']]]] = None,
+                 version: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        The CNI bridge plugin configuration.
+        Creates an etcd cluster from one or more remote systems.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] bridge: Bridge name.
-        :param pulumi.Input[str] cni_version: CNI version.
-        :param pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']] connection: The parameters with which to connect to the remote host.
-        :param pulumi.Input[bool] ip_masq: IP masq.
-        :param pulumi.Input[pulumi.InputType['CniBridgeIpamArgs']] ipam: IPAM
-        :param pulumi.Input[bool] is_gateway: Is gateway.
-        :param pulumi.Input[str] name: CNI plugin name.
-        :param pulumi.Input[str] path: Path to put the configuration file on the remote system
-        :param pulumi.Input[str] subnet: The subnet to use.
-        :param pulumi.Input[str] type: CNI plugin type.
+        :param pulumi.Input['Architecture'] architecture: TODO
+        :param pulumi.Input[str] binary_directory: TODO
+        :param pulumi.Input[pulumi.InputType['_tls.BundleArgs']] bundle: The TLS bundle.
+        :param pulumi.Input[str] configuration_directory: The directory to use for etcd configuration.
+        :param pulumi.Input[str] data_directory: The directory to use for etcd data.
+        :param Mapping[str, pulumi.Input[pulumi.InputType['EtcdNodeArgs']]] nodes: Etcd node configuration. The key should be a name used to identify the node.
+        :param pulumi.Input[str] version: The version to install.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: CniBridgePluginConfigurationArgs,
+                 args: EtcdClusterArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        The CNI bridge plugin configuration.
+        Creates an etcd cluster from one or more remote systems.
 
         :param str resource_name: The name of the resource.
-        :param CniBridgePluginConfigurationArgs args: The arguments to use to populate this resource's properties.
+        :param EtcdClusterArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(CniBridgePluginConfigurationArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(EtcdClusterArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 bridge: Optional[pulumi.Input[str]] = None,
-                 cni_version: Optional[pulumi.Input[str]] = None,
-                 connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
-                 ip_masq: Optional[pulumi.Input[bool]] = None,
-                 ipam: Optional[pulumi.Input[pulumi.InputType['CniBridgeIpamArgs']]] = None,
-                 is_gateway: Optional[pulumi.Input[bool]] = None,
-                 name: Optional[pulumi.Input[str]] = None,
-                 path: Optional[pulumi.Input[str]] = None,
-                 subnet: Optional[pulumi.Input[str]] = None,
-                 type: Optional[pulumi.Input[str]] = None,
+                 architecture: Optional[pulumi.Input['Architecture']] = None,
+                 binary_directory: Optional[pulumi.Input[str]] = None,
+                 bundle: Optional[pulumi.Input[pulumi.InputType['_tls.BundleArgs']]] = None,
+                 configuration_directory: Optional[pulumi.Input[str]] = None,
+                 data_directory: Optional[pulumi.Input[str]] = None,
+                 nodes: Optional[Mapping[str, pulumi.Input[pulumi.InputType['EtcdNodeArgs']]]] = None,
+                 version: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is not None:
             raise ValueError('ComponentResource classes do not support opts.id')
         else:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = CniBridgePluginConfigurationArgs.__new__(CniBridgePluginConfigurationArgs)
+            __props__ = EtcdClusterArgs.__new__(EtcdClusterArgs)
 
-            __props__.__dict__["bridge"] = bridge
-            __props__.__dict__["cni_version"] = cni_version
-            if connection is None and not opts.urn:
-                raise TypeError("Missing required property 'connection'")
-            __props__.__dict__["connection"] = connection
-            __props__.__dict__["ip_masq"] = ip_masq
-            __props__.__dict__["ipam"] = ipam
-            __props__.__dict__["is_gateway"] = is_gateway
-            __props__.__dict__["name"] = name
-            __props__.__dict__["path"] = path
-            __props__.__dict__["subnet"] = subnet
-            __props__.__dict__["type"] = type
-            __props__.__dict__["file"] = None
-        super(CniBridgePluginConfiguration, __self__).__init__(
-            'kubernetes-the-hard-way:remote:CniBridgePluginConfiguration',
+            __props__.__dict__["architecture"] = architecture
+            __props__.__dict__["binary_directory"] = binary_directory
+            if bundle is None and not opts.urn:
+                raise TypeError("Missing required property 'bundle'")
+            __props__.__dict__["bundle"] = bundle
+            __props__.__dict__["configuration_directory"] = configuration_directory
+            __props__.__dict__["data_directory"] = data_directory
+            if nodes is None and not opts.urn:
+                raise TypeError("Missing required property 'nodes'")
+            __props__.__dict__["nodes"] = nodes
+            __props__.__dict__["version"] = version
+            __props__.__dict__["configuration"] = None
+            __props__.__dict__["install"] = None
+            __props__.__dict__["service"] = None
+            __props__.__dict__["start"] = None
+        super(EtcdCluster, __self__).__init__(
+            'kubernetes-the-hard-way:remote:EtcdCluster',
             resource_name,
             __props__,
             opts,
             remote=True)
 
     @property
     @pulumi.getter
-    def bridge(self) -> pulumi.Output[str]:
+    def architecture(self) -> pulumi.Output[Optional['Architecture']]:
         """
-        Bridge name.
+        TODO
         """
-        return pulumi.get(self, "bridge")
+        return pulumi.get(self, "architecture")
 
     @property
-    @pulumi.getter(name="cniVersion")
-    def cni_version(self) -> pulumi.Output[str]:
+    @pulumi.getter(name="binaryDirectory")
+    def binary_directory(self) -> pulumi.Output[Optional[str]]:
         """
-        CNI version.
+        TODO
         """
-        return pulumi.get(self, "cni_version")
+        return pulumi.get(self, "binary_directory")
 
     @property
     @pulumi.getter
-    def connection(self) -> pulumi.Output['pulumi_command.remote.outputs.Connection']:
+    def bundle(self) -> pulumi.Output['_tls.outputs.Bundle']:
         """
-        The parameters with which to connect to the remote host.
+        The TLS bundle.
         """
-        return pulumi.get(self, "connection")
+        return pulumi.get(self, "bundle")
 
     @property
     @pulumi.getter
-    def file(self) -> pulumi.Output[Optional['File']]:
+    def configuration(self) -> pulumi.Output[Mapping[str, 'EtcdConfiguration']]:
         """
-        The file on the remote system.
+        Map of node name to etcd configuration.
         """
-        return pulumi.get(self, "file")
+        return pulumi.get(self, "configuration")
 
     @property
-    @pulumi.getter(name="ipMasq")
-    def ip_masq(self) -> pulumi.Output[bool]:
+    @pulumi.getter(name="configurationDirectory")
+    def configuration_directory(self) -> pulumi.Output[Optional[str]]:
         """
-        IP masq.
+        The directory to use for etcd configuration.
         """
-        return pulumi.get(self, "ip_masq")
+        return pulumi.get(self, "configuration_directory")
 
     @property
-    @pulumi.getter
-    def ipam(self) -> pulumi.Output['outputs.CniBridgeIpam']:
+    @pulumi.getter(name="dataDirectory")
+    def data_directory(self) -> pulumi.Output[Optional[str]]:
         """
-        IPAM
+        The directory to use for etcd data.
         """
-        return pulumi.get(self, "ipam")
+        return pulumi.get(self, "data_directory")
 
     @property
-    @pulumi.getter(name="isGateway")
-    def is_gateway(self) -> pulumi.Output[bool]:
+    @pulumi.getter
+    def install(self) -> pulumi.Output[Mapping[str, 'EtcdInstall']]:
         """
-        Is gateway.
+        Map of node name to etcd install.
         """
-        return pulumi.get(self, "is_gateway")
+        return pulumi.get(self, "install")
 
     @property
     @pulumi.getter
-    def name(self) -> pulumi.Output[str]:
+    def nodes(self) -> pulumi.Output[Mapping[str, 'outputs.EtcdNode']]:
         """
-        CNI plugin name.
+        Etcd node configuration. The key should be a name used to identify the node.
         """
-        return pulumi.get(self, "name")
+        return pulumi.get(self, "nodes")
 
     @property
     @pulumi.getter
-    def path(self) -> pulumi.Output[str]:
+    def service(self) -> pulumi.Output[Mapping[str, 'EtcdService']]:
         """
-        Path to put the configuration file on the remote system
+        Map of node name to etcd systemd service.
         """
-        return pulumi.get(self, "path")
+        return pulumi.get(self, "service")
 
     @property
     @pulumi.getter
-    def subnet(self) -> pulumi.Output[Optional[str]]:
+    def start(self) -> pulumi.Output[Mapping[str, 'StartEtcd']]:
         """
-        The subnet to use.
+        Map of node name to etcd start commands.
         """
-        return pulumi.get(self, "subnet")
+        return pulumi.get(self, "start")
 
     @property
     @pulumi.getter
-    def type(self) -> pulumi.Output[str]:
+    def version(self) -> pulumi.Output[Optional[str]]:
         """
-        CNI plugin type.
+        The version to install.
         """
-        return pulumi.get(self, "type")
+        return pulumi.get(self, "version")
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/remote/cni_loopback_plugin_configuration.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/remote/download.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,224 +4,207 @@
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
-from .file import File
+from .. import tools as _tools
 import pulumi_command
 
-__all__ = ['CniLoopbackPluginConfigurationArgs', 'CniLoopbackPluginConfiguration']
+__all__ = ['DownloadArgs', 'Download']
 
 @pulumi.input_type
-class CniLoopbackPluginConfigurationArgs:
+class DownloadArgs:
     def __init__(__self__, *,
                  connection: pulumi.Input['pulumi_command.remote.ConnectionArgs'],
-                 cni_version: Optional[pulumi.Input[str]] = None,
-                 name: Optional[pulumi.Input[str]] = None,
-                 path: Optional[pulumi.Input[str]] = None,
-                 type: Optional[pulumi.Input[str]] = None):
+                 destination: pulumi.Input[str],
+                 url: pulumi.Input[str],
+                 remove_on_delete: Optional[bool] = None):
         """
-        The set of arguments for constructing a CniLoopbackPluginConfiguration resource.
+        The set of arguments for constructing a Download resource.
         :param pulumi.Input['pulumi_command.remote.ConnectionArgs'] connection: The parameters with which to connect to the remote host.
-        :param pulumi.Input[str] cni_version: CNI version.
-        :param pulumi.Input[str] name: CNI plugin name.
-        :param pulumi.Input[str] path: Path to put the configuration file on the remote system
-        :param pulumi.Input[str] type: CNI plugin type.
+        :param pulumi.Input[str] destination: The fully qualified path on the remote system where the file should be downloaded to.
+        :param pulumi.Input[str] url: The URL of the file to be downloaded.
+        :param bool remove_on_delete: Remove the downloaded fiel when the resource is deleted.
         """
         pulumi.set(__self__, "connection", connection)
-        if cni_version is not None:
-            pulumi.set(__self__, "cni_version", cni_version)
-        if name is not None:
-            pulumi.set(__self__, "name", name)
-        if path is not None:
-            pulumi.set(__self__, "path", path)
-        if type is not None:
-            pulumi.set(__self__, "type", type)
+        pulumi.set(__self__, "destination", destination)
+        pulumi.set(__self__, "url", url)
+        if remove_on_delete is not None:
+            pulumi.set(__self__, "remove_on_delete", remove_on_delete)
 
     @property
     @pulumi.getter
     def connection(self) -> pulumi.Input['pulumi_command.remote.ConnectionArgs']:
         """
         The parameters with which to connect to the remote host.
         """
         return pulumi.get(self, "connection")
 
     @connection.setter
     def connection(self, value: pulumi.Input['pulumi_command.remote.ConnectionArgs']):
         pulumi.set(self, "connection", value)
 
     @property
-    @pulumi.getter(name="cniVersion")
-    def cni_version(self) -> Optional[pulumi.Input[str]]:
-        """
-        CNI version.
-        """
-        return pulumi.get(self, "cni_version")
-
-    @cni_version.setter
-    def cni_version(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "cni_version", value)
-
-    @property
     @pulumi.getter
-    def name(self) -> Optional[pulumi.Input[str]]:
+    def destination(self) -> pulumi.Input[str]:
         """
-        CNI plugin name.
+        The fully qualified path on the remote system where the file should be downloaded to.
         """
-        return pulumi.get(self, "name")
+        return pulumi.get(self, "destination")
 
-    @name.setter
-    def name(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "name", value)
+    @destination.setter
+    def destination(self, value: pulumi.Input[str]):
+        pulumi.set(self, "destination", value)
 
     @property
     @pulumi.getter
-    def path(self) -> Optional[pulumi.Input[str]]:
+    def url(self) -> pulumi.Input[str]:
         """
-        Path to put the configuration file on the remote system
+        The URL of the file to be downloaded.
         """
-        return pulumi.get(self, "path")
+        return pulumi.get(self, "url")
 
-    @path.setter
-    def path(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "path", value)
+    @url.setter
+    def url(self, value: pulumi.Input[str]):
+        pulumi.set(self, "url", value)
 
     @property
-    @pulumi.getter
-    def type(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="removeOnDelete")
+    def remove_on_delete(self) -> Optional[bool]:
         """
-        CNI plugin type.
+        Remove the downloaded fiel when the resource is deleted.
         """
-        return pulumi.get(self, "type")
+        return pulumi.get(self, "remove_on_delete")
 
-    @type.setter
-    def type(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "type", value)
+    @remove_on_delete.setter
+    def remove_on_delete(self, value: Optional[bool]):
+        pulumi.set(self, "remove_on_delete", value)
 
 
-class CniLoopbackPluginConfiguration(pulumi.ComponentResource):
+class Download(pulumi.ComponentResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 cni_version: Optional[pulumi.Input[str]] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
-                 name: Optional[pulumi.Input[str]] = None,
-                 path: Optional[pulumi.Input[str]] = None,
-                 type: Optional[pulumi.Input[str]] = None,
+                 destination: Optional[pulumi.Input[str]] = None,
+                 remove_on_delete: Optional[bool] = None,
+                 url: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        The CNI loopback plugin configuration.
+        Downloads the file specified by `url` onto a remote system.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] cni_version: CNI version.
         :param pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']] connection: The parameters with which to connect to the remote host.
-        :param pulumi.Input[str] name: CNI plugin name.
-        :param pulumi.Input[str] path: Path to put the configuration file on the remote system
-        :param pulumi.Input[str] type: CNI plugin type.
+        :param pulumi.Input[str] destination: The fully qualified path on the remote system where the file should be downloaded to.
+        :param bool remove_on_delete: Remove the downloaded fiel when the resource is deleted.
+        :param pulumi.Input[str] url: The URL of the file to be downloaded.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: CniLoopbackPluginConfigurationArgs,
+                 args: DownloadArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        The CNI loopback plugin configuration.
+        Downloads the file specified by `url` onto a remote system.
 
         :param str resource_name: The name of the resource.
-        :param CniLoopbackPluginConfigurationArgs args: The arguments to use to populate this resource's properties.
+        :param DownloadArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(CniLoopbackPluginConfigurationArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(DownloadArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 cni_version: Optional[pulumi.Input[str]] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
-                 name: Optional[pulumi.Input[str]] = None,
-                 path: Optional[pulumi.Input[str]] = None,
-                 type: Optional[pulumi.Input[str]] = None,
+                 destination: Optional[pulumi.Input[str]] = None,
+                 remove_on_delete: Optional[bool] = None,
+                 url: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is not None:
             raise ValueError('ComponentResource classes do not support opts.id')
         else:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = CniLoopbackPluginConfigurationArgs.__new__(CniLoopbackPluginConfigurationArgs)
+            __props__ = DownloadArgs.__new__(DownloadArgs)
 
-            __props__.__dict__["cni_version"] = cni_version
             if connection is None and not opts.urn:
                 raise TypeError("Missing required property 'connection'")
             __props__.__dict__["connection"] = connection
-            __props__.__dict__["name"] = name
-            __props__.__dict__["path"] = path
-            __props__.__dict__["type"] = type
-            __props__.__dict__["file"] = None
-        super(CniLoopbackPluginConfiguration, __self__).__init__(
-            'kubernetes-the-hard-way:remote:CniLoopbackPluginConfiguration',
+            if destination is None and not opts.urn:
+                raise TypeError("Missing required property 'destination'")
+            __props__.__dict__["destination"] = destination
+            __props__.__dict__["remove_on_delete"] = remove_on_delete
+            if url is None and not opts.urn:
+                raise TypeError("Missing required property 'url'")
+            __props__.__dict__["url"] = url
+            __props__.__dict__["mkdir"] = None
+            __props__.__dict__["wget"] = None
+        super(Download, __self__).__init__(
+            'kubernetes-the-hard-way:remote:Download',
             resource_name,
             __props__,
             opts,
             remote=True)
 
     @property
-    @pulumi.getter(name="cniVersion")
-    def cni_version(self) -> pulumi.Output[str]:
-        """
-        CNI version.
-        """
-        return pulumi.get(self, "cni_version")
-
-    @property
     @pulumi.getter
     def connection(self) -> pulumi.Output['pulumi_command.remote.outputs.Connection']:
         """
         The parameters with which to connect to the remote host.
         """
         return pulumi.get(self, "connection")
 
     @property
     @pulumi.getter
-    def file(self) -> pulumi.Output[Optional['File']]:
+    def destination(self) -> pulumi.Output[str]:
         """
-        The file on the remote system.
+        The fully qualified path on the remote system where the file should be downloaded to.
         """
-        return pulumi.get(self, "file")
+        return pulumi.get(self, "destination")
 
     @property
     @pulumi.getter
-    def name(self) -> pulumi.Output[str]:
+    def mkdir(self) -> pulumi.Output['_tools.Mkdir']:
+        """
+        The mkdir operation.
+        """
+        return pulumi.get(self, "mkdir")
+
+    @property
+    @pulumi.getter(name="removeOnDelete")
+    def remove_on_delete(self) -> pulumi.Output[bool]:
         """
-        CNI plugin name.
+        Remove the downloaded fiel when the resource is deleted.
         """
-        return pulumi.get(self, "name")
+        return pulumi.get(self, "remove_on_delete")
 
     @property
     @pulumi.getter
-    def path(self) -> pulumi.Output[str]:
+    def url(self) -> pulumi.Output[str]:
         """
-        Path to put the configuration file on the remote system
+        The URL of the file to be downloaded.
         """
-        return pulumi.get(self, "path")
+        return pulumi.get(self, "url")
 
     @property
     @pulumi.getter
-    def type(self) -> pulumi.Output[str]:
+    def wget(self) -> pulumi.Output['_tools.Wget']:
         """
-        CNI plugin type.
+        The wget operation.
         """
-        return pulumi.get(self, "type")
+        return pulumi.get(self, "wget")
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/remote/cni_plugin_configuration.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/remote/static_pod.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,37 +4,38 @@
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
+from .. import config as _config
 from .. import tools as _tools
-from .cni_bridge_plugin_configuration import CniBridgePluginConfiguration
-from .cni_loopback_plugin_configuration import CniLoopbackPluginConfiguration
+from .file import File
 import pulumi_command
+import pulumi_kubernetes
 
-__all__ = ['CniPluginConfigurationArgs', 'CniPluginConfiguration']
+__all__ = ['StaticPodArgs', 'StaticPod']
 
 @pulumi.input_type
-class CniPluginConfigurationArgs:
+class StaticPodArgs:
     def __init__(__self__, *,
                  connection: pulumi.Input['pulumi_command.remote.ConnectionArgs'],
-                 subnet: pulumi.Input[str],
-                 directory: Optional[pulumi.Input[str]] = None):
+                 pod: pulumi.Input['_config.PodManifestArgs'],
+                 file_name: Optional[pulumi.Input[str]] = None):
         """
-        The set of arguments for constructing a CniPluginConfiguration resource.
+        The set of arguments for constructing a StaticPod resource.
         :param pulumi.Input['pulumi_command.remote.ConnectionArgs'] connection: The parameters with which to connect to the remote host.
-        :param pulumi.Input[str] subnet: The subnet to use for the CNI bridge plugin configuration.
-        :param pulumi.Input[str] directory: The plugin configuration directory.
+        :param pulumi.Input['_config.PodManifestArgs'] pod: The pod manifest.
+        :param pulumi.Input[str] file_name: The name of the file on the remote system.
         """
         pulumi.set(__self__, "connection", connection)
-        pulumi.set(__self__, "subnet", subnet)
-        if directory is not None:
-            pulumi.set(__self__, "directory", directory)
+        pulumi.set(__self__, "pod", pod)
+        if file_name is not None:
+            pulumi.set(__self__, "file_name", file_name)
 
     @property
     @pulumi.getter
     def connection(self) -> pulumi.Input['pulumi_command.remote.ConnectionArgs']:
         """
         The parameters with which to connect to the remote host.
         """
@@ -42,151 +43,151 @@
 
     @connection.setter
     def connection(self, value: pulumi.Input['pulumi_command.remote.ConnectionArgs']):
         pulumi.set(self, "connection", value)
 
     @property
     @pulumi.getter
-    def subnet(self) -> pulumi.Input[str]:
+    def pod(self) -> pulumi.Input['_config.PodManifestArgs']:
         """
-        The subnet to use for the CNI bridge plugin configuration.
+        The pod manifest.
         """
-        return pulumi.get(self, "subnet")
+        return pulumi.get(self, "pod")
 
-    @subnet.setter
-    def subnet(self, value: pulumi.Input[str]):
-        pulumi.set(self, "subnet", value)
+    @pod.setter
+    def pod(self, value: pulumi.Input['_config.PodManifestArgs']):
+        pulumi.set(self, "pod", value)
 
     @property
-    @pulumi.getter
-    def directory(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="fileName")
+    def file_name(self) -> Optional[pulumi.Input[str]]:
         """
-        The plugin configuration directory.
+        The name of the file on the remote system.
         """
-        return pulumi.get(self, "directory")
+        return pulumi.get(self, "file_name")
 
-    @directory.setter
-    def directory(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "directory", value)
+    @file_name.setter
+    def file_name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "file_name", value)
 
 
-class CniPluginConfiguration(pulumi.ComponentResource):
+class StaticPod(pulumi.ComponentResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
-                 directory: Optional[pulumi.Input[str]] = None,
-                 subnet: Optional[pulumi.Input[str]] = None,
+                 file_name: Optional[pulumi.Input[str]] = None,
+                 pod: Optional[pulumi.Input[pulumi.InputType['_config.PodManifestArgs']]] = None,
                  __props__=None):
         """
-        The CNI plugin configuration.
+        Create a static pod manifest on a remote system.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']] connection: The parameters with which to connect to the remote host.
-        :param pulumi.Input[str] directory: The plugin configuration directory.
-        :param pulumi.Input[str] subnet: The subnet to use for the CNI bridge plugin configuration.
+        :param pulumi.Input[str] file_name: The name of the file on the remote system.
+        :param pulumi.Input[pulumi.InputType['_config.PodManifestArgs']] pod: The pod manifest.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: CniPluginConfigurationArgs,
+                 args: StaticPodArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        The CNI plugin configuration.
+        Create a static pod manifest on a remote system.
 
         :param str resource_name: The name of the resource.
-        :param CniPluginConfigurationArgs args: The arguments to use to populate this resource's properties.
+        :param StaticPodArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(CniPluginConfigurationArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(StaticPodArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
-                 directory: Optional[pulumi.Input[str]] = None,
-                 subnet: Optional[pulumi.Input[str]] = None,
+                 file_name: Optional[pulumi.Input[str]] = None,
+                 pod: Optional[pulumi.Input[pulumi.InputType['_config.PodManifestArgs']]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is not None:
             raise ValueError('ComponentResource classes do not support opts.id')
         else:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = CniPluginConfigurationArgs.__new__(CniPluginConfigurationArgs)
+            __props__ = StaticPodArgs.__new__(StaticPodArgs)
 
             if connection is None and not opts.urn:
                 raise TypeError("Missing required property 'connection'")
             __props__.__dict__["connection"] = connection
-            __props__.__dict__["directory"] = directory
-            if subnet is None and not opts.urn:
-                raise TypeError("Missing required property 'subnet'")
-            __props__.__dict__["subnet"] = subnet
-            __props__.__dict__["bridge"] = None
-            __props__.__dict__["loopback"] = None
+            __props__.__dict__["file_name"] = file_name
+            if pod is None and not opts.urn:
+                raise TypeError("Missing required property 'pod'")
+            __props__.__dict__["pod"] = pod
+            __props__.__dict__["file"] = None
             __props__.__dict__["mkdir"] = None
-        super(CniPluginConfiguration, __self__).__init__(
-            'kubernetes-the-hard-way:remote:CniPluginConfiguration',
+            __props__.__dict__["path"] = None
+        super(StaticPod, __self__).__init__(
+            'kubernetes-the-hard-way:remote:StaticPod',
             resource_name,
             __props__,
             opts,
             remote=True)
 
     @property
     @pulumi.getter
-    def bridge(self) -> pulumi.Output['CniBridgePluginConfiguration']:
-        """
-        The bridge plugin configuration.
-        """
-        return pulumi.get(self, "bridge")
-
-    @property
-    @pulumi.getter
     def connection(self) -> pulumi.Output['pulumi_command.remote.outputs.Connection']:
         """
         The parameters with which to connect to the remote host.
         """
         return pulumi.get(self, "connection")
 
     @property
     @pulumi.getter
-    def directory(self) -> pulumi.Output[str]:
+    def file(self) -> pulumi.Output['File']:
         """
-        The plugin configuration directory.
+        The remote manifest file.
         """
-        return pulumi.get(self, "directory")
+        return pulumi.get(self, "file")
 
     @property
-    @pulumi.getter
-    def loopback(self) -> pulumi.Output['CniLoopbackPluginConfiguration']:
+    @pulumi.getter(name="fileName")
+    def file_name(self) -> pulumi.Output[str]:
         """
-        The loopback plugin configuration.
+        The name of the file on the remote system.
         """
-        return pulumi.get(self, "loopback")
+        return pulumi.get(self, "file_name")
 
     @property
     @pulumi.getter
     def mkdir(self) -> pulumi.Output['_tools.Mkdir']:
         """
-        The `directory` mkdir operation.
+        The mkdir operation to ensure /etc/kubernetes/manifests exists.
         """
         return pulumi.get(self, "mkdir")
 
     @property
     @pulumi.getter
-    def subnet(self) -> pulumi.Output[str]:
+    def path(self) -> pulumi.Output[str]:
+        """
+        The path to the manifest on the remote system.
+        """
+        return pulumi.get(self, "path")
+
+    @property
+    @pulumi.getter
+    def pod(self) -> pulumi.Output['_config.outputs.PodManifest']:
         """
-        The subnet to use for the CNI bridge plugin configuration.
+        The pod manifest.
         """
-        return pulumi.get(self, "subnet")
+        return pulumi.get(self, "pod")
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/remote/cni_plugins_install.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/remote/cni_plugins_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/remote/containerd_configuration.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/remote/start_kube_proxy.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,170 +4,130 @@
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
-from . import outputs
-from ._inputs import *
-from .file import File
+from .. import tools as _tools
 import pulumi_command
 
-__all__ = ['ContainerdConfigurationArgs', 'ContainerdConfiguration']
+__all__ = ['StartKubeProxyArgs', 'StartKubeProxy']
 
 @pulumi.input_type
-class ContainerdConfigurationArgs:
+class StartKubeProxyArgs:
     def __init__(__self__, *,
-                 connection: pulumi.Input['pulumi_command.remote.ConnectionArgs'],
-                 cri: Optional['ContainerdCriPluginConfigurationArgs'] = None,
-                 path: Optional[pulumi.Input[str]] = None):
+                 connection: pulumi.Input['pulumi_command.remote.ConnectionArgs']):
         """
-        The set of arguments for constructing a ContainerdConfiguration resource.
+        The set of arguments for constructing a StartKubeProxy resource.
         :param pulumi.Input['pulumi_command.remote.ConnectionArgs'] connection: The parameters with which to connect to the remote host.
-        :param 'ContainerdCriPluginConfigurationArgs' cri: The cri configuration.
-        :param pulumi.Input[str] path: The path to put the configuration file.
         """
         pulumi.set(__self__, "connection", connection)
-        if cri is not None:
-            pulumi.set(__self__, "cri", cri)
-        if path is not None:
-            pulumi.set(__self__, "path", path)
 
     @property
     @pulumi.getter
     def connection(self) -> pulumi.Input['pulumi_command.remote.ConnectionArgs']:
         """
         The parameters with which to connect to the remote host.
         """
         return pulumi.get(self, "connection")
 
     @connection.setter
     def connection(self, value: pulumi.Input['pulumi_command.remote.ConnectionArgs']):
         pulumi.set(self, "connection", value)
 
-    @property
-    @pulumi.getter
-    def cri(self) -> Optional['ContainerdCriPluginConfigurationArgs']:
-        """
-        The cri configuration.
-        """
-        return pulumi.get(self, "cri")
 
-    @cri.setter
-    def cri(self, value: Optional['ContainerdCriPluginConfigurationArgs']):
-        pulumi.set(self, "cri", value)
-
-    @property
-    @pulumi.getter
-    def path(self) -> Optional[pulumi.Input[str]]:
-        """
-        The path to put the configuration file.
-        """
-        return pulumi.get(self, "path")
-
-    @path.setter
-    def path(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "path", value)
-
-
-class ContainerdConfiguration(pulumi.ComponentResource):
+class StartKubeProxy(pulumi.ComponentResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
-                 cri: Optional[pulumi.InputType['ContainerdCriPluginConfigurationArgs']] = None,
-                 path: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        The containerd configuration file.
+        Starts `kube-proxy` on a remote system
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']] connection: The parameters with which to connect to the remote host.
-        :param pulumi.InputType['ContainerdCriPluginConfigurationArgs'] cri: The cri configuration.
-        :param pulumi.Input[str] path: The path to put the configuration file.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: ContainerdConfigurationArgs,
+                 args: StartKubeProxyArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        The containerd configuration file.
+        Starts `kube-proxy` on a remote system
 
         :param str resource_name: The name of the resource.
-        :param ContainerdConfigurationArgs args: The arguments to use to populate this resource's properties.
+        :param StartKubeProxyArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(ContainerdConfigurationArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(StartKubeProxyArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
-                 cri: Optional[pulumi.InputType['ContainerdCriPluginConfigurationArgs']] = None,
-                 path: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is not None:
             raise ValueError('ComponentResource classes do not support opts.id')
         else:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = ContainerdConfigurationArgs.__new__(ContainerdConfigurationArgs)
+            __props__ = StartKubeProxyArgs.__new__(StartKubeProxyArgs)
 
             if connection is None and not opts.urn:
                 raise TypeError("Missing required property 'connection'")
             __props__.__dict__["connection"] = connection
-            __props__.__dict__["cri"] = cri
-            __props__.__dict__["path"] = path
-            __props__.__dict__["file"] = None
-        super(ContainerdConfiguration, __self__).__init__(
-            'kubernetes-the-hard-way:remote:ContainerdConfiguration',
+            __props__.__dict__["daemon_reload"] = None
+            __props__.__dict__["enable"] = None
+            __props__.__dict__["start"] = None
+        super(StartKubeProxy, __self__).__init__(
+            'kubernetes-the-hard-way:remote:StartKubeProxy',
             resource_name,
             __props__,
             opts,
             remote=True)
 
     @property
     @pulumi.getter
     def connection(self) -> pulumi.Output['pulumi_command.remote.outputs.Connection']:
         """
         The parameters with which to connect to the remote host.
         """
         return pulumi.get(self, "connection")
 
     @property
-    @pulumi.getter
-    def cri(self) -> pulumi.Output['outputs.ContainerdCriPluginConfiguration']:
+    @pulumi.getter(name="daemonReload")
+    def daemon_reload(self) -> pulumi.Output['_tools.Systemctl']:
         """
-        The cri configuration.
+        The daemon-reload command.
         """
-        return pulumi.get(self, "cri")
+        return pulumi.get(self, "daemon_reload")
 
     @property
     @pulumi.getter
-    def file(self) -> pulumi.Output['File']:
+    def enable(self) -> pulumi.Output['_tools.Systemctl']:
         """
-        The remote configuration file.
+        The enable command.
         """
-        return pulumi.get(self, "file")
+        return pulumi.get(self, "enable")
 
     @property
     @pulumi.getter
-    def path(self) -> pulumi.Output[Optional[str]]:
+    def start(self) -> pulumi.Output['_tools.Systemctl']:
         """
-        The path to put the configuration file.
+        The start command.
         """
-        return pulumi.get(self, "path")
+        return pulumi.get(self, "start")
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/remote/containerd_install.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/remote/containerd_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/remote/crictl_install.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/remote/crictl_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/remote/download.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/remote/file.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,38 +4,33 @@
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
-from .. import tools as _tools
 import pulumi_command
 
-__all__ = ['DownloadArgs', 'Download']
+__all__ = ['FileArgs', 'File']
 
 @pulumi.input_type
-class DownloadArgs:
+class FileArgs:
     def __init__(__self__, *,
                  connection: pulumi.Input['pulumi_command.remote.ConnectionArgs'],
-                 destination: pulumi.Input[str],
-                 url: pulumi.Input[str],
-                 remove_on_delete: Optional[bool] = None):
+                 content: pulumi.Input[str],
+                 path: pulumi.Input[str]):
         """
-        The set of arguments for constructing a Download resource.
+        The set of arguments for constructing a File resource.
         :param pulumi.Input['pulumi_command.remote.ConnectionArgs'] connection: The parameters with which to connect to the remote host.
-        :param pulumi.Input[str] destination: The fully qualified path on the remote system where the file should be downloaded to.
-        :param pulumi.Input[str] url: The URL of the file to be downloaded.
-        :param bool remove_on_delete: Remove the downloaded fiel when the resource is deleted.
+        :param pulumi.Input[str] content: The content of the file.
+        :param pulumi.Input[str] path: The path to the file on the remote host.
         """
         pulumi.set(__self__, "connection", connection)
-        pulumi.set(__self__, "destination", destination)
-        pulumi.set(__self__, "url", url)
-        if remove_on_delete is not None:
-            pulumi.set(__self__, "remove_on_delete", remove_on_delete)
+        pulumi.set(__self__, "content", content)
+        pulumi.set(__self__, "path", path)
 
     @property
     @pulumi.getter
     def connection(self) -> pulumi.Input['pulumi_command.remote.ConnectionArgs']:
         """
         The parameters with which to connect to the remote host.
         """
@@ -43,168 +38,160 @@
 
     @connection.setter
     def connection(self, value: pulumi.Input['pulumi_command.remote.ConnectionArgs']):
         pulumi.set(self, "connection", value)
 
     @property
     @pulumi.getter
-    def destination(self) -> pulumi.Input[str]:
+    def content(self) -> pulumi.Input[str]:
         """
-        The fully qualified path on the remote system where the file should be downloaded to.
+        The content of the file.
         """
-        return pulumi.get(self, "destination")
+        return pulumi.get(self, "content")
 
-    @destination.setter
-    def destination(self, value: pulumi.Input[str]):
-        pulumi.set(self, "destination", value)
+    @content.setter
+    def content(self, value: pulumi.Input[str]):
+        pulumi.set(self, "content", value)
 
     @property
     @pulumi.getter
-    def url(self) -> pulumi.Input[str]:
+    def path(self) -> pulumi.Input[str]:
         """
-        The URL of the file to be downloaded.
+        The path to the file on the remote host.
         """
-        return pulumi.get(self, "url")
+        return pulumi.get(self, "path")
 
-    @url.setter
-    def url(self, value: pulumi.Input[str]):
-        pulumi.set(self, "url", value)
+    @path.setter
+    def path(self, value: pulumi.Input[str]):
+        pulumi.set(self, "path", value)
 
-    @property
-    @pulumi.getter(name="removeOnDelete")
-    def remove_on_delete(self) -> Optional[bool]:
-        """
-        Remove the downloaded fiel when the resource is deleted.
-        """
-        return pulumi.get(self, "remove_on_delete")
-
-    @remove_on_delete.setter
-    def remove_on_delete(self, value: Optional[bool]):
-        pulumi.set(self, "remove_on_delete", value)
 
-
-class Download(pulumi.ComponentResource):
+class File(pulumi.ComponentResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
-                 destination: Optional[pulumi.Input[str]] = None,
-                 remove_on_delete: Optional[bool] = None,
-                 url: Optional[pulumi.Input[str]] = None,
+                 content: Optional[pulumi.Input[str]] = None,
+                 path: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        Downloads the file specified by `url` onto a remote system.
-
+        Create a File resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']] connection: The parameters with which to connect to the remote host.
-        :param pulumi.Input[str] destination: The fully qualified path on the remote system where the file should be downloaded to.
-        :param bool remove_on_delete: Remove the downloaded fiel when the resource is deleted.
-        :param pulumi.Input[str] url: The URL of the file to be downloaded.
+        :param pulumi.Input[str] content: The content of the file.
+        :param pulumi.Input[str] path: The path to the file on the remote host.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: DownloadArgs,
+                 args: FileArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Downloads the file specified by `url` onto a remote system.
-
+        Create a File resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
-        :param DownloadArgs args: The arguments to use to populate this resource's properties.
+        :param FileArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(DownloadArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(FileArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
-                 destination: Optional[pulumi.Input[str]] = None,
-                 remove_on_delete: Optional[bool] = None,
-                 url: Optional[pulumi.Input[str]] = None,
+                 content: Optional[pulumi.Input[str]] = None,
+                 path: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is not None:
             raise ValueError('ComponentResource classes do not support opts.id')
         else:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = DownloadArgs.__new__(DownloadArgs)
+            __props__ = FileArgs.__new__(FileArgs)
 
             if connection is None and not opts.urn:
                 raise TypeError("Missing required property 'connection'")
             __props__.__dict__["connection"] = connection
-            if destination is None and not opts.urn:
-                raise TypeError("Missing required property 'destination'")
-            __props__.__dict__["destination"] = destination
-            __props__.__dict__["remove_on_delete"] = remove_on_delete
-            if url is None and not opts.urn:
-                raise TypeError("Missing required property 'url'")
-            __props__.__dict__["url"] = url
-            __props__.__dict__["mkdir"] = None
-            __props__.__dict__["wget"] = None
-        super(Download, __self__).__init__(
-            'kubernetes-the-hard-way:remote:Download',
+            if content is None and not opts.urn:
+                raise TypeError("Missing required property 'content'")
+            __props__.__dict__["content"] = content
+            if path is None and not opts.urn:
+                raise TypeError("Missing required property 'path'")
+            __props__.__dict__["path"] = path
+            __props__.__dict__["command"] = None
+            __props__.__dict__["stderr"] = None
+            __props__.__dict__["stdin"] = None
+            __props__.__dict__["stdout"] = None
+        super(File, __self__).__init__(
+            'kubernetes-the-hard-way:remote:File',
             resource_name,
             __props__,
             opts,
             remote=True)
 
     @property
     @pulumi.getter
+    def command(self) -> pulumi.Output['pulumi_command.remote.Command']:
+        """
+        The executed command.
+        """
+        return pulumi.get(self, "command")
+
+    @property
+    @pulumi.getter
     def connection(self) -> pulumi.Output['pulumi_command.remote.outputs.Connection']:
         """
         The parameters with which to connect to the remote host.
         """
         return pulumi.get(self, "connection")
 
     @property
     @pulumi.getter
-    def destination(self) -> pulumi.Output[str]:
+    def content(self) -> pulumi.Output[str]:
         """
-        The fully qualified path on the remote system where the file should be downloaded to.
+        The content of the file.
         """
-        return pulumi.get(self, "destination")
+        return pulumi.get(self, "content")
 
     @property
     @pulumi.getter
-    def mkdir(self) -> pulumi.Output['_tools.Mkdir']:
+    def path(self) -> pulumi.Output[str]:
         """
-        The mkdir operation.
+        The path to the file on the remote host.
         """
-        return pulumi.get(self, "mkdir")
+        return pulumi.get(self, "path")
 
     @property
-    @pulumi.getter(name="removeOnDelete")
-    def remove_on_delete(self) -> pulumi.Output[bool]:
+    @pulumi.getter
+    def stderr(self) -> pulumi.Output[str]:
         """
-        Remove the downloaded fiel when the resource is deleted.
+        The standard error of the command's process
         """
-        return pulumi.get(self, "remove_on_delete")
+        return pulumi.get(self, "stderr")
 
     @property
     @pulumi.getter
-    def url(self) -> pulumi.Output[str]:
+    def stdin(self) -> pulumi.Output[str]:
         """
-        The URL of the file to be downloaded.
+        Pass a string to the command's process as standard in
         """
-        return pulumi.get(self, "url")
+        return pulumi.get(self, "stdin")
 
     @property
     @pulumi.getter
-    def wget(self) -> pulumi.Output['_tools.Wget']:
+    def stdout(self) -> pulumi.Output[str]:
         """
-        The wget operation.
+        The standard output of the command's process
         """
-        return pulumi.get(self, "wget")
+        return pulumi.get(self, "stdout")
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/remote/etcd_cluster.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/remote/provision_etcd.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,48 +4,49 @@
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
-from . import outputs
 from .. import tls as _tls
 from ._enums import *
-from ._inputs import *
 from .etcd_configuration import EtcdConfiguration
 from .etcd_install import EtcdInstall
-from .etcd_service import EtcdService
 from .start_etcd import StartEtcd
+from .systemd_service import SystemdService
 import pulumi_command
 
-__all__ = ['EtcdClusterArgs', 'EtcdCluster']
+__all__ = ['ProvisionEtcdArgs', 'ProvisionEtcd']
 
 @pulumi.input_type
-class EtcdClusterArgs:
+class ProvisionEtcdArgs:
     def __init__(__self__, *,
                  bundle: pulumi.Input['_tls.BundleArgs'],
-                 nodes: Mapping[str, pulumi.Input['EtcdNodeArgs']],
+                 connection: pulumi.Input['pulumi_command.remote.ConnectionArgs'],
+                 internal_ip: pulumi.Input[str],
                  architecture: Optional[pulumi.Input['Architecture']] = None,
                  binary_directory: Optional[pulumi.Input[str]] = None,
                  configuration_directory: Optional[pulumi.Input[str]] = None,
                  data_directory: Optional[pulumi.Input[str]] = None,
                  version: Optional[pulumi.Input[str]] = None):
         """
-        The set of arguments for constructing a EtcdCluster resource.
+        The set of arguments for constructing a ProvisionEtcd resource.
         :param pulumi.Input['_tls.BundleArgs'] bundle: The TLS bundle.
-        :param Mapping[str, pulumi.Input['EtcdNodeArgs']] nodes: Etcd node configuration. The key should be a name used to identify the node.
+        :param pulumi.Input['pulumi_command.remote.ConnectionArgs'] connection: The parameters with which to connect to the remote host.
+        :param pulumi.Input[str] internal_ip: The internal IP of the etcd node
         :param pulumi.Input['Architecture'] architecture: TODO
         :param pulumi.Input[str] binary_directory: TODO
         :param pulumi.Input[str] configuration_directory: The directory to use for etcd configuration.
         :param pulumi.Input[str] data_directory: The directory to use for etcd data.
         :param pulumi.Input[str] version: The version to install.
         """
         pulumi.set(__self__, "bundle", bundle)
-        pulumi.set(__self__, "nodes", nodes)
+        pulumi.set(__self__, "connection", connection)
+        pulumi.set(__self__, "internal_ip", internal_ip)
         if architecture is not None:
             pulumi.set(__self__, "architecture", architecture)
         if binary_directory is not None:
             pulumi.set(__self__, "binary_directory", binary_directory)
         if configuration_directory is not None:
             pulumi.set(__self__, "configuration_directory", configuration_directory)
         if data_directory is not None:
@@ -63,23 +64,35 @@
 
     @bundle.setter
     def bundle(self, value: pulumi.Input['_tls.BundleArgs']):
         pulumi.set(self, "bundle", value)
 
     @property
     @pulumi.getter
-    def nodes(self) -> Mapping[str, pulumi.Input['EtcdNodeArgs']]:
+    def connection(self) -> pulumi.Input['pulumi_command.remote.ConnectionArgs']:
         """
-        Etcd node configuration. The key should be a name used to identify the node.
+        The parameters with which to connect to the remote host.
         """
-        return pulumi.get(self, "nodes")
+        return pulumi.get(self, "connection")
 
-    @nodes.setter
-    def nodes(self, value: Mapping[str, pulumi.Input['EtcdNodeArgs']]):
-        pulumi.set(self, "nodes", value)
+    @connection.setter
+    def connection(self, value: pulumi.Input['pulumi_command.remote.ConnectionArgs']):
+        pulumi.set(self, "connection", value)
+
+    @property
+    @pulumi.getter(name="internalIp")
+    def internal_ip(self) -> pulumi.Input[str]:
+        """
+        The internal IP of the etcd node
+        """
+        return pulumi.get(self, "internal_ip")
+
+    @internal_ip.setter
+    def internal_ip(self, value: pulumi.Input[str]):
+        pulumi.set(self, "internal_ip", value)
 
     @property
     @pulumi.getter
     def architecture(self) -> Optional[pulumi.Input['Architecture']]:
         """
         TODO
         """
@@ -134,99 +147,105 @@
         return pulumi.get(self, "version")
 
     @version.setter
     def version(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "version", value)
 
 
-class EtcdCluster(pulumi.ComponentResource):
+class ProvisionEtcd(pulumi.ComponentResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  architecture: Optional[pulumi.Input['Architecture']] = None,
                  binary_directory: Optional[pulumi.Input[str]] = None,
                  bundle: Optional[pulumi.Input[pulumi.InputType['_tls.BundleArgs']]] = None,
                  configuration_directory: Optional[pulumi.Input[str]] = None,
+                 connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
                  data_directory: Optional[pulumi.Input[str]] = None,
-                 nodes: Optional[Mapping[str, pulumi.Input[pulumi.InputType['EtcdNodeArgs']]]] = None,
+                 internal_ip: Optional[pulumi.Input[str]] = None,
                  version: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        Creates an etcd cluster from one or more remote systems.
+        Starts etcd on a remote system.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input['Architecture'] architecture: TODO
         :param pulumi.Input[str] binary_directory: TODO
         :param pulumi.Input[pulumi.InputType['_tls.BundleArgs']] bundle: The TLS bundle.
         :param pulumi.Input[str] configuration_directory: The directory to use for etcd configuration.
+        :param pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']] connection: The parameters with which to connect to the remote host.
         :param pulumi.Input[str] data_directory: The directory to use for etcd data.
-        :param Mapping[str, pulumi.Input[pulumi.InputType['EtcdNodeArgs']]] nodes: Etcd node configuration. The key should be a name used to identify the node.
+        :param pulumi.Input[str] internal_ip: The internal IP of the etcd node
         :param pulumi.Input[str] version: The version to install.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: EtcdClusterArgs,
+                 args: ProvisionEtcdArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Creates an etcd cluster from one or more remote systems.
+        Starts etcd on a remote system.
 
         :param str resource_name: The name of the resource.
-        :param EtcdClusterArgs args: The arguments to use to populate this resource's properties.
+        :param ProvisionEtcdArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(EtcdClusterArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(ProvisionEtcdArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  architecture: Optional[pulumi.Input['Architecture']] = None,
                  binary_directory: Optional[pulumi.Input[str]] = None,
                  bundle: Optional[pulumi.Input[pulumi.InputType['_tls.BundleArgs']]] = None,
                  configuration_directory: Optional[pulumi.Input[str]] = None,
+                 connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
                  data_directory: Optional[pulumi.Input[str]] = None,
-                 nodes: Optional[Mapping[str, pulumi.Input[pulumi.InputType['EtcdNodeArgs']]]] = None,
+                 internal_ip: Optional[pulumi.Input[str]] = None,
                  version: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is not None:
             raise ValueError('ComponentResource classes do not support opts.id')
         else:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = EtcdClusterArgs.__new__(EtcdClusterArgs)
+            __props__ = ProvisionEtcdArgs.__new__(ProvisionEtcdArgs)
 
             __props__.__dict__["architecture"] = architecture
             __props__.__dict__["binary_directory"] = binary_directory
             if bundle is None and not opts.urn:
                 raise TypeError("Missing required property 'bundle'")
             __props__.__dict__["bundle"] = bundle
             __props__.__dict__["configuration_directory"] = configuration_directory
+            if connection is None and not opts.urn:
+                raise TypeError("Missing required property 'connection'")
+            __props__.__dict__["connection"] = connection
             __props__.__dict__["data_directory"] = data_directory
-            if nodes is None and not opts.urn:
-                raise TypeError("Missing required property 'nodes'")
-            __props__.__dict__["nodes"] = nodes
+            if internal_ip is None and not opts.urn:
+                raise TypeError("Missing required property 'internal_ip'")
+            __props__.__dict__["internal_ip"] = internal_ip
             __props__.__dict__["version"] = version
             __props__.__dict__["configuration"] = None
             __props__.__dict__["install"] = None
             __props__.__dict__["service"] = None
             __props__.__dict__["start"] = None
-        super(EtcdCluster, __self__).__init__(
-            'kubernetes-the-hard-way:remote:EtcdCluster',
+        super(ProvisionEtcd, __self__).__init__(
+            'kubernetes-the-hard-way:remote:ProvisionEtcd',
             resource_name,
             __props__,
             opts,
             remote=True)
 
     @property
     @pulumi.getter
@@ -250,65 +269,73 @@
         """
         The TLS bundle.
         """
         return pulumi.get(self, "bundle")
 
     @property
     @pulumi.getter
-    def configuration(self) -> pulumi.Output[Mapping[str, 'EtcdConfiguration']]:
+    def configuration(self) -> pulumi.Output['EtcdConfiguration']:
         """
-        Map of node name to etcd configuration.
+        Etcd configuration.
         """
         return pulumi.get(self, "configuration")
 
     @property
     @pulumi.getter(name="configurationDirectory")
     def configuration_directory(self) -> pulumi.Output[Optional[str]]:
         """
         The directory to use for etcd configuration.
         """
         return pulumi.get(self, "configuration_directory")
 
     @property
+    @pulumi.getter
+    def connection(self) -> pulumi.Output['pulumi_command.remote.outputs.Connection']:
+        """
+        The parameters with which to connect to the remote host.
+        """
+        return pulumi.get(self, "connection")
+
+    @property
     @pulumi.getter(name="dataDirectory")
     def data_directory(self) -> pulumi.Output[Optional[str]]:
         """
         The directory to use for etcd data.
         """
         return pulumi.get(self, "data_directory")
 
     @property
     @pulumi.getter
-    def install(self) -> pulumi.Output[Mapping[str, 'EtcdInstall']]:
+    def install(self) -> pulumi.Output['EtcdInstall']:
         """
-        Map of node name to etcd install.
+        Install etcd.
         """
         return pulumi.get(self, "install")
 
     @property
-    @pulumi.getter
-    def nodes(self) -> pulumi.Output[Mapping[str, 'outputs.EtcdNode']]:
+    @pulumi.getter(name="internalIp")
+    def internal_ip(self) -> pulumi.Output[str]:
         """
-        Etcd node configuration. The key should be a name used to identify the node.
+        The internal IP of the etcd node
         """
-        return pulumi.get(self, "nodes")
+        return pulumi.get(self, "internal_ip")
 
     @property
     @pulumi.getter
-    def service(self) -> pulumi.Output[Mapping[str, 'EtcdService']]:
+    def service(self) -> pulumi.Output['SystemdService']:
         """
-        Map of node name to etcd systemd service.
+        Systemd service.
         """
         return pulumi.get(self, "service")
 
     @property
     @pulumi.getter
-    def start(self) -> pulumi.Output[Mapping[str, 'StartEtcd']]:
+    def start(self) -> pulumi.Output['StartEtcd']:
         """
-        Map of node name to etcd start commands.
+        Start etcd
         """
         return pulumi.get(self, "start")
 
     @property
     @pulumi.getter
     def version(self) -> pulumi.Output[Optional[str]]:
         """
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/remote/etcd_configuration.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/remote/etcd_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/remote/etcd_install.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/remote/etcd_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/remote/etcd_service.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/remote/etcd_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/remote/file.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/remote/start_etcd.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,194 +4,130 @@
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
+from .. import tools as _tools
 import pulumi_command
 
-__all__ = ['FileArgs', 'File']
+__all__ = ['StartEtcdArgs', 'StartEtcd']
 
 @pulumi.input_type
-class FileArgs:
+class StartEtcdArgs:
     def __init__(__self__, *,
-                 connection: pulumi.Input['pulumi_command.remote.ConnectionArgs'],
-                 content: pulumi.Input[str],
-                 path: pulumi.Input[str]):
+                 connection: pulumi.Input['pulumi_command.remote.ConnectionArgs']):
         """
-        The set of arguments for constructing a File resource.
+        The set of arguments for constructing a StartEtcd resource.
         :param pulumi.Input['pulumi_command.remote.ConnectionArgs'] connection: The parameters with which to connect to the remote host.
-        :param pulumi.Input[str] content: The content of the file.
-        :param pulumi.Input[str] path: The path to the file on the remote host.
         """
         pulumi.set(__self__, "connection", connection)
-        pulumi.set(__self__, "content", content)
-        pulumi.set(__self__, "path", path)
 
     @property
     @pulumi.getter
     def connection(self) -> pulumi.Input['pulumi_command.remote.ConnectionArgs']:
         """
         The parameters with which to connect to the remote host.
         """
         return pulumi.get(self, "connection")
 
     @connection.setter
     def connection(self, value: pulumi.Input['pulumi_command.remote.ConnectionArgs']):
         pulumi.set(self, "connection", value)
 
-    @property
-    @pulumi.getter
-    def content(self) -> pulumi.Input[str]:
-        """
-        The content of the file.
-        """
-        return pulumi.get(self, "content")
 
-    @content.setter
-    def content(self, value: pulumi.Input[str]):
-        pulumi.set(self, "content", value)
-
-    @property
-    @pulumi.getter
-    def path(self) -> pulumi.Input[str]:
-        """
-        The path to the file on the remote host.
-        """
-        return pulumi.get(self, "path")
-
-    @path.setter
-    def path(self, value: pulumi.Input[str]):
-        pulumi.set(self, "path", value)
-
-
-class File(pulumi.ComponentResource):
+class StartEtcd(pulumi.ComponentResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
-                 content: Optional[pulumi.Input[str]] = None,
-                 path: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        Create a File resource with the given unique name, props, and options.
+        Starts `etcd` on a remote system
+
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']] connection: The parameters with which to connect to the remote host.
-        :param pulumi.Input[str] content: The content of the file.
-        :param pulumi.Input[str] path: The path to the file on the remote host.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: FileArgs,
+                 args: StartEtcdArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Create a File resource with the given unique name, props, and options.
+        Starts `etcd` on a remote system
+
         :param str resource_name: The name of the resource.
-        :param FileArgs args: The arguments to use to populate this resource's properties.
+        :param StartEtcdArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(FileArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(StartEtcdArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
-                 content: Optional[pulumi.Input[str]] = None,
-                 path: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is not None:
             raise ValueError('ComponentResource classes do not support opts.id')
         else:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = FileArgs.__new__(FileArgs)
+            __props__ = StartEtcdArgs.__new__(StartEtcdArgs)
 
             if connection is None and not opts.urn:
                 raise TypeError("Missing required property 'connection'")
             __props__.__dict__["connection"] = connection
-            if content is None and not opts.urn:
-                raise TypeError("Missing required property 'content'")
-            __props__.__dict__["content"] = content
-            if path is None and not opts.urn:
-                raise TypeError("Missing required property 'path'")
-            __props__.__dict__["path"] = path
-            __props__.__dict__["command"] = None
-            __props__.__dict__["stderr"] = None
-            __props__.__dict__["stdin"] = None
-            __props__.__dict__["stdout"] = None
-        super(File, __self__).__init__(
-            'kubernetes-the-hard-way:remote:File',
+            __props__.__dict__["daemon_reload"] = None
+            __props__.__dict__["enable"] = None
+            __props__.__dict__["start"] = None
+        super(StartEtcd, __self__).__init__(
+            'kubernetes-the-hard-way:remote:StartEtcd',
             resource_name,
             __props__,
             opts,
             remote=True)
 
     @property
     @pulumi.getter
-    def command(self) -> pulumi.Output['pulumi_command.remote.Command']:
-        """
-        The executed command.
-        """
-        return pulumi.get(self, "command")
-
-    @property
-    @pulumi.getter
     def connection(self) -> pulumi.Output['pulumi_command.remote.outputs.Connection']:
         """
         The parameters with which to connect to the remote host.
         """
         return pulumi.get(self, "connection")
 
     @property
-    @pulumi.getter
-    def content(self) -> pulumi.Output[str]:
-        """
-        The content of the file.
-        """
-        return pulumi.get(self, "content")
-
-    @property
-    @pulumi.getter
-    def path(self) -> pulumi.Output[str]:
-        """
-        The path to the file on the remote host.
-        """
-        return pulumi.get(self, "path")
-
-    @property
-    @pulumi.getter
-    def stderr(self) -> pulumi.Output[str]:
+    @pulumi.getter(name="daemonReload")
+    def daemon_reload(self) -> pulumi.Output['_tools.Systemctl']:
         """
-        The standard error of the command's process
+        The daemon-reload command.
         """
-        return pulumi.get(self, "stderr")
+        return pulumi.get(self, "daemon_reload")
 
     @property
     @pulumi.getter
-    def stdin(self) -> pulumi.Output[str]:
+    def enable(self) -> pulumi.Output['_tools.Systemctl']:
         """
-        Pass a string to the command's process as standard in
+        The enable command.
         """
-        return pulumi.get(self, "stdin")
+        return pulumi.get(self, "enable")
 
     @property
     @pulumi.getter
-    def stdout(self) -> pulumi.Output[str]:
+    def start(self) -> pulumi.Output['_tools.Systemctl']:
         """
-        The standard output of the command's process
+        The start command.
         """
-        return pulumi.get(self, "stdout")
+        return pulumi.get(self, "start")
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/remote/kube_api_server_install.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/remote/kube_api_server_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/remote/kube_controller_manager_install.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/remote/kube_controller_manager_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/remote/kube_proxy_install.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/remote/kube_proxy_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/remote/kube_proxy_service.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/remote/kube_proxy_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/remote/kube_scheduler_install.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/remote/kube_scheduler_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/remote/kubectl_install.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/remote/kubectl_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/remote/kubelet_install.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/remote/kubelet_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/remote/kubelet_service.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/remote/kubelet_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/remote/outputs.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/remote/outputs.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,324 +4,28 @@
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
-from . import outputs
 from ._enums import *
 import pulumi_command
 
 __all__ = [
-    'CniBridgeIpam',
-    'ContainerdCriPluginConfiguration',
-    'ContainerdCriPluginConfigurationCni',
-    'ContainerdCriPluginConfigurationContainerd',
-    'ContainerdCriPluginConfigurationContainerdRunc',
-    'ContainerdCriPluginConfigurationContainerdRuncOptions',
     'EtcdConfigurationProps',
     'EtcdNode',
     'KubeProxyConfigurationProps',
     'KubeletConfigurationProps',
     'SystemdInstallSection',
     'SystemdServiceSection',
     'SystemdUnitSection',
 ]
 
 @pulumi.output_type
-class CniBridgeIpam(dict):
-    """
-    The CNI plugins IPAM
-    """
-    def __init__(__self__, *,
-                 ranges: Optional[Sequence[Mapping[str, str]]] = None,
-                 routes: Optional[Sequence[Mapping[str, str]]] = None,
-                 type: Optional[str] = None):
-        """
-        The CNI plugins IPAM
-        :param Sequence[Mapping[str, str]] ranges: IPAM ranges.
-        :param Sequence[Mapping[str, str]] routes: IPAM routes.
-        :param str type: CNI bridge IPAM type
-        """
-        if ranges is not None:
-            pulumi.set(__self__, "ranges", ranges)
-        if routes is not None:
-            pulumi.set(__self__, "routes", routes)
-        if type is not None:
-            pulumi.set(__self__, "type", type)
-
-    @property
-    @pulumi.getter
-    def ranges(self) -> Optional[Sequence[Mapping[str, str]]]:
-        """
-        IPAM ranges.
-        """
-        return pulumi.get(self, "ranges")
-
-    @property
-    @pulumi.getter
-    def routes(self) -> Optional[Sequence[Mapping[str, str]]]:
-        """
-        IPAM routes.
-        """
-        return pulumi.get(self, "routes")
-
-    @property
-    @pulumi.getter
-    def type(self) -> Optional[str]:
-        """
-        CNI bridge IPAM type
-        """
-        return pulumi.get(self, "type")
-
-
-@pulumi.output_type
-class ContainerdCriPluginConfiguration(dict):
-    """
-    containerd cri plugin configuration.
-    """
-    def __init__(__self__, *,
-                 cni: 'outputs.ContainerdCriPluginConfigurationCni',
-                 containerd: 'outputs.ContainerdCriPluginConfigurationContainerd'):
-        """
-        containerd cri plugin configuration.
-        :param 'ContainerdCriPluginConfigurationCni' cni: cni configuration.
-        :param 'ContainerdCriPluginConfigurationContainerd' containerd: containerd configuration.
-        """
-        pulumi.set(__self__, "cni", cni)
-        pulumi.set(__self__, "containerd", containerd)
-
-    @property
-    @pulumi.getter
-    def cni(self) -> 'outputs.ContainerdCriPluginConfigurationCni':
-        """
-        cni configuration.
-        """
-        return pulumi.get(self, "cni")
-
-    @property
-    @pulumi.getter
-    def containerd(self) -> 'outputs.ContainerdCriPluginConfigurationContainerd':
-        """
-        containerd configuration.
-        """
-        return pulumi.get(self, "containerd")
-
-
-@pulumi.output_type
-class ContainerdCriPluginConfigurationCni(dict):
-    """
-    containerd cri plugin configuration.
-    """
-    @staticmethod
-    def __key_warning(key: str):
-        suggest = None
-        if key == "binDir":
-            suggest = "bin_dir"
-        elif key == "confDir":
-            suggest = "conf_dir"
-
-        if suggest:
-            pulumi.log.warn(f"Key '{key}' not found in ContainerdCriPluginConfigurationCni. Access the value via the '{suggest}' property getter instead.")
-
-    def __getitem__(self, key: str) -> Any:
-        ContainerdCriPluginConfigurationCni.__key_warning(key)
-        return super().__getitem__(key)
-
-    def get(self, key: str, default = None) -> Any:
-        ContainerdCriPluginConfigurationCni.__key_warning(key)
-        return super().get(key, default)
-
-    def __init__(__self__, *,
-                 bin_dir: Optional[str] = None,
-                 conf_dir: Optional[str] = None):
-        """
-        containerd cri plugin configuration.
-        :param str bin_dir: bin_dir
-        :param str conf_dir: conf_dir
-        """
-        if bin_dir is not None:
-            pulumi.set(__self__, "bin_dir", bin_dir)
-        if conf_dir is not None:
-            pulumi.set(__self__, "conf_dir", conf_dir)
-
-    @property
-    @pulumi.getter(name="binDir")
-    def bin_dir(self) -> Optional[str]:
-        """
-        bin_dir
-        """
-        return pulumi.get(self, "bin_dir")
-
-    @property
-    @pulumi.getter(name="confDir")
-    def conf_dir(self) -> Optional[str]:
-        """
-        conf_dir
-        """
-        return pulumi.get(self, "conf_dir")
-
-
-@pulumi.output_type
-class ContainerdCriPluginConfigurationContainerd(dict):
-    """
-    containerd cri plugin configuration.
-    """
-    @staticmethod
-    def __key_warning(key: str):
-        suggest = None
-        if key == "defaultRuntimeName":
-            suggest = "default_runtime_name"
-
-        if suggest:
-            pulumi.log.warn(f"Key '{key}' not found in ContainerdCriPluginConfigurationContainerd. Access the value via the '{suggest}' property getter instead.")
-
-    def __getitem__(self, key: str) -> Any:
-        ContainerdCriPluginConfigurationContainerd.__key_warning(key)
-        return super().__getitem__(key)
-
-    def get(self, key: str, default = None) -> Any:
-        ContainerdCriPluginConfigurationContainerd.__key_warning(key)
-        return super().get(key, default)
-
-    def __init__(__self__, *,
-                 default_runtime_name: Optional[str] = None,
-                 runtimes: Optional['outputs.ContainerdCriPluginConfigurationContainerdRunc'] = None,
-                 snapshotter: Optional[str] = None):
-        """
-        containerd cri plugin configuration.
-        :param str default_runtime_name: default_runtime_name
-        :param 'ContainerdCriPluginConfigurationContainerdRunc' runtimes: The containerd runtime configuration.
-        :param str snapshotter: snapshotter
-        """
-        if default_runtime_name is not None:
-            pulumi.set(__self__, "default_runtime_name", default_runtime_name)
-        if runtimes is not None:
-            pulumi.set(__self__, "runtimes", runtimes)
-        if snapshotter is not None:
-            pulumi.set(__self__, "snapshotter", snapshotter)
-
-    @property
-    @pulumi.getter(name="defaultRuntimeName")
-    def default_runtime_name(self) -> Optional[str]:
-        """
-        default_runtime_name
-        """
-        return pulumi.get(self, "default_runtime_name")
-
-    @property
-    @pulumi.getter
-    def runtimes(self) -> Optional['outputs.ContainerdCriPluginConfigurationContainerdRunc']:
-        """
-        The containerd runtime configuration.
-        """
-        return pulumi.get(self, "runtimes")
-
-    @property
-    @pulumi.getter
-    def snapshotter(self) -> Optional[str]:
-        """
-        snapshotter
-        """
-        return pulumi.get(self, "snapshotter")
-
-
-@pulumi.output_type
-class ContainerdCriPluginConfigurationContainerdRunc(dict):
-    """
-    containerd cri runc plugin configuration.
-    """
-    @staticmethod
-    def __key_warning(key: str):
-        suggest = None
-        if key == "runtimeType":
-            suggest = "runtime_type"
-
-        if suggest:
-            pulumi.log.warn(f"Key '{key}' not found in ContainerdCriPluginConfigurationContainerdRunc. Access the value via the '{suggest}' property getter instead.")
-
-    def __getitem__(self, key: str) -> Any:
-        ContainerdCriPluginConfigurationContainerdRunc.__key_warning(key)
-        return super().__getitem__(key)
-
-    def get(self, key: str, default = None) -> Any:
-        ContainerdCriPluginConfigurationContainerdRunc.__key_warning(key)
-        return super().get(key, default)
-
-    def __init__(__self__, *,
-                 options: 'outputs.ContainerdCriPluginConfigurationContainerdRuncOptions',
-                 runtime_type: Optional[str] = None):
-        """
-        containerd cri runc plugin configuration.
-        :param 'ContainerdCriPluginConfigurationContainerdRuncOptions' options: runc options.
-        :param str runtime_type: runtime_type
-        """
-        pulumi.set(__self__, "options", options)
-        if runtime_type is not None:
-            pulumi.set(__self__, "runtime_type", runtime_type)
-
-    @property
-    @pulumi.getter
-    def options(self) -> 'outputs.ContainerdCriPluginConfigurationContainerdRuncOptions':
-        """
-        runc options.
-        """
-        return pulumi.get(self, "options")
-
-    @property
-    @pulumi.getter(name="runtimeType")
-    def runtime_type(self) -> Optional[str]:
-        """
-        runtime_type
-        """
-        return pulumi.get(self, "runtime_type")
-
-
-@pulumi.output_type
-class ContainerdCriPluginConfigurationContainerdRuncOptions(dict):
-    """
-    containerd cri runc plugin configuration.
-    """
-    @staticmethod
-    def __key_warning(key: str):
-        suggest = None
-        if key == "systemdCgroup":
-            suggest = "systemd_cgroup"
-
-        if suggest:
-            pulumi.log.warn(f"Key '{key}' not found in ContainerdCriPluginConfigurationContainerdRuncOptions. Access the value via the '{suggest}' property getter instead.")
-
-    def __getitem__(self, key: str) -> Any:
-        ContainerdCriPluginConfigurationContainerdRuncOptions.__key_warning(key)
-        return super().__getitem__(key)
-
-    def get(self, key: str, default = None) -> Any:
-        ContainerdCriPluginConfigurationContainerdRuncOptions.__key_warning(key)
-        return super().get(key, default)
-
-    def __init__(__self__, *,
-                 systemd_cgroup: Optional[bool] = None):
-        """
-        containerd cri runc plugin configuration.
-        :param bool systemd_cgroup: SystemdCgroup
-        """
-        if systemd_cgroup is not None:
-            pulumi.set(__self__, "systemd_cgroup", systemd_cgroup)
-
-    @property
-    @pulumi.getter(name="systemdCgroup")
-    def systemd_cgroup(self) -> Optional[bool]:
-        """
-        SystemdCgroup
-        """
-        return pulumi.get(self, "systemd_cgroup")
-
-
-@pulumi.output_type
 class EtcdConfigurationProps(dict):
     """
     Props for resources that consume etcd configuration.
     """
     @staticmethod
     def __key_warning(key: str):
         suggest = None
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/remote/provision_etcd.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/remote/systemd_service.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,342 +4,260 @@
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
-from .. import tls as _tls
+from . import outputs
 from ._enums import *
-from .etcd_configuration import EtcdConfiguration
-from .etcd_install import EtcdInstall
-from .start_etcd import StartEtcd
-from .systemd_service import SystemdService
+from ._inputs import *
+from .file import File
 import pulumi_command
 
-__all__ = ['ProvisionEtcdArgs', 'ProvisionEtcd']
+__all__ = ['SystemdServiceArgs', 'SystemdService']
 
 @pulumi.input_type
-class ProvisionEtcdArgs:
+class SystemdServiceArgs:
     def __init__(__self__, *,
-                 bundle: pulumi.Input['_tls.BundleArgs'],
                  connection: pulumi.Input['pulumi_command.remote.ConnectionArgs'],
-                 internal_ip: pulumi.Input[str],
-                 architecture: Optional[pulumi.Input['Architecture']] = None,
-                 binary_directory: Optional[pulumi.Input[str]] = None,
-                 configuration_directory: Optional[pulumi.Input[str]] = None,
-                 data_directory: Optional[pulumi.Input[str]] = None,
-                 version: Optional[pulumi.Input[str]] = None):
+                 service: pulumi.Input['SystemdServiceSectionArgs'],
+                 directory: Optional[pulumi.Input[str]] = None,
+                 install: Optional[pulumi.Input['SystemdInstallSectionArgs']] = None,
+                 unit: Optional[pulumi.Input['SystemdUnitSectionArgs']] = None,
+                 unit_name: Optional[pulumi.Input[str]] = None):
         """
-        The set of arguments for constructing a ProvisionEtcd resource.
-        :param pulumi.Input['_tls.BundleArgs'] bundle: The TLS bundle.
+        The set of arguments for constructing a SystemdService resource.
         :param pulumi.Input['pulumi_command.remote.ConnectionArgs'] connection: The parameters with which to connect to the remote host.
-        :param pulumi.Input[str] internal_ip: The internal IP of the etcd node
-        :param pulumi.Input['Architecture'] architecture: TODO
-        :param pulumi.Input[str] binary_directory: TODO
-        :param pulumi.Input[str] configuration_directory: The directory to use for etcd configuration.
-        :param pulumi.Input[str] data_directory: The directory to use for etcd data.
-        :param pulumi.Input[str] version: The version to install.
+        :param pulumi.Input['SystemdServiceSectionArgs'] service: Describes the [Service] section of a systemd service file.
+        :param pulumi.Input[str] directory: The location to create the service file.
+        :param pulumi.Input['SystemdInstallSectionArgs'] install: Describes the [Install] section of a systemd service file.
+        :param pulumi.Input['SystemdUnitSectionArgs'] unit: Describes the [Unit] section of a systemd service file.
+        :param pulumi.Input[str] unit_name: Name of the systemd unit.
         """
-        pulumi.set(__self__, "bundle", bundle)
         pulumi.set(__self__, "connection", connection)
-        pulumi.set(__self__, "internal_ip", internal_ip)
-        if architecture is not None:
-            pulumi.set(__self__, "architecture", architecture)
-        if binary_directory is not None:
-            pulumi.set(__self__, "binary_directory", binary_directory)
-        if configuration_directory is not None:
-            pulumi.set(__self__, "configuration_directory", configuration_directory)
-        if data_directory is not None:
-            pulumi.set(__self__, "data_directory", data_directory)
-        if version is not None:
-            pulumi.set(__self__, "version", version)
-
-    @property
-    @pulumi.getter
-    def bundle(self) -> pulumi.Input['_tls.BundleArgs']:
-        """
-        The TLS bundle.
-        """
-        return pulumi.get(self, "bundle")
-
-    @bundle.setter
-    def bundle(self, value: pulumi.Input['_tls.BundleArgs']):
-        pulumi.set(self, "bundle", value)
+        pulumi.set(__self__, "service", service)
+        if directory is None:
+            directory = '/etc/systemd/system'
+        if directory is not None:
+            pulumi.set(__self__, "directory", directory)
+        if install is not None:
+            pulumi.set(__self__, "install", install)
+        if unit is not None:
+            pulumi.set(__self__, "unit", unit)
+        if unit_name is not None:
+            pulumi.set(__self__, "unit_name", unit_name)
 
     @property
     @pulumi.getter
     def connection(self) -> pulumi.Input['pulumi_command.remote.ConnectionArgs']:
         """
         The parameters with which to connect to the remote host.
         """
         return pulumi.get(self, "connection")
 
     @connection.setter
     def connection(self, value: pulumi.Input['pulumi_command.remote.ConnectionArgs']):
         pulumi.set(self, "connection", value)
 
     @property
-    @pulumi.getter(name="internalIp")
-    def internal_ip(self) -> pulumi.Input[str]:
-        """
-        The internal IP of the etcd node
-        """
-        return pulumi.get(self, "internal_ip")
-
-    @internal_ip.setter
-    def internal_ip(self, value: pulumi.Input[str]):
-        pulumi.set(self, "internal_ip", value)
-
-    @property
     @pulumi.getter
-    def architecture(self) -> Optional[pulumi.Input['Architecture']]:
+    def service(self) -> pulumi.Input['SystemdServiceSectionArgs']:
         """
-        TODO
+        Describes the [Service] section of a systemd service file.
         """
-        return pulumi.get(self, "architecture")
+        return pulumi.get(self, "service")
 
-    @architecture.setter
-    def architecture(self, value: Optional[pulumi.Input['Architecture']]):
-        pulumi.set(self, "architecture", value)
+    @service.setter
+    def service(self, value: pulumi.Input['SystemdServiceSectionArgs']):
+        pulumi.set(self, "service", value)
 
     @property
-    @pulumi.getter(name="binaryDirectory")
-    def binary_directory(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter
+    def directory(self) -> Optional[pulumi.Input[str]]:
         """
-        TODO
+        The location to create the service file.
         """
-        return pulumi.get(self, "binary_directory")
+        return pulumi.get(self, "directory")
 
-    @binary_directory.setter
-    def binary_directory(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "binary_directory", value)
+    @directory.setter
+    def directory(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "directory", value)
 
     @property
-    @pulumi.getter(name="configurationDirectory")
-    def configuration_directory(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter
+    def install(self) -> Optional[pulumi.Input['SystemdInstallSectionArgs']]:
         """
-        The directory to use for etcd configuration.
+        Describes the [Install] section of a systemd service file.
         """
-        return pulumi.get(self, "configuration_directory")
+        return pulumi.get(self, "install")
 
-    @configuration_directory.setter
-    def configuration_directory(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "configuration_directory", value)
+    @install.setter
+    def install(self, value: Optional[pulumi.Input['SystemdInstallSectionArgs']]):
+        pulumi.set(self, "install", value)
 
     @property
-    @pulumi.getter(name="dataDirectory")
-    def data_directory(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter
+    def unit(self) -> Optional[pulumi.Input['SystemdUnitSectionArgs']]:
         """
-        The directory to use for etcd data.
+        Describes the [Unit] section of a systemd service file.
         """
-        return pulumi.get(self, "data_directory")
+        return pulumi.get(self, "unit")
 
-    @data_directory.setter
-    def data_directory(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "data_directory", value)
+    @unit.setter
+    def unit(self, value: Optional[pulumi.Input['SystemdUnitSectionArgs']]):
+        pulumi.set(self, "unit", value)
 
     @property
-    @pulumi.getter
-    def version(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="unitName")
+    def unit_name(self) -> Optional[pulumi.Input[str]]:
         """
-        The version to install.
+        Name of the systemd unit.
         """
-        return pulumi.get(self, "version")
+        return pulumi.get(self, "unit_name")
 
-    @version.setter
-    def version(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "version", value)
+    @unit_name.setter
+    def unit_name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "unit_name", value)
 
 
-class ProvisionEtcd(pulumi.ComponentResource):
+class SystemdService(pulumi.ComponentResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 architecture: Optional[pulumi.Input['Architecture']] = None,
-                 binary_directory: Optional[pulumi.Input[str]] = None,
-                 bundle: Optional[pulumi.Input[pulumi.InputType['_tls.BundleArgs']]] = None,
-                 configuration_directory: Optional[pulumi.Input[str]] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
-                 data_directory: Optional[pulumi.Input[str]] = None,
-                 internal_ip: Optional[pulumi.Input[str]] = None,
-                 version: Optional[pulumi.Input[str]] = None,
+                 directory: Optional[pulumi.Input[str]] = None,
+                 install: Optional[pulumi.Input[pulumi.InputType['SystemdInstallSectionArgs']]] = None,
+                 service: Optional[pulumi.Input[pulumi.InputType['SystemdServiceSectionArgs']]] = None,
+                 unit: Optional[pulumi.Input[pulumi.InputType['SystemdUnitSectionArgs']]] = None,
+                 unit_name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        Starts etcd on a remote system.
+        A systemd service on a remote system.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input['Architecture'] architecture: TODO
-        :param pulumi.Input[str] binary_directory: TODO
-        :param pulumi.Input[pulumi.InputType['_tls.BundleArgs']] bundle: The TLS bundle.
-        :param pulumi.Input[str] configuration_directory: The directory to use for etcd configuration.
         :param pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']] connection: The parameters with which to connect to the remote host.
-        :param pulumi.Input[str] data_directory: The directory to use for etcd data.
-        :param pulumi.Input[str] internal_ip: The internal IP of the etcd node
-        :param pulumi.Input[str] version: The version to install.
+        :param pulumi.Input[str] directory: The location to create the service file.
+        :param pulumi.Input[pulumi.InputType['SystemdInstallSectionArgs']] install: Describes the [Install] section of a systemd service file.
+        :param pulumi.Input[pulumi.InputType['SystemdServiceSectionArgs']] service: Describes the [Service] section of a systemd service file.
+        :param pulumi.Input[pulumi.InputType['SystemdUnitSectionArgs']] unit: Describes the [Unit] section of a systemd service file.
+        :param pulumi.Input[str] unit_name: Name of the systemd unit.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: ProvisionEtcdArgs,
+                 args: SystemdServiceArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Starts etcd on a remote system.
+        A systemd service on a remote system.
 
         :param str resource_name: The name of the resource.
-        :param ProvisionEtcdArgs args: The arguments to use to populate this resource's properties.
+        :param SystemdServiceArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(ProvisionEtcdArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(SystemdServiceArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 architecture: Optional[pulumi.Input['Architecture']] = None,
-                 binary_directory: Optional[pulumi.Input[str]] = None,
-                 bundle: Optional[pulumi.Input[pulumi.InputType['_tls.BundleArgs']]] = None,
-                 configuration_directory: Optional[pulumi.Input[str]] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
-                 data_directory: Optional[pulumi.Input[str]] = None,
-                 internal_ip: Optional[pulumi.Input[str]] = None,
-                 version: Optional[pulumi.Input[str]] = None,
+                 directory: Optional[pulumi.Input[str]] = None,
+                 install: Optional[pulumi.Input[pulumi.InputType['SystemdInstallSectionArgs']]] = None,
+                 service: Optional[pulumi.Input[pulumi.InputType['SystemdServiceSectionArgs']]] = None,
+                 unit: Optional[pulumi.Input[pulumi.InputType['SystemdUnitSectionArgs']]] = None,
+                 unit_name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is not None:
             raise ValueError('ComponentResource classes do not support opts.id')
         else:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = ProvisionEtcdArgs.__new__(ProvisionEtcdArgs)
+            __props__ = SystemdServiceArgs.__new__(SystemdServiceArgs)
 
-            __props__.__dict__["architecture"] = architecture
-            __props__.__dict__["binary_directory"] = binary_directory
-            if bundle is None and not opts.urn:
-                raise TypeError("Missing required property 'bundle'")
-            __props__.__dict__["bundle"] = bundle
-            __props__.__dict__["configuration_directory"] = configuration_directory
             if connection is None and not opts.urn:
                 raise TypeError("Missing required property 'connection'")
             __props__.__dict__["connection"] = connection
-            __props__.__dict__["data_directory"] = data_directory
-            if internal_ip is None and not opts.urn:
-                raise TypeError("Missing required property 'internal_ip'")
-            __props__.__dict__["internal_ip"] = internal_ip
-            __props__.__dict__["version"] = version
-            __props__.__dict__["configuration"] = None
-            __props__.__dict__["install"] = None
-            __props__.__dict__["service"] = None
-            __props__.__dict__["start"] = None
-        super(ProvisionEtcd, __self__).__init__(
-            'kubernetes-the-hard-way:remote:ProvisionEtcd',
+            if directory is None:
+                directory = '/etc/systemd/system'
+            __props__.__dict__["directory"] = directory
+            __props__.__dict__["install"] = install
+            if service is None and not opts.urn:
+                raise TypeError("Missing required property 'service'")
+            __props__.__dict__["service"] = service
+            __props__.__dict__["unit"] = unit
+            __props__.__dict__["unit_name"] = unit_name
+            __props__.__dict__["file"] = None
+        super(SystemdService, __self__).__init__(
+            'kubernetes-the-hard-way:remote:SystemdService',
             resource_name,
             __props__,
             opts,
             remote=True)
 
     @property
     @pulumi.getter
-    def architecture(self) -> pulumi.Output[Optional['Architecture']]:
-        """
-        TODO
-        """
-        return pulumi.get(self, "architecture")
-
-    @property
-    @pulumi.getter(name="binaryDirectory")
-    def binary_directory(self) -> pulumi.Output[Optional[str]]:
-        """
-        TODO
-        """
-        return pulumi.get(self, "binary_directory")
-
-    @property
-    @pulumi.getter
-    def bundle(self) -> pulumi.Output['_tls.outputs.Bundle']:
-        """
-        The TLS bundle.
-        """
-        return pulumi.get(self, "bundle")
-
-    @property
-    @pulumi.getter
-    def configuration(self) -> pulumi.Output['EtcdConfiguration']:
-        """
-        Etcd configuration.
-        """
-        return pulumi.get(self, "configuration")
-
-    @property
-    @pulumi.getter(name="configurationDirectory")
-    def configuration_directory(self) -> pulumi.Output[Optional[str]]:
-        """
-        The directory to use for etcd configuration.
-        """
-        return pulumi.get(self, "configuration_directory")
-
-    @property
-    @pulumi.getter
     def connection(self) -> pulumi.Output['pulumi_command.remote.outputs.Connection']:
         """
         The parameters with which to connect to the remote host.
         """
         return pulumi.get(self, "connection")
 
     @property
-    @pulumi.getter(name="dataDirectory")
-    def data_directory(self) -> pulumi.Output[Optional[str]]:
+    @pulumi.getter
+    def directory(self) -> pulumi.Output[str]:
         """
-        The directory to use for etcd data.
+        The location to create the service file.
         """
-        return pulumi.get(self, "data_directory")
+        return pulumi.get(self, "directory")
 
     @property
     @pulumi.getter
-    def install(self) -> pulumi.Output['EtcdInstall']:
+    def file(self) -> pulumi.Output['File']:
         """
-        Install etcd.
+        The service file on the remote machine.
         """
-        return pulumi.get(self, "install")
+        return pulumi.get(self, "file")
 
     @property
-    @pulumi.getter(name="internalIp")
-    def internal_ip(self) -> pulumi.Output[str]:
+    @pulumi.getter
+    def install(self) -> pulumi.Output[Optional['outputs.SystemdInstallSection']]:
         """
-        The internal IP of the etcd node
+        Describes the [Install] section of a systemd service file.
         """
-        return pulumi.get(self, "internal_ip")
+        return pulumi.get(self, "install")
 
     @property
     @pulumi.getter
-    def service(self) -> pulumi.Output['SystemdService']:
+    def service(self) -> pulumi.Output['outputs.SystemdServiceSection']:
         """
-        Systemd service.
+        Describes the [Service] section of a systemd service file.
         """
         return pulumi.get(self, "service")
 
     @property
     @pulumi.getter
-    def start(self) -> pulumi.Output['StartEtcd']:
+    def unit(self) -> pulumi.Output[Optional['outputs.SystemdUnitSection']]:
         """
-        Start etcd
+        Describes the [Unit] section of a systemd service file.
         """
-        return pulumi.get(self, "start")
+        return pulumi.get(self, "unit")
 
     @property
-    @pulumi.getter
-    def version(self) -> pulumi.Output[Optional[str]]:
+    @pulumi.getter(name="unitName")
+    def unit_name(self) -> pulumi.Output[Optional[str]]:
         """
-        The version to install.
+        Name of the systemd unit.
         """
-        return pulumi.get(self, "version")
+        return pulumi.get(self, "unit_name")
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/remote/runc_install.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/remote/runc_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/remote/start_containerd.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/remote/start_containerd.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/remote/start_etcd.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/remote/start_kubelet.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,22 +7,22 @@
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from .. import tools as _tools
 import pulumi_command
 
-__all__ = ['StartEtcdArgs', 'StartEtcd']
+__all__ = ['StartKubeletArgs', 'StartKubelet']
 
 @pulumi.input_type
-class StartEtcdArgs:
+class StartKubeletArgs:
     def __init__(__self__, *,
                  connection: pulumi.Input['pulumi_command.remote.ConnectionArgs']):
         """
-        The set of arguments for constructing a StartEtcd resource.
+        The set of arguments for constructing a StartKubelet resource.
         :param pulumi.Input['pulumi_command.remote.ConnectionArgs'] connection: The parameters with which to connect to the remote host.
         """
         pulumi.set(__self__, "connection", connection)
 
     @property
     @pulumi.getter
     def connection(self) -> pulumi.Input['pulumi_command.remote.ConnectionArgs']:
@@ -32,44 +32,44 @@
         return pulumi.get(self, "connection")
 
     @connection.setter
     def connection(self, value: pulumi.Input['pulumi_command.remote.ConnectionArgs']):
         pulumi.set(self, "connection", value)
 
 
-class StartEtcd(pulumi.ComponentResource):
+class StartKubelet(pulumi.ComponentResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
                  __props__=None):
         """
-        Starts `etcd` on a remote system
+        Starts `kubelet` on a remote system
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']] connection: The parameters with which to connect to the remote host.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: StartEtcdArgs,
+                 args: StartKubeletArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Starts `etcd` on a remote system
+        Starts `kubelet` on a remote system
 
         :param str resource_name: The name of the resource.
-        :param StartEtcdArgs args: The arguments to use to populate this resource's properties.
+        :param StartKubeletArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(StartEtcdArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(StartKubeletArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
@@ -80,24 +80,24 @@
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is not None:
             raise ValueError('ComponentResource classes do not support opts.id')
         else:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = StartEtcdArgs.__new__(StartEtcdArgs)
+            __props__ = StartKubeletArgs.__new__(StartKubeletArgs)
 
             if connection is None and not opts.urn:
                 raise TypeError("Missing required property 'connection'")
             __props__.__dict__["connection"] = connection
             __props__.__dict__["daemon_reload"] = None
             __props__.__dict__["enable"] = None
             __props__.__dict__["start"] = None
-        super(StartEtcd, __self__).__init__(
-            'kubernetes-the-hard-way:remote:StartEtcd',
+        super(StartKubelet, __self__).__init__(
+            'kubernetes-the-hard-way:remote:StartKubelet',
             resource_name,
             __props__,
             opts,
             remote=True)
 
     @property
     @pulumi.getter
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/tls/_enums.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/tls/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/tls/_inputs.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/tls/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/tls/certificate.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/tls/certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/tls/encryption_key.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/tls/encryption_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/tls/outputs.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/tls/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/tls/root_ca.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/tls/root_ca.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/tools/__init__.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/tools/_enums.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/tools/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/tools/_inputs.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/tools/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/tools/chmod.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/tools/chmod.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/tools/etcdctl.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/tools/etcdctl.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/tools/hostnamectl.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/tools/hostnamectl.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/tools/mkdir.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/tools/mkdir.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/tools/mktemp.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/tools/mktemp.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/tools/mv.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/tools/mv.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/tools/outputs.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/tools/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/tools/rm.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/tools/rm.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/tools/sed.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/tools/sed.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/tools/systemctl.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/tools/systemctl.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/tools/tar.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/tools/tar.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/tools/tee.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/tools/tee.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way/tools/wget.py` & `pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way/tools/wget.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO` & `pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_kubernetes_the_hard_way
-Version: 0.0.26a1716235251
+Version: 0.0.26a1716346744
 Summary: A Pulumi implementation of Kelsey Hightower's Kubernetes the Hard Way
 License: Apache-2.0
 Project-URL: Repository, https://github.com/UnstoppableMango/pulumi-kubernetes-the-hard-way
 Keywords: pulumi,command,tls,kubernetes,category/utility,kind/component
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: parver>=0.2.1
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt` & `pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -9,30 +9,32 @@
 pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt
 pulumi_kubernetes_the_hard_way.egg-info/dependency_links.txt
 pulumi_kubernetes_the_hard_way.egg-info/requires.txt
 pulumi_kubernetes_the_hard_way.egg-info/top_level.txt
 pulumi_kubernetes_the_hard_way/config/__init__.py
 pulumi_kubernetes_the_hard_way/config/_enums.py
 pulumi_kubernetes_the_hard_way/config/_inputs.py
+pulumi_kubernetes_the_hard_way/config/cni_bridge_plugin_configuration.py
+pulumi_kubernetes_the_hard_way/config/cni_loopback_plugin_configuration.py
+pulumi_kubernetes_the_hard_way/config/containerd_configuration.py
+pulumi_kubernetes_the_hard_way/config/get_cni_bridge_plugin_configuration.py
+pulumi_kubernetes_the_hard_way/config/get_cni_loopback_plugin_configuration.py
+pulumi_kubernetes_the_hard_way/config/get_containerd_configuration.py
 pulumi_kubernetes_the_hard_way/config/get_kube_proxy_configuration.py
 pulumi_kubernetes_the_hard_way/config/get_kube_vip_manifest.py
 pulumi_kubernetes_the_hard_way/config/get_kubeconfig.py
 pulumi_kubernetes_the_hard_way/config/get_kubelet_configuration.py
 pulumi_kubernetes_the_hard_way/config/kube_proxy_configuration.py
 pulumi_kubernetes_the_hard_way/config/kube_vip_manifest.py
 pulumi_kubernetes_the_hard_way/config/kubelet_configuration.py
 pulumi_kubernetes_the_hard_way/config/outputs.py
 pulumi_kubernetes_the_hard_way/remote/__init__.py
 pulumi_kubernetes_the_hard_way/remote/_enums.py
 pulumi_kubernetes_the_hard_way/remote/_inputs.py
-pulumi_kubernetes_the_hard_way/remote/cni_bridge_plugin_configuration.py
-pulumi_kubernetes_the_hard_way/remote/cni_loopback_plugin_configuration.py
-pulumi_kubernetes_the_hard_way/remote/cni_plugin_configuration.py
 pulumi_kubernetes_the_hard_way/remote/cni_plugins_install.py
-pulumi_kubernetes_the_hard_way/remote/containerd_configuration.py
 pulumi_kubernetes_the_hard_way/remote/containerd_install.py
 pulumi_kubernetes_the_hard_way/remote/crictl_install.py
 pulumi_kubernetes_the_hard_way/remote/download.py
 pulumi_kubernetes_the_hard_way/remote/etcd_cluster.py
 pulumi_kubernetes_the_hard_way/remote/etcd_configuration.py
 pulumi_kubernetes_the_hard_way/remote/etcd_install.py
 pulumi_kubernetes_the_hard_way/remote/etcd_service.py
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.26a1716235251/pyproject.toml` & `pulumi_kubernetes_the_hard_way-0.0.26a1716346744/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_kubernetes_the_hard_way"
   description = "A Pulumi implementation of Kelsey Hightower's Kubernetes the Hard Way"
   dependencies = ["parver>=0.2.1", "pulumi>=3.91.1,<4.0.0", "pulumi-command>=0.11.1,<1.0.0", "pulumi-kubernetes>=4.11.0,<5.0.0", "pulumi-random>=4.16.1,<5.0.0", "pulumi-tls>=5.0.2,<6.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "command", "tls", "kubernetes", "category/utility", "kind/component"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "0.0.26a1716235251"
+  version = "0.0.26a1716346744"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Repository = "https://github.com/UnstoppableMango/pulumi-kubernetes-the-hard-way"
 
 [build-system]
   requires = ["setuptools>=61.0"]
```

