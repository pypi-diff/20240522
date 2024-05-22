# Comparing `tmp/catalystwan-0.33.6.post0.tar.gz` & `tmp/catalystwan-0.33.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "catalystwan-0.33.6.post0.tar", max compression
+gzip compressed data, was "catalystwan-0.33.7.tar", max compression
```

## Comparing `catalystwan-0.33.6.post0.tar` & `catalystwan-0.33.7.tar`

### file list

```diff
@@ -1,372 +1,345 @@
--rw-r--r--   0        0        0    11375 2024-05-22 16:20:45.952754 catalystwan-0.33.6.post0/LICENSE
--rw-r--r--   0        0        0    14173 2024-05-22 16:20:45.952754 catalystwan-0.33.6.post0/README.md
--rw-r--r--   0        0        0     2524 2024-05-22 16:20:45.952754 catalystwan-0.33.6.post0/catalystwan/__init__.py
--rw-r--r--   0        0        0     1533 2024-05-22 16:20:45.952754 catalystwan-0.33.6.post0/catalystwan/abstractions.py
--rw-r--r--   0        0        0        0 2024-05-22 16:20:45.952754 catalystwan-0.33.6.post0/catalystwan/api/__init__.py
--rw-r--r--   0        0        0     6689 2024-05-22 16:20:45.952754 catalystwan-0.33.6.post0/catalystwan/api/admin_tech_api.py
--rw-r--r--   0        0        0    14935 2024-05-22 16:20:45.952754 catalystwan-0.33.6.post0/catalystwan/api/administration.py
--rw-r--r--   0        0        0     6314 2024-05-22 16:20:45.952754 catalystwan-0.33.6.post0/catalystwan/api/alarms_api.py
--rw-r--r--   0        0        0     3220 2024-05-22 16:20:45.952754 catalystwan-0.33.6.post0/catalystwan/api/api_container.py
--rw-r--r--   0        0        0    11636 2024-05-22 16:20:45.952754 catalystwan-0.33.6.post0/catalystwan/api/basic_api.py
--rw-r--r--   0        0        0     2053 2024-05-22 16:20:45.952754 catalystwan-0.33.6.post0/catalystwan/api/config_device_inventory_api.py
--rw-r--r--   0        0        0     4301 2024-05-22 16:20:45.952754 catalystwan-0.33.6.post0/catalystwan/api/config_group_api.py
--rw-r--r--   0        0        0     4645 2024-05-22 16:20:45.952754 catalystwan-0.33.6.post0/catalystwan/api/configuration_groups/parcel.py
--rw-r--r--   0        0        0     1290 2024-05-22 16:20:45.952754 catalystwan-0.33.6.post0/catalystwan/api/configuration_groups/parcels/cellular_controller.py
--rw-r--r--   0        0        0     7315 2024-05-22 16:20:45.952754 catalystwan-0.33.6.post0/catalystwan/api/dashboard_api.py
--rw-r--r--   0        0        0     7360 2024-05-22 16:20:45.952754 catalystwan-0.33.6.post0/catalystwan/api/device_action_api.py
--rw-r--r--   0        0        0    15767 2024-05-22 16:20:45.952754 catalystwan-0.33.6.post0/catalystwan/api/feature_profile_api.py
--rw-r--r--   0        0        0     1919 2024-05-22 16:20:45.952754 catalystwan-0.33.6.post0/catalystwan/api/logs_api.py
--rw-r--r--   0        0        0     2449 2024-05-22 16:20:45.952754 catalystwan-0.33.6.post0/catalystwan/api/monitoring_status_api.py
--rw-r--r--   0        0        0     6036 2024-05-22 16:20:45.952754 catalystwan-0.33.6.post0/catalystwan/api/mtt_aaa_api.py
--rw-r--r--   0        0        0     4394 2024-05-22 16:20:45.952754 catalystwan-0.33.6.post0/catalystwan/api/omp_api.py
--rw-r--r--   0        0        0     5691 2024-05-22 16:20:45.952754 catalystwan-0.33.6.post0/catalystwan/api/packet_capture_api.py
--rw-r--r--   0        0        0     1654 2024-05-22 16:20:45.952754 catalystwan-0.33.6.post0/catalystwan/api/parcel_api.py
--rw-r--r--   0        0        0     5600 2024-05-22 16:20:45.952754 catalystwan-0.33.6.post0/catalystwan/api/partition_manager_api.py
--rw-r--r--   0        0        0    28976 2024-05-22 16:20:45.952754 catalystwan-0.33.6.post0/catalystwan/api/policy_api.py
--rw-r--r--   0        0        0     2284 2024-05-22 16:20:45.952754 catalystwan-0.33.6.post0/catalystwan/api/resource_pool_api.py
--rw-r--r--   0        0        0    11320 2024-05-22 16:20:45.952754 catalystwan-0.33.6.post0/catalystwan/api/software_action_api.py
--rw-r--r--   0        0        0     5473 2024-05-22 16:20:45.952754 catalystwan-0.33.6.post0/catalystwan/api/speedtest_api.py
--rw-r--r--   0        0        0     7149 2024-05-22 16:20:45.952754 catalystwan-0.33.6.post0/catalystwan/api/task_status_api.py
--rw-r--r--   0        0        0    29488 2024-05-22 16:20:45.956754 catalystwan-0.33.6.post0/catalystwan/api/template_api.py
--rw-r--r--   0        0        0     3547 2024-05-22 16:20:45.956754 catalystwan-0.33.6.post0/catalystwan/api/templates/README.md
--rw-r--r--   0        0        0      251 2024-05-22 16:20:45.956754 catalystwan-0.33.6.post0/catalystwan/api/templates/bool_str.py
--rw-r--r--   0        0        0     7430 2024-05-22 16:20:45.956754 catalystwan-0.33.6.post0/catalystwan/api/templates/cli_template.py
--rw-r--r--   0        0        0     3102 2024-05-22 16:20:45.956754 catalystwan-0.33.6.post0/catalystwan/api/templates/device_template/device_template.py
--rw-r--r--   0        0        0      571 2024-05-22 16:20:45.956754 catalystwan-0.33.6.post0/catalystwan/api/templates/device_template/device_template_payload.json.j2
--rw-r--r--   0        0        0      137 2024-05-22 16:20:45.956754 catalystwan-0.33.6.post0/catalystwan/api/templates/device_variable.py
--rw-r--r--   0        0        0     5011 2024-05-22 16:20:45.956754 catalystwan-0.33.6.post0/catalystwan/api/templates/feature_template.py
--rw-r--r--   0        0        0     6576 2024-05-22 16:20:45.956754 catalystwan-0.33.6.post0/catalystwan/api/templates/feature_template_field.py
--rw-r--r--   0        0        0      661 2024-05-22 16:20:45.956754 catalystwan-0.33.6.post0/catalystwan/api/templates/feature_template_payload.py
--rw-r--r--   0        0        0    12008 2024-05-22 16:20:45.956754 catalystwan-0.33.6.post0/catalystwan/api/templates/models/cisco_aaa_model.py
--rw-r--r--   0        0        0      995 2024-05-22 16:20:45.956754 catalystwan-0.33.6.post0/catalystwan/api/templates/models/cisco_banner_model.py
--rw-r--r--   0        0        0     2471 2024-05-22 16:20:45.956754 catalystwan-0.33.6.post0/catalystwan/api/templates/models/cisco_bfd_model.py
--rw-r--r--   0        0        0    22264 2024-05-22 16:20:45.956754 catalystwan-0.33.6.post0/catalystwan/api/templates/models/cisco_bgp_model.py
--rw-r--r--   0        0        0     5084 2024-05-22 16:20:45.956754 catalystwan-0.33.6.post0/catalystwan/api/templates/models/cisco_logging_model.py
--rw-r--r--   0        0        0     2615 2024-05-22 16:20:45.956754 catalystwan-0.33.6.post0/catalystwan/api/templates/models/cisco_ntp_model.py
--rw-r--r--   0        0        0     5581 2024-05-22 16:20:45.956754 catalystwan-0.33.6.post0/catalystwan/api/templates/models/cisco_omp_model.py
--rw-r--r--   0        0        0    10423 2024-05-22 16:20:45.956754 catalystwan-0.33.6.post0/catalystwan/api/templates/models/cisco_ospf.py
--rw-r--r--   0        0        0    21811 2024-05-22 16:20:45.956754 catalystwan-0.33.6.post0/catalystwan/api/templates/models/cisco_ospfv3.py
--rw-r--r--   0        0        0    16267 2024-05-22 16:20:45.956754 catalystwan-0.33.6.post0/catalystwan/api/templates/models/cisco_secure_internet_gateway.py
--rw-r--r--   0        0        0     4732 2024-05-22 16:20:45.956754 catalystwan-0.33.6.post0/catalystwan/api/templates/models/cisco_snmp_model.py
--rw-r--r--   0        0        0    14381 2024-05-22 16:20:45.956754 catalystwan-0.33.6.post0/catalystwan/api/templates/models/cisco_system.py
--rw-r--r--   0        0        0    37924 2024-05-22 16:20:45.956754 catalystwan-0.33.6.post0/catalystwan/api/templates/models/cisco_vpn_interface_model.py
--rw-r--r--   0        0        0    27169 2024-05-22 16:20:45.956754 catalystwan-0.33.6.post0/catalystwan/api/templates/models/cisco_vpn_model.py
--rw-r--r--   0        0        0      664 2024-05-22 16:20:45.956754 catalystwan-0.33.6.post0/catalystwan/api/templates/models/cli_template.py
--rw-r--r--   0        0        0     3112 2024-05-22 16:20:45.956754 catalystwan-0.33.6.post0/catalystwan/api/templates/models/omp_vsmart_model.py
--rw-r--r--   0        0        0     1000 2024-05-22 16:20:45.956754 catalystwan-0.33.6.post0/catalystwan/api/templates/models/security_vsmart_model.py
--rw-r--r--   0        0        0     1882 2024-05-22 16:20:45.956754 catalystwan-0.33.6.post0/catalystwan/api/templates/models/supported.py
--rw-r--r--   0        0        0     6234 2024-05-22 16:20:45.956754 catalystwan-0.33.6.post0/catalystwan/api/templates/models/system_vsmart_model.py
--rw-r--r--   0        0        0     2261 2024-05-22 16:20:45.956754 catalystwan-0.33.6.post0/catalystwan/api/templates/payloads/aaa/aaa_model.py
--rw-r--r--   0        0        0    11178 2024-05-22 16:20:45.956754 catalystwan-0.33.6.post0/catalystwan/api/templates/payloads/aaa/feature/aaa.json.j2
--rw-r--r--   0        0        0     1041 2024-05-22 16:20:45.956754 catalystwan-0.33.6.post0/catalystwan/api/templates/payloads/aaa/feature/accounting.json.j2
--rw-r--r--   0        0        0     4264 2024-05-22 16:20:45.956754 catalystwan-0.33.6.post0/catalystwan/api/templates/payloads/aaa/feature/radius.json.j2
--rw-r--r--   0        0        0     3735 2024-05-22 16:20:45.956754 catalystwan-0.33.6.post0/catalystwan/api/templates/payloads/aaa/feature/tacacs.json.j2
--rw-r--r--   0        0        0     1999 2024-05-22 16:20:45.956754 catalystwan-0.33.6.post0/catalystwan/api/templates/payloads/aaa/feature/user.json.j2
--rw-r--r--   0        0        0     2558 2024-05-22 16:20:45.956754 catalystwan-0.33.6.post0/catalystwan/api/templates/payloads/cisco_vpn/cisco_vpn_model.py
--rw-r--r--   0        0        0     4547 2024-05-22 16:20:45.956754 catalystwan-0.33.6.post0/catalystwan/api/templates/payloads/cisco_vpn/feature/cisco_vpn.json.j2
--rw-r--r--   0        0        0     1843 2024-05-22 16:20:45.956754 catalystwan-0.33.6.post0/catalystwan/api/templates/payloads/cisco_vpn/feature/dns.json.j2
--rw-r--r--   0        0        0     2247 2024-05-22 16:20:45.956754 catalystwan-0.33.6.post0/catalystwan/api/templates/payloads/cisco_vpn/feature/ipv4route.json.j2
--rw-r--r--   0        0        0     2098 2024-05-22 16:20:45.956754 catalystwan-0.33.6.post0/catalystwan/api/templates/payloads/cisco_vpn/feature/ipv6route.json.j2
--rw-r--r--   0        0        0      683 2024-05-22 16:20:45.956754 catalystwan-0.33.6.post0/catalystwan/api/templates/payloads/cisco_vpn/feature/mapping.json.j2
--rw-r--r--   0        0        0     7113 2024-05-22 16:20:45.956754 catalystwan-0.33.6.post0/catalystwan/api/templates/payloads/tenant/tenant.json.j2
--rw-r--r--   0        0        0     1460 2024-05-22 16:20:45.956754 catalystwan-0.33.6.post0/catalystwan/api/templates/payloads/tenant/tenant_model.py
--rw-r--r--   0        0        0     5013 2024-05-22 16:20:45.956754 catalystwan-0.33.6.post0/catalystwan/api/tenant_backup_restore_api.py
--rw-r--r--   0        0        0     4406 2024-05-22 16:20:45.956754 catalystwan-0.33.6.post0/catalystwan/api/tenant_management_api.py
--rw-r--r--   0        0        0     5090 2024-05-22 16:20:45.956754 catalystwan-0.33.6.post0/catalystwan/api/tenant_migration_api.py
--rw-r--r--   0        0        0    15887 2024-05-22 16:20:45.956754 catalystwan-0.33.6.post0/catalystwan/api/versions_utils.py
--rw-r--r--   0        0        0     7715 2024-05-22 16:20:45.956754 catalystwan-0.33.6.post0/catalystwan/api/virtual_image_action_api.py
--rw-r--r--   0        0        0    21802 2024-05-22 16:20:45.956754 catalystwan-0.33.6.post0/catalystwan/dataclasses.py
--rw-r--r--   0        0        0    25866 2024-05-22 16:20:45.956754 catalystwan-0.33.6.post0/catalystwan/endpoints/__init__.py
--rw-r--r--   0        0        0    11938 2024-05-22 16:20:45.956754 catalystwan-0.33.6.post0/catalystwan/endpoints/administration_user_and_group.py
--rw-r--r--   0        0        0     6731 2024-05-22 16:20:45.956754 catalystwan-0.33.6.post0/catalystwan/endpoints/certificate_management_device.py
--rw-r--r--   0        0        0     1476 2024-05-22 16:20:45.956754 catalystwan-0.33.6.post0/catalystwan/endpoints/certificate_management_vmanage.py
--rw-r--r--   0        0        0     4035 2024-05-22 16:20:45.956754 catalystwan-0.33.6.post0/catalystwan/endpoints/client.py
--rw-r--r--   0        0        0     2722 2024-05-22 16:20:45.956754 catalystwan-0.33.6.post0/catalystwan/endpoints/cluster_management.py
--rw-r--r--   0        0        0      983 2024-05-22 16:20:45.956754 catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/device/software_update.py
--rw-r--r--   0        0        0     9447 2024-05-22 16:20:45.956754 catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/disaster_recovery.py
--rw-r--r--   0        0        0     4037 2024-05-22 16:20:45.956754 catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/feature_profile/sdwan/policy_object.py
--rw-r--r--   0        0        0     2064 2024-05-22 16:20:45.956754 catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/feature_profile/sdwan/system.py
--rw-r--r--   0        0        0     4836 2024-05-22 16:20:45.960754 catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/feature_profile/sdwan/transport.py
--rw-r--r--   0        0        0     2028 2024-05-22 16:20:45.960754 catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/definition/access_control_list.py
--rw-r--r--   0        0        0     2091 2024-05-22 16:20:45.960754 catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/definition/access_control_list_ipv6.py
--rw-r--r--   0        0        0     2092 2024-05-22 16:20:45.960754 catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/definition/control.py
--rw-r--r--   0        0        0     2247 2024-05-22 16:20:45.960754 catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/definition/device_access.py
--rw-r--r--   0        0        0     2324 2024-05-22 16:20:45.960754 catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/definition/device_access_ipv6.py
--rw-r--r--   0        0        0     2174 2024-05-22 16:20:45.960754 catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/definition/hub_and_spoke.py
--rw-r--r--   0        0        0     2032 2024-05-22 16:20:45.960754 catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/definition/mesh.py
--rw-r--r--   0        0        0     2073 2024-05-22 16:20:45.960754 catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/definition/qos_map.py
--rw-r--r--   0        0        0     2132 2024-05-22 16:20:45.960754 catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/definition/rewrite.py
--rw-r--r--   0        0        0     2039 2024-05-22 16:20:45.960754 catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/definition/rule_set.py
--rw-r--r--   0        0        0     2159 2024-05-22 16:20:45.960754 catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/definition/security_group.py
--rw-r--r--   0        0        0     2104 2024-05-22 16:20:45.960754 catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/definition/traffic_data.py
--rw-r--r--   0        0        0     2263 2024-05-22 16:20:45.960754 catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/definition/vpn_membership.py
--rw-r--r--   0        0        0     2186 2024-05-22 16:20:45.960754 catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/definition/zone_based_firewall.py
--rw-r--r--   0        0        0     1793 2024-05-22 16:20:45.960754 catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/list/app.py
--rw-r--r--   0        0        0     1950 2024-05-22 16:20:45.960754 catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/list/app_probe.py
--rw-r--r--   0        0        0     1848 2024-05-22 16:20:45.960754 catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/list/as_path.py
--rw-r--r--   0        0        0     1870 2024-05-22 16:20:45.960754 catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/list/class_map.py
--rw-r--r--   0        0        0     1827 2024-05-22 16:20:45.960754 catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/list/color.py
--rw-r--r--   0        0        0     1911 2024-05-22 16:20:45.960754 catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/list/community.py
--rw-r--r--   0        0        0     2016 2024-05-22 16:20:45.960754 catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/list/data_ipv6_prefix.py
--rw-r--r--   0        0        0     1932 2024-05-22 16:20:45.960754 catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/list/data_prefix.py
--rw-r--r--   0        0        0     2079 2024-05-22 16:20:45.960754 catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/list/expanded_community.py
--rw-r--r--   0        0        0     1806 2024-05-22 16:20:45.960754 catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/list/fqdn.py
--rw-r--r--   0        0        0     1953 2024-05-22 16:20:45.960754 catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/list/geo_location.py
--rw-r--r--   0        0        0     1974 2024-05-22 16:20:45.960754 catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/list/ips_signature.py
--rw-r--r--   0        0        0     1932 2024-05-22 16:20:45.960754 catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/list/ipv6_prefix.py
--rw-r--r--   0        0        0     1890 2024-05-22 16:20:45.960754 catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/list/local_app.py
--rw-r--r--   0        0        0     1953 2024-05-22 16:20:45.960754 catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/list/local_domain.py
--rw-r--r--   0        0        0     1848 2024-05-22 16:20:45.960754 catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/list/mirror.py
--rw-r--r--   0        0        0     1874 2024-05-22 16:20:45.960754 catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/list/policer.py
--rw-r--r--   0        0        0     1806 2024-05-22 16:20:45.960754 catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/list/port.py
--rw-r--r--   0        0        0     2115 2024-05-22 16:20:45.960754 catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/list/preferred_color_group.py
--rw-r--r--   0        0        0     1848 2024-05-22 16:20:45.960754 catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/list/prefix.py
--rw-r--r--   0        0        0     1974 2024-05-22 16:20:45.960754 catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/list/protocol_name.py
--rw-r--r--   0        0        0     1781 2024-05-22 16:20:45.960754 catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/list/region.py
--rw-r--r--   0        0        0     1946 2024-05-22 16:20:45.960754 catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/list/site.py
--rw-r--r--   0        0        0     1845 2024-05-22 16:20:45.960754 catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/list/sla.py
--rw-r--r--   0        0        0     1806 2024-05-22 16:20:45.960754 catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/list/tloc.py
--rw-r--r--   0        0        0     1926 2024-05-22 16:20:45.960754 catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/list/url_allow_list.py
--rw-r--r--   0        0        0     1926 2024-05-22 16:20:45.960754 catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/list/url_block_list.py
--rw-r--r--   0        0        0     1787 2024-05-22 16:20:45.960754 catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/list/vpn.py
--rw-r--r--   0        0        0     1806 2024-05-22 16:20:45.960754 catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/list/zone.py
--rw-r--r--   0        0        0     1782 2024-05-22 16:20:45.960754 catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/security_template.py
--rw-r--r--   0        0        0     1738 2024-05-22 16:20:45.960754 catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/vedge_template.py
--rw-r--r--   0        0        0     2974 2024-05-22 16:20:45.960754 catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/vsmart_template.py
--rw-r--r--   0        0        0     8865 2024-05-22 16:20:45.960754 catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/software_actions.py
--rw-r--r--   0        0        0     6820 2024-05-22 16:20:45.960754 catalystwan-0.33.6.post0/catalystwan/endpoints/configuration_dashboard_status.py
--rw-r--r--   0        0        0    13587 2024-05-22 16:20:45.960754 catalystwan-0.33.6.post0/catalystwan/endpoints/configuration_device_actions.py
--rw-r--r--   0        0        0    13973 2024-05-22 16:20:45.960754 catalystwan-0.33.6.post0/catalystwan/endpoints/configuration_device_inventory.py
--rw-r--r--   0        0        0      881 2024-05-22 16:20:45.960754 catalystwan-0.33.6.post0/catalystwan/endpoints/configuration_device_template.py
--rw-r--r--   0        0        0     5277 2024-05-22 16:20:45.960754 catalystwan-0.33.6.post0/catalystwan/endpoints/configuration_feature_profile.py
--rw-r--r--   0        0        0     5158 2024-05-22 16:20:45.960754 catalystwan-0.33.6.post0/catalystwan/endpoints/configuration_group.py
--rw-r--r--   0        0        0    24950 2024-05-22 16:20:45.960754 catalystwan-0.33.6.post0/catalystwan/endpoints/configuration_settings.py
--rw-r--r--   0        0        0    14444 2024-05-22 16:20:45.960754 catalystwan-0.33.6.post0/catalystwan/endpoints/endpoints_container.py
--rw-r--r--   0        0        0      760 2024-05-22 16:20:45.960754 catalystwan-0.33.6.post0/catalystwan/endpoints/misc.py
--rw-r--r--   0        0        0     8272 2024-05-22 16:20:45.960754 catalystwan-0.33.6.post0/catalystwan/endpoints/monitoring/device_details.py
--rw-r--r--   0        0        0      400 2024-05-22 16:20:45.960754 catalystwan-0.33.6.post0/catalystwan/endpoints/monitoring/security_policy.py
--rw-r--r--   0        0        0      347 2024-05-22 16:20:45.960754 catalystwan-0.33.6.post0/catalystwan/endpoints/monitoring/server_info.py
--rw-r--r--   0        0        0     1929 2024-05-22 16:20:45.960754 catalystwan-0.33.6.post0/catalystwan/endpoints/monitoring/status.py
--rw-r--r--   0        0        0     1446 2024-05-22 16:20:45.960754 catalystwan-0.33.6.post0/catalystwan/endpoints/real_time_monitoring/reboot_history.py
--rw-r--r--   0        0        0     1419 2024-05-22 16:20:45.960754 catalystwan-0.33.6.post0/catalystwan/endpoints/sdavc_cloud_connector.py
--rw-r--r--   0        0        0     1047 2024-05-22 16:20:45.960754 catalystwan-0.33.6.post0/catalystwan/endpoints/tenant_backup_restore.py
--rw-r--r--   0        0        0     7648 2024-05-22 16:20:45.960754 catalystwan-0.33.6.post0/catalystwan/endpoints/tenant_management.py
--rw-r--r--   0        0        0     3582 2024-05-22 16:20:45.960754 catalystwan-0.33.6.post0/catalystwan/endpoints/tenant_migration.py
--rw-r--r--   0        0        0     3661 2024-05-22 16:20:45.960754 catalystwan-0.33.6.post0/catalystwan/endpoints/troubleshooting_tools/device_connectivity.py
--rw-r--r--   0        0        0      802 2024-05-22 16:20:45.960754 catalystwan-0.33.6.post0/catalystwan/endpoints/url_monitoring.py
--rw-r--r--   0        0        0     5735 2024-05-22 16:20:45.960754 catalystwan-0.33.6.post0/catalystwan/exceptions.py
--rw-r--r--   0        0        0     1902 2024-05-22 16:20:45.960754 catalystwan-0.33.6.post0/catalystwan/integration_tests/test_find_template_values.py
--rw-r--r--   0        0        0      676 2024-05-22 16:20:45.960754 catalystwan-0.33.6.post0/catalystwan/logging.conf
--rw-r--r--   0        0        0    14502 2024-05-22 16:20:45.960754 catalystwan-0.33.6.post0/catalystwan/models/common.py
--rw-r--r--   0        0        0      171 2024-05-22 16:20:45.960754 catalystwan-0.33.6.post0/catalystwan/models/configuration/common.py
--rw-r--r--   0        0        0     1090 2024-05-22 16:20:45.960754 catalystwan-0.33.6.post0/catalystwan/models/configuration/config_migration.py
--rw-r--r--   0        0        0    10043 2024-05-22 16:20:45.960754 catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/README.md
--rw-r--r--   0        0        0      663 2024-05-22 16:20:45.960754 catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/builder.py
--rw-r--r--   0        0        0     9117 2024-05-22 16:20:45.960754 catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/common.py
--rw-r--r--   0        0        0     1086 2024-05-22 16:20:45.960754 catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/management/vpn.py
--rw-r--r--   0        0        0     5553 2024-05-22 16:20:45.960754 catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/__init__.py
--rw-r--r--   0        0        0     1342 2024-05-22 16:20:45.960754 catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/app_probe.py
--rw-r--r--   0        0        0     1121 2024-05-22 16:20:45.960754 catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/application_list.py
--rw-r--r--   0        0        0      577 2024-05-22 16:20:45.960754 catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/color_list.py
--rw-r--r--   0        0        0     1033 2024-05-22 16:20:45.960754 catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/data_prefix.py
--rw-r--r--   0        0        0      885 2024-05-22 16:20:45.960754 catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/expanded_community_list.py
--rw-r--r--   0        0        0      731 2024-05-22 16:20:45.960754 catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/fowarding_class.py
--rw-r--r--   0        0        0     1034 2024-05-22 16:20:45.960754 catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/ipv6_data_prefix.py
--rw-r--r--   0        0        0     1034 2024-05-22 16:20:45.960754 catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/ipv6_prefix_list.py
--rw-r--r--   0        0        0     1268 2024-05-22 16:20:45.964754 catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/policier.py
--rw-r--r--   0        0        0     2867 2024-05-22 16:20:45.964754 catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/prefered_group_color.py
--rw-r--r--   0        0        0     1028 2024-05-22 16:20:45.964754 catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/prefix_list.py
--rw-r--r--   0        0        0     5197 2024-05-22 16:20:45.964754 catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/sla_class.py
--rw-r--r--   0        0        0      925 2024-05-22 16:20:45.964754 catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/standard_community.py
--rw-r--r--   0        0        0     1581 2024-05-22 16:20:45.964754 catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/tloc_list.py
--rw-r--r--   0        0        0     1177 2024-05-22 16:20:45.964754 catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/application_list.py
--rw-r--r--   0        0        0      759 2024-05-22 16:20:45.964754 catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/data_prefix.py
--rw-r--r--   0        0        0      738 2024-05-22 16:20:45.964754 catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/fqdn.py
--rw-r--r--   0        0        0     1182 2024-05-22 16:20:45.964754 catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/geolocation_list.py
--rw-r--r--   0        0        0     1496 2024-05-22 16:20:45.964754 catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/ips_signature.py
--rw-r--r--   0        0        0      801 2024-05-22 16:20:45.964754 catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/local_domain.py
--rw-r--r--   0        0        0      691 2024-05-22 16:20:45.964754 catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/protocol_list.py
--rw-r--r--   0        0        0     1131 2024-05-22 16:20:45.964754 catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/security_port.py
--rw-r--r--   0        0        0      883 2024-05-22 16:20:45.964754 catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/url.py
--rw-r--r--   0        0        0     1384 2024-05-22 16:20:45.964754 catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/zone.py
--rw-r--r--   0        0        0    14665 2024-05-22 16:20:45.964754 catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/service/acl.py
--rw-r--r--   0        0        0     8961 2024-05-22 16:20:45.964754 catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/service/appqoe.py
--rw-r--r--   0        0        0    14020 2024-05-22 16:20:45.964754 catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/service/bgp.py
--rw-r--r--   0        0        0     3448 2024-05-22 16:20:45.964754 catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/service/dhcp_server.py
--rw-r--r--   0        0        0     3835 2024-05-22 16:20:45.964754 catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/service/eigrp.py
--rw-r--r--   0        0        0     2777 2024-05-22 16:20:45.964754 catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/service/lan/common.py
--rw-r--r--   0        0        0    14424 2024-05-22 16:20:45.964754 catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/service/lan/ethernet.py
--rw-r--r--   0        0        0     9128 2024-05-22 16:20:45.964754 catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/service/lan/gre.py
--rw-r--r--   0        0        0     6575 2024-05-22 16:20:45.964754 catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/service/lan/ipsec.py
--rw-r--r--   0        0        0     7971 2024-05-22 16:20:45.964754 catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/service/lan/svi.py
--rw-r--r--   0        0        0    24489 2024-05-22 16:20:45.964754 catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/service/lan/vpn.py
--rw-r--r--   0        0        0    10081 2024-05-22 16:20:45.964754 catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/service/multicast.py
--rw-r--r--   0        0        0     3294 2024-05-22 16:20:45.964754 catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/service/object_tracker.py
--rw-r--r--   0        0        0     6725 2024-05-22 16:20:45.964754 catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/service/ospf.py
--rw-r--r--   0        0        0    11900 2024-05-22 16:20:45.964754 catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/service/ospfv3.py
--rw-r--r--   0        0        0     6391 2024-05-22 16:20:45.964754 catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/service/route_policy.py
--rw-r--r--   0        0        0     6993 2024-05-22 16:20:45.964754 catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/service/service_insertion_attachment.py
--rw-r--r--   0        0        0     5179 2024-05-22 16:20:45.964754 catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/service/switchport.py
--rw-r--r--   0        0        0     3790 2024-05-22 16:20:45.964754 catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/service/tracker.py
--rw-r--r--   0        0        0     5294 2024-05-22 16:20:45.964754 catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/service/wireless_lan.py
--rw-r--r--   0        0        0    13826 2024-05-22 16:20:45.964754 catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/system/aaa.py
--rw-r--r--   0        0        0     2179 2024-05-22 16:20:45.964754 catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/transport/cellular_controller.py
--rw-r--r--   0        0        0      167 2024-05-22 16:20:45.964754 catalystwan-0.33.6.post0/catalystwan/models/configuration/profile_type.py
--rw-r--r--   0        0        0     1041 2024-05-22 16:20:45.964754 catalystwan-0.33.6.post0/catalystwan/models/device_inventory.py
--rw-r--r--   0        0        0      341 2024-05-22 16:20:45.964754 catalystwan-0.33.6.post0/catalystwan/models/feature_profile_parcel.py
--rw-r--r--   0        0        0      785 2024-05-22 16:20:45.964754 catalystwan-0.33.6.post0/catalystwan/models/misc/application_protocols.py
--rw-r--r--   0        0        0      346 2024-05-22 16:20:45.964754 catalystwan-0.33.6.post0/catalystwan/models/monitoring/security_policy.py
--rw-r--r--   0        0        0      405 2024-05-22 16:20:45.964754 catalystwan-0.33.6.post0/catalystwan/models/monitoring/server_info.py
--rw-r--r--   0        0        0     4567 2024-05-22 16:20:45.964754 catalystwan-0.33.6.post0/catalystwan/models/policy/__init__.py
--rw-r--r--   0        0        0     9426 2024-05-22 16:20:45.964754 catalystwan-0.33.6.post0/catalystwan/models/policy/centralized.py
--rw-r--r--   0        0        0     5540 2024-05-22 16:20:45.964754 catalystwan-0.33.6.post0/catalystwan/models/policy/definitions/access_control_list.py
--rw-r--r--   0        0        0     5726 2024-05-22 16:20:45.964754 catalystwan-0.33.6.post0/catalystwan/models/policy/definitions/access_control_list_ipv6.py
--rw-r--r--   0        0        0    11851 2024-05-22 16:20:45.964754 catalystwan-0.33.6.post0/catalystwan/models/policy/definitions/control.py
--rw-r--r--   0        0        0     3861 2024-05-22 16:20:45.964754 catalystwan-0.33.6.post0/catalystwan/models/policy/definitions/device_access.py
--rw-r--r--   0        0        0     3961 2024-05-22 16:20:45.964754 catalystwan-0.33.6.post0/catalystwan/models/policy/definitions/device_access_ipv6.py
--rw-r--r--   0        0        0     3004 2024-05-22 16:20:45.964754 catalystwan-0.33.6.post0/catalystwan/models/policy/definitions/hub_and_spoke.py
--rw-r--r--   0        0        0     1184 2024-05-22 16:20:45.964754 catalystwan-0.33.6.post0/catalystwan/models/policy/definitions/mesh.py
--rw-r--r--   0        0        0     3454 2024-05-22 16:20:45.964754 catalystwan-0.33.6.post0/catalystwan/models/policy/definitions/qos_map.py
--rw-r--r--   0        0        0     1193 2024-05-22 16:20:45.964754 catalystwan-0.33.6.post0/catalystwan/models/policy/definitions/rewrite.py
--rw-r--r--   0        0        0    12252 2024-05-22 16:20:45.964754 catalystwan-0.33.6.post0/catalystwan/models/policy/definitions/rule_set.py
--rw-r--r--   0        0        0     2948 2024-05-22 16:20:45.964754 catalystwan-0.33.6.post0/catalystwan/models/policy/definitions/security_group.py
--rw-r--r--   0        0        0    13309 2024-05-22 16:20:45.964754 catalystwan-0.33.6.post0/catalystwan/models/policy/definitions/traffic_data.py
--rw-r--r--   0        0        0     1074 2024-05-22 16:20:45.964754 catalystwan-0.33.6.post0/catalystwan/models/policy/definitions/vpn_membership.py
--rw-r--r--   0        0        0     9345 2024-05-22 16:20:45.964754 catalystwan-0.33.6.post0/catalystwan/models/policy/definitions/zone_based_firewall.py
--rw-r--r--   0        0        0    10893 2024-05-22 16:20:45.964754 catalystwan-0.33.6.post0/catalystwan/models/policy/lists.py
--rw-r--r--   0        0        0    14613 2024-05-22 16:20:45.964754 catalystwan-0.33.6.post0/catalystwan/models/policy/lists_entries.py
--rw-r--r--   0        0        0     5558 2024-05-22 16:20:45.964754 catalystwan-0.33.6.post0/catalystwan/models/policy/localized.py
--rw-r--r--   0        0        0     3553 2024-05-22 16:20:45.964754 catalystwan-0.33.6.post0/catalystwan/models/policy/policy.py
--rw-r--r--   0        0        0    31904 2024-05-22 16:20:45.964754 catalystwan-0.33.6.post0/catalystwan/models/policy/policy_definition.py
--rw-r--r--   0        0        0     1274 2024-05-22 16:20:45.964754 catalystwan-0.33.6.post0/catalystwan/models/policy/policy_list.py
--rw-r--r--   0        0        0     7100 2024-05-22 16:20:45.964754 catalystwan-0.33.6.post0/catalystwan/models/policy/security.py
--rw-r--r--   0        0        0     5239 2024-05-22 16:20:45.964754 catalystwan-0.33.6.post0/catalystwan/models/tenant.py
--rw-r--r--   0        0        0      924 2024-05-22 16:20:45.964754 catalystwan-0.33.6.post0/catalystwan/models/url_monitoring.py
--rw-r--r--   0        0        0     9717 2024-05-22 16:20:45.964754 catalystwan-0.33.6.post0/catalystwan/response.py
--rw-r--r--   0        0        0    19904 2024-05-22 16:20:45.964754 catalystwan-0.33.6.post0/catalystwan/session.py
--rw-r--r--   0        0        0      116 2024-05-22 16:20:45.968754 catalystwan-0.33.6.post0/catalystwan/tests/templates/definitions/basic/alias.json
--rw-r--r--   0        0        0      114 2024-05-22 16:20:45.968754 catalystwan-0.33.6.post0/catalystwan/tests/templates/definitions/basic/basic.json
--rw-r--r--   0        0        0      109 2024-05-22 16:20:45.968754 catalystwan-0.33.6.post0/catalystwan/tests/templates/definitions/basic/basic_no_value.json
--rw-r--r--   0        0        0      848 2024-05-22 16:20:45.968754 catalystwan-0.33.6.post0/catalystwan/tests/templates/definitions/basic/children.json
--rw-r--r--   0        0        0     2348 2024-05-22 16:20:45.968754 catalystwan-0.33.6.post0/catalystwan/tests/templates/definitions/basic/children_nested.json
--rw-r--r--   0        0        0     2348 2024-05-22 16:20:45.968754 catalystwan-0.33.6.post0/catalystwan/tests/templates/definitions/basic/children_nested_datapath.json
--rw-r--r--   0        0        0      274 2024-05-22 16:20:45.968754 catalystwan-0.33.6.post0/catalystwan/tests/templates/definitions/basic/data_path.json
--rw-r--r--   0        0        0     6261 2024-05-22 16:20:45.968754 catalystwan-0.33.6.post0/catalystwan/tests/templates/definitions/cisco_aaa.json
--rw-r--r--   0        0        0    13658 2024-05-22 16:20:45.968754 catalystwan-0.33.6.post0/catalystwan/tests/templates/definitions/cisco_aaa_complex.json
--rw-r--r--   0        0        0      513 2024-05-22 16:20:45.968754 catalystwan-0.33.6.post0/catalystwan/tests/templates/definitions/cisco_banner.json
--rw-r--r--   0        0        0     2973 2024-05-22 16:20:45.968754 catalystwan-0.33.6.post0/catalystwan/tests/templates/definitions/cisco_bfd.json
--rw-r--r--   0        0        0    10040 2024-05-22 16:20:45.968754 catalystwan-0.33.6.post0/catalystwan/tests/templates/definitions/cisco_logging_complex.json
--rw-r--r--   0        0        0     4846 2024-05-22 16:20:45.968754 catalystwan-0.33.6.post0/catalystwan/tests/templates/definitions/cisco_ntp_complex.json
--rw-r--r--   0        0        0     5364 2024-05-22 16:20:45.968754 catalystwan-0.33.6.post0/catalystwan/tests/templates/definitions/cisco_omp_complex.json
--rw-r--r--   0        0        0    12410 2024-05-22 16:20:45.968754 catalystwan-0.33.6.post0/catalystwan/tests/templates/definitions/cisco_ospf_complex.json
--rw-r--r--   0        0        0    17001 2024-05-22 16:20:45.968754 catalystwan-0.33.6.post0/catalystwan/tests/templates/definitions/cisco_sig.json
--rw-r--r--   0        0        0     9266 2024-05-22 16:20:45.968754 catalystwan-0.33.6.post0/catalystwan/tests/templates/definitions/cisco_snmp_complex.json
--rw-r--r--   0        0        0    17119 2024-05-22 16:20:45.968754 catalystwan-0.33.6.post0/catalystwan/tests/templates/definitions/cisco_system_complex.json
--rw-r--r--   0        0        0      395 2024-05-22 16:20:45.968754 catalystwan-0.33.6.post0/catalystwan/tests/templates/definitions/cisco_vpn_basic.json
--rw-r--r--   0        0        0    41964 2024-05-22 16:20:45.968754 catalystwan-0.33.6.post0/catalystwan/tests/templates/definitions/cisco_vpn_complex.json
--rw-r--r--   0        0        0    27368 2024-05-22 16:20:45.968754 catalystwan-0.33.6.post0/catalystwan/tests/templates/definitions/cisco_vpn_interface_complex.json
--rw-r--r--   0        0        0     5219 2024-05-22 16:20:45.968754 catalystwan-0.33.6.post0/catalystwan/tests/templates/definitions/default_cisco_system.json
--rw-r--r--   0        0        0      712 2024-05-22 16:20:45.968754 catalystwan-0.33.6.post0/catalystwan/tests/templates/definitions/omp_vsmart_1.json
--rw-r--r--   0        0        0     1334 2024-05-22 16:20:45.968754 catalystwan-0.33.6.post0/catalystwan/tests/templates/definitions/omp_vsmart_2.json
--rw-r--r--   0        0        0     2141 2024-05-22 16:20:45.968754 catalystwan-0.33.6.post0/catalystwan/tests/templates/definitions/omp_vsmart_3.json
--rw-r--r--   0        0        0     2141 2024-05-22 16:20:45.968754 catalystwan-0.33.6.post0/catalystwan/tests/templates/definitions/omp_vsmart_complex.json
--rw-r--r--   0        0        0      651 2024-05-22 16:20:45.968754 catalystwan-0.33.6.post0/catalystwan/tests/templates/definitions/security_vsmart_complex.json
--rw-r--r--   0        0        0     3196 2024-05-22 16:20:45.968754 catalystwan-0.33.6.post0/catalystwan/tests/templates/definitions/system_vsmart_complex.json
--rw-r--r--   0        0        0     1829 2024-05-22 16:20:45.968754 catalystwan-0.33.6.post0/catalystwan/tests/templates/models/__init__.py
--rw-r--r--   0        0        0     4076 2024-05-22 16:20:45.968754 catalystwan-0.33.6.post0/catalystwan/tests/templates/models/cisco_aaa.py
--rw-r--r--   0        0        0      307 2024-05-22 16:20:45.968754 catalystwan-0.33.6.post0/catalystwan/tests/templates/models/cisco_banner.py
--rw-r--r--   0        0        0      538 2024-05-22 16:20:45.968754 catalystwan-0.33.6.post0/catalystwan/tests/templates/models/cisco_bfd.py
--rw-r--r--   0        0        0     1945 2024-05-22 16:20:45.968754 catalystwan-0.33.6.post0/catalystwan/tests/templates/models/cisco_logging.py
--rw-r--r--   0        0        0      713 2024-05-22 16:20:45.968754 catalystwan-0.33.6.post0/catalystwan/tests/templates/models/cisco_ntp.py
--rw-r--r--   0        0        0     1262 2024-05-22 16:20:45.968754 catalystwan-0.33.6.post0/catalystwan/tests/templates/models/cisco_omp.py
--rw-r--r--   0        0        0     1674 2024-05-22 16:20:45.968754 catalystwan-0.33.6.post0/catalystwan/tests/templates/models/cisco_ospf.py
--rw-r--r--   0        0        0     3078 2024-05-22 16:20:45.968754 catalystwan-0.33.6.post0/catalystwan/tests/templates/models/cisco_secure_internet_gateway.py
--rw-r--r--   0        0        0     1391 2024-05-22 16:20:45.968754 catalystwan-0.33.6.post0/catalystwan/tests/templates/models/cisco_snmp.py
--rw-r--r--   0        0        0     3270 2024-05-22 16:20:45.968754 catalystwan-0.33.6.post0/catalystwan/tests/templates/models/cisco_system.py
--rw-r--r--   0        0        0     6776 2024-05-22 16:20:45.968754 catalystwan-0.33.6.post0/catalystwan/tests/templates/models/cisco_vpn.py
--rw-r--r--   0        0        0     5740 2024-05-22 16:20:45.968754 catalystwan-0.33.6.post0/catalystwan/tests/templates/models/cisco_vpn_interface.py
--rw-r--r--   0        0        0     1515 2024-05-22 16:20:45.968754 catalystwan-0.33.6.post0/catalystwan/tests/templates/models/omp_vsmart.py
--rw-r--r--   0        0        0      372 2024-05-22 16:20:45.968754 catalystwan-0.33.6.post0/catalystwan/tests/templates/models/security_vsmart.py
--rw-r--r--   0        0        0     1170 2024-05-22 16:20:45.968754 catalystwan-0.33.6.post0/catalystwan/tests/templates/models/system_vsmart.py
--rw-r--r--   0        0        0      605 2024-05-22 16:20:45.968754 catalystwan-0.33.6.post0/catalystwan/tests/templates/schemas/basic/alias.json
--rw-r--r--   0        0        0      574 2024-05-22 16:20:45.968754 catalystwan-0.33.6.post0/catalystwan/tests/templates/schemas/basic/basic.json
--rw-r--r--   0        0        0     1810 2024-05-22 16:20:45.968754 catalystwan-0.33.6.post0/catalystwan/tests/templates/schemas/basic/children.json
--rw-r--r--   0        0        0     4005 2024-05-22 16:20:45.968754 catalystwan-0.33.6.post0/catalystwan/tests/templates/schemas/basic/children_nested.json
--rw-r--r--   0        0        0     4005 2024-05-22 16:20:45.968754 catalystwan-0.33.6.post0/catalystwan/tests/templates/schemas/basic/children_nested_datapath.json
--rw-r--r--   0        0        0      731 2024-05-22 16:20:45.968754 catalystwan-0.33.6.post0/catalystwan/tests/templates/schemas/basic/data_path.json
--rw-r--r--   0        0        0    43435 2024-05-22 16:20:45.968754 catalystwan-0.33.6.post0/catalystwan/tests/templates/schemas/cedge_aaa.json
--rw-r--r--   0        0        0     1200 2024-05-22 16:20:45.968754 catalystwan-0.33.6.post0/catalystwan/tests/templates/schemas/cisco_banner.json
--rw-r--r--   0        0        0     9495 2024-05-22 16:20:45.968754 catalystwan-0.33.6.post0/catalystwan/tests/templates/schemas/cisco_bfd.json
--rw-r--r--   0        0        0    20744 2024-05-22 16:20:45.968754 catalystwan-0.33.6.post0/catalystwan/tests/templates/schemas/cisco_logging.json
--rw-r--r--   0        0        0     8414 2024-05-22 16:20:45.968754 catalystwan-0.33.6.post0/catalystwan/tests/templates/schemas/cisco_ntp.json
--rw-r--r--   0        0        0    15153 2024-05-22 16:20:45.968754 catalystwan-0.33.6.post0/catalystwan/tests/templates/schemas/cisco_omp.json
--rw-r--r--   0        0        0    32647 2024-05-22 16:20:45.968754 catalystwan-0.33.6.post0/catalystwan/tests/templates/schemas/cisco_ospf.json
--rw-r--r--   0        0        0    56898 2024-05-22 16:20:45.968754 catalystwan-0.33.6.post0/catalystwan/tests/templates/schemas/cisco_secure_internet_gateway.json
--rw-r--r--   0        0        0    19387 2024-05-22 16:20:45.968754 catalystwan-0.33.6.post0/catalystwan/tests/templates/schemas/cisco_snmp.json
--rw-r--r--   0        0        0   106691 2024-05-22 16:20:45.968754 catalystwan-0.33.6.post0/catalystwan/tests/templates/schemas/cisco_system.json
--rw-r--r--   0        0        0    90121 2024-05-22 16:20:45.968754 catalystwan-0.33.6.post0/catalystwan/tests/templates/schemas/cisco_vpn.json
--rw-r--r--   0        0        0   104320 2024-05-22 16:20:45.972754 catalystwan-0.33.6.post0/catalystwan/tests/templates/schemas/cisco_vpn_interface.json
--rw-r--r--   0        0        0     6543 2024-05-22 16:20:45.972754 catalystwan-0.33.6.post0/catalystwan/tests/templates/schemas/omp-vsmart.json
--rw-r--r--   0        0        0     1546 2024-05-22 16:20:45.972754 catalystwan-0.33.6.post0/catalystwan/tests/templates/schemas/security-vsmart.json
--rw-r--r--   0        0        0    92208 2024-05-22 16:20:45.972754 catalystwan-0.33.6.post0/catalystwan/tests/templates/schemas/system-vsmart.json
--rw-r--r--   0        0        0     1066 2024-05-22 16:20:45.972754 catalystwan-0.33.6.post0/catalystwan/tests/templates/test_chose_model.py
--rw-r--r--   0        0        0     2598 2024-05-22 16:20:45.972754 catalystwan-0.33.6.post0/catalystwan/tests/templates/test_deserialize_model.py
--rw-r--r--   0        0        0     6762 2024-05-22 16:20:45.972754 catalystwan-0.33.6.post0/catalystwan/tests/templates/test_find_template_values.py
--rw-r--r--   0        0        0     4598 2024-05-22 16:20:45.972754 catalystwan-0.33.6.post0/catalystwan/tests/templates/test_generate_payload.py
--rw-r--r--   0        0        0     1756 2024-05-22 16:20:45.972754 catalystwan-0.33.6.post0/catalystwan/tests/templates/test_serialize_model.py
--rw-r--r--   0        0        0     8145 2024-05-22 16:20:45.972754 catalystwan-0.33.6.post0/catalystwan/tests/test_admin_tech_api.py
--rw-r--r--   0        0        0    17792 2024-05-22 16:20:45.972754 catalystwan-0.33.6.post0/catalystwan/tests/test_administration.py
--rw-r--r--   0        0        0    11116 2024-05-22 16:20:45.972754 catalystwan-0.33.6.post0/catalystwan/tests/test_alarms_api.py
--rw-r--r--   0        0        0     8229 2024-05-22 16:20:45.972754 catalystwan-0.33.6.post0/catalystwan/tests/test_cli_template.py
--rw-r--r--   0        0        0     5494 2024-05-22 16:20:45.972754 catalystwan-0.33.6.post0/catalystwan/tests/test_creation_tools.py
--rw-r--r--   0        0        0     3981 2024-05-22 16:20:45.972754 catalystwan-0.33.6.post0/catalystwan/tests/test_device_action_api.py
--rw-r--r--   0        0        0    28159 2024-05-22 16:20:45.972754 catalystwan-0.33.6.post0/catalystwan/tests/test_devices_api.py
--rw-r--r--   0        0        0    33583 2024-05-22 16:20:45.972754 catalystwan-0.33.6.post0/catalystwan/tests/test_endpoints.py
--rw-r--r--   0        0        0      894 2024-05-22 16:20:45.972754 catalystwan-0.33.6.post0/catalystwan/tests/test_feature_template_field.py
--rw-r--r--   0        0        0     1545 2024-05-22 16:20:45.972754 catalystwan-0.33.6.post0/catalystwan/tests/test_logs_api.py
--rw-r--r--   0        0        0     2896 2024-05-22 16:20:45.972754 catalystwan-0.33.6.post0/catalystwan/tests/test_monitoring_security_policy.py
--rw-r--r--   0        0        0     1809 2024-05-22 16:20:45.972754 catalystwan-0.33.6.post0/catalystwan/tests/test_monitoring_server_info.py
--rw-r--r--   0        0        0     5489 2024-05-22 16:20:45.972754 catalystwan-0.33.6.post0/catalystwan/tests/test_monitoring_status_api.py
--rw-r--r--   0        0        0    11026 2024-05-22 16:20:45.972754 catalystwan-0.33.6.post0/catalystwan/tests/test_mtt_aaa_api.py
--rw-r--r--   0        0        0    16472 2024-05-22 16:20:45.972754 catalystwan-0.33.6.post0/catalystwan/tests/test_omp_api.py
--rw-r--r--   0        0        0     5223 2024-05-22 16:20:45.972754 catalystwan-0.33.6.post0/catalystwan/tests/test_packet_capture.py
--rw-r--r--   0        0        0     5727 2024-05-22 16:20:45.972754 catalystwan-0.33.6.post0/catalystwan/tests/test_partition_manager_api.py
--rw-r--r--   0        0        0     7883 2024-05-22 16:20:45.972754 catalystwan-0.33.6.post0/catalystwan/tests/test_response.py
--rw-r--r--   0        0        0     6724 2024-05-22 16:20:45.972754 catalystwan-0.33.6.post0/catalystwan/tests/test_session.py
--rw-r--r--   0        0        0     7117 2024-05-22 16:20:45.972754 catalystwan-0.33.6.post0/catalystwan/tests/test_software_action_api.py
--rw-r--r--   0        0        0     6071 2024-05-22 16:20:45.972754 catalystwan-0.33.6.post0/catalystwan/tests/test_speed_test_api.py
--rw-r--r--   0        0        0    14926 2024-05-22 16:20:45.972754 catalystwan-0.33.6.post0/catalystwan/tests/test_task_status_api.py
--rw-r--r--   0        0        0    14965 2024-05-22 16:20:45.972754 catalystwan-0.33.6.post0/catalystwan/tests/test_templates.py
--rw-r--r--   0        0        0     3705 2024-05-22 16:20:45.972754 catalystwan-0.33.6.post0/catalystwan/tests/test_tenant_backup_restore_api.py
--rw-r--r--   0        0        0     6114 2024-05-22 16:20:45.972754 catalystwan-0.33.6.post0/catalystwan/tests/test_tenant_management_api.py
--rw-r--r--   0        0        0     4506 2024-05-22 16:20:45.972754 catalystwan-0.33.6.post0/catalystwan/tests/test_tenant_migration_api.py
--rw-r--r--   0        0        0    12377 2024-05-22 16:20:45.972754 catalystwan-0.33.6.post0/catalystwan/tests/test_typed_list.py
--rw-r--r--   0        0        0     3746 2024-05-22 16:20:45.972754 catalystwan-0.33.6.post0/catalystwan/tests/test_url_monitoring.py
--rw-r--r--   0        0        0     2968 2024-05-22 16:20:45.972754 catalystwan-0.33.6.post0/catalystwan/tests/test_version.py
--rw-r--r--   0        0        0    10377 2024-05-22 16:20:45.972754 catalystwan-0.33.6.post0/catalystwan/tests/test_version_utils.py
--rw-r--r--   0        0        0     3343 2024-05-22 16:20:45.972754 catalystwan-0.33.6.post0/catalystwan/tests/test_vmanage_auth.py
--rw-r--r--   0        0        0     9379 2024-05-22 16:20:45.972754 catalystwan-0.33.6.post0/catalystwan/typed_list.py
--rw-r--r--   0        0        0        0 2024-05-22 16:20:45.972754 catalystwan-0.33.6.post0/catalystwan/utils/__init__.py
--rw-r--r--   0        0        0      266 2024-05-22 16:20:45.972754 catalystwan-0.33.6.post0/catalystwan/utils/alarm_status.py
--rw-r--r--   0        0        0      253 2024-05-22 16:20:45.972754 catalystwan-0.33.6.post0/catalystwan/utils/certificate_status.py
--rw-r--r--   0        0        0      279 2024-05-22 16:20:45.972754 catalystwan-0.33.6.post0/catalystwan/utils/colors.py
--rw-r--r--   0        0        0      154 2024-05-22 16:20:45.972754 catalystwan-0.33.6.post0/catalystwan/utils/config_status.py
--rw-r--r--   0        0        0     4778 2024-05-22 16:20:45.972754 catalystwan-0.33.6.post0/catalystwan/utils/creation_tools.py
--rw-r--r--   0        0        0     7281 2024-05-22 16:20:45.972754 catalystwan-0.33.6.post0/catalystwan/utils/dashboard.py
--rw-r--r--   0        0        0     2110 2024-05-22 16:20:45.972754 catalystwan-0.33.6.post0/catalystwan/utils/dict.py
--rw-r--r--   0        0        0      953 2024-05-22 16:20:45.972754 catalystwan-0.33.6.post0/catalystwan/utils/feature_template/choose_model.py
--rw-r--r--   0        0        0     4882 2024-05-22 16:20:45.972754 catalystwan-0.33.6.post0/catalystwan/utils/feature_template/find_template_values.py
--rw-r--r--   0        0        0      584 2024-05-22 16:20:45.972754 catalystwan-0.33.6.post0/catalystwan/utils/operation_status.py
--rw-r--r--   0        0        0      196 2024-05-22 16:20:45.972754 catalystwan-0.33.6.post0/catalystwan/utils/personality.py
--rw-r--r--   0        0        0      360 2024-05-22 16:20:45.972754 catalystwan-0.33.6.post0/catalystwan/utils/pydantic_field.py
--rw-r--r--   0        0        0      172 2024-05-22 16:20:45.972754 catalystwan-0.33.6.post0/catalystwan/utils/reachability.py
--rw-r--r--   0        0        0      407 2024-05-22 16:20:45.972754 catalystwan-0.33.6.post0/catalystwan/utils/session_type.py
--rw-r--r--   0        0        0      149 2024-05-22 16:20:45.972754 catalystwan-0.33.6.post0/catalystwan/utils/template_type.py
--rw-r--r--   0        0        0     3930 2024-05-22 16:20:45.972754 catalystwan-0.33.6.post0/catalystwan/utils/upgrades_helper.py
--rw-r--r--   0        0        0      159 2024-05-22 16:20:45.972754 catalystwan-0.33.6.post0/catalystwan/utils/validate_status.py
--rw-r--r--   0        0        0     3032 2024-05-22 16:20:45.972754 catalystwan-0.33.6.post0/catalystwan/version.py
--rw-r--r--   0        0        0     5415 2024-05-22 16:20:45.972754 catalystwan-0.33.6.post0/catalystwan/vmanage_auth.py
--rw-r--r--   0        0        0     9946 2024-05-22 16:20:45.972754 catalystwan-0.33.6.post0/catalystwan/workflows/tenant_migration.py
--rw-r--r--   0        0        0      867 2024-05-22 16:20:45.976754 catalystwan-0.33.6.post0/pyproject.toml
--rw-r--r--   0        0        0    17811 1970-01-01 00:00:00.000000 catalystwan-0.33.6.post0/setup.py
--rw-r--r--   0        0        0    15306 1970-01-01 00:00:00.000000 catalystwan-0.33.6.post0/PKG-INFO
+-rw-r--r--   0        0        0    11375 2024-05-22 15:33:19.606312 catalystwan-0.33.7/LICENSE
+-rw-r--r--   0        0        0    13654 2024-05-22 15:33:19.606312 catalystwan-0.33.7/README.md
+-rw-r--r--   0        0        0     2524 2024-05-22 15:33:19.606312 catalystwan-0.33.7/catalystwan/__init__.py
+-rw-r--r--   0        0        0     1533 2024-05-22 15:33:19.606312 catalystwan-0.33.7/catalystwan/abstractions.py
+-rw-r--r--   0        0        0        0 2024-05-22 15:33:19.606312 catalystwan-0.33.7/catalystwan/api/__init__.py
+-rw-r--r--   0        0        0     6689 2024-05-22 15:33:19.606312 catalystwan-0.33.7/catalystwan/api/admin_tech_api.py
+-rw-r--r--   0        0        0    14935 2024-05-22 15:33:19.606312 catalystwan-0.33.7/catalystwan/api/administration.py
+-rw-r--r--   0        0        0     6314 2024-05-22 15:33:19.606312 catalystwan-0.33.7/catalystwan/api/alarms_api.py
+-rw-r--r--   0        0        0     3220 2024-05-22 15:33:19.606312 catalystwan-0.33.7/catalystwan/api/api_container.py
+-rw-r--r--   0        0        0    11636 2024-05-22 15:33:19.606312 catalystwan-0.33.7/catalystwan/api/basic_api.py
+-rw-r--r--   0        0        0     2053 2024-05-22 15:33:19.606312 catalystwan-0.33.7/catalystwan/api/config_device_inventory_api.py
+-rw-r--r--   0        0        0     4301 2024-05-22 15:33:19.606312 catalystwan-0.33.7/catalystwan/api/config_group_api.py
+-rw-r--r--   0        0        0     4645 2024-05-22 15:33:19.606312 catalystwan-0.33.7/catalystwan/api/configuration_groups/parcel.py
+-rw-r--r--   0        0        0     1290 2024-05-22 15:33:19.606312 catalystwan-0.33.7/catalystwan/api/configuration_groups/parcels/cellular_controller.py
+-rw-r--r--   0        0        0     7315 2024-05-22 15:33:19.606312 catalystwan-0.33.7/catalystwan/api/dashboard_api.py
+-rw-r--r--   0        0        0     7360 2024-05-22 15:33:19.606312 catalystwan-0.33.7/catalystwan/api/device_action_api.py
+-rw-r--r--   0        0        0    15767 2024-05-22 15:33:19.606312 catalystwan-0.33.7/catalystwan/api/feature_profile_api.py
+-rw-r--r--   0        0        0     1919 2024-05-22 15:33:19.606312 catalystwan-0.33.7/catalystwan/api/logs_api.py
+-rw-r--r--   0        0        0     2449 2024-05-22 15:33:19.606312 catalystwan-0.33.7/catalystwan/api/monitoring_status_api.py
+-rw-r--r--   0        0        0     6036 2024-05-22 15:33:19.606312 catalystwan-0.33.7/catalystwan/api/mtt_aaa_api.py
+-rw-r--r--   0        0        0     4394 2024-05-22 15:33:19.606312 catalystwan-0.33.7/catalystwan/api/omp_api.py
+-rw-r--r--   0        0        0     5691 2024-05-22 15:33:19.606312 catalystwan-0.33.7/catalystwan/api/packet_capture_api.py
+-rw-r--r--   0        0        0     1654 2024-05-22 15:33:19.606312 catalystwan-0.33.7/catalystwan/api/parcel_api.py
+-rw-r--r--   0        0        0     5600 2024-05-22 15:33:19.606312 catalystwan-0.33.7/catalystwan/api/partition_manager_api.py
+-rw-r--r--   0        0        0    28976 2024-05-22 15:33:19.606312 catalystwan-0.33.7/catalystwan/api/policy_api.py
+-rw-r--r--   0        0        0     2284 2024-05-22 15:33:19.606312 catalystwan-0.33.7/catalystwan/api/resource_pool_api.py
+-rw-r--r--   0        0        0    11320 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/software_action_api.py
+-rw-r--r--   0        0        0     5473 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/speedtest_api.py
+-rw-r--r--   0        0        0     7149 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/task_status_api.py
+-rw-r--r--   0        0        0    29260 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/template_api.py
+-rw-r--r--   0        0        0     3540 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/templates/README.md
+-rw-r--r--   0        0        0      251 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/templates/bool_str.py
+-rw-r--r--   0        0        0     7481 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/templates/cli_template.py
+-rw-r--r--   0        0        0     3107 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/templates/device_template/device_template.py
+-rw-r--r--   0        0        0      571 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/templates/device_template/device_template_payload.json.j2
+-rw-r--r--   0        0        0      137 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/templates/device_variable.py
+-rw-r--r--   0        0        0     5029 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/templates/feature_template.py
+-rw-r--r--   0        0        0     6576 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/templates/feature_template_field.py
+-rw-r--r--   0        0        0      661 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/templates/feature_template_payload.py
+-rw-r--r--   0        0        0     3244 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/templates/models/cisco_aaa_model.py
+-rw-r--r--   0        0        0      667 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/templates/models/cisco_banner_model.py
+-rw-r--r--   0        0        0     2180 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/templates/models/cisco_bfd_model.py
+-rw-r--r--   0        0        0    12522 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/templates/models/cisco_bgp_model.py
+-rw-r--r--   0        0        0     3436 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/templates/models/cisco_logging_model.py
+-rw-r--r--   0        0        0     1584 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/templates/models/cisco_ntp_model.py
+-rw-r--r--   0        0        0     3835 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/templates/models/cisco_omp_model.py
+-rw-r--r--   0        0        0     6749 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/templates/models/cisco_ospf.py
+-rw-r--r--   0        0        0    13901 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/templates/models/cisco_ospfv3.py
+-rw-r--r--   0        0        0     9589 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/templates/models/cisco_secure_internet_gateway.py
+-rw-r--r--   0        0        0     2581 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/templates/models/cisco_snmp_model.py
+-rw-r--r--   0        0        0     8986 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/templates/models/cisco_system.py
+-rw-r--r--   0        0        0    21665 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/templates/models/cisco_vpn_interface_model.py
+-rw-r--r--   0        0        0    15836 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/templates/models/cisco_vpn_model.py
+-rw-r--r--   0        0        0      472 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/templates/models/cli_template.py
+-rw-r--r--   0        0        0     1835 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/templates/models/omp_vsmart_model.py
+-rw-r--r--   0        0        0      806 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/templates/models/security_vsmart_model.py
+-rw-r--r--   0        0        0     1882 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/templates/models/supported.py
+-rw-r--r--   0        0        0     2624 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/templates/models/system_vsmart_model.py
+-rw-r--r--   0        0        0     2261 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/templates/payloads/aaa/aaa_model.py
+-rw-r--r--   0        0        0    11178 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/templates/payloads/aaa/feature/aaa.json.j2
+-rw-r--r--   0        0        0     1041 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/templates/payloads/aaa/feature/accounting.json.j2
+-rw-r--r--   0        0        0     4264 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/templates/payloads/aaa/feature/radius.json.j2
+-rw-r--r--   0        0        0     3735 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/templates/payloads/aaa/feature/tacacs.json.j2
+-rw-r--r--   0        0        0     1999 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/templates/payloads/aaa/feature/user.json.j2
+-rw-r--r--   0        0        0     2558 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/templates/payloads/cisco_vpn/cisco_vpn_model.py
+-rw-r--r--   0        0        0     4547 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/templates/payloads/cisco_vpn/feature/cisco_vpn.json.j2
+-rw-r--r--   0        0        0     1843 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/templates/payloads/cisco_vpn/feature/dns.json.j2
+-rw-r--r--   0        0        0     2247 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/templates/payloads/cisco_vpn/feature/ipv4route.json.j2
+-rw-r--r--   0        0        0     2098 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/templates/payloads/cisco_vpn/feature/ipv6route.json.j2
+-rw-r--r--   0        0        0      683 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/templates/payloads/cisco_vpn/feature/mapping.json.j2
+-rw-r--r--   0        0        0     7113 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/templates/payloads/tenant/tenant.json.j2
+-rw-r--r--   0        0        0     1460 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/templates/payloads/tenant/tenant_model.py
+-rw-r--r--   0        0        0     5013 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/tenant_backup_restore_api.py
+-rw-r--r--   0        0        0     4406 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/tenant_management_api.py
+-rw-r--r--   0        0        0     5090 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/tenant_migration_api.py
+-rw-r--r--   0        0        0    15887 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/versions_utils.py
+-rw-r--r--   0        0        0     7715 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/api/virtual_image_action_api.py
+-rw-r--r--   0        0        0    21802 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/dataclasses.py
+-rw-r--r--   0        0        0    25866 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/endpoints/__init__.py
+-rw-r--r--   0        0        0    11938 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/endpoints/administration_user_and_group.py
+-rw-r--r--   0        0        0     6731 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/endpoints/certificate_management_device.py
+-rw-r--r--   0        0        0     1476 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/endpoints/certificate_management_vmanage.py
+-rw-r--r--   0        0        0     4035 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/endpoints/client.py
+-rw-r--r--   0        0        0     2722 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/endpoints/cluster_management.py
+-rw-r--r--   0        0        0      983 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/endpoints/configuration/device/software_update.py
+-rw-r--r--   0        0        0     9447 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/endpoints/configuration/disaster_recovery.py
+-rw-r--r--   0        0        0     4037 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/endpoints/configuration/feature_profile/sdwan/policy_object.py
+-rw-r--r--   0        0        0     2064 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/endpoints/configuration/feature_profile/sdwan/system.py
+-rw-r--r--   0        0        0     4836 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/endpoints/configuration/feature_profile/sdwan/transport.py
+-rw-r--r--   0        0        0     2028 2024-05-22 15:33:19.610312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/definition/access_control_list.py
+-rw-r--r--   0        0        0     2091 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/definition/access_control_list_ipv6.py
+-rw-r--r--   0        0        0     2092 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/definition/control.py
+-rw-r--r--   0        0        0     2247 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/definition/device_access.py
+-rw-r--r--   0        0        0     2324 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/definition/device_access_ipv6.py
+-rw-r--r--   0        0        0     2174 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/definition/hub_and_spoke.py
+-rw-r--r--   0        0        0     2032 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/definition/mesh.py
+-rw-r--r--   0        0        0     2073 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/definition/qos_map.py
+-rw-r--r--   0        0        0     2132 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/definition/rewrite.py
+-rw-r--r--   0        0        0     2039 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/definition/rule_set.py
+-rw-r--r--   0        0        0     2159 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/definition/security_group.py
+-rw-r--r--   0        0        0     2104 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/definition/traffic_data.py
+-rw-r--r--   0        0        0     2263 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/definition/vpn_membership.py
+-rw-r--r--   0        0        0     2186 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/definition/zone_based_firewall.py
+-rw-r--r--   0        0        0     1793 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/app.py
+-rw-r--r--   0        0        0     1950 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/app_probe.py
+-rw-r--r--   0        0        0     1848 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/as_path.py
+-rw-r--r--   0        0        0     1870 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/class_map.py
+-rw-r--r--   0        0        0     1827 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/color.py
+-rw-r--r--   0        0        0     1911 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/community.py
+-rw-r--r--   0        0        0     2016 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/data_ipv6_prefix.py
+-rw-r--r--   0        0        0     1932 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/data_prefix.py
+-rw-r--r--   0        0        0     2079 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/expanded_community.py
+-rw-r--r--   0        0        0     1806 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/fqdn.py
+-rw-r--r--   0        0        0     1953 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/geo_location.py
+-rw-r--r--   0        0        0     1974 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/ips_signature.py
+-rw-r--r--   0        0        0     1932 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/ipv6_prefix.py
+-rw-r--r--   0        0        0     1890 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/local_app.py
+-rw-r--r--   0        0        0     1953 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/local_domain.py
+-rw-r--r--   0        0        0     1848 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/mirror.py
+-rw-r--r--   0        0        0     1874 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/policer.py
+-rw-r--r--   0        0        0     1806 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/port.py
+-rw-r--r--   0        0        0     2115 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/preferred_color_group.py
+-rw-r--r--   0        0        0     1848 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/prefix.py
+-rw-r--r--   0        0        0     1974 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/protocol_name.py
+-rw-r--r--   0        0        0     1781 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/region.py
+-rw-r--r--   0        0        0     1946 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/site.py
+-rw-r--r--   0        0        0     1845 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/sla.py
+-rw-r--r--   0        0        0     1806 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/tloc.py
+-rw-r--r--   0        0        0     1926 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/url_allow_list.py
+-rw-r--r--   0        0        0     1926 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/url_block_list.py
+-rw-r--r--   0        0        0     1787 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/vpn.py
+-rw-r--r--   0        0        0     1806 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/zone.py
+-rw-r--r--   0        0        0     1782 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/security_template.py
+-rw-r--r--   0        0        0     1738 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/vedge_template.py
+-rw-r--r--   0        0        0     2974 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/vsmart_template.py
+-rw-r--r--   0        0        0     8865 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration/software_actions.py
+-rw-r--r--   0        0        0     6820 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration_dashboard_status.py
+-rw-r--r--   0        0        0    13587 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration_device_actions.py
+-rw-r--r--   0        0        0    13973 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration_device_inventory.py
+-rw-r--r--   0        0        0      881 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration_device_template.py
+-rw-r--r--   0        0        0     5277 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration_feature_profile.py
+-rw-r--r--   0        0        0     5158 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration_group.py
+-rw-r--r--   0        0        0    24950 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/configuration_settings.py
+-rw-r--r--   0        0        0    14444 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/endpoints_container.py
+-rw-r--r--   0        0        0      760 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/misc.py
+-rw-r--r--   0        0        0     8272 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/monitoring/device_details.py
+-rw-r--r--   0        0        0      400 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/monitoring/security_policy.py
+-rw-r--r--   0        0        0      347 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/monitoring/server_info.py
+-rw-r--r--   0        0        0     1929 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/monitoring/status.py
+-rw-r--r--   0        0        0     1446 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/real_time_monitoring/reboot_history.py
+-rw-r--r--   0        0        0     1419 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/sdavc_cloud_connector.py
+-rw-r--r--   0        0        0     1047 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/tenant_backup_restore.py
+-rw-r--r--   0        0        0     7648 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/tenant_management.py
+-rw-r--r--   0        0        0     3582 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/tenant_migration.py
+-rw-r--r--   0        0        0     3661 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/troubleshooting_tools/device_connectivity.py
+-rw-r--r--   0        0        0      802 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/endpoints/url_monitoring.py
+-rw-r--r--   0        0        0     5735 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/exceptions.py
+-rw-r--r--   0        0        0     1902 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/integration_tests/test_find_template_values.py
+-rw-r--r--   0        0        0      676 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/logging.conf
+-rw-r--r--   0        0        0     3079 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/models/common.py
+-rw-r--r--   0        0        0      171 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/models/configuration/common.py
+-rw-r--r--   0        0        0     1090 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/models/configuration/config_migration.py
+-rw-r--r--   0        0        0    10043 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/README.md
+-rw-r--r--   0        0        0      663 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/builder.py
+-rw-r--r--   0        0        0     9117 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/common.py
+-rw-r--r--   0        0        0     1086 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/management/vpn.py
+-rw-r--r--   0        0        0     5553 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/__init__.py
+-rw-r--r--   0        0        0     1342 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/app_probe.py
+-rw-r--r--   0        0        0     1121 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/application_list.py
+-rw-r--r--   0        0        0      577 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/color_list.py
+-rw-r--r--   0        0        0     1033 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/data_prefix.py
+-rw-r--r--   0        0        0      885 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/expanded_community_list.py
+-rw-r--r--   0        0        0      731 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/fowarding_class.py
+-rw-r--r--   0        0        0     1034 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/ipv6_data_prefix.py
+-rw-r--r--   0        0        0     1034 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/ipv6_prefix_list.py
+-rw-r--r--   0        0        0     1268 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/policier.py
+-rw-r--r--   0        0        0     2867 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/prefered_group_color.py
+-rw-r--r--   0        0        0     1028 2024-05-22 15:33:19.614312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/prefix_list.py
+-rw-r--r--   0        0        0     5197 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/sla_class.py
+-rw-r--r--   0        0        0      925 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/standard_community.py
+-rw-r--r--   0        0        0     1581 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/tloc_list.py
+-rw-r--r--   0        0        0     1177 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/application_list.py
+-rw-r--r--   0        0        0      759 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/data_prefix.py
+-rw-r--r--   0        0        0      738 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/fqdn.py
+-rw-r--r--   0        0        0     1182 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/geolocation_list.py
+-rw-r--r--   0        0        0     1496 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/ips_signature.py
+-rw-r--r--   0        0        0      801 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/local_domain.py
+-rw-r--r--   0        0        0      691 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/protocol_list.py
+-rw-r--r--   0        0        0     1131 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/security_port.py
+-rw-r--r--   0        0        0      883 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/url.py
+-rw-r--r--   0        0        0     1384 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/zone.py
+-rw-r--r--   0        0        0    14665 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/service/acl.py
+-rw-r--r--   0        0        0     8961 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/service/appqoe.py
+-rw-r--r--   0        0        0    14020 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/service/bgp.py
+-rw-r--r--   0        0        0     3448 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/service/dhcp_server.py
+-rw-r--r--   0        0        0     3835 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/service/eigrp.py
+-rw-r--r--   0        0        0     2777 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/service/lan/common.py
+-rw-r--r--   0        0        0    14424 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/service/lan/ethernet.py
+-rw-r--r--   0        0        0     9128 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/service/lan/gre.py
+-rw-r--r--   0        0        0     6575 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/service/lan/ipsec.py
+-rw-r--r--   0        0        0     7971 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/service/lan/svi.py
+-rw-r--r--   0        0        0    24489 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/service/lan/vpn.py
+-rw-r--r--   0        0        0    10081 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/service/multicast.py
+-rw-r--r--   0        0        0     3294 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/service/object_tracker.py
+-rw-r--r--   0        0        0     6725 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/service/ospf.py
+-rw-r--r--   0        0        0    11900 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/service/ospfv3.py
+-rw-r--r--   0        0        0     6391 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/service/route_policy.py
+-rw-r--r--   0        0        0     6993 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/service/service_insertion_attachment.py
+-rw-r--r--   0        0        0     5179 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/service/switchport.py
+-rw-r--r--   0        0        0     3790 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/service/tracker.py
+-rw-r--r--   0        0        0     5294 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/service/wireless_lan.py
+-rw-r--r--   0        0        0    13826 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/system/aaa.py
+-rw-r--r--   0        0        0     2179 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/transport/cellular_controller.py
+-rw-r--r--   0        0        0      167 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/configuration/profile_type.py
+-rw-r--r--   0        0        0     1041 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/device_inventory.py
+-rw-r--r--   0        0        0      341 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/feature_profile_parcel.py
+-rw-r--r--   0        0        0      785 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/misc/application_protocols.py
+-rw-r--r--   0        0        0      346 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/monitoring/security_policy.py
+-rw-r--r--   0        0        0      405 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/monitoring/server_info.py
+-rw-r--r--   0        0        0     4567 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/policy/__init__.py
+-rw-r--r--   0        0        0     9426 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/policy/centralized.py
+-rw-r--r--   0        0        0     5540 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/policy/definitions/access_control_list.py
+-rw-r--r--   0        0        0     5726 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/policy/definitions/access_control_list_ipv6.py
+-rw-r--r--   0        0        0    11851 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/policy/definitions/control.py
+-rw-r--r--   0        0        0     3861 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/policy/definitions/device_access.py
+-rw-r--r--   0        0        0     3961 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/policy/definitions/device_access_ipv6.py
+-rw-r--r--   0        0        0     3004 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/policy/definitions/hub_and_spoke.py
+-rw-r--r--   0        0        0     1184 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/policy/definitions/mesh.py
+-rw-r--r--   0        0        0     3454 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/policy/definitions/qos_map.py
+-rw-r--r--   0        0        0     1193 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/policy/definitions/rewrite.py
+-rw-r--r--   0        0        0    12252 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/policy/definitions/rule_set.py
+-rw-r--r--   0        0        0     2948 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/policy/definitions/security_group.py
+-rw-r--r--   0        0        0    13309 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/policy/definitions/traffic_data.py
+-rw-r--r--   0        0        0     1074 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/policy/definitions/vpn_membership.py
+-rw-r--r--   0        0        0     9345 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/policy/definitions/zone_based_firewall.py
+-rw-r--r--   0        0        0    10893 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/policy/lists.py
+-rw-r--r--   0        0        0    14613 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/policy/lists_entries.py
+-rw-r--r--   0        0        0     5558 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/policy/localized.py
+-rw-r--r--   0        0        0     3553 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/policy/policy.py
+-rw-r--r--   0        0        0    31904 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/policy/policy_definition.py
+-rw-r--r--   0        0        0     1274 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/policy/policy_list.py
+-rw-r--r--   0        0        0     7100 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/policy/security.py
+-rw-r--r--   0        0        0     5239 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/tenant.py
+-rw-r--r--   0        0        0      924 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/models/url_monitoring.py
+-rw-r--r--   0        0        0     9717 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/response.py
+-rw-r--r--   0        0        0    19888 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/session.py
+-rw-r--r--   0        0        0      401 2024-05-22 15:33:19.618312 catalystwan-0.33.7/catalystwan/tests/templates/definitions/Basic_Cisco_VPN_Model.json
+-rw-r--r--   0        0        0      513 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/templates/definitions/banner_1.json
+-rw-r--r--   0        0        0      116 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/templates/definitions/basic/alias.json
+-rw-r--r--   0        0        0      114 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/templates/definitions/basic/basic.json
+-rw-r--r--   0        0        0      109 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/templates/definitions/basic/basic_no_value.json
+-rw-r--r--   0        0        0      848 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/templates/definitions/basic/children.json
+-rw-r--r--   0        0        0     2348 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/templates/definitions/basic/children_nested.json
+-rw-r--r--   0        0        0     2348 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/templates/definitions/basic/children_nested_datapath.json
+-rw-r--r--   0        0        0      274 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/templates/definitions/basic/data_path.json
+-rw-r--r--   0        0        0     2973 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/templates/definitions/cisco_bfd.json
+-rw-r--r--   0        0        0    11100 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/templates/definitions/complex_aaa.json
+-rw-r--r--   0        0        0    41165 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/templates/definitions/complex_cisco_vpn.json
+-rw-r--r--   0        0        0     5219 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/templates/definitions/default_cisco_system.json
+-rw-r--r--   0        0        0     5505 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/templates/definitions/iuo.json
+-rw-r--r--   0        0        0      249 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/templates/definitions/omp_1.json
+-rw-r--r--   0        0        0      875 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/templates/definitions/omp_2.json
+-rw-r--r--   0        0        0     1682 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/templates/definitions/omp_3.json
+-rw-r--r--   0        0        0      662 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/templates/models/__init__.py
+-rw-r--r--   0        0        0     2828 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/templates/models/cisco_aaa.py
+-rw-r--r--   0        0        0      303 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/templates/models/cisco_banner.py
+-rw-r--r--   0        0        0      587 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/templates/models/cisco_bfd.py
+-rw-r--r--   0        0        0      344 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/templates/models/cisco_system.py
+-rw-r--r--   0        0        0     8078 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/templates/models/cisco_vpn.py
+-rw-r--r--   0        0        0     1091 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/templates/models/omp_vsmart.py
+-rw-r--r--   0        0        0      605 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/templates/schemas/basic/alias.json
+-rw-r--r--   0        0        0      574 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/templates/schemas/basic/basic.json
+-rw-r--r--   0        0        0     1810 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/templates/schemas/basic/children.json
+-rw-r--r--   0        0        0     4005 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/templates/schemas/basic/children_nested.json
+-rw-r--r--   0        0        0     4005 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/templates/schemas/basic/children_nested_datapath.json
+-rw-r--r--   0        0        0      731 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/templates/schemas/basic/data_path.json
+-rw-r--r--   0        0        0    43436 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/templates/schemas/cedge_aaa.json
+-rw-r--r--   0        0        0     1200 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/templates/schemas/cisco_banner.json
+-rw-r--r--   0        0        0     9495 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/templates/schemas/cisco_bfd.json
+-rw-r--r--   0        0        0    99045 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/templates/schemas/cisco_system.json
+-rw-r--r--   0        0        0    87854 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/templates/schemas/cisco_vpn.json
+-rw-r--r--   0        0        0     5939 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/templates/schemas/omp-vsmart.json
+-rw-r--r--   0        0        0     1381 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/templates/test_chose_model.py
+-rw-r--r--   0        0        0     2598 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/templates/test_deserialize_model.py
+-rw-r--r--   0        0        0     6762 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/templates/test_find_template_values.py
+-rw-r--r--   0        0        0     4598 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/templates/test_generate_payload.py
+-rw-r--r--   0        0        0     1756 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/templates/test_serialize_model.py
+-rw-r--r--   0        0        0     8145 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/test_admin_tech_api.py
+-rw-r--r--   0        0        0    17792 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/test_administration.py
+-rw-r--r--   0        0        0    11116 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/test_alarms_api.py
+-rw-r--r--   0        0        0     8322 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/test_cli_template.py
+-rw-r--r--   0        0        0     5494 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/test_creation_tools.py
+-rw-r--r--   0        0        0     3981 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/test_device_action_api.py
+-rw-r--r--   0        0        0    28159 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/test_devices_api.py
+-rw-r--r--   0        0        0    33583 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/test_endpoints.py
+-rw-r--r--   0        0        0      894 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/test_feature_template_field.py
+-rw-r--r--   0        0        0     1545 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/test_logs_api.py
+-rw-r--r--   0        0        0     2896 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/test_monitoring_security_policy.py
+-rw-r--r--   0        0        0     1809 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/test_monitoring_server_info.py
+-rw-r--r--   0        0        0     5489 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/test_monitoring_status_api.py
+-rw-r--r--   0        0        0    11026 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/test_mtt_aaa_api.py
+-rw-r--r--   0        0        0    16472 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/test_omp_api.py
+-rw-r--r--   0        0        0     5223 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/test_packet_capture.py
+-rw-r--r--   0        0        0     5727 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/test_partition_manager_api.py
+-rw-r--r--   0        0        0     7883 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/test_response.py
+-rw-r--r--   0        0        0     6724 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/test_session.py
+-rw-r--r--   0        0        0     7117 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/test_software_action_api.py
+-rw-r--r--   0        0        0     6071 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/test_speed_test_api.py
+-rw-r--r--   0        0        0    14926 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/test_task_status_api.py
+-rw-r--r--   0        0        0    15050 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/test_templates.py
+-rw-r--r--   0        0        0     3705 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/test_tenant_backup_restore_api.py
+-rw-r--r--   0        0        0     6114 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/test_tenant_management_api.py
+-rw-r--r--   0        0        0     4506 2024-05-22 15:33:19.622312 catalystwan-0.33.7/catalystwan/tests/test_tenant_migration_api.py
+-rw-r--r--   0        0        0    12377 2024-05-22 15:33:19.626312 catalystwan-0.33.7/catalystwan/tests/test_typed_list.py
+-rw-r--r--   0        0        0     3746 2024-05-22 15:33:19.626312 catalystwan-0.33.7/catalystwan/tests/test_url_monitoring.py
+-rw-r--r--   0        0        0     2968 2024-05-22 15:33:19.626312 catalystwan-0.33.7/catalystwan/tests/test_version.py
+-rw-r--r--   0        0        0    10377 2024-05-22 15:33:19.626312 catalystwan-0.33.7/catalystwan/tests/test_version_utils.py
+-rw-r--r--   0        0        0     3343 2024-05-22 15:33:19.626312 catalystwan-0.33.7/catalystwan/tests/test_vmanage_auth.py
+-rw-r--r--   0        0        0     9379 2024-05-22 15:33:19.626312 catalystwan-0.33.7/catalystwan/typed_list.py
+-rw-r--r--   0        0        0        0 2024-05-22 15:33:19.626312 catalystwan-0.33.7/catalystwan/utils/__init__.py
+-rw-r--r--   0        0        0      266 2024-05-22 15:33:19.626312 catalystwan-0.33.7/catalystwan/utils/alarm_status.py
+-rw-r--r--   0        0        0      253 2024-05-22 15:33:19.626312 catalystwan-0.33.7/catalystwan/utils/certificate_status.py
+-rw-r--r--   0        0        0      279 2024-05-22 15:33:19.626312 catalystwan-0.33.7/catalystwan/utils/colors.py
+-rw-r--r--   0        0        0      154 2024-05-22 15:33:19.626312 catalystwan-0.33.7/catalystwan/utils/config_status.py
+-rw-r--r--   0        0        0     4778 2024-05-22 15:33:19.626312 catalystwan-0.33.7/catalystwan/utils/creation_tools.py
+-rw-r--r--   0        0        0     7281 2024-05-22 15:33:19.626312 catalystwan-0.33.7/catalystwan/utils/dashboard.py
+-rw-r--r--   0        0        0     2863 2024-05-22 15:33:19.626312 catalystwan-0.33.7/catalystwan/utils/device_model.py
+-rw-r--r--   0        0        0     2110 2024-05-22 15:33:19.626312 catalystwan-0.33.7/catalystwan/utils/dict.py
+-rw-r--r--   0        0        0      953 2024-05-22 15:33:19.626312 catalystwan-0.33.7/catalystwan/utils/feature_template/choose_model.py
+-rw-r--r--   0        0        0     4882 2024-05-22 15:33:19.626312 catalystwan-0.33.7/catalystwan/utils/feature_template/find_template_values.py
+-rw-r--r--   0        0        0      584 2024-05-22 15:33:19.626312 catalystwan-0.33.7/catalystwan/utils/operation_status.py
+-rw-r--r--   0        0        0      196 2024-05-22 15:33:19.626312 catalystwan-0.33.7/catalystwan/utils/personality.py
+-rw-r--r--   0        0        0      360 2024-05-22 15:33:19.626312 catalystwan-0.33.7/catalystwan/utils/pydantic_field.py
+-rw-r--r--   0        0        0      172 2024-05-22 15:33:19.626312 catalystwan-0.33.7/catalystwan/utils/reachability.py
+-rw-r--r--   0        0        0      407 2024-05-22 15:33:19.626312 catalystwan-0.33.7/catalystwan/utils/session_type.py
+-rw-r--r--   0        0        0      149 2024-05-22 15:33:19.626312 catalystwan-0.33.7/catalystwan/utils/template_type.py
+-rw-r--r--   0        0        0    17168 2024-05-22 15:33:19.626312 catalystwan-0.33.7/catalystwan/utils/timezone.py
+-rw-r--r--   0        0        0     3930 2024-05-22 15:33:19.626312 catalystwan-0.33.7/catalystwan/utils/upgrades_helper.py
+-rw-r--r--   0        0        0      159 2024-05-22 15:33:19.626312 catalystwan-0.33.7/catalystwan/utils/validate_status.py
+-rw-r--r--   0        0        0     3032 2024-05-22 15:33:19.626312 catalystwan-0.33.7/catalystwan/version.py
+-rw-r--r--   0        0        0     5415 2024-05-22 15:33:19.626312 catalystwan-0.33.7/catalystwan/vmanage_auth.py
+-rw-r--r--   0        0        0     9946 2024-05-22 15:33:19.626312 catalystwan-0.33.7/catalystwan/workflows/tenant_migration.py
+-rw-r--r--   0        0        0      862 2024-05-22 15:33:19.626312 catalystwan-0.33.7/pyproject.toml
+-rw-r--r--   0        0        0    17267 1970-01-01 00:00:00.000000 catalystwan-0.33.7/setup.py
+-rw-r--r--   0        0        0    14781 1970-01-01 00:00:00.000000 catalystwan-0.33.7/PKG-INFO
```

### Comparing `catalystwan-0.33.6.post0/LICENSE` & `catalystwan-0.33.7/LICENSE`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/README.md` & `catalystwan-0.33.7/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -387,33 +387,14 @@
 target_api.store_token(migration_id, token_path)
 # migrate network
 migrate_task = origin_api.migrate_network(token_path)
 migrate_task.wait_for_completed()
 ```
 </details>
 
-<details>
-    <summary> <b>Feature Templates</b> <i>(click to expand)</i></summary>
-
-```python
-from catalystwan.api.templates.models.omp_vsmart_model import OMPvSmart
-
-omp_vsmart = OMPvSmart(
-    name="my_first_template",
-    description="NA",
-    device_models=["vsmart"]
-    
-)
-
-session.api.templates.create(omp_vsmart)
-```
-
-More details about how to use and how to add new: [Feature Templates README.md](https://github.com/cisco-open/cisco-catalyst-wan-sdk/blob/main/catalystwan/api/templates/README.md)
-</details>
-
 ### Note:
 To remove `InsecureRequestWarning`, you can include in your scripts (warning is suppressed when `catalystwan_devel` environment variable is set):
 ```Python
 import urllib3
 urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 ```
```

#### html2text {}

```diff
@@ -150,21 +150,15 @@
 origin_api.export_tenant(tenant=tenant) remote_filename =
 export_task.wait_for_file() # download origin_api.download(export_path,
 remote_filename) # import import_task = target_api.import_tenant(export_path,
 tenant.migration_key) import_task.wait_for_completed() # get token migration_id
 = import_task.import_info.migration_token_query_params.migration_id
 target_api.store_token(migration_id, token_path) # migrate network migrate_task
 = origin_api.migrate_network(token_path) migrate_task.wait_for_completed() ```
-FFeeaattuurree TTeemmppllaatteess (click to expand) ```python from
-catalystwan.api.templates.models.omp_vsmart_model import OMPvSmart omp_vsmart =
-OMPvSmart( name="my_first_template", description="NA", device_models=["vsmart"]
-) session.api.templates.create(omp_vsmart) ``` More details about how to use
-and how to add new: [Feature Templates README.md](https://github.com/cisco-
-open/cisco-catalyst-wan-sdk/blob/main/catalystwan/api/templates/README.md) ###
-Note: To remove `InsecureRequestWarning`, you can include in your scripts
+### Note: To remove `InsecureRequestWarning`, you can include in your scripts
 (warning is suppressed when `catalystwan_devel` environment variable is set):
 ```Python import urllib3 urllib3.disable_warnings
 (urllib3.exceptions.InsecureRequestWarning) ``` ## Catching Exceptions
 ```python try: session.api.users.delete("bogus-user-name") except
 ManagerHTTPError as error: # Process an error. print
 (error.response.status_code) print(error.info.code) print(error.info.message)
 print(error.info.details) ``` ## [Supported API endpoints](https://github.com/
```

### Comparing `catalystwan-0.33.6.post0/catalystwan/__init__.py` & `catalystwan-0.33.7/catalystwan/__init__.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/abstractions.py` & `catalystwan-0.33.7/catalystwan/abstractions.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/api/admin_tech_api.py` & `catalystwan-0.33.7/catalystwan/api/admin_tech_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/api/administration.py` & `catalystwan-0.33.7/catalystwan/api/administration.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/api/alarms_api.py` & `catalystwan-0.33.7/catalystwan/api/alarms_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/api/api_container.py` & `catalystwan-0.33.7/catalystwan/api/api_container.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/api/basic_api.py` & `catalystwan-0.33.7/catalystwan/api/basic_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/api/config_device_inventory_api.py` & `catalystwan-0.33.7/catalystwan/api/config_device_inventory_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/api/config_group_api.py` & `catalystwan-0.33.7/catalystwan/api/config_group_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/api/configuration_groups/parcel.py` & `catalystwan-0.33.7/catalystwan/api/configuration_groups/parcel.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/api/configuration_groups/parcels/cellular_controller.py` & `catalystwan-0.33.7/catalystwan/api/configuration_groups/parcels/cellular_controller.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/api/dashboard_api.py` & `catalystwan-0.33.7/catalystwan/api/dashboard_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/api/device_action_api.py` & `catalystwan-0.33.7/catalystwan/api/device_action_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/api/feature_profile_api.py` & `catalystwan-0.33.7/catalystwan/api/feature_profile_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/api/logs_api.py` & `catalystwan-0.33.7/catalystwan/api/logs_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/api/monitoring_status_api.py` & `catalystwan-0.33.7/catalystwan/api/monitoring_status_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/api/mtt_aaa_api.py` & `catalystwan-0.33.7/catalystwan/api/mtt_aaa_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/api/omp_api.py` & `catalystwan-0.33.7/catalystwan/api/omp_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/api/packet_capture_api.py` & `catalystwan-0.33.7/catalystwan/api/packet_capture_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/api/parcel_api.py` & `catalystwan-0.33.7/catalystwan/api/parcel_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/api/partition_manager_api.py` & `catalystwan-0.33.7/catalystwan/api/partition_manager_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/api/policy_api.py` & `catalystwan-0.33.7/catalystwan/api/policy_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/api/resource_pool_api.py` & `catalystwan-0.33.7/catalystwan/api/resource_pool_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/api/software_action_api.py` & `catalystwan-0.33.7/catalystwan/api/software_action_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/api/speedtest_api.py` & `catalystwan-0.33.7/catalystwan/api/speedtest_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/api/task_status_api.py` & `catalystwan-0.33.7/catalystwan/api/task_status_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/api/template_api.py` & `catalystwan-0.33.7/catalystwan/api/template_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 import json
 import logging
 from enum import Enum
 from typing import TYPE_CHECKING, Any, Optional, Type, overload
 
 from ciscoconfparse import CiscoConfParse  # type: ignore
-from typing_extensions import deprecated
 
 from catalystwan.api.task_status_api import Task
 from catalystwan.api.templates.cli_template import CLITemplate
 from catalystwan.api.templates.device_template.device_template import (
     DeviceSpecificValue,
     DeviceTemplate,
     GeneralTemplate,
@@ -36,18 +35,18 @@
 from catalystwan.api.templates.models.cisco_vpn_model import CiscoVPNModel
 from catalystwan.api.templates.models.cli_template import CliTemplateModel
 from catalystwan.api.templates.models.omp_vsmart_model import OMPvSmart
 from catalystwan.api.templates.models.security_vsmart_model import SecurityvSmart
 from catalystwan.api.templates.models.system_vsmart_model import SystemVsmart
 from catalystwan.dataclasses import Device, DeviceTemplateInfo, FeatureTemplateInfo, FeatureTemplatesTypes, TemplateInfo
 from catalystwan.endpoints.configuration_device_template import FeatureToCLIPayload
-from catalystwan.exceptions import AttachedError, CatalystwanDeprecationWarning, TemplateNotFoundError
-from catalystwan.models.common import DeviceModel
+from catalystwan.exceptions import AttachedError, TemplateNotFoundError
 from catalystwan.response import ManagerResponse
 from catalystwan.typed_list import DataSequence
+from catalystwan.utils.device_model import DeviceModel
 from catalystwan.utils.dict import merge
 from catalystwan.utils.pydantic_field import get_extra_field
 from catalystwan.utils.template_type import TemplateType
 
 if TYPE_CHECKING:
     from catalystwan.session import ManagerSession
 
@@ -434,17 +433,14 @@
 
         if not template_id:
             raise NotImplementedError()
 
         logger.info(f"Template {template.template_name} ({template_type}) was created successfully ({template_id}).")
         return template_id
 
-    @deprecated(
-        "Obsolete way to use Feature Templates - only Feature Templates", category=CatalystwanDeprecationWarning
-    )
     def _create_feature_template(self, template: FeatureTemplate) -> str:
         payload = template.generate_payload(self.session)
         response = self.session.post("/dataservice/template/feature", json=json.loads(payload))
         template_id = response.json()["templateId"]
 
         return template_id
 
@@ -556,25 +552,24 @@
     def generate_feature_template_payload(
         self, template: FeatureTemplate, schema: Any, debug: bool = False
     ) -> FeatureTemplatePayload:
         payload = FeatureTemplatePayload(
             name=template.template_name,
             description=template.template_description,
             template_type=template.type,
-            device_types=[device_model for device_model in template.device_models],
+            device_types=[device_model.value for device_model in template.device_models],
             definition={},
         )  # type: ignore
 
         fr_template_fields = [FeatureTemplateField(**field) for field in schema["fields"]]  # TODO
         json_dumped_template = template.model_dump(mode="json")
         # "name"
         for field in fr_template_fields:
             value = None
             priority_order = None
-            json_dumped_value = None
             # TODO How to discover Device specific variable
             if field.key in template.device_specific_variables:
                 value = template.device_specific_variables[field.key]
             else:
                 for field_name, field_value in template.model_fields.items():
                     data_path = get_extra_field(field_value, "data_path", default=[])
                     vmanage_key = get_extra_field(field_value, "vmanage_key")
@@ -604,15 +599,15 @@
         """Verify if selected template can be used with provided device model"""
 
         template_type = self._get_feature_template_types().filter(name=template.type).single_or_default()
 
         available_devices_for_template = [device["name"] for device in template_type.device_models]
 
         provided_device_models = [
-            dev_mod if type(dev_mod) is DeviceModel else dev_mod for dev_mod in template.device_models
+            dev_mod.value if type(dev_mod) is DeviceModel else dev_mod for dev_mod in template.device_models
         ]
 
         if not all(dev in available_devices_for_template for dev in provided_device_models):
             logger.debug(f"Available devices for template '{template.type}': {available_devices_for_template}")
             raise DeviceModelError(template, provided_device_models)
         return True
```

### Comparing `catalystwan-0.33.6.post0/catalystwan/api/templates/README.md` & `catalystwan-0.33.7/catalystwan/api/templates/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,101 +1,87 @@
 # How to use
 
 ## Feature Template Creation
 
 ```python
-from catalystwan.api.templates.models.omp_vsmart_model import OMPvSmart
-
 omp_vsmart = OMPvSmart(
     name="my_first_template",
     description="NA",
-    device_models=["vsmart"]
+    device_models=[DeviceModel.VSMART]
     
 )
 
 session.api.templates.create(omp_vsmart)
 ```
 
 ## Add new Feature Template in Cisco Catalyst WAN SDK
+These steps will help you to automate feature template creation. We'll explain what to do and why, so everyone will have deep understanding how our templates work. In the example we will try to create `OMP` Feature Template for vSmart. 
 
-These steps will help you to automate feature template creation. We'll explain what to do and why, so everyone will have deep understanding how our templates work. In the example we will try to create `OMP` Feature Template for vSmart.
-
-1. Get your template type name and version.
+1. Get your template type name and version. 
     >Note: display name is not template type name!
-
 - For example, you could extract it from response body. Go to your Manager and create any template which you would like to automate in catalystwan. Send template creation request and check for `templateType` and `templateMinVersion` variable names. `OMP` (display name) for vSmart has `omp-vsmart` template type name.
 
 2. With corresponding `templateType` we are able to create new class which implements `FeatureTemplate` interface. Create new file in `catalystwan\api\templates\models\` and copy-paste the code and change name of the class with its type attribute.
 
-```python
-from pathlib import Path
-from typing import ClassVar
-from pydantic import ConfigDict
-from catalystwan.api.templates.feature_template import FeatureTemplate
-
-
-class OMPvSmart(FeatureTemplate):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+	```python
+	from pathlib import Path
+	from typing import ClassVar
+	from pydantic import ConfigDict
+	from catalystwan.api.templates.feature_template import FeatureTemplate
 
-    payload_path: ClassVar[Path] = Path(__file__).parent / "DEPRECATED"
-    type: ClassVar[str] = "omp-vsmart"
-```
 
+	class OMPvSmart(FeatureTemplate):
+		model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+			
+		payload_path: ClassVar[Path] = Path(__file__).parent / "DEPRECATED"
+		type: ClassVar[str] = "omp-vsmart"
+	```
 3. (This step is temporary) Find `is_created_by_generator` method in `template_api` and add your new template class.
 
-```python
-ported_templates = (..., OMPvSmart)
-```
-
-NOTE: This step will be removed once all template payloads will be generated automatically.
-
+	```python
+	ported_templates = (..., OMPvSmart)
+	```
+	NOTE: This step will be removed once all template payloads will be generated automatically.
 4. (This step is temporary) Find `available_models` definition in 'supported' and add your new template class.
-
-```python
-available_models = {
-    (...)
-    'omp_vsmart': OMPvSmart
-}
-```
-
-NOTE: This step will be removed once all template payloads will be generated dynamically.
-
+	```python
+	available_models = {
+		(...)
+		'omp_vsmart': OMPvSmart
+	}
+	```
+	NOTE: This step will be removed once all template payloads will be generated dynamically.
 5. We can try to create our first template with default values.
+   ```python
+	omp_vsmart = OMPvSmart(
+		name="my_first_template",
+		description="NA",
+		device_models=[DeviceModel.VSMART]
+	)
+
+	session.api.templates.create(omp_vsmart)
+	```
+	If everything went successfuly, we will get similar message 
 
-```python
-omp_vsmart = OMPvSmart(
-    name="my_first_template",
-    description="NA",
-    device_models=["vsmart"]
-)
-
-session.api.templates.create(omp_vsmart)
-```
-
-If everything went successfuly, we will get similar message:
-
-`Template my_first_template (FeatureTemplate) was created successfully (7e56acdd-640e-45dc-9335-87abc697995f).`
+	`Template my_first_template (FeatureTemplate) was created successfully (7e56acdd-640e-45dc-9335-87abc697995f).`
 
 6. We can check whether our template is created sucessfully in Manager manually. If there is an error, please create an issue with error and try go to the 7th step.
-
-### Customize Feature Template fields
-
+   
+### Customize Feature Template fields.
 7. Run below code with already created session and changed corresponding variables.
 
-```python
-# TODO: Use 2nd layer.
-import json
+    ```python
+    # TODO: Use 2nd layer.
+    import json
 
 
-template_type = "omp-vsmart" # Change this value
-template_version = "15.0.0" # Change this value
-endpoint = f"/dataservice/template/feature/types/definition/{template_type}/{template_version}"
+    template_type = "omp-vsmart" # Change this value
+    template_version = "15.0.0" # Change this value
+    endpoint = f"/dataservice/template/feature/types/definition/{template_type}/{template_version}"
 
-schema = session.get(url=endpoint).json()
+    schema = session.get(url=endpoint).json()
 
-with open(f"response_{template_type}.json", "w") as f:
-    f.write(json.dumps(schema, indent=4))
-```
+    with open(f"response_{template_type}.json", "w") as f:
+        f.write(json.dumps(schema, indent=4))
+    ```
 
 8. Open `response_{template_type}.json` file.
-
 9. Find `fields` key. The value should be list of dictionaries. Get every possible key in the dictionary and fill our class with every possible key. You can find the code in `catalystwan\api\templates\models\omp_vsmart_model.py` file.
```

### Comparing `catalystwan-0.33.6.post0/catalystwan/api/templates/cli_template.py` & `catalystwan-0.33.7/catalystwan/api/templates/cli_template.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from attr import define  # type: ignore
 from ciscoconfparse import CiscoConfParse  # type: ignore
 from requests.exceptions import HTTPError
 
 from catalystwan.dataclasses import Device
 from catalystwan.exceptions import TemplateTypeError
-from catalystwan.models.common import DeviceModel
+from catalystwan.utils.device_model import DeviceModel
 from catalystwan.utils.template_type import TemplateType
 
 logger = logging.getLogger(__name__)
 
 if TYPE_CHECKING:
     from catalystwan.session import ManagerSession
 
@@ -63,24 +63,24 @@
         return self.config
 
     def generate_payload(self) -> dict:
         config_str = "\n".join(self.config.ioscfg)
         payload = {
             "templateName": self.template_name,
             "templateDescription": self.template_description,
-            "deviceType": self.device_model,
+            "deviceType": self.device_model.value,
             "templateConfiguration": config_str,
             "factoryDefault": False,
             "configType": "file",
         }
         if self.device_model not in [
-            "vedge",
-            "vsmart",
-            "vmanage",
-            "vedge-cloud",
+            DeviceModel.VEDGE,
+            DeviceModel.VSMART,
+            DeviceModel.VMANAGE,
+            DeviceModel.VBOND,
         ]:
             payload["cliType"] = "device"
             payload["draftMode"] = False
         return payload
 
     def update(self, session: ManagerSession, id: str, config: CiscoConfParse) -> bool:
         """Update an existing cli template.
@@ -96,15 +96,15 @@
         """
         self.config = config
         config_str = "\n".join(self.config.ioscfg)
         payload = {
             "templateId": id,
             "templateName": self.template_name,
             "templateDescription": self.template_description,
-            "deviceType": self.device_model,
+            "deviceType": self.device_model.value,
             "templateConfiguration": config_str,
             "factoryDefault": False,
             "configType": "file",
             "draftMode": False,
         }
         endpoint = f"/dataservice/template/device/{id}"
         try:
```

### Comparing `catalystwan-0.33.6.post0/catalystwan/api/templates/device_template/device_template.py` & `catalystwan-0.33.7/catalystwan/api/templates/device_template/device_template.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import logging
 from pathlib import Path
 from typing import TYPE_CHECKING, Final, List
 
 from jinja2 import DebugUndefined, Environment, FileSystemLoader, meta  # type: ignore
 from pydantic import BaseModel, ConfigDict, Field, field_validator
 
-from catalystwan.models.common import DeviceModel
+from catalystwan.utils.device_model import DeviceModel
 
 if TYPE_CHECKING:
     from catalystwan.session import ManagerSession
 
 logger = logging.getLogger(__name__)
```

### Comparing `catalystwan-0.33.6.post0/catalystwan/api/templates/device_template/device_template_payload.json.j2` & `catalystwan-0.33.7/catalystwan/api/templates/device_template/device_template_payload.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/api/templates/feature_template.py` & `catalystwan-0.33.7/catalystwan/api/templates/feature_template.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Dict, List, Union, cast
 
 from jinja2 import DebugUndefined, Environment, FileSystemLoader, meta  # type: ignore
 from pydantic import BaseModel, model_validator
 
 from catalystwan.api.templates.device_variable import DeviceVariable
-from catalystwan.models.common import DeviceModel
+from catalystwan.utils.device_model import DeviceModel
 from catalystwan.utils.dict import FlattenedDictValue, flatten_dict
 from catalystwan.utils.feature_template.find_template_values import find_template_values
 from catalystwan.utils.pydantic_field import get_extra_field
 
 if TYPE_CHECKING:
     from catalystwan.session import ManagerSession
 
@@ -124,10 +124,10 @@
 
         values_from_template_definition = find_template_values(template_definition_as_dict)
         flattened_values = flatten_dict(values_from_template_definition)
 
         return feature_template_model(
             template_name=template_info.name,
             template_description=template_info.description,
-            device_models=[model for model in template_info.device_type],
+            device_models=[DeviceModel(model) for model in template_info.device_type],
             **flattened_values,
         )
```

### Comparing `catalystwan-0.33.6.post0/catalystwan/api/templates/feature_template_field.py` & `catalystwan-0.33.7/catalystwan/api/templates/feature_template_field.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/api/templates/feature_template_payload.py` & `catalystwan-0.33.7/catalystwan/api/templates/feature_template_payload.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/api/templates/models/cisco_aaa_model.py` & `catalystwan-0.33.7/catalystwan/api/templates/models/cisco_bgp_model.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,332 +1,259 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
+from enum import Enum
 from pathlib import Path
-from typing import ClassVar, List, Literal, Optional
+from typing import ClassVar, List, Optional
 
 from pydantic import ConfigDict, Field
 
 from catalystwan.api.templates.bool_str import BoolStr
 from catalystwan.api.templates.feature_template import FeatureTemplate, FeatureTemplateValidator
 
-Privilage = Literal["1", "15"]
 
-AccountingMethod = Literal["commands", "exec", "network", "system"]
+class Export(FeatureTemplateValidator):
+    asn_ip: str = Field(json_schema_extra={"vmanage_key": "asn-ip"})
+    model_config = ConfigDict(populate_by_name=True)
+
 
-AuthorizationMethod = Literal["commands"]
+class Import(FeatureTemplateValidator):
+    asn_ip: str = Field(json_schema_extra={"vmanage_key": "asn-ip"})
+    model_config = ConfigDict(populate_by_name=True)
 
-DomainStripping = Literal["yes", "no", "right-to-left"]
 
-AuthenticationType = Literal["any", "all", "session-key"]
+class RouteTargetIpv4(FeatureTemplateValidator):
+    vpn_id: int = Field(json_schema_extra={"vmanage_key": "vpn-id"})
+    export: List[Export]
+    import_: List[Import] = Field(json_schema_extra={"vmanage_key": "import"})
+    model_config = ConfigDict(populate_by_name=True)
 
 
-class PubkeyChain(FeatureTemplateValidator):
-    key_string: str = Field(
-        description="Set the RSA key string",
-        json_schema_extra={"vmanage_key": "key-string"},
-    )
-    key_type: Optional[str] = Field(
-        default="ssh-rsa",
-        description="Only RSA is supported",
-        json_schema_extra={"vmanage_key": "key-type"},
-    )
+class RouteTargetIpv6(FeatureTemplateValidator):
+    vpn_id: int = Field(json_schema_extra={"vmanage_key": "vpn-id"})
+    export: List[Export]
+    import_: List[Import] = Field(json_schema_extra={"vmanage_key": "import"})
+    model_config = ConfigDict(populate_by_name=True)
 
 
-class User(FeatureTemplateValidator):
-    name: str = Field(description="The name of the user")
-    password: Optional[str] = Field(default=None, description="The password for the user")
-    secret: Optional[str] = Field(default=None, description="The secret for the user")
-    privilege: Optional[Privilage] = Field(default="15", description="The privilege level for the user")
-    pubkey_chain: Optional[List[PubkeyChain]] = Field(
-        default=None,
-        description="List of public keys for the user",
-        json_schema_extra={"vmanage_key": "pubkey-chain"},
-    )
+class MplsInterface(FeatureTemplateValidator):
+    if_name: Optional[str] = Field(default=None, json_schema_extra={"vmanage_key": "if-name"})
+    model_config = ConfigDict(populate_by_name=True)
 
 
-class AccountingRule(FeatureTemplateValidator):
+class AddressFamilyType(str, Enum):
+    IPV4_UNICAST = "ipv4-unicast"
+
+
+class AggregateAddress(FeatureTemplateValidator):
+    prefix: str
+    as_set: Optional[BoolStr] = Field(default=None, json_schema_extra={"vmanage_key": "as-set"})
+    summary_only: Optional[BoolStr] = Field(default=None, json_schema_extra={"vmanage_key": "summary-only"})
     model_config = ConfigDict(populate_by_name=True)
 
-    rule_id: str = Field(
-        description="Accounting Rule ID",
-        json_schema_extra={"vmanage_key": "rule-id"},
-    )
-    method: AccountingMethod = Field(
-        description="Configure Accounting Method",
-        json_schema_extra={"vmanage_key": "method"},
-    )
-    level: Optional[Privilage] = Field(
-        default=None,
-        description="Privilege level when method is commands",
-        json_schema_extra={"vmanage_key": "level"},
-    )
-    start_stop: Optional[BoolStr] = Field(
-        default=True,
-        description="Enable Start-Stop",
-        json_schema_extra={"vmanage_key": "start-stop"},
-    )
-    group: str = Field(
-        description="List of groups.",
-        json_schema_extra={"vmanage_key": "group"},
-    )
+
+class Ipv6AggregateAddress(FeatureTemplateValidator):
+    prefix: str
+    as_set: Optional[bool] = Field(False, json_schema_extra={"vmanage_key": "as-set"})
+    summary_only: Optional[bool] = Field(False, json_schema_extra={"vmanage_key": "summary-only"})
+    model_config = ConfigDict(populate_by_name=True)
+
+
+class Network(FeatureTemplateValidator):
+    prefix: str
+
+
+class Ipv6Network(FeatureTemplateValidator):
+    prefix: str
+
+
+class Protocol(str, Enum):
+    STATIC = "static"
+    CONNECTED = "connected"
+    OSPF = "ospf"
+    OSPFV3 = "ospfv3"
+    OMP = "omp"
+    EIGRP = "eigrp"
+    NAT = "nat"
 
 
-class AuthorizationRules(FeatureTemplateValidator):
+class Redistribute(FeatureTemplateValidator):
+    protocol: Protocol
+    route_policy: Optional[str] = Field(default=None, json_schema_extra={"vmanage_key": "route-policy"})
     model_config = ConfigDict(populate_by_name=True)
 
-    rule_id: str = Field(
-        description="Authorization Rule ID",
-        json_schema_extra={"vmanage_key": "rule-id"},
-    )
-    method: AuthorizationMethod = Field(
-        description="Configure Authorization Method",
-        json_schema_extra={"vmanage_key": "method"},
-    )
-    level: Optional[Privilage] = Field(
-        default=None,
-        description="Privilege level when method is commands",
-        json_schema_extra={"vmanage_key": "level"},
-    )
-    group: str = Field(
-        description="List of groups.",
-        json_schema_extra={"vmanage_key": "group"},
-    )
-    authenticated: Optional[BoolStr] = Field(
-        default=False,
-        description="Succeed if user has authenticated",
-        json_schema_extra={"vmanage_key": "if-authenticated"},
+
+class AddressFamily(FeatureTemplateValidator):
+    family_type: AddressFamilyType = Field(json_schema_extra={"vmanage_key": "family-type"})
+    aggregate_address: Optional[List[AggregateAddress]] = Field(
+        default=None, json_schema_extra={"vmanage_key": "aggregate-address"}
+    )
+    ipv6_aggregate_address: Optional[List[Ipv6AggregateAddress]] = Field(
+        default=None, json_schema_extra={"vmanage_key": "ipv6-aggregate-address"}
+    )
+    network: Optional[List[Network]] = None
+    ipv6_network: Optional[List[Ipv6Network]] = Field(default=None, json_schema_extra={"vmanage_key": "ipv6-network"})
+    paths: Optional[int] = Field(default=None, json_schema_extra={"data_path": ["maximum-paths"]})
+    originate: Optional[BoolStr] = Field(default=None, json_schema_extra={"data_path": ["default-information"]})
+    policy_name: Optional[str] = Field(
+        default=None, json_schema_extra={"data_path": ["table-map"], "vmanage_key": "name"}
     )
+    filter: Optional[BoolStr] = Field(default=None, json_schema_extra={"data_path": ["table-map"]})
+    redistribute: Optional[List[Redistribute]] = None
+    model_config = ConfigDict(populate_by_name=True)
 
 
-class RadiusServer(FeatureTemplateValidator):
-    model_config = ConfigDict(populate_by_name=True, coerce_numbers_to_str=True)
+class NeighborFamilyType(str, Enum):
+    IPV4_UNICAST = "ipv4-unicast"
+    VPNV4_UNICAST = "vpnv4-unicast"
+    VPNV6_UNICAST = "vpnv6-unicast"
 
-    address: str = Field(description="The IP address or hostname of the RADIUS server")
-    auth_port: int = Field(
-        default=1812,
-        json_schema_extra={"vmanage_key": "auth-port"},
-        description="The authentication port for the RADIUS server",
-    )
-    acct_port: int = Field(
-        default=1813,
-        json_schema_extra={"vmanage_key": "acct-port"},
-        description="The accounting port for the RADIUS server",
-    )
-    timeout: int = Field(default=5, description="The timeout period in seconds for the RADIUS server")
-    retransmit: int = Field(default=3, description="The number of retransmit attempts for the RADIUS server")
-    key: str = Field(description="The key for the RADIUS server")
-    secret_key: Optional[str] = Field(
-        default=None,
-        json_schema_extra={"vmanage_key": "secret-key"},
-        description="The secret key for the RADIUS server",
-    )
-    key_enum: Optional[str] = Field(
-        default=None,
-        json_schema_extra={"vmanage_key": "key-enum"},
-        description="The key enumeration for the RADIUS server",
-    )
-    key_type: Optional[str] = Field(
-        default=None,
-        json_schema_extra={"vmanage_key": "key-type"},
-        description="The key type for the RADIUS server",
-    )
 
+class Direction(str, Enum):
+    IN = "in"
+    OUT = "out"
 
-class RadiusGroup(FeatureTemplateValidator):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
 
-    group_name: str = Field(
-        json_schema_extra={"vmanage_key": "group-name"},
-        description="The name of the RADIUS group",
-    )
-    vpn: Optional[int] = Field(description="The VPN ID for the RADIUS group")
-    source_interface: Optional[str] = Field(
-        json_schema_extra={"vmanage_key": "source-interface"},
-        description="The source interface for the RADIUS group",
-    )
-    server: List[RadiusServer] = Field(default=[], description="The list of RADIUS servers for the group")
+class RoutePolicy(FeatureTemplateValidator):
+    direction: Direction
+    pol_name: str = Field(json_schema_extra={"vmanage_key": "pol-name"})
+    model_config = ConfigDict(populate_by_name=True)
 
 
-class RadiusVPN(FeatureTemplateValidator):
-    name: str = Field(
-        description="VPN ID",
-        json_schema_extra={
-            "vmanage_key": "name",
-        },
+class NeighborAddressFamily(FeatureTemplateValidator):
+    family_type: NeighborFamilyType = Field(json_schema_extra={"vmanage_key": "family-type"})
+    prefix_num: Optional[int] = Field(
+        default=None, json_schema_extra={"data_path": ["maximum-prefixes"], "vmanage_key": "prefix-num"}
+    )
+    threshold: Optional[int] = Field(default=None, json_schema_extra={"data_path": ["maximum-prefixes"]})
+    restart: Optional[int] = Field(default=None, json_schema_extra={"data_path": ["maximum-prefixes"]})
+    warning_only: Optional[bool] = Field(
+        default=None, json_schema_extra={"data_path": ["maximum-prefixes"], "vmanage_key": "warning-only"}
     )
-    server_key: str = Field(
-        default=None,
-        description="Specify a RADIUS client server-key",
-        json_schema_extra={
-            "vmanage_key": "server-key",
-        },
-    )  # needs enryption
+    route_policy: Optional[List[RoutePolicy]] = Field(default=None, json_schema_extra={"vmanage_key": "route-policy"})
+    model_config = ConfigDict(populate_by_name=True)
 
 
-class RadiusClient(FeatureTemplateValidator):
-    ip: str = Field(
-        description="The Client IP",
-        json_schema_extra={"vmanage_key": "ip"},
+class Neighbor(FeatureTemplateValidator):
+    address: str
+    description: Optional[str] = None
+    shutdown: Optional[BoolStr] = None
+    remote_as: int = Field(json_schema_extra={"vmanage_key": "remote-as"})
+    keepalive: Optional[int] = Field(default=None, json_schema_extra={"data_path": ["timers"]})
+    holdtime: Optional[int] = Field(default=None, json_schema_extra={"data_path": ["timers"]})
+    if_name: Optional[str] = Field(
+        default=None, json_schema_extra={"data_path": ["update-source"], "vmanage_key": "if-name"}
+    )
+    next_hop_self: Optional[BoolStr] = Field(default=None, json_schema_extra={"vmanage_key": "next-hop-self"})
+    send_community: Optional[BoolStr] = Field(default=None, json_schema_extra={"vmanage_key": "send-community"})
+    send_ext_community: Optional[BoolStr] = Field(default=None, json_schema_extra={"vmanage_key": "send-ext-community"})
+    ebgp_multihop: Optional[int] = Field(default=None, json_schema_extra={"vmanage_key": "ebgp-multihop"})
+    password: Optional[str] = None
+    send_label: Optional[BoolStr] = Field(default=None, json_schema_extra={"vmanage_key": "send-label"})
+    send_label_explicit: Optional[BoolStr] = Field(
+        default=None, json_schema_extra={"vmanage_key": "send-label-explicit"}
+    )
+    as_override: Optional[BoolStr] = Field(default=None, json_schema_extra={"vmanage_key": "as-override"})
+    as_number: Optional[int] = Field(
+        default=None, json_schema_extra={"data_path": ["allowas-in"], "vmanage_key": "as-number"}
     )
-    vpn: List[RadiusVPN] = Field(
-        description="The VPN Configuration",
-        json_schema_extra={"vmanage_key": "vpn"},
+    address_family: Optional[List[NeighborAddressFamily]] = Field(
+        default=None, json_schema_extra={"vmanage_key": "address-family"}
     )
+    model_config = ConfigDict(populate_by_name=True)
 
 
-class TacacsServer(FeatureTemplateValidator):
-    model_config = ConfigDict(populate_by_name=True)
+class IPv6NeighborFamilyType(str, Enum):
+    IPV6_UNICAST = "ipv6-unicast"
 
-    address: str = Field(description="The IP address or hostname of the TACACS+ server")
-    key: str = Field(description="The key for the TACACS+ server")
-    port: int = Field(default=49, description="The port for the TACACS+ server")
-    timeout: int = Field(default=5, description="The timeout period in seconds for the TACACS+ server")
-    secret_key: Optional[str] = Field(
-        default=None,
-        json_schema_extra={"vmanage_key": "secret-key"},
-        description="The secret key for the TACACS+ server",
+
+class IPv6NeighborAddressFamily(FeatureTemplateValidator):
+    family_type: IPv6NeighborFamilyType = Field(json_schema_extra={"vmanage_key": "family-type"})
+    prefix_num: Optional[int] = Field(
+        0, json_schema_extra={"data_path": ["maximum-prefixes"], "vmanage_key": "prefix-num"}
     )
-    key_enum: Optional[str] = Field(
-        default=None,
-        json_schema_extra={"vmanage_key": "key-enum"},
-        description="The key enumeration for the TACACS+ server",
+    threshold: Optional[int] = Field(default=None, json_schema_extra={"data_path": ["maximum-prefixes"]})
+    restart: Optional[int] = Field(default=None, json_schema_extra={"data_path": ["maximum-prefixes"]})
+    warning_only: Optional[bool] = Field(
+        False, json_schema_extra={"data_path": ["maximum-prefixes"], "vmanage_key": "warning-only"}
     )
-
-
-class TacacsGroup(FeatureTemplateValidator):
+    route_policy: Optional[List[RoutePolicy]] = Field(default=None, json_schema_extra={"vmanage_key": "route-policy"})
     model_config = ConfigDict(populate_by_name=True)
 
-    group_name: str = Field(
-        json_schema_extra={"vmanage_key": "group-name"},
-        description="The name of the TACACS+ group",
+
+class Ipv6Neighbor(FeatureTemplateValidator):
+    address: str
+    description: Optional[str] = None
+    shutdown: Optional[BoolStr] = None
+    remote_as: int = Field(default=None, json_schema_extra={"vmanage_key": "remote-as"})
+    keepalive: Optional[int] = Field(default=None, json_schema_extra={"data_path": ["timers"]})
+    holdtime: Optional[int] = Field(default=None, json_schema_extra={"data_path": ["timers"]})
+    if_name: Optional[str] = Field(
+        default=None, json_schema_extra={"data_path": ["update-source"], "vmanage_key": "if-name"}
+    )
+    next_hop_self: Optional[BoolStr] = Field(default=False, json_schema_extra={"vmanage_key": "next-hop-self"})
+    send_community: Optional[BoolStr] = Field(default=True, json_schema_extra={"vmanage_key": "send-community"})
+    send_ext_community: Optional[BoolStr] = Field(default=True, json_schema_extra={"vmanage_key": "send-ext-community"})
+    ebgp_multihop: Optional[int] = Field(1, json_schema_extra={"vmanage_key": "ebgp-multihop"})
+    password: Optional[str] = None
+    send_label: Optional[BoolStr] = Field(default=False, json_schema_extra={"vmanage_key": "send-label"})
+    send_label_explicit: Optional[BoolStr] = Field(
+        default=False, json_schema_extra={"vmanage_key": "send-label-explicit"}
+    )
+    as_override: Optional[BoolStr] = Field(default=False, json_schema_extra={"vmanage_key": "as-override"})
+    as_number: Optional[int] = Field(
+        default=None, json_schema_extra={"data_path": ["allowas-in"], "vmanage_key": "as-number"}
     )
-    vpn: int = Field(default=0, description="The VPN ID for the TACACS+ group")
-    source_interface: Optional[str] = Field(
-        default=None,
-        json_schema_extra={"vmanage_key": "source-interface"},
-        description="The source interface for the TACACS+ group",
+    address_family: Optional[List[IPv6NeighborAddressFamily]] = Field(
+        default=None, json_schema_extra={"vmanage_key": "address-family"}
     )
-    server: List[TacacsServer] = Field(default=[], description="The list of TACACS+ servers for the group")
+    model_config = ConfigDict(populate_by_name=True)
 
 
-class CiscoAAAModel(FeatureTemplate):
+class CiscoBGPModel(FeatureTemplate):
     model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-    _docs_description: str = "Cisco AAA Feature Template configuration"
 
-    authentication_group: Optional[BoolStr] = Field(
-        default=False,
-        json_schema_extra={
-            "data_path": ["authentication", "dot1x", "default"],
-            "vmanage_key": "authentication_group",
-        },
-        description="Whether to enable the authentication group, GUI equivalent: Authentication Param",
-    )
-    accounting_group: Optional[BoolStr] = Field(
-        default=False,
-        json_schema_extra={
-            "data_path": ["accounting", "dot1x", "default", "start-stop"],
-            "vmanage_key": "accounting_group",
-        },
-        description="Whether to enable the accounting group, GUI equivalent: Accounting Param",
-    )
-    server_auth_order: str = Field(
-        default="local",
-        json_schema_extra={"vmanage_key": "server-auth-order"},
-        description="ServerGroups authentication order to user access",
-    )  # example: "local,tacacs-5,radius-4"
-    user: Optional[List[User]] = Field(default=None, description="List of local user configurations")
-
-    accounting_rules: Optional[List[AccountingRule]] = Field(
-        default=None,
-        description="Configure the accounting rules",
-        json_schema_extra={
-            "data_path": ["accounting"],
-            "vmanage_key": "accounting-rule",
-        },
-    )
-
-    authorization_console: Optional[BoolStr] = Field(
-        default=None,
-        description="For enabling console authorization",
-        json_schema_extra={
-            "data_path": ["authorization"],
-            "vmanage_key": "authorization-console",
-        },
-    )
-    authorization_config_commands: Optional[BoolStr] = Field(
-        default=None,
-        description="For configuration mode commands",
-        json_schema_extra={
-            "data_path": ["authorization"],
-            "vmanage_key": "authorization-config-commands",
-        },
-    )
-    authorization_rules: Optional[List[AuthorizationRules]] = Field(
-        default=None,
-        description="Configure the accounting rules",
-        json_schema_extra={
-            "data_path": ["authorization"],
-            "vmanage_key": "authorization-rule",
-        },
-    )
-    radius: Optional[List[RadiusGroup]] = Field(default=None, description="List of Radius group configurations")
-    radius_client: Optional[List[RadiusClient]] = Field(
-        default=None,
-        json_schema_extra={
-            "data_path": ["radius-dynamic-author"],
-            "vmanage_key": "radius-client",
-        },
-        description="Specify a RADIUS client",
-    )
-    domain_stripping: Optional[DomainStripping] = Field(
-        default=None,
-        json_schema_extra={
-            "data_path": ["radius-dynamic-author"],
-            "vmanage_key": "domain-stripping",
-        },
-        description="The domain stripping configuration",
-    )
-    authentication_type: Optional[AuthenticationType] = Field(
-        default="any",
-        json_schema_extra={
-            "data_path": ["radius-dynamic-author"],
-            "vmanage_key": "auth-type",
-        },
-        description="Authentication Type",
-    )
-    port: Optional[int] = Field(
-        default=1700,
-        json_schema_extra={
-            "data_path": ["radius-dynamic-author"],
-            "vmanage_key": "port",
-        },
-        description="Specify Radius Dynamic Author Port",
-    )
-    server_key_password: Optional[str] = Field(
-        default=None,
-        json_schema_extra={
-            "data_path": ["radius-dynamic-author"],
-            "vmanage_key": "rda-server-key",
-        },
-        description="Specify a radius dynamic author server-key",
-    )  # needs encryption
-
-    cts_authorization_list: Optional[str] = Field(
-        default=None,
-        json_schema_extra={
-            "data_path": ["radius-trustsec"],
-            "vmanage_key": "cts-auth-list",
-        },
-        description="Specify a radius dynamic author server-key",
-    )
-    radius_trustsec_group: Optional[str] = Field(
-        default=None,
-        json_schema_extra={
-            "data_path": ["radius-trustsec"],
-            "vmanage_key": "radius-trustsec-group",
-        },
-        description="RADIUS trustsec group",
+    as_num: Optional[str] = Field(default=None, json_schema_extra={"data_path": ["bgp"], "vmanage_key": "as-num"})
+    shutdown: Optional[BoolStr] = Field(default=None, json_schema_extra={"data_path": ["bgp"]})
+    router_id: Optional[str] = Field(default=None, json_schema_extra={"data_path": ["bgp"], "vmanage_key": "router-id"})
+    propagate_aspath: Optional[bool] = Field(
+        default=None, json_schema_extra={"data_path": ["bgp"], "vmanage_key": "propagate-aspath"}
+    )
+    propagate_community: Optional[bool] = Field(
+        default=None, json_schema_extra={"data_path": ["bgp"], "vmanage_key": "propagate-community"}
+    )
+    route_target_ipv4: List[RouteTargetIpv4] = Field(
+        [], json_schema_extra={"data_path": ["bgp", "target"], "vmanage_key": "route-target-ipv4"}
+    )
+    route_target_ipv6: List[RouteTargetIpv6] = Field(
+        [], json_schema_extra={"data_path": ["bgp", "target"], "vmanage_key": "route-target-ipv6"}
+    )
+    mpls_interface: Optional[List[MplsInterface]] = Field(
+        default=None, json_schema_extra={"data_path": ["bgp"], "vmanage_key": "mpls-interface"}
+    )
+    external: Optional[int] = Field(default=None, json_schema_extra={"data_path": ["bgp", "distance"]})
+    internal: Optional[int] = Field(default=None, json_schema_extra={"data_path": ["bgp", "distance"]})
+    local: Optional[int] = Field(default=None, json_schema_extra={"data_path": ["bgp", "distance"]})
+    keepalive: Optional[int] = Field(default=None, json_schema_extra={"data_path": ["bgp", "timers"]})
+    holdtime: Optional[int] = Field(default=None, json_schema_extra={"data_path": ["bgp", "timers"]})
+    always_compare: Optional[bool] = Field(
+        default=None, json_schema_extra={"data_path": ["bgp", "best-path", "med"], "vmanage_key": "always-compare"}
+    )
+    deterministic: Optional[BoolStr] = Field(default=None, json_schema_extra={"data_path": ["bgp", "best-path", "med"]})
+    missing_as_worst: Optional[BoolStr] = Field(
+        default=None, json_schema_extra={"data_path": ["bgp", "best-path", "med"], "vmanage_key": "missing-as-worst"}
+    )
+    compare_router_id: Optional[BoolStr] = Field(
+        default=None, json_schema_extra={"data_path": ["bgp", "best-path"], "vmanage_key": "compare-router-id"}
+    )
+    multipath_relax: Optional[BoolStr] = Field(
+        default=None, json_schema_extra={"data_path": ["bgp", "best-path", "as-path"], "vmanage_key": "multipath-relax"}
+    )
+    address_family: Optional[List[AddressFamily]] = Field(
+        default=None, json_schema_extra={"data_path": ["bgp"], "vmanage_key": "address-family"}
+    )
+    neighbor: Optional[List[Neighbor]] = Field(default=None, json_schema_extra={"data_path": ["bgp"]})
+    ipv6_neighbor: Optional[List[Ipv6Neighbor]] = Field(
+        default=None, json_schema_extra={"data_path": ["bgp"], "vmanage_key": "ipv6-neighbor"}
     )
-    tacacs: Optional[List[TacacsGroup]] = Field(default=None, description="List of TACACS group configurations")
 
     payload_path: ClassVar[Path] = Path(__file__).parent / "DEPRECATED"
-    type: ClassVar[str] = "cedge_aaa"
+    type: ClassVar[str] = "cisco_bgp"
```

### Comparing `catalystwan-0.33.6.post0/catalystwan/api/templates/models/cisco_ntp_model.py` & `catalystwan-0.33.7/catalystwan/api/templates/models/cisco_snmp_model.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,60 +1,88 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
+from enum import Enum
 from pathlib import Path
 from typing import ClassVar, List, Optional
 
 from pydantic import ConfigDict, Field
 
 from catalystwan.api.templates.bool_str import BoolStr
 from catalystwan.api.templates.feature_template import FeatureTemplate, FeatureTemplateValidator
 
 
-class Server(FeatureTemplateValidator):
-    model_config = ConfigDict(populate_by_name=True)
+class Oid(FeatureTemplateValidator):
+    id: str
+    exclude: Optional[BoolStr] = None
+
+
+class View(FeatureTemplateValidator):
+    name: str
+    oid: Optional[List[Oid]] = None
+
+
+class Authorization(str, Enum):
+    READ_ONLY = "read-only"
+
+
+class Community(FeatureTemplateValidator):
+    name: str
+    view: str
+    authorization: Authorization
 
-    name: str = Field(description="The hostname or IP address of the NTP server")
-    key: Optional[int] = Field(default=None, description="The identifier for the authentication key")
-    vpn: Optional[int] = Field(default=None, description="The VPN ID associated with the NTP server")
-    version: Optional[int] = Field(default=None, description="The NTP version used")
-    source_interface: Optional[str] = Field(
-        default=None,
-        json_schema_extra={"vmanage_key": "source-interface"},
-        description="The source interface for NTP messages",
-    )
-    prefer: Optional[BoolStr] = Field(default=None, description="Whether this server is preferred over others")
 
+class SecurityLevel(str, Enum):
+    NOAUTHNOPRIV = "no-auth-no-priv"
+    AUTHNOPRIV = "auth-no-priv"
+    AUTHPRIV = "auth-priv"
 
-class Authentication(FeatureTemplateValidator):
+
+class Group(FeatureTemplateValidator):
+    name: str
+    security_level: SecurityLevel = Field(json_schema_extra={"vmanage_key": "security-level"})
+    view: str
+    model_config = ConfigDict(populate_by_name=True)
+
+
+class Auth(str, Enum):
+    MD5 = "md5"
+    SHA = "sha"
+
+
+class Priv(str, Enum):
+    AES_CFB_128 = "aes-cfb-128"
+
+
+class User(FeatureTemplateValidator):
+    name: str
+    auth: Optional[Auth] = None
+    auth_password: Optional[str] = Field(default=None, json_schema_extra={"vmanage_key": "auth-password"})
+    priv: Optional[Priv] = None
+    priv_password: Optional[str] = Field(default=None, json_schema_extra={"vmanage_key": "priv-password"})
+    group: str
     model_config = ConfigDict(populate_by_name=True)
 
-    number: int = Field(description="The authentication key number")
-    md5: str = Field(description="The MD5 hash used for authentication")
+
+class Target(FeatureTemplateValidator):
+    vpn_id: int = Field(json_schema_extra={"vmanage_key": "vpn-id"})
+    ip: str
+    port: int
+    community_name: str = Field(default=None, json_schema_extra={"vmanage_key": "community-name"})
+    user: Optional[str] = None
+    source_interface: str = Field(default=None, json_schema_extra={"vmanage_key": "source-interface"})
+    model_config = ConfigDict(populate_by_name=True)
 
 
-class CiscoNTPModel(FeatureTemplate):
+class CiscoSNMPModel(FeatureTemplate):
     model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-    _docs_description: str = "Cisco NTP Feature Template configuration"
 
-    server: List[Server] = Field(default=[], description="List of NTP servers")
-    authentication: Optional[List[Authentication]] = Field(
-        default=None, json_schema_extra={"data_path": ["keys"]}, description="List of authentication keys"
-    )
-    trusted: Optional[List[int]] = Field(
-        default=None, json_schema_extra={"data_path": ["keys"]}, description="List of trusted key numbers"
-    )
-    enable: Optional[BoolStr] = Field(
-        default=None, json_schema_extra={"data_path": ["master"]}, description="Whether the device is an NTP master"
-    )
-    stratum: Optional[int] = Field(
-        default=None,
-        json_schema_extra={"data_path": ["master"]},
-        description="The stratum level if the device is an NTP master",
-    )
-    source: Optional[str] = Field(
-        default=None,
-        json_schema_extra={"data_path": ["master"]},
-        description="The source interface for NTP messages if the device is an NTP master",
-    )
+    shutdown: Optional[BoolStr] = True
+    contact: Optional[str] = None
+    location: Optional[str] = None
+    view: Optional[List[View]] = None
+    community: Optional[List[Community]] = None
+    group: Optional[List[Group]] = None
+    user: Optional[List[User]] = None
+    target: Optional[List[Target]] = Field(default=None, json_schema_extra={"data_path": ["trap"]})
 
     payload_path: ClassVar[Path] = Path(__file__).parent / "DEPRECATED"
-    type: ClassVar[str] = "cisco_ntp"
+    type: ClassVar[str] = "cisco_snmp"
```

### Comparing `catalystwan-0.33.6.post0/catalystwan/api/templates/models/supported.py` & `catalystwan-0.33.7/catalystwan/api/templates/models/supported.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -14,23 +14,23 @@
 from catalystwan.api.templates.models.cisco_vpn_model import CiscoVPNModel
 from catalystwan.api.templates.models.omp_vsmart_model import OMPvSmart
 from catalystwan.api.templates.models.security_vsmart_model import SecurityvSmart
 from catalystwan.api.templates.models.system_vsmart_model import SystemVsmart
 
 available_models = {
     "cisco_aaa": CiscoAAAModel,
-    "cisco_banner": CiscoBannerModel,
     "cisco_bfd": CiscoBFDModel,
+    "cisco_banner": CiscoBannerModel,
     "cisco_ntp": CiscoNTPModel,
     "cisco_ospf": CiscoOSPFModel,
     "cisco_logging": CiscoLoggingModel,
+    "omp_vsmart": OMPvSmart,
+    "security_vsmart": SecurityvSmart,
+    "system_vsmart": SystemVsmart,
     "cisco_vpn_interface": CiscoVpnInterfaceModel,
     "cisco_system": CiscoSystemModel,
     "cisco_vpn": CiscoVPNModel,
     "cisco_snmp": CiscoSNMPModel,
     "cisco_system": CiscoSystemModel,
     "cisco_secure_internet_gateway": CiscoSecureInternetGatewayModel,
     "cisco_omp": CiscoOMPModel,
-    "omp_vsmart": OMPvSmart,
-    "security_vsmart": SecurityvSmart,
-    "system_vsmart": SystemVsmart,
 }
```

### Comparing `catalystwan-0.33.6.post0/catalystwan/api/templates/payloads/aaa/aaa_model.py` & `catalystwan-0.33.7/catalystwan/api/templates/payloads/aaa/aaa_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/api/templates/payloads/aaa/feature/aaa.json.j2` & `catalystwan-0.33.7/catalystwan/api/templates/payloads/aaa/feature/aaa.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/api/templates/payloads/aaa/feature/accounting.json.j2` & `catalystwan-0.33.7/catalystwan/api/templates/payloads/aaa/feature/accounting.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/api/templates/payloads/aaa/feature/radius.json.j2` & `catalystwan-0.33.7/catalystwan/api/templates/payloads/aaa/feature/radius.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/api/templates/payloads/aaa/feature/tacacs.json.j2` & `catalystwan-0.33.7/catalystwan/api/templates/payloads/aaa/feature/tacacs.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/api/templates/payloads/aaa/feature/user.json.j2` & `catalystwan-0.33.7/catalystwan/api/templates/payloads/aaa/feature/user.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/api/templates/payloads/cisco_vpn/cisco_vpn_model.py` & `catalystwan-0.33.7/catalystwan/api/templates/payloads/cisco_vpn/cisco_vpn_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/api/templates/payloads/cisco_vpn/feature/cisco_vpn.json.j2` & `catalystwan-0.33.7/catalystwan/api/templates/payloads/cisco_vpn/feature/cisco_vpn.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/api/templates/payloads/cisco_vpn/feature/dns.json.j2` & `catalystwan-0.33.7/catalystwan/api/templates/payloads/cisco_vpn/feature/dns.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/api/templates/payloads/cisco_vpn/feature/ipv4route.json.j2` & `catalystwan-0.33.7/catalystwan/api/templates/payloads/cisco_vpn/feature/ipv4route.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/api/templates/payloads/cisco_vpn/feature/ipv6route.json.j2` & `catalystwan-0.33.7/catalystwan/api/templates/payloads/cisco_vpn/feature/ipv6route.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/api/templates/payloads/cisco_vpn/feature/mapping.json.j2` & `catalystwan-0.33.7/catalystwan/api/templates/payloads/cisco_vpn/feature/mapping.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/api/templates/payloads/tenant/tenant.json.j2` & `catalystwan-0.33.7/catalystwan/api/templates/payloads/tenant/tenant.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/api/templates/payloads/tenant/tenant_model.py` & `catalystwan-0.33.7/catalystwan/api/templates/payloads/tenant/tenant_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/api/tenant_backup_restore_api.py` & `catalystwan-0.33.7/catalystwan/api/tenant_backup_restore_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/api/tenant_management_api.py` & `catalystwan-0.33.7/catalystwan/api/tenant_management_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/api/tenant_migration_api.py` & `catalystwan-0.33.7/catalystwan/api/tenant_migration_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/api/versions_utils.py` & `catalystwan-0.33.7/catalystwan/api/versions_utils.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/api/virtual_image_action_api.py` & `catalystwan-0.33.7/catalystwan/api/virtual_image_action_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/dataclasses.py` & `catalystwan-0.33.7/catalystwan/dataclasses.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/endpoints/__init__.py` & `catalystwan-0.33.7/catalystwan/endpoints/__init__.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/endpoints/administration_user_and_group.py` & `catalystwan-0.33.7/catalystwan/endpoints/administration_user_and_group.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/endpoints/certificate_management_device.py` & `catalystwan-0.33.7/catalystwan/endpoints/certificate_management_device.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/endpoints/certificate_management_vmanage.py` & `catalystwan-0.33.7/catalystwan/endpoints/certificate_management_vmanage.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/endpoints/client.py` & `catalystwan-0.33.7/catalystwan/endpoints/client.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/endpoints/cluster_management.py` & `catalystwan-0.33.7/catalystwan/endpoints/cluster_management.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/device/software_update.py` & `catalystwan-0.33.7/catalystwan/endpoints/configuration/device/software_update.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/disaster_recovery.py` & `catalystwan-0.33.7/catalystwan/endpoints/configuration/disaster_recovery.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/feature_profile/sdwan/policy_object.py` & `catalystwan-0.33.7/catalystwan/endpoints/configuration/feature_profile/sdwan/policy_object.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/feature_profile/sdwan/system.py` & `catalystwan-0.33.7/catalystwan/endpoints/configuration/feature_profile/sdwan/system.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/feature_profile/sdwan/transport.py` & `catalystwan-0.33.7/catalystwan/endpoints/configuration/feature_profile/sdwan/transport.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/definition/access_control_list.py` & `catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/definition/access_control_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/definition/access_control_list_ipv6.py` & `catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/definition/access_control_list_ipv6.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/definition/control.py` & `catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/definition/control.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/definition/device_access.py` & `catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/definition/device_access.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/definition/device_access_ipv6.py` & `catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/definition/device_access_ipv6.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/definition/hub_and_spoke.py` & `catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/definition/hub_and_spoke.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/definition/mesh.py` & `catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/definition/mesh.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/definition/qos_map.py` & `catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/definition/qos_map.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/definition/rewrite.py` & `catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/definition/rewrite.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/definition/rule_set.py` & `catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/definition/rule_set.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/definition/security_group.py` & `catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/definition/security_group.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/definition/traffic_data.py` & `catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/definition/traffic_data.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/definition/vpn_membership.py` & `catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/definition/vpn_membership.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/definition/zone_based_firewall.py` & `catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/definition/zone_based_firewall.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/list/app.py` & `catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/app.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/list/app_probe.py` & `catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/app_probe.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/list/as_path.py` & `catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/as_path.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/list/class_map.py` & `catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/class_map.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/list/color.py` & `catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/color.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/list/community.py` & `catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/community.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/list/data_ipv6_prefix.py` & `catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/data_ipv6_prefix.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/list/data_prefix.py` & `catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/data_prefix.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/list/expanded_community.py` & `catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/expanded_community.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/list/fqdn.py` & `catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/fqdn.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/list/geo_location.py` & `catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/geo_location.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/list/ips_signature.py` & `catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/ips_signature.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/list/ipv6_prefix.py` & `catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/ipv6_prefix.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/list/local_app.py` & `catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/local_app.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/list/local_domain.py` & `catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/local_domain.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/list/mirror.py` & `catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/mirror.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/list/policer.py` & `catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/policer.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/list/port.py` & `catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/port.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/list/preferred_color_group.py` & `catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/preferred_color_group.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/list/prefix.py` & `catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/prefix.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/list/protocol_name.py` & `catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/protocol_name.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/list/region.py` & `catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/region.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/list/site.py` & `catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/site.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/list/sla.py` & `catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/sla.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/list/tloc.py` & `catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/tloc.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/list/url_allow_list.py` & `catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/url_allow_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/list/url_block_list.py` & `catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/url_block_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/list/vpn.py` & `catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/vpn.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/list/zone.py` & `catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/list/zone.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/security_template.py` & `catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/security_template.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/vedge_template.py` & `catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/vedge_template.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/policy/vsmart_template.py` & `catalystwan-0.33.7/catalystwan/endpoints/configuration/policy/vsmart_template.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/endpoints/configuration/software_actions.py` & `catalystwan-0.33.7/catalystwan/endpoints/configuration/software_actions.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/endpoints/configuration_dashboard_status.py` & `catalystwan-0.33.7/catalystwan/endpoints/configuration_dashboard_status.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/endpoints/configuration_device_actions.py` & `catalystwan-0.33.7/catalystwan/endpoints/configuration_device_actions.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/endpoints/configuration_device_inventory.py` & `catalystwan-0.33.7/catalystwan/endpoints/configuration_device_inventory.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/endpoints/configuration_device_template.py` & `catalystwan-0.33.7/catalystwan/endpoints/configuration_device_template.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/endpoints/configuration_feature_profile.py` & `catalystwan-0.33.7/catalystwan/endpoints/configuration_feature_profile.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/endpoints/configuration_group.py` & `catalystwan-0.33.7/catalystwan/endpoints/configuration_group.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/endpoints/configuration_settings.py` & `catalystwan-0.33.7/catalystwan/endpoints/configuration_settings.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/endpoints/endpoints_container.py` & `catalystwan-0.33.7/catalystwan/endpoints/endpoints_container.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/endpoints/misc.py` & `catalystwan-0.33.7/catalystwan/endpoints/misc.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/endpoints/monitoring/device_details.py` & `catalystwan-0.33.7/catalystwan/endpoints/monitoring/device_details.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/endpoints/monitoring/status.py` & `catalystwan-0.33.7/catalystwan/endpoints/monitoring/status.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/endpoints/real_time_monitoring/reboot_history.py` & `catalystwan-0.33.7/catalystwan/endpoints/real_time_monitoring/reboot_history.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/endpoints/sdavc_cloud_connector.py` & `catalystwan-0.33.7/catalystwan/endpoints/sdavc_cloud_connector.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/endpoints/tenant_backup_restore.py` & `catalystwan-0.33.7/catalystwan/endpoints/tenant_backup_restore.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/endpoints/tenant_management.py` & `catalystwan-0.33.7/catalystwan/endpoints/tenant_management.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/endpoints/tenant_migration.py` & `catalystwan-0.33.7/catalystwan/endpoints/tenant_migration.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/endpoints/troubleshooting_tools/device_connectivity.py` & `catalystwan-0.33.7/catalystwan/endpoints/troubleshooting_tools/device_connectivity.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/endpoints/url_monitoring.py` & `catalystwan-0.33.7/catalystwan/endpoints/url_monitoring.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/exceptions.py` & `catalystwan-0.33.7/catalystwan/exceptions.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/integration_tests/test_find_template_values.py` & `catalystwan-0.33.7/catalystwan/integration_tests/test_find_template_values.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/logging.conf` & `catalystwan-0.33.7/catalystwan/logging.conf`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/models/configuration/config_migration.py` & `catalystwan-0.33.7/catalystwan/models/configuration/config_migration.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/README.md` & `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/README.md`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/builder.py` & `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/builder.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/common.py` & `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/common.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/management/vpn.py` & `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/management/vpn.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/__init__.py` & `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/__init__.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/app_probe.py` & `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/app_probe.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/application_list.py` & `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/application_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/color_list.py` & `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/color_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/data_prefix.py` & `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/data_prefix.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/expanded_community_list.py` & `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/expanded_community_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/fowarding_class.py` & `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/fowarding_class.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/ipv6_data_prefix.py` & `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/ipv6_data_prefix.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/ipv6_prefix_list.py` & `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/ipv6_prefix_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/policier.py` & `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/policier.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/prefered_group_color.py` & `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/prefered_group_color.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/prefix_list.py` & `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/prefix_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/sla_class.py` & `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/sla_class.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/standard_community.py` & `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/standard_community.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/tloc_list.py` & `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/tloc_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/application_list.py` & `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/application_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/data_prefix.py` & `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/data_prefix.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/fqdn.py` & `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/fqdn.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/geolocation_list.py` & `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/geolocation_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/ips_signature.py` & `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/ips_signature.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/local_domain.py` & `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/local_domain.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/protocol_list.py` & `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/protocol_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/security_port.py` & `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/security_port.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/url.py` & `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/url.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/zone.py` & `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/zone.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/service/acl.py` & `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/service/acl.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/service/appqoe.py` & `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/service/appqoe.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/service/bgp.py` & `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/service/bgp.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/service/dhcp_server.py` & `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/service/dhcp_server.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/service/eigrp.py` & `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/service/eigrp.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/service/lan/common.py` & `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/service/lan/common.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/service/lan/ethernet.py` & `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/service/lan/ethernet.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/service/lan/gre.py` & `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/service/lan/gre.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/service/lan/ipsec.py` & `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/service/lan/ipsec.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/service/lan/svi.py` & `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/service/lan/svi.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/service/lan/vpn.py` & `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/service/lan/vpn.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/service/multicast.py` & `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/service/multicast.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/service/object_tracker.py` & `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/service/object_tracker.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/service/ospf.py` & `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/service/ospf.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/service/ospfv3.py` & `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/service/ospfv3.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/service/route_policy.py` & `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/service/route_policy.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/service/service_insertion_attachment.py` & `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/service/service_insertion_attachment.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/service/switchport.py` & `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/service/switchport.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/service/tracker.py` & `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/service/tracker.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/service/wireless_lan.py` & `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/service/wireless_lan.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/system/aaa.py` & `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/system/aaa.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/models/configuration/feature_profile/sdwan/transport/cellular_controller.py` & `catalystwan-0.33.7/catalystwan/models/configuration/feature_profile/sdwan/transport/cellular_controller.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/models/device_inventory.py` & `catalystwan-0.33.7/catalystwan/models/device_inventory.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/models/misc/application_protocols.py` & `catalystwan-0.33.7/catalystwan/models/misc/application_protocols.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/models/policy/__init__.py` & `catalystwan-0.33.7/catalystwan/models/policy/__init__.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/models/policy/centralized.py` & `catalystwan-0.33.7/catalystwan/models/policy/centralized.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/models/policy/definitions/access_control_list.py` & `catalystwan-0.33.7/catalystwan/models/policy/definitions/access_control_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/models/policy/definitions/access_control_list_ipv6.py` & `catalystwan-0.33.7/catalystwan/models/policy/definitions/access_control_list_ipv6.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/models/policy/definitions/control.py` & `catalystwan-0.33.7/catalystwan/models/policy/definitions/control.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/models/policy/definitions/device_access.py` & `catalystwan-0.33.7/catalystwan/models/policy/definitions/device_access.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/models/policy/definitions/device_access_ipv6.py` & `catalystwan-0.33.7/catalystwan/models/policy/definitions/device_access_ipv6.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/models/policy/definitions/hub_and_spoke.py` & `catalystwan-0.33.7/catalystwan/models/policy/definitions/hub_and_spoke.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/models/policy/definitions/mesh.py` & `catalystwan-0.33.7/catalystwan/models/policy/definitions/mesh.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/models/policy/definitions/qos_map.py` & `catalystwan-0.33.7/catalystwan/models/policy/definitions/qos_map.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/models/policy/definitions/rewrite.py` & `catalystwan-0.33.7/catalystwan/models/policy/definitions/rewrite.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/models/policy/definitions/rule_set.py` & `catalystwan-0.33.7/catalystwan/models/policy/definitions/rule_set.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/models/policy/definitions/security_group.py` & `catalystwan-0.33.7/catalystwan/models/policy/definitions/security_group.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/models/policy/definitions/traffic_data.py` & `catalystwan-0.33.7/catalystwan/models/policy/definitions/traffic_data.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/models/policy/definitions/vpn_membership.py` & `catalystwan-0.33.7/catalystwan/models/policy/definitions/vpn_membership.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/models/policy/definitions/zone_based_firewall.py` & `catalystwan-0.33.7/catalystwan/models/policy/definitions/zone_based_firewall.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/models/policy/lists.py` & `catalystwan-0.33.7/catalystwan/models/policy/lists.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/models/policy/lists_entries.py` & `catalystwan-0.33.7/catalystwan/models/policy/lists_entries.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/models/policy/localized.py` & `catalystwan-0.33.7/catalystwan/models/policy/localized.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/models/policy/policy.py` & `catalystwan-0.33.7/catalystwan/models/policy/policy.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/models/policy/policy_definition.py` & `catalystwan-0.33.7/catalystwan/models/policy/policy_definition.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/models/policy/policy_list.py` & `catalystwan-0.33.7/catalystwan/models/policy/policy_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/models/policy/security.py` & `catalystwan-0.33.7/catalystwan/models/policy/security.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/models/tenant.py` & `catalystwan-0.33.7/catalystwan/models/tenant.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/models/url_monitoring.py` & `catalystwan-0.33.7/catalystwan/models/url_monitoring.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/response.py` & `catalystwan-0.33.7/catalystwan/response.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/session.py` & `catalystwan-0.33.7/catalystwan/session.py`

 * *Files 0% similar despite different names*

```diff
@@ -417,15 +417,15 @@
 
     def get_tenant_id(self) -> str:
         """Gets tenant UUID for its subdomain.
 
         Returns:
             Tenant UUID.
         """
-        tenants = self.get("dataservice/tenant").dataseq(Tenant, validate=False)
+        tenants = self.get("dataservice/tenant").dataseq(Tenant)
         tenant = tenants.filter(subdomain=self.subdomain).single_or_default()
 
         if not tenant or not tenant.tenant_id:
             raise TenantSubdomainNotFound(f"Tenant ID for sub-domain: {self.subdomain} not found")
 
         return tenant.tenant_id
```

### Comparing `catalystwan-0.33.6.post0/catalystwan/tests/templates/definitions/basic/children.json` & `catalystwan-0.33.7/catalystwan/tests/templates/definitions/basic/children.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/tests/templates/definitions/basic/children_nested.json` & `catalystwan-0.33.7/catalystwan/tests/templates/definitions/basic/children_nested.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/tests/templates/definitions/basic/children_nested_datapath.json` & `catalystwan-0.33.7/catalystwan/tests/templates/definitions/basic/children_nested_datapath.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/tests/templates/definitions/cisco_aaa.json` & `catalystwan-0.33.7/catalystwan/tests/templates/definitions/iuo.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8927021329365079%*

 * *Differences: {"'templateDefinition'": "{'user': {'vipValue': {0: {'pubkey-chain': "*

 * *                         "OrderedDict([('vipObjectType', 'tree'), ('vipPrimaryKey', "*

 * *                         "['key-string']), ('vipType', 'ignore'), ('vipValue', [])])}, 1: "*

 * *                         "{'privilege': {'vipValue': '14'}, 'pubkey-chain': "*

 * *                         "OrderedDict([('vipObjectType', 'tree'), ('vipPrimaryKey', "*

 * *                         "['key-string']), ('vipType', 'ignore'), ('vipValue', [])])}}}, delete: "*

 * * […]*

```diff
@@ -1,37 +1,13 @@
 {
     "deviceType": [
         "vedge-C8000V"
     ],
     "factoryDefault": false,
     "templateDefinition": {
-        "accounting": {
-            "dot1x": {
-                "default": {
-                    "start-stop": {
-                        "accounting_group": {
-                            "vipObjectType": "object",
-                            "vipType": "constant",
-                            "vipValue": "false"
-                        }
-                    }
-                }
-            }
-        },
-        "authentication": {
-            "dot1x": {
-                "default": {
-                    "authentication_group": {
-                        "vipObjectType": "object",
-                        "vipType": "constant",
-                        "vipValue": "true"
-                    }
-                }
-            }
-        },
         "radius": {
             "vipObjectType": "tree",
             "vipPrimaryKey": [
                 "group-name"
             ],
             "vipType": "constant",
             "vipValue": [
@@ -91,31 +67,14 @@
                         "vipObjectType": "object",
                         "vipType": "constant",
                         "vipValue": 1
                     }
                 }
             ]
         },
-        "radius-dynamic-author": {
-            "auth-type": {
-                "vipObjectType": "object",
-                "vipType": "constant",
-                "vipValue": "any"
-            },
-            "domain-stripping": {
-                "vipObjectType": "object",
-                "vipType": "constant",
-                "vipValue": "no"
-            },
-            "port": {
-                "vipObjectType": "object",
-                "vipType": "constant",
-                "vipValue": 1700
-            }
-        },
         "server-auth-order": {
             "vipObjectType": "object",
             "vipType": "constant",
             "vipValue": "local"
         },
         "user": {
             "vipObjectType": "tree",
@@ -136,14 +95,22 @@
                         "vipValue": "str"
                     },
                     "privilege": {
                         "vipObjectType": "object",
                         "vipType": "constant",
                         "vipValue": "15"
                     },
+                    "pubkey-chain": {
+                        "vipObjectType": "tree",
+                        "vipPrimaryKey": [
+                            "key-string"
+                        ],
+                        "vipType": "ignore",
+                        "vipValue": []
+                    },
                     "secret": {
                         "vipObjectType": "object",
                         "vipType": "constant",
                         "vipValue": "zyx"
                     }
                 },
                 {
@@ -156,23 +123,31 @@
                         "vipObjectType": "object",
                         "vipType": "constant",
                         "vipValue": "rnd"
                     },
                     "privilege": {
                         "vipObjectType": "object",
                         "vipType": "constant",
-                        "vipValue": "1"
+                        "vipValue": "14"
+                    },
+                    "pubkey-chain": {
+                        "vipObjectType": "tree",
+                        "vipPrimaryKey": [
+                            "key-string"
+                        ],
+                        "vipType": "ignore",
+                        "vipValue": []
                     },
                     "secret": {
                         "vipObjectType": "object",
                         "vipType": "constant",
                         "vipValue": "dnr"
                     }
                 }
             ]
         }
     },
     "templateDescription": "zyx",
     "templateMinVersion": "15.0.0",
-    "templateName": "cisco_aaa",
+    "templateName": "iuo",
     "templateType": "cedge_aaa"
 }
```

### Comparing `catalystwan-0.33.6.post0/catalystwan/tests/templates/definitions/cisco_aaa_complex.json` & `catalystwan-0.33.7/catalystwan/tests/templates/definitions/complex_aaa.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7447652134855679%*

 * *Differences: {"'deviceType'": '[]',*

 * * "'templateDefinition'": "{'server-auth-order': {'vipValue': 'local'}, 'user': {'vipValue': {1: "*

 * *                         "{'name': {'vipValue': 'test2'}, 'password': {'vipValue': '*****'}, "*

 * *                         "'secret': {'vipValue': 'secret'}, 'pubkey-chain': "*

 * *                         "OrderedDict([('vipObjectType', 'tree'), ('vipPrimaryKey', "*

 * *                         "['key-string']), ('vipType', 'ignore'), ('vipValue', [])])}, insert: "*

 * *                         "[(0, Orde […]*

```diff
@@ -1,133 +1,23 @@
 {
-    "deviceType": [
-        "vedge-C8000V"
-    ],
+    "deviceType": [],
     "factoryDefault": false,
     "templateDefinition": {
-        "accounting": {
-            "accounting-rule": {
-                "vipObjectType": "tree",
-                "vipPrimaryKey": [
-                    "rule-id"
-                ],
-                "vipType": "constant",
-                "vipValue": [
-                    {
-                        "group": {
-                            "vipObjectType": "object",
-                            "vipType": "constant",
-                            "vipValue": "radius-4,tacacs-5"
-                        },
-                        "level": {
-                            "vipObjectType": "object",
-                            "vipType": "constant",
-                            "vipValue": "1"
-                        },
-                        "method": {
-                            "vipObjectType": "object",
-                            "vipType": "constant",
-                            "vipValue": "commands"
-                        },
-                        "rule-id": {
-                            "vipObjectType": "object",
-                            "vipType": "constant",
-                            "vipValue": "1111"
-                        },
-                        "start-stop": {
-                            "vipObjectType": "object",
-                            "vipType": "constant",
-                            "vipValue": "false"
-                        }
-                    }
-                ]
-            },
-            "dot1x": {
-                "default": {
-                    "start-stop": {
-                        "accounting_group": {
-                            "vipObjectType": "object",
-                            "vipType": "constant",
-                            "vipValue": "true"
-                        }
-                    }
-                }
-            }
-        },
-        "authentication": {
-            "dot1x": {
-                "default": {
-                    "authentication_group": {
-                        "vipObjectType": "object",
-                        "vipType": "constant",
-                        "vipValue": "true"
-                    }
-                }
-            }
-        },
-        "authorization": {
-            "authorization-config-commands": {
-                "vipObjectType": "object",
-                "vipType": "constant",
-                "vipValue": "true"
-            },
-            "authorization-console": {
-                "vipObjectType": "object",
-                "vipType": "constant",
-                "vipValue": "true"
-            },
-            "authorization-rule": {
-                "vipObjectType": "tree",
-                "vipPrimaryKey": [
-                    "rule-id"
-                ],
-                "vipType": "constant",
-                "vipValue": [
-                    {
-                        "group": {
-                            "vipObjectType": "object",
-                            "vipType": "constant",
-                            "vipValue": "radius-4,tacacs-5"
-                        },
-                        "if-authenticated": {
-                            "vipObjectType": "object",
-                            "vipType": "constant",
-                            "vipValue": "true"
-                        },
-                        "level": {
-                            "vipObjectType": "object",
-                            "vipType": "constant",
-                            "vipValue": "15"
-                        },
-                        "method": {
-                            "vipObjectType": "object",
-                            "vipType": "constant",
-                            "vipValue": "commands"
-                        },
-                        "rule-id": {
-                            "vipObjectType": "object",
-                            "vipType": "constant",
-                            "vipValue": "12"
-                        }
-                    }
-                ]
-            }
-        },
         "radius": {
             "vipObjectType": "tree",
             "vipPrimaryKey": [
                 "group-name"
             ],
             "vipType": "constant",
             "vipValue": [
                 {
                     "group-name": {
                         "vipObjectType": "object",
                         "vipType": "constant",
-                        "vipValue": "radius-4"
+                        "vipValue": "group1"
                     },
                     "server": {
                         "vipObjectType": "tree",
                         "vipPrimaryKey": [
                             "address"
                         ],
                         "vipType": "constant",
@@ -142,186 +32,178 @@
                                     "vipObjectType": "object",
                                     "vipType": "constant",
                                     "vipValue": "1.1.1.1"
                                 },
                                 "auth-port": {
                                     "vipObjectType": "object",
                                     "vipType": "constant",
-                                    "vipValue": 1000
+                                    "vipValue": 1812
                                 },
                                 "key": {
                                     "vipObjectType": "object",
                                     "vipType": "constant",
-                                    "vipValue": "radius_key"
+                                    "vipValue": "test_key"
                                 },
                                 "retransmit": {
                                     "vipObjectType": "object",
                                     "vipType": "constant",
+                                    "vipValue": 3
+                                },
+                                "secret-key": {
+                                    "vipObjectType": "object",
+                                    "vipType": "constant",
+                                    "vipValue": "secret_key"
+                                },
+                                "timeout": {
+                                    "vipObjectType": "object",
+                                    "vipType": "constant",
                                     "vipValue": 5
+                                }
+                            }
+                        ]
+                    },
+                    "source-interface": {
+                        "vipObjectType": "object",
+                        "vipType": "constant",
+                        "vipValue": "Gig1"
+                    },
+                    "vpn": {
+                        "vipObjectType": "object",
+                        "vipType": "constant",
+                        "vipValue": 10
+                    }
+                },
+                {
+                    "group-name": {
+                        "vipObjectType": "object",
+                        "vipType": "constant",
+                        "vipValue": "group2"
+                    },
+                    "server": {
+                        "vipObjectType": "tree",
+                        "vipPrimaryKey": [
+                            "address"
+                        ],
+                        "vipType": "constant",
+                        "vipValue": [
+                            {
+                                "acct-port": {
+                                    "vipObjectType": "object",
+                                    "vipType": "constant",
+                                    "vipValue": 1813
+                                },
+                                "address": {
+                                    "vipObjectType": "object",
+                                    "vipType": "constant",
+                                    "vipValue": "1.1.2.1"
+                                },
+                                "auth-port": {
+                                    "vipObjectType": "object",
+                                    "vipType": "constant",
+                                    "vipValue": 1812
+                                },
+                                "key": {
+                                    "vipObjectType": "object",
+                                    "vipType": "constant",
+                                    "vipValue": "test_key2"
+                                },
+                                "retransmit": {
+                                    "vipObjectType": "object",
+                                    "vipType": "constant",
+                                    "vipValue": 3
                                 },
                                 "secret-key": {
                                     "vipObjectType": "object",
                                     "vipType": "constant",
-                                    "vipValue": "secret_radius_key"
+                                    "vipValue": "secret_key2"
                                 },
                                 "timeout": {
                                     "vipObjectType": "object",
                                     "vipType": "constant",
-                                    "vipValue": 10
+                                    "vipValue": 5
                                 }
                             }
                         ]
                     },
                     "source-interface": {
                         "vipObjectType": "object",
                         "vipType": "constant",
-                        "vipValue": "FortyGigabitEthernet0/"
+                        "vipValue": "Gig2"
                     },
                     "vpn": {
                         "vipObjectType": "object",
                         "vipType": "constant",
-                        "vipValue": 4
+                        "vipValue": 11
                     }
                 }
             ]
         },
-        "radius-dynamic-author": {
-            "auth-type": {
-                "vipObjectType": "object",
-                "vipType": "constant",
-                "vipValue": "any"
-            },
-            "domain-stripping": {
-                "vipObjectType": "object",
-                "vipType": "constant",
-                "vipValue": "right-to-left"
-            },
-            "port": {
-                "vipObjectType": "object",
-                "vipType": "constant",
-                "vipValue": 1163
-            },
-            "radius-client": {
-                "vipObjectType": "tree",
-                "vipPrimaryKey": [
-                    "ip"
-                ],
-                "vipType": "constant",
-                "vipValue": [
-                    {
-                        "ip": {
-                            "vipObjectType": "object",
-                            "vipType": "constant",
-                            "vipValue": "10.1.1.1"
-                        },
-                        "vpn": {
-                            "vipObjectType": "tree",
-                            "vipPrimaryKey": [
-                                "name"
-                            ],
-                            "vipType": "constant",
-                            "vipValue": [
-                                {
-                                    "name": {
-                                        "vipObjectType": "object",
-                                        "vipType": "constant",
-                                        "vipValue": "radiuscoa_vpn_name"
-                                    },
-                                    "server-key": {
-                                        "vipObjectType": "object",
-                                        "vipType": "constant",
-                                        "vipValue": "secure_radius_server_key"
-                                    }
-                                }
-                            ]
-                        }
-                    }
-                ]
-            },
-            "rda-server-key": {
-                "vipObjectType": "object",
-                "vipType": "constant",
-                "vipValue": "secure_server_key_password"
-            }
-        },
-        "radius-trustsec": {
-            "cts-auth-list": {
-                "vipObjectType": "object",
-                "vipType": "constant",
-                "vipValue": "example_element"
-            },
-            "radius-trustsec-group": {
-                "vipObjectType": "object",
-                "vipType": "constant",
-                "vipValue": "radius-4"
-            }
-        },
         "server-auth-order": {
             "vipObjectType": "object",
             "vipType": "constant",
-            "vipValue": "local,radius-4,tacacs-5"
+            "vipValue": "local"
         },
         "tacacs": {
             "vipObjectType": "tree",
             "vipPrimaryKey": [
                 "group-name"
             ],
             "vipType": "constant",
             "vipValue": [
                 {
                     "group-name": {
                         "vipObjectType": "object",
                         "vipType": "constant",
-                        "vipValue": "tacacs-5"
+                        "vipValue": "group1"
                     },
                     "server": {
                         "vipObjectType": "tree",
                         "vipPrimaryKey": [
                             "address"
                         ],
                         "vipType": "constant",
                         "vipValue": [
                             {
                                 "address": {
                                     "vipObjectType": "object",
                                     "vipType": "constant",
-                                    "vipValue": "2.2.2.2"
+                                    "vipValue": "1.1.1.1"
                                 },
                                 "key": {
                                     "vipObjectType": "object",
                                     "vipType": "constant",
-                                    "vipValue": "tacacs_key"
+                                    "vipValue": "key"
                                 },
                                 "port": {
                                     "vipObjectType": "object",
                                     "vipType": "constant",
                                     "vipValue": 49
                                 },
                                 "secret-key": {
                                     "vipObjectType": "object",
                                     "vipType": "constant",
-                                    "vipValue": "secret_tacacs_key,"
+                                    "vipValue": "secret_key"
                                 },
                                 "timeout": {
                                     "vipObjectType": "object",
                                     "vipType": "constant",
                                     "vipValue": 5
                                 }
                             }
                         ]
                     },
                     "source-interface": {
                         "vipObjectType": "object",
                         "vipType": "constant",
-                        "vipValue": "GigabitEthernet0/0"
+                        "vipValue": "Gig0"
                     },
                     "vpn": {
                         "vipObjectType": "object",
                         "vipType": "constant",
-                        "vipValue": 5
+                        "vipValue": 0
                     }
                 }
             ]
         },
         "user": {
             "vipObjectType": "tree",
             "vipPrimaryKey": [
@@ -329,33 +211,71 @@
             ],
             "vipType": "constant",
             "vipValue": [
                 {
                     "name": {
                         "vipObjectType": "object",
                         "vipType": "constant",
-                        "vipValue": "example_user"
+                        "vipValue": "test1"
                     },
                     "password": {
                         "vipObjectType": "object",
                         "vipType": "constant",
-                        "vipValue": "secure_password"
+                        "vipValue": "*****"
+                    },
+                    "privilege": {
+                        "vipObjectType": "object",
+                        "vipType": "constant",
+                        "vipValue": "1"
+                    },
+                    "pubkey-chain": {
+                        "vipObjectType": "tree",
+                        "vipPrimaryKey": [
+                            "key-string"
+                        ],
+                        "vipType": "ignore",
+                        "vipValue": []
+                    },
+                    "secret": {
+                        "vipObjectType": "object",
+                        "vipType": "constant",
+                        "vipValue": "secret"
+                    }
+                },
+                {
+                    "name": {
+                        "vipObjectType": "object",
+                        "vipType": "constant",
+                        "vipValue": "test2"
+                    },
+                    "password": {
+                        "vipObjectType": "object",
+                        "vipType": "constant",
+                        "vipValue": "*****"
                     },
                     "privilege": {
                         "vipObjectType": "object",
                         "vipType": "constant",
                         "vipValue": "15"
                     },
+                    "pubkey-chain": {
+                        "vipObjectType": "tree",
+                        "vipPrimaryKey": [
+                            "key-string"
+                        ],
+                        "vipType": "ignore",
+                        "vipValue": []
+                    },
                     "secret": {
                         "vipObjectType": "object",
                         "vipType": "constant",
-                        "vipValue": "secure_secret"
+                        "vipValue": "secret"
                     }
                 }
             ]
         }
     },
-    "templateDescription": "cisco_aaa_complex",
+    "templateDescription": "na",
     "templateMinVersion": "15.0.0",
-    "templateName": "cisco_aaa_complex",
+    "templateName": "complex_aaa",
     "templateType": "cedge_aaa"
 }
```

### Comparing `catalystwan-0.33.6.post0/catalystwan/tests/templates/definitions/cisco_banner.json` & `catalystwan-0.33.7/catalystwan/tests/templates/definitions/banner_1.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/tests/templates/definitions/cisco_bfd.json` & `catalystwan-0.33.7/catalystwan/tests/templates/definitions/cisco_bfd.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/tests/templates/definitions/cisco_ntp_complex.json` & `catalystwan-0.33.7/catalystwan/tests/templates/definitions/default_cisco_system.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6428571428571429%*

 * *Differences: {"'deviceType'": "['vedge-C8000V']",*

 * * "'templateDefinition'": "{replace: OrderedDict([('clock', OrderedDict([('timezone', "*

 * *                         "OrderedDict([('vipObjectType', 'object'), ('vipType', 'ignore'), "*

 * *                         "('vipValue', 'UTC')]))])), ('gps-location', OrderedDict([('latitude', "*

 * *                         "OrderedDict([('vipObjectType', 'object'), ('vipType', 'ignore')])), "*

 * *                         "('longitude', OrderedDict([('vipObjectType', 'object'), ('vipType', "*

 * *      […]*

```diff
@@ -1,143 +1,184 @@
 {
-    "deviceType": [],
+    "deviceType": [
+        "vedge-C8000V"
+    ],
     "factoryDefault": false,
     "templateDefinition": {
-        "keys": {
-            "authentication": {
-                "vipObjectType": "tree",
-                "vipPrimaryKey": [
-                    "number"
-                ],
-                "vipType": "constant",
-                "vipValue": [
-                    {
-                        "md5": {
-                            "vipObjectType": "object",
-                            "vipType": "constant",
-                            "vipValue": "md5key1"
-                        },
-                        "number": {
-                            "vipObjectType": "object",
-                            "vipType": "constant",
-                            "vipValue": 1
-                        }
-                    },
-                    {
-                        "md5": {
-                            "vipObjectType": "object",
-                            "vipType": "constant",
-                            "vipValue": "md5key2"
-                        },
-                        "number": {
-                            "vipObjectType": "object",
-                            "vipType": "constant",
-                            "vipValue": 2
-                        }
-                    }
-                ]
+        "admin-tech-on-failure": {
+            "vipObjectType": "object",
+            "vipType": "ignore",
+            "vipValue": "true"
+        },
+        "affinity-group": {
+            "affinity-group-number": {
+                "vipObjectType": "object",
+                "vipType": "ignore"
             },
-            "trusted": {
+            "preference": {
                 "vipObjectType": "list",
-                "vipType": "constant",
-                "vipValue": [
-                    1,
-                    2
-                ]
+                "vipType": "ignore"
             }
         },
-        "master": {
-            "enable": {
+        "clock": {
+            "timezone": {
                 "vipObjectType": "object",
-                "vipType": "constant",
-                "vipValue": "true"
+                "vipType": "ignore",
+                "vipValue": "UTC"
+            }
+        },
+        "console-baud-rate": {
+            "vipObjectType": "object",
+            "vipType": "notIgnore",
+            "vipValue": "9600"
+        },
+        "control-session-pps": {
+            "vipObjectType": "object",
+            "vipType": "ignore",
+            "vipValue": 300
+        },
+        "controller-group-list": {
+            "vipObjectType": "list",
+            "vipType": "ignore"
+        },
+        "description": {
+            "vipObjectType": "object",
+            "vipType": "ignore"
+        },
+        "device-groups": {
+            "vipObjectType": "list",
+            "vipType": "ignore"
+        },
+        "enable-mrf-migration": {},
+        "gps-location": {
+            "geo-fencing": {
+                "enable": {
+                    "vipObjectType": "object",
+                    "vipType": "ignore",
+                    "vipValue": "false"
+                },
+                "range": {},
+                "sms": {
+                    "enable": {},
+                    "mobile-number": {
+                        "vipType": "ignore",
+                        "vipValue": []
+                    }
+                }
+            },
+            "latitude": {
+                "vipObjectType": "object",
+                "vipType": "ignore"
             },
-            "source": {
+            "longitude": {
+                "vipObjectType": "object",
+                "vipType": "ignore"
+            }
+        },
+        "host-name": {
+            "vipObjectType": "object",
+            "vipType": "variableName",
+            "vipValue": "",
+            "vipVariableName": "system_host_name"
+        },
+        "idle-timeout": {
+            "vipObjectType": "object",
+            "vipType": "ignore"
+        },
+        "location": {
+            "vipObjectType": "object",
+            "vipType": "ignore"
+        },
+        "max-omp-sessions": {
+            "vipObjectType": "object",
+            "vipType": "ignore"
+        },
+        "migration-bgp-community": {},
+        "multi-tenant": {
+            "vipObjectType": "node-only",
+            "vipType": "notIgnore",
+            "vipValue": "false"
+        },
+        "object-track": {
+            "vipObjectType": "tree",
+            "vipPrimaryKey": [
+                "object-number"
+            ],
+            "vipType": "ignore",
+            "vipValue": []
+        },
+        "on-demand": {
+            "enable": {
                 "vipObjectType": "object",
-                "vipType": "constant",
-                "vipValue": "Loopback0"
+                "vipType": "ignore",
+                "vipValue": "false"
             },
-            "stratum": {
+            "idle-timeout": {
                 "vipObjectType": "object",
-                "vipType": "constant",
-                "vipValue": 2
+                "vipType": "ignore",
+                "vipValue": 10
             }
         },
-        "server": {
+        "overlay-id": {
+            "vipObjectType": "object",
+            "vipType": "ignore",
+            "vipValue": 1
+        },
+        "port-hop": {
+            "vipObjectType": "object",
+            "vipType": "ignore",
+            "vipValue": "true"
+        },
+        "port-offset": {
+            "vipObjectType": "object",
+            "vipType": "ignore",
+            "vipValue": 0
+        },
+        "region-id": {},
+        "role": {},
+        "secondary-region": {},
+        "site-id": {
+            "vipObjectType": "object",
+            "vipType": "variableName",
+            "vipValue": "",
+            "vipVariableName": "system_site_id"
+        },
+        "system-ip": {
+            "vipObjectType": "object",
+            "vipType": "variableName",
+            "vipValue": "",
+            "vipVariableName": "system_system_ip"
+        },
+        "track-default-gateway": {
+            "vipObjectType": "object",
+            "vipType": "ignore",
+            "vipValue": "true"
+        },
+        "track-interface-tag": {
+            "vipObjectType": "object",
+            "vipType": "ignore"
+        },
+        "track-transport": {
+            "vipObjectType": "object",
+            "vipType": "ignore",
+            "vipValue": "true"
+        },
+        "tracker": {
             "vipObjectType": "tree",
             "vipPrimaryKey": [
                 "name"
             ],
-            "vipType": "constant",
-            "vipValue": [
-                {
-                    "key": {
-                        "vipObjectType": "object",
-                        "vipType": "constant",
-                        "vipValue": 1
-                    },
-                    "name": {
-                        "vipObjectType": "object",
-                        "vipType": "constant",
-                        "vipValue": "0.pool.ntp.org"
-                    },
-                    "prefer": {
-                        "vipObjectType": "object",
-                        "vipType": "constant",
-                        "vipValue": "true"
-                    },
-                    "source-interface": {
-                        "vipObjectType": "object",
-                        "vipType": "constant",
-                        "vipValue": "GigabitEthernet0/0"
-                    },
-                    "version": {
-                        "vipObjectType": "object",
-                        "vipType": "constant",
-                        "vipValue": 4
-                    },
-                    "vpn": {
-                        "vipObjectType": "object",
-                        "vipType": "constant",
-                        "vipValue": 10
-                    }
-                },
-                {
-                    "key": {
-                        "vipObjectType": "object",
-                        "vipType": "constant",
-                        "vipValue": 2
-                    },
-                    "name": {
-                        "vipObjectType": "object",
-                        "vipType": "constant",
-                        "vipValue": "1.pool.ntp.org"
-                    },
-                    "prefer": {
-                        "vipObjectType": "object",
-                        "vipType": "constant",
-                        "vipValue": "false"
-                    },
-                    "source-interface": {
-                        "vipObjectType": "object",
-                        "vipType": "constant",
-                        "vipValue": "GigabitEthernet0/1"
-                    },
-                    "version": {
-                        "vipObjectType": "object",
-                        "vipType": "constant",
-                        "vipValue": 4
-                    },
-                    "vpn": {
-                        "vipObjectType": "object",
-                        "vipType": "constant",
-                        "vipValue": 20
-                    }
-                }
-            ]
+            "vipType": "ignore",
+            "vipValue": []
+        },
+        "transport-gateway": {
+            "vipObjectType": "object",
+            "vipType": "ignore",
+            "vipValue": "false",
+            "vipVariableName": "system_transport_gateway"
         }
     },
-    "templateDescription": "cisco_ntp_complex",
+    "templateDescription": "default",
     "templateMinVersion": "15.0.0",
-    "templateName": "cisco_ntp_complex",
-    "templateType": "cisco_ntp"
+    "templateName": "default_cisco_system",
+    "templateType": "cisco_system"
 }
```

### Comparing `catalystwan-0.33.6.post0/catalystwan/tests/templates/definitions/cisco_vpn_complex.json` & `catalystwan-0.33.7/catalystwan/tests/templates/definitions/complex_cisco_vpn.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8571392154477351%*

 * *Differences: {"'templateDefinition'": "{'omp': {'advertise': {'vipValue': {0: {'prefix-list': {'vipValue': {0: "*

 * *                         "{'aggregate-only': {'vipValue': True}, delete: ['region']}}}}}}, "*

 * *                         "'ipv6-advertise': {'vipValue': {0: {'prefix-list': {'vipValue': {0: "*

 * *                         "{'aggregate-only': {'vipValue': False}, delete: ['region']}}}}, 1: "*

 * *                         "{'prefix-list': {'vipValue': {0: {'aggregate-only': {'vipValue': True}, "*

 * *                         "de […]*

```diff
@@ -508,15 +508,15 @@
                             "vipObjectType": "object",
                             "vipType": "constant",
                             "vipValue": "2.1.1.1"
                         },
                         "static-nat-direction": {
                             "vipObjectType": "object",
                             "vipType": "constant",
-                            "vipValue": "inside"
+                            "vipValue": "outside"
                         },
                         "translate-ip": {
                             "vipObjectType": "object",
                             "vipType": "constant",
                             "vipValue": "2.1.1.2"
                         }
                     }
@@ -596,35 +596,35 @@
                                 "vipObjectType": "object",
                                 "vipType": "constant",
                                 "vipValue": "10.10.10.10"
                             },
                             "leak_from_global": {
                                 "vipObjectType": "object",
                                 "vipType": "constant",
-                                "vipValue": "true"
+                                "vipValue": true
                             },
                             "leak_from_global_protocol": {
                                 "vipObjectType": "object",
                                 "vipType": "constant",
                                 "vipValue": "connected"
                             },
                             "leak_to_global": {
                                 "vipObjectType": "object",
                                 "vipType": "constant",
-                                "vipValue": "false"
+                                "vipValue": false
                             },
                             "name": {
                                 "vipObjectType": "object",
                                 "vipType": "constant",
                                 "vipValue": "pool"
                             },
                             "overload": {
                                 "vipObjectType": "node-only",
                                 "vipType": "constant",
-                                "vipValue": "false"
+                                "vipValue": false
                             },
                             "start-address": {
                                 "vipObjectType": "object",
                                 "vipType": "constant",
                                 "vipValue": "1.1.1.1"
                             }
                         }
@@ -648,25 +648,20 @@
                             ],
                             "vipType": "constant",
                             "vipValue": [
                                 {
                                     "aggregate-only": {
                                         "vipObjectType": "object",
                                         "vipType": "constant",
-                                        "vipValue": "true"
+                                        "vipValue": true
                                     },
                                     "prefix-entry": {
                                         "vipObjectType": "object",
                                         "vipType": "constant",
                                         "vipValue": "prefix_entry"
-                                    },
-                                    "region": {
-                                        "vipObjectType": "object",
-                                        "vipType": "constant",
-                                        "vipValue": "access"
                                     }
                                 }
                             ]
                         },
                         "protocol": {
                             "vipObjectType": "object",
                             "vipType": "constant",
@@ -702,25 +697,20 @@
                             ],
                             "vipType": "constant",
                             "vipValue": [
                                 {
                                     "aggregate-only": {
                                         "vipObjectType": "object",
                                         "vipType": "constant",
-                                        "vipValue": "false"
+                                        "vipValue": false
                                     },
                                     "prefix-entry": {
                                         "vipObjectType": "object",
                                         "vipType": "constant",
                                         "vipValue": "prefix_entryv6"
-                                    },
-                                    "region": {
-                                        "vipObjectType": "object",
-                                        "vipType": "constant",
-                                        "vipValue": "core"
                                     }
                                 }
                             ]
                         },
                         "protocol": {
                             "vipObjectType": "object",
                             "vipType": "constant",
@@ -747,25 +737,20 @@
                             ],
                             "vipType": "constant",
                             "vipValue": [
                                 {
                                     "aggregate-only": {
                                         "vipObjectType": "object",
                                         "vipType": "constant",
-                                        "vipValue": "true"
+                                        "vipValue": true
                                     },
                                     "prefix-entry": {
                                         "vipObjectType": "object",
                                         "vipType": "constant",
                                         "vipValue": "prefix_entryv6-connected"
-                                    },
-                                    "region": {
-                                        "vipObjectType": "object",
-                                        "vipType": "constant",
-                                        "vipValue": "access"
                                     }
                                 }
                             ]
                         },
                         "protocol": {
                             "vipObjectType": "object",
                             "vipType": "constant",
@@ -1070,12 +1055,12 @@
         },
         "vpn-id": {
             "vipObjectType": "object",
             "vipType": "constant",
             "vipValue": 0
         }
     },
-    "templateDescription": "cisco_vpn_complex",
+    "templateDescription": "NA",
     "templateMinVersion": "15.0.0",
-    "templateName": "cisco_vpn_complex",
+    "templateName": "test_vpn_new",
     "templateType": "cisco_vpn"
 }
```

### Comparing `catalystwan-0.33.6.post0/catalystwan/tests/templates/definitions/omp_vsmart_1.json` & `catalystwan-0.33.7/catalystwan/tests/templates/definitions/omp_2.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7857142857142857%*

 * *Differences: {"'templateDefinition'": "{replace: OrderedDict([('graceful-restart', "*

 * *                         "OrderedDict([('vipObjectType', 'object'), ('vipType', 'constant'), "*

 * *                         "('vipValue', 'false')])), ('send-backup-paths', "*

 * *                         "OrderedDict([('vipObjectType', 'object'), ('vipType', 'constant'), "*

 * *                         "('vipValue', 'false')])), ('shutdown', OrderedDict([('vipObjectType', "*

 * *                         "'object'), ('vipType', 'constant'), ('vipValue', ' […]*

```diff
@@ -1,26 +1,34 @@
 {
     "deviceType": [
         "vedge-C8000V"
     ],
     "factoryDefault": false,
     "templateDefinition": {
-        "filter-route": {
-            "outbound": {
-                "affinity-group-preference": {
-                    "vipObjectType": "object",
-                    "vipType": "constant",
-                    "vipValue": "false"
-                },
-                "tloc-color": {
-                    "vipObjectType": "object",
-                    "vipType": "constant",
-                    "vipValue": "false"
-                }
+        "graceful-restart": {
+            "vipObjectType": "object",
+            "vipType": "constant",
+            "vipValue": "false"
+        },
+        "send-backup-paths": {
+            "vipObjectType": "object",
+            "vipType": "constant",
+            "vipValue": "false"
+        },
+        "shutdown": {
+            "vipObjectType": "object",
+            "vipType": "constant",
+            "vipValue": "true"
+        },
+        "timers": {
+            "holdtime": {
+                "vipObjectType": "object",
+                "vipType": "constant",
+                "vipValue": 30
             }
         }
     },
-    "templateDescription": "default",
+    "templateDescription": "some changes",
     "templateMinVersion": "15.0.0",
-    "templateName": "omp_vsmart_1",
+    "templateName": "omp_2",
     "templateType": "omp-vsmart"
 }
```

### Comparing `catalystwan-0.33.6.post0/catalystwan/tests/templates/definitions/omp_vsmart_2.json` & `catalystwan-0.33.7/catalystwan/tests/templates/definitions/omp_3.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8214285714285714%*

 * *Differences: {"'templateDefinition'": "{'send-backup-paths': {'vipValue': 'true'}, 'shutdown': {'vipValue': "*

 * *                         "'false'}, 'timers': {'advertisement-interval': "*

 * *                         "OrderedDict([('vipObjectType', 'object'), ('vipType', 'constant'), "*

 * *                         "('vipValue', 3)]), 'graceful-restart-timer': OrderedDict([('vipValue', "*

 * *                         "''), ('vipType', 'variableName'), ('vipObjectType', 'object'), "*

 * *                         "('vipVariableName', 'omp_grac […]*

```diff
@@ -1,48 +1,57 @@
 {
     "deviceType": [
         "vedge-C8000V"
     ],
     "factoryDefault": false,
     "templateDefinition": {
-        "filter-route": {
-            "outbound": {
-                "affinity-group-preference": {
-                    "vipObjectType": "object",
-                    "vipType": "constant",
-                    "vipValue": "false"
-                },
-                "tloc-color": {
-                    "vipObjectType": "object",
-                    "vipType": "constant",
-                    "vipValue": "false"
-                }
-            }
+        "discard-rejected": {
+            "vipObjectType": "object",
+            "vipType": "variableName",
+            "vipValue": "",
+            "vipVariableName": "omp_discard_rejected_custom"
         },
         "graceful-restart": {
             "vipObjectType": "object",
             "vipType": "constant",
             "vipValue": "false"
         },
         "send-backup-paths": {
             "vipObjectType": "object",
             "vipType": "constant",
-            "vipValue": "false"
+            "vipValue": "true"
+        },
+        "send-path-limit": {
+            "vipObjectType": "object",
+            "vipType": "variableName",
+            "vipValue": "",
+            "vipVariableName": "omp_send_path_limit"
         },
         "shutdown": {
             "vipObjectType": "object",
             "vipType": "constant",
-            "vipValue": "true"
+            "vipValue": "false"
         },
         "timers": {
+            "advertisement-interval": {
+                "vipObjectType": "object",
+                "vipType": "constant",
+                "vipValue": 3
+            },
+            "graceful-restart-timer": {
+                "vipObjectType": "object",
+                "vipType": "variableName",
+                "vipValue": "",
+                "vipVariableName": "omp_graceful_restart_timer"
+            },
             "holdtime": {
                 "vipObjectType": "object",
                 "vipType": "constant",
                 "vipValue": 30
             }
         }
     },
-    "templateDescription": "some changes",
+    "templateDescription": "advanced",
     "templateMinVersion": "15.0.0",
-    "templateName": "omp_vsmart_2",
+    "templateName": "omp_3",
     "templateType": "omp-vsmart"
 }
```

### Comparing `catalystwan-0.33.6.post0/catalystwan/tests/templates/models/cisco_bfd.py` & `catalystwan-0.33.7/catalystwan/tests/templates/models/cisco_bfd.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
-from catalystwan.api.templates.models.cisco_bfd_model import CiscoBFDModel, Color
+from catalystwan.api.templates.models.cisco_bfd_model import CiscoBFDModel, Color, ColorType
 
-cisco_bfd = CiscoBFDModel(  # type: ignore
+bfd_model = CiscoBFDModel(  # type: ignore
     template_name="cisco_bfd",
     template_description="na",
     multiplier=100,
     poll_interval=50,
     default_dscp=50,
     color=[
-        Color(color="biz-internet", hello_interval=50, multipler=100, pmtu_discovery=False, dscp=100),  # type: ignore
-        Color(color="silver", hello_interval=150, multipler=10, dscp=20),  # type: ignore
+        Color(  # type: ignore
+            color=ColorType.BIZ_INTERNET, hello_interval=50, multipler=100, pmtu_discovery=False, dscp=100
+        ),
+        Color(color=ColorType.SILVER, hello_interval=150, multipler=10, dscp=20),  # type: ignore
     ],
 )
```

### Comparing `catalystwan-0.33.6.post0/catalystwan/tests/templates/models/cisco_vpn.py` & `catalystwan-0.33.7/catalystwan/tests/templates/models/cisco_vpn.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,72 +1,95 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # type: ignore
 
 from catalystwan.api.templates.models.cisco_vpn_model import (
     Advertise,
+    AdvertiseProtocol,
+    AdvertiseProtocolSubType,
     CiscoVPNModel,
+    Direction,
     Dns,
     DnsIpv6,
     GreRoute,
     Host,
     IpsecRoute,
     Ipv6Advertise,
+    Ipv6AdvertiseProtocol,
+    Ipv6AdvertiseProtocolSubType,
+    LeakFromGlobalProtocol,
+    Nat,
     Natpool,
     NextHop,
     NextHopv6,
+    Overload,
     Pool,
     PortForward,
     PrefixList,
+    Proto,
+    Region,
+    Role,
     RouteExport,
+    RouteExportProtocol,
+    RouteExportProtocolSubType,
     RouteExportRedistribute,
+    RouteExportRedistributeProtocol,
     RouteImport,
     RouteImportFrom,
+    RouteImportFromProtocol,
+    RouteImportFromProtocolSubType,
     RouteImportFromRedistribute,
+    RouteImportFromRedistributeProtocol,
+    RouteImportProtocol,
+    RouteImportProtocolSubType,
     RouteImportRedistribute,
+    RouteImportRedistributeProtocol,
     Routev4,
     Routev6,
     Service,
     ServiceRoute,
     Static,
+    StaticNatDirection,
     SubnetStatic,
+    SvcType,
 )
+from catalystwan.utils.device_model import DeviceModel
 
-cisco_vpn_basic = CiscoVPNModel(
-    template_name="cisco_vpn_basic", template_description="Primitive", device_models=["vedge-C8000V"]
+basic_cisco_vpn = CiscoVPNModel(
+    template_name="Basic_Cisco_VPN_Model", template_description="Primitive", device_models=[DeviceModel.VEDGE_C8000V]
 )  # type: ignore
 
 
-cisco_vpn_complex = CiscoVPNModel(
-    template_name="cisco_vpn_complex",
-    template_description="cisco_vpn_complex",
-    device_models=["vedge-cloud"],
+complex_vpn_model = CiscoVPNModel(
+    template_name="complex_cisco_vpn",
+    template_description="NA",
+    device_models=[DeviceModel.VEDGE],
     vpn_name="test_vpn_name",
     omp_admin_distance_ipv4=10,
     omp_admin_distance_ipv6=100,
     route_v4=[Routev4(prefix="prefixv4", next_hop=[NextHop(address="1.1.1.1")])],
-    route_v6=[Routev6(prefix="prefixv6", next_hop=[NextHopv6(address="2.2.2.2")], nat="NAT64")],
-    dns=[Dns(dns_addr="1.1.1.1"), Dns(dns_addr="2.2.2.2", role="secondary")],
+    route_v6=[Routev6(prefix="prefixv6", next_hop=[NextHopv6(address="2.2.2.2")], nat=Nat.NAT64)],
+    dns=[Dns(dns_addr="1.1.1.1"), Dns(dns_addr="2.2.2.2", role=Role.SECONDARY)],
     dns_ipv6=[DnsIpv6(dns_addr="30a8:b25e:3db5:fe9f:231f:7478:4181:9234")],
     host=[Host(hostname="test_hostname", ip=["1.1.1.1"])],
     service=[
         Service(
-            svc_type="appqoe",
+            svc_type=SvcType.APPQOE,
             address=["1.1.1.1"],
             interface="Gig0/0/1",
             track_enable=False,
         ),
         Service(
-            svc_type="FW",
+            svc_type=SvcType.FW,
             address=["1.1.122.1", "2.2.2.2"],
             interface="Gig0/0/2",
             track_enable=True,
         ),
         Service(
-            svc_type="IDP",
+            svc_type=SvcType.IDP,
             address=["1.1.122.2", "3.2.2.2"],
             interface="Gig0/0/3",
             track_enable=False,
         ),
     ],
     service_route=[
         ServiceRoute(prefix="service_route", vpn=1),
@@ -78,163 +101,170 @@
     ],
     ipsec_route=[
         IpsecRoute(prefix="ipsec-prefix", vpn=10, interface=["ge0/0", "Gig0/0/1"]),
         IpsecRoute(prefix="prefix-2", vpn=100),
     ],
     advertise=[
         Advertise(
-            protocol="aggregate",
+            protocol=AdvertiseProtocol.AGGREGATE,
             route_policy="route-policy",
-            protocol_sub_type=["external"],
+            protocol_sub_type=[AdvertiseProtocolSubType.EXTERNAL],
             prefix_list=[
                 PrefixList(
                     prefix_entry="prefix_entry",
                     aggregate_only=True,
-                    region="access",
+                    region=Region.ACCESS,
                 )
             ],
         )
     ],
     ipv6_advertise=[
         Ipv6Advertise(
-            protocol="aggregate",
+            protocol=Ipv6AdvertiseProtocol.AGGREGATE,
             route_policy="route-policyv6",
-            protocol_sub_type=["external"],
+            protocol_sub_type=[Ipv6AdvertiseProtocolSubType.EXTERNAL],
             prefix_list=[
                 PrefixList(
                     prefix_entry="prefix_entryv6",
                     aggregate_only=False,
-                    region="core",
+                    region=Region.CORE,
                 )
             ],
         ),
         Ipv6Advertise(
-            protocol="connected",
+            protocol=Ipv6AdvertiseProtocol.CONNECTED,
             route_policy="route-policyv6-connected",
-            protocol_sub_type=["external"],
+            protocol_sub_type=[Ipv6AdvertiseProtocolSubType.EXTERNAL],
             prefix_list=[
                 PrefixList(
                     prefix_entry="prefix_entryv6-connected",
                     aggregate_only=True,
-                    region="access",
+                    region=Region.ACCESS,
                 )
             ],
         ),
     ],
     pool=[
         Pool(
             name="pool",
             start_address="1.1.1.1",
             end_address="10.10.10.10",
             overload=False,
             leak_from_global=True,
-            leak_from_global_protocol="connected",
+            leak_from_global_protocol=LeakFromGlobalProtocol.CONNECTED,
             leak_to_global=False,
         )
     ],
     natpool=[
         Natpool(
             name=1,
             prefix_length=24,
             range_start="10",
             range_end="100",
-            overload="false",
-            direction="inside",
+            overload=Overload.FALSE,
+            direction=Direction.INSIDE,
             tracker_id=10,
         ),
-        Natpool(name=2, prefix_length=24, range_start="10", range_end="100", overload="true", direction="outside"),
+        Natpool(
+            name=2,
+            prefix_length=24,
+            range_start="10",
+            range_end="100",
+            overload=Overload.TRUE,
+            direction=Direction.OUTSIDE,
+        ),
     ],
     static=[
         Static(
             pool_name=1,
             source_ip="1.1.1.1",
             translate_ip="1.1.1.2",
-            static_nat_direction="inside",
+            static_nat_direction=StaticNatDirection.INSIDE,
             tracker_id=1,
         ),
         Static(
             pool_name=2,
             source_ip="2.1.1.1",
             translate_ip="2.1.1.2",
-            static_nat_direction="inside",
+            static_nat_direction=StaticNatDirection.OUTSIDE,
         ),
     ],
     subnet_static=[
         SubnetStatic(
             source_ip_subnet="1.1.1.1",
             translate_ip_subnet="2.2.2.2",
             prefix_length=24,
-            static_nat_direction="outside",
+            static_nat_direction=StaticNatDirection.OUTSIDE,
         ),
         SubnetStatic(
             source_ip_subnet="1.1.2.1",
             translate_ip_subnet="2.3.2.2",
             prefix_length=24,
-            static_nat_direction="inside",
+            static_nat_direction=StaticNatDirection.INSIDE,
             tracker_id=10,
         ),
     ],
     port_forward=[
         PortForward(
             pool_name=1,
             source_port=1000,
             translate_port=2000,
             source_ip="1.1.1.1",
             translate_ip="2.2.2.2",
-            proto="tcp",
+            proto=Proto.TCP,
         ),
         PortForward(
             pool_name=2,
             source_port=1000,
             translate_port=2000,
             source_ip="1.1.4.1",
             translate_ip="2.2.3.2",
-            proto="udp",
+            proto=Proto.UDP,
         ),
     ],
     route_import=[
         RouteImport(
-            protocol="bgp",
-            protocol_sub_type=["external"],
+            protocol=RouteImportProtocol.BGP,
+            protocol_sub_type=[RouteImportProtocolSubType.EXTERNAL],
             route_policy="test_route_policy",
             redistribute=[
                 RouteImportRedistribute(
-                    protocol="eigrp",
+                    protocol=RouteImportRedistributeProtocol.EIGRP,
                     route_policy="test_route_policy",
                 )
             ],
         )
     ],
     route_import_from=[
         RouteImportFrom(
             source_vpn=1,
-            protocol="connected",
-            protocol_sub_type=["external"],
+            protocol=RouteImportFromProtocol.CONNECTED,
+            protocol_sub_type=[RouteImportFromProtocolSubType.EXTERNAL],
             route_policy="test_route_policy",
-            redistribute=[RouteImportFromRedistribute(protocol="bgp")],
+            redistribute=[RouteImportFromRedistribute(protocol=RouteImportFromRedistributeProtocol.BGP)],
         ),
         RouteImportFrom(
             source_vpn=100,
-            protocol="bgp",
-            protocol_sub_type=["external"],
+            protocol=RouteImportFromProtocol.BGP,
+            protocol_sub_type=[RouteImportFromProtocolSubType.EXTERNAL],
             route_policy="test_route_policy",
             redistribute=[
                 RouteImportFromRedistribute(
-                    protocol="eigrp",
+                    protocol=RouteImportFromRedistributeProtocol.EIGRP,
                     route_policy="test_route_policy",
                 )
             ],
         ),
     ],
     route_export=[
         RouteExport(
-            protocol="static",
-            protocol_sub_type=["external"],
+            protocol=RouteExportProtocol.STATIC,
+            protocol_sub_type=[RouteExportProtocolSubType.EXTERNAL],
             redistribute=[
                 RouteExportRedistribute(
-                    protocol="ospf",
+                    protocol=RouteExportRedistributeProtocol.OSPF,
                     route_policy="test_route_policy",
                 )
             ],
         )
     ],
 )
```

### Comparing `catalystwan-0.33.6.post0/catalystwan/tests/templates/schemas/basic/alias.json` & `catalystwan-0.33.7/catalystwan/tests/templates/schemas/basic/alias.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/tests/templates/schemas/basic/basic.json` & `catalystwan-0.33.7/catalystwan/tests/templates/schemas/basic/basic.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/tests/templates/schemas/basic/children.json` & `catalystwan-0.33.7/catalystwan/tests/templates/schemas/basic/children.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/tests/templates/schemas/basic/children_nested.json` & `catalystwan-0.33.7/catalystwan/tests/templates/schemas/basic/children_nested.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/tests/templates/schemas/basic/children_nested_datapath.json` & `catalystwan-0.33.7/catalystwan/tests/templates/schemas/basic/children_nested_datapath.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/tests/templates/schemas/basic/data_path.json` & `catalystwan-0.33.7/catalystwan/tests/templates/schemas/basic/data_path.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/tests/templates/schemas/cedge_aaa.json` & `catalystwan-0.33.7/catalystwan/tests/templates/schemas/cedge_aaa.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'nameSpace'": "'http: //viptela.com/cedge_aaa'"}*

```diff
@@ -1175,11 +1175,11 @@
             ],
             "primaryKeys": [
                 "rule-id"
             ]
         }
     ],
     "name": "cedge_aaa",
-    "nameSpace": "http://viptela.com/cedge_aaa",
+    "nameSpace": "http: //viptela.com/cedge_aaa",
     "xmlPath": [],
     "xmlRootTag": "aaa"
 }
```

### Comparing `catalystwan-0.33.6.post0/catalystwan/tests/templates/schemas/cisco_banner.json` & `catalystwan-0.33.7/catalystwan/tests/templates/schemas/cisco_banner.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/tests/templates/schemas/cisco_bfd.json` & `catalystwan-0.33.7/catalystwan/tests/templates/schemas/cisco_bfd.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/tests/templates/schemas/cisco_ntp.json` & `catalystwan-0.33.7/catalystwan/tests/templates/schemas/omp-vsmart.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5372135416666667%*

 * *Differences: {"'fields'": "{0: {'key': 'graceful-restart', 'description': 'Graceful Restart for OMP', "*

 * *             "'details': 'Enable or disable OMP graceful restart', 'optionType': {insert: [(1, "*

 * *             "'variable')]}, 'objectType': 'object', 'dataType': OrderedDict([('type', 'boolean'), "*

 * *             "('default', 'true')]), delete: ['primaryKeys', 'children']}, 1: {'key': "*

 * *             "'send-path-limit', 'description': 'Number of Paths Advertised per Prefix', "*

 * *             "'details': 'Set number of equa […]*

```diff
@@ -1,265 +1,202 @@
 {
     "fields": [
         {
-            "children": [
-                {
-                    "dataPath": [],
-                    "dataType": {
-                        "type": "string"
-                    },
-                    "defaultOption": "constant",
-                    "description": "Hostname/IP Address",
-                    "details": "Set hostname or IP address of server",
-                    "key": "name",
-                    "objectType": "object",
-                    "optionType": [
-                        "constant",
-                        "variable"
-                    ]
-                },
-                {
-                    "dataPath": [],
-                    "dataType": {
-                        "max": 4294967295,
-                        "min": 1,
-                        "type": "number"
-                    },
-                    "defaultOption": "ignore",
-                    "description": "Authentication Key ID",
-                    "details": "Set authentication key for the server",
-                    "key": "key",
-                    "objectType": "object",
-                    "optionType": [
-                        "constant",
-                        "variable",
-                        "ignore"
-                    ]
-                },
-                {
-                    "dataPath": [],
-                    "dataType": {
-                        "default": 0,
-                        "max": 65530,
-                        "min": 0,
-                        "type": "number"
-                    },
-                    "defaultOption": "ignore",
-                    "description": "VPN ID",
-                    "details": "Set VPN in which NTP server is located",
-                    "key": "vpn",
-                    "objectType": "object",
-                    "optionType": [
-                        "constant",
-                        "variable",
-                        "ignore"
-                    ]
-                },
-                {
-                    "dataPath": [],
-                    "dataType": {
-                        "default": 4,
-                        "max": 4,
-                        "min": 1,
-                        "type": "number"
-                    },
-                    "defaultOption": "ignore",
-                    "description": "Version",
-                    "details": "Set NTP version",
-                    "key": "version",
-                    "objectType": "object",
-                    "optionType": [
-                        "constant",
-                        "variable",
-                        "ignore"
-                    ]
-                },
-                {
-                    "dataPath": [],
-                    "dataType": {
-                        "maxLength": 32,
-                        "minLength": 0,
-                        "type": "string"
-                    },
-                    "defaultOption": "ignore",
-                    "description": "Source Interface",
-                    "details": "Set interface to use to reach NTP server",
-                    "key": "source-interface",
-                    "objectType": "object",
-                    "optionType": [
-                        "constant",
-                        "variable",
-                        "ignore"
-                    ]
-                },
-                {
-                    "dataPath": [],
-                    "dataType": {
-                        "default": "false",
-                        "type": "boolean"
-                    },
-                    "defaultOption": "ignore",
-                    "description": "Prefer",
-                    "details": "Prefer this NTP server",
-                    "key": "prefer",
-                    "objectType": "object",
-                    "optionType": [
-                        "constant",
-                        "variable",
-                        "ignore"
-                    ]
-                }
-            ],
             "dataPath": [],
+            "dataType": {
+                "default": "true",
+                "type": "boolean"
+            },
             "defaultOption": "ignore",
-            "description": "NTP Server (up to 4)",
-            "details": "Configure NTP servers",
-            "key": "server",
-            "objectType": "tree",
+            "description": "Graceful Restart for OMP",
+            "details": "Enable or disable OMP graceful restart",
+            "key": "graceful-restart",
+            "objectType": "object",
             "optionType": [
                 "constant",
+                "variable",
+                "ignore"
+            ]
+        },
+        {
+            "dataPath": [],
+            "dataType": {
+                "default": 4,
+                "max": 32,
+                "min": 1,
+                "type": "number"
+            },
+            "defaultOption": "ignore",
+            "description": "Number of Paths Advertised per Prefix",
+            "details": "Set number of equal-cost routes advertised by vSmart to vEdge",
+            "key": "send-path-limit",
+            "objectType": "object",
+            "optionType": [
+                "constant",
+                "variable",
+                "ignore"
+            ]
+        },
+        {
+            "dataPath": [],
+            "dataType": {
+                "default": "false",
+                "type": "boolean"
+            },
+            "defaultOption": "ignore",
+            "description": "Send Backup Paths",
+            "details": "Enable or disable advertisement of backup routes to vEdges",
+            "key": "send-backup-paths",
+            "objectType": "object",
+            "optionType": [
+                "constant",
+                "variable",
+                "ignore"
+            ]
+        },
+        {
+            "dataPath": [],
+            "dataType": {
+                "default": "false",
+                "type": "boolean"
+            },
+            "defaultOption": "ignore",
+            "description": "Discard Rejected Routes",
+            "details": "Enable or disable discarding of routes rejected by policy",
+            "key": "discard-rejected",
+            "objectType": "object",
+            "optionType": [
+                "constant",
+                "variable",
                 "ignore"
-            ],
-            "primaryKeys": [
-                "name"
             ]
         },
         {
-            "children": [
-                {
-                    "dataPath": [],
-                    "dataType": {
-                        "max": 4294967295,
-                        "min": 1,
-                        "type": "number"
-                    },
-                    "defaultOption": "constant",
-                    "description": "Authentication Key ID",
-                    "details": "MD5 authentication key ID",
-                    "key": "number",
-                    "objectType": "object",
-                    "optionType": [
-                        "constant",
-                        "variable"
-                    ]
+            "dataPath": [],
+            "dataType": {
+                "default": "false",
+                "label": {
+                    "off": "No",
+                    "on": "Yes"
                 },
-                {
-                    "dataPath": [],
-                    "dataType": {
-                        "maxLength": 32,
-                        "minLength": 1,
-                        "type": "passphrase"
-                    },
-                    "defaultOption": "constant",
-                    "description": "Authentication Value",
-                    "details": "Enter cleartext or AES-encrypted MD5 authentication key",
-                    "key": "md5",
-                    "objectType": "object",
-                    "optionType": [
-                        "constant",
-                        "variable"
-                    ]
-                }
-            ],
+                "type": "boolean"
+            },
+            "defaultOption": "ignore",
+            "description": "Shutdown",
+            "details": "Enable or disable OMP",
+            "key": "shutdown",
+            "objectType": "object",
+            "optionType": [
+                "constant",
+                "variable",
+                "ignore"
+            ]
+        },
+        {
             "dataPath": [
-                "keys"
+                "timers"
             ],
+            "dataType": {
+                "default": 1,
+                "max": 65535,
+                "min": 0,
+                "type": "number"
+            },
             "defaultOption": "ignore",
-            "description": "Authentication",
-            "details": "Set MD5 authentication key",
-            "key": "authentication",
-            "objectType": "tree",
+            "description": "Advertisement Interval (seconds)",
+            "details": "Set the time between OMP Update packets",
+            "key": "advertisement-interval",
+            "objectType": "object",
             "optionType": [
                 "constant",
+                "variable",
                 "ignore"
-            ],
-            "primaryKeys": [
-                "number"
             ]
         },
         {
             "dataPath": [
-                "keys"
+                "timers"
             ],
             "dataType": {
-                "max": 65535,
+                "default": 43200,
+                "max": 604800,
                 "min": 1,
                 "type": "number"
             },
             "defaultOption": "ignore",
-            "description": "Trusted Keys",
-            "details": "Designate authentication key as trustworthy",
-            "key": "trusted",
-            "objectType": "list",
+            "description": "Graceful Restart Timer (seconds)",
+            "details": "Set the OMP graceful restart timer",
+            "key": "graceful-restart-timer",
+            "objectType": "object",
             "optionType": [
                 "constant",
                 "variable",
                 "ignore"
             ]
         },
         {
             "dataPath": [
-                "master"
+                "timers"
             ],
             "dataType": {
-                "default": "false",
-                "type": "boolean"
+                "default": 300,
+                "max": 3600,
+                "min": 1,
+                "type": "number"
             },
             "defaultOption": "ignore",
-            "description": "Master",
-            "details": "Configure device as NTP master",
-            "key": "enable",
+            "description": "EOR Timer",
+            "details": "End of RIB timer <1..604800> seconds",
+            "key": "eor-timer",
             "objectType": "object",
             "optionType": [
                 "constant",
                 "variable",
                 "ignore"
             ]
         },
         {
             "dataPath": [
-                "master"
+                "timers"
             ],
             "dataType": {
-                "max": 15,
-                "min": 1,
+                "default": 60,
+                "range": "0,3-65535",
                 "type": "number"
             },
             "defaultOption": "ignore",
-            "description": "Stratum",
-            "details": "Master Stratum <1..15>",
-            "key": "stratum",
+            "description": "Hold Time (seconds)",
+            "details": "Set how long to wait before closing OMP peer connection",
+            "key": "holdtime",
             "objectType": "object",
             "optionType": [
                 "constant",
                 "variable",
                 "ignore"
             ]
         },
         {
             "dataPath": [
-                "master"
+                "filter-route",
+                "outbound"
             ],
             "dataType": {
-                "maxLength": 32,
-                "minLength": 0,
-                "type": "string"
+                "default": "false",
+                "type": "boolean"
             },
             "defaultOption": "ignore",
-            "description": "Source",
-            "details": "Set interface for NTP Master",
-            "key": "source",
+            "description": "Enable Filtering Route Updates Based on Affinity",
+            "details": "Filter routes based on affinity preference list",
+            "key": "affinity-group-preference",
             "objectType": "object",
             "optionType": [
                 "constant",
                 "variable",
                 "ignore"
             ]
         }
     ],
-    "name": "cisco_ntp",
-    "nameSpace": "http://viptela.com/system",
-    "xmlPath": [
-        "system"
-    ],
-    "xmlRootTag": "ntp"
+    "name": "OMP",
+    "nameSpace": "http://viptela.com/omp",
+    "xmlPath": [],
+    "xmlRootTag": "omp"
 }
```

### Comparing `catalystwan-0.33.6.post0/catalystwan/tests/templates/schemas/cisco_secure_internet_gateway.json` & `catalystwan-0.33.7/catalystwan/tests/templates/schemas/cisco_vpn.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8470889475746531%*

 * *Differences: {"'fields'": "{1: {'key': 'name', 'description': 'Name', 'details': 'Name', 'optionType': {insert: "*

 * *             "[(2, 'ignore')], delete: [0]}, 'dataType': {'minLength': 1, 'maxLength': 32, delete: "*

 * *             "['default']}}, 7: {'key': 'dns-ipv6', 'description': 'DNS', 'details': 'DNS', "*

 * *             "'optionType': {insert: [(2, 'ignore')]}, 'defaultOption': 'ignore', 'primaryKeys': "*

 * *             "['dns-addr'], 'children': {0: {'key': 'dns-addr', 'description': 'DNS Address', "*

 * *             "'detail […]*

```diff
@@ -16,1505 +16,2437 @@
             "optionType": [
                 "constant"
             ]
         },
         {
             "dataPath": [],
             "dataType": {
-                "default": "",
+                "maxLength": 32,
+                "minLength": 1,
                 "type": "string"
             },
             "defaultOption": "ignore",
-            "description": "Child Organization Id",
-            "details": "Child Organization Id",
-            "key": "childOrgId",
+            "description": "Name",
+            "details": "Name",
+            "key": "name",
             "objectType": "object",
             "optionType": [
-                "ignore",
                 "constant",
-                "variable"
+                "variable",
+                "ignore"
+            ]
+        },
+        {
+            "dataPath": [],
+            "dataType": {
+                "default": 0,
+                "max": 65527,
+                "min": 0,
+                "type": "number"
+            },
+            "defaultOption": "constant",
+            "description": "Tenant VPN",
+            "details": "Tenant VPN",
+            "key": "tenant-vpn-id",
+            "objectType": "object",
+            "optionType": [
+                "constant"
+            ]
+        },
+        {
+            "dataPath": [],
+            "dataType": {
+                "type": "string"
+            },
+            "defaultOption": "constant",
+            "description": "Select Tenant",
+            "details": "Org Name selected",
+            "key": "org-name",
+            "objectType": "object",
+            "optionType": [
+                "constant"
+            ]
+        },
+        {
+            "dataPath": [],
+            "dataType": {
+                "max": 255,
+                "min": 1,
+                "type": "number"
+            },
+            "defaultOption": "ignore",
+            "description": "OMP Admin Distance IPv4",
+            "details": "omp-admin-distance-ipv4",
+            "key": "omp-admin-distance-ipv4",
+            "objectType": "object",
+            "optionType": [
+                "constant",
+                "variable",
+                "ignore"
+            ]
+        },
+        {
+            "dataPath": [],
+            "dataType": {
+                "max": 255,
+                "min": 1,
+                "type": "number"
+            },
+            "defaultOption": "ignore",
+            "description": "OMP Admin Distance IPv6",
+            "details": "omp-admin-distance-ipv6",
+            "key": "omp-admin-distance-ipv6",
+            "objectType": "object",
+            "optionType": [
+                "constant",
+                "variable",
+                "ignore"
             ]
         },
         {
             "children": [
                 {
                     "dataPath": [],
                     "dataType": {
-                        "max": 255,
-                        "maxLength": 8,
-                        "min": 1,
-                        "minLength": 4,
-                        "type": "string"
+                        "type": "ip"
                     },
                     "defaultOption": "constant",
-                    "description": "Interface Name (1..255)",
-                    "details": "Interface name: IPsec when present",
-                    "key": "if-name",
+                    "description": "DNS Address",
+                    "details": "DNS Address",
+                    "key": "dns-addr",
                     "objectType": "object",
                     "optionType": [
                         "constant"
                     ]
                 },
                 {
                     "dataPath": [],
                     "dataType": {
-                        "default": "false",
-                        "type": "boolean"
+                        "default": "primary",
+                        "type": "enum",
+                        "values": [
+                            {
+                                "key": "primary",
+                                "value": "Primary"
+                            },
+                            {
+                                "key": "secondary",
+                                "value": "Secondary"
+                            }
+                        ]
+                    },
+                    "defaultOption": "ignore",
+                    "description": "Role",
+                    "details": "Role",
+                    "key": "role",
+                    "objectType": "object",
+                    "optionType": [
+                        "constant",
+                        "variable",
+                        "ignore"
+                    ]
+                }
+            ],
+            "dataPath": [],
+            "defaultOption": "ignore",
+            "description": "DNS",
+            "details": "DNS",
+            "key": "dns",
+            "objectType": "tree",
+            "optionType": [
+                "constant",
+                "variable",
+                "ignore"
+            ],
+            "primaryKeys": [
+                "dns-addr"
+            ]
+        },
+        {
+            "children": [
+                {
+                    "dataPath": [],
+                    "dataType": {
+                        "type": "ipv6"
                     },
                     "defaultOption": "constant",
-                    "description": "Auto Tunnel Mode",
-                    "details": "Auto Tunnel Mode",
-                    "key": "auto",
+                    "description": "DNS Address",
+                    "details": "DNS Address",
+                    "key": "dns-addr",
                     "objectType": "object",
                     "optionType": [
                         "constant"
                     ]
                 },
                 {
                     "dataPath": [],
                     "dataType": {
-                        "default": "false",
-                        "label": {
-                            "off": "No",
-                            "on": "Yes"
-                        },
-                        "type": "boolean"
+                        "default": "primary",
+                        "type": "enum",
+                        "values": [
+                            {
+                                "key": "primary",
+                                "value": "Primary"
+                            },
+                            {
+                                "key": "secondary",
+                                "value": "Secondary"
+                            }
+                        ]
                     },
-                    "defaultOption": "notIgnore",
-                    "description": "Shutdown",
-                    "details": "Administrative state",
-                    "key": "shutdown",
+                    "defaultOption": "ignore",
+                    "description": "Role",
+                    "details": "Role",
+                    "key": "role",
                     "objectType": "object",
                     "optionType": [
                         "constant",
-                        "notIgnore"
+                        "variable",
+                        "ignore"
                     ]
-                },
+                }
+            ],
+            "dataPath": [],
+            "defaultOption": "ignore",
+            "description": "DNS",
+            "details": "DNS",
+            "key": "dns-ipv6",
+            "objectType": "tree",
+            "optionType": [
+                "constant",
+                "variable",
+                "ignore"
+            ],
+            "primaryKeys": [
+                "dns-addr"
+            ]
+        },
+        {
+            "dataPath": [
+                "ecmp-hash-key"
+            ],
+            "dataType": {
+                "default": "false",
+                "type": "boolean"
+            },
+            "defaultOption": "ignore",
+            "description": "Enhance ECMP Keying",
+            "details": "Optional packet fields for ECMP keying",
+            "key": "layer4",
+            "objectType": "object",
+            "optionType": [
+                "constant",
+                "variable",
+                "ignore"
+            ]
+        },
+        {
+            "children": [
                 {
                     "dataPath": [],
                     "dataType": {
                         "maxLength": 128,
                         "minLength": 1,
-                        "type": "string"
+                        "type": "dnsHostName"
                     },
-                    "defaultOption": "ignore",
-                    "description": "Description",
-                    "details": "Interface description",
-                    "key": "description",
+                    "defaultOption": "constant",
+                    "description": "Hostname",
+                    "details": "Hostname",
+                    "key": "hostname",
                     "objectType": "object",
                     "optionType": [
                         "constant",
-                        "variable",
-                        "ignore"
+                        "variable"
                     ]
                 },
                 {
-                    "dataPath": [
-                        "ip"
-                    ],
+                    "dataPath": [],
                     "dataType": {
-                        "default": "true",
-                        "type": "boolean"
+                        "max": 8,
+                        "type": "ip"
                     },
                     "defaultOption": "constant",
-                    "description": "Unnumbered Interface",
-                    "details": "Unnumbered interface",
-                    "key": "unnumbered",
-                    "objectType": "node-only",
+                    "description": "List of IP",
+                    "details": "List of IP",
+                    "key": "ip",
+                    "objectType": "list",
                     "optionType": [
-                        "constant"
+                        "constant",
+                        "variable"
                     ]
-                },
+                }
+            ],
+            "dataPath": [],
+            "defaultOption": "ignore",
+            "description": "Static DNS Mapping",
+            "details": "Static DNS mapping",
+            "key": "host",
+            "objectType": "tree",
+            "optionType": [
+                "constant",
+                "variable",
+                "ignore"
+            ],
+            "primaryKeys": [
+                "hostname"
+            ]
+        },
+        {
+            "children": [
                 {
-                    "dataPath": [
-                        "ip"
-                    ],
+                    "dataPath": [],
                     "dataType": {
-                        "type": "ipv4-prefix"
+                        "type": "enum",
+                        "values": [
+                            {
+                                "key": "FW",
+                                "value": "FW"
+                            },
+                            {
+                                "key": "IDS",
+                                "value": "IDS"
+                            },
+                            {
+                                "key": "IDP",
+                                "value": "IDP"
+                            },
+                            {
+                                "key": "netsvc1",
+                                "value": "netsvc1"
+                            },
+                            {
+                                "key": "netsvc2",
+                                "value": "netsvc2"
+                            },
+                            {
+                                "key": "netsvc3",
+                                "value": "netsvc3"
+                            },
+                            {
+                                "key": "netsvc4",
+                                "value": "netsvc4"
+                            },
+                            {
+                                "key": "TE",
+                                "value": "TE"
+                            },
+                            {
+                                "key": "appqoe",
+                                "value": "appqoe"
+                            }
+                        ]
                     },
-                    "defaultOption": "ignore",
-                    "description": "IPv4 address",
-                    "details": "Assign IPv4 address",
-                    "key": "address",
+                    "defaultOption": "constant",
+                    "description": "Service Type",
+                    "details": "Service Type",
+                    "key": "svc-type",
                     "objectType": "object",
                     "optionType": [
-                        "constant",
-                        "variable",
-                        "ignore"
+                        "constant"
                     ]
                 },
                 {
                     "dataPath": [],
                     "dataType": {
                         "type": "ipv4"
                     },
                     "defaultOption": "constant",
-                    "description": "Tunnel Source IP Address",
-                    "details": "Tunnel source IP Address",
-                    "key": "tunnel-source",
-                    "objectType": "object",
+                    "description": "IPv4 address",
+                    "details": "List of IPv4 address",
+                    "key": "address",
+                    "maxChildren": "4",
+                    "minChildren": "0",
+                    "objectType": "list",
                     "optionType": [
                         "constant",
                         "variable"
                     ]
                 },
                 {
                     "dataPath": [],
-                    "dataType": {
-                        "maxLength": 32,
-                        "minLength": 1,
-                        "type": "string"
-                    },
+                    "dataType": "string",
                     "defaultOption": "constant",
-                    "description": "Tunnel Source Interface",
-                    "details": "<1..32 characters> Interface name: ge0/<0-..> or ge0/<0-..>.vlanid",
-                    "key": "tunnel-source-interface",
+                    "description": "Interface",
+                    "details": "Tracking Service",
+                    "key": "interface",
                     "objectType": "object",
                     "optionType": [
                         "constant",
                         "variable"
                     ]
                 },
                 {
                     "dataPath": [],
                     "dataType": {
-                        "maxLength": 32,
-                        "minLength": 1,
-                        "type": "string"
+                        "default": "true",
+                        "type": "boolean"
                     },
-                    "defaultOption": "constant",
-                    "description": "Tunnel Route-via Interface",
-                    "details": "<1..32 characters> Interface name: ge0/<0-..> or ge0/<0-..>.vlanid",
-                    "key": "tunnel-route-via",
+                    "defaultOption": "ignore",
+                    "description": "Tracking",
+                    "details": "Tracking Service",
+                    "key": "track-enable",
                     "objectType": "object",
                     "optionType": [
                         "constant",
-                        "variable"
+                        "variable",
+                        "ignore"
                     ]
-                },
+                }
+            ],
+            "dataPath": [],
+            "defaultOption": "ignore",
+            "description": "Service",
+            "details": "Configure services",
+            "key": "service",
+            "objectType": "tree",
+            "optionType": [
+                "constant",
+                "variable",
+                "ignore"
+            ],
+            "primaryKeys": [
+                "svc-type"
+            ]
+        },
+        {
+            "children": [
                 {
                     "dataPath": [],
                     "dataType": {
-                        "type": "string"
+                        "type": "ipv4-prefix"
                     },
-                    "default": "dynamic",
                     "defaultOption": "constant",
-                    "description": "Tunnel Destination IP Address/FQDN(Ipsec)",
-                    "details": "Tunnel destination IP address",
-                    "key": "tunnel-destination",
+                    "description": "Prefix",
+                    "details": "Prefix",
+                    "key": "prefix",
                     "objectType": "object",
                     "optionType": [
                         "constant",
                         "variable"
                     ]
                 },
                 {
                     "dataPath": [],
                     "dataType": {
-                        "default": "sig",
-                        "type": "enum",
-                        "values": [
-                            {
-                                "key": "sig",
-                                "value": "Secure Internet Gateway"
-                            }
-                        ]
+                        "default": 0,
+                        "max": 0,
+                        "min": 0,
+                        "type": "number"
                     },
                     "defaultOption": "constant",
-                    "description": "Application",
-                    "details": "Enable Application Tunnel Type",
-                    "key": "application",
+                    "description": "VPN",
+                    "details": "Destination VPN to resolve the prefix",
+                    "key": "vpn",
                     "objectType": "object",
                     "optionType": [
                         "constant"
                     ]
                 },
                 {
                     "dataPath": [],
                     "dataType": {
                         "default": "sig",
                         "type": "enum",
                         "values": [
                             {
                                 "key": "sig",
-                                "value": "Secure Internet Gateway"
+                                "value": "SIG"
                             }
                         ]
                     },
-                    "defaultOption": "constant",
-                    "description": "Application",
-                    "details": "Enable Application Tunnel Type",
-                    "key": "application",
+                    "defaultOption": "notIgnore",
+                    "description": "Service",
+                    "details": "Service",
+                    "key": "service",
                     "objectType": "object",
                     "optionType": [
-                        "constant"
+                        "constant",
+                        "notIgnore"
                     ]
-                },
+                }
+            ],
+            "dataPath": [
+                "ip"
+            ],
+            "defaultOption": "ignore",
+            "description": "IPv4 Static Service Route",
+            "details": "Configure IPv4 Static Service Routes",
+            "key": "service-route",
+            "objectType": "tree",
+            "optionType": [
+                "constant",
+                "ignore"
+            ],
+            "primaryKeys": [
+                "prefix"
+            ]
+        },
+        {
+            "children": [
                 {
                     "dataPath": [],
                     "dataType": {
-                        "default": "secure-internet-gateway-umbrella",
-                        "type": "enum",
-                        "values": [
-                            {
-                                "key": "secure-internet-gateway-umbrella",
-                                "value": "Umbrella"
-                            },
-                            {
-                                "key": "secure-internet-gateway-zscaler",
-                                "value": "Zscaler"
-                            },
-                            {
-                                "key": "secure-internet-gateway-other",
-                                "value": "Generic"
-                            }
-                        ]
+                        "type": "ipv4-prefix"
                     },
                     "defaultOption": "constant",
-                    "description": "SIG Provider",
-                    "details": "SIG Tunnel Provider",
-                    "key": "tunnel-set",
+                    "description": "Prefix",
+                    "details": "Prefix",
+                    "key": "prefix",
                     "objectType": "object",
                     "optionType": [
-                        "constant"
+                        "constant",
+                        "variable"
                     ]
                 },
                 {
+                    "children": [
+                        {
+                            "dataPath": [],
+                            "dataType": {
+                                "type": "string"
+                            },
+                            "defaultOption": "constant",
+                            "description": "Address",
+                            "details": "IP Address",
+                            "key": "address",
+                            "objectType": "object",
+                            "optionType": [
+                                "constant",
+                                "variable"
+                            ]
+                        },
+                        {
+                            "dataPath": [],
+                            "dataType": {
+                                "default": 1,
+                                "max": 255,
+                                "min": 1,
+                                "type": "number"
+                            },
+                            "defaultOption": "ignore",
+                            "description": "Distance",
+                            "details": "Administrative distance",
+                            "key": "distance",
+                            "objectType": "object",
+                            "optionType": [
+                                "constant",
+                                "variable",
+                                "ignore"
+                            ]
+                        }
+                    ],
                     "dataPath": [],
-                    "dataType": {
-                        "default": "primary-dc",
-                        "type": "enum",
-                        "values": [
-                            {
-                                "key": "primary-dc",
-                                "value": "Primary"
+                    "defaultOption": "ignore",
+                    "description": "IP Gateway",
+                    "details": "IP gateway address",
+                    "key": "next-hop",
+                    "objectType": "tree",
+                    "optionType": [
+                        "constant",
+                        "variable",
+                        "ignore"
+                    ],
+                    "primaryKeys": [
+                        "address"
+                    ]
+                },
+                {
+                    "children": [
+                        {
+                            "dataPath": [],
+                            "dataType": {
+                                "type": "string"
                             },
-                            {
-                                "key": "secondary-dc",
-                                "value": "Secondary"
-                            }
-                        ]
-                    },
-                    "defaultOption": "constant",
-                    "description": "Data-Center",
-                    "details": "SIG Tunnel Data Center",
-                    "key": "tunnel-dc-preference",
-                    "objectType": "object",
+                            "defaultOption": "constant",
+                            "description": "Address",
+                            "details": "IP Address",
+                            "key": "address",
+                            "objectType": "object",
+                            "optionType": [
+                                "constant",
+                                "variable"
+                            ]
+                        },
+                        {
+                            "dataPath": [],
+                            "dataType": {
+                                "default": 1,
+                                "max": 255,
+                                "min": 1,
+                                "type": "number"
+                            },
+                            "defaultOption": "ignore",
+                            "description": "Distance",
+                            "details": "Administrative distance",
+                            "key": "distance",
+                            "objectType": "object",
+                            "optionType": [
+                                "constant",
+                                "variable",
+                                "ignore"
+                            ]
+                        },
+                        {
+                            "dataPath": [],
+                            "dataType": {
+                                "type": "string"
+                            },
+                            "defaultOption": "constant",
+                            "description": "Tracker",
+                            "details": "Static route tracker",
+                            "key": "tracker",
+                            "objectType": "object",
+                            "optionType": [
+                                "constant",
+                                "variable"
+                            ]
+                        }
+                    ],
+                    "dataPath": [],
+                    "defaultOption": "ignore",
+                    "description": "IP Gateway",
+                    "details": "IP gateway address",
+                    "key": "next-hop-with-track",
+                    "objectType": "tree",
                     "optionType": [
-                        "constant"
+                        "constant",
+                        "variable",
+                        "ignore"
+                    ],
+                    "primaryKeys": [
+                        "address"
                     ]
                 },
                 {
                     "dataPath": [],
                     "dataType": {
-                        "max": 1460,
-                        "min": 500,
-                        "type": "number"
+                        "default": "false",
+                        "type": "boolean"
                     },
                     "defaultOption": "ignore",
-                    "description": "TCP MSS",
-                    "details": "TCP MSS on SYN packets, in bytes",
-                    "key": "tcp-mss-adjust",
-                    "objectType": "object",
+                    "description": "null0",
+                    "details": "null0",
+                    "key": "null0",
+                    "objectType": "node-only",
                     "optionType": [
                         "constant",
                         "variable",
                         "ignore"
                     ]
                 },
                 {
                     "dataPath": [],
                     "dataType": {
-                        "default": 1400,
-                        "max": 2000,
-                        "min": 576,
+                        "default": 1,
+                        "max": 255,
+                        "min": 1,
                         "type": "number"
                     },
-                    "defaultOption": "notIgnore",
-                    "description": "IP MTU",
-                    "details": "Interface MTU <576..2000>, in bytes",
-                    "key": "mtu",
+                    "defaultOption": "ignore",
+                    "description": "Distance",
+                    "details": "Administrative distance",
+                    "key": "distance",
                     "objectType": "object",
                     "optionType": [
                         "constant",
                         "variable",
-                        "notIgnore"
+                        "ignore"
                     ]
                 },
                 {
-                    "dataPath": [
-                        "dead-peer-detection"
-                    ],
+                    "dataPath": [],
                     "dataType": {
-                        "default": 10,
-                        "max": 65535,
-                        "min": 0,
+                        "default": 0,
+                        "range": "0",
                         "type": "number"
                     },
                     "defaultOption": "ignore",
-                    "description": "DPD Interval",
-                    "details": "IKE keepalive interval (seconds)",
-                    "key": "dpd-interval",
+                    "description": "VPN",
+                    "details": "Destination VPN(!=0 or !=512) to resolve the prefix",
+                    "key": "vpn",
                     "objectType": "object",
                     "optionType": [
                         "constant",
                         "variable",
                         "ignore"
                     ]
                 },
                 {
-                    "dataPath": [
-                        "dead-peer-detection"
-                    ],
+                    "dataPath": [],
                     "dataType": {
-                        "default": 3,
-                        "max": 255,
-                        "min": 0,
-                        "type": "number"
+                        "default": "false",
+                        "type": "boolean"
                     },
                     "defaultOption": "ignore",
-                    "description": "DPD Retries",
-                    "details": "IKE keepalive retries",
-                    "key": "dpd-retries",
-                    "objectType": "object",
+                    "description": "DHCP",
+                    "details": "Default Gateway obtained from DHCP",
+                    "key": "dhcp",
+                    "objectType": "node-only",
                     "optionType": [
                         "constant",
                         "variable",
                         "ignore"
                     ]
-                },
+                }
+            ],
+            "dataPath": [
+                "ip"
+            ],
+            "defaultOption": "ignore",
+            "description": "IPv4 Static Route",
+            "details": "Configure IPv4 Static Routes",
+            "key": "route",
+            "objectType": "tree",
+            "optionType": [
+                "constant",
+                "variable",
+                "ignore"
+            ],
+            "primaryKeys": [
+                "prefix"
+            ]
+        },
+        {
+            "children": [
                 {
-                    "dataPath": [
-                        "ike"
-                    ],
+                    "dataPath": [],
                     "dataType": {
-                        "default": 2,
-                        "max": 2,
-                        "min": 1,
-                        "type": "number"
+                        "type": "ipv6-prefix"
                     },
                     "defaultOption": "constant",
-                    "description": "IKE Version",
-                    "details": "IKE Version <1..2>",
-                    "key": "ike-version",
+                    "description": "Prefix",
+                    "details": "Prefix",
+                    "key": "prefix",
                     "objectType": "object",
                     "optionType": [
                         "constant",
+                        "variable"
+                    ]
+                },
+                {
+                    "children": [
+                        {
+                            "dataPath": [],
+                            "dataType": {
+                                "type": "ipv6"
+                            },
+                            "defaultOption": "constant",
+                            "description": "Address",
+                            "details": "IP Address",
+                            "key": "address",
+                            "objectType": "object",
+                            "optionType": [
+                                "constant",
+                                "variable"
+                            ]
+                        },
+                        {
+                            "dataPath": [],
+                            "dataType": {
+                                "default": 1,
+                                "max": 255,
+                                "min": 1,
+                                "type": "number"
+                            },
+                            "defaultOption": "ignore",
+                            "description": "Distance",
+                            "details": "Administrative distance",
+                            "key": "distance",
+                            "objectType": "object",
+                            "optionType": [
+                                "constant",
+                                "variable",
+                                "ignore"
+                            ]
+                        }
+                    ],
+                    "dataPath": [],
+                    "defaultOption": "ignore",
+                    "description": "IP Gateway",
+                    "details": "IP gateway address",
+                    "key": "next-hop",
+                    "objectType": "tree",
+                    "optionType": [
+                        "constant",
                         "variable",
                         "ignore"
+                    ],
+                    "primaryKeys": [
+                        "address"
                     ]
                 },
                 {
-                    "dataPath": [
-                        "ike",
-                        "authentication-type",
-                        "pre-shared-key"
-                    ],
+                    "dataPath": [],
                     "dataType": {
-                        "maxLength": 127,
-                        "minLength": 1,
-                        "type": "restrictedPassphrase"
+                        "default": "false",
+                        "type": "boolean"
                     },
                     "defaultOption": "ignore",
-                    "description": "Preshared Key",
-                    "details": "Use preshared key to authenticate IKE peer",
-                    "key": "pre-shared-secret",
-                    "objectType": "object",
+                    "description": "null0",
+                    "details": "null0",
+                    "key": "null0",
+                    "objectType": "node-only",
                     "optionType": [
                         "constant",
                         "variable",
                         "ignore"
                     ]
                 },
                 {
-                    "dataPath": [
-                        "ike"
-                    ],
+                    "dataPath": [],
                     "dataType": {
-                        "default": 14400,
-                        "max": 1209600,
-                        "min": 300,
+                        "default": 0,
+                        "range": "0",
                         "type": "number"
                     },
                     "defaultOption": "ignore",
-                    "description": "IKE Rekey Interval (seconds)",
-                    "details": "IKE rekey interval <300..1209600> seconds",
-                    "key": "ike-rekey-interval",
+                    "description": "VPN",
+                    "details": "Destination VPN(!=0 or !=512) to resolve the prefix",
+                    "key": "vpn",
                     "objectType": "object",
                     "optionType": [
                         "constant",
                         "variable",
                         "ignore"
                     ]
                 },
                 {
-                    "dataPath": [
-                        "ike"
-                    ],
+                    "dataPath": [],
                     "dataType": {
-                        "default": "aes256-cbc-sha1",
-                        "type": "enum",
+                        "default": "NAT64",
+                        "type": "radioButtonList",
                         "values": [
                             {
-                                "key": "aes256-cbc-sha1",
-                                "value": "AES 256 CBC SHA1"
+                                "label": "NAT64",
+                                "value": "NAT64"
                             },
                             {
-                                "key": "aes256-cbc-sha2",
-                                "value": "AES 256 CBC SHA2"
-                            },
-                            {
-                                "key": "aes128-cbc-sha1",
-                                "value": "AES 128 CBC SHA1"
-                            },
-                            {
-                                "key": "aes128-cbc-sha2",
-                                "value": "AES 128 CBC SHA2"
+                                "label": "NAT66",
+                                "value": "NAT66"
                             }
                         ]
                     },
-                    "defaultOption": "ignore",
-                    "description": "IKE Cipher Suite",
-                    "details": "IKE identity the IKE preshared secret belongs to",
-                    "key": "ike-ciphersuite",
+                    "defaultOption": "constant",
+                    "description": "NAT",
+                    "details": "NAT",
+                    "key": "nat",
                     "objectType": "object",
                     "optionType": [
                         "constant",
                         "variable",
                         "ignore"
                     ]
-                },
+                }
+            ],
+            "dataPath": [
+                "ipv6"
+            ],
+            "defaultOption": "ignore",
+            "description": "IPv6 Static Route",
+            "details": "Configure IPv6 Static Routes",
+            "key": "route",
+            "objectType": "tree",
+            "optionType": [
+                "constant",
+                "variable",
+                "ignore"
+            ],
+            "primaryKeys": [
+                "prefix"
+            ]
+        },
+        {
+            "children": [
                 {
-                    "dataPath": [
-                        "ike"
-                    ],
+                    "dataPath": [],
                     "dataType": {
-                        "default": "14",
-                        "type": "enum",
-                        "values": [
-                            {
-                                "key": "2",
-                                "value": "2 1024-bit modulus"
-                            },
-                            {
-                                "key": "5",
-                                "value": "5 1536-bit modulus"
-                            },
-                            {
-                                "key": "14",
-                                "value": "14 2048-bit modulus"
-                            },
-                            {
-                                "key": "15",
-                                "value": "15 3072-bit modulus"
-                            },
-                            {
-                                "key": "16",
-                                "value": "16 4096-bit modulus"
-                            },
-                            {
-                                "key": "19",
-                                "value": "19 256-bit random ECP"
-                            },
-                            {
-                                "key": "20",
-                                "value": "20 384-bit random ECP"
-                            },
-                            {
-                                "key": "21",
-                                "value": "21 521-bit random ECP"
-                            }
-                        ]
+                        "type": "ipv4-prefix"
                     },
-                    "defaultOption": "notIgnore",
-                    "description": "IKE Diffie-Hellman Group",
-                    "details": "IKE Diffie Hellman Groups",
-                    "key": "ike-group",
+                    "defaultOption": "constant",
+                    "description": "Prefix",
+                    "details": "Prefix",
+                    "key": "prefix",
                     "objectType": "object",
                     "optionType": [
                         "constant",
-                        "variable",
-                        "notIgnore"
+                        "variable"
                     ]
                 },
                 {
-                    "dataPath": [
-                        "ike",
-                        "authentication-type"
-                    ],
+                    "dataPath": [],
                     "dataType": {
-                        "default": "true",
-                        "type": "boolean"
+                        "default": 0,
+                        "max": 0,
+                        "min": 0,
+                        "type": "number"
                     },
                     "defaultOption": "constant",
-                    "description": "Preshared Key",
-                    "details": "Use preshared key to authenticate IKE peer",
-                    "key": "pre-shared-key-dynamic",
-                    "objectType": "node-only",
+                    "description": "VPN",
+                    "details": "Destination VPN to resolve the prefix",
+                    "key": "vpn",
+                    "objectType": "object",
                     "optionType": [
                         "constant"
                     ]
                 },
                 {
-                    "dataPath": [
-                        "ike",
-                        "authentication-type",
-                        "pre-shared-key"
-                    ],
+                    "dataPath": [],
                     "dataType": {
-                        "maxLength": 63,
-                        "minLength": 1,
-                        "type": "ike"
+                        "type": "string"
                     },
                     "defaultOption": "ignore",
-                    "description": "IKE ID for local End point",
-                    "details": "IKE ID for the local endpoint. Input IPv4 address, domain name, or email address",
-                    "key": "ike-local-id",
-                    "objectType": "object",
+                    "description": "GRE Interface (Maximum entries allowed: 2)",
+                    "details": "List of GRE Interfaces",
+                    "key": "interface",
+                    "maxChildren": "2",
+                    "minChildren": "0",
+                    "objectType": "list",
                     "optionType": [
                         "constant",
                         "variable",
                         "ignore"
                     ]
-                },
+                }
+            ],
+            "dataPath": [
+                "ip"
+            ],
+            "defaultOption": "ignore",
+            "description": "IPv4 Static GRE Route",
+            "details": "Configure routes pointing to a GRE tunnel",
+            "key": "gre-route",
+            "objectType": "tree",
+            "optionType": [
+                "constant",
+                "variable",
+                "ignore"
+            ],
+            "primaryKeys": [
+                "prefix"
+            ]
+        },
+        {
+            "children": [
                 {
-                    "dataPath": [
-                        "ike",
-                        "authentication-type",
-                        "pre-shared-key"
-                    ],
+                    "dataPath": [],
                     "dataType": {
-                        "maxLength": 63,
-                        "minLength": 1,
-                        "type": "ike"
+                        "type": "ipv4-prefix"
                     },
-                    "defaultOption": "ignore",
-                    "description": "IKE ID for Remote End point",
-                    "details": "IKE ID for the remote endpoint. Input IPv4 address, domain name, or email address",
-                    "key": "ike-remote-id",
+                    "defaultOption": "constant",
+                    "description": "Prefix",
+                    "details": "Prefix",
+                    "key": "prefix",
                     "objectType": "object",
                     "optionType": [
                         "constant",
-                        "variable",
-                        "ignore"
+                        "variable"
                     ]
                 },
                 {
-                    "dataPath": [
-                        "ipsec"
-                    ],
+                    "dataPath": [],
                     "dataType": {
-                        "default": 3600,
-                        "max": 1209600,
-                        "min": 300,
+                        "default": 0,
+                        "max": 0,
+                        "min": 0,
                         "type": "number"
                     },
-                    "defaultOption": "ignore",
-                    "description": "IPsec Rekey Interval (seconds)",
-                    "details": "IPsec rekey interval <300..1209600> seconds",
-                    "key": "ipsec-rekey-interval",
+                    "defaultOption": "constant",
+                    "description": "VPN",
+                    "details": "Destination VPN to resolve the prefix",
+                    "key": "vpn",
                     "objectType": "object",
                     "optionType": [
-                        "constant",
-                        "variable",
-                        "ignore"
+                        "constant"
                     ]
                 },
                 {
-                    "dataPath": [
-                        "ipsec"
-                    ],
+                    "dataPath": [],
                     "dataType": {
-                        "default": 512,
-                        "max": 4096,
-                        "min": 64,
-                        "type": "number"
+                        "type": "interfaceList"
                     },
                     "defaultOption": "ignore",
-                    "description": "IPsec Replay Window",
-                    "details": "Replay window size 32..8192 (must be a power of 2)",
-                    "key": "ipsec-replay-window",
-                    "objectType": "object",
+                    "description": "IPSEC Interface (Maximum entries allowed: 2)",
+                    "details": "List of IPSEC Interfaces (Separated by commas)",
+                    "key": "interface",
+                    "maxChildren": "2",
+                    "minChildren": "0",
+                    "objectType": "list",
                     "optionType": [
                         "constant",
                         "variable",
                         "ignore"
                     ]
-                },
+                }
+            ],
+            "dataPath": [
+                "ip"
+            ],
+            "defaultOption": "ignore",
+            "description": "IPv4 Static IPSEC Route",
+            "details": "Configure routes pointing to a IPSEC tunnel",
+            "key": "ipsec-route",
+            "objectType": "tree",
+            "optionType": [
+                "constant",
+                "variable",
+                "ignore"
+            ],
+            "primaryKeys": [
+                "prefix"
+            ]
+        },
+        {
+            "children": [
                 {
-                    "dataPath": [
-                        "ipsec"
-                    ],
+                    "dataPath": [],
                     "dataType": {
-                        "default": "aes256-gcm",
                         "type": "enum",
                         "values": [
                             {
-                                "key": "aes256-cbc-sha1",
-                                "value": "AES 256 CBC SHA1"
+                                "key": "bgp",
+                                "value": "BGP"
                             },
                             {
-                                "key": "aes256-cbc-sha384",
-                                "value": "AES 256 CBC SHA 384"
+                                "key": "ospf",
+                                "value": "OSPF"
                             },
                             {
-                                "key": "aes256-cbc-sha256",
-                                "value": "AES 256 CBC SHA 256"
+                                "key": "ospfv3",
+                                "value": "OSPFV3"
                             },
                             {
-                                "key": "aes256-cbc-sha512",
-                                "value": "AES 256 CBC SHA 512"
+                                "key": "connected",
+                                "value": "Connected"
                             },
                             {
-                                "key": "aes256-gcm",
-                                "value": "AES 256 GCM"
+                                "key": "static",
+                                "value": "Static"
                             },
                             {
-                                "key": "null-sha1",
-                                "value": "Null SHA1"
+                                "key": "network",
+                                "value": "Network"
                             },
                             {
-                                "key": "null-sha384",
-                                "value": "Nul SHA 384"
+                                "key": "aggregate",
+                                "value": "Aggregate"
                             },
                             {
-                                "key": "null-sha256",
-                                "value": "Nul SHA 256"
+                                "key": "eigrp",
+                                "value": "EIGRP"
                             },
                             {
-                                "key": "null-sha512",
-                                "value": "Nul SHA 512"
+                                "key": "lisp",
+                                "value": "LISP"
+                            },
+                            {
+                                "key": "isis",
+                                "value": "ISIS"
                             }
                         ]
                     },
-                    "defaultOption": "notIgnore",
-                    "description": "IPsec Cipher Suite",
-                    "details": "IPsec(ESP) encryption and integrity protocol",
-                    "key": "ipsec-ciphersuite",
+                    "defaultOption": "constant",
+                    "description": "Protocol",
+                    "details": "Advertised routes protocol",
+                    "key": "protocol",
                     "objectType": "object",
                     "optionType": [
                         "constant",
                         "variable",
-                        "notIgnore"
+                        "ignore"
                     ]
                 },
                 {
-                    "dataPath": [
-                        "ipsec"
-                    ],
+                    "dataPath": [],
                     "dataType": {
-                        "default": "none",
-                        "type": "enum",
-                        "values": [
-                            {
-                                "key": "group-2",
-                                "value": "Group-2 1024-bit modulus"
-                            },
-                            {
-                                "key": "group-5",
-                                "value": "Group-5 1536-bit modulus"
-                            },
-                            {
-                                "key": "group-14",
-                                "value": "Group-14 2048-bit modulus"
-                            },
-                            {
-                                "key": "group-15",
-                                "value": "Group-15 3072-bit modulus"
-                            },
-                            {
-                                "key": "group-16",
-                                "value": "Group-16 4096-bit modulus"
-                            },
-                            {
-                                "key": "group-19",
-                                "value": "Group-19 256-bit random ECP"
-                            },
-                            {
-                                "key": "group-20",
-                                "value": "Group-20 384-bit random ECP"
-                            },
-                            {
-                                "key": "group-21",
-                                "value": "Group-21 521-bit random ECP"
-                            },
-                            {
-                                "key": "none",
-                                "value": "None"
-                            }
-                        ]
+                        "maxLength": 127,
+                        "minLength": 1,
+                        "type": "string"
                     },
-                    "defaultOption": "notIgnore",
-                    "description": "Perfect Forward Secrecy",
-                    "details": "IPsec perfect forward secrecy settings",
-                    "key": "perfect-forward-secrecy",
+                    "defaultOption": "ignore",
+                    "description": "Route Policy",
+                    "details": "Set Route Policy to OMP",
+                    "key": "route-policy",
                     "objectType": "object",
                     "optionType": [
                         "constant",
                         "variable",
-                        "notIgnore"
+                        "ignore"
                     ]
                 },
                 {
                     "dataPath": [],
                     "dataType": {
                         "type": "enum",
                         "values": [
                             {
-                                "key": "",
-                                "value": ""
+                                "key": "external",
+                                "value": "External"
                             }
                         ]
                     },
                     "defaultOption": "ignore",
-                    "description": "Tracker",
-                    "details": "Enable tracker for this interface",
-                    "key": "tracker",
-                    "objectType": "object",
-                    "optionType": [
-                        "constant",
-                        "ignore"
-                    ]
-                },
-                {
-                    "dataPath": [],
-                    "dataType": {
-                        "default": "true",
-                        "type": "boolean"
-                    },
-                    "defaultOption": "ignore",
-                    "description": "Track this interface for SIG",
-                    "details": "Enable/disable SIG tracking",
-                    "key": "track-enable",
-                    "objectType": "object",
+                    "key": "protocol-sub-type",
+                    "minElements": 1,
+                    "objectType": "list",
                     "optionType": [
                         "constant",
+                        "variable",
                         "ignore"
                     ]
                 },
                 {
+                    "children": [
+                        {
+                            "dataPath": [],
+                            "dataType": {
+                                "type": "ipv4-prefix"
+                            },
+                            "defaultOption": "constant",
+                            "description": "Prefix",
+                            "details": "Prefix",
+                            "key": "prefix-entry",
+                            "objectType": "object",
+                            "optionType": [
+                                "constant",
+                                "variable"
+                            ]
+                        },
+                        {
+                            "dataPath": [],
+                            "dataType": {
+                                "default": "false",
+                                "type": "boolean"
+                            },
+                            "defaultOption": "ignore",
+                            "description": "Aggregate Only",
+                            "details": "Aggregate Only",
+                            "key": "aggregate-only",
+                            "objectType": "object",
+                            "optionType": [
+                                "constant",
+                                "variable",
+                                "ignore"
+                            ]
+                        }
+                    ],
                     "dataPath": [],
-                    "dataType": {
-                        "default": "Auto",
-                        "type": "ipv4"
-                    },
                     "defaultOption": "ignore",
-                    "description": "Source Public IP",
-                    "details": "Public IP required to setup GRE tunnel to Zscaler",
-                    "key": "tunnel-public-ip",
-                    "objectType": "object",
+                    "key": "prefix-list",
+                    "minElements": 1,
+                    "objectType": "tree",
                     "optionType": [
                         "constant",
                         "variable",
                         "ignore"
+                    ],
+                    "primaryKeys": [
+                        "prefix-entry"
                     ]
                 }
             ],
-            "dataPath": [],
-            "defaultOption": "constant",
-            "description": "IPSec Interface",
-            "details": "Interface name: IPsec when present",
-            "key": "interface",
-            "maxElements": 4,
-            "minElements": 1,
+            "dataPath": [
+                "omp"
+            ],
+            "defaultOption": "ignore",
+            "description": "Advertise",
+            "details": "Advertise routes to OMP",
+            "key": "advertise",
             "objectType": "tree",
             "optionType": [
                 "constant",
-                "variable"
+                "variable",
+                "ignore"
             ],
             "primaryKeys": [
-                "if-name"
+                "protocol"
             ]
         },
         {
             "children": [
                 {
                     "dataPath": [],
                     "dataType": {
-                        "default": "sig",
                         "type": "enum",
                         "values": [
                             {
-                                "key": "sig",
-                                "value": "SIG"
+                                "key": "bgp",
+                                "value": "BGP"
+                            },
+                            {
+                                "key": "ospf",
+                                "value": "Ospf"
+                            },
+                            {
+                                "key": "connected",
+                                "value": "Connected"
+                            },
+                            {
+                                "key": "static",
+                                "value": "Static"
+                            },
+                            {
+                                "key": "network",
+                                "value": "Network"
+                            },
+                            {
+                                "key": "aggregate",
+                                "value": "Aggregate"
                             }
                         ]
                     },
                     "defaultOption": "constant",
-                    "description": "Service Type",
-                    "details": "Service Type",
-                    "key": "svc-type",
+                    "description": "Protocol",
+                    "details": "Advertised routes protocol",
+                    "key": "protocol",
                     "objectType": "object",
                     "optionType": [
-                        "constant"
+                        "constant",
+                        "variable",
+                        "ignore"
+                    ]
+                },
+                {
+                    "dataPath": [],
+                    "dataType": {
+                        "maxLength": 127,
+                        "minLength": 1,
+                        "type": "string"
+                    },
+                    "defaultOption": "ignore",
+                    "description": "Route Policy",
+                    "key": "route-policy",
+                    "objectType": "object",
+                    "optionType": [
+                        "constant",
+                        "variable",
+                        "ignore"
+                    ]
+                },
+                {
+                    "dataPath": [],
+                    "dataType": {
+                        "type": "enum",
+                        "values": [
+                            {
+                                "key": "external",
+                                "value": "External"
+                            }
+                        ]
+                    },
+                    "defaultOption": "ignore",
+                    "key": "protocol-sub-type",
+                    "minElements": 1,
+                    "objectType": "list",
+                    "optionType": [
+                        "constant",
+                        "variable",
+                        "ignore"
                     ]
                 },
                 {
                     "children": [
                         {
                             "dataPath": [],
                             "dataType": {
-                                "type": "enum",
-                                "values": [
-                                    {
-                                        "key": "",
-                                        "value": ""
-                                    }
-                                ]
-                            },
-                            "defaultOption": "constant",
-                            "description": "Active Tunnel Interface",
-                            "details": "Active Tunnel Interface for SIG",
-                            "key": "active-interface",
-                            "objectType": "object",
-                            "optionType": [
-                                "constant"
-                            ]
-                        },
-                        {
-                            "dataPath": [],
-                            "dataType": {
-                                "default": 1,
-                                "max": 255,
-                                "min": 1,
-                                "type": "number"
-                            },
-                            "defaultOption": "constant",
-                            "description": "Weight",
-                            "details": "Active Tunnel Interface Weight",
-                            "key": "active-interface-weight",
-                            "objectType": "object",
-                            "optionType": [
-                                "constant"
-                            ]
-                        },
-                        {
-                            "dataPath": [],
-                            "dataType": {
-                                "type": "enum",
-                                "values": [
-                                    {
-                                        "key": "",
-                                        "value": ""
-                                    }
-                                ]
+                                "type": "ipv6-prefix"
                             },
                             "defaultOption": "constant",
-                            "description": "Backup Tunnel Interface",
-                            "details": "Backup Tunnel Interface for SIG",
-                            "key": "backup-interface",
+                            "description": "Prefix",
+                            "details": "Prefix",
+                            "key": "prefix-entry",
                             "objectType": "object",
                             "optionType": [
-                                "constant"
+                                "constant",
+                                "variable"
                             ]
                         },
                         {
                             "dataPath": [],
                             "dataType": {
-                                "default": 1,
-                                "max": 255,
-                                "min": 1,
-                                "type": "number"
+                                "default": "false",
+                                "type": "boolean"
                             },
-                            "defaultOption": "constant",
-                            "description": "Weight",
-                            "details": "Backup Tunnel Interface Weight",
-                            "key": "backup-interface-weight",
+                            "defaultOption": "ignore",
+                            "description": "Aggregate Only",
+                            "details": "Aggregate Only",
+                            "key": "aggregate-only",
                             "objectType": "object",
                             "optionType": [
-                                "constant"
+                                "constant",
+                                "variable",
+                                "ignore"
                             ]
                         }
                     ],
-                    "dataPath": [
-                        "ha-pairs"
-                    ],
-                    "defaultOption": "constant",
-                    "description": "Interface Pair",
-                    "details": "Interface Pair for active and backup",
-                    "key": "interface-pair",
-                    "maxElements": 4,
+                    "dataPath": [],
+                    "defaultOption": "ignore",
+                    "key": "prefix-list",
                     "minElements": 1,
                     "objectType": "tree",
                     "optionType": [
-                        "constant"
+                        "constant",
+                        "variable",
+                        "ignore"
                     ],
                     "primaryKeys": [
-                        "active-interface",
-                        "backup-interface"
+                        "prefix-entry"
+                    ]
+                }
+            ],
+            "dataPath": [
+                "omp"
+            ],
+            "defaultOption": "ignore",
+            "description": "Advertise",
+            "details": "Advertise routes to OMP",
+            "key": "ipv6-advertise",
+            "objectType": "tree",
+            "optionType": [
+                "constant",
+                "variable",
+                "ignore"
+            ],
+            "primaryKeys": [
+                "protocol"
+            ]
+        },
+        {
+            "children": [
+                {
+                    "dataPath": [],
+                    "dataType": {
+                        "maxLength": 32,
+                        "minLength": 1,
+                        "type": "string"
+                    },
+                    "defaultOption": "constant",
+                    "description": "NAT64 Pool name",
+                    "details": "NAT64 Pool name",
+                    "key": "name",
+                    "objectType": "object",
+                    "optionType": [
+                        "constant"
                     ]
                 },
                 {
-                    "dataPath": [
-                        "zscaler-location-settings"
-                    ],
+                    "dataPath": [],
                     "dataType": {
-                        "default": "false",
-                        "type": "boolean"
+                        "type": "ipv4"
                     },
-                    "defaultOption": "ignore",
-                    "description": "Authentication Required",
-                    "details": "Enforce Authentication",
-                    "key": "auth-required",
+                    "defaultOption": "constant",
+                    "description": "NAT 64 v4 Pool Range Start",
+                    "details": "Starting IP address of NAT pool range",
+                    "key": "start-address",
                     "objectType": "object",
                     "optionType": [
                         "constant",
-                        "ignore"
+                        "variable"
                     ]
                 },
                 {
-                    "dataPath": [
-                        "zscaler-location-settings"
-                    ],
+                    "dataPath": [],
                     "dataType": {
-                        "default": "false",
-                        "type": "boolean"
+                        "type": "ipv4"
                     },
-                    "defaultOption": "ignore",
-                    "description": "XFF Forwarding",
-                    "details": "XFF forwarding enabled",
-                    "key": "xff-forward-enabled",
+                    "defaultOption": "constant",
+                    "description": "NAT 64 v4 Pool Range End",
+                    "details": "Ending IP address of NAT pool range",
+                    "key": "end-address",
                     "objectType": "object",
                     "optionType": [
                         "constant",
-                        "ignore"
+                        "variable"
                     ]
                 },
                 {
-                    "dataPath": [
-                        "zscaler-location-settings"
-                    ],
+                    "dataPath": [],
                     "dataType": {
                         "default": "false",
                         "type": "boolean"
                     },
                     "defaultOption": "ignore",
-                    "description": "Enable Firewall",
-                    "details": "Firewall enabled",
-                    "key": "ofw-enabled",
-                    "objectType": "object",
+                    "description": "NAT 64 Overload",
+                    "details": "NAT 64 Overload Option",
+                    "key": "overload",
+                    "objectType": "node-only",
                     "optionType": [
                         "constant",
+                        "variable",
                         "ignore"
                     ]
                 },
                 {
-                    "dataPath": [
-                        "zscaler-location-settings"
-                    ],
+                    "dataPath": [],
                     "dataType": {
                         "default": "false",
                         "type": "boolean"
                     },
-                    "defaultOption": "ignore",
-                    "description": "Enable IPS Control",
-                    "details": "Enable IPS Control",
-                    "key": "ips-control",
+                    "defaultOption": "constant",
+                    "description": "Enable Route Leaking from Global VPN",
+                    "details": "Enable Route Leaking from Global VPN to this Service VPN",
+                    "key": "leak_from_global",
                     "objectType": "object",
                     "optionType": [
-                        "constant",
-                        "ignore"
+                        "constant"
                     ]
                 },
                 {
-                    "dataPath": [
-                        "zscaler-location-settings"
-                    ],
+                    "dataPath": [],
+                    "dataType": {
+                        "type": "enum",
+                        "values": [
+                            {
+                                "key": "all",
+                                "value": "All"
+                            },
+                            {
+                                "key": "static",
+                                "value": "Static"
+                            },
+                            {
+                                "key": "mobile",
+                                "value": "Mobile"
+                            },
+                            {
+                                "key": "connected",
+                                "value": "Connected"
+                            },
+                            {
+                                "key": "rip",
+                                "value": "Rip"
+                            },
+                            {
+                                "key": "odr",
+                                "value": "Odr"
+                            }
+                        ]
+                    },
+                    "defaultOption": "constant",
+                    "description": "Protocol",
+                    "details": "Select protocol for route leaking",
+                    "key": "leak_from_global_protocol",
+                    "objectType": "object",
+                    "optionType": [
+                        "constant"
+                    ]
+                },
+                {
+                    "dataPath": [],
                     "dataType": {
                         "default": "false",
                         "type": "boolean"
                     },
-                    "defaultOption": "ignore",
-                    "description": "Enable Caution",
-                    "details": "Enable Caution",
-                    "key": "caution-enabled",
+                    "defaultOption": "constant",
+                    "description": "Enable Route Leaking to Global VPN",
+                    "details": "Enable Route Leaking from this Service VPN to Global VPN",
+                    "key": "leak_to_global",
+                    "objectType": "object",
+                    "optionType": [
+                        "constant"
+                    ]
+                }
+            ],
+            "dataPath": [
+                "nat64",
+                "v4"
+            ],
+            "defaultOption": "ignore",
+            "description": "NAT64 V4 Pool",
+            "details": "Set NAT64 v4 pool range",
+            "key": "pool",
+            "objectType": "tree",
+            "optionType": [
+                "constant",
+                "variable",
+                "ignore"
+            ],
+            "primaryKeys": [
+                "name"
+            ]
+        },
+        {
+            "children": [
+                {
+                    "dataPath": [],
+                    "dataType": {
+                        "max": 31,
+                        "min": 1,
+                        "type": "number"
+                    },
+                    "defaultOption": "constant",
+                    "description": "NAT Pool Name",
+                    "details": "NAT Pool Name, natpool1..31",
+                    "key": "name",
                     "objectType": "object",
                     "optionType": [
                         "constant",
-                        "ignore"
+                        "variable"
                     ]
                 },
                 {
-                    "dataPath": [
-                        "zscaler-location-settings",
-                        "datacenters"
-                    ],
+                    "dataPath": [],
                     "dataType": {
-                        "default": "Auto",
-                        "type": "string"
+                        "max": 32,
+                        "min": 1,
+                        "type": "number"
                     },
-                    "defaultOption": "ignore",
-                    "description": "Primary Data-Center",
-                    "details": "Custom Primary Datacenter",
-                    "key": "primary-data-center",
+                    "defaultOption": "constant",
+                    "description": "NAT Pool Prefix Length",
+                    "details": "Ending IP address of NAT Pool Prefix Length",
+                    "key": "prefix-length",
                     "objectType": "object",
                     "optionType": [
                         "constant",
-                        "ignore",
                         "variable"
                     ]
                 },
                 {
-                    "dataPath": [
-                        "zscaler-location-settings",
-                        "datacenters"
-                    ],
+                    "dataPath": [],
                     "dataType": {
-                        "default": "Auto",
-                        "type": "string"
+                        "type": "ipv4"
                     },
-                    "defaultOption": "ignore",
-                    "description": "Secondary Data-Center",
-                    "details": "Custom Secondary Datacenter",
-                    "key": "secondary-data-center",
+                    "defaultOption": "constant",
+                    "description": "NAT Pool Range Start",
+                    "details": "Starting IP address of NAT pool range",
+                    "key": "range-start",
                     "objectType": "object",
                     "optionType": [
                         "constant",
-                        "ignore",
                         "variable"
                     ]
                 },
                 {
-                    "dataPath": [
-                        "zscaler-location-settings",
-                        "surrogate"
-                    ],
+                    "dataPath": [],
                     "dataType": {
-                        "default": "false",
+                        "type": "ipv4"
+                    },
+                    "defaultOption": "constant",
+                    "description": "NAT Pool Range End",
+                    "details": "Ending IP address of NAT pool range",
+                    "key": "range-end",
+                    "objectType": "object",
+                    "optionType": [
+                        "constant",
+                        "variable"
+                    ]
+                },
+                {
+                    "dataPath": [],
+                    "dataType": {
+                        "default": "true",
                         "type": "boolean"
                     },
                     "defaultOption": "ignore",
-                    "description": "Enable Surrogate IP",
-                    "details": "Enable Surrogate IP",
-                    "key": "ip",
+                    "description": "NAT Overload",
+                    "details": "Enable port translation(PAT)",
+                    "key": "overload",
                     "objectType": "object",
                     "optionType": [
                         "constant",
+                        "variable",
                         "ignore"
                     ]
                 },
                 {
-                    "dataPath": [
-                        "zscaler-location-settings",
-                        "surrogate"
-                    ],
+                    "dataPath": [],
                     "dataType": {
-                        "default": 0,
-                        "max:": 4294967296,
-                        "min": 0,
+                        "type": "enum",
+                        "values": [
+                            {
+                                "key": "inside",
+                                "value": "Inside"
+                            },
+                            {
+                                "key": "outside",
+                                "value": "Outside"
+                            }
+                        ]
+                    },
+                    "defaultOption": "constant",
+                    "description": "NAT Direction",
+                    "details": "Direction of NAT translation",
+                    "key": "direction",
+                    "objectType": "object",
+                    "optionType": [
+                        "constant",
+                        "variable"
+                    ]
+                },
+                {
+                    "dataPath": [],
+                    "dataType": {
+                        "max": 1000,
+                        "min": 1,
                         "type": "number"
                     },
                     "defaultOption": "ignore",
-                    "description": "Idle Time to Disassociation",
-                    "details": "Idle time to disassociation",
-                    "key": "idle-time",
+                    "description": "Add Object/Object Group Tracker",
+                    "details": "Add Object/Object Group Tracker",
+                    "key": "tracker-id",
                     "objectType": "object",
                     "optionType": [
                         "constant",
+                        "variable",
+                        "ignore"
+                    ]
+                }
+            ],
+            "dataPath": [
+                "nat"
+            ],
+            "defaultOption": "ignore",
+            "description": "NAT Pool",
+            "details": "Configure NAT Pool entries",
+            "key": "natpool",
+            "objectType": "tree",
+            "optionType": [
+                "constant",
+                "variable",
+                "ignore"
+            ],
+            "primaryKeys": [
+                "name"
+            ]
+        },
+        {
+            "children": [
+                {
+                    "dataPath": [],
+                    "dataType": {
+                        "type": "enum",
+                        "values": []
+                    },
+                    "defaultOption": "ignore",
+                    "description": "NAT Pool Name",
+                    "details": "NAT Pool Name, natpool1..31",
+                    "key": "pool-name",
+                    "objectType": "object",
+                    "optionType": [
+                        "constant",
+                        "variable",
                         "ignore"
                     ]
                 },
                 {
-                    "dataPath": [
-                        "zscaler-location-settings",
-                        "surrogate"
-                    ],
+                    "dataPath": [],
+                    "dataType": {
+                        "type": "ipv4"
+                    },
+                    "defaultOption": "constant",
+                    "description": "Source IP Address",
+                    "details": "Source IP address to be translated",
+                    "key": "source-ip",
+                    "objectType": "object",
+                    "optionType": [
+                        "constant",
+                        "variable"
+                    ]
+                },
+                {
+                    "dataPath": [],
+                    "dataType": {
+                        "type": "ipv4"
+                    },
+                    "defaultOption": "constant",
+                    "description": "Translated Source IP Address",
+                    "details": "Statically translated source IP address",
+                    "key": "translate-ip",
+                    "objectType": "object",
+                    "optionType": [
+                        "constant",
+                        "variable"
+                    ]
+                },
+                {
+                    "dataPath": [],
                     "dataType": {
-                        "default": "MINUTE",
                         "type": "enum",
                         "values": [
                             {
-                                "key": "MINUTE",
-                                "value": "MINUTE"
+                                "key": "inside",
+                                "value": "Inside"
                             },
                             {
-                                "key": "HOUR",
-                                "value": "HOUR"
-                            },
-                            {
-                                "key": "DAY",
-                                "value": "DAY"
+                                "key": "outside",
+                                "value": "Outside"
                             }
                         ]
                     },
-                    "defaultOption": "ignore",
-                    "description": "Display Time Unit",
-                    "details": "Display time unit",
-                    "key": "display-time-unit",
+                    "defaultOption": "constant",
+                    "description": "Static NAT Direction",
+                    "details": "Direction of static NAT translation",
+                    "key": "static-nat-direction",
                     "objectType": "object",
                     "optionType": [
                         "constant",
-                        "ignore"
+                        "variable"
                     ]
                 },
                 {
-                    "dataPath": [
-                        "zscaler-location-settings",
-                        "surrogate"
-                    ],
+                    "dataPath": [],
                     "dataType": {
-                        "default": "false",
-                        "type": "boolean"
+                        "max": 1000,
+                        "min": 1,
+                        "type": "number"
                     },
                     "defaultOption": "ignore",
-                    "description": "Enforce Surrogate IP for known browsers",
-                    "details": "Enforce Surrogate IP for known browsers",
-                    "key": "ip-enforced-for-known-browsers",
+                    "description": "Add Object/Object Group Tracker",
+                    "details": "Add Object/Object Group Tracker",
+                    "key": "tracker-id",
                     "objectType": "object",
                     "optionType": [
                         "constant",
+                        "variable",
                         "ignore"
                     ]
+                }
+            ],
+            "dataPath": [
+                "nat"
+            ],
+            "defaultOption": "ignore",
+            "description": "Static NAT Rules",
+            "details": "Configure static NAT entries",
+            "key": "static",
+            "objectType": "tree",
+            "optionType": [
+                "constant",
+                "variable",
+                "ignore"
+            ],
+            "primaryKeys": [
+                "source-ip",
+                "translate-ip"
+            ]
+        },
+        {
+            "children": [
+                {
+                    "dataPath": [],
+                    "dataType": {
+                        "type": "ipv4"
+                    },
+                    "defaultOption": "constant",
+                    "description": "Source IP Subnet",
+                    "details": "Source IP Subnet to be translated",
+                    "key": "source-ip-subnet",
+                    "objectType": "object",
+                    "optionType": [
+                        "constant",
+                        "variable"
+                    ]
                 },
                 {
-                    "dataPath": [
-                        "zscaler-location-settings",
-                        "surrogate"
-                    ],
+                    "dataPath": [],
                     "dataType": {
-                        "default": 0,
-                        "max:": 4294967296,
-                        "min": 0,
+                        "type": "ipv4"
+                    },
+                    "defaultOption": "constant",
+                    "description": "Translated Source IP Subnet",
+                    "details": "Statically translated source IP Subnet",
+                    "key": "translate-ip-subnet",
+                    "objectType": "object",
+                    "optionType": [
+                        "constant",
+                        "variable"
+                    ]
+                },
+                {
+                    "dataPath": [],
+                    "dataType": {
+                        "max": 32,
+                        "min": 1,
                         "type": "number"
                     },
-                    "defaultOption": "ignore",
-                    "description": "Refresh Time",
-                    "details": "Refresh time for re-validation of surrogacy in minutes",
-                    "key": "refresh-time",
+                    "defaultOption": "constant",
+                    "description": "Network Prefix Length",
+                    "details": "Network Prefix Length",
+                    "key": "prefix-length",
                     "objectType": "object",
                     "optionType": [
                         "constant",
-                        "ignore"
+                        "variable"
                     ]
                 },
                 {
-                    "dataPath": [
-                        "zscaler-location-settings",
-                        "surrogate"
-                    ],
+                    "dataPath": [],
                     "dataType": {
-                        "default": "MINUTE",
                         "type": "enum",
                         "values": [
                             {
-                                "key": "MINUTE",
-                                "value": "MINUTE"
-                            },
-                            {
-                                "key": "HOUR",
-                                "value": "HOUR"
+                                "key": "inside",
+                                "value": "Inside"
                             },
                             {
-                                "key": "DAY",
-                                "value": "DAY"
+                                "key": "outside",
+                                "value": "Outside"
                             }
                         ]
                     },
-                    "defaultOption": "ignore",
-                    "description": "Refresh Time Unit",
-                    "details": "Refresh Time unit",
-                    "key": "refresh-time-unit",
+                    "defaultOption": "constant",
+                    "description": "Static NAT Direction",
+                    "details": "Direction of static NAT translation",
+                    "key": "static-nat-direction",
                     "objectType": "object",
                     "optionType": [
                         "constant",
-                        "ignore"
+                        "variable"
                     ]
                 },
                 {
-                    "dataPath": [
-                        "zscaler-location-settings",
-                        "aup"
-                    ],
+                    "dataPath": [],
                     "dataType": {
-                        "default": "false",
-                        "type": "boolean"
+                        "max": 1000,
+                        "min": 1,
+                        "type": "number"
                     },
                     "defaultOption": "ignore",
-                    "description": "Enable AUP",
-                    "details": "Enable Acceptable User Policy",
-                    "key": "enabled",
+                    "description": "Add Object/Object Group Tracker",
+                    "details": "Add Object/Object Group Tracker",
+                    "key": "tracker-id",
                     "objectType": "object",
                     "optionType": [
                         "constant",
+                        "variable",
                         "ignore"
                     ]
-                },
+                }
+            ],
+            "dataPath": [
+                "nat"
+            ],
+            "defaultOption": "ignore",
+            "description": "Static NAT Subnet Rules",
+            "details": "Configure static NAT Subnet entries",
+            "key": "subnet-static",
+            "objectType": "tree",
+            "optionType": [
+                "constant",
+                "variable",
+                "ignore"
+            ],
+            "primaryKeys": [
+                "source-ip-subnet",
+                "translate-ip-subnet"
+            ]
+        },
+        {
+            "children": [
                 {
-                    "dataPath": [
-                        "zscaler-location-settings",
-                        "aup"
-                    ],
+                    "dataPath": [],
                     "dataType": {
-                        "default": "false",
-                        "type": "boolean"
+                        "type": "enum",
+                        "values": []
                     },
                     "defaultOption": "ignore",
-                    "description": "First Time AUP Block Internet Access",
-                    "details": "For first-time Acceptable User Policy behavior, block Internet access",
-                    "key": "block-internet-until-accepted",
+                    "description": "NAT Pool Name",
+                    "details": "NAT Pool Name, natpool1..31",
+                    "key": "pool-name",
                     "objectType": "object",
                     "optionType": [
                         "constant",
+                        "variable",
                         "ignore"
                     ]
                 },
                 {
-                    "dataPath": [
-                        "zscaler-location-settings",
-                        "aup"
-                    ],
+                    "dataPath": [],
                     "dataType": {
-                        "default": "false",
-                        "type": "boolean"
+                        "default": 0,
+                        "type": "number"
                     },
-                    "defaultOption": "ignore",
-                    "description": "Force SSL Inspection",
-                    "details": "For first-time Acceptable User Policy behavior, force SSL inspection",
-                    "key": "force-ssl-inspection",
+                    "defaultOption": "constant",
+                    "description": "Source Port",
+                    "details": "Source Port",
+                    "key": "source-port",
                     "objectType": "object",
                     "optionType": [
                         "constant",
-                        "ignore"
+                        "variable"
                     ]
                 },
                 {
-                    "dataPath": [
-                        "zscaler-location-settings",
-                        "aup"
-                    ],
+                    "dataPath": [],
                     "dataType": {
                         "default": 0,
                         "type": "number"
                     },
-                    "defaultOption": "ignore",
-                    "description": "AUP Frequency",
-                    "details": "Custom Acceptable User Policy frequency in days",
-                    "key": "timeout",
+                    "defaultOption": "constant",
+                    "description": "Translate Port",
+                    "details": "Translate Port",
+                    "key": "translate-port",
                     "objectType": "object",
                     "optionType": [
                         "constant",
-                        "ignore"
+                        "variable"
                     ]
                 },
                 {
-                    "dataPath": [
-                        "zscaler-location-settings"
-                    ],
+                    "dataPath": [],
                     "dataType": {
-                        "default": "Auto",
-                        "type": "string"
+                        "type": "ipv4"
                     },
-                    "defaultOption": "ignore",
-                    "description": "Zscaler Location Name",
-                    "details": "Zscaler location name (optional)",
-                    "key": "location-name",
+                    "defaultOption": "constant",
+                    "description": "Source IP Address",
+                    "details": "Source IP address to be translated",
+                    "key": "source-ip",
                     "objectType": "object",
                     "optionType": [
-                        "ignore",
+                        "constant",
                         "variable"
                     ]
                 },
                 {
-                    "dataPath": [
-                        "umbrella-data-center"
-                    ],
+                    "dataPath": [],
                     "dataType": {
-                        "default": "Auto",
-                        "type": "string"
+                        "type": "ipv4"
                     },
-                    "defaultOption": "ignore",
-                    "description": "Umbrella Primary Data-Center",
-                    "details": "Umbrella Primary Datacenter",
-                    "key": "data-center-primary",
+                    "defaultOption": "constant",
+                    "description": "Translated Source IP Address",
+                    "details": "Statically translated source IP address",
+                    "key": "translate-ip",
                     "objectType": "object",
                     "optionType": [
                         "constant",
-                        "ignore",
                         "variable"
                     ]
                 },
                 {
-                    "dataPath": [
-                        "umbrella-data-center"
-                    ],
+                    "dataPath": [],
                     "dataType": {
-                        "default": "Auto",
-                        "type": "string"
+                        "type": "enum",
+                        "values": [
+                            {
+                                "key": "tcp",
+                                "value": "TCP"
+                            },
+                            {
+                                "key": "udp",
+                                "value": "UDP"
+                            }
+                        ]
                     },
-                    "defaultOption": "ignore",
-                    "description": "Umbrella Secondary Data-Center",
-                    "details": "Umbrella Secondary Datacenter",
-                    "key": "data-center-secondary",
+                    "defaultOption": "constant",
+                    "description": "Protocol",
+                    "details": "Protocol",
+                    "key": "proto",
                     "objectType": "object",
                     "optionType": [
                         "constant",
-                        "ignore",
                         "variable"
                     ]
                 }
             ],
-            "dataPath": [],
-            "defaultOption": "constant",
-            "description": "Service",
-            "details": "Configure services",
-            "key": "service",
+            "dataPath": [
+                "nat"
+            ],
+            "defaultOption": "ignore",
+            "description": "Port Forward",
+            "details": "Configure Port Forward entries",
+            "key": "port-forward",
             "objectType": "tree",
             "optionType": [
-                "constant"
+                "constant",
+                "variable",
+                "ignore"
             ],
             "primaryKeys": [
-                "svc-type"
+                "source-port",
+                "translate-port",
+                "source-ip",
+                "translate-ip",
+                "proto"
             ]
         },
         {
+            "children": [
+                {
+                    "dataPath": [],
+                    "dataType": {
+                        "type": "enum",
+                        "values": [
+                            {
+                                "key": "static",
+                                "value": "static"
+                            },
+                            {
+                                "key": "connected",
+                                "value": "connected"
+                            },
+                            {
+                                "key": "bgp",
+                                "value": "bgp"
+                            },
+                            {
+                                "key": "ospf",
+                                "value": "ospf"
+                            }
+                        ]
+                    },
+                    "defaultOption": "constant",
+                    "description": "Route Protocol Leak from Global to Service",
+                    "details": "Select a Route Protocol to enable route leaking from Global VPN to this Service VPN",
+                    "key": "protocol",
+                    "objectType": "object",
+                    "optionType": [
+                        "constant",
+                        "variable"
+                    ]
+                },
+                {
+                    "dataPath": [],
+                    "dataType": {
+                        "default": "external",
+                        "type": "enum",
+                        "values": [
+                            {
+                                "key": "external",
+                                "value": "external"
+                            }
+                        ]
+                    },
+                    "defaultOption": "constant",
+                    "key": "protocol-sub-type",
+                    "minElements": 1,
+                    "objectType": "list",
+                    "optionType": [
+                        "constant",
+                        "variable"
+                    ]
+                },
+                {
+                    "dataPath": [],
+                    "dataType": {
+                        "default": "",
+                        "type": "enum",
+                        "values": []
+                    },
+                    "defaultOption": "ignore",
+                    "description": "Route Policy Leak from Global to Service",
+                    "details": "Select a Route Policy to enable route leaking from Global VPN to this Service VPN",
+                    "key": "route-policy",
+                    "objectType": "object",
+                    "optionType": [
+                        "constant",
+                        "ignore"
+                    ]
+                },
+                {
+                    "children": [
+                        {
+                            "dataPath": [],
+                            "dataType": {
+                                "type": "enum",
+                                "values": [
+                                    {
+                                        "key": "bgp",
+                                        "value": "bgp"
+                                    },
+                                    {
+                                        "key": "eigrp",
+                                        "value": "eigrp"
+                                    },
+                                    {
+                                        "key": "ospf",
+                                        "value": "ospf"
+                                    }
+                                ]
+                            },
+                            "defaultOption": "constant",
+                            "description": "Protocol",
+                            "details": "Select a Route Protocol to enable redistribution",
+                            "key": "protocol",
+                            "objectType": "object",
+                            "optionType": [
+                                "constant",
+                                "variable"
+                            ]
+                        },
+                        {
+                            "dataPath": [],
+                            "dataType": {
+                                "default": "",
+                                "type": "enum",
+                                "values": []
+                            },
+                            "defaultOption": "ignore",
+                            "description": "Redistribution Policy",
+                            "details": "Select a Route Policy to enable redistribution",
+                            "key": "route-policy",
+                            "objectType": "object",
+                            "optionType": [
+                                "constant",
+                                "ignore"
+                            ]
+                        }
+                    ],
+                    "dataPath": [],
+                    "defaultOption": "ignore",
+                    "description": "Redistribute To Protocol",
+                    "details": "Enable redistribution of replicated route protocol",
+                    "key": "redistribute",
+                    "objectType": "tree",
+                    "optionType": [
+                        "constant",
+                        "variable",
+                        "ignore"
+                    ],
+                    "primaryKeys": [
+                        "protocol"
+                    ]
+                }
+            ],
             "dataPath": [],
-            "dataType": {
-                "type": "ipv4-prefix"
-            },
-            "defaultOption": "constant",
-            "description": "Source IP Address",
-            "details": "Source IP address for Tracker",
-            "key": "tracker-src-ip",
-            "objectType": "object",
+            "defaultOption": "ignore",
+            "description": "Enable route leaking from Global VPN",
+            "details": "Enable route leaking from Global VPN to this Service VPN",
+            "key": "route-import",
+            "objectType": "tree",
             "optionType": [
                 "constant",
-                "variable"
+                "variable",
+                "ignore"
+            ],
+            "primaryKeys": [
+                "protocol"
             ]
         },
         {
             "children": [
                 {
                     "dataPath": [],
                     "dataType": {
-                        "maxLength": 128,
-                        "minLength": 1,
-                        "type": "string"
+                        "default": 1,
+                        "max": 65530,
+                        "min": 1,
+                        "type": "number"
                     },
                     "defaultOption": "constant",
-                    "description": "Name",
-                    "details": "Tracker name",
-                    "key": "name",
+                    "description": "Source VPN",
+                    "details": "Select a Source VPN where route leaks from",
+                    "key": "source-vpn",
                     "objectType": "object",
                     "optionType": [
-                        "constant"
+                        "constant",
+                        "variable"
                     ]
                 },
                 {
                     "dataPath": [],
                     "dataType": {
-                        "maxLength": 512,
-                        "minLength": 0,
-                        "type": "string"
+                        "type": "enum",
+                        "values": [
+                            {
+                                "key": "static",
+                                "value": "static"
+                            },
+                            {
+                                "key": "connected",
+                                "value": "connected"
+                            },
+                            {
+                                "key": "bgp",
+                                "value": "bgp"
+                            },
+                            {
+                                "key": "ospf",
+                                "value": "ospf"
+                            },
+                            {
+                                "key": "eigrp",
+                                "value": "eigrp"
+                            }
+                        ]
                     },
                     "defaultOption": "constant",
-                    "description": "API url of endpoint",
-                    "details": "API url of endpoint",
-                    "key": "endpoint-api-url",
+                    "description": "Route Protocol Leak to Current VPN",
+                    "details": "Select a Route Protocol to enable route leaking to current VPN",
+                    "key": "protocol",
                     "objectType": "object",
                     "optionType": [
                         "constant",
                         "variable"
                     ]
                 },
                 {
                     "dataPath": [],
                     "dataType": {
-                        "default": 300,
-                        "max": 1000,
-                        "min": 100,
-                        "type": "number"
+                        "default": "external",
+                        "type": "enum",
+                        "values": [
+                            {
+                                "key": "external",
+                                "value": "external"
+                            }
+                        ]
                     },
-                    "defaultOption": "ignore",
-                    "description": "Threshold",
-                    "details": "Probe Timeout threshold <100..1000> milliseconds",
-                    "key": "threshold",
-                    "objectType": "object",
+                    "defaultOption": "constant",
+                    "key": "protocol-sub-type",
+                    "minElements": 1,
+                    "objectType": "list",
                     "optionType": [
                         "constant",
-                        "variable",
-                        "ignore"
+                        "variable"
                     ]
                 },
                 {
                     "dataPath": [],
                     "dataType": {
-                        "default": 60,
-                        "max": 600,
-                        "min": 20,
-                        "type": "number"
+                        "default": "",
+                        "type": "enum",
+                        "values": []
                     },
                     "defaultOption": "ignore",
-                    "description": "Interval",
-                    "details": "Probe interval <10..600> seconds",
-                    "key": "interval",
+                    "description": "Route Policy Leak to Current VPN",
+                    "details": "Select a Route Policy to enable route leaking to current VPN",
+                    "key": "route-policy",
                     "objectType": "object",
                     "optionType": [
                         "constant",
+                        "ignore",
+                        "variable"
+                    ]
+                },
+                {
+                    "children": [
+                        {
+                            "dataPath": [],
+                            "dataType": {
+                                "type": "enum",
+                                "values": [
+                                    {
+                                        "key": "bgp",
+                                        "value": "bgp"
+                                    },
+                                    {
+                                        "key": "eigrp",
+                                        "value": "eigrp"
+                                    },
+                                    {
+                                        "key": "ospf",
+                                        "value": "ospf"
+                                    }
+                                ]
+                            },
+                            "defaultOption": "constant",
+                            "description": "Protocol",
+                            "details": "Select a Route Protocol to enable redistribution",
+                            "key": "protocol",
+                            "objectType": "object",
+                            "optionType": [
+                                "constant",
+                                "variable"
+                            ]
+                        },
+                        {
+                            "dataPath": [],
+                            "dataType": {
+                                "default": "",
+                                "type": "enum",
+                                "values": []
+                            },
+                            "defaultOption": "ignore",
+                            "description": "Redistribution Policy",
+                            "details": "Select a Route Policy to enable redistribution",
+                            "key": "route-policy",
+                            "objectType": "object",
+                            "optionType": [
+                                "constant",
+                                "ignore",
+                                "variable"
+                            ]
+                        }
+                    ],
+                    "dataPath": [],
+                    "defaultOption": "ignore",
+                    "description": "Redistribute To Protocol",
+                    "details": "Enable redistribution of replicated route protocol",
+                    "key": "redistribute",
+                    "objectType": "tree",
+                    "optionType": [
+                        "constant",
                         "variable",
                         "ignore"
+                    ],
+                    "primaryKeys": [
+                        "protocol"
                     ]
-                },
+                }
+            ],
+            "dataPath": [],
+            "defaultOption": "ignore",
+            "description": "Enable inter-service VPN route leak",
+            "details": "Enable route leak from Service VPN to current VPN",
+            "key": "route-import-from",
+            "objectType": "tree",
+            "optionType": [
+                "constant",
+                "variable",
+                "ignore"
+            ],
+            "primaryKeys": [
+                "source-vpn",
+                "protocol"
+            ]
+        },
+        {
+            "children": [
                 {
                     "dataPath": [],
                     "dataType": {
-                        "default": 3,
-                        "max": 10,
-                        "min": 1,
-                        "type": "number"
+                        "type": "enum",
+                        "values": [
+                            {
+                                "key": "static",
+                                "value": "static"
+                            },
+                            {
+                                "key": "connected",
+                                "value": "connected"
+                            },
+                            {
+                                "key": "bgp",
+                                "value": "bgp"
+                            },
+                            {
+                                "key": "eigrp",
+                                "value": "eigrp"
+                            },
+                            {
+                                "key": "ospf",
+                                "value": "ospf"
+                            }
+                        ]
                     },
-                    "defaultOption": "ignore",
-                    "description": "Multiplier",
-                    "details": "Probe failure multiplier <1..10> failed attempts",
-                    "key": "multiplier",
+                    "defaultOption": "constant",
+                    "description": "Route Protocol Leak from Service to Global",
+                    "details": "Select a Route Protocol to enable route leaking from this Service VPN to Global VPN",
+                    "key": "protocol",
                     "objectType": "object",
                     "optionType": [
                         "constant",
-                        "variable",
-                        "ignore"
+                        "variable"
                     ]
                 },
                 {
                     "dataPath": [],
                     "dataType": {
-                        "default": " SIG",
+                        "default": "external",
                         "type": "enum",
                         "values": [
                             {
-                                "key": "SIG",
-                                "value": "SIG"
+                                "key": "external",
+                                "value": "external"
                             }
                         ]
                     },
                     "defaultOption": "constant",
-                    "description": "Tracker Type",
-                    "details": "",
-                    "key": "tracker-type",
+                    "key": "protocol-sub-type",
+                    "minElements": 1,
+                    "objectType": "list",
+                    "optionType": [
+                        "constant",
+                        "variable"
+                    ]
+                },
+                {
+                    "dataPath": [],
+                    "dataType": {
+                        "default": "",
+                        "type": "enum",
+                        "values": []
+                    },
+                    "defaultOption": "ignore",
+                    "description": "Route Policy Leak from Service to Global",
+                    "details": "Select a Route Policy to enable route leaking from this Service VPN to Global VPN",
+                    "key": "route-policy",
                     "objectType": "object",
                     "optionType": [
-                        "constant"
+                        "constant",
+                        "ignore"
+                    ]
+                },
+                {
+                    "children": [
+                        {
+                            "dataPath": [],
+                            "dataType": {
+                                "type": "enum",
+                                "values": [
+                                    {
+                                        "key": "bgp",
+                                        "value": "bgp"
+                                    },
+                                    {
+                                        "key": "ospf",
+                                        "value": "ospf"
+                                    }
+                                ]
+                            },
+                            "defaultOption": "constant",
+                            "description": "Protocol",
+                            "details": "Select a Route Protocol to enable redistribution",
+                            "key": "protocol",
+                            "objectType": "object",
+                            "optionType": [
+                                "constant",
+                                "variable"
+                            ]
+                        },
+                        {
+                            "dataPath": [],
+                            "dataType": {
+                                "default": "",
+                                "type": "enum",
+                                "values": []
+                            },
+                            "defaultOption": "ignore",
+                            "description": "Redistribution Policy",
+                            "details": "Select a Route Policy to enable redistribution",
+                            "key": "route-policy",
+                            "objectType": "object",
+                            "optionType": [
+                                "constant",
+                                "ignore"
+                            ]
+                        }
+                    ],
+                    "dataPath": [],
+                    "defaultOption": "ignore",
+                    "description": "Redistribute To Protocol",
+                    "details": "Enable redistribution of replicated route protocol",
+                    "key": "redistribute",
+                    "objectType": "tree",
+                    "optionType": [
+                        "constant",
+                        "variable",
+                        "ignore"
+                    ],
+                    "primaryKeys": [
+                        "protocol"
                     ]
                 }
             ],
             "dataPath": [],
             "defaultOption": "ignore",
-            "description": "Tracker",
-            "details": "Tracker configuration",
-            "key": "tracker",
+            "description": "Enable route leaking to Global VPN",
+            "details": "Enable route leaking to Global VPN from this Service VPN",
+            "key": "route-export",
             "objectType": "tree",
             "optionType": [
                 "constant",
+                "variable",
                 "ignore"
             ],
             "primaryKeys": [
-                "tracker-type",
-                "name"
+                "protocol"
             ]
         }
     ],
-    "name": "cisco_secure_internet_gateway",
+    "name": "cisco_vpn",
     "nameSpace": "http://viptela.com/vpn",
     "uniqueKey": "vpn-id",
     "xmlPath": [
         "vpn"
     ],
     "xmlRootTag": "vpn-instance"
 }
```

### Comparing `catalystwan-0.33.6.post0/catalystwan/tests/templates/schemas/cisco_system.json` & `catalystwan-0.33.7/catalystwan/tests/templates/schemas/cisco_system.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9844444444444445%*

 * *Differences: {"'fields'": '{delete: [44, 43, 42, 41, 37, 36, 15]}'}*

```diff
@@ -1968,60 +1968,14 @@
                 "constant",
                 "variable"
             ]
         },
         {
             "dataPath": [],
             "dataType": {
-                "type": "enum",
-                "values": [
-                    {
-                        "key": "type-1",
-                        "value": "type-1"
-                    },
-                    {
-                        "key": "type-2",
-                        "value": "type-2"
-                    },
-                    {
-                        "key": "type-3",
-                        "value": "type-3"
-                    },
-                    {
-                        "key": "cloud",
-                        "value": "cloud"
-                    },
-                    {
-                        "key": "branch",
-                        "value": "branch"
-                    },
-                    {
-                        "key": "br",
-                        "value": "br"
-                    },
-                    {
-                        "key": "spoke",
-                        "value": "spoke"
-                    }
-                ]
-            },
-            "defaultOption": "ignore",
-            "description": "Site Type",
-            "details": "Configure site type",
-            "key": "site-type",
-            "objectType": "list",
-            "optionType": [
-                "constant",
-                "ignore",
-                "variable"
-            ]
-        },
-        {
-            "dataPath": [],
-            "dataType": {
                 "default": 0,
                 "max": 19,
                 "min": 0,
                 "type": "number"
             },
             "defaultOption": "ignore",
             "description": "Port Offset",
@@ -2833,86 +2787,14 @@
             "optionType": [
                 "constant",
                 "variable",
                 "ignore"
             ]
         },
         {
-            "dataPath": [
-                "affinity-group"
-            ],
-            "dataType": {
-                "default": "false",
-                "type": "boolean"
-            },
-            "defaultOption": "ignore",
-            "description": "Affinity Group Preference Auto",
-            "details": "Enable affinity preference auto flag",
-            "key": "preference-auto",
-            "objectType": "object",
-            "optionType": [
-                "constant",
-                "variable",
-                "ignore"
-            ]
-        },
-        {
-            "children": [
-                {
-                    "dataPath": [],
-                    "dataType": {
-                        "max": 63,
-                        "min": 1,
-                        "type": "number"
-                    },
-                    "defaultOption": "ignore",
-                    "description": "Affinity Group Number",
-                    "details": "Router affinity group number",
-                    "key": "affinity-group-number",
-                    "objectType": "object",
-                    "optionType": [
-                        "constant",
-                        "ignore"
-                    ]
-                },
-                {
-                    "dataPath": [],
-                    "dataType": {
-                        "maxLength": 11,
-                        "minLength": 1,
-                        "type": "string"
-                    },
-                    "defaultOption": "ignore",
-                    "description": "VRFs",
-                    "details": "Range of VRFs",
-                    "key": "vrf-range",
-                    "objectType": "object",
-                    "optionType": [
-                        "constant",
-                        "ignore"
-                    ]
-                }
-            ],
-            "dataPath": [
-                "affinity-group"
-            ],
-            "defaultOption": "ignore",
-            "description": "Affinity Group Number for VRFs",
-            "details": "Set Affinity per VRF",
-            "key": "affinity-per-vrf",
-            "objectType": "tree",
-            "optionType": [
-                "constant",
-                "ignore"
-            ],
-            "primaryKeys": [
-                "affinity-group-number"
-            ]
-        },
-        {
             "dataPath": [],
             "dataType": {
                 "default": "false",
                 "type": "boolean"
             },
             "defaultOption": "ignore",
             "description": "Transport Gateway",
@@ -2962,138 +2844,14 @@
             "details": "Set BGP community during migration from BGP-core based network",
             "key": "migration-bgp-community",
             "objectType": "object",
             "optionType": [
                 "constant",
                 "ignore"
             ]
-        },
-        {
-            "dataPath": [],
-            "dataType": {
-                "default": "false",
-                "type": "boolean"
-            },
-            "defaultOption": "ignore",
-            "description": "Management Region",
-            "details": "Enable Management Region",
-            "key": "enable-management-region",
-            "objectType": "object",
-            "optionType": [
-                "constant",
-                "ignore",
-                "variable"
-            ]
-        },
-        {
-            "children": [
-                {
-                    "dataPath": [],
-                    "dataType": {
-                        "max": 65531,
-                        "min": 0,
-                        "type": "number"
-                    },
-                    "defaultOption": "constant",
-                    "description": "VRF ID",
-                    "details": "VRF ID for management region",
-                    "key": "vrf-id",
-                    "objectType": "object",
-                    "optionType": [
-                        "constant",
-                        "variable"
-                    ]
-                },
-                {
-                    "dataPath": [],
-                    "dataType": {
-                        "max": 63,
-                        "min": 1,
-                        "type": "number"
-                    },
-                    "defaultOption": "ignore",
-                    "description": "List of affinity group preferences for VRF",
-                    "details": "List of affinity group preferences for VRF",
-                    "key": "gateway-preference",
-                    "objectType": "list",
-                    "optionType": [
-                        "constant",
-                        "variable",
-                        "ignore"
-                    ]
-                }
-            ],
-            "dataPath": [
-                "management-region"
-            ],
-            "defaultOption": "ignore",
-            "description": "VRF Name",
-            "details": "VRF Name for Management Region",
-            "key": "vrf",
-            "maxElements": 1,
-            "objectType": "tree",
-            "optionType": [
-                "constant",
-                "ignore"
-            ],
-            "primaryKeys": [
-                "vrf-id"
-            ]
-        },
-        {
-            "dataPath": [],
-            "dataType": {
-                "default": "false",
-                "type": "boolean"
-            },
-            "defaultOption": "ignore",
-            "description": "Management Gateway",
-            "details": "Enable Management Gateway",
-            "key": "management-gateway",
-            "objectType": "object",
-            "optionType": [
-                "constant",
-                "ignore",
-                "variable"
-            ]
-        },
-        {
-            "dataPath": [],
-            "dataType": {
-                "default": "disabled",
-                "type": "enum",
-                "values": [
-                    {
-                        "key": "disabled",
-                        "value": "Disabled"
-                    },
-                    {
-                        "key": "aggressive",
-                        "value": "Aggressive"
-                    },
-                    {
-                        "key": "moderate",
-                        "value": "Moderate"
-                    },
-                    {
-                        "key": "conservative",
-                        "value": "Conservative"
-                    }
-                ]
-            },
-            "defaultOption": "ignore",
-            "description": "Enhanced App-Aware Routing",
-            "details": "Enable SLA Dampening and Enhanced App-Aware Routing.",
-            "key": "epfr",
-            "objectType": "object",
-            "optionType": [
-                "constant",
-                "variable",
-                "ignore"
-            ]
         }
     ],
     "name": "cisco_system",
     "nameSpace": "http://viptela.com/system",
     "xmlPath": [],
     "xmlRootTag": "system"
 }
```

### Comparing `catalystwan-0.33.6.post0/catalystwan/tests/templates/test_deserialize_model.py` & `catalystwan-0.33.7/catalystwan/tests/templates/test_deserialize_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/tests/templates/test_find_template_values.py` & `catalystwan-0.33.7/catalystwan/tests/templates/test_find_template_values.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/tests/templates/test_generate_payload.py` & `catalystwan-0.33.7/catalystwan/tests/templates/test_generate_payload.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/tests/templates/test_serialize_model.py` & `catalystwan-0.33.7/catalystwan/tests/templates/test_serialize_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/tests/test_admin_tech_api.py` & `catalystwan-0.33.7/catalystwan/tests/test_admin_tech_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/tests/test_administration.py` & `catalystwan-0.33.7/catalystwan/tests/test_administration.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/tests/test_alarms_api.py` & `catalystwan-0.33.7/catalystwan/tests/test_alarms_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/tests/test_cli_template.py` & `catalystwan-0.33.7/catalystwan/tests/test_cli_template.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from urllib.error import HTTPError
 
 from ciscoconfparse import CiscoConfParse  # type: ignore
 
 from catalystwan.api.templates.cli_template import CLITemplate
 from catalystwan.dataclasses import Device
 from catalystwan.exceptions import TemplateTypeError
+from catalystwan.utils.device_model import DeviceModel
 
 
 class TestCLITemplate(unittest.TestCase):
     def setUp(self):
         self.config = """
         system\n
         host-name               host5\n
@@ -35,29 +36,29 @@
         self.template = CiscoConfParse(self.config.splitlines())
 
     @patch("catalystwan.session.ManagerSession")
     def test_load_success(self, mock_session):
         # Arrange
         mock_session.get_json.return_value = {"configType": "file", "templateConfiguration": self.config}
         # Act
-        temp = CLITemplate(template_name="test", template_description="test", device_model="vedge-cloud")
+        temp = CLITemplate(template_name="test", template_description="test", device_model=DeviceModel.VEDGE)
         answer = temp.load(session=mock_session, id="temp_id")
         # Assert
         self.assertEqual(answer.ioscfg, self.template.ioscfg)
 
     @patch("catalystwan.session.ManagerSession")
     def test_load_raise(self, mock_session):
         # Arrange
         mock_session.get_json.return_value = {
             "templateName": "test",
             "configType": "template",
             "templateConfiguration": self.config,
         }
         # Act
-        temp = CLITemplate(template_name="test", template_description="test", device_model="vedge-cloud")
+        temp = CLITemplate(template_name="test", template_description="test", device_model=DeviceModel.VEDGE)
 
         def answer():
             return temp.load(session=mock_session, id="temp_id")
 
         # Assert
         self.assertRaises(TemplateTypeError, answer)
 
@@ -74,23 +75,23 @@
             local_system_ip="mock_ip",
             status="normal",
             memUsage=1.0,
             connected_vManages=["192.168.0.1"],
             model="vedge-cloud",
         )
         # Act
-        temp = CLITemplate(template_name="test", template_description="test", device_model="vedge-cloud")
+        temp = CLITemplate(template_name="test", template_description="test", device_model=DeviceModel.VEDGE)
         answer = temp.load_running(session=mock_session, device=device)
         # Assert
         self.assertEqual(answer.ioscfg, self.template.ioscfg)
 
     def test_generate_payload(self):
         # Arrange
         template = CLITemplate(
-            template_name="test", template_description="test", device_model="vedge-cloud", config=self.template
+            template_name="test", template_description="test", device_model=DeviceModel.VEDGE, config=self.template
         )
         # Act
         answer = template.generate_payload()
         # Assert
         templateConfiguration = (
             "        system\n"
             "        host-name               host5\n"
@@ -121,15 +122,15 @@
         self.assertEqual(answer, proper_answer)
 
     def test_generate_payload_cedge(self):
         # Arrange
         template = CLITemplate(
             template_name="test",
             template_description="test",
-            device_model="vedge-C8000V",
+            device_model=DeviceModel.VEDGE_C8000V,
             config=self.template,
         )
         # Act
         answer = template.generate_payload()
         # Assert
         templateConfiguration = (
             "        system\n"
@@ -169,15 +170,15 @@
         templateConfiguration = (
             "        system\n"
             "        host-name               host6\n"
             "        system-ip               192.168.1.26\n"
         )
         config = CiscoConfParse(templateConfiguration.splitlines())
         # Act
-        template = CLITemplate(template_name="test", template_description="test", device_model="vedge-cloud")
+        template = CLITemplate(template_name="test", template_description="test", device_model=DeviceModel.VEDGE)
         result = template.update(session=mock_session, id="temp_id", config=config)
         # Assert
         self.assertTrue(result)
 
     @patch("catalystwan.session.ManagerSession")
     def test_update_template_failure(self, mock_session):
         # Arrange
@@ -186,15 +187,15 @@
 
         templateConfiguration = (
             "        system\n"
             "        host-name               host6\n"
             "        system-ip               192.168.1.26\n"
         )
         config = CiscoConfParse(templateConfiguration.splitlines())
-        template = CLITemplate(template_name="test", template_description="test", device_model="vedge-cloud")
+        template = CLITemplate(template_name="test", template_description="test", device_model=DeviceModel.VEDGE)
 
         # Act
         with self.assertRaises(HTTPError):
             template.update(session=mock_session, id="temp_id", config=config)
 
     def test_compare_template(self):
         # Arrange
@@ -208,11 +209,11 @@
             "        system\n"
             "        host-name               host6\n"
             "        system-ip               192.168.1.26\n"
         )
         config2 = CiscoConfParse(templateConfiguration2.splitlines())
         # Act
         result = CLITemplate(
-            template_name="test", template_description="test", device_model="vedge-cloud"
+            template_name="test", template_description="test", device_model=DeviceModel.VEDGE
         ).compare_template(config1, config2)
         # Assert
         self.assertEqual(result, "")
```

### Comparing `catalystwan-0.33.6.post0/catalystwan/tests/test_creation_tools.py` & `catalystwan-0.33.7/catalystwan/tests/test_creation_tools.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/tests/test_device_action_api.py` & `catalystwan-0.33.7/catalystwan/tests/test_device_action_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/tests/test_devices_api.py` & `catalystwan-0.33.7/catalystwan/tests/test_devices_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/tests/test_endpoints.py` & `catalystwan-0.33.7/catalystwan/tests/test_endpoints.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/tests/test_feature_template_field.py` & `catalystwan-0.33.7/catalystwan/tests/test_feature_template_field.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/tests/test_logs_api.py` & `catalystwan-0.33.7/catalystwan/tests/test_logs_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/tests/test_monitoring_security_policy.py` & `catalystwan-0.33.7/catalystwan/tests/test_monitoring_security_policy.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/tests/test_monitoring_server_info.py` & `catalystwan-0.33.7/catalystwan/tests/test_monitoring_server_info.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/tests/test_monitoring_status_api.py` & `catalystwan-0.33.7/catalystwan/tests/test_monitoring_status_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/tests/test_mtt_aaa_api.py` & `catalystwan-0.33.7/catalystwan/tests/test_mtt_aaa_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/tests/test_omp_api.py` & `catalystwan-0.33.7/catalystwan/tests/test_omp_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/tests/test_packet_capture.py` & `catalystwan-0.33.7/catalystwan/tests/test_packet_capture.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/tests/test_partition_manager_api.py` & `catalystwan-0.33.7/catalystwan/tests/test_partition_manager_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/tests/test_response.py` & `catalystwan-0.33.7/catalystwan/tests/test_response.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/tests/test_session.py` & `catalystwan-0.33.7/catalystwan/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/tests/test_software_action_api.py` & `catalystwan-0.33.7/catalystwan/tests/test_software_action_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/tests/test_speed_test_api.py` & `catalystwan-0.33.7/catalystwan/tests/test_speed_test_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/tests/test_task_status_api.py` & `catalystwan-0.33.7/catalystwan/tests/test_task_status_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/tests/test_templates.py` & `catalystwan-0.33.7/catalystwan/tests/test_templates.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from catalystwan.api.templates.device_template.device_template import DeviceTemplate
 from catalystwan.api.templates.feature_template import FeatureTemplate
 from catalystwan.api.templates.models.cisco_aaa_model import CiscoAAAModel
 from catalystwan.api.templates.payloads.aaa.aaa_model import AAAModel, AuthenticationOrder
 from catalystwan.dataclasses import Device, FeatureTemplateInfo, TemplateInfo
 from catalystwan.typed_list import DataSequence
 from catalystwan.utils.creation_tools import create_dataclass
+from catalystwan.utils.device_model import DeviceModel
 from catalystwan.utils.personality import Personality
 from catalystwan.utils.reachability import Reachability
 
 
 class TestTemplatesAPI(unittest.TestCase):
     def setUp(self):
         self.data_template = [
@@ -125,22 +126,22 @@
                 ),
                 "aaa_id",
             ),
             (
                 DeviceTemplate(  # type: ignore
                     template_name="test_device_template",
                     template_description="test_device_template_description",
-                    device_type="vedge-2000",
+                    device_type=DeviceModel.VEDGE_2000,
                     general_templates=[],
                 ),
                 "device_template_id",
             ),
             (
                 CLITemplate(  # type: ignore
-                    template_name="test", template_description="test", device_model="vedge-100"
+                    template_name="test", template_description="test", device_model=DeviceModel.VEDGE
                 ),
                 "cli_id",
             ),
             (
                 CiscoAAAModel(  # type: ignore
                     template_name="test_aaa_model",
                     template_description="test_aaa_description",
@@ -188,21 +189,21 @@
                         auth_disable_audit_logs=True,
                         auth_admin_order=True,
                         auth_disable_netconf_logs=False,
                     ),
                     DeviceTemplate(  # type: ignore
                         template_name="test_device_template",
                         template_description="test_device_template_description",
-                        device_type="vedge-2000",
+                        device_type=DeviceModel.VEDGE_2000,
                         general_templates=[],
                     ),
                     CLITemplate(  # type: ignore
                         template_name="test_cli_template",
                         template_description="test_cli_description",
-                        device_model="vedge-cloud",
+                        device_model=DeviceModel.VBOND,
                     ),
                     CiscoAAAModel(  # type: ignore
                         template_name="test_aaa_model",
                         template_description="test_aaa_description",
                     ),
                 ],
                 ["aaa_id", "device_template_id", "cli_id", "generator_id"],
```

### Comparing `catalystwan-0.33.6.post0/catalystwan/tests/test_tenant_backup_restore_api.py` & `catalystwan-0.33.7/catalystwan/tests/test_tenant_backup_restore_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/tests/test_tenant_management_api.py` & `catalystwan-0.33.7/catalystwan/tests/test_tenant_management_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/tests/test_tenant_migration_api.py` & `catalystwan-0.33.7/catalystwan/tests/test_tenant_migration_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/tests/test_typed_list.py` & `catalystwan-0.33.7/catalystwan/tests/test_typed_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/tests/test_url_monitoring.py` & `catalystwan-0.33.7/catalystwan/tests/test_url_monitoring.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/tests/test_version.py` & `catalystwan-0.33.7/catalystwan/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/tests/test_version_utils.py` & `catalystwan-0.33.7/catalystwan/tests/test_version_utils.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/tests/test_vmanage_auth.py` & `catalystwan-0.33.7/catalystwan/tests/test_vmanage_auth.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/typed_list.py` & `catalystwan-0.33.7/catalystwan/typed_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/utils/creation_tools.py` & `catalystwan-0.33.7/catalystwan/utils/creation_tools.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/utils/dashboard.py` & `catalystwan-0.33.7/catalystwan/utils/dashboard.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/utils/dict.py` & `catalystwan-0.33.7/catalystwan/utils/dict.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/utils/feature_template/choose_model.py` & `catalystwan-0.33.7/catalystwan/utils/feature_template/choose_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/utils/feature_template/find_template_values.py` & `catalystwan-0.33.7/catalystwan/utils/feature_template/find_template_values.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/utils/operation_status.py` & `catalystwan-0.33.7/catalystwan/utils/operation_status.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/utils/upgrades_helper.py` & `catalystwan-0.33.7/catalystwan/utils/upgrades_helper.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/version.py` & `catalystwan-0.33.7/catalystwan/version.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/vmanage_auth.py` & `catalystwan-0.33.7/catalystwan/vmanage_auth.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/catalystwan/workflows/tenant_migration.py` & `catalystwan-0.33.7/catalystwan/workflows/tenant_migration.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6.post0/pyproject.toml` & `catalystwan-0.33.7/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "catalystwan"
-version = "0.33.6post0"
+version = "0.33.7"
 description = "Cisco Catalyst WAN SDK for Python"
 authors = ["kagorski <kagorski@cisco.com>"]
 readme = "README.md"
 repository = "https://github.com/cisco-open/cisco-catalyst-wan-sdk"
 
 [tool.poetry.dependencies]
 python = "^3.8.0"
```

### Comparing `catalystwan-0.33.6.post0/setup.py` & `catalystwan-0.33.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,17 +66,17 @@
  'requests-toolbelt>=1.0.0,<2.0.0',
  'requests>=2.27.1,<3.0.0',
  'tenacity>=8.1.0,<9.0.0',
  'typing-extensions>=4.6.1,<5.0.0']
 
 setup_kwargs = {
     'name': 'catalystwan',
-    'version': '0.33.6.post0',
+    'version': '0.33.7',
     'description': 'Cisco Catalyst WAN SDK for Python',
-    'long_description': '<p align="center">\n  <a href="#"><img src="docs/images/catalystwan.svg" alt="Cisco Catalyst WAN SDK Logo" style="height:150px" />\n</p>\n\n[![Python-Supported](https://img.shields.io/static/v1?label=Python&logo=Python&color=3776AB&message=3.8%20|%203.9%20|%203.10%20|%203.11%20|%203.12)](https://www.python.org/)\n\nCisco Catalyst WAN SDK is a package for creating simple and parallel automatic requests via official SD-WAN Manager API. It is intended to serve as a multiple session handler (provider, provider as a tenant, tenant). The library is not dependent on environment which is being run in, you just need a connection to any SD-WAN Manager.\n\n## Important Notice: Early Beta Release\n\nWelcome to the Cisco Catalyst WAN SDK!\n\nWe are thrilled to announce that Cisco Catalyst WAN SDK is now available in early beta. This is an exciting step forward in enabling developers to harness the full potential of Cisco\'s networking solutions.  Please be aware that, as an early beta release, this version of the SDK is still undergoing development and testing. As such, it is provided "as is" and support to address any issues are limited and best effort.\n\n## Not recommend to use in production environments.\nWe encourage developers to explore and test the SDK\'s capabilities, but please exercise caution when using it in production environments.  We are dedicated to improving the Cisco Catalyst WAN SDK and we value your input. Your feedback is crucial to us-it will guide us in refining and enhancing the SDK to better meet your needs.\nTo report any issues, share your insights, or suggest improvements, please visit our Issues page on GitHub or reach out to us through the provided communication channels.\n\nThank you for being a part of our development journey!\n\n## Installation\n```console\npip install catalystwan\n```\n\n## Manager Session\nIn order to execute SDK APIs **ManagerSession** needs to be created. The fastest way to get started is to use `create_manager_session()` method which configures session, performs authentication for given credentials and returns **ManagerSession** instance in operational state. **ManagerSession** provides a collection of supported APIs in `api` instance variable.\nPlease check example below:\n\n```python\nfrom catalystwan.session import create_manager_session\n\nurl = "example.com"\nusername = "admin"\npassword = "password123"\n\nwith create_manager_session(url=url, username=username, password=password) as session:\n    devices = session.api.devices.get()\n    print(devices)\n```\n**ManagerSession** extends [requests.Session](https://requests.readthedocs.io/en/latest/user/advanced/#session-objects) so all functionality from [requests](https://requests.readthedocs.io/en/latest/) library is avaiable to user, it also implements python [contextmanager](https://docs.python.org/3.8/library/contextlib.html#contextlib.contextmanager) and automatically frees server resources on exit.\n\n<details>\n    <summary> <b>Configure Manager Session before using</b> <i>(click to expand)</i></summary>\n\nIt is possible to configure **ManagerSession** prior sending any request.\n\n```python\nfrom catalystwan.session import ManagerSession\n\nurl = "example.com"\nusername = "admin"\npassword = "password123"\n\n# configure session using constructor - nothing will be sent to target server yet\nsession = ManagerSession(url=url, username=username, password=password)\n# login and send requests\nsession.login()\nsession.get("/dataservice/device")\nsession.close()\n```\nWhen interacting with the SDWAN Manager API without using a context manager, it\'s important \nto manually execute the `close()` method to release the user session resource.\nEnsure that the `close()` method is called after you have finished using the session to maintain optimal resource management and avoid potential errors.\n\n</details>\n\n<details>\n    <summary> <b>Login as Tenant</b> <i>(click to expand)</i></summary>\n\nTenant domain needs to be provided in url together with Tenant credentials.\n\n```python\nfrom catalystwan.session import create_manager_session\n\nurl = "tenant.example.com"\nusername = "tenant_user"\npassword = "password123"\n\nwith create_manager_session(url=url, username=username, password=password) as session:\n    print(session.session_type)\n```\n\n</details>\n\n<details>\n    <summary> <b>Login as Provider-as-Tenant</b> <i>(click to expand)</i></summary>\n\nTenant `subdomain` needs to be provided as additional argument together with Provider credentials.\n\n```python\nfrom catalystwan.session import create_manager_session\n\nurl = "example.com"\nusername = "provider"\npassword = "password123"\nsubdomain = "tenant.example.com"\n\nwith create_manager_session(url=url, username=username, password=password, subdomain=subdomain) as session:\n    print(session.session_type)\n```\n\n</details>\n\n\n\n## API usage examples\nAll examples below assumes `session` variable contains logged-in [Manager Session](#Manager-Session) instance.\n\n<details>\n    <summary> <b>Get devices</b> <i>(click to expand)</i></summary>\n\n```python\ndevices = session.api.devices.get()\n```\n\n</details>\n\n<details>\n    <summary> <b>Admin Tech</b> <i>(click to expand)</i></summary>\n\n```Python\nadmin_tech_file = session.api.admin_tech.generate("172.16.255.11")\nsession.api.admin_tech.download(admin_tech_file)\nsession.api.admin_tech.delete(admin_tech_file)\n```\n</details>\n\n<details>\n    <summary> <b>Speed test</b> <i>(click to expand)</i></summary>\n\n```python\ndevices = session.api.devices.get()\nspeedtest = session.api.speedtest.speedtest(devices[0], devices[1])\n```\n\n</details>\n\n<details>\n    <summary> <b>Upgrade device</b> <i>(click to expand)</i></summary>\n\n```python\n# Prepare devices list\ncontrollers = session.endpoints.configuration_device_inventory.get_device_details(\'controllers\')\nvsmarts = controllers.filter(personality=Personality.VSMART)\nimage = "viptela-20.7.2-x86_64.tar.gz"\n\n# Upload image\nsession.api.repository.upload_image(image)\n\n# Install software\n\ninstall_task = session.api.software.install(devices=vsmarts, image=image)\n\n# Check action status\ninstall_task.wait_for_completed()\n```\n\n</details>\n\n<details>\n    <summary> <b>Get alarms</b> <i>(click to expand)</i></summary>\nTo get all alarms:\n\n```python\nalarms = session.api.alarms.get()\n```\n\nTo get all not viewed alarms:\n\n```python\nnot_viewed_alarms = session.api.alarms.get().filter(viewed=False)\n```\n\nTo get all alarms from past `n` hours:\n\n```python\nn = 24\nalarms_from_n_hours = session.api.alarms.get(from_time=n)\n```\n\nTo get all critical alarms from past `n` hours:\n\n```python\nfrom catalystwan.utils.alarm_status import Severity\nn = 48\ncritical_alarms = session.api.alarms.get(from_time=n).filter(severity=Severity.CRITICAL)\n```\n\n</details>\n\n<details>\n    <summary> <b>Users</b> <i>(click to expand)</i></summary>\n\n```python\n# Get all users\nsession.api.users.get()\n\n# Create user\nfrom catalystwan.endpoints.administration_user_and_group import User\nnew_user = User(username="new_user", password="new_user", group=["netadmin"], description="new user")\nsession.api.users.create(new_user)\n\n# Update user data\nnew_user_update = UserUpdateRequest(username="new_user", group=["netadmin", "netops"], locale="en_US", description="updated-new_user-description")\nsession.api.users.update(new_user_update)\n\n# Update user password\nsession.api.users.update_password("new_user", "n3W-P4s$w0rd")\n\n# Reset user\nsession.api.users.reset("new_user")\n\n# Delete user\nsession.api.users.delete("new_user")\n\n# Get current user authentication type and role\nsession.api.users.get_auth_type()\nsession.api.users.get_role()\n```\n\n</details>\n\n<details>\n    <summary> <b>User Groups</b> <i>(click to expand)</i></summary>\n\n```python\n# Get all user groups\nsession.api.user_groups.get()\n\n# Create user group\ngroup = UserGroup("new_user_group", [])\ngroup.enable_read({"Audit Log", "Alarms"})\ngroup.enable_read_and_write({"Device Inventory"})\nsession.api.user_groups.create(group)\n\n# Update user group\ngroup.disable({"Alarms"})\nsession.api.user_groups.update(group)\n\n# Delete user group\nsession.api.user_groups.delete(group.group_name)\n```\n\n</details>\n\n</details>\n\n<details>\n    <summary> <b>Sessions</b> <i>(click to expand)</i></summary>\n\n```python\n# Get all active sessions\nactive_sessions = session.api.sessions.get()\n\n# Invalidate sessions for given user\nnew_user_sessions = active_sessions.filter(raw_username="new_user")\nsession.api.sessions.invalidate(new_user_sessions)\n```\n\n</details>\n\n<details>\n    <summary> <b>Resource Groups</b> <i>(click to expand)</i></summary>\n\n```python\n# get resource groups\nsession.api.resource_groups.get()\n\n# create resource group\nnew_resource_group = ResourceGroup(\n    name="new_resource_group",\n    desc="Custom Resource Group #1",\n    siteIds=[]\n)\nsession.api.resource_groups.create(new_resource_group)\n\n# update resource group\nresource_group = session.api.resource_groups.get().filter(name="new_resource_group").single_or_default()\nupdated_resource_group = ResourceGroupUpdateRequest(\n    id=resource_group.id,\n    name=resource_group.name,\n    desc="Custom Resource Group #1 with updated description and site ids",\n    siteIds=[200]\n)\n\n# switch to resource group view\nsession.api.resource_groups.switch("new_resource_group")\n\n# delete resource group\nsession.api.resource_groups.delete(resource_group.id)\n```\n\n</details>\n\n<details>\n    <summary> <b>Tenant management</b> <i>(click to expand)</i></summary>\n\n```python\napi = session.api.tenant_management\n# create tenants\ntenants = [\n    Tenant(\n        name="tenant1",\n        org_name="CiscoDevNet",\n        subdomain="alpha.bravo.net",\n        desc="This is tenant for unit tests",\n        edge_connector_enable=True,\n        edge_connector_system_ip="172.16.255.81",\n        edge_connector_tunnel_interface_name="GigabitEthernet1",\n        wan_edge_forecast=1,\n    )\n]\ncreate_task = api.create(tenants)\ncreate_task.wait_for_completed()\n# list all tenants\ntenants_data = api.get_all()\n# pick tenant from list by name\ntenant = tenants_data.filter(name="tenant1").single_or_default()\n# get selected tenant id\ntenant_id = tenant.tenant_id\n# get vsession id of selected tenant\nvsessionid = api.vsession_id(tenant_id)\n# delete tenant by ids\ndelete_task = api.delete([tenant_id])\ndelete_task.wait_for_completed()\n# others\napi.get_hosting_capacity_on_vsmarts()\napi.get_statuses()\napi.get_vsmart_mapping()\n```\n</details>\n\n<details>\n    <summary> <b>Tenant migration</b> <i>(click to expand)</i></summary>\n\n```python\nfrom pathlib import Path\nfrom catalystwan.session import create_manager_session\nfrom catalystwan.models.tenant import TenantExport\nfrom catalystwan.workflows.tenant_migration import migration_workflow\n\ntenant = TenantExport(\n    name="mango",\n    desc="Mango tenant description",\n    org_name="Provider Org-Mango Inc",\n    subdomain="mango.fruits.com",\n    wan_edge_forecast=100,\n    migration_key="MangoTenantMigrationKey",   # only for SDWAN Manager >= 20.13\n    is_destination_overlay_mt=True,            # only for SDWAN Manager >= 20.13\n)\n\nwith create_manager_session(url="10.0.1.15", username="st-admin", password="") as origin_session, \\\n     create_manager_session(url="10.9.0.16", username="mt-provider-admin", password="") as target_session:\n    migration_workflow(\n        origin_session=origin_session,\n        target_session=target_session,\n        workdir=Path("workdir"),\n        tenant=tenant,\n        validator="10.9.12.26"\n    )\n```\n\n`migration_workflow` performs multi-step migration procedure according to [Migrate Single-Tenant Cisco SD-WAN Overlay to Multitenant Cisco SD-WAN Deployment](https://www.cisco.com/c/en/us/td/docs/routers/sdwan/configuration/system-interface/vedge-20-x/systems-interfaces-book/sdwan-multitenancy.html#concept_sjj_jmm_z4b)\n\n\nSince 20.13 also MT to ST is supported (just provide suitable origin/target sessions, and `is_destination_overlay_mt` parameter)\n\n\nEach step of the `migration_workflow` procedure can be executed independently using api methods: `export_tenant`, `download`, `import_tenant`, `store_token`, `migrate_network`\n\n```python\norigin_api = origin_session.api.tenant_migration_api\ntarget_api = target_session.api.tenant_migration_api\ntenant_file = Path("~/tenant.tar.gz")\ntoken_file = Path("~/tenant-token.txt")\n# export\nexport_task = origin_api.export_tenant(tenant=tenant)\nremote_filename = export_task.wait_for_file()\n# download\norigin_api.download(export_path, remote_filename)\n# import\nimport_task = target_api.import_tenant(export_path, tenant.migration_key)\nimport_task.wait_for_completed()\n# get token\nmigration_id = import_task.import_info.migration_token_query_params.migration_id\ntarget_api.store_token(migration_id, token_path)\n# migrate network\nmigrate_task = origin_api.migrate_network(token_path)\nmigrate_task.wait_for_completed()\n```\n</details>\n\n<details>\n    <summary> <b>Feature Templates</b> <i>(click to expand)</i></summary>\n\n```python\nfrom catalystwan.api.templates.models.omp_vsmart_model import OMPvSmart\n\nomp_vsmart = OMPvSmart(\n    name="my_first_template",\n    description="NA",\n    device_models=["vsmart"]\n    \n)\n\nsession.api.templates.create(omp_vsmart)\n```\n\nMore details about how to use and how to add new: [Feature Templates README.md](https://github.com/cisco-open/cisco-catalyst-wan-sdk/blob/main/catalystwan/api/templates/README.md)\n</details>\n\n### Note:\nTo remove `InsecureRequestWarning`, you can include in your scripts (warning is suppressed when `catalystwan_devel` environment variable is set):\n```Python\nimport urllib3\nurllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)\n```\n\n## Catching Exceptions\n```python\ntry:\n    session.api.users.delete("bogus-user-name")\nexcept ManagerHTTPError as error:\n    # Process an error.\n    print(error.response.status_code)\n    print(error.info.code)\n    print(error.info.message)\n    print(error.info.details)\n\n```\n\n## [Supported API endpoints](https://github.com/cisco-open/cisco-catalyst-wan-sdk/blob/main/ENDPOINTS.md)\n\n\n## [Contributing, bug reporting and feature requests](https://github.com/cisco-open/cisco-catalyst-wan-sdk/blob/main/CONTRIBUTING.md)\n\n## Seeking support\n\nYou can contact us by submitting [issues](https://github.com/cisco-open/cisco-catalyst-wan-sdk/issues), or directly via mail on catalystwan@cisco.com.\n',
+    'long_description': '<p align="center">\n  <a href="#"><img src="docs/images/catalystwan.svg" alt="Cisco Catalyst WAN SDK Logo" style="height:150px" />\n</p>\n\n[![Python-Supported](https://img.shields.io/static/v1?label=Python&logo=Python&color=3776AB&message=3.8%20|%203.9%20|%203.10%20|%203.11%20|%203.12)](https://www.python.org/)\n\nCisco Catalyst WAN SDK is a package for creating simple and parallel automatic requests via official SD-WAN Manager API. It is intended to serve as a multiple session handler (provider, provider as a tenant, tenant). The library is not dependent on environment which is being run in, you just need a connection to any SD-WAN Manager.\n\n## Important Notice: Early Beta Release\n\nWelcome to the Cisco Catalyst WAN SDK!\n\nWe are thrilled to announce that Cisco Catalyst WAN SDK is now available in early beta. This is an exciting step forward in enabling developers to harness the full potential of Cisco\'s networking solutions.  Please be aware that, as an early beta release, this version of the SDK is still undergoing development and testing. As such, it is provided "as is" and support to address any issues are limited and best effort.\n\n## Not recommend to use in production environments.\nWe encourage developers to explore and test the SDK\'s capabilities, but please exercise caution when using it in production environments.  We are dedicated to improving the Cisco Catalyst WAN SDK and we value your input. Your feedback is crucial to us-it will guide us in refining and enhancing the SDK to better meet your needs.\nTo report any issues, share your insights, or suggest improvements, please visit our Issues page on GitHub or reach out to us through the provided communication channels.\n\nThank you for being a part of our development journey!\n\n## Installation\n```console\npip install catalystwan\n```\n\n## Manager Session\nIn order to execute SDK APIs **ManagerSession** needs to be created. The fastest way to get started is to use `create_manager_session()` method which configures session, performs authentication for given credentials and returns **ManagerSession** instance in operational state. **ManagerSession** provides a collection of supported APIs in `api` instance variable.\nPlease check example below:\n\n```python\nfrom catalystwan.session import create_manager_session\n\nurl = "example.com"\nusername = "admin"\npassword = "password123"\n\nwith create_manager_session(url=url, username=username, password=password) as session:\n    devices = session.api.devices.get()\n    print(devices)\n```\n**ManagerSession** extends [requests.Session](https://requests.readthedocs.io/en/latest/user/advanced/#session-objects) so all functionality from [requests](https://requests.readthedocs.io/en/latest/) library is avaiable to user, it also implements python [contextmanager](https://docs.python.org/3.8/library/contextlib.html#contextlib.contextmanager) and automatically frees server resources on exit.\n\n<details>\n    <summary> <b>Configure Manager Session before using</b> <i>(click to expand)</i></summary>\n\nIt is possible to configure **ManagerSession** prior sending any request.\n\n```python\nfrom catalystwan.session import ManagerSession\n\nurl = "example.com"\nusername = "admin"\npassword = "password123"\n\n# configure session using constructor - nothing will be sent to target server yet\nsession = ManagerSession(url=url, username=username, password=password)\n# login and send requests\nsession.login()\nsession.get("/dataservice/device")\nsession.close()\n```\nWhen interacting with the SDWAN Manager API without using a context manager, it\'s important \nto manually execute the `close()` method to release the user session resource.\nEnsure that the `close()` method is called after you have finished using the session to maintain optimal resource management and avoid potential errors.\n\n</details>\n\n<details>\n    <summary> <b>Login as Tenant</b> <i>(click to expand)</i></summary>\n\nTenant domain needs to be provided in url together with Tenant credentials.\n\n```python\nfrom catalystwan.session import create_manager_session\n\nurl = "tenant.example.com"\nusername = "tenant_user"\npassword = "password123"\n\nwith create_manager_session(url=url, username=username, password=password) as session:\n    print(session.session_type)\n```\n\n</details>\n\n<details>\n    <summary> <b>Login as Provider-as-Tenant</b> <i>(click to expand)</i></summary>\n\nTenant `subdomain` needs to be provided as additional argument together with Provider credentials.\n\n```python\nfrom catalystwan.session import create_manager_session\n\nurl = "example.com"\nusername = "provider"\npassword = "password123"\nsubdomain = "tenant.example.com"\n\nwith create_manager_session(url=url, username=username, password=password, subdomain=subdomain) as session:\n    print(session.session_type)\n```\n\n</details>\n\n\n\n## API usage examples\nAll examples below assumes `session` variable contains logged-in [Manager Session](#Manager-Session) instance.\n\n<details>\n    <summary> <b>Get devices</b> <i>(click to expand)</i></summary>\n\n```python\ndevices = session.api.devices.get()\n```\n\n</details>\n\n<details>\n    <summary> <b>Admin Tech</b> <i>(click to expand)</i></summary>\n\n```Python\nadmin_tech_file = session.api.admin_tech.generate("172.16.255.11")\nsession.api.admin_tech.download(admin_tech_file)\nsession.api.admin_tech.delete(admin_tech_file)\n```\n</details>\n\n<details>\n    <summary> <b>Speed test</b> <i>(click to expand)</i></summary>\n\n```python\ndevices = session.api.devices.get()\nspeedtest = session.api.speedtest.speedtest(devices[0], devices[1])\n```\n\n</details>\n\n<details>\n    <summary> <b>Upgrade device</b> <i>(click to expand)</i></summary>\n\n```python\n# Prepare devices list\ncontrollers = session.endpoints.configuration_device_inventory.get_device_details(\'controllers\')\nvsmarts = controllers.filter(personality=Personality.VSMART)\nimage = "viptela-20.7.2-x86_64.tar.gz"\n\n# Upload image\nsession.api.repository.upload_image(image)\n\n# Install software\n\ninstall_task = session.api.software.install(devices=vsmarts, image=image)\n\n# Check action status\ninstall_task.wait_for_completed()\n```\n\n</details>\n\n<details>\n    <summary> <b>Get alarms</b> <i>(click to expand)</i></summary>\nTo get all alarms:\n\n```python\nalarms = session.api.alarms.get()\n```\n\nTo get all not viewed alarms:\n\n```python\nnot_viewed_alarms = session.api.alarms.get().filter(viewed=False)\n```\n\nTo get all alarms from past `n` hours:\n\n```python\nn = 24\nalarms_from_n_hours = session.api.alarms.get(from_time=n)\n```\n\nTo get all critical alarms from past `n` hours:\n\n```python\nfrom catalystwan.utils.alarm_status import Severity\nn = 48\ncritical_alarms = session.api.alarms.get(from_time=n).filter(severity=Severity.CRITICAL)\n```\n\n</details>\n\n<details>\n    <summary> <b>Users</b> <i>(click to expand)</i></summary>\n\n```python\n# Get all users\nsession.api.users.get()\n\n# Create user\nfrom catalystwan.endpoints.administration_user_and_group import User\nnew_user = User(username="new_user", password="new_user", group=["netadmin"], description="new user")\nsession.api.users.create(new_user)\n\n# Update user data\nnew_user_update = UserUpdateRequest(username="new_user", group=["netadmin", "netops"], locale="en_US", description="updated-new_user-description")\nsession.api.users.update(new_user_update)\n\n# Update user password\nsession.api.users.update_password("new_user", "n3W-P4s$w0rd")\n\n# Reset user\nsession.api.users.reset("new_user")\n\n# Delete user\nsession.api.users.delete("new_user")\n\n# Get current user authentication type and role\nsession.api.users.get_auth_type()\nsession.api.users.get_role()\n```\n\n</details>\n\n<details>\n    <summary> <b>User Groups</b> <i>(click to expand)</i></summary>\n\n```python\n# Get all user groups\nsession.api.user_groups.get()\n\n# Create user group\ngroup = UserGroup("new_user_group", [])\ngroup.enable_read({"Audit Log", "Alarms"})\ngroup.enable_read_and_write({"Device Inventory"})\nsession.api.user_groups.create(group)\n\n# Update user group\ngroup.disable({"Alarms"})\nsession.api.user_groups.update(group)\n\n# Delete user group\nsession.api.user_groups.delete(group.group_name)\n```\n\n</details>\n\n</details>\n\n<details>\n    <summary> <b>Sessions</b> <i>(click to expand)</i></summary>\n\n```python\n# Get all active sessions\nactive_sessions = session.api.sessions.get()\n\n# Invalidate sessions for given user\nnew_user_sessions = active_sessions.filter(raw_username="new_user")\nsession.api.sessions.invalidate(new_user_sessions)\n```\n\n</details>\n\n<details>\n    <summary> <b>Resource Groups</b> <i>(click to expand)</i></summary>\n\n```python\n# get resource groups\nsession.api.resource_groups.get()\n\n# create resource group\nnew_resource_group = ResourceGroup(\n    name="new_resource_group",\n    desc="Custom Resource Group #1",\n    siteIds=[]\n)\nsession.api.resource_groups.create(new_resource_group)\n\n# update resource group\nresource_group = session.api.resource_groups.get().filter(name="new_resource_group").single_or_default()\nupdated_resource_group = ResourceGroupUpdateRequest(\n    id=resource_group.id,\n    name=resource_group.name,\n    desc="Custom Resource Group #1 with updated description and site ids",\n    siteIds=[200]\n)\n\n# switch to resource group view\nsession.api.resource_groups.switch("new_resource_group")\n\n# delete resource group\nsession.api.resource_groups.delete(resource_group.id)\n```\n\n</details>\n\n<details>\n    <summary> <b>Tenant management</b> <i>(click to expand)</i></summary>\n\n```python\napi = session.api.tenant_management\n# create tenants\ntenants = [\n    Tenant(\n        name="tenant1",\n        org_name="CiscoDevNet",\n        subdomain="alpha.bravo.net",\n        desc="This is tenant for unit tests",\n        edge_connector_enable=True,\n        edge_connector_system_ip="172.16.255.81",\n        edge_connector_tunnel_interface_name="GigabitEthernet1",\n        wan_edge_forecast=1,\n    )\n]\ncreate_task = api.create(tenants)\ncreate_task.wait_for_completed()\n# list all tenants\ntenants_data = api.get_all()\n# pick tenant from list by name\ntenant = tenants_data.filter(name="tenant1").single_or_default()\n# get selected tenant id\ntenant_id = tenant.tenant_id\n# get vsession id of selected tenant\nvsessionid = api.vsession_id(tenant_id)\n# delete tenant by ids\ndelete_task = api.delete([tenant_id])\ndelete_task.wait_for_completed()\n# others\napi.get_hosting_capacity_on_vsmarts()\napi.get_statuses()\napi.get_vsmart_mapping()\n```\n</details>\n\n<details>\n    <summary> <b>Tenant migration</b> <i>(click to expand)</i></summary>\n\n```python\nfrom pathlib import Path\nfrom catalystwan.session import create_manager_session\nfrom catalystwan.models.tenant import TenantExport\nfrom catalystwan.workflows.tenant_migration import migration_workflow\n\ntenant = TenantExport(\n    name="mango",\n    desc="Mango tenant description",\n    org_name="Provider Org-Mango Inc",\n    subdomain="mango.fruits.com",\n    wan_edge_forecast=100,\n    migration_key="MangoTenantMigrationKey",   # only for SDWAN Manager >= 20.13\n    is_destination_overlay_mt=True,            # only for SDWAN Manager >= 20.13\n)\n\nwith create_manager_session(url="10.0.1.15", username="st-admin", password="") as origin_session, \\\n     create_manager_session(url="10.9.0.16", username="mt-provider-admin", password="") as target_session:\n    migration_workflow(\n        origin_session=origin_session,\n        target_session=target_session,\n        workdir=Path("workdir"),\n        tenant=tenant,\n        validator="10.9.12.26"\n    )\n```\n\n`migration_workflow` performs multi-step migration procedure according to [Migrate Single-Tenant Cisco SD-WAN Overlay to Multitenant Cisco SD-WAN Deployment](https://www.cisco.com/c/en/us/td/docs/routers/sdwan/configuration/system-interface/vedge-20-x/systems-interfaces-book/sdwan-multitenancy.html#concept_sjj_jmm_z4b)\n\n\nSince 20.13 also MT to ST is supported (just provide suitable origin/target sessions, and `is_destination_overlay_mt` parameter)\n\n\nEach step of the `migration_workflow` procedure can be executed independently using api methods: `export_tenant`, `download`, `import_tenant`, `store_token`, `migrate_network`\n\n```python\norigin_api = origin_session.api.tenant_migration_api\ntarget_api = target_session.api.tenant_migration_api\ntenant_file = Path("~/tenant.tar.gz")\ntoken_file = Path("~/tenant-token.txt")\n# export\nexport_task = origin_api.export_tenant(tenant=tenant)\nremote_filename = export_task.wait_for_file()\n# download\norigin_api.download(export_path, remote_filename)\n# import\nimport_task = target_api.import_tenant(export_path, tenant.migration_key)\nimport_task.wait_for_completed()\n# get token\nmigration_id = import_task.import_info.migration_token_query_params.migration_id\ntarget_api.store_token(migration_id, token_path)\n# migrate network\nmigrate_task = origin_api.migrate_network(token_path)\nmigrate_task.wait_for_completed()\n```\n</details>\n\n### Note:\nTo remove `InsecureRequestWarning`, you can include in your scripts (warning is suppressed when `catalystwan_devel` environment variable is set):\n```Python\nimport urllib3\nurllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)\n```\n\n## Catching Exceptions\n```python\ntry:\n    session.api.users.delete("bogus-user-name")\nexcept ManagerHTTPError as error:\n    # Process an error.\n    print(error.response.status_code)\n    print(error.info.code)\n    print(error.info.message)\n    print(error.info.details)\n\n```\n\n## [Supported API endpoints](https://github.com/cisco-open/cisco-catalyst-wan-sdk/blob/main/ENDPOINTS.md)\n\n\n## [Contributing, bug reporting and feature requests](https://github.com/cisco-open/cisco-catalyst-wan-sdk/blob/main/CONTRIBUTING.md)\n\n## Seeking support\n\nYou can contact us by submitting [issues](https://github.com/cisco-open/cisco-catalyst-wan-sdk/issues), or directly via mail on catalystwan@cisco.com.\n',
     'author': 'kagorski',
     'author_email': 'kagorski@cisco.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/cisco-open/cisco-catalyst-wan-sdk',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -34,15 +34,15 @@
 'catalystwan.tests.templates': ['definitions/*', 'definitions/basic/*',
 'schemas/*', 'schemas/basic/*']} install_requires = \ ['Jinja2>=3.1.2,<4.0.0',
 'attrs>=21.4.0,<22.0.0', 'ciscoconfparse==1.9.41', 'clint>=0.5.1,<0.6.0',
 'flake8-quotes>=3.3.1,<4.0.0', 'packaging>=23.0,<24.0', 'pydantic>=2.5,<3.0',
 'python-dateutil>=2.8.2,<3.0.0', 'requests-toolbelt>=1.0.0,<2.0.0',
 'requests>=2.27.1,<3.0.0', 'tenacity>=8.1.0,<9.0.0', 'typing-
 extensions>=4.6.1,<5.0.0'] setup_kwargs = { 'name': 'catalystwan', 'version':
-'0.33.6.post0', 'description': 'Cisco Catalyst WAN SDK for Python',
+'0.33.7', 'description': 'Cisco Catalyst WAN SDK for Python',
 'long_description': '
                       \n _[_C_i_s_c_o_ _C_a_t_a_l_y_s_t_ _W_A_N_ _S_D_K_ _L_o_g_o_]_\_n
 \n\n[![Python-Supported](https://img.shields.io/static/
 v1?label=Python&logo=Python&color=3776AB&message=3.8%20|%203.9%20|%203.10%20|%203.11%20|%203.12)]
 (https://www.python.org/)\n\nCisco Catalyst WAN SDK is a package for creating
 simple and parallel automatic requests via official SD-WAN Manager API. It is
 intended to serve as a multiple session handler (provider, provider as a
@@ -209,23 +209,16 @@
 export_task.wait_for_file()\n# download\norigin_api.download(export_path,
 remote_filename)\n# import\nimport_task = target_api.import_tenant(export_path,
 tenant.migration_key)\nimport_task.wait_for_completed()\n# get
 token\nmigration_id =
 import_task.import_info.migration_token_query_params.migration_id\ntarget_api.store_token
 (migration_id, token_path)\n# migrate network\nmigrate_task =
 origin_api.migrate_network(token_path)\nmigrate_task.wait_for_completed
-()\n```\n\n\n\n FFeeaattuurree TTeemmppllaatteess (click to expand)\n\n```python\nfrom
-catalystwan.api.templates.models.omp_vsmart_model import
-OMPvSmart\n\nomp_vsmart = OMPvSmart(\n name="my_first_template",\n
-description="NA",\n device_models=["vsmart"]\n
-\n)\n\nsession.api.templates.create(omp_vsmart)\n```\n\nMore details about how
-to use and how to add new: [Feature Templates README.md](https://github.com/
-cisco-open/cisco-catalyst-wan-sdk/blob/main/catalystwan/api/templates/
-README.md)\n\n\n### Note:\nTo remove `InsecureRequestWarning`, you can include
-in your scripts (warning is suppressed when `catalystwan_devel` environment
+()\n```\n\n\n### Note:\nTo remove `InsecureRequestWarning`, you can include in
+your scripts (warning is suppressed when `catalystwan_devel` environment
 variable is set):\n```Python\nimport urllib3\nurllib3.disable_warnings
 (urllib3.exceptions.InsecureRequestWarning)\n```\n\n## Catching
 Exceptions\n```python\ntry:\n session.api.users.delete("bogus-user-
 name")\nexcept ManagerHTTPError as error:\n # Process an error.\n print
 (error.response.status_code)\n print(error.info.code)\n print
 (error.info.message)\n print(error.info.details)\n\n```\n\n## [Supported API
 endpoints](https://github.com/cisco-open/cisco-catalyst-wan-sdk/blob/main/
```

### Comparing `catalystwan-0.33.6.post0/PKG-INFO` & `catalystwan-0.33.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catalystwan
-Version: 0.33.6.post0
+Version: 0.33.7
 Summary: Cisco Catalyst WAN SDK for Python
 Home-page: https://github.com/cisco-open/cisco-catalyst-wan-sdk
 Author: kagorski
 Author-email: kagorski@cisco.com
 Requires-Python: >=3.8.0,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -415,33 +415,14 @@
 target_api.store_token(migration_id, token_path)
 # migrate network
 migrate_task = origin_api.migrate_network(token_path)
 migrate_task.wait_for_completed()
 ```
 </details>
 
-<details>
-    <summary> <b>Feature Templates</b> <i>(click to expand)</i></summary>
-
-```python
-from catalystwan.api.templates.models.omp_vsmart_model import OMPvSmart
-
-omp_vsmart = OMPvSmart(
-    name="my_first_template",
-    description="NA",
-    device_models=["vsmart"]
-    
-)
-
-session.api.templates.create(omp_vsmart)
-```
-
-More details about how to use and how to add new: [Feature Templates README.md](https://github.com/cisco-open/cisco-catalyst-wan-sdk/blob/main/catalystwan/api/templates/README.md)
-</details>
-
 ### Note:
 To remove `InsecureRequestWarning`, you can include in your scripts (warning is suppressed when `catalystwan_devel` environment variable is set):
 ```Python
 import urllib3
 urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 ```
```

#### html2text {}

```diff
@@ -1,23 +1,22 @@
-Metadata-Version: 2.1 Name: catalystwan Version: 0.33.6.post0 Summary: Cisco
-Catalyst WAN SDK for Python Home-page: https://github.com/cisco-open/cisco-
-catalyst-wan-sdk Author: kagorski Author-email: kagorski@cisco.com Requires-
-Python: >=3.8.0,<4.0.0 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Requires-Dist: Jinja2
-(>=3.1.2,<4.0.0) Requires-Dist: attrs (>=21.4.0,<22.0.0) Requires-Dist:
-ciscoconfparse (==1.9.41) Requires-Dist: clint (>=0.5.1,<0.6.0) Requires-Dist:
-flake8-quotes (>=3.3.1,<4.0.0) Requires-Dist: packaging (>=23.0,<24.0)
-Requires-Dist: pydantic (>=2.5,<3.0) Requires-Dist: python-dateutil
-(>=2.8.2,<3.0.0) Requires-Dist: requests (>=2.27.1,<3.0.0) Requires-Dist:
-requests-toolbelt (>=1.0.0,<2.0.0) Requires-Dist: tenacity (>=8.1.0,<9.0.0)
-Requires-Dist: typing-extensions (>=4.6.1,<5.0.0) Project-URL: Repository,
-https://github.com/cisco-open/cisco-catalyst-wan-sdk Description-Content-Type:
-text/markdown
+Metadata-Version: 2.1 Name: catalystwan Version: 0.33.7 Summary: Cisco Catalyst
+WAN SDK for Python Home-page: https://github.com/cisco-open/cisco-catalyst-wan-
+sdk Author: kagorski Author-email: kagorski@cisco.com Requires-Python:
+>=3.8.0,<4.0.0 Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
+Requires-Dist: attrs (>=21.4.0,<22.0.0) Requires-Dist: ciscoconfparse
+(==1.9.41) Requires-Dist: clint (>=0.5.1,<0.6.0) Requires-Dist: flake8-quotes
+(>=3.3.1,<4.0.0) Requires-Dist: packaging (>=23.0,<24.0) Requires-Dist:
+pydantic (>=2.5,<3.0) Requires-Dist: python-dateutil (>=2.8.2,<3.0.0) Requires-
+Dist: requests (>=2.27.1,<3.0.0) Requires-Dist: requests-toolbelt
+(>=1.0.0,<2.0.0) Requires-Dist: tenacity (>=8.1.0,<9.0.0) Requires-Dist:
+typing-extensions (>=4.6.1,<5.0.0) Project-URL: Repository, https://github.com/
+cisco-open/cisco-catalyst-wan-sdk Description-Content-Type: text/markdown
                          _[_C_i_s_c_o_ _C_a_t_a_l_y_s_t_ _W_A_N_ _S_D_K_ _L_o_g_o_]
 [![Python-Supported](https://img.shields.io/static/
 v1?label=Python&logo=Python&color=3776AB&message=3.8%20|%203.9%20|%203.10%20|%203.11%20|%203.12)]
 (https://www.python.org/) Cisco Catalyst WAN SDK is a package for creating
 simple and parallel automatic requests via official SD-WAN Manager API. It is
 intended to serve as a multiple session handler (provider, provider as a
 tenant, tenant). The library is not dependent on environment which is being run
@@ -166,21 +165,15 @@
 origin_api.export_tenant(tenant=tenant) remote_filename =
 export_task.wait_for_file() # download origin_api.download(export_path,
 remote_filename) # import import_task = target_api.import_tenant(export_path,
 tenant.migration_key) import_task.wait_for_completed() # get token migration_id
 = import_task.import_info.migration_token_query_params.migration_id
 target_api.store_token(migration_id, token_path) # migrate network migrate_task
 = origin_api.migrate_network(token_path) migrate_task.wait_for_completed() ```
-FFeeaattuurree TTeemmppllaatteess (click to expand) ```python from
-catalystwan.api.templates.models.omp_vsmart_model import OMPvSmart omp_vsmart =
-OMPvSmart( name="my_first_template", description="NA", device_models=["vsmart"]
-) session.api.templates.create(omp_vsmart) ``` More details about how to use
-and how to add new: [Feature Templates README.md](https://github.com/cisco-
-open/cisco-catalyst-wan-sdk/blob/main/catalystwan/api/templates/README.md) ###
-Note: To remove `InsecureRequestWarning`, you can include in your scripts
+### Note: To remove `InsecureRequestWarning`, you can include in your scripts
 (warning is suppressed when `catalystwan_devel` environment variable is set):
 ```Python import urllib3 urllib3.disable_warnings
 (urllib3.exceptions.InsecureRequestWarning) ``` ## Catching Exceptions
 ```python try: session.api.users.delete("bogus-user-name") except
 ManagerHTTPError as error: # Process an error. print
 (error.response.status_code) print(error.info.code) print(error.info.message)
 print(error.info.details) ``` ## [Supported API endpoints](https://github.com/
```

