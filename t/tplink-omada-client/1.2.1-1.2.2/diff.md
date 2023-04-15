# Comparing `tmp/tplink_omada_client-1.2.1.tar.gz` & `tmp/tplink_omada_client-1.2.2.tar.gz`

## Comparing `tplink_omada_client-1.2.1.tar` & `tplink_omada_client-1.2.2.tar`

### file list

```diff
@@ -1,34 +1,35 @@
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.1/.pylintrc
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.1/Dockerfile.dev
--rw-r--r--   0        0        0     3817 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.1/package_constraints.txt
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.1/requirements.txt
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.1/requirements_test.txt
--rwxr-xr-x   0        0        0     3375 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.1/sample_client.py
--rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.1/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.1/.github/workflows/python-package.yml
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.1/.vscode/launch.json
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.1/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.1/src/tplink_omada_client/__init__.py
--rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.1/src/tplink_omada_client/definitions.py
--rw-r--r--   0        0        0    14464 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.1/src/tplink_omada_client/devices.py
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.1/src/tplink_omada_client/exceptions.py
--rw-r--r--   0        0        0     6875 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.1/src/tplink_omada_client/omadaapiconnection.py
--rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.1/src/tplink_omada_client/omadaclient.py
--rw-r--r--   0        0        0    10480 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.1/src/tplink_omada_client/omadasiteclient.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.1/src/tplink_omada_client/py.typed
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.1/src/tplink_omada_client/cli/__init__.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.1/src/tplink_omada_client/cli/__main__.py
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.1/src/tplink_omada_client/cli/command_devices.py
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.1/src/tplink_omada_client/cli/command_switch.py
--rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.1/src/tplink_omada_client/cli/command_switches.py
--rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.1/src/tplink_omada_client/cli/command_target.py
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.1/src/tplink_omada_client/cli/command_targets.py
--rw-r--r--   0        0        0     2376 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.1/src/tplink_omada_client/cli/config.py
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.1/src/tplink_omada_client/cli/util.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.1/tests/conftest.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.1/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.1/LICENSE
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.1/README.md
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.2/.pylintrc
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.2/Dockerfile.dev
+-rw-r--r--   0        0        0     3817 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.2/package_constraints.txt
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.2/requirements.txt
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.2/requirements_test.txt
+-rwxr-xr-x   0        0        0     3375 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.2/sample_client.py
+-rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.2/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.2/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.2/.vscode/launch.json
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.2/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.2/src/tplink_omada_client/__init__.py
+-rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.2/src/tplink_omada_client/definitions.py
+-rw-r--r--   0        0        0    14103 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.2/src/tplink_omada_client/devices.py
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.2/src/tplink_omada_client/exceptions.py
+-rw-r--r--   0        0        0     6875 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.2/src/tplink_omada_client/omadaapiconnection.py
+-rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.2/src/tplink_omada_client/omadaclient.py
+-rw-r--r--   0        0        0    10480 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.2/src/tplink_omada_client/omadasiteclient.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.2/src/tplink_omada_client/py.typed
+-rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.2/src/tplink_omada_client/cli/__init__.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.2/src/tplink_omada_client/cli/__main__.py
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.2/src/tplink_omada_client/cli/command_default.py
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.2/src/tplink_omada_client/cli/command_devices.py
+-rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.2/src/tplink_omada_client/cli/command_switch.py
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.2/src/tplink_omada_client/cli/command_switches.py
+-rw-r--r--   0        0        0     1977 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.2/src/tplink_omada_client/cli/command_target.py
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.2/src/tplink_omada_client/cli/command_targets.py
+-rw-r--r--   0        0        0     3386 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.2/src/tplink_omada_client/cli/config.py
+-rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.2/src/tplink_omada_client/cli/util.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.2/tests/conftest.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.2/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.2/LICENSE
+-rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.2/README.md
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0     2910 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.2/PKG-INFO
```

### Comparing `tplink_omada_client-1.2.1/Dockerfile.dev` & `tplink_omada_client-1.2.2/Dockerfile.dev`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.2.1/package_constraints.txt` & `tplink_omada_client-1.2.2/package_constraints.txt`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.2.1/sample_client.py` & `tplink_omada_client-1.2.2/sample_client.py`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.2.1/.devcontainer/devcontainer.json` & `tplink_omada_client-1.2.2/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.2.1/.github/workflows/python-package.yml` & `tplink_omada_client-1.2.2/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.2.1/.github/workflows/python-publish.yml` & `tplink_omada_client-1.2.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.2.1/src/tplink_omada_client/definitions.py` & `tplink_omada_client-1.2.2/src/tplink_omada_client/definitions.py`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.2.1/src/tplink_omada_client/devices.py` & `tplink_omada_client-1.2.2/src/tplink_omada_client/devices.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 """
 Definitions for Omada device objects
 
 APs, Switches and Routers
 """
-from typing import Any, Dict, List, Optional
+from typing import Any, List, Optional
 from .definitions import (
     BandwidthControl,
     DeviceStatus,
     DeviceStatusCategory,
     Eth802Dot1X,
     LinkSpeed,
     LinkStatus,
     PoEMode,
     PortType,
 )
 
+class OmadaApiData:
+    def __init__(self, data: dict[str, Any]):
+        self._data = data
 
-class OmadaDevice:
-    """Details of a device connected to the controller"""
+    @property
+    def raw_data(self) -> dict[str, Any]:
+        return self._data
 
-    def __init__(self, data: Dict[str, Any]):
-        self._data = data
+
+class OmadaDevice(OmadaApiData):
+    """Details of a device connected to the controller"""
 
     @property
     def type(self) -> str:
         """The type of the device. Its value can be "ap", "gateway", and "switch"."""
         return self._data["type"]
 
     @property
@@ -88,20 +93,17 @@
 
     @property
     def fw_download(self) -> bool:
         """True, if a firmware upgrade is being downloaded."""
         return self._data["fwDownload"]
 
 
-class OmadaLink:
+class OmadaLink(OmadaApiData):
     """Up/Downlink connection from a switch/ap device."""
 
-    def __init__(self, data: Dict[str, Any]):
-        self._data = data
-
     @property
     def mac(self) -> str:
         """The MAC of the linked device."""
         return self._data["mac"]
 
     @property
     def name(self) -> str:
@@ -133,20 +135,17 @@
         return self._data["model"]
 
 
 class OmadaUplink(OmadaLink):
     """Uplink connection from a switch/ap device."""
 
 
-class OmadaPortStatus:
+class OmadaPortStatus(OmadaApiData):
     """Status information for a switch port."""
 
-    def __init__(self, data: Dict[str, Any]):
-        self._data = data
-
     @property
     def link_status(self) -> LinkStatus:
         """Port's link status."""
         return self._data["linkStatus"]
 
     @property
     def link_speed(self) -> LinkSpeed:
@@ -177,20 +176,17 @@
 
     @property
     def stp_discarding(self) -> bool:
         """Stp blocking status in spanning tree."""
         return self._data["stpDiscarding"]
 
 
-class OmadaSwitchPort:
+class OmadaSwitchPort(OmadaApiData):
     """Port on a switch/gateway device."""
 
-    def __init__(self, data: Dict[str, Any]):
-        self._data = data
-
     @property
     def port(self) -> int:
         """The port's number."""
         return self._data["port"]
 
     @property
     def name(self) -> str:
@@ -219,20 +215,17 @@
 
     @property
     def port_status(self) -> OmadaPortStatus:
         """Status of the port."""
         return OmadaPortStatus(self._data["portStatus"])
 
 
-class OmadaSwitchDeviceCaps:
+class OmadaSwitchDeviceCaps(OmadaApiData):
     """Capabilities of a switch."""
 
-    def __init__(self, data: Dict[str, Any]):
-        self._data = data
-
     @property
     def poe_ports(self) -> int:
         """Number of PoE ports supported."""
         return self._data["poePortNum"]
 
     @property
     def supports_poe(self) -> bool:
@@ -280,20 +273,17 @@
 
     @property
     def device_capabilities(self) -> OmadaSwitchDeviceCaps:
         """Capabilities of the switch."""
         return OmadaSwitchDeviceCaps(self._data["devCap"])
 
 
-class OmadaAccesPointLanPortSettings:
+class OmadaAccesPointLanPortSettings(OmadaApiData):
     """A LAN port on an access point."""
 
-    def __init__(self, data: Dict[str, Any]):
-        self._data = data
-
     @property
     def port_name(self) -> str:
         """Name of the port - can't be edited"""
         return self._data["lanPort"]
 
     @property
     def supports_vlan(self) -> bool:
@@ -445,20 +435,17 @@
 
     @property
     def port_isolation_enabled(self) -> bool:
         """Port isolation (Danger!)"""
         return self._data["portIsolationEnable"]
 
 
-class OmadaPortProfile:
+class OmadaPortProfile(OmadaApiData):
     """Definition of a switch port configuration profile."""
 
-    def __init__(self, data: Dict[str, Any]):
-        self._data = data
-
     @property
     def profile_id(self) -> str:
         """ID of this profile."""
         return self._data["id"]
 
     @property
     def site(self) -> str:
@@ -507,32 +494,26 @@
 
     @property
     def port_isolation_enabled(self) -> bool:
         """Port isolation (Danger!)"""
         return self._data["portIsolationEnable"]
 
 
-class OmadaInterfaceDetails:
+class OmadaInterfaceDetails(OmadaApiData):
     """Basic UI Information about controller."""
 
-    def __init__(self, data: Dict[str, Any]):
-        self._data = data
-
     @property
     def controller_name(self) -> str:
         """Display name of the controller."""
         return self._data["controllerName"]
 
 
-class OmadaFirmwareUpdate:
+class OmadaFirmwareUpdate(OmadaApiData):
     """Status information for a switch port."""
 
-    def __init__(self, data: Dict[str, Any]):
-        self._data = data
-
     @property
     def current_version(self) -> str:
         """Device's current firmware version."""
         return self._data["curFwVer"]
 
     @property
     def latest_version(self) -> str:
```

### Comparing `tplink_omada_client-1.2.1/src/tplink_omada_client/exceptions.py` & `tplink_omada_client-1.2.2/src/tplink_omada_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.2.1/src/tplink_omada_client/omadaapiconnection.py` & `tplink_omada_client-1.2.2/src/tplink_omada_client/omadaapiconnection.py`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.2.1/src/tplink_omada_client/omadaclient.py` & `tplink_omada_client-1.2.2/src/tplink_omada_client/omadaclient.py`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.2.1/src/tplink_omada_client/omadasiteclient.py` & `tplink_omada_client-1.2.2/src/tplink_omada_client/omadasiteclient.py`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.2.1/src/tplink_omada_client/cli/__init__.py` & `tplink_omada_client-1.2.2/src/tplink_omada_client/cli/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,36 +8,39 @@
 
 from . import (
     command_devices,
     command_switch,
     command_switches,
     command_target,
     command_targets,
+    command_default
 )
 
 def main(argv: Union[Sequence[str], None] = None) -> int:
     """Entry point for Omada CLI"""
     if argv is None:
         argv = sys.argv[1:]
     parser = argparse.ArgumentParser()
     parser.add_argument(
         '-t', '--target',
         help="The target Omada controller",
+        default=""
     )
 
     subparsers = parser.add_subparsers(
         title='Available commands',
         metavar='command',
     )
 
     command_devices.arg_parser(subparsers)
     command_switch.arg_parser(subparsers)
     command_switches.arg_parser(subparsers)
     command_target.arg_parser(subparsers)
     command_targets.arg_parser(subparsers)
+    command_default.arg_parser(subparsers)
 
     try:
         args = parser.parse_args(args=argv)
         if "func" in args:
             return asyncio.run(args.func(vars(args)))
         parser.print_help()
         return 1
```

### Comparing `tplink_omada_client-1.2.1/src/tplink_omada_client/cli/command_devices.py` & `tplink_omada_client-1.2.2/src/tplink_omada_client/cli/command_default.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,22 @@
-"""Implementation for 'devices' command"""
+"""Implementation of 'default' command"""
+from argparse import _SubParsersAction, ArgumentError
+import getpass
 
-from argparse import _SubParsersAction
-
-from .config import get_target_config, to_omada_connection
 from .util import assert_target_argument
+from .config import ControllerConfig, set_default_target, to_omada_connection, get_target_config
 
-async def command_devices(args) -> int:
-    """Executes 'devices' command"""
-    controller = assert_target_argument(args)
-    config = get_target_config(controller)
+async def command_target(args) -> int:
+    """Executes 'default' command"""
+    target = assert_target_argument(args)
+    config = get_target_config(target)
 
-    async with to_omada_connection(config) as client:
-        site_client = await client.get_site_client(config.site)
-        for device in await site_client.get_devices():
-            print(f"{device.mac} {device.ip_address:>15} {device.type:>6}  {device.name:20} {device.model_display_name}")
+    set_default_target(target)
     return 0
 
 def arg_parser(subparsers: _SubParsersAction) -> None:
-    """Configures arguments parser for 'devices' command"""
-    devices_parser = subparsers.add_parser(
-        "devices",
-        aliases=['d'],
-        help="Lists devices managed by Omada Controller")
-    devices_parser.set_defaults(func=command_devices)
+    """Configures argument parser for 'default' command"""
+    set_parser = subparsers.add_parser(
+        "default",
+        help="Sets the default target",
+    )
+    set_parser.set_defaults(func=command_target)
```

### Comparing `tplink_omada_client-1.2.1/src/tplink_omada_client/cli/command_switch.py` & `tplink_omada_client-1.2.2/src/tplink_omada_client/cli/command_switch.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 """Implementation for 'switch' command"""
 
 from argparse import ArgumentParser
 
 from .config import get_target_config, to_omada_connection
-from .util import assert_target_argument
+from .util import dump_raw_data, get_mac, get_target_argument
 
 async def command_switch(args) -> int:
     """Executes 'switch' command"""
-    controller = assert_target_argument(args)
+    controller = get_target_argument(args)
     config = get_target_config(controller)
 
     async with to_omada_connection(config) as client:
         site_client = await client.get_site_client(config.site)
-        switch = await site_client.get_switch(args['mac'])
+        mac = await get_mac(site_client, args['mac'])
+        switch = await site_client.get_switch(mac)
         print(f"Name: {switch.name}")
         print(f"Address: {switch.mac} ({switch.ip_address})")
         print(f"Ports: {switch.number_of_ports}")
         print(f"Supports PoE: {switch.device_capabilities.supports_poe}")
         if switch.device_capabilities.supports_poe:
             print(f"PoE ports: {switch.device_capabilities.poe_ports}")
         print(f"Model: {switch.model_display_name}")
@@ -25,21 +26,25 @@
         if switch.uplink:
             print(f"Uplink switch: {switch.uplink.mac} {switch.uplink.name}")
         if len(switch.downlink) > 0:
             print("Downlink devices:")
             for downlink in switch.downlink:
                 print(f"- {downlink.mac} {downlink.name}")
 
+        dump_raw_data(args, switch)
+
     return 0
 
 def arg_parser(subparsers) -> None:
     """Configures arguments parser for 'switches' command"""
     switch_parser: ArgumentParser = subparsers.add_parser(
         "switch",
         help="Shows details about the specified switch"
     )
     switch_parser.set_defaults(func=command_switch)
 
     switch_parser.add_argument(
         "mac",
-        help="The MAC address of the switch",
+        help="The MAC address or name of the switch",
     )
+    switch_parser.add_argument('-d', '--dump', help="Output raw device information",  action='store_true')
+
```

### Comparing `tplink_omada_client-1.2.1/src/tplink_omada_client/cli/command_switches.py` & `tplink_omada_client-1.2.2/src/tplink_omada_client/cli/command_switches.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Implementation for 'switches' command"""
 
 from argparse import _SubParsersAction
 
 from .config import get_target_config, to_omada_connection
-from .util import assert_target_argument
+from .util import dump_raw_data, get_target_argument
 
 async def command_switches(args) -> int:
     """Executes 'switches' command"""
-    controller = assert_target_argument(args)
+    controller = get_target_argument(args)
     config = get_target_config(controller)
 
     async with to_omada_connection(config) as client:
         site_client = await client.get_site_client(config.site)
         for switch in await site_client.get_switches():
             print(f"{switch.mac} {switch.ip_address:>15}  {switch.name:20} ", end="")
             for port in switch.ports:
@@ -21,17 +21,20 @@
                     print("\u2611", end="")
                 else:
                     print("\u2610", end="")
                 if port.port_status.poe_active:
                     print("\u26a1", end="")
                 else:
                     print("  ", end="")
+
+            dump_raw_data(args, switch)
             print()
     return 0
 
 def arg_parser(subparsers: _SubParsersAction) -> None:
     """Configures arguments parser for 'switches' command"""
     switches_parser = subparsers.add_parser(
         "switches",
         aliases=['s'],
         help="Lists switches managed by Omada Controller")
     switches_parser.set_defaults(func=command_switches)
+    switches_parser.add_argument('-d', '--dump', help="Output raw device information",  action='store_true')
```

### Comparing `tplink_omada_client-1.2.1/src/tplink_omada_client/cli/command_target.py` & `tplink_omada_client-1.2.2/src/tplink_omada_client/cli/command_target.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 """Implementation of 'target' command"""
-from argparse import _SubParsersAction
+from argparse import _SubParsersAction, ArgumentError
 import getpass
+import json
 
-from .util import assert_target_argument
+from .util import get_target_argument
 from .config import ControllerConfig, set_target_config, to_omada_connection
 
 async def command_target(args) -> int:
     """Executes 'target' command"""
-    target = assert_target_argument(args)
+    target = get_target_argument(args)
+
     if args['password']:
         password = args['password']
     else:
         password = getpass.getpass()
     config = ControllerConfig(
         url=args['url'],
         username=args['username'],
         password=password,
         site=args['site'],
     )
+    
     # Connect to controller to validate config
     async with to_omada_connection(config) as client:
         name = await client.get_controller_name()
         for site in await client.get_sites():
             if args['site'] == site.name:
                 print(f"Set target {target} to controller {name} and site {site.name}")
-                set_target_config(target, config)
+                set_target_config(target, config, args['set_default'])
 
-    return 1
+    return 0
 
 def arg_parser(subparsers: _SubParsersAction) -> None:
     """Configures argument parser for 'target' command"""
     set_parser = subparsers.add_parser(
         "target",
         help="Add Omada Controller to list of targets",
     )
@@ -50,8 +53,13 @@
         help="The user's password, password will be prompted if not provided",
     )
     set_parser.add_argument(
         '--site',
         help="The Omada site to user",
         default = "Default",
     )
+    set_parser.add_argument(
+        '-sd',
+        '--set-default',
+        help="Set this target as the default",
+        action='store_true')
```

### Comparing `tplink_omada_client-1.2.1/src/tplink_omada_client/cli/command_targets.py` & `tplink_omada_client-1.2.2/src/tplink_omada_client/cli/command_targets.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 from .config import (
     get_targets,
 )
 
 async def command_targets(args) -> int: # pylint: disable=unused-argument
     """Executes 'targets' command"""
     controllers = get_targets()
-    for (controller, url) in controllers:
-        print(f"{controller:15} {url}")
+    for (controller, url, is_default) in controllers:
+        print(f"{('*' if is_default else' ')} {controller:15} {url}")
     return 0
 
 def arg_parser(subparsers: _SubParsersAction) -> None:
     """Configures argument parser for 'targets' command"""
     # targets
     controllers_parser = subparsers.add_parser(
         "targets",
```

### Comparing `tplink_omada_client-1.2.1/src/tplink_omada_client/cli/config.py` & `tplink_omada_client-1.2.2/src/tplink_omada_client/cli/config.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,64 +1,91 @@
-"""Responsible for ~/.omada.ini"""
+"""Responsible for ~/.omada.cfg"""
 from configparser import ConfigParser
 from dataclasses import dataclass
 from pathlib import Path
 
 from tplink_omada_client.omadaclient import OmadaClient
 
 _CONFIG_FILE: Path = Path.home() / '.omada.cfg'
 _CONTROLLER_SECTION_PREFIX: str = 'controller:'
+_CLI_SECTION: str = "cli"
+_DEFAULT_TARGET: str = "default_target"
 
 @dataclass
 class ControllerConfig:
     """Holds config needed to issue calls to Omada controller"""
     url: str
     username: str
     password: str
     site: str
 
-def get_targets() -> list[tuple[str, str]]:
+def get_targets() -> list[tuple[str, str, bool]]:
     """Get all the controllers in config file"""
     config_parser = _read_config_file()
+    default_target = config_parser[_CLI_SECTION][_DEFAULT_TARGET] if _CLI_SECTION in config_parser else ""
     targets = []
     for (target, config) in config_parser.items():
         if target.startswith(_CONTROLLER_SECTION_PREFIX):
             name = target[len(_CONTROLLER_SECTION_PREFIX):]
-            targets.append((name, config["url"]))
+            targets.append((name, config["url"], name == default_target))
     return targets
 
 def get_target_config(name: str) -> ControllerConfig:
     """Using controller name to create Omada site client"""
     config = _read_config_file()
+
+    if name == "":
+        if _CLI_SECTION in config:
+            name = config[_CLI_SECTION][_DEFAULT_TARGET]
+        if not name:
+            raise ValueError(f"No target specified, and no default target has been configured.")
+        
     stored_name = _to_stored_name(name)
     if config.has_section(stored_name):
         stored_config = config[stored_name]
         return ControllerConfig(**stored_config)
     raise ValueError(f"Could not find target named '{name}'")
 
-def set_target_config(name: str, config: ControllerConfig) -> None:
+def set_target_config(name: str, config: ControllerConfig, set_default: bool) -> None:
     """Stores controller config in users's config file"""
     stored_name = _to_stored_name(name)
     config_parser = _read_config_file()
     config_parser.remove_section(stored_name)
     config_parser.add_section(stored_name)
     config_parser.set(stored_name, "url", config.url)
     config_parser.set(stored_name, "username", config.username)
     config_parser.set(stored_name, "password", config.password)
     config_parser.set(stored_name, "site", config.site)
-    with _CONFIG_FILE.open(mode='w') as file:
-        config_parser.write(file)
+    if set_default:
+        if not config_parser[_CLI_SECTION]:
+            config_parser[_CLI_SECTION] = {}
+        config_parser[_CLI_SECTION][_DEFAULT_TARGET] = name
+
+    _write_config_file(config_parser)
+
+def set_default_target(name: str) -> None:
+    config_parser = _read_config_file()
+    if _CLI_SECTION not in config_parser:
+        config_parser[_CLI_SECTION] = {}
+    config_parser[_CLI_SECTION][_DEFAULT_TARGET] = name
+    _write_config_file(config_parser)
 
 def to_omada_connection(config: ControllerConfig) -> OmadaClient:
     """Create a OmadaClient based on a ControllerConfig object"""
     return OmadaClient(config.url, username=config.username, password=config.password)
 
 def _read_config_file() -> ConfigParser:
     """Read's the user's config file"""
     config = ConfigParser()
     if _CONFIG_FILE.exists():
         with _CONFIG_FILE.open() as file:
             config.read_file(file)
     return config
 
+def _write_config_file(config_parser):
+    """Write the user's config file"""
+    with _CONFIG_FILE.open(mode='w') as file:
+        config_parser.write(file)
+
+
 def _to_stored_name(name: str) -> str:
     return _CONTROLLER_SECTION_PREFIX + name
```

### Comparing `tplink_omada_client-1.2.1/LICENSE` & `tplink_omada_client-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.2.1/README.md` & `tplink_omada_client-1.2.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -25,35 +25,38 @@
 
 ## CLI
 
 This package provides a simple CLI for interacting with one or more Omada Controllers. To start using the
 CLI, you must first target a Controller.
 
 ```sh
-$ omada -t NAME target --url https://your.omada.controller.here --user admin --password password --site MySite
+$ omada -t NAME target --url https://your.omada.controller.here --user admin --password password --site MySite --set-default
 ```
 
 Where `NAME` is a name of your choosing to identify the targeted controller. `--site` defaults to the Omada
 default site name, 'Default'.  If you do not provide a password as an argument, you will be prompted for a
 password.
 
 Once you have successfully targeted a controller you can test that things are working by running:
 
 ```sh
-$ omada -t NAME devices
+$ omada devices
 ```
 
 This will list all the devices being managed by your controller.
 
 To see a list of all the available commands, run:
 
 ```sh
 $ omada -h
 ```
 
+You can set up multiple targets (controllers and sites), and specify the target with the `-t <NAME>` parameter.
+If you don't specify a target, the default will be used, if that has been set.
+
 The CLI is still young so if there is any functionality you need, please create an issue and let us know.
 
 ## Future
 
 The available API surface is quite large. More of this could be exposed in the future.
 There is an undocumented Websocket API which could potentially be used to get a stream of updates. However,
 I'm not sure how fully featured this subscription channel is on the controller. It seems to be rarely used,
```

### Comparing `tplink_omada_client-1.2.1/pyproject.toml` & `tplink_omada_client-1.2.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "tplink_omada_client"
-version = "1.2.1"
+version = "1.2.2"
 authors = [
   { name="Mark Godwin", email="author@example.com" },
 ]
 description = "Python wrapper for TP-Link Omada SDN Controller API (OC200/OC300/Software Controller)"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `tplink_omada_client-1.2.1/PKG-INFO` & `tplink_omada_client-1.2.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tplink_omada_client
-Version: 1.2.1
+Version: 1.2.2
 Summary: Python wrapper for TP-Link Omada SDN Controller API (OC200/OC300/Software Controller)
 Project-URL: Homepage, https://github.com/MarkGodwin/tplink-omada-api
 Project-URL: Bug Tracker, https://github.com/MarkGodwin/tplink-omada-api/issues
 Author-email: Mark Godwin <author@example.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -40,35 +40,38 @@
 
 ## CLI
 
 This package provides a simple CLI for interacting with one or more Omada Controllers. To start using the
 CLI, you must first target a Controller.
 
 ```sh
-$ omada -t NAME target --url https://your.omada.controller.here --user admin --password password --site MySite
+$ omada -t NAME target --url https://your.omada.controller.here --user admin --password password --site MySite --set-default
 ```
 
 Where `NAME` is a name of your choosing to identify the targeted controller. `--site` defaults to the Omada
 default site name, 'Default'.  If you do not provide a password as an argument, you will be prompted for a
 password.
 
 Once you have successfully targeted a controller you can test that things are working by running:
 
 ```sh
-$ omada -t NAME devices
+$ omada devices
 ```
 
 This will list all the devices being managed by your controller.
 
 To see a list of all the available commands, run:
 
 ```sh
 $ omada -h
 ```
 
+You can set up multiple targets (controllers and sites), and specify the target with the `-t <NAME>` parameter.
+If you don't specify a target, the default will be used, if that has been set.
+
 The CLI is still young so if there is any functionality you need, please create an issue and let us know.
 
 ## Future
 
 The available API surface is quite large. More of this could be exposed in the future.
 There is an undocumented Websocket API which could potentially be used to get a stream of updates. However,
 I'm not sure how fully featured this subscription channel is on the controller. It seems to be rarely used,
```

