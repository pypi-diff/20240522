# Comparing `tmp/pulumi_equinix-0.9.0.tar.gz` & `tmp/pulumi_equinix-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_equinix-0.9.0.tar", last modified: Tue May 14 14:31:30 2024, max compression
+gzip compressed data, was "pulumi_equinix-0.9.1.tar", last modified: Tue May 14 16:38:52 2024, max compression
```

## Comparing `pulumi_equinix-0.9.0.tar` & `pulumi_equinix-0.9.1.tar`

### file list

```diff
@@ -1,104 +1,104 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:31:30.665773 pulumi_equinix-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     5463 2024-05-14 14:31:30.665773 pulumi_equinix-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5078 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:31:30.653773 pulumi_equinix-0.9.0/pulumi_equinix/
--rw-r--r--   0 runner    (1001) docker     (127)     6522 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/_enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     9277 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:31:30.653773 pulumi_equinix-0.9.0/pulumi_equinix/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/config/vars.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:31:30.657773 pulumi_equinix-0.9.0/pulumi_equinix/fabric/
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/fabric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/fabric/_enums.py
--rw-r--r--   0 runner    (1001) docker     (127)   234801 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/fabric/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    41117 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/fabric/cloud_router.py
--rw-r--r--   0 runner    (1001) docker     (127)    43191 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/fabric/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    14853 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/fabric/get_cloud_router.py
--rw-r--r--   0 runner    (1001) docker     (127)    14560 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/fabric/get_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     9379 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/fabric/get_network.py
--rw-r--r--   0 runner    (1001) docker     (127)    12758 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/fabric/get_port.py
--rw-r--r--   0 runner    (1001) docker     (127)     6762 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/fabric/get_ports.py
--rw-r--r--   0 runner    (1001) docker     (127)    14442 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/fabric/get_routing_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)    15526 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/fabric/get_service_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     9698 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/fabric/get_service_profiles.py
--rw-r--r--   0 runner    (1001) docker     (127)    25175 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/fabric/network.py
--rw-r--r--   0 runner    (1001) docker     (127)   449076 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/fabric/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    37312 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/fabric/routing_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)    52222 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/fabric/service_profile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:31:30.661773 pulumi_equinix-0.9.0/pulumi_equinix/metal/
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6412 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/_enums.py
--rw-r--r--   0 runner    (1001) docker     (127)    43843 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    12084 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/bgp_session.py
--rw-r--r--   0 runner    (1001) docker     (127)   116295 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     9604 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/device_network_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    18663 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/gateway.py
--rw-r--r--   0 runner    (1001) docker     (127)    17219 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/get_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     4511 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/get_device_bgp_neighbors.py
--rw-r--r--   0 runner    (1001) docker     (127)     9274 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/get_devices.py
--rw-r--r--   0 runner    (1001) docker     (127)     6654 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/get_facility.py
--rw-r--r--   0 runner    (1001) docker     (127)     6953 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/get_gateway.py
--rw-r--r--   0 runner    (1001) docker     (127)     8319 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/get_hardware_reservation.py
--rw-r--r--   0 runner    (1001) docker     (127)    14211 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/get_interconnection.py
--rw-r--r--   0 runner    (1001) docker     (127)     9195 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/get_ip_block_ranges.py
--rw-r--r--   0 runner    (1001) docker     (127)     4580 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/get_metro.py
--rw-r--r--   0 runner    (1001) docker     (127)     6395 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/get_operating_system.py
--rw-r--r--   0 runner    (1001) docker     (127)     6939 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/get_organization.py
--rw-r--r--   0 runner    (1001) docker     (127)    10989 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/get_plans.py
--rw-r--r--   0 runner    (1001) docker     (127)    10533 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/get_port.py
--rw-r--r--   0 runner    (1001) docker     (127)    12080 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/get_precreated_ip_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     7489 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/get_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     7397 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/get_project_ssh_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    11542 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/get_reserved_ip_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/get_spot_market_price.py
--rw-r--r--   0 runner    (1001) docker     (127)     7813 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/get_spot_market_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    12360 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/get_virtual_circuit.py
--rw-r--r--   0 runner    (1001) docker     (127)     8619 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/get_vlan.py
--rw-r--r--   0 runner    (1001) docker     (127)     6153 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/get_vrf.py
--rw-r--r--   0 runner    (1001) docker     (127)    51542 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/interconnection.py
--rw-r--r--   0 runner    (1001) docker     (127)    20819 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/ip_attachment.py
--rw-r--r--   0 runner    (1001) docker     (127)    17879 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/organization.py
--rw-r--r--   0 runner    (1001) docker     (127)    22528 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/organization_member.py
--rw-r--r--   0 runner    (1001) docker     (127)    74111 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    27669 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/port.py
--rw-r--r--   0 runner    (1001) docker     (127)    20188 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/port_vlan_attachment.py
--rw-r--r--   0 runner    (1001) docker     (127)    22695 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/project.py
--rw-r--r--   0 runner    (1001) docker     (127)    13513 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/project_api_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    14977 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/project_ssh_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    48329 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/reserved_ip_block.py
--rw-r--r--   0 runner    (1001) docker     (127)    29621 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/spot_market_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    13635 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/ssh_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    12291 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/user_api_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    42484 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/virtual_circuit.py
--rw-r--r--   0 runner    (1001) docker     (127)    17497 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/vlan.py
--rw-r--r--   0 runner    (1001) docker     (127)    18262 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/metal/vrf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:31:30.665773 pulumi_equinix-0.9.0/pulumi_equinix/networkedge/
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/networkedge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/networkedge/_enums.py
--rw-r--r--   0 runner    (1001) docker     (127)    69946 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/networkedge/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    25536 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/networkedge/acl_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    23170 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/networkedge/bgp.py
--rw-r--r--   0 runner    (1001) docker     (127)   104546 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/networkedge/device.py
--rw-r--r--   0 runner    (1001) docker     (127)    29791 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/networkedge/device_link.py
--rw-r--r--   0 runner    (1001) docker     (127)     6849 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/networkedge/get_account.py
--rw-r--r--   0 runner    (1001) docker     (127)    26748 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/networkedge/get_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     9343 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/networkedge/get_device_platform.py
--rw-r--r--   0 runner    (1001) docker     (127)     9468 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/networkedge/get_device_software.py
--rw-r--r--   0 runner    (1001) docker     (127)     6639 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/networkedge/get_device_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    23179 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/networkedge/network_file.py
--rw-r--r--   0 runner    (1001) docker     (127)    99377 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/networkedge/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    14390 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/networkedge/ssh_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    11962 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/networkedge/ssh_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    14168 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 14:31:30.653773 pulumi_equinix-0.9.0/pulumi_equinix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5463 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/pulumi_equinix.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 14:31:30.665773 pulumi_equinix-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-05-14 14:31:30.000000 pulumi_equinix-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:38:52.920770 pulumi_equinix-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     5463 2024-05-14 16:38:52.920770 pulumi_equinix-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5078 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:38:52.900770 pulumi_equinix-0.9.1/pulumi_equinix/
+-rw-r--r--   0 runner    (1001) docker     (127)     6522 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix/_enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9277 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:38:52.904770 pulumi_equinix-0.9.1/pulumi_equinix/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix/config/vars.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:38:52.908770 pulumi_equinix-0.9.1/pulumi_equinix/fabric/
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix/fabric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix/fabric/_enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)   234801 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix/fabric/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41117 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix/fabric/cloud_router.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43191 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix/fabric/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14853 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix/fabric/get_cloud_router.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14560 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix/fabric/get_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9379 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix/fabric/get_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12758 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix/fabric/get_port.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6762 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix/fabric/get_ports.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14442 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix/fabric/get_routing_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15526 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix/fabric/get_service_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9698 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix/fabric/get_service_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25175 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix/fabric/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)   449076 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix/fabric/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37312 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix/fabric/routing_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52222 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix/fabric/service_profile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:38:52.916770 pulumi_equinix-0.9.1/pulumi_equinix/metal/
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix/metal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6412 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix/metal/_enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43843 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix/metal/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12084 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix/metal/bgp_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)   116295 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix/metal/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9604 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix/metal/device_network_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18663 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix/metal/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17219 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix/metal/get_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4511 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix/metal/get_device_bgp_neighbors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9274 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix/metal/get_devices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6654 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix/metal/get_facility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6953 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix/metal/get_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8319 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix/metal/get_hardware_reservation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14211 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix/metal/get_interconnection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9195 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix/metal/get_ip_block_ranges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4580 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix/metal/get_metro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6395 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix/metal/get_operating_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6939 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix/metal/get_organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10989 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix/metal/get_plans.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10533 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix/metal/get_port.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12080 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix/metal/get_precreated_ip_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7489 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix/metal/get_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7397 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix/metal/get_project_ssh_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11542 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix/metal/get_reserved_ip_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix/metal/get_spot_market_price.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7813 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix/metal/get_spot_market_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12360 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix/metal/get_virtual_circuit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8619 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix/metal/get_vlan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6153 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix/metal/get_vrf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51542 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix/metal/interconnection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20819 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix/metal/ip_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17879 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix/metal/organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22528 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix/metal/organization_member.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74111 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix/metal/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27669 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix/metal/port.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20188 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix/metal/port_vlan_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22695 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix/metal/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13513 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix/metal/project_api_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14977 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix/metal/project_ssh_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48329 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix/metal/reserved_ip_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29621 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix/metal/spot_market_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13635 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix/metal/ssh_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12291 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix/metal/user_api_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42484 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix/metal/virtual_circuit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17497 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix/metal/vlan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18262 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix/metal/vrf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:38:52.920770 pulumi_equinix-0.9.1/pulumi_equinix/networkedge/
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix/networkedge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix/networkedge/_enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69946 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix/networkedge/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25536 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix/networkedge/acl_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23170 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix/networkedge/bgp.py
+-rw-r--r--   0 runner    (1001) docker     (127)   104546 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix/networkedge/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29791 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix/networkedge/device_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6849 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix/networkedge/get_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26748 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix/networkedge/get_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9343 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix/networkedge/get_device_platform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9468 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix/networkedge/get_device_software.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6639 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix/networkedge/get_device_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23179 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix/networkedge/network_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    99377 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix/networkedge/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14390 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix/networkedge/ssh_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11962 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix/networkedge/ssh_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14168 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:38:52.904770 pulumi_equinix-0.9.1/pulumi_equinix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5463 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/pulumi_equinix.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 16:38:52.920770 pulumi_equinix-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-05-14 16:38:52.000000 pulumi_equinix-0.9.1/setup.py
```

### Comparing `pulumi_equinix-0.9.0/PKG-INFO` & `pulumi_equinix-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_equinix
-Version: 0.9.0
+Version: 0.9.1
 Summary: A Pulumi package for creating and managing equinix cloud resources.
 Home-page: https://deploy.equinix.com/
 License: Apache-2.0
 Project-URL: Repository, https://github.com/equinix/pulumi-equinix
 Keywords: pulumi equinix category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `pulumi_equinix-0.9.0/README.md` & `pulumi_equinix-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.9.0/pulumi_equinix/__init__.py` & `pulumi_equinix-0.9.1/pulumi_equinix/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.9.0/pulumi_equinix/_enums.py` & `pulumi_equinix-0.9.1/pulumi_equinix/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.9.0/pulumi_equinix/_utilities.py` & `pulumi_equinix-0.9.1/pulumi_equinix/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.9.0/pulumi_equinix/config/vars.py` & `pulumi_equinix-0.9.1/pulumi_equinix/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.9.0/pulumi_equinix/fabric/__init__.py` & `pulumi_equinix-0.9.1/pulumi_equinix/fabric/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.9.0/pulumi_equinix/fabric/_enums.py` & `pulumi_equinix-0.9.1/pulumi_equinix/fabric/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.9.0/pulumi_equinix/fabric/_inputs.py` & `pulumi_equinix-0.9.1/pulumi_equinix/fabric/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.9.0/pulumi_equinix/fabric/cloud_router.py` & `pulumi_equinix-0.9.1/pulumi_equinix/fabric/cloud_router.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.9.0/pulumi_equinix/fabric/connection.py` & `pulumi_equinix-0.9.1/pulumi_equinix/fabric/connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.9.0/pulumi_equinix/fabric/get_cloud_router.py` & `pulumi_equinix-0.9.1/pulumi_equinix/fabric/get_cloud_router.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.9.0/pulumi_equinix/fabric/get_connection.py` & `pulumi_equinix-0.9.1/pulumi_equinix/fabric/get_connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.9.0/pulumi_equinix/fabric/get_network.py` & `pulumi_equinix-0.9.1/pulumi_equinix/fabric/get_network.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.9.0/pulumi_equinix/fabric/get_port.py` & `pulumi_equinix-0.9.1/pulumi_equinix/fabric/get_port.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.9.0/pulumi_equinix/fabric/get_ports.py` & `pulumi_equinix-0.9.1/pulumi_equinix/fabric/get_ports.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.9.0/pulumi_equinix/fabric/get_routing_protocol.py` & `pulumi_equinix-0.9.1/pulumi_equinix/fabric/get_routing_protocol.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.9.0/pulumi_equinix/fabric/get_service_profile.py` & `pulumi_equinix-0.9.1/pulumi_equinix/fabric/get_service_profile.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.9.0/pulumi_equinix/fabric/get_service_profiles.py` & `pulumi_equinix-0.9.1/pulumi_equinix/fabric/get_service_profiles.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.9.0/pulumi_equinix/fabric/network.py` & `pulumi_equinix-0.9.1/pulumi_equinix/fabric/network.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.9.0/pulumi_equinix/fabric/outputs.py` & `pulumi_equinix-0.9.1/pulumi_equinix/fabric/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.9.0/pulumi_equinix/fabric/routing_protocol.py` & `pulumi_equinix-0.9.1/pulumi_equinix/fabric/routing_protocol.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.9.0/pulumi_equinix/fabric/service_profile.py` & `pulumi_equinix-0.9.1/pulumi_equinix/fabric/service_profile.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.9.0/pulumi_equinix/metal/__init__.py` & `pulumi_equinix-0.9.1/pulumi_equinix/metal/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.9.0/pulumi_equinix/metal/_enums.py` & `pulumi_equinix-0.9.1/pulumi_equinix/metal/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.9.0/pulumi_equinix/metal/_inputs.py` & `pulumi_equinix-0.9.1/pulumi_equinix/metal/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.9.0/pulumi_equinix/metal/bgp_session.py` & `pulumi_equinix-0.9.1/pulumi_equinix/metal/bgp_session.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.9.0/pulumi_equinix/metal/device.py` & `pulumi_equinix-0.9.1/pulumi_equinix/metal/device.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.9.0/pulumi_equinix/metal/device_network_type.py` & `pulumi_equinix-0.9.1/pulumi_equinix/metal/device_network_type.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.9.0/pulumi_equinix/metal/gateway.py` & `pulumi_equinix-0.9.1/pulumi_equinix/metal/gateway.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.9.0/pulumi_equinix/metal/get_device.py` & `pulumi_equinix-0.9.1/pulumi_equinix/metal/get_device.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.9.0/pulumi_equinix/metal/get_device_bgp_neighbors.py` & `pulumi_equinix-0.9.1/pulumi_equinix/metal/get_device_bgp_neighbors.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.9.0/pulumi_equinix/metal/get_devices.py` & `pulumi_equinix-0.9.1/pulumi_equinix/metal/get_devices.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.9.0/pulumi_equinix/metal/get_facility.py` & `pulumi_equinix-0.9.1/pulumi_equinix/metal/get_facility.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.9.0/pulumi_equinix/metal/get_gateway.py` & `pulumi_equinix-0.9.1/pulumi_equinix/metal/get_gateway.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.9.0/pulumi_equinix/metal/get_hardware_reservation.py` & `pulumi_equinix-0.9.1/pulumi_equinix/metal/get_hardware_reservation.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.9.0/pulumi_equinix/metal/get_interconnection.py` & `pulumi_equinix-0.9.1/pulumi_equinix/metal/get_interconnection.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.9.0/pulumi_equinix/metal/get_ip_block_ranges.py` & `pulumi_equinix-0.9.1/pulumi_equinix/metal/get_ip_block_ranges.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.9.0/pulumi_equinix/metal/get_metro.py` & `pulumi_equinix-0.9.1/pulumi_equinix/metal/get_metro.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.9.0/pulumi_equinix/metal/get_operating_system.py` & `pulumi_equinix-0.9.1/pulumi_equinix/metal/get_operating_system.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.9.0/pulumi_equinix/metal/get_organization.py` & `pulumi_equinix-0.9.1/pulumi_equinix/metal/get_organization.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.9.0/pulumi_equinix/metal/get_plans.py` & `pulumi_equinix-0.9.1/pulumi_equinix/metal/get_plans.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.9.0/pulumi_equinix/metal/get_port.py` & `pulumi_equinix-0.9.1/pulumi_equinix/metal/get_port.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.9.0/pulumi_equinix/metal/get_precreated_ip_block.py` & `pulumi_equinix-0.9.1/pulumi_equinix/metal/get_precreated_ip_block.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.9.0/pulumi_equinix/metal/get_project.py` & `pulumi_equinix-0.9.1/pulumi_equinix/metal/get_project.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.9.0/pulumi_equinix/metal/get_project_ssh_key.py` & `pulumi_equinix-0.9.1/pulumi_equinix/metal/get_project_ssh_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.9.0/pulumi_equinix/metal/get_reserved_ip_block.py` & `pulumi_equinix-0.9.1/pulumi_equinix/metal/get_reserved_ip_block.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.9.0/pulumi_equinix/metal/get_spot_market_price.py` & `pulumi_equinix-0.9.1/pulumi_equinix/metal/get_spot_market_price.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.9.0/pulumi_equinix/metal/get_spot_market_request.py` & `pulumi_equinix-0.9.1/pulumi_equinix/metal/get_spot_market_request.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.9.0/pulumi_equinix/metal/get_virtual_circuit.py` & `pulumi_equinix-0.9.1/pulumi_equinix/metal/get_virtual_circuit.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.9.0/pulumi_equinix/metal/get_vlan.py` & `pulumi_equinix-0.9.1/pulumi_equinix/metal/get_vlan.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.9.0/pulumi_equinix/metal/get_vrf.py` & `pulumi_equinix-0.9.1/pulumi_equinix/metal/get_vrf.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.9.0/pulumi_equinix/metal/interconnection.py` & `pulumi_equinix-0.9.1/pulumi_equinix/metal/interconnection.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.9.0/pulumi_equinix/metal/ip_attachment.py` & `pulumi_equinix-0.9.1/pulumi_equinix/metal/ip_attachment.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.9.0/pulumi_equinix/metal/organization.py` & `pulumi_equinix-0.9.1/pulumi_equinix/metal/organization.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.9.0/pulumi_equinix/metal/organization_member.py` & `pulumi_equinix-0.9.1/pulumi_equinix/metal/organization_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.9.0/pulumi_equinix/metal/outputs.py` & `pulumi_equinix-0.9.1/pulumi_equinix/metal/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.9.0/pulumi_equinix/metal/port.py` & `pulumi_equinix-0.9.1/pulumi_equinix/metal/port.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.9.0/pulumi_equinix/metal/port_vlan_attachment.py` & `pulumi_equinix-0.9.1/pulumi_equinix/metal/port_vlan_attachment.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.9.0/pulumi_equinix/metal/project.py` & `pulumi_equinix-0.9.1/pulumi_equinix/metal/project.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.9.0/pulumi_equinix/metal/project_api_key.py` & `pulumi_equinix-0.9.1/pulumi_equinix/metal/project_api_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.9.0/pulumi_equinix/metal/project_ssh_key.py` & `pulumi_equinix-0.9.1/pulumi_equinix/metal/project_ssh_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.9.0/pulumi_equinix/metal/reserved_ip_block.py` & `pulumi_equinix-0.9.1/pulumi_equinix/metal/reserved_ip_block.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.9.0/pulumi_equinix/metal/spot_market_request.py` & `pulumi_equinix-0.9.1/pulumi_equinix/metal/spot_market_request.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.9.0/pulumi_equinix/metal/ssh_key.py` & `pulumi_equinix-0.9.1/pulumi_equinix/metal/ssh_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.9.0/pulumi_equinix/metal/user_api_key.py` & `pulumi_equinix-0.9.1/pulumi_equinix/metal/user_api_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.9.0/pulumi_equinix/metal/virtual_circuit.py` & `pulumi_equinix-0.9.1/pulumi_equinix/metal/virtual_circuit.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.9.0/pulumi_equinix/metal/vlan.py` & `pulumi_equinix-0.9.1/pulumi_equinix/metal/vlan.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.9.0/pulumi_equinix/metal/vrf.py` & `pulumi_equinix-0.9.1/pulumi_equinix/metal/vrf.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.9.0/pulumi_equinix/networkedge/__init__.py` & `pulumi_equinix-0.9.1/pulumi_equinix/networkedge/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.9.0/pulumi_equinix/networkedge/_enums.py` & `pulumi_equinix-0.9.1/pulumi_equinix/networkedge/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.9.0/pulumi_equinix/networkedge/_inputs.py` & `pulumi_equinix-0.9.1/pulumi_equinix/networkedge/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.9.0/pulumi_equinix/networkedge/acl_template.py` & `pulumi_equinix-0.9.1/pulumi_equinix/networkedge/acl_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.9.0/pulumi_equinix/networkedge/bgp.py` & `pulumi_equinix-0.9.1/pulumi_equinix/networkedge/bgp.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.9.0/pulumi_equinix/networkedge/device.py` & `pulumi_equinix-0.9.1/pulumi_equinix/networkedge/device.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.9.0/pulumi_equinix/networkedge/device_link.py` & `pulumi_equinix-0.9.1/pulumi_equinix/networkedge/device_link.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.9.0/pulumi_equinix/networkedge/get_account.py` & `pulumi_equinix-0.9.1/pulumi_equinix/networkedge/get_account.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.9.0/pulumi_equinix/networkedge/get_device.py` & `pulumi_equinix-0.9.1/pulumi_equinix/networkedge/get_device.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.9.0/pulumi_equinix/networkedge/get_device_platform.py` & `pulumi_equinix-0.9.1/pulumi_equinix/networkedge/get_device_platform.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.9.0/pulumi_equinix/networkedge/get_device_software.py` & `pulumi_equinix-0.9.1/pulumi_equinix/networkedge/get_device_software.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.9.0/pulumi_equinix/networkedge/get_device_type.py` & `pulumi_equinix-0.9.1/pulumi_equinix/networkedge/get_device_type.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.9.0/pulumi_equinix/networkedge/network_file.py` & `pulumi_equinix-0.9.1/pulumi_equinix/networkedge/network_file.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.9.0/pulumi_equinix/networkedge/outputs.py` & `pulumi_equinix-0.9.1/pulumi_equinix/networkedge/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.9.0/pulumi_equinix/networkedge/ssh_key.py` & `pulumi_equinix-0.9.1/pulumi_equinix/networkedge/ssh_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.9.0/pulumi_equinix/networkedge/ssh_user.py` & `pulumi_equinix-0.9.1/pulumi_equinix/networkedge/ssh_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.9.0/pulumi_equinix/provider.py` & `pulumi_equinix-0.9.1/pulumi_equinix/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.9.0/pulumi_equinix.egg-info/PKG-INFO` & `pulumi_equinix-0.9.1/pulumi_equinix.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-equinix
-Version: 0.9.0
+Version: 0.9.1
 Summary: A Pulumi package for creating and managing equinix cloud resources.
 Home-page: https://deploy.equinix.com/
 License: Apache-2.0
 Project-URL: Repository, https://github.com/equinix/pulumi-equinix
 Keywords: pulumi equinix category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `pulumi_equinix-0.9.0/pulumi_equinix.egg-info/SOURCES.txt` & `pulumi_equinix-0.9.1/pulumi_equinix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_equinix-0.9.0/setup.py` & `pulumi_equinix-0.9.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.9.0"
+VERSION = "0.9.1"
 def readme():
     try:
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "equinix Pulumi Package - Development Version"
```

