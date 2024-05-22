# Comparing `tmp/kthcloud-0.4.0a0.tar.gz` & `tmp/kthcloud-0.5.0a0.tar.gz`

## Comparing `kthcloud-0.4.0a0.tar` & `kthcloud-0.5.0a0.tar`

### file list

```diff
@@ -1,66 +1,67 @@
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v2/lib/.keep
--rw-r--r--   0        0        0     2557 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/__init__.py
--rw-r--r--   0        0        0    64414 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/_base_client.py
--rw-r--r--   0        0        0    17628 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/_client.py
--rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/_compat.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/_constants.py
--rw-r--r--   0        0        0     3244 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/_exceptions.py
--rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/_files.py
--rw-r--r--   0        0        0    26876 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/_models.py
--rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/_qs.py
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/_resource.py
--rw-r--r--   0        0        0    28489 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/_response.py
--rw-r--r--   0        0        0    10148 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/_streaming.py
--rw-r--r--   0        0        0     6142 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/_types.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/py.typed
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/_utils/__init__.py
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/_utils/_logs.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/_utils/_proxy.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/_utils/_streams.py
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/_utils/_sync.py
--rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/_utils/_transform.py
--rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/_utils/_typing.py
--rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/_utils/_utils.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/lib/.keep
--rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/resources/__init__.py
--rw-r--r--   0        0        0     8641 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/resources/gpu_groups.py
--rw-r--r--   0        0        0    20320 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/resources/gpu_leases.py
--rw-r--r--   0        0        0     7678 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/resources/snapshots.py
--rw-r--r--   0        0        0     5082 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/resources/vm_actions.py
--rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/resources/vms/__init__.py
--rw-r--r--   0        0        0     5200 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/resources/vms/snapshot.py
--rw-r--r--   0        0        0    21148 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/resources/vms/vms.py
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/types/__init__.py
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/types/gpu_group.py
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/types/gpu_group_list_params.py
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/types/gpu_group_list_response.py
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/types/gpu_lease_create_params.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/types/gpu_lease_created.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/types/gpu_lease_deleted.py
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/types/gpu_lease_list_params.py
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/types/gpu_lease_list_response.py
--rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/types/gpu_lease_read.py
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/types/gpu_lease_update_params.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/types/gpu_lease_updated.py
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/types/snapshot_list_params.py
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/types/snapshot_list_response.py
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/types/vm_action_create_params.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/types/vm_action_created.py
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/types/vm_create_params.py
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/types/vm_created.py
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/types/vm_deleted.py
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/types/vm_list_params.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/types/vm_list_response.py
--rw-r--r--   0        0        0     3180 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/types/vm_read.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/types/vm_snapshot_created.py
--rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/types/vm_update_params.py
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/types/vm_updated.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/types/shared/__init__.py
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/types/shared/vm_snapshot_read.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/types/vms/__init__.py
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/types/vms/vm_snapshot_deleted.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/.gitignore
--rw-r--r--   0        0        0    11351 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/LICENSE
--rw-r--r--   0        0        0     4470 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/pyproject.toml
--rw-r--r--   0        0        0    12680 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/PKG-INFO
+-rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/__init__.py
+-rw-r--r--   0        0        0    64414 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/_base_client.py
+-rw-r--r--   0        0        0    17326 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/_client.py
+-rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/_compat.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/_constants.py
+-rw-r--r--   0        0        0     3224 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/_exceptions.py
+-rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/_files.py
+-rw-r--r--   0        0        0    26876 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/_models.py
+-rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/_qs.py
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/_resource.py
+-rw-r--r--   0        0        0    28387 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/_response.py
+-rw-r--r--   0        0        0    10108 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/_streaming.py
+-rw-r--r--   0        0        0     6129 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/_types.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/py.typed
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/_utils/__init__.py
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/_utils/_logs.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/_utils/_proxy.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/_utils/_streams.py
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/_utils/_sync.py
+-rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/_utils/_transform.py
+-rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/_utils/_typing.py
+-rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/_utils/_utils.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/lib/.keep
+-rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/resources/__init__.py
+-rw-r--r--   0        0        0     8641 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/resources/gpu_groups.py
+-rw-r--r--   0        0        0    20320 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/resources/gpu_leases.py
+-rw-r--r--   0        0        0     7678 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/resources/snapshots.py
+-rw-r--r--   0        0        0     5082 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/resources/vm_actions.py
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/resources/vms/__init__.py
+-rw-r--r--   0        0        0     5200 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/resources/vms/snapshot.py
+-rw-r--r--   0        0        0    21148 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/resources/vms/vms.py
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/types/__init__.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/types/gpu_group.py
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/types/gpu_group_list_params.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/types/gpu_group_list_response.py
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/types/gpu_lease_create_params.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/types/gpu_lease_created.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/types/gpu_lease_deleted.py
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/types/gpu_lease_list_params.py
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/types/gpu_lease_list_response.py
+-rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/types/gpu_lease_read.py
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/types/gpu_lease_update_params.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/types/gpu_lease_updated.py
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/types/snapshot_list_params.py
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/types/snapshot_list_response.py
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/types/vm_action_create_params.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/types/vm_action_created.py
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/types/vm_create_params.py
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/types/vm_created.py
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/types/vm_deleted.py
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/types/vm_list_params.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/types/vm_list_response.py
+-rw-r--r--   0        0        0     3180 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/types/vm_read.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/types/vm_snapshot_created.py
+-rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/types/vm_update_params.py
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/types/vm_updated.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/types/shared/__init__.py
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/types/shared/vm_snapshot_read.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/types/vms/__init__.py
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud/types/vms/vm_snapshot_deleted.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud_go_deploy_v2/lib/.keep
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/src/kthcloud_go_deploy_v_/lib/.keep
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/.gitignore
+-rw-r--r--   0        0        0    11338 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/LICENSE
+-rw-r--r--   0        0        0     4405 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/pyproject.toml
+-rw-r--r--   0        0        0    12219 2020-02-02 00:00:00.000000 kthcloud-0.5.0a0/PKG-INFO
```

### Comparing `kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/__init__.py` & `kthcloud-0.5.0a0/src/kthcloud/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,38 +3,38 @@
 from . import types
 from ._types import NOT_GIVEN, NoneType, NotGiven, Transport, ProxiesTypes
 from ._utils import file_from_path
 from ._client import (
     Client,
     Stream,
     Timeout,
+    Kthcloud,
     Transport,
     AsyncClient,
     AsyncStream,
+    AsyncKthcloud,
     RequestOptions,
-    KthcloudGoDeployV2,
-    AsyncKthcloudGoDeployV2,
 )
 from ._models import BaseModel
 from ._version import __title__, __version__
 from ._response import APIResponse as APIResponse, AsyncAPIResponse as AsyncAPIResponse
 from ._constants import DEFAULT_TIMEOUT, DEFAULT_MAX_RETRIES, DEFAULT_CONNECTION_LIMITS
 from ._exceptions import (
     APIError,
     ConflictError,
+    KthcloudError,
     NotFoundError,
     APIStatusError,
     RateLimitError,
     APITimeoutError,
     BadRequestError,
     APIConnectionError,
     AuthenticationError,
     InternalServerError,
     PermissionDeniedError,
-    KthcloudGoDeployV2Error,
     UnprocessableEntityError,
     APIResponseValidationError,
 )
 from ._base_client import DefaultHttpxClient, DefaultAsyncHttpxClient
 from ._utils._logs import setup_logging as _setup_logging
 
 __all__ = [
@@ -42,15 +42,15 @@
     "__version__",
     "__title__",
     "NoneType",
     "Transport",
     "ProxiesTypes",
     "NotGiven",
     "NOT_GIVEN",
-    "KthcloudGoDeployV2Error",
+    "KthcloudError",
     "APIError",
     "APIStatusError",
     "APITimeoutError",
     "APIConnectionError",
     "APIResponseValidationError",
     "BadRequestError",
     "AuthenticationError",
@@ -62,32 +62,32 @@
     "InternalServerError",
     "Timeout",
     "RequestOptions",
     "Client",
     "AsyncClient",
     "Stream",
     "AsyncStream",
-    "KthcloudGoDeployV2",
-    "AsyncKthcloudGoDeployV2",
+    "Kthcloud",
+    "AsyncKthcloud",
     "file_from_path",
     "BaseModel",
     "DEFAULT_TIMEOUT",
     "DEFAULT_MAX_RETRIES",
     "DEFAULT_CONNECTION_LIMITS",
     "DefaultHttpxClient",
     "DefaultAsyncHttpxClient",
 ]
 
 _setup_logging()
 
 # Update the __module__ attribute for exported symbols so that
 # error messages point to this module instead of the module
 # it was originally defined in, e.g.
-# kthcloud_go_deploy_v_._exceptions.NotFoundError -> kthcloud_go_deploy_v_.NotFoundError
+# kthcloud._exceptions.NotFoundError -> kthcloud.NotFoundError
 __locals = locals()
 for __name in __all__:
     if not __name.startswith("__"):
         try:
-            __locals[__name].__module__ = "kthcloud_go_deploy_v_"
+            __locals[__name].__module__ = "kthcloud"
         except (TypeError, AttributeError):
             # Some of our exported symbols are builtins which we can't set attributes for.
             pass
```

### Comparing `kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/_base_client.py` & `kthcloud-0.5.0a0/src/kthcloud/_base_client.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/_client.py` & `kthcloud-0.5.0a0/src/kthcloud/_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,42 +21,42 @@
 )
 from ._utils import (
     is_given,
     get_async_library,
 )
 from ._version import __version__
 from ._streaming import Stream as Stream, AsyncStream as AsyncStream
-from ._exceptions import APIStatusError, KthcloudGoDeployV2Error
+from ._exceptions import KthcloudError, APIStatusError
 from ._base_client import (
     DEFAULT_MAX_RETRIES,
     SyncAPIClient,
     AsyncAPIClient,
 )
 
 __all__ = [
     "Timeout",
     "Transport",
     "ProxiesTypes",
     "RequestOptions",
     "resources",
-    "KthcloudGoDeployV2",
-    "AsyncKthcloudGoDeployV2",
+    "Kthcloud",
+    "AsyncKthcloud",
     "Client",
     "AsyncClient",
 ]
 
 
-class KthcloudGoDeployV2(SyncAPIClient):
+class Kthcloud(SyncAPIClient):
     gpu_groups: resources.GPUGroupsResource
     gpu_leases: resources.GPULeasesResource
     snapshots: resources.SnapshotsResource
     vm_actions: resources.VmActionsResource
     vms: resources.VmsResource
-    with_raw_response: KthcloudGoDeployV2WithRawResponse
-    with_streaming_response: KthcloudGoDeployV2WithStreamedResponse
+    with_raw_response: KthcloudWithRawResponse
+    with_streaming_response: KthcloudWithStreamedResponse
 
     # client options
     api_key: str
 
     def __init__(
         self,
         *,
@@ -76,28 +76,28 @@
         #
         # This parameter may be removed or changed in the future.
         # If you rely on this feature, please open a GitHub issue
         # outlining your use-case to help us decide if it should be
         # part of our public interface in the future.
         _strict_response_validation: bool = False,
     ) -> None:
-        """Construct a new synchronous kthcloud-go-deploy-v2 client instance.
+        """Construct a new synchronous kthcloud client instance.
 
         This automatically infers the `api_key` argument from the `KTHCLOUD_API_KEY` environment variable if it is not provided.
         """
         if api_key is None:
             api_key = os.environ.get("KTHCLOUD_API_KEY")
         if api_key is None:
-            raise KthcloudGoDeployV2Error(
+            raise KthcloudError(
                 "The api_key client option must be set either by passing api_key to the client or by setting the KTHCLOUD_API_KEY environment variable"
             )
         self.api_key = api_key
 
         if base_url is None:
-            base_url = os.environ.get("KTHCLOUD_GO_DEPLOY_V2_BASE_URL")
+            base_url = os.environ.get("KTHCLOUD_BASE_URL")
         if base_url is None:
             base_url = f"https://api.cloud.cbh.kth.se/deploy/"
 
         super().__init__(
             version=__version__,
             base_url=base_url,
             max_retries=max_retries,
@@ -109,16 +109,16 @@
         )
 
         self.gpu_groups = resources.GPUGroupsResource(self)
         self.gpu_leases = resources.GPULeasesResource(self)
         self.snapshots = resources.SnapshotsResource(self)
         self.vm_actions = resources.VmActionsResource(self)
         self.vms = resources.VmsResource(self)
-        self.with_raw_response = KthcloudGoDeployV2WithRawResponse(self)
-        self.with_streaming_response = KthcloudGoDeployV2WithStreamedResponse(self)
+        self.with_raw_response = KthcloudWithRawResponse(self)
+        self.with_streaming_response = KthcloudWithStreamedResponse(self)
 
     @property
     @override
     def qs(self) -> Querystring:
         return Querystring(array_format="comma")
 
     @property
@@ -217,22 +217,22 @@
             return _exceptions.RateLimitError(err_msg, response=response, body=body)
 
         if response.status_code >= 500:
             return _exceptions.InternalServerError(err_msg, response=response, body=body)
         return APIStatusError(err_msg, response=response, body=body)
 
 
-class AsyncKthcloudGoDeployV2(AsyncAPIClient):
+class AsyncKthcloud(AsyncAPIClient):
     gpu_groups: resources.AsyncGPUGroupsResource
     gpu_leases: resources.AsyncGPULeasesResource
     snapshots: resources.AsyncSnapshotsResource
     vm_actions: resources.AsyncVmActionsResource
     vms: resources.AsyncVmsResource
-    with_raw_response: AsyncKthcloudGoDeployV2WithRawResponse
-    with_streaming_response: AsyncKthcloudGoDeployV2WithStreamedResponse
+    with_raw_response: AsyncKthcloudWithRawResponse
+    with_streaming_response: AsyncKthcloudWithStreamedResponse
 
     # client options
     api_key: str
 
     def __init__(
         self,
         *,
@@ -252,28 +252,28 @@
         #
         # This parameter may be removed or changed in the future.
         # If you rely on this feature, please open a GitHub issue
         # outlining your use-case to help us decide if it should be
         # part of our public interface in the future.
         _strict_response_validation: bool = False,
     ) -> None:
-        """Construct a new async kthcloud-go-deploy-v2 client instance.
+        """Construct a new async kthcloud client instance.
 
         This automatically infers the `api_key` argument from the `KTHCLOUD_API_KEY` environment variable if it is not provided.
         """
         if api_key is None:
             api_key = os.environ.get("KTHCLOUD_API_KEY")
         if api_key is None:
-            raise KthcloudGoDeployV2Error(
+            raise KthcloudError(
                 "The api_key client option must be set either by passing api_key to the client or by setting the KTHCLOUD_API_KEY environment variable"
             )
         self.api_key = api_key
 
         if base_url is None:
-            base_url = os.environ.get("KTHCLOUD_GO_DEPLOY_V2_BASE_URL")
+            base_url = os.environ.get("KTHCLOUD_BASE_URL")
         if base_url is None:
             base_url = f"https://api.cloud.cbh.kth.se/deploy/"
 
         super().__init__(
             version=__version__,
             base_url=base_url,
             max_retries=max_retries,
@@ -285,16 +285,16 @@
         )
 
         self.gpu_groups = resources.AsyncGPUGroupsResource(self)
         self.gpu_leases = resources.AsyncGPULeasesResource(self)
         self.snapshots = resources.AsyncSnapshotsResource(self)
         self.vm_actions = resources.AsyncVmActionsResource(self)
         self.vms = resources.AsyncVmsResource(self)
-        self.with_raw_response = AsyncKthcloudGoDeployV2WithRawResponse(self)
-        self.with_streaming_response = AsyncKthcloudGoDeployV2WithStreamedResponse(self)
+        self.with_raw_response = AsyncKthcloudWithRawResponse(self)
+        self.with_streaming_response = AsyncKthcloudWithStreamedResponse(self)
 
     @property
     @override
     def qs(self) -> Querystring:
         return Querystring(array_format="comma")
 
     @property
@@ -393,46 +393,46 @@
             return _exceptions.RateLimitError(err_msg, response=response, body=body)
 
         if response.status_code >= 500:
             return _exceptions.InternalServerError(err_msg, response=response, body=body)
         return APIStatusError(err_msg, response=response, body=body)
 
 
-class KthcloudGoDeployV2WithRawResponse:
-    def __init__(self, client: KthcloudGoDeployV2) -> None:
+class KthcloudWithRawResponse:
+    def __init__(self, client: Kthcloud) -> None:
         self.gpu_groups = resources.GPUGroupsResourceWithRawResponse(client.gpu_groups)
         self.gpu_leases = resources.GPULeasesResourceWithRawResponse(client.gpu_leases)
         self.snapshots = resources.SnapshotsResourceWithRawResponse(client.snapshots)
         self.vm_actions = resources.VmActionsResourceWithRawResponse(client.vm_actions)
         self.vms = resources.VmsResourceWithRawResponse(client.vms)
 
 
-class AsyncKthcloudGoDeployV2WithRawResponse:
-    def __init__(self, client: AsyncKthcloudGoDeployV2) -> None:
+class AsyncKthcloudWithRawResponse:
+    def __init__(self, client: AsyncKthcloud) -> None:
         self.gpu_groups = resources.AsyncGPUGroupsResourceWithRawResponse(client.gpu_groups)
         self.gpu_leases = resources.AsyncGPULeasesResourceWithRawResponse(client.gpu_leases)
         self.snapshots = resources.AsyncSnapshotsResourceWithRawResponse(client.snapshots)
         self.vm_actions = resources.AsyncVmActionsResourceWithRawResponse(client.vm_actions)
         self.vms = resources.AsyncVmsResourceWithRawResponse(client.vms)
 
 
-class KthcloudGoDeployV2WithStreamedResponse:
-    def __init__(self, client: KthcloudGoDeployV2) -> None:
+class KthcloudWithStreamedResponse:
+    def __init__(self, client: Kthcloud) -> None:
         self.gpu_groups = resources.GPUGroupsResourceWithStreamingResponse(client.gpu_groups)
         self.gpu_leases = resources.GPULeasesResourceWithStreamingResponse(client.gpu_leases)
         self.snapshots = resources.SnapshotsResourceWithStreamingResponse(client.snapshots)
         self.vm_actions = resources.VmActionsResourceWithStreamingResponse(client.vm_actions)
         self.vms = resources.VmsResourceWithStreamingResponse(client.vms)
 
 
-class AsyncKthcloudGoDeployV2WithStreamedResponse:
-    def __init__(self, client: AsyncKthcloudGoDeployV2) -> None:
+class AsyncKthcloudWithStreamedResponse:
+    def __init__(self, client: AsyncKthcloud) -> None:
         self.gpu_groups = resources.AsyncGPUGroupsResourceWithStreamingResponse(client.gpu_groups)
         self.gpu_leases = resources.AsyncGPULeasesResourceWithStreamingResponse(client.gpu_leases)
         self.snapshots = resources.AsyncSnapshotsResourceWithStreamingResponse(client.snapshots)
         self.vm_actions = resources.AsyncVmActionsResourceWithStreamingResponse(client.vm_actions)
         self.vms = resources.AsyncVmsResourceWithStreamingResponse(client.vms)
 
 
-Client = KthcloudGoDeployV2
+Client = Kthcloud
 
-AsyncClient = AsyncKthcloudGoDeployV2
+AsyncClient = AsyncKthcloud
```

### Comparing `kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/_compat.py` & `kthcloud-0.5.0a0/src/kthcloud/_compat.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/_exceptions.py` & `kthcloud-0.5.0a0/src/kthcloud/_exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,19 +14,19 @@
     "ConflictError",
     "UnprocessableEntityError",
     "RateLimitError",
     "InternalServerError",
 ]
 
 
-class KthcloudGoDeployV2Error(Exception):
+class KthcloudError(Exception):
     pass
 
 
-class APIError(KthcloudGoDeployV2Error):
+class APIError(KthcloudError):
     message: str
     request: httpx.Request
 
     body: object | None
     """The API response body.
 
     If the API responded with a valid JSON structure then this property will be the
```

### Comparing `kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/_files.py` & `kthcloud-0.5.0a0/src/kthcloud/_files.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/_models.py` & `kthcloud-0.5.0a0/src/kthcloud/_models.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/_qs.py` & `kthcloud-0.5.0a0/src/kthcloud/_qs.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/_resource.py` & `kthcloud-0.5.0a0/src/kthcloud/_resource.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,37 +4,37 @@
 
 import time
 from typing import TYPE_CHECKING
 
 import anyio
 
 if TYPE_CHECKING:
-    from ._client import KthcloudGoDeployV2, AsyncKthcloudGoDeployV2
+    from ._client import Kthcloud, AsyncKthcloud
 
 
 class SyncAPIResource:
-    _client: KthcloudGoDeployV2
+    _client: Kthcloud
 
-    def __init__(self, client: KthcloudGoDeployV2) -> None:
+    def __init__(self, client: Kthcloud) -> None:
         self._client = client
         self._get = client.get
         self._post = client.post
         self._patch = client.patch
         self._put = client.put
         self._delete = client.delete
         self._get_api_list = client.get_api_list
 
     def _sleep(self, seconds: float) -> None:
         time.sleep(seconds)
 
 
 class AsyncAPIResource:
-    _client: AsyncKthcloudGoDeployV2
+    _client: AsyncKthcloud
 
-    def __init__(self, client: AsyncKthcloudGoDeployV2) -> None:
+    def __init__(self, client: AsyncKthcloud) -> None:
         self._client = client
         self._get = client.get
         self._post = client.post
         self._patch = client.patch
         self._put = client.put
         self._delete = client.delete
         self._get_api_list = client.get_api_list
```

### Comparing `kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/_response.py` & `kthcloud-0.5.0a0/src/kthcloud/_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 import pydantic
 
 from ._types import NoneType
 from ._utils import is_given, extract_type_arg, is_annotated_type, extract_type_var_from_base
 from ._models import BaseModel, is_basemodel
 from ._constants import RAW_RESPONSE_HEADER, OVERRIDE_CAST_TO_HEADER
 from ._streaming import Stream, AsyncStream, is_stream_class_type, extract_stream_chunk_type
-from ._exceptions import KthcloudGoDeployV2Error, APIResponseValidationError
+from ._exceptions import KthcloudError, APIResponseValidationError
 
 if TYPE_CHECKING:
     from ._models import FinalRequestOptions
     from ._base_client import BaseClient
 
 
 P = ParamSpec("P")
@@ -199,17 +199,15 @@
             # the response class ourselves but that is something that should be supported directly in httpx
             # as it would be easy to incorrectly construct the Response object due to the multitude of arguments.
             if cast_to != httpx.Response:
                 raise ValueError(f"Subclasses of httpx.Response cannot be passed to `cast_to`")
             return cast(R, response)
 
         if inspect.isclass(origin) and not issubclass(origin, BaseModel) and issubclass(origin, pydantic.BaseModel):
-            raise TypeError(
-                "Pydantic models must subclass our base model type, e.g. `from kthcloud_go_deploy_v_ import BaseModel`"
-            )
+            raise TypeError("Pydantic models must subclass our base model type, e.g. `from kthcloud import BaseModel`")
 
         if (
             cast_to is not object
             and not origin is list
             and not origin is dict
             and not origin is Union
             and not issubclass(origin, BaseModel)
@@ -269,15 +267,15 @@
 
         For lower-level control, see `.read()`, `.json()`, `.iter_bytes()`.
 
         You can customise the type that the response is parsed into through
         the `to` argument, e.g.
 
         ```py
-        from kthcloud_go_deploy_v_ import BaseModel
+        from kthcloud import BaseModel
 
 
         class MyModel(BaseModel):
             foo: str
 
 
         obj = response.parse(to=MyModel)
@@ -373,15 +371,15 @@
 
         For lower-level control, see `.read()`, `.json()`, `.iter_bytes()`.
 
         You can customise the type that the response is parsed into through
         the `to` argument, e.g.
 
         ```py
-        from kthcloud_go_deploy_v_ import BaseModel
+        from kthcloud import BaseModel
 
 
         class MyModel(BaseModel):
             foo: str
 
 
         obj = response.parse(to=MyModel)
@@ -544,19 +542,19 @@
             async for data in self.iter_bytes(chunk_size):
                 await f.write(data)
 
 
 class MissingStreamClassError(TypeError):
     def __init__(self) -> None:
         super().__init__(
-            "The `stream` argument was set to `True` but the `stream_cls` argument was not given. See `kthcloud_go_deploy_v_._streaming` for reference",
+            "The `stream` argument was set to `True` but the `stream_cls` argument was not given. See `kthcloud._streaming` for reference",
         )
 
 
-class StreamAlreadyConsumed(KthcloudGoDeployV2Error):
+class StreamAlreadyConsumed(KthcloudError):
     """
     Attempted to read or stream content, but the content has already
     been streamed.
 
     This can happen if you use a method like `.iter_lines()` and then attempt
     to read th entire response body afterwards, e.g.
```

### Comparing `kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/_streaming.py` & `kthcloud-0.5.0a0/src/kthcloud/_streaming.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from typing_extensions import Self, Protocol, TypeGuard, override, get_origin, runtime_checkable
 
 import httpx
 
 from ._utils import extract_type_var_from_base
 
 if TYPE_CHECKING:
-    from ._client import KthcloudGoDeployV2, AsyncKthcloudGoDeployV2
+    from ._client import Kthcloud, AsyncKthcloud
 
 
 _T = TypeVar("_T")
 
 
 class Stream(Generic[_T]):
     """Provides the core interface to iterate over a synchronous stream response."""
@@ -26,15 +26,15 @@
     _decoder: SSEBytesDecoder
 
     def __init__(
         self,
         *,
         cast_to: type[_T],
         response: httpx.Response,
-        client: KthcloudGoDeployV2,
+        client: Kthcloud,
     ) -> None:
         self.response = response
         self._cast_to = cast_to
         self._client = client
         self._decoder = client._make_sse_decoder()
         self._iterator = self.__stream__()
 
@@ -89,15 +89,15 @@
     _decoder: SSEDecoder | SSEBytesDecoder
 
     def __init__(
         self,
         *,
         cast_to: type[_T],
         response: httpx.Response,
-        client: AsyncKthcloudGoDeployV2,
+        client: AsyncKthcloud,
     ) -> None:
         self.response = response
         self._cast_to = cast_to
         self._client = client
         self._decoder = client._make_sse_decoder()
         self._iterator = self.__stream__()
```

### Comparing `kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/_types.py` & `kthcloud-0.5.0a0/src/kthcloud/_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 # method that uses `ResponseT` which would lead to an unacceptable
 # amount of code duplication and make it unreadable. See _base_client.py
 # for example usage.
 #
 # This unfortunately means that you will either have
 # to import this type and pass it explicitly:
 #
-# from kthcloud_go_deploy_v_ import NoneType
+# from kthcloud import NoneType
 # client.get('/foo', cast_to=NoneType)
 #
 # or build it yourself:
 #
 # client.get('/foo', cast_to=type(None))
 if TYPE_CHECKING:
     NoneType: Type[None]
```

### Comparing `kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/_utils/__init__.py` & `kthcloud-0.5.0a0/src/kthcloud/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/_utils/_logs.py` & `kthcloud-0.5.0a0/src/kthcloud/_utils/_logs.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import os
 import logging
 
-logger: logging.Logger = logging.getLogger("kthcloud_go_deploy_v_")
+logger: logging.Logger = logging.getLogger("kthcloud")
 httpx_logger: logging.Logger = logging.getLogger("httpx")
 
 
 def _basic_config() -> None:
-    # e.g. [2023-10-05 14:12:26 - kthcloud_go_deploy_v_._base_client:818 - DEBUG] HTTP Request: POST http://127.0.0.1:4010/foo/bar "200 OK"
+    # e.g. [2023-10-05 14:12:26 - kthcloud._base_client:818 - DEBUG] HTTP Request: POST http://127.0.0.1:4010/foo/bar "200 OK"
     logging.basicConfig(
         format="[%(asctime)s - %(name)s:%(lineno)d - %(levelname)s] %(message)s",
         datefmt="%Y-%m-%d %H:%M:%S",
     )
 
 
 def setup_logging() -> None:
-    env = os.environ.get("KTHCLOUD_GO_DEPLOY_V2_LOG")
+    env = os.environ.get("KTHCLOUD_LOG")
     if env == "debug":
         _basic_config()
         logger.setLevel(logging.DEBUG)
         httpx_logger.setLevel(logging.DEBUG)
     elif env == "info":
         _basic_config()
         logger.setLevel(logging.INFO)
```

### Comparing `kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/_utils/_proxy.py` & `kthcloud-0.5.0a0/src/kthcloud/_utils/_proxy.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/_utils/_sync.py` & `kthcloud-0.5.0a0/src/kthcloud/_utils/_sync.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/_utils/_transform.py` & `kthcloud-0.5.0a0/src/kthcloud/_utils/_transform.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/_utils/_typing.py` & `kthcloud-0.5.0a0/src/kthcloud/_utils/_typing.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/_utils/_utils.py` & `kthcloud-0.5.0a0/src/kthcloud/_utils/_utils.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/resources/__init__.py` & `kthcloud-0.5.0a0/src/kthcloud/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/resources/gpu_groups.py` & `kthcloud-0.5.0a0/src/kthcloud/resources/gpu_groups.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/resources/gpu_leases.py` & `kthcloud-0.5.0a0/src/kthcloud/resources/gpu_leases.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/resources/snapshots.py` & `kthcloud-0.5.0a0/src/kthcloud/resources/snapshots.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/resources/vm_actions.py` & `kthcloud-0.5.0a0/src/kthcloud/resources/vm_actions.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/resources/vms/__init__.py` & `kthcloud-0.5.0a0/src/kthcloud/resources/vms/__init__.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/resources/vms/snapshot.py` & `kthcloud-0.5.0a0/src/kthcloud/resources/vms/snapshot.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/resources/vms/vms.py` & `kthcloud-0.5.0a0/src/kthcloud/resources/vms/vms.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/types/__init__.py` & `kthcloud-0.5.0a0/src/kthcloud/types/__init__.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/types/gpu_group.py` & `kthcloud-0.5.0a0/src/kthcloud/types/gpu_group.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/types/gpu_lease_create_params.py` & `kthcloud-0.5.0a0/src/kthcloud/types/gpu_lease_create_params.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/types/gpu_lease_list_params.py` & `kthcloud-0.5.0a0/src/kthcloud/types/gpu_lease_list_params.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/types/gpu_lease_read.py` & `kthcloud-0.5.0a0/src/kthcloud/types/gpu_lease_read.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/types/gpu_lease_update_params.py` & `kthcloud-0.5.0a0/src/kthcloud/types/gpu_lease_update_params.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/types/vm_create_params.py` & `kthcloud-0.5.0a0/src/kthcloud/types/vm_create_params.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/types/vm_list_params.py` & `kthcloud-0.5.0a0/src/kthcloud/types/vm_list_params.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/types/vm_read.py` & `kthcloud-0.5.0a0/src/kthcloud/types/vm_read.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/types/vm_update_params.py` & `kthcloud-0.5.0a0/src/kthcloud/types/vm_update_params.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.4.0a0/LICENSE` & `kthcloud-0.5.0a0/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright 2024 Kthcloud Go Deploy V2
+   Copyright 2024 Kthcloud
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `kthcloud-0.4.0a0/pyproject.toml` & `kthcloud-0.5.0a0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
 name = "kthcloud"
-version = "0.4.0-alpha"
-description = "The official Python library for the kthcloud-go-deploy-v2 API"
+version = "0.5.0-alpha"
+description = "The official Python library for the kthcloud API"
 dynamic = ["readme"]
 license = "Apache-2.0"
 authors = [
-{ name = "Kthcloud Go Deploy V2", email = "dev@cloud.cbh.kth.se" },
+{ name = "Kthcloud", email = "dev@cloud.cbh.kth.se" },
 ]
 dependencies = [
     "httpx>=0.23.0, <1",
     "pydantic>=1.9.0, <3",
     "typing-extensions>=4.7, <5",
     "anyio>=3.5.0, <5",
     "distro>=1.7.0, <2",
@@ -80,28 +80,28 @@
 "fix:ruff" = "ruff --fix ."
 
 typecheck = { chain = [
   "typecheck:pyright",
   "typecheck:mypy"
 ]}
 "typecheck:pyright" = "pyright"
-"typecheck:verify-types" = "pyright --verifytypes kthcloud_go_deploy_v_ --ignoreexternal"
+"typecheck:verify-types" = "pyright --verifytypes kthcloud --ignoreexternal"
 "typecheck:mypy" = "mypy ."
 
 [build-system]
 requires = ["hatchling", "hatch-fancy-pypi-readme"]
 build-backend = "hatchling.build"
 
 [tool.hatch.build]
 include = [
   "src/*"
 ]
 
 [tool.hatch.build.targets.wheel]
-packages = ["src/kthcloud_go_deploy_v_"]
+packages = ["src/kthcloud"]
 
 [tool.hatch.metadata.hooks.fancy-pypi-readme]
 content-type = "text/markdown"
 
 [[tool.hatch.metadata.hooks.fancy-pypi-readme.fragments]]
 path = "README.md"
 
@@ -183,14 +183,14 @@
 "functools.lru_cache".msg = "This function does not retain type information for the wrapped function's arguments; The `lru_cache` function from `_utils` should be used instead"
 
 [tool.ruff.lint.isort]
 length-sort = true
 length-sort-straight = true
 combine-as-imports = true
 extra-standard-library = ["typing_extensions"]
-known-first-party = ["kthcloud_go_deploy_v_", "tests"]
+known-first-party = ["kthcloud", "tests"]
 
 [tool.ruff.per-file-ignores]
 "bin/**.py" = ["T201", "T203"]
 "scripts/**.py" = ["T201", "T203"]
 "tests/**.py" = ["T201", "T203"]
 "examples/**.py" = ["T201", "T203"]
```

### Comparing `kthcloud-0.4.0a0/PKG-INFO` & `kthcloud-0.5.0a0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.3
 Name: kthcloud
-Version: 0.4.0a0
-Summary: The official Python library for the kthcloud-go-deploy-v2 API
+Version: 0.5.0a0
+Summary: The official Python library for the kthcloud API
 Project-URL: Homepage, https://github.com/kthcloud/python-sdk
 Project-URL: Repository, https://github.com/kthcloud/python-sdk
-Author-email: Kthcloud Go Deploy V2 <dev@cloud.cbh.kth.se>
+Author-email: Kthcloud <dev@cloud.cbh.kth.se>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: OS Independent
@@ -28,43 +28,47 @@
 Requires-Dist: distro<2,>=1.7.0
 Requires-Dist: httpx<1,>=0.23.0
 Requires-Dist: pydantic<3,>=1.9.0
 Requires-Dist: sniffio
 Requires-Dist: typing-extensions<5,>=4.7
 Description-Content-Type: text/markdown
 
+
+
+
 # kthcloud Python SDK
 
+
 [![PyPI version](https://img.shields.io/pypi/v/kthcloud.svg)](https://pypi.org/project/kthcloud/)
 
-The Kthcloud Go Deploy V2 Python library provides convenient access to the Kthcloud Go Deploy V2 REST API from any Python 3.7+
+The Kthcloud Python library provides convenient access to the Kthcloud REST API from any Python 3.7+
 application. The library includes type definitions for all request params and response fields,
 and offers both synchronous and asynchronous clients powered by [httpx](https://github.com/encode/httpx).
 
 It is generated with [Stainless](https://www.stainlessapi.com/).
 
 ## Documentation
 
-The REST API documentation can be found [on github.com](https://github.com/kthcloud/go-deploy). The full API of this library can be found in [api.md](https://github.com/kthcloud/python-sdk/tree/main/api.md).
+The REST API documentation can be found [on docs.cloud.cbh.kth.se](https://docs.cloud.cbh.kth.se/). The full API of this library can be found in [api.md](https://github.com/kthcloud/python-sdk/tree/main/api.md).
 
 ## Installation
 
 ```sh
 # install from PyPI
 pip install --pre kthcloud
 ```
 
 ## Usage
 
 The full API of this library can be found in [api.md](https://github.com/kthcloud/python-sdk/tree/main/api.md).
 
 ```python
-from kthcloud_go_deploy_v_ import KthcloudGoDeployV2
+from kthcloud import Kthcloud
 
-client = KthcloudGoDeployV2()
+client = Kthcloud()
 
 vm_created = client.vms.create(
     cpu_cores=1,
     disk_size=10,
     name="xxx",
     ram=1,
     ssh_public_key="string",
@@ -75,21 +79,21 @@
 While you can provide an `api_key` keyword argument,
 we recommend using [python-dotenv](https://pypi.org/project/python-dotenv/)
 to add `KTHCLOUD_API_KEY="My API Key"` to your `.env` file
 so that your API Key is not stored in source control.
 
 ## Async usage
 
-Simply import `AsyncKthcloudGoDeployV2` instead of `KthcloudGoDeployV2` and use `await` with each API call:
+Simply import `AsyncKthcloud` instead of `Kthcloud` and use `await` with each API call:
 
 ```python
 import asyncio
-from kthcloud_go_deploy_v_ import AsyncKthcloudGoDeployV2
+from kthcloud import AsyncKthcloud
 
-client = AsyncKthcloudGoDeployV2()
+client = AsyncKthcloud()
 
 
 async def main() -> None:
     vm_created = await client.vms.create(
         cpu_cores=1,
         disk_size=10,
         name="xxx",
@@ -111,41 +115,41 @@
 - Serializing back into JSON, `model.to_json()`
 - Converting to a dictionary, `model.to_dict()`
 
 Typed requests and responses provide autocomplete and documentation within your editor. If you would like to see type errors in VS Code to help catch bugs earlier, set `python.analysis.typeCheckingMode` to `basic`.
 
 ## Handling errors
 
-When the library is unable to connect to the API (for example, due to network connection problems or a timeout), a subclass of `kthcloud_go_deploy_v_.APIConnectionError` is raised.
+When the library is unable to connect to the API (for example, due to network connection problems or a timeout), a subclass of `kthcloud.APIConnectionError` is raised.
 
 When the API returns a non-success status code (that is, 4xx or 5xx
-response), a subclass of `kthcloud_go_deploy_v_.APIStatusError` is raised, containing `status_code` and `response` properties.
+response), a subclass of `kthcloud.APIStatusError` is raised, containing `status_code` and `response` properties.
 
-All errors inherit from `kthcloud_go_deploy_v_.APIError`.
+All errors inherit from `kthcloud.APIError`.
 
 ```python
-import kthcloud_go_deploy_v_
-from kthcloud_go_deploy_v_ import KthcloudGoDeployV2
+import kthcloud
+from kthcloud import Kthcloud
 
-client = KthcloudGoDeployV2()
+client = Kthcloud()
 
 try:
     client.vms.create(
         cpu_cores=1,
         disk_size=10,
         name="xxx",
         ram=1,
         ssh_public_key="string",
     )
-except kthcloud_go_deploy_v_.APIConnectionError as e:
+except kthcloud.APIConnectionError as e:
     print("The server could not be reached")
     print(e.__cause__)  # an underlying Exception, likely raised within httpx.
-except kthcloud_go_deploy_v_.RateLimitError as e:
+except kthcloud.RateLimitError as e:
     print("A 429 status code was received; we should back off a bit.")
-except kthcloud_go_deploy_v_.APIStatusError as e:
+except kthcloud.APIStatusError as e:
     print("Another non-200-range status code was received")
     print(e.status_code)
     print(e.response)
 ```
 
 Error codes are as followed:
 
@@ -165,18 +169,18 @@
 Certain errors are automatically retried 2 times by default, with a short exponential backoff.
 Connection errors (for example, due to a network connectivity problem), 408 Request Timeout, 409 Conflict,
 429 Rate Limit, and >=500 Internal errors are all retried by default.
 
 You can use the `max_retries` option to configure or disable retry settings:
 
 ```python
-from kthcloud_go_deploy_v_ import KthcloudGoDeployV2
+from kthcloud import Kthcloud
 
 # Configure the default for all requests:
-client = KthcloudGoDeployV2(
+client = Kthcloud(
     # default is 2
     max_retries=0,
 )
 
 # Or, configure per-request:
 client.with_options(max_retries=5).vms.create(
     cpu_cores=1,
@@ -189,24 +193,24 @@
 
 ### Timeouts
 
 By default requests time out after 1 minute. You can configure this with a `timeout` option,
 which accepts a float or an [`httpx.Timeout`](https://www.python-httpx.org/advanced/#fine-tuning-the-configuration) object:
 
 ```python
-from kthcloud_go_deploy_v_ import KthcloudGoDeployV2
+from kthcloud import Kthcloud
 
 # Configure the default for all requests:
-client = KthcloudGoDeployV2(
+client = Kthcloud(
     # 20 seconds (default is 1 minute)
     timeout=20.0,
 )
 
 # More granular control:
-client = KthcloudGoDeployV2(
+client = Kthcloud(
     timeout=httpx.Timeout(60.0, read=5.0, write=10.0, connect=2.0),
 )
 
 # Override per-request:
 client.with_options(timeout=5.0).vms.create(
     cpu_cores=1,
     disk_size=10,
@@ -222,18 +226,18 @@
 
 ## Advanced
 
 ### Logging
 
 We use the standard library [`logging`](https://docs.python.org/3/library/logging.html) module.
 
-You can enable logging by setting the environment variable `KTHCLOUD_GO_DEPLOY_V2_LOG` to `debug`.
+You can enable logging by setting the environment variable `KTHCLOUD_LOG` to `debug`.
 
 ```shell
-$ export KTHCLOUD_GO_DEPLOY_V2_LOG=debug
+$ export KTHCLOUD_LOG=debug
 ```
 
 ### How to tell whether `None` means `null` or missing
 
 In an API response, a field may be explicitly `null`, or missing entirely; in either case, its value is `None` in this library. You can differentiate the two cases with `.model_fields_set`:
 
 ```py
@@ -245,33 +249,33 @@
 ```
 
 ### Accessing raw response data (e.g. headers)
 
 The "raw" Response object can be accessed by prefixing `.with_raw_response.` to any HTTP method call, e.g.,
 
 ```py
-from kthcloud_go_deploy_v_ import KthcloudGoDeployV2
+from kthcloud import Kthcloud
 
-client = KthcloudGoDeployV2()
+client = Kthcloud()
 response = client.vms.with_raw_response.create(
     cpu_cores=1,
     disk_size=10,
     name="xxx",
     ram=1,
     ssh_public_key="string",
 )
 print(response.headers.get('X-My-Header'))
 
 vm = response.parse()  # get the object that `vms.create()` would have returned
 print(vm.id)
 ```
 
-These methods return an [`APIResponse`](https://github.com/kthcloud/python-sdk/tree/main/src/kthcloud_go_deploy_v_/_response.py) object.
+These methods return an [`APIResponse`](https://github.com/kthcloud/python-sdk/tree/main/src/kthcloud/_response.py) object.
 
-The async client returns an [`AsyncAPIResponse`](https://github.com/kthcloud/python-sdk/tree/main/src/kthcloud_go_deploy_v_/_response.py) with the same structure, the only difference being `await`able methods for reading the response content.
+The async client returns an [`AsyncAPIResponse`](https://github.com/kthcloud/python-sdk/tree/main/src/kthcloud/_response.py) with the same structure, the only difference being `await`able methods for reading the response content.
 
 #### `.with_streaming_response`
 
 The above interface eagerly reads the full response body when you make the request, which may not always be what you want.
 
 To stream the response body, use `.with_streaming_response` instead, which requires a context manager and only reads the response body once you call `.read()`, `.text()`, `.json()`, `.iter_bytes()`, `.iter_text()`, `.iter_lines()` or `.parse()`. In the async client, these are async methods.
 
@@ -331,18 +335,18 @@
 You can directly override the [httpx client](https://www.python-httpx.org/api/#client) to customize it for your use case, including:
 
 - Support for proxies
 - Custom transports
 - Additional [advanced](https://www.python-httpx.org/advanced/#client-instances) functionality
 
 ```python
-from kthcloud_go_deploy_v_ import KthcloudGoDeployV2, DefaultHttpxClient
+from kthcloud import Kthcloud, DefaultHttpxClient
 
-client = KthcloudGoDeployV2(
-    # Or use the `KTHCLOUD_GO_DEPLOY_V2_BASE_URL` env var
+client = Kthcloud(
+    # Or use the `KTHCLOUD_BASE_URL` env var
     base_url="http://my.test.server.example.com:8083",
     http_client=DefaultHttpxClient(
         proxies="http://my.test.proxy.example.com",
         transport=httpx.HTTPTransport(local_address="0.0.0.0"),
     ),
 )
 ```
```

