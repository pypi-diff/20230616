# Comparing `tmp/netbox_initializers-3.5.0.tar.gz` & `tmp/netbox_initializers-3.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox_initializers-3.5.0.tar", max compression
+gzip compressed data, was "netbox_initializers-3.5.1.tar", max compression
```

## Comparing `netbox_initializers-3.5.0.tar` & `netbox_initializers-3.5.1.tar`

### file list

```diff
@@ -1,101 +1,103 @@
--rw-r--r--   0        0        0    11358 2023-04-29 11:02:12.951142 netbox_initializers-3.5.0/LICENSE
--rw-r--r--   0        0        0     1503 2023-04-29 11:02:12.951142 netbox_initializers-3.5.0/README.md
--rw-r--r--   0        0        0      754 2023-04-29 11:02:12.951142 netbox_initializers-3.5.0/pyproject.toml
--rw-r--r--   0        0        0      353 2023-04-29 11:02:12.951142 netbox_initializers-3.5.0/src/netbox_initializers/__init__.py
--rw-r--r--   0        0        0     6050 2023-04-29 11:02:12.951142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/__init__.py
--rw-r--r--   0        0        0     1549 2023-04-29 11:02:12.951142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/aggregates.py
--rw-r--r--   0        0        0     1206 2023-04-29 11:02:12.951142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/asns.py
--rw-r--r--   0        0        0     8992 2023-04-29 11:02:12.951142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/cables.py
--rw-r--r--   0        0        0      842 2023-04-29 11:02:12.951142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/circuit_types.py
--rw-r--r--   0        0        0     1462 2023-04-29 11:02:12.951142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/circuits.py
--rw-r--r--   0        0        0      724 2023-04-29 11:02:12.951142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/cluster_groups.py
--rw-r--r--   0        0        0      711 2023-04-29 11:02:12.955142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/cluster_types.py
--rw-r--r--   0        0        0     1535 2023-04-29 11:02:12.955142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/clusters.py
--rw-r--r--   0        0        0     1167 2023-04-29 11:02:12.955142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/contact_groups.py
--rw-r--r--   0        0        0      842 2023-04-29 11:02:12.955142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/contact_roles.py
--rw-r--r--   0        0        0     1083 2023-04-29 11:02:12.955142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/contacts.py
--rw-r--r--   0        0        0     6133 2023-04-29 11:02:12.955142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/custom_fields.py
--rw-r--r--   0        0        0     1432 2023-04-29 11:02:12.955142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/custom_links.py
--rw-r--r--   0        0        0      956 2023-04-29 11:02:12.955142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/device_roles.py
--rw-r--r--   0        0        0     5458 2023-04-29 11:02:12.955142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/device_types.py
--rw-r--r--   0        0        0     1975 2023-04-29 11:02:12.955142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/devices.py
--rw-r--r--   0        0        0      856 2023-04-29 11:02:12.955142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/groups.py
--rw-r--r--   0        0        0     2919 2023-04-29 11:02:12.955142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/interfaces.py
--rw-r--r--   0        0        0     3022 2023-04-29 11:02:12.955142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/ip_addresses.py
--rw-r--r--   0        0        0      963 2023-04-29 11:02:12.955142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/locations.py
--rw-r--r--   0        0        0      703 2023-04-29 11:02:12.955142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/manufacturers.py
--rw-r--r--   0        0        0     3107 2023-04-29 11:02:12.955142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/object_permissions.py
--rw-r--r--   0        0        0      965 2023-04-29 11:02:12.955142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/platforms.py
--rw-r--r--   0        0        0     1451 2023-04-29 11:02:12.955142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/power_feeds.py
--rw-r--r--   0        0        0     1468 2023-04-29 11:02:12.955142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/power_panels.py
--rw-r--r--   0        0        0      618 2023-04-29 11:02:12.955142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/prefix_vlan_roles.py
--rw-r--r--   0        0        0     1453 2023-04-29 11:02:12.955142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/prefixes.py
--rw-r--r--   0        0        0     2240 2023-04-29 11:02:12.955142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/primary_ips.py
--rw-r--r--   0        0        0     1235 2023-04-29 11:02:12.955142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/providers.py
--rw-r--r--   0        0        0      931 2023-04-29 11:02:12.955142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/rack_roles.py
--rw-r--r--   0        0        0     1460 2023-04-29 11:02:12.955142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/racks.py
--rw-r--r--   0        0        0      908 2023-04-29 11:02:12.955142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/regions.py
--rw-r--r--   0        0        0      569 2023-04-29 11:02:12.955142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/rirs.py
--rw-r--r--   0        0        0     1179 2023-04-29 11:02:12.955142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/route_targets.py
--rw-r--r--   0        0        0     1122 2023-04-29 11:02:12.955142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/services.py
--rw-r--r--   0        0        0     1085 2023-04-29 11:02:12.955142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/sites.py
--rw-r--r--   0        0        0      835 2023-04-29 11:02:12.955142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/tags.py
--rw-r--r--   0        0        0      702 2023-04-29 11:02:12.955142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/tenant_groups.py
--rw-r--r--   0        0        0     1068 2023-04-29 11:02:12.955142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/tenants.py
--rw-r--r--   0        0        0      925 2023-04-29 11:02:12.955142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/users.py
--rw-r--r--   0        0        0     1957 2023-04-29 11:02:12.955142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/virtual_machines.py
--rw-r--r--   0        0        0     1232 2023-04-29 11:02:12.955142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/virtualization_interfaces.py
--rw-r--r--   0        0        0     2035 2023-04-29 11:02:12.955142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/vlan_groups.py
--rw-r--r--   0        0        0     1293 2023-04-29 11:02:12.955142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/vlans.py
--rw-r--r--   0        0        0     1080 2023-04-29 11:02:12.955142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/vrfs.py
--rw-r--r--   0        0        0     1288 2023-04-29 11:02:12.955142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/webhooks.py
--rw-r--r--   0        0        0      152 2023-04-29 11:02:12.955142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/yaml/aggregates.yml
--rw-r--r--   0        0        0      108 2023-04-29 11:02:12.955142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/yaml/asns.yml
--rw-r--r--   0        0        0     2299 2023-04-29 11:02:12.955142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/yaml/cables.yml
--rw-r--r--   0        0        0       98 2023-04-29 11:02:12.955142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/yaml/circuit_types.yml
--rw-r--r--   0        0        0      146 2023-04-29 11:02:12.955142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/yaml/circuits.yml
--rw-r--r--   0        0        0       72 2023-04-29 11:02:12.955142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/yaml/cluster_groups.yml
--rw-r--r--   0        0        0       36 2023-04-29 11:02:12.955142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/yaml/cluster_types.yml
--rw-r--r--   0        0        0      130 2023-04-29 11:02:12.955142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/yaml/clusters.yml
--rw-r--r--   0        0        0      264 2023-04-29 11:02:12.955142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/yaml/contact_groups.yml
--rw-r--r--   0        0        0      110 2023-04-29 11:02:12.955142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/yaml/contact_roles.yml
--rw-r--r--   0        0        0      694 2023-04-29 11:02:12.955142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/yaml/contacts.yml
--rw-r--r--   0        0        0     2753 2023-04-29 11:02:12.955142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/yaml/custom_fields.yml
--rw-r--r--   0        0        0      472 2023-04-29 11:02:12.955142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/yaml/custom_links.yml
--rw-r--r--   0        0        0      272 2023-04-29 11:02:12.955142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/yaml/device_roles.yml
--rw-r--r--   0        0        0     1511 2023-04-29 11:02:12.955142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/yaml/device_types.yml
--rw-r--r--   0        0        0     1066 2023-04-29 11:02:12.955142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/yaml/devices.yml
--rw-r--r--   0        0        0      124 2023-04-29 11:02:12.955142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/yaml/groups.yml
--rw-r--r--   0        0        0      744 2023-04-29 11:02:12.955142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/yaml/interfaces.yml
--rw-r--r--   0        0        0      847 2023-04-29 11:02:12.955142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/yaml/ip_addresses.yml
--rw-r--r--   0        0        0      219 2023-04-29 11:02:12.955142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/yaml/locations.yml
--rw-r--r--   0        0        0      136 2023-04-29 11:02:12.955142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/yaml/manufacturers.yml
--rw-r--r--   0        0        0     1079 2023-04-29 11:02:12.955142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/yaml/object_permissions.yml
--rw-r--r--   0        0        0      467 2023-04-29 11:02:12.955142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/yaml/platforms.yml
--rw-r--r--   0        0        0      316 2023-04-29 11:02:12.955142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/yaml/power_feeds.yml
--rw-r--r--   0        0        0      117 2023-04-29 11:02:12.955142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/yaml/power_panels.yml
--rw-r--r--   0        0        0       52 2023-04-29 11:02:12.955142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/yaml/prefix_vlan_roles.yml
--rw-r--r--   0        0        0      522 2023-04-29 11:02:12.955142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/yaml/prefixes.yml
--rw-r--r--   0        0        0      102 2023-04-29 11:02:12.955142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/yaml/providers.yml
--rw-r--r--   0        0        0      200 2023-04-29 11:02:12.955142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/yaml/rack_roles.yml
--rw-r--r--   0        0        0      723 2023-04-29 11:02:12.955142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/yaml/racks.yml
--rw-r--r--   0        0        0      198 2023-04-29 11:02:12.955142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/yaml/regions.yml
--rw-r--r--   0        0        0      179 2023-04-29 11:02:12.955142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/yaml/rirs.yml
--rw-r--r--   0        0        0       62 2023-04-29 11:02:12.955142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/yaml/route_targets.yml
--rw-r--r--   0        0        0      265 2023-04-29 11:02:12.955142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/yaml/services.yml
--rw-r--r--   0        0        0      679 2023-04-29 11:02:12.955142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/yaml/sites.yml
--rw-r--r--   0        0        0      192 2023-04-29 11:02:12.955142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/yaml/tags.yml
--rw-r--r--   0        0        0      100 2023-04-29 11:02:12.955142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/yaml/tenant_groups.yml
--rw-r--r--   0        0        0       98 2023-04-29 11:02:12.955142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/yaml/tenants.yml
--rw-r--r--   0        0        0      449 2023-04-29 11:02:12.955142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/yaml/users.yml
--rw-r--r--   0        0        0      779 2023-04-29 11:02:12.955142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/yaml/virtual_machines.yml
--rw-r--r--   0        0        0      346 2023-04-29 11:02:12.955142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/yaml/virtualization_interfaces.yml
--rw-r--r--   0        0        0      585 2023-04-29 11:02:12.955142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/yaml/vlan_groups.yml
--rw-r--r--   0        0        0      309 2023-04-29 11:02:12.955142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/yaml/vlans.yml
--rw-r--r--   0        0        0      166 2023-04-29 11:02:12.955142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/yaml/vrfs.yml
--rw-r--r--   0        0        0      555 2023-04-29 11:02:12.955142 netbox_initializers-3.5.0/src/netbox_initializers/initializers/yaml/webhooks.yml
--rw-r--r--   0        0        0        0 2023-04-29 11:02:12.955142 netbox_initializers-3.5.0/src/netbox_initializers/management/__init__.py
--rw-r--r--   0        0        0        0 2023-04-29 11:02:12.955142 netbox_initializers-3.5.0/src/netbox_initializers/management/commands/__init__.py
--rw-r--r--   0        0        0     1705 2023-04-29 11:02:12.955142 netbox_initializers-3.5.0/src/netbox_initializers/management/commands/copy_initializers_examples.py
--rw-r--r--   0        0        0     1359 2023-04-29 11:02:12.955142 netbox_initializers-3.5.0/src/netbox_initializers/management/commands/load_initializer_data.py
--rw-r--r--   0        0        0     2404 1970-01-01 00:00:00.000000 netbox_initializers-3.5.0/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-06-16 15:38:20.973119 netbox_initializers-3.5.1/LICENSE
+-rw-r--r--   0        0        0     1503 2023-06-16 15:38:20.973119 netbox_initializers-3.5.1/README.md
+-rw-r--r--   0        0        0      754 2023-06-16 15:38:20.973119 netbox_initializers-3.5.1/pyproject.toml
+-rw-r--r--   0        0        0      353 2023-06-16 15:38:20.973119 netbox_initializers-3.5.1/src/netbox_initializers/__init__.py
+-rw-r--r--   0        0        0     6130 2023-06-16 15:38:20.973119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/__init__.py
+-rw-r--r--   0        0        0     1549 2023-06-16 15:38:20.973119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/aggregates.py
+-rw-r--r--   0        0        0     1206 2023-06-16 15:38:20.973119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/asns.py
+-rw-r--r--   0        0        0     8992 2023-06-16 15:38:20.973119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/cables.py
+-rw-r--r--   0        0        0      842 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/circuit_types.py
+-rw-r--r--   0        0        0     1462 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/circuits.py
+-rw-r--r--   0        0        0      724 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/cluster_groups.py
+-rw-r--r--   0        0        0      711 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/cluster_types.py
+-rw-r--r--   0        0        0     1535 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/clusters.py
+-rw-r--r--   0        0        0     1217 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/config_templates.py
+-rw-r--r--   0        0        0     1167 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/contact_groups.py
+-rw-r--r--   0        0        0      842 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/contact_roles.py
+-rw-r--r--   0        0        0     1083 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/contacts.py
+-rw-r--r--   0        0        0     6133 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/custom_fields.py
+-rw-r--r--   0        0        0     1432 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/custom_links.py
+-rw-r--r--   0        0        0      956 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/device_roles.py
+-rw-r--r--   0        0        0     5458 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/device_types.py
+-rw-r--r--   0        0        0     2065 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/devices.py
+-rw-r--r--   0        0        0      856 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/groups.py
+-rw-r--r--   0        0        0     2919 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/interfaces.py
+-rw-r--r--   0        0        0     3022 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/ip_addresses.py
+-rw-r--r--   0        0        0      963 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/locations.py
+-rw-r--r--   0        0        0      703 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/manufacturers.py
+-rw-r--r--   0        0        0     3107 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/object_permissions.py
+-rw-r--r--   0        0        0      965 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/platforms.py
+-rw-r--r--   0        0        0     1451 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/power_feeds.py
+-rw-r--r--   0        0        0     1468 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/power_panels.py
+-rw-r--r--   0        0        0      618 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/prefix_vlan_roles.py
+-rw-r--r--   0        0        0     1453 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/prefixes.py
+-rw-r--r--   0        0        0     2240 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/primary_ips.py
+-rw-r--r--   0        0        0     1235 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/providers.py
+-rw-r--r--   0        0        0      931 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/rack_roles.py
+-rw-r--r--   0        0        0     1460 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/racks.py
+-rw-r--r--   0        0        0      908 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/regions.py
+-rw-r--r--   0        0        0      569 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/rirs.py
+-rw-r--r--   0        0        0     1179 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/route_targets.py
+-rw-r--r--   0        0        0     1122 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/services.py
+-rw-r--r--   0        0        0     1085 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/sites.py
+-rw-r--r--   0        0        0      835 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/tags.py
+-rw-r--r--   0        0        0      702 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/tenant_groups.py
+-rw-r--r--   0        0        0     1068 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/tenants.py
+-rw-r--r--   0        0        0      925 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/users.py
+-rw-r--r--   0        0        0     1957 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/virtual_machines.py
+-rw-r--r--   0        0        0     1232 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/virtualization_interfaces.py
+-rw-r--r--   0        0        0     2035 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/vlan_groups.py
+-rw-r--r--   0        0        0     1293 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/vlans.py
+-rw-r--r--   0        0        0     1080 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/vrfs.py
+-rw-r--r--   0        0        0     1288 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/webhooks.py
+-rw-r--r--   0        0        0      152 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/aggregates.yml
+-rw-r--r--   0        0        0      108 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/asns.yml
+-rw-r--r--   0        0        0     2299 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/cables.yml
+-rw-r--r--   0        0        0       98 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/circuit_types.yml
+-rw-r--r--   0        0        0      146 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/circuits.yml
+-rw-r--r--   0        0        0       72 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/cluster_groups.yml
+-rw-r--r--   0        0        0       36 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/cluster_types.yml
+-rw-r--r--   0        0        0      130 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/clusters.yml
+-rw-r--r--   0        0        0      148 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/config_templates.yml
+-rw-r--r--   0        0        0      264 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/contact_groups.yml
+-rw-r--r--   0        0        0      110 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/contact_roles.yml
+-rw-r--r--   0        0        0      694 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/contacts.yml
+-rw-r--r--   0        0        0     2753 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/custom_fields.yml
+-rw-r--r--   0        0        0      472 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/custom_links.yml
+-rw-r--r--   0        0        0      272 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/device_roles.yml
+-rw-r--r--   0        0        0     1511 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/device_types.yml
+-rw-r--r--   0        0        0     1105 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/devices.yml
+-rw-r--r--   0        0        0      124 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/groups.yml
+-rw-r--r--   0        0        0      744 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/interfaces.yml
+-rw-r--r--   0        0        0      847 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/ip_addresses.yml
+-rw-r--r--   0        0        0      219 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/locations.yml
+-rw-r--r--   0        0        0      136 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/manufacturers.yml
+-rw-r--r--   0        0        0     1079 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/object_permissions.yml
+-rw-r--r--   0        0        0      467 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/platforms.yml
+-rw-r--r--   0        0        0      316 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/power_feeds.yml
+-rw-r--r--   0        0        0      117 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/power_panels.yml
+-rw-r--r--   0        0        0       52 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/prefix_vlan_roles.yml
+-rw-r--r--   0        0        0      522 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/prefixes.yml
+-rw-r--r--   0        0        0      102 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/providers.yml
+-rw-r--r--   0        0        0      200 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/rack_roles.yml
+-rw-r--r--   0        0        0      723 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/racks.yml
+-rw-r--r--   0        0        0      198 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/regions.yml
+-rw-r--r--   0        0        0      179 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/rirs.yml
+-rw-r--r--   0        0        0       62 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/route_targets.yml
+-rw-r--r--   0        0        0      265 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/services.yml
+-rw-r--r--   0        0        0      679 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/sites.yml
+-rw-r--r--   0        0        0      192 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/tags.yml
+-rw-r--r--   0        0        0      100 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/tenant_groups.yml
+-rw-r--r--   0        0        0       98 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/tenants.yml
+-rw-r--r--   0        0        0      449 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/users.yml
+-rw-r--r--   0        0        0      779 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/virtual_machines.yml
+-rw-r--r--   0        0        0      346 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/virtualization_interfaces.yml
+-rw-r--r--   0        0        0      585 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/vlan_groups.yml
+-rw-r--r--   0        0        0      309 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/vlans.yml
+-rw-r--r--   0        0        0      166 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/vrfs.yml
+-rw-r--r--   0        0        0      555 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/webhooks.yml
+-rw-r--r--   0        0        0        0 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/management/commands/__init__.py
+-rw-r--r--   0        0        0     1705 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/management/commands/copy_initializers_examples.py
+-rw-r--r--   0        0        0     1359 2023-06-16 15:38:20.977119 netbox_initializers-3.5.1/src/netbox_initializers/management/commands/load_initializer_data.py
+-rw-r--r--   0        0        0     2404 1970-01-01 00:00:00.000000 netbox_initializers-3.5.1/PKG-INFO
```

### Comparing `netbox_initializers-3.5.0/LICENSE` & `netbox_initializers-3.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.0/README.md` & `netbox_initializers-3.5.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -32,10 +32,10 @@
 
 ## Netbox Docker image
 
 The initializers where a part of the Docker image and where then extracted into a Netbox plugin. This was done to split the release cycle of the initializers and the image.
 To use the new plugin in a the Netbox Docker image, it musst be installad into the image. To this, the following example can be used as a starting point:
 
 ```dockerfile
-FROM netboxcommunity/netbox:v3.4
+FROM netboxcommunity/netbox:v3.5
 RUN /opt/netbox/venv/bin/pip install "netbox-initializers==3.5.*"
 ```
```

### Comparing `netbox_initializers-3.5.0/pyproject.toml` & `netbox_initializers-3.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,19 +7,19 @@
   "Topic :: System :: Systems Administration"
 ]
 description = "Load initial data into Netbox"
 license = "Apache-2.0"
 name = "netbox-initializers"
 readme = "README.md"
 repository = "https://github.com/tobiasge/netbox-initializers"
-version = "3.5.0"
+version = "3.5.1"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-"ruamel.yaml" = "0.17.21"
+"ruamel.yaml" = "0.17.31"
 
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core"]
 
 [tool.black]
 line_length = 100
```

### Comparing `netbox_initializers-3.5.0/src/netbox_initializers/initializers/__init__.py` & `netbox_initializers-3.5.1/src/netbox_initializers/initializers/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 INITIALIZER_ORDER = (
     "users",
     "groups",
     "object_permissions",
     "custom_fields",
     "custom_links",
     "tags",
+    "config_templates",
     "webhooks",
     "tenant_groups",
     "tenants",
     "regions",
     "sites",
     "locations",
     "rack_roles",
@@ -147,14 +148,15 @@
 from .asns import ASNInitializer
 from .cables import CableInitializer
 from .circuit_types import CircuitTypeInitializer
 from .circuits import CircuitInitializer
 from .cluster_groups import ClusterGroupInitializer
 from .cluster_types import ClusterTypesInitializer
 from .clusters import ClusterInitializer
+from .config_templates import ConfigTemplateInitializer
 from .contact_groups import ContactGroupInitializer
 from .contact_roles import ContactRoleInitializer
 from .contacts import ContactInitializer
 from .custom_fields import CustomFieldInitializer
 from .custom_links import CustomLinkInitializer
 from .device_roles import DeviceRoleInitializer
 from .device_types import DeviceTypeInitializer
```

### Comparing `netbox_initializers-3.5.0/src/netbox_initializers/initializers/aggregates.py` & `netbox_initializers-3.5.1/src/netbox_initializers/initializers/aggregates.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.0/src/netbox_initializers/initializers/asns.py` & `netbox_initializers-3.5.1/src/netbox_initializers/initializers/asns.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.0/src/netbox_initializers/initializers/cables.py` & `netbox_initializers-3.5.1/src/netbox_initializers/initializers/cables.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.0/src/netbox_initializers/initializers/circuit_types.py` & `netbox_initializers-3.5.1/src/netbox_initializers/initializers/circuit_types.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.0/src/netbox_initializers/initializers/circuits.py` & `netbox_initializers-3.5.1/src/netbox_initializers/initializers/circuits.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.0/src/netbox_initializers/initializers/cluster_groups.py` & `netbox_initializers-3.5.1/src/netbox_initializers/initializers/cluster_groups.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.0/src/netbox_initializers/initializers/cluster_types.py` & `netbox_initializers-3.5.1/src/netbox_initializers/initializers/cluster_types.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.0/src/netbox_initializers/initializers/clusters.py` & `netbox_initializers-3.5.1/src/netbox_initializers/initializers/clusters.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.0/src/netbox_initializers/initializers/contact_groups.py` & `netbox_initializers-3.5.1/src/netbox_initializers/initializers/contact_groups.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.0/src/netbox_initializers/initializers/contact_roles.py` & `netbox_initializers-3.5.1/src/netbox_initializers/initializers/contact_roles.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.0/src/netbox_initializers/initializers/contacts.py` & `netbox_initializers-3.5.1/src/netbox_initializers/initializers/contacts.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.0/src/netbox_initializers/initializers/custom_fields.py` & `netbox_initializers-3.5.1/src/netbox_initializers/initializers/custom_fields.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.0/src/netbox_initializers/initializers/custom_links.py` & `netbox_initializers-3.5.1/src/netbox_initializers/initializers/custom_links.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.0/src/netbox_initializers/initializers/device_roles.py` & `netbox_initializers-3.5.1/src/netbox_initializers/initializers/device_roles.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.0/src/netbox_initializers/initializers/device_types.py` & `netbox_initializers-3.5.1/src/netbox_initializers/initializers/device_types.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.0/src/netbox_initializers/initializers/devices.py` & `netbox_initializers-3.5.1/src/netbox_initializers/initializers/devices.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 from dcim.models import Device, DeviceRole, DeviceType, Location, Platform, Rack, Site
+from extras.models import ConfigTemplate
 from tenancy.models import Tenant
 from virtualization.models import Cluster
 
 from . import BaseInitializer, register_initializer
 
 MATCH_PARAMS = ["device_type", "name", "site"]
 REQUIRED_ASSOCS = {
     "device_role": (DeviceRole, "name"),
     "device_type": (DeviceType, "model"),
     "site": (Site, "name"),
 }
 OPTIONAL_ASSOCS = {
-    "tenant": (Tenant, "name"),
-    "platform": (Platform, "name"),
-    "rack": (Rack, "name"),
     "cluster": (Cluster, "name"),
+    "config_template": (ConfigTemplate, "name"),
     "location": (Location, "name"),
+    "platform": (Platform, "name"),
+    "rack": (Rack, "name"),
+    "tenant": (Tenant, "name"),
 }
 
 
 class DeviceInitializer(BaseInitializer):
     data_file_name = "devices.yml"
 
     def load_data(self):
```

### Comparing `netbox_initializers-3.5.0/src/netbox_initializers/initializers/groups.py` & `netbox_initializers-3.5.1/src/netbox_initializers/initializers/groups.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.0/src/netbox_initializers/initializers/interfaces.py` & `netbox_initializers-3.5.1/src/netbox_initializers/initializers/interfaces.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.0/src/netbox_initializers/initializers/ip_addresses.py` & `netbox_initializers-3.5.1/src/netbox_initializers/initializers/ip_addresses.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.0/src/netbox_initializers/initializers/locations.py` & `netbox_initializers-3.5.1/src/netbox_initializers/initializers/locations.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.0/src/netbox_initializers/initializers/manufacturers.py` & `netbox_initializers-3.5.1/src/netbox_initializers/initializers/manufacturers.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.0/src/netbox_initializers/initializers/object_permissions.py` & `netbox_initializers-3.5.1/src/netbox_initializers/initializers/object_permissions.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.0/src/netbox_initializers/initializers/platforms.py` & `netbox_initializers-3.5.1/src/netbox_initializers/initializers/platforms.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.0/src/netbox_initializers/initializers/power_feeds.py` & `netbox_initializers-3.5.1/src/netbox_initializers/initializers/power_feeds.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.0/src/netbox_initializers/initializers/power_panels.py` & `netbox_initializers-3.5.1/src/netbox_initializers/initializers/power_panels.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.0/src/netbox_initializers/initializers/prefix_vlan_roles.py` & `netbox_initializers-3.5.1/src/netbox_initializers/initializers/prefix_vlan_roles.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.0/src/netbox_initializers/initializers/prefixes.py` & `netbox_initializers-3.5.1/src/netbox_initializers/initializers/prefixes.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.0/src/netbox_initializers/initializers/primary_ips.py` & `netbox_initializers-3.5.1/src/netbox_initializers/initializers/primary_ips.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.0/src/netbox_initializers/initializers/providers.py` & `netbox_initializers-3.5.1/src/netbox_initializers/initializers/providers.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.0/src/netbox_initializers/initializers/rack_roles.py` & `netbox_initializers-3.5.1/src/netbox_initializers/initializers/rack_roles.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.0/src/netbox_initializers/initializers/racks.py` & `netbox_initializers-3.5.1/src/netbox_initializers/initializers/racks.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.0/src/netbox_initializers/initializers/regions.py` & `netbox_initializers-3.5.1/src/netbox_initializers/initializers/regions.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.0/src/netbox_initializers/initializers/rirs.py` & `netbox_initializers-3.5.1/src/netbox_initializers/initializers/rirs.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.0/src/netbox_initializers/initializers/route_targets.py` & `netbox_initializers-3.5.1/src/netbox_initializers/initializers/route_targets.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.0/src/netbox_initializers/initializers/services.py` & `netbox_initializers-3.5.1/src/netbox_initializers/initializers/services.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.0/src/netbox_initializers/initializers/sites.py` & `netbox_initializers-3.5.1/src/netbox_initializers/initializers/sites.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.0/src/netbox_initializers/initializers/tags.py` & `netbox_initializers-3.5.1/src/netbox_initializers/initializers/tags.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.0/src/netbox_initializers/initializers/tenant_groups.py` & `netbox_initializers-3.5.1/src/netbox_initializers/initializers/tenant_groups.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.0/src/netbox_initializers/initializers/tenants.py` & `netbox_initializers-3.5.1/src/netbox_initializers/initializers/tenants.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.0/src/netbox_initializers/initializers/users.py` & `netbox_initializers-3.5.1/src/netbox_initializers/initializers/users.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.0/src/netbox_initializers/initializers/virtual_machines.py` & `netbox_initializers-3.5.1/src/netbox_initializers/initializers/virtual_machines.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.0/src/netbox_initializers/initializers/virtualization_interfaces.py` & `netbox_initializers-3.5.1/src/netbox_initializers/initializers/virtualization_interfaces.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.0/src/netbox_initializers/initializers/vlan_groups.py` & `netbox_initializers-3.5.1/src/netbox_initializers/initializers/vlan_groups.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.0/src/netbox_initializers/initializers/vlans.py` & `netbox_initializers-3.5.1/src/netbox_initializers/initializers/vlans.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.0/src/netbox_initializers/initializers/vrfs.py` & `netbox_initializers-3.5.1/src/netbox_initializers/initializers/vrfs.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.0/src/netbox_initializers/initializers/webhooks.py` & `netbox_initializers-3.5.1/src/netbox_initializers/initializers/webhooks.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.0/src/netbox_initializers/initializers/yaml/cables.yml` & `netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/cables.yml`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.0/src/netbox_initializers/initializers/yaml/contacts.yml` & `netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/contacts.yml`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.0/src/netbox_initializers/initializers/yaml/custom_fields.yml` & `netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/custom_fields.yml`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.0/src/netbox_initializers/initializers/yaml/device_types.yml` & `netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/device_types.yml`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.0/src/netbox_initializers/initializers/yaml/devices.yml` & `netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/devices.yml`

 * *Files 5% similar despite different names*

```diff
@@ -47,9 +47,11 @@
 # - name: server04
 #   device_role: server
 #   device_type: Other
 #   site: SING 1
 #   location: cage 101
 #   face: front
 #   position: 3
+#   config_template: configtemplate1
 #   custom_field_data:
 #     text_field: Description
+#
```

### Comparing `netbox_initializers-3.5.0/src/netbox_initializers/initializers/yaml/interfaces.yml` & `netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/interfaces.yml`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.0/src/netbox_initializers/initializers/yaml/ip_addresses.yml` & `netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/ip_addresses.yml`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.0/src/netbox_initializers/initializers/yaml/object_permissions.yml` & `netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/object_permissions.yml`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.0/src/netbox_initializers/initializers/yaml/prefixes.yml` & `netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/prefixes.yml`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.0/src/netbox_initializers/initializers/yaml/racks.yml` & `netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/racks.yml`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.0/src/netbox_initializers/initializers/yaml/sites.yml` & `netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/sites.yml`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.0/src/netbox_initializers/initializers/yaml/virtual_machines.yml` & `netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/virtual_machines.yml`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.0/src/netbox_initializers/initializers/yaml/vlan_groups.yml` & `netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/vlan_groups.yml`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.0/src/netbox_initializers/initializers/yaml/webhooks.yml` & `netbox_initializers-3.5.1/src/netbox_initializers/initializers/yaml/webhooks.yml`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.0/src/netbox_initializers/management/commands/copy_initializers_examples.py` & `netbox_initializers-3.5.1/src/netbox_initializers/management/commands/copy_initializers_examples.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.0/src/netbox_initializers/management/commands/load_initializer_data.py` & `netbox_initializers-3.5.1/src/netbox_initializers/management/commands/load_initializer_data.py`

 * *Files identical despite different names*

### Comparing `netbox_initializers-3.5.0/PKG-INFO` & `netbox_initializers-3.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-initializers
-Version: 3.5.0
+Version: 3.5.1
 Summary: Load initial data into Netbox
 Home-page: https://github.com/tobiasge/netbox-initializers
 License: Apache-2.0
 Author: Tobias Genannt
 Author-email: tobias.genannt@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Environment :: Plugins
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Networking
 Classifier: Topic :: System :: Systems Administration
-Requires-Dist: ruamel.yaml (==0.17.21)
+Requires-Dist: ruamel.yaml (==0.17.31)
 Project-URL: Repository, https://github.com/tobiasge/netbox-initializers
 Description-Content-Type: text/markdown
 
 # Netbox Initializers Plugin
 
 Load data from YAML files into Netbox
 
@@ -55,11 +55,11 @@
 
 ## Netbox Docker image
 
 The initializers where a part of the Docker image and where then extracted into a Netbox plugin. This was done to split the release cycle of the initializers and the image.
 To use the new plugin in a the Netbox Docker image, it musst be installad into the image. To this, the following example can be used as a starting point:
 
 ```dockerfile
-FROM netboxcommunity/netbox:v3.4
+FROM netboxcommunity/netbox:v3.5
 RUN /opt/netbox/venv/bin/pip install "netbox-initializers==3.5.*"
 ```
```

