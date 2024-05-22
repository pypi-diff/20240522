# Comparing `tmp/pulumi_proxmoxve-6.7.0.tar.gz` & `tmp/pulumi_proxmoxve-6.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_proxmoxve-6.7.0.tar", last modified: Sat May 18 07:39:44 2024, max compression
+gzip compressed data, was "pulumi_proxmoxve-6.7.1.tar", last modified: Wed May 22 16:13:12 2024, max compression
```

## Comparing `pulumi_proxmoxve-6.7.0.tar` & `pulumi_proxmoxve-6.7.1.tar`

### file list

```diff
@@ -1,113 +1,114 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:39:44.974943 pulumi_proxmoxve-6.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-05-18 07:39:44.974943 pulumi_proxmoxve-6.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6356 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:39:44.962943 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/
--rw-r--r--   0 runner    (1001) docker     (127)     6781 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15492 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9295 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    17555 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/acl.py
--rw-r--r--   0 runner    (1001) docker     (127)    22894 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/certifi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:39:44.962943 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/cluster/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6270 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/cluster/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6822 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/cluster/get_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)    53365 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/cluster/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     5692 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/cluster/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:39:44.966943 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7007 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/config/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/config/vars.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:39:44.966943 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/ct/
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/ct/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36258 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/ct/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    64491 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/ct/container.py
--rw-r--r--   0 runner    (1001) docker     (127)    31452 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/ct/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9231 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/dns.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:39:44.966943 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/download/
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/download/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38006 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/download/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     6188 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/get_node.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:39:44.966943 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/ha/
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/ha/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5390 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/ha/get_ha_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/ha/get_ha_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     6209 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/ha/get_ha_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     4145 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/ha/get_ha_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)    16647 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/ha/ha_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    18177 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/ha/ha_resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:39:44.966943 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/hardware/
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/hardware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5305 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/hardware/get_mappings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:39:44.966943 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/hardware/mapping/
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/hardware/mapping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6138 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/hardware/mapping/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4507 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/hardware/mapping/get_pci.py
--rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/hardware/mapping/get_usb.py
--rw-r--r--   0 runner    (1001) docker     (127)     8778 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/hardware/mapping/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    11996 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/hardware/mapping/pci.py
--rw-r--r--   0 runner    (1001) docker     (127)    10684 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/hardware/mapping/usb.py
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/hardware/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    12925 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/hosts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:39:44.970943 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/network/
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25888 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/network/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    15402 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/network/firewall.py
--rw-r--r--   0 runner    (1001) docker     (127)    15973 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/network/firewall_alias.py
--rw-r--r--   0 runner    (1001) docker     (127)    17304 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/network/firewall_ip_set.py
--rw-r--r--   0 runner    (1001) docker     (127)    32979 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/network/firewall_options.py
--rw-r--r--   0 runner    (1001) docker     (127)    16679 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/network/firewall_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)    17992 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/network/firewall_security_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/network/get_dns.py
--rw-r--r--   0 runner    (1001) docker     (127)     4794 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/network/get_hosts.py
--rw-r--r--   0 runner    (1001) docker     (127)     4242 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/network/get_time.py
--rw-r--r--   0 runner    (1001) docker     (127)     3956 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/network/get_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    24800 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/network/network_bridge.py
--rw-r--r--   0 runner    (1001) docker     (127)    25201 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/network/network_vlan.py
--rw-r--r--   0 runner    (1001) docker     (127)    22405 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/network/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5371 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:39:44.974943 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/permission/
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/permission/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6185 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/permission/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4215 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/permission/get_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/permission/get_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/permission/get_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/permission/get_pools.py
--rw-r--r--   0 runner    (1001) docker     (127)     3263 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/permission/get_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/permission/get_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)     6877 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/permission/get_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     6427 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/permission/get_users.py
--rw-r--r--   0 runner    (1001) docker     (127)    11465 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/permission/group.py
--rw-r--r--   0 runner    (1001) docker     (127)     9837 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/permission/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9044 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/permission/pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     8325 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/permission/role.py
--rw-r--r--   0 runner    (1001) docker     (127)    25525 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/permission/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    14153 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:39:44.974943 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/storage/
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5983 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/storage/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    30347 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/storage/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     7490 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/storage/get_datastores.py
--rw-r--r--   0 runner    (1001) docker     (127)     5702 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/storage/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9983 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/time.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:39:44.974943 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/user/
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16708 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/user/token.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:39:44.974943 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/vm/
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/vm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    87349 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/vm/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4439 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/vm/get_virtual_machine.py
--rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/vm/get_virtual_machines.py
--rw-r--r--   0 runner    (1001) docker     (127)    75190 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/vm/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)   123851 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/vm/virtual_machine.py
--rw-r--r--   0 runner    (1001) docker     (127)    18045 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/vm2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:39:44.962943 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/pulumi_proxmoxve.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 07:39:44.974943 pulumi_proxmoxve-6.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-18 07:39:44.000000 pulumi_proxmoxve-6.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:13:12.043790 pulumi_proxmoxve-6.7.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-05-22 16:13:12.043790 pulumi_proxmoxve-6.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6356 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:13:12.031790 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/
+-rw-r--r--   0 runner    (1001) docker     (127)     6804 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29531 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9295 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17555 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/acl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22894 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/certifi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:13:12.031790 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/cluster/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6270 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/cluster/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6822 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/cluster/get_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53365 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/cluster/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5692 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/cluster/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:13:12.031790 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7007 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/config/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/config/vars.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:13:12.035790 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/ct/
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/ct/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36258 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/ct/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64491 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/ct/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31452 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/ct/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9231 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/dns.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:13:12.035790 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/download/
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/download/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38006 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/download/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6188 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/get_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8061 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/get_vm2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:13:12.035790 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/ha/
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/ha/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5390 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/ha/get_ha_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/ha/get_ha_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6209 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/ha/get_ha_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4145 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/ha/get_ha_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16647 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/ha/ha_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18177 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/ha/ha_resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:13:12.035790 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/hardware/
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/hardware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5305 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/hardware/get_mappings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:13:12.035790 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/hardware/mapping/
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/hardware/mapping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6138 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/hardware/mapping/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4507 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/hardware/mapping/get_pci.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/hardware/mapping/get_usb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8778 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/hardware/mapping/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11996 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/hardware/mapping/pci.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10684 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/hardware/mapping/usb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/hardware/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12925 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/hosts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:13:12.039790 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/network/
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25888 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/network/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15402 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/network/firewall.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15973 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/network/firewall_alias.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17304 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/network/firewall_ip_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32979 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/network/firewall_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16679 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/network/firewall_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17992 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/network/firewall_security_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/network/get_dns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4794 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/network/get_hosts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4242 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/network/get_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3956 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/network/get_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24800 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/network/network_bridge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25201 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/network/network_vlan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22405 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/network/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16471 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:13:12.039790 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/permission/
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/permission/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6185 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/permission/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4215 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/permission/get_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/permission/get_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/permission/get_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/permission/get_pools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3263 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/permission/get_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/permission/get_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6877 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/permission/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6427 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/permission/get_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11465 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/permission/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9837 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/permission/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9044 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/permission/pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8325 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/permission/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25525 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/permission/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14153 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:13:12.039790 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5983 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/storage/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30347 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/storage/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7490 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/storage/get_datastores.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5702 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/storage/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9983 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/time.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:13:12.043790 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/user/
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16708 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/user/token.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:13:12.043790 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/vm/
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/vm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    87349 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/vm/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4439 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/vm/get_virtual_machine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/vm/get_virtual_machines.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75190 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/vm/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   123851 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/vm/virtual_machine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19471 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/vm2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:13:12.031790 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-05-22 16:13:12.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-05-22 16:13:12.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 16:13:12.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 16:13:12.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-22 16:13:12.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-22 16:13:12.000000 pulumi_proxmoxve-6.7.1/pulumi_proxmoxve.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 16:13:12.043790 pulumi_proxmoxve-6.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-22 16:13:11.000000 pulumi_proxmoxve-6.7.1/setup.py
```

### Comparing `pulumi_proxmoxve-6.7.0/PKG-INFO` & `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pulumi_proxmoxve
-Version: 6.7.0
+Name: pulumi-proxmoxve
+Version: 6.7.1
 Summary: A Pulumi package for creating and managing Proxmox Virtual Environment cloud resources.
 Home-page: https://github.com/muhlba91/pulumi-proxmoxve
 License: Apache-2.0
 Project-URL: Repository, https://github.com/muhlba91/pulumi-proxmoxve
 Keywords: pulumi proxmox proxmoxve
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `pulumi_proxmoxve-6.7.0/README.md` & `pulumi_proxmoxve-6.7.1/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/__init__.py` & `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from . import _utilities
 import typing
 # Export this package's modules as members:
 from .acl import *
 from .certifi import *
 from .dns import *
 from .get_node import *
+from .get_vm2 import *
 from .hosts import *
 from .provider import *
 from .time import *
 from .vm2 import *
 from ._inputs import *
 from . import outputs
```

### Comparing `pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/_inputs.py` & `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/provider.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,366 +4,323 @@
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
+from ._inputs import *
 
-__all__ = [
-    'HostsEntryArgs',
-    'ProviderSshArgs',
-    'ProviderSshNodeArgs',
-    'Vm2CloneArgs',
-    'Vm2TimeoutsArgs',
-]
+__all__ = ['ProviderArgs', 'Provider']
 
 @pulumi.input_type
-class HostsEntryArgs:
+class ProviderArgs:
     def __init__(__self__, *,
-                 address: pulumi.Input[str],
-                 hostnames: pulumi.Input[Sequence[pulumi.Input[str]]]):
-        """
-        :param pulumi.Input[str] address: The IP address.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] hostnames: The hostnames.
+                 api_token: Optional[pulumi.Input[str]] = None,
+                 endpoint: Optional[pulumi.Input[str]] = None,
+                 insecure: Optional[pulumi.Input[bool]] = None,
+                 min_tls: Optional[pulumi.Input[str]] = None,
+                 otp: Optional[pulumi.Input[str]] = None,
+                 password: Optional[pulumi.Input[str]] = None,
+                 ssh: Optional[pulumi.Input['ProviderSshArgs']] = None,
+                 tmp_dir: Optional[pulumi.Input[str]] = None,
+                 username: Optional[pulumi.Input[str]] = None):
         """
-        pulumi.set(__self__, "address", address)
-        pulumi.set(__self__, "hostnames", hostnames)
+        The set of arguments for constructing a Provider resource.
+        :param pulumi.Input[str] api_token: The API token for the Proxmox VE API.
+        :param pulumi.Input[str] endpoint: The endpoint for the Proxmox VE API.
+        :param pulumi.Input[bool] insecure: Whether to skip the TLS verification step.
+        :param pulumi.Input[str] min_tls: The minimum required TLS version for API calls.Supported values: `1.0|1.1|1.2|1.3`. Defaults to `1.3`.
+        :param pulumi.Input[str] otp: The one-time password for the Proxmox VE API.
+        :param pulumi.Input[str] password: The password for the Proxmox VE API.
+        :param pulumi.Input['ProviderSshArgs'] ssh: The SSH configuration for the Proxmox nodes.
+        :param pulumi.Input[str] tmp_dir: The alternative temporary directory.
+        :param pulumi.Input[str] username: The username for the Proxmox VE API.
+        """
+        if api_token is not None:
+            pulumi.set(__self__, "api_token", api_token)
+        if endpoint is not None:
+            pulumi.set(__self__, "endpoint", endpoint)
+        if insecure is not None:
+            pulumi.set(__self__, "insecure", insecure)
+        if min_tls is not None:
+            pulumi.set(__self__, "min_tls", min_tls)
+        if otp is not None:
+            warnings.warn("""The `otp` attribute is deprecated and will be removed in a future release. Please use the `api_token` attribute instead.""", DeprecationWarning)
+            pulumi.log.warn("""otp is deprecated: The `otp` attribute is deprecated and will be removed in a future release. Please use the `api_token` attribute instead.""")
+        if otp is not None:
+            pulumi.set(__self__, "otp", otp)
+        if password is not None:
+            pulumi.set(__self__, "password", password)
+        if ssh is not None:
+            pulumi.set(__self__, "ssh", ssh)
+        if tmp_dir is not None:
+            pulumi.set(__self__, "tmp_dir", tmp_dir)
+        if username is not None:
+            pulumi.set(__self__, "username", username)
 
     @property
-    @pulumi.getter
-    def address(self) -> pulumi.Input[str]:
+    @pulumi.getter(name="apiToken")
+    def api_token(self) -> Optional[pulumi.Input[str]]:
         """
-        The IP address.
+        The API token for the Proxmox VE API.
         """
-        return pulumi.get(self, "address")
+        return pulumi.get(self, "api_token")
 
-    @address.setter
-    def address(self, value: pulumi.Input[str]):
-        pulumi.set(self, "address", value)
+    @api_token.setter
+    def api_token(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "api_token", value)
 
     @property
     @pulumi.getter
-    def hostnames(self) -> pulumi.Input[Sequence[pulumi.Input[str]]]:
+    def endpoint(self) -> Optional[pulumi.Input[str]]:
         """
-        The hostnames.
+        The endpoint for the Proxmox VE API.
         """
-        return pulumi.get(self, "hostnames")
-
-    @hostnames.setter
-    def hostnames(self, value: pulumi.Input[Sequence[pulumi.Input[str]]]):
-        pulumi.set(self, "hostnames", value)
+        return pulumi.get(self, "endpoint")
 
-
-@pulumi.input_type
-class ProviderSshArgs:
-    def __init__(__self__, *,
-                 agent: Optional[pulumi.Input[bool]] = None,
-                 agent_socket: Optional[pulumi.Input[str]] = None,
-                 nodes: Optional[pulumi.Input[Sequence[pulumi.Input['ProviderSshNodeArgs']]]] = None,
-                 password: Optional[pulumi.Input[str]] = None,
-                 private_key: Optional[pulumi.Input[str]] = None,
-                 socks5_password: Optional[pulumi.Input[str]] = None,
-                 socks5_server: Optional[pulumi.Input[str]] = None,
-                 socks5_username: Optional[pulumi.Input[str]] = None,
-                 username: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[bool] agent: Whether to use the SSH agent for authentication. Takes precedence over the `private_key` and `password` fields. Defaults to the value of the `PROXMOX_VE_SSH_AGENT` environment variable, or `false` if not set.
-        :param pulumi.Input[str] agent_socket: The path to the SSH agent socket. Defaults to the value of the `SSH_AUTH_SOCK` environment variable.
-        :param pulumi.Input[Sequence[pulumi.Input['ProviderSshNodeArgs']]] nodes: Overrides for SSH connection configuration for a Proxmox VE node.
-        :param pulumi.Input[str] password: The password used for the SSH connection. Defaults to the value of the `password` field of the `provider` block.
-        :param pulumi.Input[str] private_key: The unencrypted private key (in PEM format) used for the SSH connection. Defaults to the value of the `PROXMOX_VE_SSH_PRIVATE_KEY` environment variable.
-        :param pulumi.Input[str] socks5_password: The password for the SOCKS5 proxy server. Defaults to the value of the `PROXMOX_VE_SSH_SOCKS5_PASSWORD` environment variable.
-        :param pulumi.Input[str] socks5_server: The address:port of the SOCKS5 proxy server. Defaults to the value of the `PROXMOX_VE_SSH_SOCKS5_SERVER` environment variable.
-        :param pulumi.Input[str] socks5_username: The username for the SOCKS5 proxy server. Defaults to the value of the `PROXMOX_VE_SSH_SOCKS5_USERNAME` environment variable.
-        :param pulumi.Input[str] username: The username used for the SSH connection. Defaults to the value of the `username` field of the `provider` block.
-        """
-        if agent is not None:
-            pulumi.set(__self__, "agent", agent)
-        if agent_socket is not None:
-            pulumi.set(__self__, "agent_socket", agent_socket)
-        if nodes is not None:
-            pulumi.set(__self__, "nodes", nodes)
-        if password is not None:
-            pulumi.set(__self__, "password", password)
-        if private_key is not None:
-            pulumi.set(__self__, "private_key", private_key)
-        if socks5_password is not None:
-            pulumi.set(__self__, "socks5_password", socks5_password)
-        if socks5_server is not None:
-            pulumi.set(__self__, "socks5_server", socks5_server)
-        if socks5_username is not None:
-            pulumi.set(__self__, "socks5_username", socks5_username)
-        if username is not None:
-            pulumi.set(__self__, "username", username)
+    @endpoint.setter
+    def endpoint(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "endpoint", value)
 
     @property
     @pulumi.getter
-    def agent(self) -> Optional[pulumi.Input[bool]]:
+    def insecure(self) -> Optional[pulumi.Input[bool]]:
         """
-        Whether to use the SSH agent for authentication. Takes precedence over the `private_key` and `password` fields. Defaults to the value of the `PROXMOX_VE_SSH_AGENT` environment variable, or `false` if not set.
+        Whether to skip the TLS verification step.
         """
-        return pulumi.get(self, "agent")
+        return pulumi.get(self, "insecure")
 
-    @agent.setter
-    def agent(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "agent", value)
+    @insecure.setter
+    def insecure(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "insecure", value)
 
     @property
-    @pulumi.getter(name="agentSocket")
-    def agent_socket(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="minTls")
+    def min_tls(self) -> Optional[pulumi.Input[str]]:
         """
-        The path to the SSH agent socket. Defaults to the value of the `SSH_AUTH_SOCK` environment variable.
+        The minimum required TLS version for API calls.Supported values: `1.0|1.1|1.2|1.3`. Defaults to `1.3`.
         """
-        return pulumi.get(self, "agent_socket")
+        return pulumi.get(self, "min_tls")
 
-    @agent_socket.setter
-    def agent_socket(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "agent_socket", value)
+    @min_tls.setter
+    def min_tls(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "min_tls", value)
 
     @property
     @pulumi.getter
-    def nodes(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ProviderSshNodeArgs']]]]:
+    def otp(self) -> Optional[pulumi.Input[str]]:
         """
-        Overrides for SSH connection configuration for a Proxmox VE node.
+        The one-time password for the Proxmox VE API.
         """
-        return pulumi.get(self, "nodes")
+        warnings.warn("""The `otp` attribute is deprecated and will be removed in a future release. Please use the `api_token` attribute instead.""", DeprecationWarning)
+        pulumi.log.warn("""otp is deprecated: The `otp` attribute is deprecated and will be removed in a future release. Please use the `api_token` attribute instead.""")
+
+        return pulumi.get(self, "otp")
 
-    @nodes.setter
-    def nodes(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ProviderSshNodeArgs']]]]):
-        pulumi.set(self, "nodes", value)
+    @otp.setter
+    def otp(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "otp", value)
 
     @property
     @pulumi.getter
     def password(self) -> Optional[pulumi.Input[str]]:
         """
-        The password used for the SSH connection. Defaults to the value of the `password` field of the `provider` block.
+        The password for the Proxmox VE API.
         """
         return pulumi.get(self, "password")
 
     @password.setter
     def password(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "password", value)
 
     @property
-    @pulumi.getter(name="privateKey")
-    def private_key(self) -> Optional[pulumi.Input[str]]:
-        """
-        The unencrypted private key (in PEM format) used for the SSH connection. Defaults to the value of the `PROXMOX_VE_SSH_PRIVATE_KEY` environment variable.
-        """
-        return pulumi.get(self, "private_key")
-
-    @private_key.setter
-    def private_key(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "private_key", value)
-
-    @property
-    @pulumi.getter(name="socks5Password")
-    def socks5_password(self) -> Optional[pulumi.Input[str]]:
-        """
-        The password for the SOCKS5 proxy server. Defaults to the value of the `PROXMOX_VE_SSH_SOCKS5_PASSWORD` environment variable.
-        """
-        return pulumi.get(self, "socks5_password")
-
-    @socks5_password.setter
-    def socks5_password(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "socks5_password", value)
-
-    @property
-    @pulumi.getter(name="socks5Server")
-    def socks5_server(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter
+    def ssh(self) -> Optional[pulumi.Input['ProviderSshArgs']]:
         """
-        The address:port of the SOCKS5 proxy server. Defaults to the value of the `PROXMOX_VE_SSH_SOCKS5_SERVER` environment variable.
+        The SSH configuration for the Proxmox nodes.
         """
-        return pulumi.get(self, "socks5_server")
+        return pulumi.get(self, "ssh")
 
-    @socks5_server.setter
-    def socks5_server(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "socks5_server", value)
+    @ssh.setter
+    def ssh(self, value: Optional[pulumi.Input['ProviderSshArgs']]):
+        pulumi.set(self, "ssh", value)
 
     @property
-    @pulumi.getter(name="socks5Username")
-    def socks5_username(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="tmpDir")
+    def tmp_dir(self) -> Optional[pulumi.Input[str]]:
         """
-        The username for the SOCKS5 proxy server. Defaults to the value of the `PROXMOX_VE_SSH_SOCKS5_USERNAME` environment variable.
+        The alternative temporary directory.
         """
-        return pulumi.get(self, "socks5_username")
+        return pulumi.get(self, "tmp_dir")
 
-    @socks5_username.setter
-    def socks5_username(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "socks5_username", value)
+    @tmp_dir.setter
+    def tmp_dir(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "tmp_dir", value)
 
     @property
     @pulumi.getter
     def username(self) -> Optional[pulumi.Input[str]]:
         """
-        The username used for the SSH connection. Defaults to the value of the `username` field of the `provider` block.
+        The username for the Proxmox VE API.
         """
         return pulumi.get(self, "username")
 
     @username.setter
     def username(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "username", value)
 
 
-@pulumi.input_type
-class ProviderSshNodeArgs:
-    def __init__(__self__, *,
-                 address: pulumi.Input[str],
-                 name: pulumi.Input[str],
-                 port: Optional[pulumi.Input[int]] = None):
-        """
-        :param pulumi.Input[str] address: The address of the Proxmox VE node.
-        :param pulumi.Input[str] name: The name of the Proxmox VE node.
-        :param pulumi.Input[int] port: The port of the Proxmox VE node.
-        """
-        pulumi.set(__self__, "address", address)
-        pulumi.set(__self__, "name", name)
-        if port is not None:
-            pulumi.set(__self__, "port", port)
-
-    @property
-    @pulumi.getter
-    def address(self) -> pulumi.Input[str]:
-        """
-        The address of the Proxmox VE node.
-        """
-        return pulumi.get(self, "address")
-
-    @address.setter
-    def address(self, value: pulumi.Input[str]):
-        pulumi.set(self, "address", value)
-
-    @property
-    @pulumi.getter
-    def name(self) -> pulumi.Input[str]:
-        """
-        The name of the Proxmox VE node.
-        """
-        return pulumi.get(self, "name")
+class Provider(pulumi.ProviderResource):
+    @overload
+    def __init__(__self__,
+                 resource_name: str,
+                 opts: Optional[pulumi.ResourceOptions] = None,
+                 api_token: Optional[pulumi.Input[str]] = None,
+                 endpoint: Optional[pulumi.Input[str]] = None,
+                 insecure: Optional[pulumi.Input[bool]] = None,
+                 min_tls: Optional[pulumi.Input[str]] = None,
+                 otp: Optional[pulumi.Input[str]] = None,
+                 password: Optional[pulumi.Input[str]] = None,
+                 ssh: Optional[pulumi.Input[pulumi.InputType['ProviderSshArgs']]] = None,
+                 tmp_dir: Optional[pulumi.Input[str]] = None,
+                 username: Optional[pulumi.Input[str]] = None,
+                 __props__=None):
+        """
+        The provider type for the proxmox package. By default, resources use package-wide configuration
+        settings, however an explicit `Provider` instance may be created and passed during resource
+        construction to achieve fine-grained programmatic control over provider settings. See the
+        [documentation](https://www.pulumi.com/docs/reference/programming-model/#providers) for more information.
+
+        :param str resource_name: The name of the resource.
+        :param pulumi.ResourceOptions opts: Options for the resource.
+        :param pulumi.Input[str] api_token: The API token for the Proxmox VE API.
+        :param pulumi.Input[str] endpoint: The endpoint for the Proxmox VE API.
+        :param pulumi.Input[bool] insecure: Whether to skip the TLS verification step.
+        :param pulumi.Input[str] min_tls: The minimum required TLS version for API calls.Supported values: `1.0|1.1|1.2|1.3`. Defaults to `1.3`.
+        :param pulumi.Input[str] otp: The one-time password for the Proxmox VE API.
+        :param pulumi.Input[str] password: The password for the Proxmox VE API.
+        :param pulumi.Input[pulumi.InputType['ProviderSshArgs']] ssh: The SSH configuration for the Proxmox nodes.
+        :param pulumi.Input[str] tmp_dir: The alternative temporary directory.
+        :param pulumi.Input[str] username: The username for the Proxmox VE API.
+        """
+        ...
+    @overload
+    def __init__(__self__,
+                 resource_name: str,
+                 args: Optional[ProviderArgs] = None,
+                 opts: Optional[pulumi.ResourceOptions] = None):
+        """
+        The provider type for the proxmox package. By default, resources use package-wide configuration
+        settings, however an explicit `Provider` instance may be created and passed during resource
+        construction to achieve fine-grained programmatic control over provider settings. See the
+        [documentation](https://www.pulumi.com/docs/reference/programming-model/#providers) for more information.
+
+        :param str resource_name: The name of the resource.
+        :param ProviderArgs args: The arguments to use to populate this resource's properties.
+        :param pulumi.ResourceOptions opts: Options for the resource.
+        """
+        ...
+    def __init__(__self__, resource_name: str, *args, **kwargs):
+        resource_args, opts = _utilities.get_resource_args_opts(ProviderArgs, pulumi.ResourceOptions, *args, **kwargs)
+        if resource_args is not None:
+            __self__._internal_init(resource_name, opts, **resource_args.__dict__)
+        else:
+            __self__._internal_init(resource_name, *args, **kwargs)
+
+    def _internal_init(__self__,
+                 resource_name: str,
+                 opts: Optional[pulumi.ResourceOptions] = None,
+                 api_token: Optional[pulumi.Input[str]] = None,
+                 endpoint: Optional[pulumi.Input[str]] = None,
+                 insecure: Optional[pulumi.Input[bool]] = None,
+                 min_tls: Optional[pulumi.Input[str]] = None,
+                 otp: Optional[pulumi.Input[str]] = None,
+                 password: Optional[pulumi.Input[str]] = None,
+                 ssh: Optional[pulumi.Input[pulumi.InputType['ProviderSshArgs']]] = None,
+                 tmp_dir: Optional[pulumi.Input[str]] = None,
+                 username: Optional[pulumi.Input[str]] = None,
+                 __props__=None):
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
+        if not isinstance(opts, pulumi.ResourceOptions):
+            raise TypeError('Expected resource options to be a ResourceOptions instance')
+        if opts.id is None:
+            if __props__ is not None:
+                raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
+            __props__ = ProviderArgs.__new__(ProviderArgs)
 
-    @name.setter
-    def name(self, value: pulumi.Input[str]):
-        pulumi.set(self, "name", value)
+            __props__.__dict__["api_token"] = None if api_token is None else pulumi.Output.secret(api_token)
+            __props__.__dict__["endpoint"] = endpoint
+            __props__.__dict__["insecure"] = pulumi.Output.from_input(insecure).apply(pulumi.runtime.to_json) if insecure is not None else None
+            __props__.__dict__["min_tls"] = min_tls
+            __props__.__dict__["otp"] = otp
+            __props__.__dict__["password"] = None if password is None else pulumi.Output.secret(password)
+            __props__.__dict__["ssh"] = pulumi.Output.from_input(ssh).apply(pulumi.runtime.to_json) if ssh is not None else None
+            __props__.__dict__["tmp_dir"] = tmp_dir
+            __props__.__dict__["username"] = username
+        secret_opts = pulumi.ResourceOptions(additional_secret_outputs=["apiToken", "password"])
+        opts = pulumi.ResourceOptions.merge(opts, secret_opts)
+        super(Provider, __self__).__init__(
+            'proxmoxve',
+            resource_name,
+            __props__,
+            opts)
 
     @property
-    @pulumi.getter
-    def port(self) -> Optional[pulumi.Input[int]]:
-        """
-        The port of the Proxmox VE node.
-        """
-        return pulumi.get(self, "port")
-
-    @port.setter
-    def port(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "port", value)
-
-
-@pulumi.input_type
-class Vm2CloneArgs:
-    def __init__(__self__, *,
-                 id: pulumi.Input[int],
-                 retries: Optional[pulumi.Input[int]] = None):
+    @pulumi.getter(name="apiToken")
+    def api_token(self) -> pulumi.Output[Optional[str]]:
         """
-        :param pulumi.Input[int] id: The ID of the VM to clone.
-        :param pulumi.Input[int] retries: The number of retries to perform when cloning the VM (default: 3).
+        The API token for the Proxmox VE API.
         """
-        pulumi.set(__self__, "id", id)
-        if retries is not None:
-            pulumi.set(__self__, "retries", retries)
+        return pulumi.get(self, "api_token")
 
     @property
     @pulumi.getter
-    def id(self) -> pulumi.Input[int]:
+    def endpoint(self) -> pulumi.Output[Optional[str]]:
         """
-        The ID of the VM to clone.
+        The endpoint for the Proxmox VE API.
         """
-        return pulumi.get(self, "id")
-
-    @id.setter
-    def id(self, value: pulumi.Input[int]):
-        pulumi.set(self, "id", value)
+        return pulumi.get(self, "endpoint")
 
     @property
-    @pulumi.getter
-    def retries(self) -> Optional[pulumi.Input[int]]:
+    @pulumi.getter(name="minTls")
+    def min_tls(self) -> pulumi.Output[Optional[str]]:
         """
-        The number of retries to perform when cloning the VM (default: 3).
+        The minimum required TLS version for API calls.Supported values: `1.0|1.1|1.2|1.3`. Defaults to `1.3`.
         """
-        return pulumi.get(self, "retries")
-
-    @retries.setter
-    def retries(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "retries", value)
-
-
-@pulumi.input_type
-class Vm2TimeoutsArgs:
-    def __init__(__self__, *,
-                 create: Optional[pulumi.Input[str]] = None,
-                 delete: Optional[pulumi.Input[str]] = None,
-                 read: Optional[pulumi.Input[str]] = None,
-                 update: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] create: A string that can be [parsed as a duration](https://pkg.go.dev/time#ParseDuration) consisting of numbers and unit suffixes, such as "30s" or "2h45m". Valid time units are "s" (seconds), "m" (minutes), "h" (hours).
-        :param pulumi.Input[str] delete: A string that can be [parsed as a duration](https://pkg.go.dev/time#ParseDuration) consisting of numbers and unit suffixes, such as "30s" or "2h45m". Valid time units are "s" (seconds), "m" (minutes), "h" (hours). Setting a timeout for a Delete operation is only applicable if changes are saved into state before the destroy operation occurs.
-        :param pulumi.Input[str] read: A string that can be [parsed as a duration](https://pkg.go.dev/time#ParseDuration) consisting of numbers and unit suffixes, such as "30s" or "2h45m". Valid time units are "s" (seconds), "m" (minutes), "h" (hours). Read operations occur during any refresh or planning operation when refresh is enabled.
-        :param pulumi.Input[str] update: A string that can be [parsed as a duration](https://pkg.go.dev/time#ParseDuration) consisting of numbers and unit suffixes, such as "30s" or "2h45m". Valid time units are "s" (seconds), "m" (minutes), "h" (hours).
-        """
-        if create is not None:
-            pulumi.set(__self__, "create", create)
-        if delete is not None:
-            pulumi.set(__self__, "delete", delete)
-        if read is not None:
-            pulumi.set(__self__, "read", read)
-        if update is not None:
-            pulumi.set(__self__, "update", update)
+        return pulumi.get(self, "min_tls")
 
     @property
     @pulumi.getter
-    def create(self) -> Optional[pulumi.Input[str]]:
+    def otp(self) -> pulumi.Output[Optional[str]]:
         """
-        A string that can be [parsed as a duration](https://pkg.go.dev/time#ParseDuration) consisting of numbers and unit suffixes, such as "30s" or "2h45m". Valid time units are "s" (seconds), "m" (minutes), "h" (hours).
+        The one-time password for the Proxmox VE API.
         """
-        return pulumi.get(self, "create")
+        warnings.warn("""The `otp` attribute is deprecated and will be removed in a future release. Please use the `api_token` attribute instead.""", DeprecationWarning)
+        pulumi.log.warn("""otp is deprecated: The `otp` attribute is deprecated and will be removed in a future release. Please use the `api_token` attribute instead.""")
 
-    @create.setter
-    def create(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "create", value)
+        return pulumi.get(self, "otp")
 
     @property
     @pulumi.getter
-    def delete(self) -> Optional[pulumi.Input[str]]:
+    def password(self) -> pulumi.Output[Optional[str]]:
         """
-        A string that can be [parsed as a duration](https://pkg.go.dev/time#ParseDuration) consisting of numbers and unit suffixes, such as "30s" or "2h45m". Valid time units are "s" (seconds), "m" (minutes), "h" (hours). Setting a timeout for a Delete operation is only applicable if changes are saved into state before the destroy operation occurs.
+        The password for the Proxmox VE API.
         """
-        return pulumi.get(self, "delete")
-
-    @delete.setter
-    def delete(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "delete", value)
+        return pulumi.get(self, "password")
 
     @property
-    @pulumi.getter
-    def read(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="tmpDir")
+    def tmp_dir(self) -> pulumi.Output[Optional[str]]:
         """
-        A string that can be [parsed as a duration](https://pkg.go.dev/time#ParseDuration) consisting of numbers and unit suffixes, such as "30s" or "2h45m". Valid time units are "s" (seconds), "m" (minutes), "h" (hours). Read operations occur during any refresh or planning operation when refresh is enabled.
+        The alternative temporary directory.
         """
-        return pulumi.get(self, "read")
-
-    @read.setter
-    def read(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "read", value)
+        return pulumi.get(self, "tmp_dir")
 
     @property
     @pulumi.getter
-    def update(self) -> Optional[pulumi.Input[str]]:
+    def username(self) -> pulumi.Output[Optional[str]]:
         """
-        A string that can be [parsed as a duration](https://pkg.go.dev/time#ParseDuration) consisting of numbers and unit suffixes, such as "30s" or "2h45m". Valid time units are "s" (seconds), "m" (minutes), "h" (hours).
+        The username for the Proxmox VE API.
         """
-        return pulumi.get(self, "update")
-
-    @update.setter
-    def update(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "update", value)
-
+        return pulumi.get(self, "username")
```

### Comparing `pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/_utilities.py` & `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/acl.py` & `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/acl.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/certifi.py` & `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/certifi.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/cluster/_inputs.py` & `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/cluster/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/cluster/get_nodes.py` & `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/cluster/get_nodes.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/cluster/options.py` & `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/cluster/options.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/cluster/outputs.py` & `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/cluster/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/config/outputs.py` & `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/config/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/config/vars.py` & `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/ct/_inputs.py` & `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/ct/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/ct/container.py` & `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/ct/container.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/ct/outputs.py` & `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/ct/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/dns.py` & `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/dns.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/download/file.py` & `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/download/file.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/get_node.py` & `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/get_node.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/ha/get_ha_group.py` & `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/ha/get_ha_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/ha/get_ha_groups.py` & `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/ha/get_ha_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/ha/get_ha_resource.py` & `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/ha/get_ha_resource.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/ha/get_ha_resources.py` & `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/ha/get_ha_resources.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/ha/ha_group.py` & `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/ha/ha_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/ha/ha_resource.py` & `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/ha/ha_resource.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/hardware/__init__.py` & `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/hardware/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/hardware/get_mappings.py` & `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/hardware/get_mappings.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/hardware/mapping/_inputs.py` & `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/hardware/mapping/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/hardware/mapping/get_pci.py` & `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/hardware/mapping/get_pci.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/hardware/mapping/get_usb.py` & `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/hardware/mapping/get_usb.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/hardware/mapping/outputs.py` & `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/hardware/mapping/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/hardware/mapping/pci.py` & `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/hardware/mapping/pci.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/hardware/mapping/usb.py` & `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/hardware/mapping/usb.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/hardware/outputs.py` & `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/hardware/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/hosts.py` & `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/hosts.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/network/__init__.py` & `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/network/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/network/_inputs.py` & `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/network/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/network/firewall.py` & `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/network/firewall.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/network/firewall_alias.py` & `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/network/firewall_alias.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/network/firewall_ip_set.py` & `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/network/firewall_ip_set.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/network/firewall_options.py` & `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/network/firewall_options.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/network/firewall_rules.py` & `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/network/firewall_rules.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/network/firewall_security_group.py` & `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/network/firewall_security_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/network/get_dns.py` & `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/network/get_dns.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/network/get_hosts.py` & `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/network/get_hosts.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/network/get_time.py` & `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/network/get_time.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/network/get_version.py` & `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/network/get_version.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/network/network_bridge.py` & `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/network/network_bridge.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/network/network_vlan.py` & `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/network/network_vlan.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/network/outputs.py` & `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/network/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/permission/__init__.py` & `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/permission/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/permission/_inputs.py` & `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/permission/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/permission/get_group.py` & `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/permission/get_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/permission/get_groups.py` & `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/permission/get_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/permission/get_pool.py` & `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/permission/get_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/permission/get_pools.py` & `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/permission/get_pools.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/permission/get_role.py` & `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/permission/get_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/permission/get_roles.py` & `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/permission/get_roles.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/permission/get_user.py` & `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/permission/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/permission/get_users.py` & `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/permission/get_users.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/permission/group.py` & `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/permission/group.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/permission/outputs.py` & `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/permission/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/permission/pool.py` & `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/permission/pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/permission/role.py` & `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/permission/role.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/permission/user.py` & `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/permission/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/provider.py` & `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/user/token.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,324 +3,423 @@
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
-from . import _utilities
-from ._inputs import *
+from .. import _utilities
 
-__all__ = ['ProviderArgs', 'Provider']
+__all__ = ['TokenArgs', 'Token']
 
 @pulumi.input_type
-class ProviderArgs:
+class TokenArgs:
     def __init__(__self__, *,
-                 api_token: Optional[pulumi.Input[str]] = None,
-                 endpoint: Optional[pulumi.Input[str]] = None,
-                 insecure: Optional[pulumi.Input[bool]] = None,
-                 min_tls: Optional[pulumi.Input[str]] = None,
-                 otp: Optional[pulumi.Input[str]] = None,
-                 password: Optional[pulumi.Input[str]] = None,
-                 ssh: Optional[pulumi.Input['ProviderSshArgs']] = None,
-                 tmp_dir: Optional[pulumi.Input[str]] = None,
-                 username: Optional[pulumi.Input[str]] = None):
-        """
-        The set of arguments for constructing a Provider resource.
-        :param pulumi.Input[str] api_token: The API token for the Proxmox VE API.
-        :param pulumi.Input[str] endpoint: The endpoint for the Proxmox VE API.
-        :param pulumi.Input[bool] insecure: Whether to skip the TLS verification step.
-        :param pulumi.Input[str] min_tls: The minimum required TLS version for API calls.Supported values: `1.0|1.1|1.2|1.3`. Defaults to `1.3`.
-        :param pulumi.Input[str] otp: The one-time password for the Proxmox VE API.
-        :param pulumi.Input[str] password: The password for the Proxmox VE API.
-        :param pulumi.Input['ProviderSshArgs'] ssh: The SSH configuration for the Proxmox nodes.
-        :param pulumi.Input[str] tmp_dir: The alternative temporary directory.
-        :param pulumi.Input[str] username: The username for the Proxmox VE API.
-        """
-        if api_token is not None:
-            pulumi.set(__self__, "api_token", api_token)
-        if endpoint is not None:
-            pulumi.set(__self__, "endpoint", endpoint)
-        if insecure is not None:
-            pulumi.set(__self__, "insecure", insecure)
-        if min_tls is not None:
-            pulumi.set(__self__, "min_tls", min_tls)
-        if otp is not None:
-            warnings.warn("""The `otp` attribute is deprecated and will be removed in a future release. Please use the `api_token` attribute instead.""", DeprecationWarning)
-            pulumi.log.warn("""otp is deprecated: The `otp` attribute is deprecated and will be removed in a future release. Please use the `api_token` attribute instead.""")
-        if otp is not None:
-            pulumi.set(__self__, "otp", otp)
-        if password is not None:
-            pulumi.set(__self__, "password", password)
-        if ssh is not None:
-            pulumi.set(__self__, "ssh", ssh)
-        if tmp_dir is not None:
-            pulumi.set(__self__, "tmp_dir", tmp_dir)
-        if username is not None:
-            pulumi.set(__self__, "username", username)
-
-    @property
-    @pulumi.getter(name="apiToken")
-    def api_token(self) -> Optional[pulumi.Input[str]]:
-        """
-        The API token for the Proxmox VE API.
-        """
-        return pulumi.get(self, "api_token")
-
-    @api_token.setter
-    def api_token(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "api_token", value)
+                 token_name: pulumi.Input[str],
+                 user_id: pulumi.Input[str],
+                 comment: Optional[pulumi.Input[str]] = None,
+                 expiration_date: Optional[pulumi.Input[str]] = None,
+                 privileges_separation: Optional[pulumi.Input[bool]] = None):
+        """
+        The set of arguments for constructing a Token resource.
+        :param pulumi.Input[str] token_name: User-specific token identifier.
+        :param pulumi.Input[str] user_id: User identifier.
+        :param pulumi.Input[str] comment: Comment for the token.
+        :param pulumi.Input[str] expiration_date: Expiration date for the token.
+        :param pulumi.Input[bool] privileges_separation: Restrict API token privileges with separate ACLs (default), or give full privileges of corresponding user.
+        """
+        pulumi.set(__self__, "token_name", token_name)
+        pulumi.set(__self__, "user_id", user_id)
+        if comment is not None:
+            pulumi.set(__self__, "comment", comment)
+        if expiration_date is not None:
+            pulumi.set(__self__, "expiration_date", expiration_date)
+        if privileges_separation is not None:
+            pulumi.set(__self__, "privileges_separation", privileges_separation)
 
     @property
-    @pulumi.getter
-    def endpoint(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="tokenName")
+    def token_name(self) -> pulumi.Input[str]:
         """
-        The endpoint for the Proxmox VE API.
+        User-specific token identifier.
         """
-        return pulumi.get(self, "endpoint")
+        return pulumi.get(self, "token_name")
 
-    @endpoint.setter
-    def endpoint(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "endpoint", value)
+    @token_name.setter
+    def token_name(self, value: pulumi.Input[str]):
+        pulumi.set(self, "token_name", value)
+
+    @property
+    @pulumi.getter(name="userId")
+    def user_id(self) -> pulumi.Input[str]:
+        """
+        User identifier.
+        """
+        return pulumi.get(self, "user_id")
+
+    @user_id.setter
+    def user_id(self, value: pulumi.Input[str]):
+        pulumi.set(self, "user_id", value)
 
     @property
     @pulumi.getter
-    def insecure(self) -> Optional[pulumi.Input[bool]]:
+    def comment(self) -> Optional[pulumi.Input[str]]:
         """
-        Whether to skip the TLS verification step.
+        Comment for the token.
         """
-        return pulumi.get(self, "insecure")
+        return pulumi.get(self, "comment")
 
-    @insecure.setter
-    def insecure(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "insecure", value)
+    @comment.setter
+    def comment(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "comment", value)
 
     @property
-    @pulumi.getter(name="minTls")
-    def min_tls(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="expirationDate")
+    def expiration_date(self) -> Optional[pulumi.Input[str]]:
         """
-        The minimum required TLS version for API calls.Supported values: `1.0|1.1|1.2|1.3`. Defaults to `1.3`.
+        Expiration date for the token.
         """
-        return pulumi.get(self, "min_tls")
+        return pulumi.get(self, "expiration_date")
 
-    @min_tls.setter
-    def min_tls(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "min_tls", value)
+    @expiration_date.setter
+    def expiration_date(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "expiration_date", value)
 
     @property
-    @pulumi.getter
-    def otp(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="privilegesSeparation")
+    def privileges_separation(self) -> Optional[pulumi.Input[bool]]:
         """
-        The one-time password for the Proxmox VE API.
+        Restrict API token privileges with separate ACLs (default), or give full privileges of corresponding user.
         """
-        warnings.warn("""The `otp` attribute is deprecated and will be removed in a future release. Please use the `api_token` attribute instead.""", DeprecationWarning)
-        pulumi.log.warn("""otp is deprecated: The `otp` attribute is deprecated and will be removed in a future release. Please use the `api_token` attribute instead.""")
+        return pulumi.get(self, "privileges_separation")
 
-        return pulumi.get(self, "otp")
+    @privileges_separation.setter
+    def privileges_separation(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "privileges_separation", value)
 
-    @otp.setter
-    def otp(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "otp", value)
+
+@pulumi.input_type
+class _TokenState:
+    def __init__(__self__, *,
+                 comment: Optional[pulumi.Input[str]] = None,
+                 expiration_date: Optional[pulumi.Input[str]] = None,
+                 privileges_separation: Optional[pulumi.Input[bool]] = None,
+                 token_name: Optional[pulumi.Input[str]] = None,
+                 user_id: Optional[pulumi.Input[str]] = None,
+                 value: Optional[pulumi.Input[str]] = None):
+        """
+        Input properties used for looking up and filtering Token resources.
+        :param pulumi.Input[str] comment: Comment for the token.
+        :param pulumi.Input[str] expiration_date: Expiration date for the token.
+        :param pulumi.Input[bool] privileges_separation: Restrict API token privileges with separate ACLs (default), or give full privileges of corresponding user.
+        :param pulumi.Input[str] token_name: User-specific token identifier.
+        :param pulumi.Input[str] user_id: User identifier.
+        :param pulumi.Input[str] value: API token value used for authentication. It is populated only when creating a new token, and can't be retrieved at import.
+        """
+        if comment is not None:
+            pulumi.set(__self__, "comment", comment)
+        if expiration_date is not None:
+            pulumi.set(__self__, "expiration_date", expiration_date)
+        if privileges_separation is not None:
+            pulumi.set(__self__, "privileges_separation", privileges_separation)
+        if token_name is not None:
+            pulumi.set(__self__, "token_name", token_name)
+        if user_id is not None:
+            pulumi.set(__self__, "user_id", user_id)
+        if value is not None:
+            pulumi.set(__self__, "value", value)
 
     @property
     @pulumi.getter
-    def password(self) -> Optional[pulumi.Input[str]]:
+    def comment(self) -> Optional[pulumi.Input[str]]:
         """
-        The password for the Proxmox VE API.
+        Comment for the token.
         """
-        return pulumi.get(self, "password")
+        return pulumi.get(self, "comment")
 
-    @password.setter
-    def password(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "password", value)
+    @comment.setter
+    def comment(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "comment", value)
 
     @property
-    @pulumi.getter
-    def ssh(self) -> Optional[pulumi.Input['ProviderSshArgs']]:
+    @pulumi.getter(name="expirationDate")
+    def expiration_date(self) -> Optional[pulumi.Input[str]]:
+        """
+        Expiration date for the token.
+        """
+        return pulumi.get(self, "expiration_date")
+
+    @expiration_date.setter
+    def expiration_date(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "expiration_date", value)
+
+    @property
+    @pulumi.getter(name="privilegesSeparation")
+    def privileges_separation(self) -> Optional[pulumi.Input[bool]]:
         """
-        The SSH configuration for the Proxmox nodes.
+        Restrict API token privileges with separate ACLs (default), or give full privileges of corresponding user.
         """
-        return pulumi.get(self, "ssh")
+        return pulumi.get(self, "privileges_separation")
 
-    @ssh.setter
-    def ssh(self, value: Optional[pulumi.Input['ProviderSshArgs']]):
-        pulumi.set(self, "ssh", value)
+    @privileges_separation.setter
+    def privileges_separation(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "privileges_separation", value)
 
     @property
-    @pulumi.getter(name="tmpDir")
-    def tmp_dir(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="tokenName")
+    def token_name(self) -> Optional[pulumi.Input[str]]:
         """
-        The alternative temporary directory.
+        User-specific token identifier.
         """
-        return pulumi.get(self, "tmp_dir")
+        return pulumi.get(self, "token_name")
 
-    @tmp_dir.setter
-    def tmp_dir(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "tmp_dir", value)
+    @token_name.setter
+    def token_name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "token_name", value)
+
+    @property
+    @pulumi.getter(name="userId")
+    def user_id(self) -> Optional[pulumi.Input[str]]:
+        """
+        User identifier.
+        """
+        return pulumi.get(self, "user_id")
+
+    @user_id.setter
+    def user_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "user_id", value)
 
     @property
     @pulumi.getter
-    def username(self) -> Optional[pulumi.Input[str]]:
+    def value(self) -> Optional[pulumi.Input[str]]:
         """
-        The username for the Proxmox VE API.
+        API token value used for authentication. It is populated only when creating a new token, and can't be retrieved at import.
         """
-        return pulumi.get(self, "username")
+        return pulumi.get(self, "value")
 
-    @username.setter
-    def username(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "username", value)
+    @value.setter
+    def value(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "value", value)
 
 
-class Provider(pulumi.ProviderResource):
+class Token(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 api_token: Optional[pulumi.Input[str]] = None,
-                 endpoint: Optional[pulumi.Input[str]] = None,
-                 insecure: Optional[pulumi.Input[bool]] = None,
-                 min_tls: Optional[pulumi.Input[str]] = None,
-                 otp: Optional[pulumi.Input[str]] = None,
-                 password: Optional[pulumi.Input[str]] = None,
-                 ssh: Optional[pulumi.Input[pulumi.InputType['ProviderSshArgs']]] = None,
-                 tmp_dir: Optional[pulumi.Input[str]] = None,
-                 username: Optional[pulumi.Input[str]] = None,
+                 comment: Optional[pulumi.Input[str]] = None,
+                 expiration_date: Optional[pulumi.Input[str]] = None,
+                 privileges_separation: Optional[pulumi.Input[bool]] = None,
+                 token_name: Optional[pulumi.Input[str]] = None,
+                 user_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        The provider type for the proxmox package. By default, resources use package-wide configuration
-        settings, however an explicit `Provider` instance may be created and passed during resource
-        construction to achieve fine-grained programmatic control over provider settings. See the
-        [documentation](https://www.pulumi.com/docs/reference/programming-model/#providers) for more information.
+        User API tokens.
+
+        ## Example Usage
+
+        ```python
+        import pulumi
+        import pulumi_proxmoxve as proxmoxve
+
+        # if creating a user token, the user must be created first
+        user = proxmoxve.permission.User("user",
+            comment="Managed by Terraform",
+            email="user@pve",
+            enabled=True,
+            expiration_date="2034-01-01T22:00:00Z",
+            user_id="user@pve")
+        user_token = proxmoxve.user.Token("userToken",
+            comment="Managed by Terraform",
+            expiration_date="2033-01-01T22:00:00Z",
+            token_name="tk1",
+            user_id=user.user_id)
+        ```
+
+        ## Import
+
+        #!/usr/bin/env sh
+
+        #Tokens can be imported using they identifiers in format `user_id!token_name` format, e.g.:
+
+        ```sh
+        $ pulumi import proxmoxve:User/token:Token token1 user@pve!token1
+        ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] api_token: The API token for the Proxmox VE API.
-        :param pulumi.Input[str] endpoint: The endpoint for the Proxmox VE API.
-        :param pulumi.Input[bool] insecure: Whether to skip the TLS verification step.
-        :param pulumi.Input[str] min_tls: The minimum required TLS version for API calls.Supported values: `1.0|1.1|1.2|1.3`. Defaults to `1.3`.
-        :param pulumi.Input[str] otp: The one-time password for the Proxmox VE API.
-        :param pulumi.Input[str] password: The password for the Proxmox VE API.
-        :param pulumi.Input[pulumi.InputType['ProviderSshArgs']] ssh: The SSH configuration for the Proxmox nodes.
-        :param pulumi.Input[str] tmp_dir: The alternative temporary directory.
-        :param pulumi.Input[str] username: The username for the Proxmox VE API.
+        :param pulumi.Input[str] comment: Comment for the token.
+        :param pulumi.Input[str] expiration_date: Expiration date for the token.
+        :param pulumi.Input[bool] privileges_separation: Restrict API token privileges with separate ACLs (default), or give full privileges of corresponding user.
+        :param pulumi.Input[str] token_name: User-specific token identifier.
+        :param pulumi.Input[str] user_id: User identifier.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: Optional[ProviderArgs] = None,
+                 args: TokenArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        The provider type for the proxmox package. By default, resources use package-wide configuration
-        settings, however an explicit `Provider` instance may be created and passed during resource
-        construction to achieve fine-grained programmatic control over provider settings. See the
-        [documentation](https://www.pulumi.com/docs/reference/programming-model/#providers) for more information.
+        User API tokens.
+
+        ## Example Usage
+
+        ```python
+        import pulumi
+        import pulumi_proxmoxve as proxmoxve
+
+        # if creating a user token, the user must be created first
+        user = proxmoxve.permission.User("user",
+            comment="Managed by Terraform",
+            email="user@pve",
+            enabled=True,
+            expiration_date="2034-01-01T22:00:00Z",
+            user_id="user@pve")
+        user_token = proxmoxve.user.Token("userToken",
+            comment="Managed by Terraform",
+            expiration_date="2033-01-01T22:00:00Z",
+            token_name="tk1",
+            user_id=user.user_id)
+        ```
+
+        ## Import
+
+        #!/usr/bin/env sh
+
+        #Tokens can be imported using they identifiers in format `user_id!token_name` format, e.g.:
+
+        ```sh
+        $ pulumi import proxmoxve:User/token:Token token1 user@pve!token1
+        ```
 
         :param str resource_name: The name of the resource.
-        :param ProviderArgs args: The arguments to use to populate this resource's properties.
+        :param TokenArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(ProviderArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(TokenArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 api_token: Optional[pulumi.Input[str]] = None,
-                 endpoint: Optional[pulumi.Input[str]] = None,
-                 insecure: Optional[pulumi.Input[bool]] = None,
-                 min_tls: Optional[pulumi.Input[str]] = None,
-                 otp: Optional[pulumi.Input[str]] = None,
-                 password: Optional[pulumi.Input[str]] = None,
-                 ssh: Optional[pulumi.Input[pulumi.InputType['ProviderSshArgs']]] = None,
-                 tmp_dir: Optional[pulumi.Input[str]] = None,
-                 username: Optional[pulumi.Input[str]] = None,
+                 comment: Optional[pulumi.Input[str]] = None,
+                 expiration_date: Optional[pulumi.Input[str]] = None,
+                 privileges_separation: Optional[pulumi.Input[bool]] = None,
+                 token_name: Optional[pulumi.Input[str]] = None,
+                 user_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = ProviderArgs.__new__(ProviderArgs)
+            __props__ = TokenArgs.__new__(TokenArgs)
 
-            __props__.__dict__["api_token"] = None if api_token is None else pulumi.Output.secret(api_token)
-            __props__.__dict__["endpoint"] = endpoint
-            __props__.__dict__["insecure"] = pulumi.Output.from_input(insecure).apply(pulumi.runtime.to_json) if insecure is not None else None
-            __props__.__dict__["min_tls"] = min_tls
-            __props__.__dict__["otp"] = otp
-            __props__.__dict__["password"] = None if password is None else pulumi.Output.secret(password)
-            __props__.__dict__["ssh"] = pulumi.Output.from_input(ssh).apply(pulumi.runtime.to_json) if ssh is not None else None
-            __props__.__dict__["tmp_dir"] = tmp_dir
-            __props__.__dict__["username"] = username
-        secret_opts = pulumi.ResourceOptions(additional_secret_outputs=["apiToken", "password"])
+            __props__.__dict__["comment"] = comment
+            __props__.__dict__["expiration_date"] = expiration_date
+            __props__.__dict__["privileges_separation"] = privileges_separation
+            if token_name is None and not opts.urn:
+                raise TypeError("Missing required property 'token_name'")
+            __props__.__dict__["token_name"] = token_name
+            if user_id is None and not opts.urn:
+                raise TypeError("Missing required property 'user_id'")
+            __props__.__dict__["user_id"] = user_id
+            __props__.__dict__["value"] = None
+        secret_opts = pulumi.ResourceOptions(additional_secret_outputs=["value"])
         opts = pulumi.ResourceOptions.merge(opts, secret_opts)
-        super(Provider, __self__).__init__(
-            'proxmoxve',
+        super(Token, __self__).__init__(
+            'proxmoxve:User/token:Token',
             resource_name,
             __props__,
             opts)
 
-    @property
-    @pulumi.getter(name="apiToken")
-    def api_token(self) -> pulumi.Output[Optional[str]]:
+    @staticmethod
+    def get(resource_name: str,
+            id: pulumi.Input[str],
+            opts: Optional[pulumi.ResourceOptions] = None,
+            comment: Optional[pulumi.Input[str]] = None,
+            expiration_date: Optional[pulumi.Input[str]] = None,
+            privileges_separation: Optional[pulumi.Input[bool]] = None,
+            token_name: Optional[pulumi.Input[str]] = None,
+            user_id: Optional[pulumi.Input[str]] = None,
+            value: Optional[pulumi.Input[str]] = None) -> 'Token':
         """
-        The API token for the Proxmox VE API.
-        """
-        return pulumi.get(self, "api_token")
+        Get an existing Token resource's state with the given name, id, and optional extra
+        properties used to qualify the lookup.
+
+        :param str resource_name: The unique name of the resulting resource.
+        :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
+        :param pulumi.ResourceOptions opts: Options for the resource.
+        :param pulumi.Input[str] comment: Comment for the token.
+        :param pulumi.Input[str] expiration_date: Expiration date for the token.
+        :param pulumi.Input[bool] privileges_separation: Restrict API token privileges with separate ACLs (default), or give full privileges of corresponding user.
+        :param pulumi.Input[str] token_name: User-specific token identifier.
+        :param pulumi.Input[str] user_id: User identifier.
+        :param pulumi.Input[str] value: API token value used for authentication. It is populated only when creating a new token, and can't be retrieved at import.
+        """
+        opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
+
+        __props__ = _TokenState.__new__(_TokenState)
+
+        __props__.__dict__["comment"] = comment
+        __props__.__dict__["expiration_date"] = expiration_date
+        __props__.__dict__["privileges_separation"] = privileges_separation
+        __props__.__dict__["token_name"] = token_name
+        __props__.__dict__["user_id"] = user_id
+        __props__.__dict__["value"] = value
+        return Token(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
-    def endpoint(self) -> pulumi.Output[Optional[str]]:
+    def comment(self) -> pulumi.Output[Optional[str]]:
         """
-        The endpoint for the Proxmox VE API.
+        Comment for the token.
         """
-        return pulumi.get(self, "endpoint")
+        return pulumi.get(self, "comment")
 
     @property
-    @pulumi.getter(name="minTls")
-    def min_tls(self) -> pulumi.Output[Optional[str]]:
+    @pulumi.getter(name="expirationDate")
+    def expiration_date(self) -> pulumi.Output[Optional[str]]:
         """
-        The minimum required TLS version for API calls.Supported values: `1.0|1.1|1.2|1.3`. Defaults to `1.3`.
+        Expiration date for the token.
         """
-        return pulumi.get(self, "min_tls")
+        return pulumi.get(self, "expiration_date")
 
     @property
-    @pulumi.getter
-    def otp(self) -> pulumi.Output[Optional[str]]:
+    @pulumi.getter(name="privilegesSeparation")
+    def privileges_separation(self) -> pulumi.Output[bool]:
         """
-        The one-time password for the Proxmox VE API.
+        Restrict API token privileges with separate ACLs (default), or give full privileges of corresponding user.
         """
-        warnings.warn("""The `otp` attribute is deprecated and will be removed in a future release. Please use the `api_token` attribute instead.""", DeprecationWarning)
-        pulumi.log.warn("""otp is deprecated: The `otp` attribute is deprecated and will be removed in a future release. Please use the `api_token` attribute instead.""")
-
-        return pulumi.get(self, "otp")
+        return pulumi.get(self, "privileges_separation")
 
     @property
-    @pulumi.getter
-    def password(self) -> pulumi.Output[Optional[str]]:
+    @pulumi.getter(name="tokenName")
+    def token_name(self) -> pulumi.Output[str]:
         """
-        The password for the Proxmox VE API.
+        User-specific token identifier.
         """
-        return pulumi.get(self, "password")
+        return pulumi.get(self, "token_name")
 
     @property
-    @pulumi.getter(name="tmpDir")
-    def tmp_dir(self) -> pulumi.Output[Optional[str]]:
+    @pulumi.getter(name="userId")
+    def user_id(self) -> pulumi.Output[str]:
         """
-        The alternative temporary directory.
+        User identifier.
         """
-        return pulumi.get(self, "tmp_dir")
+        return pulumi.get(self, "user_id")
 
     @property
     @pulumi.getter
-    def username(self) -> pulumi.Output[Optional[str]]:
+    def value(self) -> pulumi.Output[str]:
         """
-        The username for the Proxmox VE API.
+        API token value used for authentication. It is populated only when creating a new token, and can't be retrieved at import.
         """
-        return pulumi.get(self, "username")
+        return pulumi.get(self, "value")
```

### Comparing `pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/storage/_inputs.py` & `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/storage/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/storage/file.py` & `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/storage/file.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/storage/get_datastores.py` & `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/storage/get_datastores.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/storage/outputs.py` & `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/storage/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/time.py` & `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/time.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/user/token.py` & `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/vm2.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,423 +3,478 @@
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
-from .. import _utilities
+from . import _utilities
+from . import outputs
+from ._inputs import *
 
-__all__ = ['TokenArgs', 'Token']
+__all__ = ['Vm2Args', 'Vm2']
 
 @pulumi.input_type
-class TokenArgs:
+class Vm2Args:
     def __init__(__self__, *,
-                 token_name: pulumi.Input[str],
-                 user_id: pulumi.Input[str],
-                 comment: Optional[pulumi.Input[str]] = None,
-                 expiration_date: Optional[pulumi.Input[str]] = None,
-                 privileges_separation: Optional[pulumi.Input[bool]] = None):
+                 node_name: pulumi.Input[str],
+                 clone: Optional[pulumi.Input['Vm2CloneArgs']] = None,
+                 cpu: Optional[pulumi.Input['Vm2CpuArgs']] = None,
+                 description: Optional[pulumi.Input[str]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
+                 tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 template: Optional[pulumi.Input[bool]] = None,
+                 timeouts: Optional[pulumi.Input['Vm2TimeoutsArgs']] = None):
+        """
+        The set of arguments for constructing a Vm2 resource.
+        :param pulumi.Input[str] node_name: The name of the node where the VM is provisioned.
+        :param pulumi.Input['Vm2CloneArgs'] clone: The cloning configuration.
+        :param pulumi.Input['Vm2CpuArgs'] cpu: The CPU configuration.
+        :param pulumi.Input[str] description: The description of the VM.
+        :param pulumi.Input[str] name: The name of the VM. Doesn't have to be unique.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: The tags assigned to the VM.
+        :param pulumi.Input[bool] template: Set to true to create a VM template.
+        """
+        pulumi.set(__self__, "node_name", node_name)
+        if clone is not None:
+            pulumi.set(__self__, "clone", clone)
+        if cpu is not None:
+            pulumi.set(__self__, "cpu", cpu)
+        if description is not None:
+            pulumi.set(__self__, "description", description)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
+        if tags is not None:
+            pulumi.set(__self__, "tags", tags)
+        if template is not None:
+            pulumi.set(__self__, "template", template)
+        if timeouts is not None:
+            pulumi.set(__self__, "timeouts", timeouts)
+
+    @property
+    @pulumi.getter(name="nodeName")
+    def node_name(self) -> pulumi.Input[str]:
+        """
+        The name of the node where the VM is provisioned.
+        """
+        return pulumi.get(self, "node_name")
+
+    @node_name.setter
+    def node_name(self, value: pulumi.Input[str]):
+        pulumi.set(self, "node_name", value)
+
+    @property
+    @pulumi.getter
+    def clone(self) -> Optional[pulumi.Input['Vm2CloneArgs']]:
         """
-        The set of arguments for constructing a Token resource.
-        :param pulumi.Input[str] token_name: User-specific token identifier.
-        :param pulumi.Input[str] user_id: User identifier.
-        :param pulumi.Input[str] comment: Comment for the token.
-        :param pulumi.Input[str] expiration_date: Expiration date for the token.
-        :param pulumi.Input[bool] privileges_separation: Restrict API token privileges with separate ACLs (default), or give full privileges of corresponding user.
+        The cloning configuration.
         """
-        pulumi.set(__self__, "token_name", token_name)
-        pulumi.set(__self__, "user_id", user_id)
-        if comment is not None:
-            pulumi.set(__self__, "comment", comment)
-        if expiration_date is not None:
-            pulumi.set(__self__, "expiration_date", expiration_date)
-        if privileges_separation is not None:
-            pulumi.set(__self__, "privileges_separation", privileges_separation)
+        return pulumi.get(self, "clone")
+
+    @clone.setter
+    def clone(self, value: Optional[pulumi.Input['Vm2CloneArgs']]):
+        pulumi.set(self, "clone", value)
 
     @property
-    @pulumi.getter(name="tokenName")
-    def token_name(self) -> pulumi.Input[str]:
+    @pulumi.getter
+    def cpu(self) -> Optional[pulumi.Input['Vm2CpuArgs']]:
         """
-        User-specific token identifier.
+        The CPU configuration.
         """
-        return pulumi.get(self, "token_name")
+        return pulumi.get(self, "cpu")
 
-    @token_name.setter
-    def token_name(self, value: pulumi.Input[str]):
-        pulumi.set(self, "token_name", value)
+    @cpu.setter
+    def cpu(self, value: Optional[pulumi.Input['Vm2CpuArgs']]):
+        pulumi.set(self, "cpu", value)
 
     @property
-    @pulumi.getter(name="userId")
-    def user_id(self) -> pulumi.Input[str]:
+    @pulumi.getter
+    def description(self) -> Optional[pulumi.Input[str]]:
         """
-        User identifier.
+        The description of the VM.
         """
-        return pulumi.get(self, "user_id")
+        return pulumi.get(self, "description")
 
-    @user_id.setter
-    def user_id(self, value: pulumi.Input[str]):
-        pulumi.set(self, "user_id", value)
+    @description.setter
+    def description(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "description", value)
 
     @property
     @pulumi.getter
-    def comment(self) -> Optional[pulumi.Input[str]]:
+    def name(self) -> Optional[pulumi.Input[str]]:
         """
-        Comment for the token.
+        The name of the VM. Doesn't have to be unique.
         """
-        return pulumi.get(self, "comment")
+        return pulumi.get(self, "name")
 
-    @comment.setter
-    def comment(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "comment", value)
+    @name.setter
+    def name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "name", value)
 
     @property
-    @pulumi.getter(name="expirationDate")
-    def expiration_date(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter
+    def tags(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        Expiration date for the token.
+        The tags assigned to the VM.
         """
-        return pulumi.get(self, "expiration_date")
+        return pulumi.get(self, "tags")
 
-    @expiration_date.setter
-    def expiration_date(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "expiration_date", value)
+    @tags.setter
+    def tags(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "tags", value)
 
     @property
-    @pulumi.getter(name="privilegesSeparation")
-    def privileges_separation(self) -> Optional[pulumi.Input[bool]]:
+    @pulumi.getter
+    def template(self) -> Optional[pulumi.Input[bool]]:
         """
-        Restrict API token privileges with separate ACLs (default), or give full privileges of corresponding user.
+        Set to true to create a VM template.
         """
-        return pulumi.get(self, "privileges_separation")
+        return pulumi.get(self, "template")
+
+    @template.setter
+    def template(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "template", value)
 
-    @privileges_separation.setter
-    def privileges_separation(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "privileges_separation", value)
+    @property
+    @pulumi.getter
+    def timeouts(self) -> Optional[pulumi.Input['Vm2TimeoutsArgs']]:
+        return pulumi.get(self, "timeouts")
+
+    @timeouts.setter
+    def timeouts(self, value: Optional[pulumi.Input['Vm2TimeoutsArgs']]):
+        pulumi.set(self, "timeouts", value)
 
 
 @pulumi.input_type
-class _TokenState:
+class _Vm2State:
     def __init__(__self__, *,
-                 comment: Optional[pulumi.Input[str]] = None,
-                 expiration_date: Optional[pulumi.Input[str]] = None,
-                 privileges_separation: Optional[pulumi.Input[bool]] = None,
-                 token_name: Optional[pulumi.Input[str]] = None,
-                 user_id: Optional[pulumi.Input[str]] = None,
-                 value: Optional[pulumi.Input[str]] = None):
+                 clone: Optional[pulumi.Input['Vm2CloneArgs']] = None,
+                 cpu: Optional[pulumi.Input['Vm2CpuArgs']] = None,
+                 description: Optional[pulumi.Input[str]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
+                 node_name: Optional[pulumi.Input[str]] = None,
+                 tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 template: Optional[pulumi.Input[bool]] = None,
+                 timeouts: Optional[pulumi.Input['Vm2TimeoutsArgs']] = None):
+        """
+        Input properties used for looking up and filtering Vm2 resources.
+        :param pulumi.Input['Vm2CloneArgs'] clone: The cloning configuration.
+        :param pulumi.Input['Vm2CpuArgs'] cpu: The CPU configuration.
+        :param pulumi.Input[str] description: The description of the VM.
+        :param pulumi.Input[str] name: The name of the VM. Doesn't have to be unique.
+        :param pulumi.Input[str] node_name: The name of the node where the VM is provisioned.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: The tags assigned to the VM.
+        :param pulumi.Input[bool] template: Set to true to create a VM template.
+        """
+        if clone is not None:
+            pulumi.set(__self__, "clone", clone)
+        if cpu is not None:
+            pulumi.set(__self__, "cpu", cpu)
+        if description is not None:
+            pulumi.set(__self__, "description", description)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
+        if node_name is not None:
+            pulumi.set(__self__, "node_name", node_name)
+        if tags is not None:
+            pulumi.set(__self__, "tags", tags)
+        if template is not None:
+            pulumi.set(__self__, "template", template)
+        if timeouts is not None:
+            pulumi.set(__self__, "timeouts", timeouts)
+
+    @property
+    @pulumi.getter
+    def clone(self) -> Optional[pulumi.Input['Vm2CloneArgs']]:
         """
-        Input properties used for looking up and filtering Token resources.
-        :param pulumi.Input[str] comment: Comment for the token.
-        :param pulumi.Input[str] expiration_date: Expiration date for the token.
-        :param pulumi.Input[bool] privileges_separation: Restrict API token privileges with separate ACLs (default), or give full privileges of corresponding user.
-        :param pulumi.Input[str] token_name: User-specific token identifier.
-        :param pulumi.Input[str] user_id: User identifier.
-        :param pulumi.Input[str] value: API token value used for authentication. It is populated only when creating a new token, and can't be retrieved at import.
+        The cloning configuration.
         """
-        if comment is not None:
-            pulumi.set(__self__, "comment", comment)
-        if expiration_date is not None:
-            pulumi.set(__self__, "expiration_date", expiration_date)
-        if privileges_separation is not None:
-            pulumi.set(__self__, "privileges_separation", privileges_separation)
-        if token_name is not None:
-            pulumi.set(__self__, "token_name", token_name)
-        if user_id is not None:
-            pulumi.set(__self__, "user_id", user_id)
-        if value is not None:
-            pulumi.set(__self__, "value", value)
+        return pulumi.get(self, "clone")
+
+    @clone.setter
+    def clone(self, value: Optional[pulumi.Input['Vm2CloneArgs']]):
+        pulumi.set(self, "clone", value)
 
     @property
     @pulumi.getter
-    def comment(self) -> Optional[pulumi.Input[str]]:
+    def cpu(self) -> Optional[pulumi.Input['Vm2CpuArgs']]:
         """
-        Comment for the token.
+        The CPU configuration.
         """
-        return pulumi.get(self, "comment")
+        return pulumi.get(self, "cpu")
 
-    @comment.setter
-    def comment(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "comment", value)
+    @cpu.setter
+    def cpu(self, value: Optional[pulumi.Input['Vm2CpuArgs']]):
+        pulumi.set(self, "cpu", value)
 
     @property
-    @pulumi.getter(name="expirationDate")
-    def expiration_date(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter
+    def description(self) -> Optional[pulumi.Input[str]]:
         """
-        Expiration date for the token.
+        The description of the VM.
         """
-        return pulumi.get(self, "expiration_date")
+        return pulumi.get(self, "description")
 
-    @expiration_date.setter
-    def expiration_date(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "expiration_date", value)
+    @description.setter
+    def description(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "description", value)
 
     @property
-    @pulumi.getter(name="privilegesSeparation")
-    def privileges_separation(self) -> Optional[pulumi.Input[bool]]:
+    @pulumi.getter
+    def name(self) -> Optional[pulumi.Input[str]]:
         """
-        Restrict API token privileges with separate ACLs (default), or give full privileges of corresponding user.
+        The name of the VM. Doesn't have to be unique.
         """
-        return pulumi.get(self, "privileges_separation")
+        return pulumi.get(self, "name")
 
-    @privileges_separation.setter
-    def privileges_separation(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "privileges_separation", value)
+    @name.setter
+    def name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "name", value)
 
     @property
-    @pulumi.getter(name="tokenName")
-    def token_name(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="nodeName")
+    def node_name(self) -> Optional[pulumi.Input[str]]:
         """
-        User-specific token identifier.
+        The name of the node where the VM is provisioned.
         """
-        return pulumi.get(self, "token_name")
+        return pulumi.get(self, "node_name")
 
-    @token_name.setter
-    def token_name(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "token_name", value)
+    @node_name.setter
+    def node_name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "node_name", value)
 
     @property
-    @pulumi.getter(name="userId")
-    def user_id(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter
+    def tags(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        User identifier.
+        The tags assigned to the VM.
         """
-        return pulumi.get(self, "user_id")
+        return pulumi.get(self, "tags")
 
-    @user_id.setter
-    def user_id(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "user_id", value)
+    @tags.setter
+    def tags(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "tags", value)
 
     @property
     @pulumi.getter
-    def value(self) -> Optional[pulumi.Input[str]]:
+    def template(self) -> Optional[pulumi.Input[bool]]:
         """
-        API token value used for authentication. It is populated only when creating a new token, and can't be retrieved at import.
+        Set to true to create a VM template.
         """
-        return pulumi.get(self, "value")
+        return pulumi.get(self, "template")
+
+    @template.setter
+    def template(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "template", value)
+
+    @property
+    @pulumi.getter
+    def timeouts(self) -> Optional[pulumi.Input['Vm2TimeoutsArgs']]:
+        return pulumi.get(self, "timeouts")
 
-    @value.setter
-    def value(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "value", value)
+    @timeouts.setter
+    def timeouts(self, value: Optional[pulumi.Input['Vm2TimeoutsArgs']]):
+        pulumi.set(self, "timeouts", value)
 
 
-class Token(pulumi.CustomResource):
+class Vm2(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 comment: Optional[pulumi.Input[str]] = None,
-                 expiration_date: Optional[pulumi.Input[str]] = None,
-                 privileges_separation: Optional[pulumi.Input[bool]] = None,
-                 token_name: Optional[pulumi.Input[str]] = None,
-                 user_id: Optional[pulumi.Input[str]] = None,
+                 clone: Optional[pulumi.Input[pulumi.InputType['Vm2CloneArgs']]] = None,
+                 cpu: Optional[pulumi.Input[pulumi.InputType['Vm2CpuArgs']]] = None,
+                 description: Optional[pulumi.Input[str]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
+                 node_name: Optional[pulumi.Input[str]] = None,
+                 tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 template: Optional[pulumi.Input[bool]] = None,
+                 timeouts: Optional[pulumi.Input[pulumi.InputType['Vm2TimeoutsArgs']]] = None,
                  __props__=None):
         """
-        User API tokens.
+        !> **DO NOT USE**
+        This is an experimental implementation of a Proxmox VM resource using Plugin Framework.<br><br>It is a Proof of Concept, highly experimental and **will** change in future. It does not support all features of the Proxmox API for VMs and **MUST NOT** be used in production.
 
-        ## Example Usage
-
-        ```python
-        import pulumi
-        import pulumi_proxmoxve as proxmoxve
-
-        # if creating a user token, the user must be created first
-        user = proxmoxve.permission.User("user",
-            comment="Managed by Terraform",
-            email="user@pve",
-            enabled=True,
-            expiration_date="2034-01-01T22:00:00Z",
-            user_id="user@pve")
-        user_token = proxmoxve.user.Token("userToken",
-            comment="Managed by Terraform",
-            expiration_date="2033-01-01T22:00:00Z",
-            token_name="tk1",
-            user_id=user.user_id)
-        ```
-
-        ## Import
-
-        #!/usr/bin/env sh
-
-        #Tokens can be imported using they identifiers in format `user_id!token_name` format, e.g.:
-
-        ```sh
-        $ pulumi import proxmoxve:User/token:Token token1 user@pve!token1
-        ```
+        > Many attributes are marked as **optional** _and_ **computed** in the schema,
+        hence you may seem added to the plan with "(known after apply)" status, even if they are not set in the configuration.
+        This is done to support the `clone` operation, when a VM is created from an existing VM or template,
+        and the source attributes are copied to the clone.<br><br>
+        Computed attributes allow the provider to set those attributes without user input.
+        The attributes are also marked as optional to allow the practitioner to set (or overwrite) them if needed.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] comment: Comment for the token.
-        :param pulumi.Input[str] expiration_date: Expiration date for the token.
-        :param pulumi.Input[bool] privileges_separation: Restrict API token privileges with separate ACLs (default), or give full privileges of corresponding user.
-        :param pulumi.Input[str] token_name: User-specific token identifier.
-        :param pulumi.Input[str] user_id: User identifier.
+        :param pulumi.Input[pulumi.InputType['Vm2CloneArgs']] clone: The cloning configuration.
+        :param pulumi.Input[pulumi.InputType['Vm2CpuArgs']] cpu: The CPU configuration.
+        :param pulumi.Input[str] description: The description of the VM.
+        :param pulumi.Input[str] name: The name of the VM. Doesn't have to be unique.
+        :param pulumi.Input[str] node_name: The name of the node where the VM is provisioned.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: The tags assigned to the VM.
+        :param pulumi.Input[bool] template: Set to true to create a VM template.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: TokenArgs,
+                 args: Vm2Args,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        User API tokens.
-
-        ## Example Usage
+        !> **DO NOT USE**
+        This is an experimental implementation of a Proxmox VM resource using Plugin Framework.<br><br>It is a Proof of Concept, highly experimental and **will** change in future. It does not support all features of the Proxmox API for VMs and **MUST NOT** be used in production.
 
-        ```python
-        import pulumi
-        import pulumi_proxmoxve as proxmoxve
-
-        # if creating a user token, the user must be created first
-        user = proxmoxve.permission.User("user",
-            comment="Managed by Terraform",
-            email="user@pve",
-            enabled=True,
-            expiration_date="2034-01-01T22:00:00Z",
-            user_id="user@pve")
-        user_token = proxmoxve.user.Token("userToken",
-            comment="Managed by Terraform",
-            expiration_date="2033-01-01T22:00:00Z",
-            token_name="tk1",
-            user_id=user.user_id)
-        ```
-
-        ## Import
-
-        #!/usr/bin/env sh
-
-        #Tokens can be imported using they identifiers in format `user_id!token_name` format, e.g.:
-
-        ```sh
-        $ pulumi import proxmoxve:User/token:Token token1 user@pve!token1
-        ```
+        > Many attributes are marked as **optional** _and_ **computed** in the schema,
+        hence you may seem added to the plan with "(known after apply)" status, even if they are not set in the configuration.
+        This is done to support the `clone` operation, when a VM is created from an existing VM or template,
+        and the source attributes are copied to the clone.<br><br>
+        Computed attributes allow the provider to set those attributes without user input.
+        The attributes are also marked as optional to allow the practitioner to set (or overwrite) them if needed.
 
         :param str resource_name: The name of the resource.
-        :param TokenArgs args: The arguments to use to populate this resource's properties.
+        :param Vm2Args args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(TokenArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(Vm2Args, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 comment: Optional[pulumi.Input[str]] = None,
-                 expiration_date: Optional[pulumi.Input[str]] = None,
-                 privileges_separation: Optional[pulumi.Input[bool]] = None,
-                 token_name: Optional[pulumi.Input[str]] = None,
-                 user_id: Optional[pulumi.Input[str]] = None,
+                 clone: Optional[pulumi.Input[pulumi.InputType['Vm2CloneArgs']]] = None,
+                 cpu: Optional[pulumi.Input[pulumi.InputType['Vm2CpuArgs']]] = None,
+                 description: Optional[pulumi.Input[str]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
+                 node_name: Optional[pulumi.Input[str]] = None,
+                 tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 template: Optional[pulumi.Input[bool]] = None,
+                 timeouts: Optional[pulumi.Input[pulumi.InputType['Vm2TimeoutsArgs']]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = TokenArgs.__new__(TokenArgs)
+            __props__ = Vm2Args.__new__(Vm2Args)
 
-            __props__.__dict__["comment"] = comment
-            __props__.__dict__["expiration_date"] = expiration_date
-            __props__.__dict__["privileges_separation"] = privileges_separation
-            if token_name is None and not opts.urn:
-                raise TypeError("Missing required property 'token_name'")
-            __props__.__dict__["token_name"] = token_name
-            if user_id is None and not opts.urn:
-                raise TypeError("Missing required property 'user_id'")
-            __props__.__dict__["user_id"] = user_id
-            __props__.__dict__["value"] = None
-        secret_opts = pulumi.ResourceOptions(additional_secret_outputs=["value"])
-        opts = pulumi.ResourceOptions.merge(opts, secret_opts)
-        super(Token, __self__).__init__(
-            'proxmoxve:User/token:Token',
+            __props__.__dict__["clone"] = clone
+            __props__.__dict__["cpu"] = cpu
+            __props__.__dict__["description"] = description
+            __props__.__dict__["name"] = name
+            if node_name is None and not opts.urn:
+                raise TypeError("Missing required property 'node_name'")
+            __props__.__dict__["node_name"] = node_name
+            __props__.__dict__["tags"] = tags
+            __props__.__dict__["template"] = template
+            __props__.__dict__["timeouts"] = timeouts
+        super(Vm2, __self__).__init__(
+            'proxmoxve:index/vm2:Vm2',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
-            comment: Optional[pulumi.Input[str]] = None,
-            expiration_date: Optional[pulumi.Input[str]] = None,
-            privileges_separation: Optional[pulumi.Input[bool]] = None,
-            token_name: Optional[pulumi.Input[str]] = None,
-            user_id: Optional[pulumi.Input[str]] = None,
-            value: Optional[pulumi.Input[str]] = None) -> 'Token':
+            clone: Optional[pulumi.Input[pulumi.InputType['Vm2CloneArgs']]] = None,
+            cpu: Optional[pulumi.Input[pulumi.InputType['Vm2CpuArgs']]] = None,
+            description: Optional[pulumi.Input[str]] = None,
+            name: Optional[pulumi.Input[str]] = None,
+            node_name: Optional[pulumi.Input[str]] = None,
+            tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+            template: Optional[pulumi.Input[bool]] = None,
+            timeouts: Optional[pulumi.Input[pulumi.InputType['Vm2TimeoutsArgs']]] = None) -> 'Vm2':
         """
-        Get an existing Token resource's state with the given name, id, and optional extra
+        Get an existing Vm2 resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] comment: Comment for the token.
-        :param pulumi.Input[str] expiration_date: Expiration date for the token.
-        :param pulumi.Input[bool] privileges_separation: Restrict API token privileges with separate ACLs (default), or give full privileges of corresponding user.
-        :param pulumi.Input[str] token_name: User-specific token identifier.
-        :param pulumi.Input[str] user_id: User identifier.
-        :param pulumi.Input[str] value: API token value used for authentication. It is populated only when creating a new token, and can't be retrieved at import.
+        :param pulumi.Input[pulumi.InputType['Vm2CloneArgs']] clone: The cloning configuration.
+        :param pulumi.Input[pulumi.InputType['Vm2CpuArgs']] cpu: The CPU configuration.
+        :param pulumi.Input[str] description: The description of the VM.
+        :param pulumi.Input[str] name: The name of the VM. Doesn't have to be unique.
+        :param pulumi.Input[str] node_name: The name of the node where the VM is provisioned.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: The tags assigned to the VM.
+        :param pulumi.Input[bool] template: Set to true to create a VM template.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _TokenState.__new__(_TokenState)
+        __props__ = _Vm2State.__new__(_Vm2State)
 
-        __props__.__dict__["comment"] = comment
-        __props__.__dict__["expiration_date"] = expiration_date
-        __props__.__dict__["privileges_separation"] = privileges_separation
-        __props__.__dict__["token_name"] = token_name
-        __props__.__dict__["user_id"] = user_id
-        __props__.__dict__["value"] = value
-        return Token(resource_name, opts=opts, __props__=__props__)
+        __props__.__dict__["clone"] = clone
+        __props__.__dict__["cpu"] = cpu
+        __props__.__dict__["description"] = description
+        __props__.__dict__["name"] = name
+        __props__.__dict__["node_name"] = node_name
+        __props__.__dict__["tags"] = tags
+        __props__.__dict__["template"] = template
+        __props__.__dict__["timeouts"] = timeouts
+        return Vm2(resource_name, opts=opts, __props__=__props__)
+
+    @property
+    @pulumi.getter
+    def clone(self) -> pulumi.Output[Optional['outputs.Vm2Clone']]:
+        """
+        The cloning configuration.
+        """
+        return pulumi.get(self, "clone")
 
     @property
     @pulumi.getter
-    def comment(self) -> pulumi.Output[Optional[str]]:
+    def cpu(self) -> pulumi.Output['outputs.Vm2Cpu']:
         """
-        Comment for the token.
+        The CPU configuration.
         """
-        return pulumi.get(self, "comment")
+        return pulumi.get(self, "cpu")
 
     @property
-    @pulumi.getter(name="expirationDate")
-    def expiration_date(self) -> pulumi.Output[Optional[str]]:
+    @pulumi.getter
+    def description(self) -> pulumi.Output[Optional[str]]:
         """
-        Expiration date for the token.
+        The description of the VM.
         """
-        return pulumi.get(self, "expiration_date")
+        return pulumi.get(self, "description")
 
     @property
-    @pulumi.getter(name="privilegesSeparation")
-    def privileges_separation(self) -> pulumi.Output[bool]:
+    @pulumi.getter
+    def name(self) -> pulumi.Output[str]:
         """
-        Restrict API token privileges with separate ACLs (default), or give full privileges of corresponding user.
+        The name of the VM. Doesn't have to be unique.
         """
-        return pulumi.get(self, "privileges_separation")
+        return pulumi.get(self, "name")
 
     @property
-    @pulumi.getter(name="tokenName")
-    def token_name(self) -> pulumi.Output[str]:
+    @pulumi.getter(name="nodeName")
+    def node_name(self) -> pulumi.Output[str]:
         """
-        User-specific token identifier.
+        The name of the node where the VM is provisioned.
         """
-        return pulumi.get(self, "token_name")
+        return pulumi.get(self, "node_name")
 
     @property
-    @pulumi.getter(name="userId")
-    def user_id(self) -> pulumi.Output[str]:
+    @pulumi.getter
+    def tags(self) -> pulumi.Output[Sequence[str]]:
         """
-        User identifier.
+        The tags assigned to the VM.
         """
-        return pulumi.get(self, "user_id")
+        return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter
-    def value(self) -> pulumi.Output[str]:
+    def template(self) -> pulumi.Output[Optional[bool]]:
         """
-        API token value used for authentication. It is populated only when creating a new token, and can't be retrieved at import.
+        Set to true to create a VM template.
         """
-        return pulumi.get(self, "value")
+        return pulumi.get(self, "template")
+
+    @property
+    @pulumi.getter
+    def timeouts(self) -> pulumi.Output[Optional['outputs.Vm2Timeouts']]:
+        return pulumi.get(self, "timeouts")
```

### Comparing `pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/vm/_inputs.py` & `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/vm/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/vm/get_virtual_machine.py` & `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/vm/get_virtual_machine.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/vm/get_virtual_machines.py` & `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/vm/get_virtual_machines.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/vm/outputs.py` & `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/vm/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.0/pulumi_proxmoxve/vm/virtual_machine.py` & `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve/vm/virtual_machine.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.7.0/pulumi_proxmoxve.egg-info/PKG-INFO` & `pulumi_proxmoxve-6.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pulumi-proxmoxve
-Version: 6.7.0
+Name: pulumi_proxmoxve
+Version: 6.7.1
 Summary: A Pulumi package for creating and managing Proxmox Virtual Environment cloud resources.
 Home-page: https://github.com/muhlba91/pulumi-proxmoxve
 License: Apache-2.0
 Project-URL: Repository, https://github.com/muhlba91/pulumi-proxmoxve
 Keywords: pulumi proxmox proxmoxve
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `pulumi_proxmoxve-6.7.0/pulumi_proxmoxve.egg-info/SOURCES.txt` & `pulumi_proxmoxve-6.7.1/pulumi_proxmoxve.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 pulumi_proxmoxve/__init__.py
 pulumi_proxmoxve/_inputs.py
 pulumi_proxmoxve/_utilities.py
 pulumi_proxmoxve/acl.py
 pulumi_proxmoxve/certifi.py
 pulumi_proxmoxve/dns.py
 pulumi_proxmoxve/get_node.py
+pulumi_proxmoxve/get_vm2.py
 pulumi_proxmoxve/hosts.py
 pulumi_proxmoxve/outputs.py
 pulumi_proxmoxve/provider.py
 pulumi_proxmoxve/pulumi-plugin.json
 pulumi_proxmoxve/py.typed
 pulumi_proxmoxve/time.py
 pulumi_proxmoxve/vm2.py
```

### Comparing `pulumi_proxmoxve-6.7.0/setup.py` & `pulumi_proxmoxve-6.7.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "6.7.0"
+VERSION = "6.7.1"
 def readme():
     try:
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "proxmoxve Pulumi Package - Development Version"
```

