# Comparing `tmp/hotsos-1.18.post3.tar.gz` & `tmp/hotsos-1.18.post4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hotsos-1.18.post3.tar", last modified: Wed May 22 10:59:02 2024, max compression
+gzip compressed data, was "hotsos-1.18.post4.tar", last modified: Wed May 22 12:18:06 2024, max compression
```

## Comparing `hotsos-1.18.post3.tar` & `hotsos-1.18.post4.tar`

### file list

```diff
@@ -1,441 +1,441 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.763236 hotsos-1.18.post3/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-22 10:58:49.000000 hotsos-1.18.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-22 10:58:49.000000 hotsos-1.18.post3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-05-22 10:59:02.763236 hotsos-1.18.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-22 10:58:49.000000 hotsos-1.18.post3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.711236 hotsos-1.18.post3/hotsos/
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-22 10:58:55.000000 hotsos-1.18.post3/hotsos/.repo-info
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    15279 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/cli.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9421 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.711236 hotsos-1.18.post3/hotsos/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10725 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/analytics.py
--rw-r--r--   0 runner    (1001) docker     (127)     9584 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/config.py
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.715236 hotsos-1.18.post3/hotsos/core/host_helpers/
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/host_helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/host_helpers/apparmor.py
--rw-r--r--   0 runner    (1001) docker     (127)    42176 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/host_helpers/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/host_helpers/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     4665 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/host_helpers/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/host_helpers/filestat.py
--rw-r--r--   0 runner    (1001) docker     (127)    13279 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/host_helpers/network.py
--rw-r--r--   0 runner    (1001) docker     (127)    14487 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/host_helpers/packaging.py
--rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/host_helpers/pebble.py
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/host_helpers/ssl.py
--rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/host_helpers/sysctl.py
--rw-r--r--   0 runner    (1001) docker     (127)    15568 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/host_helpers/systemd.py
--rw-r--r--   0 runner    (1001) docker     (127)     3303 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/host_helpers/uptime.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.715236 hotsos-1.18.post3/hotsos/core/issues/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/issues/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/issues/issue_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     5375 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/issues/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/log.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.715236 hotsos-1.18.post3/hotsos/core/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.715236 hotsos-1.18.post3/hotsos/core/plugins/juju/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/plugins/juju/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/plugins/juju/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     8187 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/plugins/juju/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.719236 hotsos-1.18.post3/hotsos/core/plugins/kernel/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/plugins/kernel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/plugins/kernel/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/plugins/kernel/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.719236 hotsos-1.18.post3/hotsos/core/plugins/kernel/kernlog/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/plugins/kernel/kernlog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14673 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/plugins/kernel/kernlog/calltrace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/plugins/kernel/kernlog/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/plugins/kernel/kernlog/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     9200 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/plugins/kernel/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)    20751 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/plugins/kernel/net.py
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/plugins/kernel/sysfs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/plugins/kubernetes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.719236 hotsos-1.18.post3/hotsos/core/plugins/lxd/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/plugins/lxd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/plugins/lxd/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/plugins/maas.py
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/plugins/mysql.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.719236 hotsos-1.18.post3/hotsos/core/plugins/openstack/
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/plugins/openstack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8811 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/plugins/openstack/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    63860 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/plugins/openstack/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3979 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/plugins/openstack/neutron.py
--rw-r--r--   0 runner    (1001) docker     (127)    11108 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/plugins/openstack/nova.py
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/plugins/openstack/octavia.py
--rw-r--r--   0 runner    (1001) docker     (127)    20116 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/plugins/openstack/openstack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.719236 hotsos-1.18.post3/hotsos/core/plugins/openvswitch/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/plugins/openvswitch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/plugins/openvswitch/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     4830 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/plugins/openvswitch/ovn.py
--rw-r--r--   0 runner    (1001) docker     (127)     7055 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/plugins/openvswitch/ovs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/plugins/pacemaker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.719236 hotsos-1.18.post3/hotsos/core/plugins/rabbitmq/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/plugins/rabbitmq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/plugins/rabbitmq/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     8826 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/plugins/rabbitmq/report.py
--rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/plugins/sosreport.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.723236 hotsos-1.18.post3/hotsos/core/plugins/storage/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/plugins/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7927 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/plugins/storage/bcache.py
--rw-r--r--   0 runner    (1001) docker     (127)    38954 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/plugins/storage/ceph.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.723236 hotsos-1.18.post3/hotsos/core/plugins/system/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/plugins/system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/plugins/system/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     7081 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/plugins/system/system.py
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/plugins/vault.py
--rw-r--r--   0 runner    (1001) docker     (127)    15227 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/plugintools.py
--rw-r--r--   0 runner    (1001) docker     (127)     4038 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/root_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.723236 hotsos-1.18.post3/hotsos/core/ycheck/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/ycheck/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.723236 hotsos-1.18.post3/hotsos/core/ycheck/engine/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/ycheck/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/ycheck/engine/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.723236 hotsos-1.18.post3/hotsos/core/ycheck/engine/properties/
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/ycheck/engine/properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8767 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/ycheck/engine/properties/checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    17125 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/ycheck/engine/properties/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     8427 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/ycheck/engine/properties/conclusions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/ycheck/engine/properties/inputdef.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.723236 hotsos-1.18.post3/hotsos/core/ycheck/engine/properties/requires/
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/ycheck/engine/properties/requires/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7464 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/ycheck/engine/properties/requires/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     4382 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/ycheck/engine/properties/requires/requires.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.727236 hotsos-1.18.post3/hotsos/core/ycheck/engine/properties/requires/types/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/ycheck/engine/properties/requires/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8541 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/ycheck/engine/properties/requires/types/apt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/ycheck/engine/properties/requires/types/binary.py
--rw-r--r--   0 runner    (1001) docker     (127)     7956 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/ycheck/engine/properties/requires/types/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/ycheck/engine/properties/requires/types/path.py
--rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/ycheck/engine/properties/requires/types/pebble.py
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/ycheck/engine/properties/requires/types/property.py
--rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/ycheck/engine/properties/requires/types/snap.py
--rw-r--r--   0 runner    (1001) docker     (127)     5032 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/ycheck/engine/properties/requires/types/systemd.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/ycheck/engine/properties/requires/types/varops.py
--rw-r--r--   0 runner    (1001) docker     (127)    15943 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/ycheck/engine/properties/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/ycheck/engine/properties/vardef.py
--rw-r--r--   0 runner    (1001) docker     (127)    27167 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/ycheck/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     5992 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/core/ycheck/scenarios.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.647237 hotsos-1.18.post3/hotsos/defs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.647237 hotsos-1.18.post3/hotsos/defs/events/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.727236 hotsos-1.18.post3/hotsos/defs/events/openstack/
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/events/openstack/apache.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/events/openstack/apparmor.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/events/openstack/http-requests.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.727236 hotsos-1.18.post3/hotsos/defs/events/openstack/neutron/
--rw-r--r--   0 runner    (1001) docker     (127)     3218 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/events/openstack/neutron/agents.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/events/openstack/neutron/ml2-routers.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.727236 hotsos-1.18.post3/hotsos/defs/events/openstack/nova/
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/events/openstack/nova/external-events.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.727236 hotsos-1.18.post3/hotsos/defs/events/openstack/nova/migrations/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.727236 hotsos-1.18.post3/hotsos/defs/events/openstack/nova/migrations/live-migration/
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/events/openstack/nova/migrations/live-migration/dst-pre-live-migration.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/events/openstack/nova/migrations/live-migration/src-migration.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/events/openstack/nova/migrations/live-migration/src-post-live-migration.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/events/openstack/nova/migrations/migrations.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/events/openstack/nova/nova-compute.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/events/openstack/octavia.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.647237 hotsos-1.18.post3/hotsos/defs/events/openvswitch/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.727236 hotsos-1.18.post3/hotsos/defs/events/openvswitch/ovn/
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/events/openvswitch/ovn/errors-and-warnings.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/events/openvswitch/ovn/ovn-central.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/events/openvswitch/ovn/ovn-controller.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.731236 hotsos-1.18.post3/hotsos/defs/events/openvswitch/ovs/
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/events/openvswitch/ovs/bfd.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/events/openvswitch/ovs/datapath-checks.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/events/openvswitch/ovs/errors-and-warnings.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/events/openvswitch/ovs/ovs-vswitchd.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.647237 hotsos-1.18.post3/hotsos/defs/events/storage/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.647237 hotsos-1.18.post3/hotsos/defs/events/storage/ceph/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.731236 hotsos-1.18.post3/hotsos/defs/events/storage/ceph/mon/
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/events/storage/ceph/mon/mon.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/events/storage/ceph/mon/monlogs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.731236 hotsos-1.18.post3/hotsos/defs/events/storage/ceph/osd/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/events/storage/ceph/osd/osd.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/events/storage/ceph/osd/osdlogs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.707236 hotsos-1.18.post3/hotsos/defs/scenarios/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.731236 hotsos-1.18.post3/hotsos/defs/scenarios/juju/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.731236 hotsos-1.18.post3/hotsos/defs/scenarios/juju/bugs/
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/juju/bugs/lp1812361.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/juju/bugs/lp1852502.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/juju/bugs/lp1858519.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/juju/bugs/lp1895040.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/juju/bugs/lp1910958.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/juju/bugs/lp1948906.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/juju/bugs/lp1983140.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/juju/bugs/lp1983506.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/juju/bugs/lp1996230.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/juju/charm_unit_checks.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/juju/juju.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/juju/juju_binary_cve.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/juju/juju_pebble_cve.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/juju/jujud_machine_checks.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/juju/snap_channel.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.735236 hotsos-1.18.post3/hotsos/defs/scenarios/kernel/
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/kernel/amd_iommu_pt.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/kernel/disk_failure.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/kernel/kernlog_calltrace.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/kernel/memory.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.735236 hotsos-1.18.post3/hotsos/defs/scenarios/kernel/network/
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/kernel/network/misc.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/kernel/network/netlink.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     7335 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/kernel/network/tcp.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3580 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/kernel/network/udp.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/kernel/qla2xxx.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.735236 hotsos-1.18.post3/hotsos/defs/scenarios/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/kubernetes/kubernetes.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/kubernetes/system_cpufreq_mode.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.735236 hotsos-1.18.post3/hotsos/defs/scenarios/lxd/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.735236 hotsos-1.18.post3/hotsos/defs/scenarios/lxd/bugs/
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/lxd/bugs/lp1807628.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/lxd/lxcfs_deadlock.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/lxd/snap_channel.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.735236 hotsos-1.18.post3/hotsos/defs/scenarios/maas/
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/maas/maas_proxy_issue.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.735236 hotsos-1.18.post3/hotsos/defs/scenarios/mysql/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.735236 hotsos-1.18.post3/hotsos/defs/scenarios/mysql/bugs/
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/mysql/bugs/lp1959861.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/mysql/bugs/lp1971565.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/mysql/bugs/lp2039444.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/mysql/bugs/lp372017.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/mysql/mysql.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/mysql/mysql_connections.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.739236 hotsos-1.18.post3/hotsos/defs/scenarios/openstack/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.651237 hotsos-1.18.post3/hotsos/defs/scenarios/openstack/barbican/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.739236 hotsos-1.18.post3/hotsos/defs/scenarios/openstack/barbican/bugs/
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/openstack/barbican/bugs/lp1946787.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.651237 hotsos-1.18.post3/hotsos/defs/scenarios/openstack/cinder/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.739236 hotsos-1.18.post3/hotsos/defs/scenarios/openstack/cinder/bugs/
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/openstack/cinder/bugs/lp2004555.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/openstack/eol.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.651237 hotsos-1.18.post3/hotsos/defs/scenarios/openstack/keystone/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.739236 hotsos-1.18.post3/hotsos/defs/scenarios/openstack/keystone/bugs/
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/openstack/keystone/bugs/lp1896125.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.739236 hotsos-1.18.post3/hotsos/defs/scenarios/openstack/masakari/
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/openstack/masakari/pacemaker_remote.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.739236 hotsos-1.18.post3/hotsos/defs/scenarios/openstack/neutron/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.739236 hotsos-1.18.post3/hotsos/defs/scenarios/openstack/neutron/bugs/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/openstack/neutron/bugs/lp1794991.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/openstack/neutron/bugs/lp1883089.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/openstack/neutron/bugs/lp1896506.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/openstack/neutron/bugs/lp1907686.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/openstack/neutron/bugs/lp1927868.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/openstack/neutron/bugs/lp1928031.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/openstack/neutron/bugs/lp1929832.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/openstack/neutron/bugs/lp1948466.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/openstack/neutron/bugs/lp1960319.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/openstack/neutron/bugs/lp1965297.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/openstack/neutron/bugs/lp1979089.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/openstack/neutron/bugs/lp1980211.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/openstack/neutron/bugs/lp1993628.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/openstack/neutron/bugs/lp1996594.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/openstack/neutron/neutron_ovs_cleanup.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/openstack/neutron/oslo_privsep_errors.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/openstack/neutron/ovn_stale_db.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/openstack/neutron/ovndb_leader_bouncing.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.743236 hotsos-1.18.post3/hotsos/defs/scenarios/openstack/nova/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.743236 hotsos-1.18.post3/hotsos/defs/scenarios/openstack/nova/bugs/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/openstack/nova/bugs/lp1761062.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/openstack/nova/bugs/lp1860743.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/openstack/nova/bugs/lp1888395.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/openstack/nova/bugs/lp1904580.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/openstack/nova/bugs/lp1944619.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/openstack/nova/bugs/lp1967956.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/openstack/nova/bugs/lp2004555.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/openstack/nova/bugs/lp2012284.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/openstack/nova/config_checks.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6035 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/openstack/nova/cpu_pinning.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/openstack/nova/service_mem_usage.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.743236 hotsos-1.18.post3/hotsos/defs/scenarios/openstack/octavia/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.743236 hotsos-1.18.post3/hotsos/defs/scenarios/openstack/octavia/bugs/
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/openstack/octavia/bugs/lp2029857.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/openstack/octavia/bugs/sb1896125.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/openstack/octavia/excessive_failovers.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/openstack/octavia/hm_port_health.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/openstack/openstack.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/openstack/openstack_apache2_certificates.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/openstack/openstack_charm_conflicts.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.743236 hotsos-1.18.post3/hotsos/defs/scenarios/openstack/openstack_charms/
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/openstack/openstack_charms/nova_cc_ssh_known_hosts_fail.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/openstack/pkgs_from_mixed_releases_found.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/openstack/system_cpufreq_mode.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/openstack/systemd_masked_services.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.743236 hotsos-1.18.post3/hotsos/defs/scenarios/openvswitch/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.743236 hotsos-1.18.post3/hotsos/defs/scenarios/openvswitch/bugs/
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/openvswitch/bugs/lp1839592.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/openvswitch/bugs/lp1978806.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/openvswitch/dpdk_config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/openvswitch/dpif_lost_packets.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/openvswitch/dpif_resubmit_actions.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/openvswitch/openvswitch.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.747236 hotsos-1.18.post3/hotsos/defs/scenarios/openvswitch/ovn/
--rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/openvswitch/ovn/bfd_flapping.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.747236 hotsos-1.18.post3/hotsos/defs/scenarios/openvswitch/ovn/bugs/
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/openvswitch/ovn/bugs/lp1865127.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/openvswitch/ovn/bugs/lp1917475.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/openvswitch/ovn/ovn_central_certs_logs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/openvswitch/ovn/ovn_central_services.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/openvswitch/ovn/ovn_certs_valid.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/openvswitch/ovn/ovn_chassis_certs_logs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/openvswitch/ovn/ovn_elections.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/openvswitch/ovn/ovn_upgrades.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/openvswitch/ovn/service_mem_usage.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/openvswitch/service_restarts.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.747236 hotsos-1.18.post3/hotsos/defs/scenarios/pacemaker/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.747236 hotsos-1.18.post3/hotsos/defs/scenarios/pacemaker/bugs/
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/pacemaker/bugs/lp1874719.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/pacemaker/pacemaker.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.747236 hotsos-1.18.post3/hotsos/defs/scenarios/rabbitmq/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.747236 hotsos-1.18.post3/hotsos/defs/scenarios/rabbitmq/bugs/
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/rabbitmq/bugs/lp1943937.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/rabbitmq/cluster_config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/rabbitmq/cluster_logchecks.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/rabbitmq/cluster_resources.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/rabbitmq/rabbitmq.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.747236 hotsos-1.18.post3/hotsos/defs/scenarios/sosreport/
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/sosreport/plugin_timeouts.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.747236 hotsos-1.18.post3/hotsos/defs/scenarios/storage/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.747236 hotsos-1.18.post3/hotsos/defs/scenarios/storage/bcache/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/storage/bcache/bcache.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/storage/bcache/bdev.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/storage/bcache/cacheset.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.703236 hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.747236 hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-mgr/
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-mgr/autoscaler_overlap_roots.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.751236 hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-mon/
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-mon/auth_insecure_global_id_reclaim_allowed.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-mon/autoscaler_bug.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-mon/bluefs_size.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-mon/bluefs_spillover.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph-mon.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph_address_overlap.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph_cluster_health.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph_versions_mismatch.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-mon/crushmap_bucket_checks.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-mon/empty_clog.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-mon/eol.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-mon/laggy_pgs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-mon/large_omap_objects.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-mon/meta_backend_mon.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-mon/mon_db_too_big.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-mon/mon_elections_flapping.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_flapping.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_maps_backlog_too_large.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_messenger_v2_protocol.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_slow_heartbeats.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_slow_ops.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_unusual_raw.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-mon/pg_imbalance.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-mon/pg_overdose.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-mon/required_osd_release_mismatch.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-mon/rgw_frontend.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-mon/ssds_using_bcache.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-mon/unresponsive_mon_mgr.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.755236 hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-osd/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.755236 hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/
--rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp1936136.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp1959649.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp1996010.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp2013960.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp2016845.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-osd/ceph-osd.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-osd/ceph_address_overlap.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-osd/eol.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-osd/filestore_to_bluestore_upgrade.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-osd/juju_ceph_no_bcache_tuning.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-osd/meta_backend_osd.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-osd/osd_flapping.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-osd/osd_latency.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-osd/osd_slow_ops.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-osd/pg_overdose.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-osd/ssd_osds_no_discard.yaml.disabled
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-osd/system_cpufreq_mode.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.755236 hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-rgw/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.755236 hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-rgw/bugs/
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-rgw/bugs/lp1974138.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-rgw/rgw_frontend_rgw.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.755236 hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/common/
--rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/common/ceph_charm_conflicts.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.755236 hotsos-1.18.post3/hotsos/defs/scenarios/storage/nfs/
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/storage/nfs/nfs-detect-mount-name-resolution-failure.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/storage/storage.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.755236 hotsos-1.18.post3/hotsos/defs/scenarios/system/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/system/system.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/system/unattended_upgrades.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.755236 hotsos-1.18.post3/hotsos/defs/scenarios/vault/
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/defs/scenarios/vault/snap_channel.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.755236 hotsos-1.18.post3/hotsos/plugin_extensions/
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/plugin_extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.759236 hotsos-1.18.post3/hotsos/plugin_extensions/juju/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/plugin_extensions/juju/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/plugin_extensions/juju/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.759236 hotsos-1.18.post3/hotsos/plugin_extensions/kernel/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/plugin_extensions/kernel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/plugin_extensions/kernel/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.759236 hotsos-1.18.post3/hotsos/plugin_extensions/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/plugin_extensions/kubernetes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/plugin_extensions/kubernetes/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.759236 hotsos-1.18.post3/hotsos/plugin_extensions/lxd/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/plugin_extensions/lxd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/plugin_extensions/lxd/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.759236 hotsos-1.18.post3/hotsos/plugin_extensions/maas/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/plugin_extensions/maas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/plugin_extensions/maas/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.759236 hotsos-1.18.post3/hotsos/plugin_extensions/mysql/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/plugin_extensions/mysql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/plugin_extensions/mysql/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.759236 hotsos-1.18.post3/hotsos/plugin_extensions/openstack/
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/plugin_extensions/openstack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.759236 hotsos-1.18.post3/hotsos/plugin_extensions/openstack/agent/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/plugin_extensions/openstack/agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14361 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/plugin_extensions/openstack/agent/events.py
--rw-r--r--   0 runner    (1001) docker     (127)    11635 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/plugin_extensions/openstack/agent/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/plugin_extensions/openstack/nova_external_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     3864 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/plugin_extensions/openstack/service_features.py
--rw-r--r--   0 runner    (1001) docker     (127)     6560 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/plugin_extensions/openstack/service_network_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/plugin_extensions/openstack/summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     6733 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/plugin_extensions/openstack/vm_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.759236 hotsos-1.18.post3/hotsos/plugin_extensions/openvswitch/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/plugin_extensions/openvswitch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9596 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/plugin_extensions/openvswitch/event_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3045 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/plugin_extensions/openvswitch/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.763236 hotsos-1.18.post3/hotsos/plugin_extensions/pacemaker/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/plugin_extensions/pacemaker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/plugin_extensions/pacemaker/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.763236 hotsos-1.18.post3/hotsos/plugin_extensions/rabbitmq/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/plugin_extensions/rabbitmq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/plugin_extensions/rabbitmq/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.763236 hotsos-1.18.post3/hotsos/plugin_extensions/sosreport/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/plugin_extensions/sosreport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/plugin_extensions/sosreport/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.763236 hotsos-1.18.post3/hotsos/plugin_extensions/storage/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/plugin_extensions/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/plugin_extensions/storage/bcache_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     4142 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/plugin_extensions/storage/ceph_event_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/plugin_extensions/storage/ceph_summary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.763236 hotsos-1.18.post3/hotsos/plugin_extensions/system/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/plugin_extensions/system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6515 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/plugin_extensions/system/checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/plugin_extensions/system/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.763236 hotsos-1.18.post3/hotsos/plugin_extensions/vault/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/plugin_extensions/vault/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/plugin_extensions/vault/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.763236 hotsos-1.18.post3/hotsos/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/templates/content_dict.html
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/templates/content_list.html
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/templates/footer.html
--rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-05-22 10:58:49.000000 hotsos-1.18.post3/hotsos/templates/header.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:59:02.763236 hotsos-1.18.post3/hotsos.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-05-22 10:59:02.000000 hotsos-1.18.post3/hotsos.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    16724 2024-05-22 10:59:02.000000 hotsos-1.18.post3/hotsos.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 10:59:02.000000 hotsos-1.18.post3/hotsos.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-22 10:59:02.000000 hotsos-1.18.post3/hotsos.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-22 10:59:02.000000 hotsos-1.18.post3/hotsos.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-22 10:59:02.000000 hotsos-1.18.post3/hotsos.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-22 10:58:49.000000 hotsos-1.18.post3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-22 10:58:49.000000 hotsos-1.18.post3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 10:59:02.763236 hotsos-1.18.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-22 10:58:49.000000 hotsos-1.18.post3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.372111 hotsos-1.18.post4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-22 12:17:53.000000 hotsos-1.18.post4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-22 12:17:53.000000 hotsos-1.18.post4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-05-22 12:18:06.368111 hotsos-1.18.post4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-22 12:17:53.000000 hotsos-1.18.post4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.316111 hotsos-1.18.post4/hotsos/
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-22 12:17:59.000000 hotsos-1.18.post4/hotsos/.repo-info
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15279 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9421 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.316111 hotsos-1.18.post4/hotsos/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10725 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/analytics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9584 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.320111 hotsos-1.18.post4/hotsos/core/host_helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/host_helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/host_helpers/apparmor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42176 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/host_helpers/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/host_helpers/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4665 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/host_helpers/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/host_helpers/filestat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13279 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/host_helpers/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14487 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/host_helpers/packaging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/host_helpers/pebble.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/host_helpers/ssl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/host_helpers/sysctl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15568 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/host_helpers/systemd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3303 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/host_helpers/uptime.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.320111 hotsos-1.18.post4/hotsos/core/issues/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/issues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/issues/issue_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5375 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/issues/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/log.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.324111 hotsos-1.18.post4/hotsos/core/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.324111 hotsos-1.18.post4/hotsos/core/plugins/juju/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/plugins/juju/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/plugins/juju/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8187 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/plugins/juju/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.324111 hotsos-1.18.post4/hotsos/core/plugins/kernel/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/plugins/kernel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/plugins/kernel/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/plugins/kernel/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.324111 hotsos-1.18.post4/hotsos/core/plugins/kernel/kernlog/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/plugins/kernel/kernlog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14673 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/plugins/kernel/kernlog/calltrace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/plugins/kernel/kernlog/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/plugins/kernel/kernlog/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9200 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/plugins/kernel/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20751 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/plugins/kernel/net.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/plugins/kernel/sysfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/plugins/kubernetes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.324111 hotsos-1.18.post4/hotsos/core/plugins/lxd/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/plugins/lxd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/plugins/lxd/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/plugins/maas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/plugins/mysql.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.324111 hotsos-1.18.post4/hotsos/core/plugins/openstack/
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/plugins/openstack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8811 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/plugins/openstack/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63860 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/plugins/openstack/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3979 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/plugins/openstack/neutron.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11108 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/plugins/openstack/nova.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/plugins/openstack/octavia.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20116 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/plugins/openstack/openstack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.328111 hotsos-1.18.post4/hotsos/core/plugins/openvswitch/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/plugins/openvswitch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/plugins/openvswitch/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4830 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/plugins/openvswitch/ovn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7055 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/plugins/openvswitch/ovs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/plugins/pacemaker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.328111 hotsos-1.18.post4/hotsos/core/plugins/rabbitmq/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/plugins/rabbitmq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/plugins/rabbitmq/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8826 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/plugins/rabbitmq/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/plugins/sosreport.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.328111 hotsos-1.18.post4/hotsos/core/plugins/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/plugins/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7927 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/plugins/storage/bcache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38954 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/plugins/storage/ceph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.328111 hotsos-1.18.post4/hotsos/core/plugins/system/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/plugins/system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/plugins/system/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7081 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/plugins/system/system.py
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/plugins/vault.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15227 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/plugintools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4038 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/root_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.328111 hotsos-1.18.post4/hotsos/core/ycheck/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/ycheck/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.328111 hotsos-1.18.post4/hotsos/core/ycheck/engine/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/ycheck/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/ycheck/engine/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.328111 hotsos-1.18.post4/hotsos/core/ycheck/engine/properties/
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/ycheck/engine/properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8767 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/ycheck/engine/properties/checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17125 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/ycheck/engine/properties/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8427 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/ycheck/engine/properties/conclusions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/ycheck/engine/properties/inputdef.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.332111 hotsos-1.18.post4/hotsos/core/ycheck/engine/properties/requires/
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/ycheck/engine/properties/requires/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7464 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/ycheck/engine/properties/requires/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4382 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/ycheck/engine/properties/requires/requires.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.332111 hotsos-1.18.post4/hotsos/core/ycheck/engine/properties/requires/types/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/ycheck/engine/properties/requires/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8541 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/ycheck/engine/properties/requires/types/apt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/ycheck/engine/properties/requires/types/binary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7956 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/ycheck/engine/properties/requires/types/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/ycheck/engine/properties/requires/types/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/ycheck/engine/properties/requires/types/pebble.py
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/ycheck/engine/properties/requires/types/property.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/ycheck/engine/properties/requires/types/snap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5032 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/ycheck/engine/properties/requires/types/systemd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/ycheck/engine/properties/requires/types/varops.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15943 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/ycheck/engine/properties/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/ycheck/engine/properties/vardef.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27167 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/ycheck/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5992 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/core/ycheck/scenarios.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.252111 hotsos-1.18.post4/hotsos/defs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.252111 hotsos-1.18.post4/hotsos/defs/events/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.332111 hotsos-1.18.post4/hotsos/defs/events/openstack/
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/events/openstack/apache.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/events/openstack/apparmor.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/events/openstack/http-requests.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.332111 hotsos-1.18.post4/hotsos/defs/events/openstack/neutron/
+-rw-r--r--   0 runner    (1001) docker     (127)     3218 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/events/openstack/neutron/agents.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/events/openstack/neutron/ml2-routers.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.332111 hotsos-1.18.post4/hotsos/defs/events/openstack/nova/
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/events/openstack/nova/external-events.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.332111 hotsos-1.18.post4/hotsos/defs/events/openstack/nova/migrations/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.336111 hotsos-1.18.post4/hotsos/defs/events/openstack/nova/migrations/live-migration/
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/events/openstack/nova/migrations/live-migration/dst-pre-live-migration.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/events/openstack/nova/migrations/live-migration/src-migration.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/events/openstack/nova/migrations/live-migration/src-post-live-migration.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/events/openstack/nova/migrations/migrations.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/events/openstack/nova/nova-compute.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/events/openstack/octavia.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.252111 hotsos-1.18.post4/hotsos/defs/events/openvswitch/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.336111 hotsos-1.18.post4/hotsos/defs/events/openvswitch/ovn/
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/events/openvswitch/ovn/errors-and-warnings.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/events/openvswitch/ovn/ovn-central.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/events/openvswitch/ovn/ovn-controller.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.336111 hotsos-1.18.post4/hotsos/defs/events/openvswitch/ovs/
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/events/openvswitch/ovs/bfd.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/events/openvswitch/ovs/datapath-checks.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/events/openvswitch/ovs/errors-and-warnings.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/events/openvswitch/ovs/ovs-vswitchd.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.252111 hotsos-1.18.post4/hotsos/defs/events/storage/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.252111 hotsos-1.18.post4/hotsos/defs/events/storage/ceph/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.336111 hotsos-1.18.post4/hotsos/defs/events/storage/ceph/mon/
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/events/storage/ceph/mon/mon.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/events/storage/ceph/mon/monlogs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.336111 hotsos-1.18.post4/hotsos/defs/events/storage/ceph/osd/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/events/storage/ceph/osd/osd.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/events/storage/ceph/osd/osdlogs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.312111 hotsos-1.18.post4/hotsos/defs/scenarios/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.336111 hotsos-1.18.post4/hotsos/defs/scenarios/juju/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.340111 hotsos-1.18.post4/hotsos/defs/scenarios/juju/bugs/
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/juju/bugs/lp1812361.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/juju/bugs/lp1852502.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/juju/bugs/lp1858519.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/juju/bugs/lp1895040.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/juju/bugs/lp1910958.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/juju/bugs/lp1948906.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/juju/bugs/lp1983140.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/juju/bugs/lp1983506.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/juju/bugs/lp1996230.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/juju/charm_unit_checks.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/juju/juju.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/juju/juju_binary_cve.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/juju/juju_pebble_cve.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/juju/jujud_machine_checks.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/juju/snap_channel.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.340111 hotsos-1.18.post4/hotsos/defs/scenarios/kernel/
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/kernel/amd_iommu_pt.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/kernel/disk_failure.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/kernel/kernlog_calltrace.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/kernel/memory.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.340111 hotsos-1.18.post4/hotsos/defs/scenarios/kernel/network/
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/kernel/network/misc.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/kernel/network/netlink.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     7335 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/kernel/network/tcp.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3580 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/kernel/network/udp.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/kernel/qla2xxx.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.340111 hotsos-1.18.post4/hotsos/defs/scenarios/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/kubernetes/kubernetes.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/kubernetes/system_cpufreq_mode.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.340111 hotsos-1.18.post4/hotsos/defs/scenarios/lxd/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.340111 hotsos-1.18.post4/hotsos/defs/scenarios/lxd/bugs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/lxd/bugs/lp1807628.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/lxd/lxcfs_deadlock.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/lxd/snap_channel.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.340111 hotsos-1.18.post4/hotsos/defs/scenarios/maas/
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/maas/maas_proxy_issue.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.340111 hotsos-1.18.post4/hotsos/defs/scenarios/mysql/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.340111 hotsos-1.18.post4/hotsos/defs/scenarios/mysql/bugs/
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/mysql/bugs/lp1959861.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/mysql/bugs/lp1971565.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/mysql/bugs/lp2039444.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/mysql/bugs/lp372017.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/mysql/mysql.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/mysql/mysql_connections.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.344111 hotsos-1.18.post4/hotsos/defs/scenarios/openstack/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.252111 hotsos-1.18.post4/hotsos/defs/scenarios/openstack/barbican/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.344111 hotsos-1.18.post4/hotsos/defs/scenarios/openstack/barbican/bugs/
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/openstack/barbican/bugs/lp1946787.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.256111 hotsos-1.18.post4/hotsos/defs/scenarios/openstack/cinder/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.344111 hotsos-1.18.post4/hotsos/defs/scenarios/openstack/cinder/bugs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/openstack/cinder/bugs/lp2004555.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/openstack/eol.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.256111 hotsos-1.18.post4/hotsos/defs/scenarios/openstack/keystone/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.344111 hotsos-1.18.post4/hotsos/defs/scenarios/openstack/keystone/bugs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/openstack/keystone/bugs/lp1896125.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.344111 hotsos-1.18.post4/hotsos/defs/scenarios/openstack/masakari/
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/openstack/masakari/pacemaker_remote.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.344111 hotsos-1.18.post4/hotsos/defs/scenarios/openstack/neutron/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.348111 hotsos-1.18.post4/hotsos/defs/scenarios/openstack/neutron/bugs/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/openstack/neutron/bugs/lp1794991.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/openstack/neutron/bugs/lp1883089.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/openstack/neutron/bugs/lp1896506.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/openstack/neutron/bugs/lp1907686.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/openstack/neutron/bugs/lp1927868.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/openstack/neutron/bugs/lp1928031.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/openstack/neutron/bugs/lp1929832.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/openstack/neutron/bugs/lp1948466.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/openstack/neutron/bugs/lp1960319.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/openstack/neutron/bugs/lp1965297.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/openstack/neutron/bugs/lp1979089.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/openstack/neutron/bugs/lp1980211.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/openstack/neutron/bugs/lp1993628.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/openstack/neutron/bugs/lp1996594.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/openstack/neutron/neutron_ovs_cleanup.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/openstack/neutron/oslo_privsep_errors.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/openstack/neutron/ovn_stale_db.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/openstack/neutron/ovndb_leader_bouncing.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.348111 hotsos-1.18.post4/hotsos/defs/scenarios/openstack/nova/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.348111 hotsos-1.18.post4/hotsos/defs/scenarios/openstack/nova/bugs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/openstack/nova/bugs/lp1761062.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/openstack/nova/bugs/lp1860743.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/openstack/nova/bugs/lp1888395.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/openstack/nova/bugs/lp1904580.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/openstack/nova/bugs/lp1944619.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/openstack/nova/bugs/lp1967956.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/openstack/nova/bugs/lp2004555.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/openstack/nova/bugs/lp2012284.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/openstack/nova/config_checks.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6035 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/openstack/nova/cpu_pinning.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/openstack/nova/service_mem_usage.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.348111 hotsos-1.18.post4/hotsos/defs/scenarios/openstack/octavia/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.348111 hotsos-1.18.post4/hotsos/defs/scenarios/openstack/octavia/bugs/
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/openstack/octavia/bugs/lp2029857.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/openstack/octavia/bugs/sb1896125.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/openstack/octavia/excessive_failovers.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/openstack/octavia/hm_port_health.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/openstack/openstack.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/openstack/openstack_apache2_certificates.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/openstack/openstack_charm_conflicts.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.348111 hotsos-1.18.post4/hotsos/defs/scenarios/openstack/openstack_charms/
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/openstack/openstack_charms/nova_cc_ssh_known_hosts_fail.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/openstack/pkgs_from_mixed_releases_found.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/openstack/system_cpufreq_mode.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/openstack/systemd_masked_services.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.348111 hotsos-1.18.post4/hotsos/defs/scenarios/openvswitch/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.348111 hotsos-1.18.post4/hotsos/defs/scenarios/openvswitch/bugs/
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/openvswitch/bugs/lp1839592.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/openvswitch/bugs/lp1978806.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/openvswitch/dpdk_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/openvswitch/dpif_lost_packets.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/openvswitch/dpif_resubmit_actions.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/openvswitch/openvswitch.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.352111 hotsos-1.18.post4/hotsos/defs/scenarios/openvswitch/ovn/
+-rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/openvswitch/ovn/bfd_flapping.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.352111 hotsos-1.18.post4/hotsos/defs/scenarios/openvswitch/ovn/bugs/
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/openvswitch/ovn/bugs/lp1865127.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/openvswitch/ovn/bugs/lp1917475.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/openvswitch/ovn/ovn_central_certs_logs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/openvswitch/ovn/ovn_central_services.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/openvswitch/ovn/ovn_certs_valid.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/openvswitch/ovn/ovn_chassis_certs_logs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/openvswitch/ovn/ovn_elections.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/openvswitch/ovn/ovn_upgrades.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/openvswitch/ovn/service_mem_usage.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/openvswitch/service_restarts.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.352111 hotsos-1.18.post4/hotsos/defs/scenarios/pacemaker/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.352111 hotsos-1.18.post4/hotsos/defs/scenarios/pacemaker/bugs/
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/pacemaker/bugs/lp1874719.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/pacemaker/pacemaker.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.352111 hotsos-1.18.post4/hotsos/defs/scenarios/rabbitmq/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.352111 hotsos-1.18.post4/hotsos/defs/scenarios/rabbitmq/bugs/
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/rabbitmq/bugs/lp1943937.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/rabbitmq/cluster_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/rabbitmq/cluster_logchecks.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/rabbitmq/cluster_resources.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/rabbitmq/rabbitmq.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.352111 hotsos-1.18.post4/hotsos/defs/scenarios/sosreport/
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/sosreport/plugin_timeouts.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.352111 hotsos-1.18.post4/hotsos/defs/scenarios/storage/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.352111 hotsos-1.18.post4/hotsos/defs/scenarios/storage/bcache/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/storage/bcache/bcache.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/storage/bcache/bdev.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/storage/bcache/cacheset.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.308111 hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.352111 hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-mgr/
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-mgr/autoscaler_overlap_roots.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.360111 hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-mon/
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-mon/auth_insecure_global_id_reclaim_allowed.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-mon/autoscaler_bug.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-mon/bluefs_size.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-mon/bluefs_spillover.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph-mon.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph_address_overlap.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph_cluster_health.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph_versions_mismatch.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-mon/crushmap_bucket_checks.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-mon/empty_clog.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-mon/eol.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-mon/laggy_pgs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-mon/large_omap_objects.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-mon/meta_backend_mon.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-mon/mon_db_too_big.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-mon/mon_elections_flapping.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_flapping.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_maps_backlog_too_large.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_messenger_v2_protocol.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_slow_heartbeats.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_slow_ops.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_unusual_raw.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-mon/pg_imbalance.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-mon/pg_overdose.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-mon/required_osd_release_mismatch.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-mon/rgw_frontend.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-mon/ssds_using_bcache.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-mon/unresponsive_mon_mgr.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.360111 hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-osd/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.360111 hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp1936136.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp1959649.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp1996010.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp2013960.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp2016845.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-osd/ceph-osd.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-osd/ceph_address_overlap.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-osd/eol.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-osd/filestore_to_bluestore_upgrade.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-osd/juju_ceph_no_bcache_tuning.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-osd/meta_backend_osd.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-osd/osd_flapping.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-osd/osd_latency.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-osd/osd_slow_ops.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-osd/pg_overdose.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-osd/ssd_osds_no_discard.yaml.disabled
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-osd/system_cpufreq_mode.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.360111 hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-rgw/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.360111 hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-rgw/bugs/
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-rgw/bugs/lp1974138.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-rgw/rgw_frontend_rgw.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.360111 hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/common/
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/common/ceph_charm_conflicts.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.360111 hotsos-1.18.post4/hotsos/defs/scenarios/storage/nfs/
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/storage/nfs/nfs-detect-mount-name-resolution-failure.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/storage/storage.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.364111 hotsos-1.18.post4/hotsos/defs/scenarios/system/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/system/system.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/system/unattended_upgrades.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.364111 hotsos-1.18.post4/hotsos/defs/scenarios/vault/
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/defs/scenarios/vault/snap_channel.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.364111 hotsos-1.18.post4/hotsos/plugin_extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/plugin_extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.364111 hotsos-1.18.post4/hotsos/plugin_extensions/juju/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/plugin_extensions/juju/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/plugin_extensions/juju/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.364111 hotsos-1.18.post4/hotsos/plugin_extensions/kernel/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/plugin_extensions/kernel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/plugin_extensions/kernel/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.364111 hotsos-1.18.post4/hotsos/plugin_extensions/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/plugin_extensions/kubernetes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/plugin_extensions/kubernetes/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.364111 hotsos-1.18.post4/hotsos/plugin_extensions/lxd/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/plugin_extensions/lxd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/plugin_extensions/lxd/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.364111 hotsos-1.18.post4/hotsos/plugin_extensions/maas/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/plugin_extensions/maas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/plugin_extensions/maas/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.364111 hotsos-1.18.post4/hotsos/plugin_extensions/mysql/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/plugin_extensions/mysql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/plugin_extensions/mysql/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.364111 hotsos-1.18.post4/hotsos/plugin_extensions/openstack/
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/plugin_extensions/openstack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.364111 hotsos-1.18.post4/hotsos/plugin_extensions/openstack/agent/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/plugin_extensions/openstack/agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14361 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/plugin_extensions/openstack/agent/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11635 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/plugin_extensions/openstack/agent/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/plugin_extensions/openstack/nova_external_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3864 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/plugin_extensions/openstack/service_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6560 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/plugin_extensions/openstack/service_network_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/plugin_extensions/openstack/summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6733 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/plugin_extensions/openstack/vm_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.368111 hotsos-1.18.post4/hotsos/plugin_extensions/openvswitch/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/plugin_extensions/openvswitch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9596 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/plugin_extensions/openvswitch/event_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3045 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/plugin_extensions/openvswitch/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.368111 hotsos-1.18.post4/hotsos/plugin_extensions/pacemaker/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/plugin_extensions/pacemaker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/plugin_extensions/pacemaker/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.368111 hotsos-1.18.post4/hotsos/plugin_extensions/rabbitmq/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/plugin_extensions/rabbitmq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/plugin_extensions/rabbitmq/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.368111 hotsos-1.18.post4/hotsos/plugin_extensions/sosreport/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/plugin_extensions/sosreport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/plugin_extensions/sosreport/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.368111 hotsos-1.18.post4/hotsos/plugin_extensions/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/plugin_extensions/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/plugin_extensions/storage/bcache_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4142 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/plugin_extensions/storage/ceph_event_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/plugin_extensions/storage/ceph_summary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.368111 hotsos-1.18.post4/hotsos/plugin_extensions/system/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/plugin_extensions/system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6515 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/plugin_extensions/system/checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/plugin_extensions/system/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.368111 hotsos-1.18.post4/hotsos/plugin_extensions/vault/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/plugin_extensions/vault/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/plugin_extensions/vault/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.368111 hotsos-1.18.post4/hotsos/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/templates/content_dict.html
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/templates/content_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/templates/footer.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-05-22 12:17:53.000000 hotsos-1.18.post4/hotsos/templates/header.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:18:06.368111 hotsos-1.18.post4/hotsos.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-05-22 12:18:06.000000 hotsos-1.18.post4/hotsos.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16724 2024-05-22 12:18:06.000000 hotsos-1.18.post4/hotsos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 12:18:06.000000 hotsos-1.18.post4/hotsos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-22 12:18:06.000000 hotsos-1.18.post4/hotsos.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-22 12:18:06.000000 hotsos-1.18.post4/hotsos.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-22 12:18:06.000000 hotsos-1.18.post4/hotsos.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-22 12:17:53.000000 hotsos-1.18.post4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-22 12:17:53.000000 hotsos-1.18.post4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 12:18:06.372111 hotsos-1.18.post4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-22 12:17:53.000000 hotsos-1.18.post4/setup.py
```

### Comparing `hotsos-1.18.post3/LICENSE` & `hotsos-1.18.post4/LICENSE`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/PKG-INFO` & `hotsos-1.18.post4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hotsos
-Version: 1.18.post3
+Version: 1.18.post4
 Summary: Software analysis toolkit. Define checks in high-level language and leverage library to perform analysis of common Cloud applications.
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: importlib-metadata; python_version >= "3.8"
 Requires-Dist: click
 Requires-Dist: cryptography
```

### Comparing `hotsos-1.18.post3/README.md` & `hotsos-1.18.post4/README.md`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/cli.py` & `hotsos-1.18.post4/hotsos/cli.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/client.py` & `hotsos-1.18.post4/hotsos/client.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/core/analytics.py` & `hotsos-1.18.post4/hotsos/core/analytics.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/core/config.py` & `hotsos-1.18.post4/hotsos/core/config.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/core/factory.py` & `hotsos-1.18.post4/hotsos/core/factory.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/core/host_helpers/__init__.py` & `hotsos-1.18.post4/hotsos/core/host_helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/core/host_helpers/apparmor.py` & `hotsos-1.18.post4/hotsos/core/host_helpers/apparmor.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/core/host_helpers/cli.py` & `hotsos-1.18.post4/hotsos/core/host_helpers/cli.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/core/host_helpers/common.py` & `hotsos-1.18.post4/hotsos/core/host_helpers/common.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/core/host_helpers/config.py` & `hotsos-1.18.post4/hotsos/core/host_helpers/config.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/core/host_helpers/filestat.py` & `hotsos-1.18.post4/hotsos/core/host_helpers/filestat.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/core/host_helpers/network.py` & `hotsos-1.18.post4/hotsos/core/host_helpers/network.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/core/host_helpers/packaging.py` & `hotsos-1.18.post4/hotsos/core/host_helpers/packaging.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/core/host_helpers/pebble.py` & `hotsos-1.18.post4/hotsos/core/host_helpers/pebble.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/core/host_helpers/ssl.py` & `hotsos-1.18.post4/hotsos/core/host_helpers/ssl.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/core/host_helpers/sysctl.py` & `hotsos-1.18.post4/hotsos/core/host_helpers/sysctl.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/core/host_helpers/systemd.py` & `hotsos-1.18.post4/hotsos/core/host_helpers/systemd.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/core/host_helpers/uptime.py` & `hotsos-1.18.post4/hotsos/core/host_helpers/uptime.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/core/issues/issue_types.py` & `hotsos-1.18.post4/hotsos/core/issues/issue_types.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/core/issues/utils.py` & `hotsos-1.18.post4/hotsos/core/issues/utils.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/core/log.py` & `hotsos-1.18.post4/hotsos/core/log.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/core/plugins/juju/common.py` & `hotsos-1.18.post4/hotsos/core/plugins/juju/common.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/core/plugins/juju/resources.py` & `hotsos-1.18.post4/hotsos/core/plugins/juju/resources.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/core/plugins/kernel/common.py` & `hotsos-1.18.post4/hotsos/core/plugins/kernel/common.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/core/plugins/kernel/config.py` & `hotsos-1.18.post4/hotsos/core/plugins/kernel/config.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/core/plugins/kernel/kernlog/calltrace.py` & `hotsos-1.18.post4/hotsos/core/plugins/kernel/kernlog/calltrace.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/core/plugins/kernel/kernlog/common.py` & `hotsos-1.18.post4/hotsos/core/plugins/kernel/kernlog/common.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/core/plugins/kernel/kernlog/events.py` & `hotsos-1.18.post4/hotsos/core/plugins/kernel/kernlog/events.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/core/plugins/kernel/memory.py` & `hotsos-1.18.post4/hotsos/core/plugins/kernel/memory.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/core/plugins/kernel/net.py` & `hotsos-1.18.post4/hotsos/core/plugins/kernel/net.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/core/plugins/kernel/sysfs.py` & `hotsos-1.18.post4/hotsos/core/plugins/kernel/sysfs.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/core/plugins/kubernetes.py` & `hotsos-1.18.post4/hotsos/core/plugins/kubernetes.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/core/plugins/lxd/common.py` & `hotsos-1.18.post4/hotsos/core/plugins/lxd/common.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/core/plugins/maas.py` & `hotsos-1.18.post4/hotsos/core/plugins/maas.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/core/plugins/mysql.py` & `hotsos-1.18.post4/hotsos/core/plugins/mysql.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/core/plugins/openstack/common.py` & `hotsos-1.18.post4/hotsos/core/plugins/openstack/common.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/core/plugins/openstack/exceptions.py` & `hotsos-1.18.post4/hotsos/core/plugins/openstack/exceptions.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/core/plugins/openstack/neutron.py` & `hotsos-1.18.post4/hotsos/core/plugins/openstack/neutron.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/core/plugins/openstack/nova.py` & `hotsos-1.18.post4/hotsos/core/plugins/openstack/nova.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/core/plugins/openstack/octavia.py` & `hotsos-1.18.post4/hotsos/core/plugins/openstack/octavia.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/core/plugins/openstack/openstack.py` & `hotsos-1.18.post4/hotsos/core/plugins/openstack/openstack.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/core/plugins/openvswitch/common.py` & `hotsos-1.18.post4/hotsos/core/plugins/openvswitch/common.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/core/plugins/openvswitch/ovn.py` & `hotsos-1.18.post4/hotsos/core/plugins/openvswitch/ovn.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/core/plugins/openvswitch/ovs.py` & `hotsos-1.18.post4/hotsos/core/plugins/openvswitch/ovs.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/core/plugins/pacemaker.py` & `hotsos-1.18.post4/hotsos/core/plugins/pacemaker.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/core/plugins/rabbitmq/common.py` & `hotsos-1.18.post4/hotsos/core/plugins/rabbitmq/common.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/core/plugins/rabbitmq/report.py` & `hotsos-1.18.post4/hotsos/core/plugins/rabbitmq/report.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/core/plugins/sosreport.py` & `hotsos-1.18.post4/hotsos/core/plugins/sosreport.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/core/plugins/storage/bcache.py` & `hotsos-1.18.post4/hotsos/core/plugins/storage/bcache.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/core/plugins/storage/ceph.py` & `hotsos-1.18.post4/hotsos/core/plugins/storage/ceph.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/core/plugins/system/system.py` & `hotsos-1.18.post4/hotsos/core/plugins/system/system.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/core/plugins/vault.py` & `hotsos-1.18.post4/hotsos/core/plugins/vault.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/core/plugintools.py` & `hotsos-1.18.post4/hotsos/core/plugintools.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/core/root_manager.py` & `hotsos-1.18.post4/hotsos/core/root_manager.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/core/search.py` & `hotsos-1.18.post4/hotsos/core/search.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/core/utils.py` & `hotsos-1.18.post4/hotsos/core/utils.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/core/ycheck/engine/common.py` & `hotsos-1.18.post4/hotsos/core/ycheck/engine/common.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/core/ycheck/engine/properties/checks.py` & `hotsos-1.18.post4/hotsos/core/ycheck/engine/properties/checks.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/core/ycheck/engine/properties/common.py` & `hotsos-1.18.post4/hotsos/core/ycheck/engine/properties/common.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/core/ycheck/engine/properties/conclusions.py` & `hotsos-1.18.post4/hotsos/core/ycheck/engine/properties/conclusions.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/core/ycheck/engine/properties/inputdef.py` & `hotsos-1.18.post4/hotsos/core/ycheck/engine/properties/inputdef.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/core/ycheck/engine/properties/requires/common.py` & `hotsos-1.18.post4/hotsos/core/ycheck/engine/properties/requires/common.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/core/ycheck/engine/properties/requires/requires.py` & `hotsos-1.18.post4/hotsos/core/ycheck/engine/properties/requires/requires.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/core/ycheck/engine/properties/requires/types/apt.py` & `hotsos-1.18.post4/hotsos/core/ycheck/engine/properties/requires/types/apt.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/core/ycheck/engine/properties/requires/types/binary.py` & `hotsos-1.18.post4/hotsos/core/ycheck/engine/properties/requires/types/binary.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/core/ycheck/engine/properties/requires/types/config.py` & `hotsos-1.18.post4/hotsos/core/ycheck/engine/properties/requires/types/config.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/core/ycheck/engine/properties/requires/types/path.py` & `hotsos-1.18.post4/hotsos/core/ycheck/engine/properties/requires/types/path.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/core/ycheck/engine/properties/requires/types/pebble.py` & `hotsos-1.18.post4/hotsos/core/ycheck/engine/properties/requires/types/pebble.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/core/ycheck/engine/properties/requires/types/property.py` & `hotsos-1.18.post4/hotsos/core/ycheck/engine/properties/requires/types/property.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/core/ycheck/engine/properties/requires/types/snap.py` & `hotsos-1.18.post4/hotsos/core/ycheck/engine/properties/requires/types/snap.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/core/ycheck/engine/properties/requires/types/systemd.py` & `hotsos-1.18.post4/hotsos/core/ycheck/engine/properties/requires/types/systemd.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/core/ycheck/engine/properties/requires/types/varops.py` & `hotsos-1.18.post4/hotsos/core/ycheck/engine/properties/requires/types/varops.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/core/ycheck/engine/properties/search.py` & `hotsos-1.18.post4/hotsos/core/ycheck/engine/properties/search.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/core/ycheck/engine/properties/vardef.py` & `hotsos-1.18.post4/hotsos/core/ycheck/engine/properties/vardef.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/core/ycheck/events.py` & `hotsos-1.18.post4/hotsos/core/ycheck/events.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/core/ycheck/scenarios.py` & `hotsos-1.18.post4/hotsos/core/ycheck/scenarios.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/events/openstack/apparmor.yaml` & `hotsos-1.18.post4/hotsos/defs/events/openstack/apparmor.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/events/openstack/neutron/agents.yaml` & `hotsos-1.18.post4/hotsos/defs/events/openstack/neutron/agents.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/events/openstack/nova/external-events.yaml` & `hotsos-1.18.post4/hotsos/defs/events/openstack/nova/external-events.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/events/openstack/octavia.yaml` & `hotsos-1.18.post4/hotsos/defs/events/openstack/octavia.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/events/openvswitch/ovn/errors-and-warnings.yaml` & `hotsos-1.18.post4/hotsos/defs/events/openvswitch/ovn/errors-and-warnings.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/events/openvswitch/ovn/ovn-central.yaml` & `hotsos-1.18.post4/hotsos/defs/events/openvswitch/ovn/ovn-central.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/events/openvswitch/ovn/ovn-controller.yaml` & `hotsos-1.18.post4/hotsos/defs/events/openvswitch/ovn/ovn-controller.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/events/openvswitch/ovs/datapath-checks.yaml` & `hotsos-1.18.post4/hotsos/defs/events/openvswitch/ovs/datapath-checks.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/events/openvswitch/ovs/ovs-vswitchd.yaml` & `hotsos-1.18.post4/hotsos/defs/events/openvswitch/ovs/ovs-vswitchd.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/events/storage/ceph/mon/monlogs.yaml` & `hotsos-1.18.post4/hotsos/defs/events/storage/ceph/mon/monlogs.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/events/storage/ceph/osd/osdlogs.yaml` & `hotsos-1.18.post4/hotsos/defs/events/storage/ceph/osd/osdlogs.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/juju/bugs/lp1812361.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/juju/bugs/lp1812361.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/juju/bugs/lp1852502.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/juju/bugs/lp1852502.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/juju/bugs/lp1858519.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/juju/bugs/lp1858519.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/juju/bugs/lp1895040.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/juju/bugs/lp1895040.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/juju/bugs/lp1910958.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/juju/bugs/lp1910958.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/juju/bugs/lp1948906.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/juju/bugs/lp1948906.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/juju/bugs/lp1996230.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/juju/bugs/lp1996230.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/juju/charm_unit_checks.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/juju/charm_unit_checks.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/juju/juju_binary_cve.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/juju/juju_binary_cve.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/juju/juju_pebble_cve.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/juju/juju_pebble_cve.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/juju/snap_channel.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/juju/snap_channel.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/kernel/amd_iommu_pt.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/kernel/amd_iommu_pt.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/kernel/disk_failure.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/kernel/disk_failure.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/kernel/kernlog_calltrace.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/kernel/kernlog_calltrace.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/kernel/memory.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/kernel/memory.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/kernel/network/misc.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/kernel/network/misc.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/kernel/network/netlink.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/kernel/network/netlink.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/kernel/network/tcp.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/kernel/network/tcp.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/kernel/network/udp.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/kernel/network/udp.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/kernel/qla2xxx.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/kernel/qla2xxx.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/kubernetes/system_cpufreq_mode.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/kubernetes/system_cpufreq_mode.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/lxd/bugs/lp1807628.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/lxd/bugs/lp1807628.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/lxd/lxcfs_deadlock.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/lxd/lxcfs_deadlock.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/lxd/snap_channel.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/lxd/snap_channel.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/maas/maas_proxy_issue.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/maas/maas_proxy_issue.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/mysql/bugs/lp1959861.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/mysql/bugs/lp1959861.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/mysql/bugs/lp1971565.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/mysql/bugs/lp1971565.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/mysql/bugs/lp2039444.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/mysql/bugs/lp2039444.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/mysql/mysql_connections.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/mysql/mysql_connections.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/openstack/barbican/bugs/lp1946787.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/openstack/barbican/bugs/lp1946787.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/openstack/cinder/bugs/lp2004555.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/openstack/cinder/bugs/lp2004555.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/openstack/eol.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/openstack/eol.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/openstack/keystone/bugs/lp1896125.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/openstack/keystone/bugs/lp1896125.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/openstack/masakari/pacemaker_remote.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/openstack/masakari/pacemaker_remote.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/openstack/neutron/bugs/lp1794991.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/openstack/neutron/bugs/lp1794991.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/openstack/neutron/bugs/lp1896506.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/openstack/neutron/bugs/lp1896506.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/openstack/neutron/bugs/lp1907686.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/openstack/neutron/bugs/lp1907686.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/openstack/neutron/bugs/lp1927868.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/openstack/neutron/bugs/lp1927868.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/openstack/neutron/bugs/lp1948466.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/openstack/neutron/bugs/lp1948466.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/openstack/neutron/bugs/lp1960319.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/openstack/neutron/bugs/lp1960319.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/openstack/neutron/bugs/lp1979089.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/openstack/neutron/bugs/lp1979089.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/openstack/neutron/bugs/lp1980211.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/openstack/neutron/bugs/lp1980211.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/openstack/neutron/bugs/lp1993628.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/openstack/neutron/bugs/lp1993628.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/openstack/neutron/bugs/lp1996594.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/openstack/neutron/bugs/lp1996594.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/openstack/neutron/neutron_ovs_cleanup.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/openstack/neutron/neutron_ovs_cleanup.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/openstack/neutron/oslo_privsep_errors.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/openstack/neutron/oslo_privsep_errors.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/openstack/neutron/ovn_stale_db.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/openstack/neutron/ovn_stale_db.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/openstack/neutron/ovndb_leader_bouncing.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/openstack/neutron/ovndb_leader_bouncing.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/openstack/nova/bugs/lp1761062.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/openstack/nova/bugs/lp1761062.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/openstack/nova/bugs/lp1860743.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/openstack/nova/bugs/lp1860743.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/openstack/nova/bugs/lp1888395.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/openstack/nova/bugs/lp1888395.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/openstack/nova/bugs/lp1904580.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/openstack/nova/bugs/lp1904580.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/openstack/nova/bugs/lp1967956.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/openstack/nova/bugs/lp1967956.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/openstack/nova/bugs/lp2004555.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/openstack/nova/bugs/lp2004555.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/openstack/nova/bugs/lp2012284.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/openstack/nova/bugs/lp2012284.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/openstack/nova/config_checks.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/openstack/nova/config_checks.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/openstack/nova/cpu_pinning.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/openstack/nova/cpu_pinning.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/openstack/nova/service_mem_usage.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/openstack/nova/service_mem_usage.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/openstack/octavia/bugs/lp2029857.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/openstack/octavia/bugs/lp2029857.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/openstack/octavia/bugs/sb1896125.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/openstack/octavia/bugs/sb1896125.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/openstack/octavia/excessive_failovers.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/openstack/octavia/excessive_failovers.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/openstack/octavia/hm_port_health.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/openstack/octavia/hm_port_health.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/openstack/openstack_apache2_certificates.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/openstack/openstack_apache2_certificates.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/openstack/openstack_charm_conflicts.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/openstack/openstack_charm_conflicts.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/openstack/openstack_charms/nova_cc_ssh_known_hosts_fail.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/openstack/openstack_charms/nova_cc_ssh_known_hosts_fail.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/openstack/system_cpufreq_mode.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/openstack/system_cpufreq_mode.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/openstack/systemd_masked_services.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/openstack/systemd_masked_services.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/openvswitch/bugs/lp1839592.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/openvswitch/bugs/lp1839592.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/openvswitch/bugs/lp1978806.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/openvswitch/bugs/lp1978806.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/openvswitch/dpdk_config.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/openvswitch/dpdk_config.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/openvswitch/dpif_lost_packets.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/openvswitch/dpif_lost_packets.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/openvswitch/dpif_resubmit_actions.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/openvswitch/dpif_resubmit_actions.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/openvswitch/ovn/bfd_flapping.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/openvswitch/ovn/bfd_flapping.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/openvswitch/ovn/bugs/lp1865127.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/openvswitch/ovn/bugs/lp1865127.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/openvswitch/ovn/ovn_central_certs_logs.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/openvswitch/ovn/ovn_central_certs_logs.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/openvswitch/ovn/ovn_central_services.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/openvswitch/ovn/ovn_central_services.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/openvswitch/ovn/ovn_certs_valid.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/openvswitch/ovn/ovn_certs_valid.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/openvswitch/ovn/ovn_chassis_certs_logs.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/openvswitch/ovn/ovn_chassis_certs_logs.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/openvswitch/ovn/ovn_elections.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/openvswitch/ovn/ovn_elections.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/openvswitch/ovn/ovn_upgrades.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/openvswitch/ovn/ovn_upgrades.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/openvswitch/ovn/service_mem_usage.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/openvswitch/ovn/service_mem_usage.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/openvswitch/service_restarts.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/openvswitch/service_restarts.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/pacemaker/bugs/lp1874719.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/pacemaker/bugs/lp1874719.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/rabbitmq/bugs/lp1943937.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/rabbitmq/bugs/lp1943937.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/rabbitmq/cluster_config.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/rabbitmq/cluster_config.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/rabbitmq/cluster_logchecks.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/rabbitmq/cluster_logchecks.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/rabbitmq/cluster_resources.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/rabbitmq/cluster_resources.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/sosreport/plugin_timeouts.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/sosreport/plugin_timeouts.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/storage/bcache/bdev.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/storage/bcache/bdev.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/storage/bcache/cacheset.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/storage/bcache/cacheset.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-mgr/autoscaler_overlap_roots.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-mgr/autoscaler_overlap_roots.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-mon/auth_insecure_global_id_reclaim_allowed.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-mon/auth_insecure_global_id_reclaim_allowed.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-mon/autoscaler_bug.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-mon/autoscaler_bug.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-mon/bluefs_size.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-mon/bluefs_size.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-mon/bluefs_spillover.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-mon/bluefs_spillover.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph-mon.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph-mon.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph_address_overlap.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph_address_overlap.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph_cluster_health.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph_cluster_health.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph_versions_mismatch.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-mon/ceph_versions_mismatch.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-mon/crushmap_bucket_checks.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-mon/crushmap_bucket_checks.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-mon/empty_clog.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-mon/empty_clog.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-mon/eol.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-mon/eol.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-mon/laggy_pgs.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-mon/laggy_pgs.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-mon/large_omap_objects.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-mon/large_omap_objects.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-mon/meta_backend_mon.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-mon/meta_backend_mon.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-mon/mon_db_too_big.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-mon/mon_db_too_big.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-mon/mon_elections_flapping.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-mon/mon_elections_flapping.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_flapping.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_flapping.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_maps_backlog_too_large.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_maps_backlog_too_large.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_messenger_v2_protocol.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_messenger_v2_protocol.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_slow_heartbeats.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_slow_heartbeats.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_slow_ops.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_slow_ops.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_unusual_raw.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-mon/osd_unusual_raw.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-mon/pg_imbalance.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-mon/pg_imbalance.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-mon/pg_overdose.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-mon/pg_overdose.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-mon/required_osd_release_mismatch.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-mon/required_osd_release_mismatch.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-mon/rgw_frontend.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-mon/rgw_frontend.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-mon/ssds_using_bcache.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-mon/ssds_using_bcache.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-mon/unresponsive_mon_mgr.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-mon/unresponsive_mon_mgr.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp1936136.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp1936136.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp1959649.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp1959649.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp1996010.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp1996010.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp2013960.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp2013960.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp2016845.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-osd/bugs/lp2016845.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-osd/ceph_address_overlap.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-osd/ceph_address_overlap.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-osd/eol.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-osd/eol.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-osd/filestore_to_bluestore_upgrade.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-osd/filestore_to_bluestore_upgrade.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-osd/juju_ceph_no_bcache_tuning.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-osd/juju_ceph_no_bcache_tuning.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-osd/meta_backend_osd.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-osd/meta_backend_osd.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-osd/osd_flapping.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-osd/osd_flapping.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-osd/osd_latency.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-osd/osd_latency.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-osd/osd_slow_ops.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-osd/osd_slow_ops.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-osd/pg_overdose.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-osd/pg_overdose.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-osd/ssd_osds_no_discard.yaml.disabled` & `hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-osd/ssd_osds_no_discard.yaml.disabled`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-osd/system_cpufreq_mode.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-osd/system_cpufreq_mode.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-rgw/bugs/lp1974138.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-rgw/bugs/lp1974138.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/ceph-rgw/rgw_frontend_rgw.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/ceph-rgw/rgw_frontend_rgw.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/storage/ceph/common/ceph_charm_conflicts.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/storage/ceph/common/ceph_charm_conflicts.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/storage/nfs/nfs-detect-mount-name-resolution-failure.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/storage/nfs/nfs-detect-mount-name-resolution-failure.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/defs/scenarios/vault/snap_channel.yaml` & `hotsos-1.18.post4/hotsos/defs/scenarios/vault/snap_channel.yaml`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/plugin_extensions/juju/summary.py` & `hotsos-1.18.post4/hotsos/plugin_extensions/juju/summary.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/plugin_extensions/kernel/summary.py` & `hotsos-1.18.post4/hotsos/plugin_extensions/kernel/summary.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/plugin_extensions/kubernetes/summary.py` & `hotsos-1.18.post4/hotsos/plugin_extensions/kubernetes/summary.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/plugin_extensions/lxd/summary.py` & `hotsos-1.18.post4/hotsos/plugin_extensions/lxd/summary.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/plugin_extensions/openstack/agent/events.py` & `hotsos-1.18.post4/hotsos/plugin_extensions/openstack/agent/events.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/plugin_extensions/openstack/agent/exceptions.py` & `hotsos-1.18.post4/hotsos/plugin_extensions/openstack/agent/exceptions.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/plugin_extensions/openstack/nova_external_events.py` & `hotsos-1.18.post4/hotsos/plugin_extensions/openstack/nova_external_events.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/plugin_extensions/openstack/service_features.py` & `hotsos-1.18.post4/hotsos/plugin_extensions/openstack/service_features.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/plugin_extensions/openstack/service_network_checks.py` & `hotsos-1.18.post4/hotsos/plugin_extensions/openstack/service_network_checks.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/plugin_extensions/openstack/summary.py` & `hotsos-1.18.post4/hotsos/plugin_extensions/openstack/summary.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/plugin_extensions/openstack/vm_info.py` & `hotsos-1.18.post4/hotsos/plugin_extensions/openstack/vm_info.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/plugin_extensions/openvswitch/event_checks.py` & `hotsos-1.18.post4/hotsos/plugin_extensions/openvswitch/event_checks.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/plugin_extensions/openvswitch/summary.py` & `hotsos-1.18.post4/hotsos/plugin_extensions/openvswitch/summary.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/plugin_extensions/pacemaker/summary.py` & `hotsos-1.18.post4/hotsos/plugin_extensions/pacemaker/summary.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/plugin_extensions/rabbitmq/summary.py` & `hotsos-1.18.post4/hotsos/plugin_extensions/rabbitmq/summary.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/plugin_extensions/storage/bcache_summary.py` & `hotsos-1.18.post4/hotsos/plugin_extensions/storage/bcache_summary.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/plugin_extensions/storage/ceph_event_checks.py` & `hotsos-1.18.post4/hotsos/plugin_extensions/storage/ceph_event_checks.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/plugin_extensions/storage/ceph_summary.py` & `hotsos-1.18.post4/hotsos/plugin_extensions/storage/ceph_summary.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/plugin_extensions/system/checks.py` & `hotsos-1.18.post4/hotsos/plugin_extensions/system/checks.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/plugin_extensions/system/summary.py` & `hotsos-1.18.post4/hotsos/plugin_extensions/system/summary.py`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos/templates/header.html` & `hotsos-1.18.post4/hotsos/templates/header.html`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/hotsos.egg-info/PKG-INFO` & `hotsos-1.18.post4/hotsos.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hotsos
-Version: 1.18.post3
+Version: 1.18.post4
 Summary: Software analysis toolkit. Define checks in high-level language and leverage library to perform analysis of common Cloud applications.
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: importlib-metadata; python_version >= "3.8"
 Requires-Dist: click
 Requires-Dist: cryptography
```

### Comparing `hotsos-1.18.post3/hotsos.egg-info/SOURCES.txt` & `hotsos-1.18.post4/hotsos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hotsos-1.18.post3/pyproject.toml` & `hotsos-1.18.post4/pyproject.toml`

 * *Files identical despite different names*

