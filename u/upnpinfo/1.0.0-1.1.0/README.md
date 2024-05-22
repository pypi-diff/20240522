# Comparing `tmp/upnpinfo-1.0.0.tar.gz` & `tmp/upnpinfo-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upnpinfo-1.0.0.tar", last modified: Fri May 10 00:38:42 2024, max compression
+gzip compressed data, was "upnpinfo-1.1.0.tar", last modified: Wed May 22 02:35:25 2024, max compression
```

## Comparing `upnpinfo-1.0.0.tar` & `upnpinfo-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 mike       (501) staff       (20)        0 2024-05-10 00:38:42.596489 upnpinfo-1.0.0/
--rw-r--r--   0 mike       (501) staff       (20)     1067 2024-05-09 23:37:31.000000 upnpinfo-1.0.0/LICENSE
--rw-r--r--   0 mike       (501) staff       (20)     3161 2024-05-10 00:38:42.596277 upnpinfo-1.0.0/PKG-INFO
--rw-r--r--   0 mike       (501) staff       (20)     1343 2024-05-10 00:27:44.000000 upnpinfo-1.0.0/README.md
--rw-r--r--   0 mike       (501) staff       (20)      794 2024-05-10 00:37:36.000000 upnpinfo-1.0.0/pyproject.toml
--rw-r--r--   0 mike       (501) staff       (20)       38 2024-05-10 00:38:42.596542 upnpinfo-1.0.0/setup.cfg
-drwxr-xr-x   0 mike       (501) staff       (20)        0 2024-05-10 00:38:42.593274 upnpinfo-1.0.0/src/
-drwxr-xr-x   0 mike       (501) staff       (20)        0 2024-05-10 00:38:42.594513 upnpinfo-1.0.0/src/upnpinfo/
--rw-r--r--   0 mike       (501) staff       (20)      148 2024-05-09 07:41:05.000000 upnpinfo-1.0.0/src/upnpinfo/__init__.py
--rw-r--r--   0 mike       (501) staff       (20)     7619 2024-05-09 03:55:09.000000 upnpinfo-1.0.0/src/upnpinfo/cli.py
--rw-r--r--   0 mike       (501) staff       (20)     1946 2024-05-09 07:33:54.000000 upnpinfo-1.0.0/src/upnpinfo/upnp.py
-drwxr-xr-x   0 mike       (501) staff       (20)        0 2024-05-10 00:38:42.595829 upnpinfo-1.0.0/src/upnpinfo.egg-info/
--rw-r--r--   0 mike       (501) staff       (20)     3161 2024-05-10 00:38:42.000000 upnpinfo-1.0.0/src/upnpinfo.egg-info/PKG-INFO
--rw-r--r--   0 mike       (501) staff       (20)      334 2024-05-10 00:38:42.000000 upnpinfo-1.0.0/src/upnpinfo.egg-info/SOURCES.txt
--rw-r--r--   0 mike       (501) staff       (20)        1 2024-05-10 00:38:42.000000 upnpinfo-1.0.0/src/upnpinfo.egg-info/dependency_links.txt
--rw-r--r--   0 mike       (501) staff       (20)       42 2024-05-10 00:38:42.000000 upnpinfo-1.0.0/src/upnpinfo.egg-info/entry_points.txt
--rw-r--r--   0 mike       (501) staff       (20)       63 2024-05-10 00:38:42.000000 upnpinfo-1.0.0/src/upnpinfo.egg-info/requires.txt
--rw-r--r--   0 mike       (501) staff       (20)        9 2024-05-10 00:38:42.000000 upnpinfo-1.0.0/src/upnpinfo.egg-info/top_level.txt
+drwxr-xr-x   0 mike       (501) staff       (20)        0 2024-05-22 02:35:25.479210 upnpinfo-1.1.0/
+-rw-r--r--   0 mike       (501) staff       (20)     1067 2024-05-09 23:37:31.000000 upnpinfo-1.1.0/LICENSE
+-rw-r--r--   0 mike       (501) staff       (20)     8054 2024-05-22 02:35:25.479008 upnpinfo-1.1.0/PKG-INFO
+-rw-r--r--   0 mike       (501) staff       (20)     6236 2024-05-22 02:16:24.000000 upnpinfo-1.1.0/README.md
+-rw-r--r--   0 mike       (501) staff       (20)      794 2024-05-22 02:16:24.000000 upnpinfo-1.1.0/pyproject.toml
+-rw-r--r--   0 mike       (501) staff       (20)       38 2024-05-22 02:35:25.479250 upnpinfo-1.1.0/setup.cfg
+drwxr-xr-x   0 mike       (501) staff       (20)        0 2024-05-22 02:35:25.471743 upnpinfo-1.1.0/src/
+drwxr-xr-x   0 mike       (501) staff       (20)        0 2024-05-22 02:35:25.472984 upnpinfo-1.1.0/src/upnpinfo/
+-rw-r--r--   0 mike       (501) staff       (20)       29 2024-05-22 02:16:24.000000 upnpinfo-1.1.0/src/upnpinfo/__init__.py
+-rw-r--r--   0 mike       (501) staff       (20)     1635 2024-05-22 02:16:24.000000 upnpinfo-1.1.0/src/upnpinfo/cli.py
+-rw-r--r--   0 mike       (501) staff       (20)     8164 2024-05-22 02:16:24.000000 upnpinfo-1.1.0/src/upnpinfo/display.py
+-rw-r--r--   0 mike       (501) staff       (20)     3306 2024-05-22 02:16:24.000000 upnpinfo-1.1.0/src/upnpinfo/upnp.py
+drwxr-xr-x   0 mike       (501) staff       (20)        0 2024-05-22 02:35:25.478530 upnpinfo-1.1.0/src/upnpinfo.egg-info/
+-rw-r--r--   0 mike       (501) staff       (20)     8054 2024-05-22 02:35:25.000000 upnpinfo-1.1.0/src/upnpinfo.egg-info/PKG-INFO
+-rw-r--r--   0 mike       (501) staff       (20)      360 2024-05-22 02:35:25.000000 upnpinfo-1.1.0/src/upnpinfo.egg-info/SOURCES.txt
+-rw-r--r--   0 mike       (501) staff       (20)        1 2024-05-22 02:35:25.000000 upnpinfo-1.1.0/src/upnpinfo.egg-info/dependency_links.txt
+-rw-r--r--   0 mike       (501) staff       (20)       42 2024-05-22 02:35:25.000000 upnpinfo-1.1.0/src/upnpinfo.egg-info/entry_points.txt
+-rw-r--r--   0 mike       (501) staff       (20)       63 2024-05-22 02:35:25.000000 upnpinfo-1.1.0/src/upnpinfo.egg-info/requires.txt
+-rw-r--r--   0 mike       (501) staff       (20)        9 2024-05-22 02:35:25.000000 upnpinfo-1.1.0/src/upnpinfo.egg-info/top_level.txt
```

### Comparing `upnpinfo-1.0.0/LICENSE` & `upnpinfo-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `upnpinfo-1.0.0/pyproject.toml` & `upnpinfo-1.1.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 where = ["./src"]
 
 [project]
 name = "upnpinfo"
-version = "1.0.0"
+version = "1.1.0"
 description = "Retrieve UPnP device information from the local network"
 authors = [
     { name = "Mike Joblin" },
 ]
 license = { file = "LICENSE" }
 readme = "README.md"
 classifiers = [
```

### Comparing `upnpinfo-1.0.0/src/upnpinfo/cli.py` & `upnpinfo-1.1.0/src/upnpinfo/display.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,97 +1,49 @@
+from __future__ import annotations
+
 import json
 from urllib.parse import urlparse
 
 import click
 from rich.columns import Columns
-from rich.console import Console
 from rich.table import box, Table
 from rich.text import Text
-from rich.traceback import install
 
-from upnpinfo import (
+from upnpinfo.upnp import (
     device_summary,
     discover_upnp_devices,
     get_upnp_device,
-    service_actions,
+    device_service_details,
 )
 
 
-install(suppress=[click])
-
-
-@click.command()
-@click.option(
-    "--timeout",
-    "-t",
-    help="UPnP discovery timeout (seconds).",
-    metavar="SECS",
-    type=click.INT,
-    default=1,
-    show_default=True,
-)
-@click.option(
-    "--device",
-    "-d",
-    help="Device name, UDN, or UPnP location URL.",
-    metavar="DEVICE",
-    type=click.STRING,
-)
-@click.option(
-    "--no-color",
-    help="Disable color.",
-    is_flag=True,
-    default=False,
-)
-@click.option(
-    "--json",
-    "as_json",
-    help="Display results as JSON.",
-    is_flag=True,
-    default=False,
-)
-def cli(timeout, device, no_color, as_json):
-    """
-    Retrieves UPnP device information from the local network.
-
-    Defaults to showing a summary of all devices found on the local network
-    using UPnP discovery. Use --device to retrieve detailed information on a
-    specific device.
-    """
-    console = Console(no_color=no_color, highlight=not no_color)
-
-    if device:
-        handle_show_single_device(console, device, timeout, no_color, as_json)
-    else:
-        handle_show_all_devices(console, timeout, no_color, as_json)
-
-
-def handle_show_all_devices(console, timeout, plain_output, as_json):
-    """Discover UPnP devices on the local network and display a summary."""
+def display_all_devices(
+    console, script_name, wanted_device_types, timeout, plain_output, as_json
+):
+    """Display a summary of all UPnP devices found on the local network."""
     with console.status("Discovering UPnP devices..."):
         devices = discover_upnp_devices(timeout=timeout)
 
-    unique_devices = []  # Remove duplicate devices (based on UDN)
-    device_udns = []
+    if len(devices) <= 0:
+        console.print("No UPnP devices found.")
 
-    for device in devices:
-        # if device.udn not in device_udns:
-        if device.udn not in device_udns:
-            unique_devices.append(device)
-            device_udns.append(device.udn)
+    # Exclude unwanted device types
+    filtered_devices = [
+        device for device in devices if _device_type_match(device, wanted_device_types)
+    ]
 
-    if len(unique_devices) <= 0:
-        console.print("No UPnP devices found.")
+    if len(filtered_devices) <= 0:
+        console.print("No matching UPnP devices found.")
 
         return
 
     # Create a list of unique device information summary dicts
     device_summaries = []
 
-    for device in unique_devices:
+    for device in filtered_devices:
         device_summaries.append(device_summary(device))
 
     if as_json:
         # Dump the device summaries as JSON
         console.print(json.dumps(device_summaries, indent=4))
     else:
         # Display a table of unique device information summaries
@@ -114,60 +66,75 @@
         ):
             # Extract just the hostname from the full location URL
             parsed_location = urlparse(device["location"])
             address = parsed_location.hostname
 
             # Extract just the device type name from the full device type
             # e.g. urn:schemas-upnp-org:device:MediaRenderer:1 -> MediaRenderer
-            device_type = device["device_type"]
+            found_device_types = device["device_type"]
 
             try:
-                device_type = device_type.split(":")[3]
+                found_device_types = found_device_types.split(":")[3]
             except IndexError:
                 pass
 
             table.add_row(
                 device["friendly_name"] or "-",
                 device["manufacturer"] or "-",
                 device["model_description"] or "-",
                 device["model_name"] or "-",
-                device_type or "-",
+                found_device_types or "-",
                 address or "-",
             )
 
         # Display the table and a footer message showing how to get detailed
         # info on a device
 
-        script_name = click.get_current_context().info_name
-
         console.print(
             table,
-            Text(f"Run \"{script_name} --device '<name>'\" to view device details.\n"),
+            Text(f"Run \"{script_name} '<name>'\" to view device details.\n"),
         )
 
 
-def handle_show_single_device(console, device_input, timeout, plain_output, as_json):
+def display_single_device(
+    console, device_input, wanted_device_types, timeout, plain_output, as_json
+):
     """Display detailed information on a single UPnP device."""
+    found_multiple = False
+
     # Check if the input is a URL. If it's not then we assume it's a device
     # name and attempt to find that name in the list of all discovered devices.
     device_input_as_url = urlparse(device_input)
 
     if device_input_as_url.hostname is None:
-        # See if the device input was a device name or a UDN
+        # See if the device input was a device friendly name or a UDN
         with console.status(f"Finding device: {device_input} ..."):
             all_devices = discover_upnp_devices(timeout=timeout)
 
         try:
-            location = [
+            locations = [
                 device
                 for device in all_devices
-                if device.friendly_name == device_input or device.udn == device_input
-            ][0].location
+                if (device.friendly_name == device_input or device.udn == device_input)
+                and _device_type_match(device, wanted_device_types)
+            ]
+
+            found_multiple = len(locations) > 1
+
+            location = locations[0].location
         except (IndexError, AttributeError):
-            console.print(f"UPnP device not found: {device_input}")
+            msg = f"UPnP device not found: {device_input}"
+
+            if len(wanted_device_types) > 0:
+                msg += f" (type: {', '.join(wanted_device_types)})"
+
+            console.print(msg)
+            console.print(
+                "If the device specifier and optional type are valid, try a longer --timeout"
+            )
 
             return
     else:
         # Device input was a URL
         location = device_input
 
     try:
@@ -175,15 +142,15 @@
         with console.status(f"Retrieving details for device: {device_input} ..."):
             device = get_upnp_device(location)
     except Exception as e:
         console.print(e)
 
         return
 
-    actions = service_actions(device)
+    service_details = device_service_details(device)
 
     if as_json:
         # Dump the device details as JSON
         console.print(json.dumps(device_summary(device), indent=4))
     else:
         # Prepare a table of device details
         details_table = Table(
@@ -196,45 +163,83 @@
         details_table.add_column("Field", justify="right")
         details_table.add_column(
             "Value", justify="left", style=None if plain_output else "bold"
         )
 
         details_table.add_row("Friendly name:", device.friendly_name or "-")
         details_table.add_row("UDN:", device.udn or "-")
-        details_table.add_row("Device type:", device.device_type or "-")
+        details_table.add_row("Device type:", device.device_type or "-", style=None)
         details_table.add_row("Manufacturer:", device.manufacturer or "-")
         details_table.add_row("Manufacturer URL:", device.manufacturer_url or "-")
         details_table.add_row("Model name:", device.model_name or "-")
         details_table.add_row("Model number:", device.model_number or "-")
         details_table.add_row("Model description:", device.model_description or "-")
         details_table.add_row("Location:", device.location or "-")
-        details_table.add_row("Services:", ", ".join(sorted(actions.keys())) or "-")
+        details_table.add_row(
+            "Services:", ", ".join(sorted(service_details.keys())) or "-"
+        )
 
         # Prepare columns showing the actions available for each service
         service_columns = []
 
-        for service_name in actions.keys():
+        for service_name in service_details.keys():
             service_table = Table(
                 show_header=True,
                 header_style=None if plain_output else "bold",
                 box=box.SIMPLE_HEAD,
                 pad_edge=False,
             )
 
             service_table.add_column(service_name)
 
-            for service_action in actions[service_name]:
-                service_table.add_row(service_action)
+            # Add the actions for this service
+            actions = service_details[service_name]["actions"]
+
+            if len(actions) > 0:
+                for action in actions:
+                    service_table.add_row(action)
+            else:
+                service_table.add_row("No actions")
+
+            # Add the URL to retrieve details for this service
+            scpd_url = service_details[service_name]["scpd_url"]
+
+            if scpd_url is not None:
+                service_table.add_row()
+                service_table.add_row(scpd_url)
 
             service_columns.append(service_table)
 
         # Display the details table and (if present) the service action tables
         if len(service_columns) > 0:
             console.print(
                 details_table, Text(" Service actions:"), Columns(service_columns)
             )
         else:
             console.print(details_table)
 
+        if found_multiple:
+            console.print(
+                "Note: Only the first matching device is displayed; "
+                + "use --type to display a different device for this host."
+            )
+
 
-if __name__ == "__main__":
-    cli()
+def _device_type_match(device, device_types: tuple[click.STRING]) -> bool:
+    """Determine whether the given device's type is included in device_types.
+
+    If device_types is an empty tuple, then the device is assumed to match.
+    """
+    if len(device_types) <= 0:
+        return True
+
+    # This isn't strictly checking
+    return (
+        len(
+            [
+                device_type
+                for device_type in device_types
+                if device.device_type.split(":")[3] == device_type
+            ]
+        )
+        > 0
+    )
```

