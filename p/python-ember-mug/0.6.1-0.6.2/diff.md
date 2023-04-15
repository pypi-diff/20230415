# Comparing `tmp/python_ember_mug-0.6.1.tar.gz` & `tmp/python_ember_mug-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_ember_mug-0.6.1.tar", max compression
+gzip compressed data, was "python_ember_mug-0.6.2.tar", max compression
```

## Comparing `python_ember_mug-0.6.1.tar` & `python_ember_mug-0.6.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1069 2023-04-14 00:55:32.669181 python_ember_mug-0.6.1/LICENSE
--rw-r--r--   0        0        0     5219 2023-04-14 00:55:32.669181 python_ember_mug-0.6.1/README.md
--rwxr-xr-x   0        0        0      187 2023-04-14 00:55:32.669181 python_ember_mug-0.6.1/ember_mug/__init__.py
--rw-r--r--   0        0        0      106 2023-04-14 00:55:32.669181 python_ember_mug-0.6.1/ember_mug/__main__.py
--rw-r--r--   0        0        0      296 2023-04-14 00:55:32.669181 python_ember_mug-0.6.1/ember_mug/cli/__init__.py
--rw-r--r--   0        0        0     8471 2023-04-14 00:55:32.669181 python_ember_mug-0.6.1/ember_mug/cli/commands.py
--rw-r--r--   0        0        0     2910 2023-04-14 00:55:32.669181 python_ember_mug-0.6.1/ember_mug/cli/helpers.py
--rw-r--r--   0        0        0     4698 2023-04-14 00:55:32.669181 python_ember_mug-0.6.1/ember_mug/consts.py
--rw-r--r--   0        0        0     6264 2023-04-14 00:55:32.669181 python_ember_mug-0.6.1/ember_mug/data.py
--rw-r--r--   0        0        0      605 2023-04-14 00:55:32.669181 python_ember_mug-0.6.1/ember_mug/formatting.py
--rw-r--r--   0        0        0    17156 2023-04-14 00:55:32.669181 python_ember_mug-0.6.1/ember_mug/mug.py
--rw-r--r--   0        0        0     2112 2023-04-14 00:55:32.669181 python_ember_mug-0.6.1/ember_mug/scanner.py
--rw-r--r--   0        0        0     1963 2023-04-14 00:55:32.669181 python_ember_mug-0.6.1/ember_mug/utils.py
--rw-r--r--   0        0        0     2894 2023-04-14 00:55:32.673181 python_ember_mug-0.6.1/pyproject.toml
--rw-r--r--   0        0        0       46 2023-04-14 00:55:32.673181 python_ember_mug-0.6.1/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-04-14 00:55:32.673181 python_ember_mug-0.6.1/tests/cli/__init__.py
--rw-r--r--   0        0        0     7832 2023-04-14 00:55:32.673181 python_ember_mug-0.6.1/tests/cli/test_commands.py
--rw-r--r--   0        0        0     2645 2023-04-14 00:55:32.673181 python_ember_mug-0.6.1/tests/cli/test_helpers.py
--rw-r--r--   0        0        0     1156 2023-04-14 00:55:32.673181 python_ember_mug-0.6.1/tests/conftest.py
--rw-r--r--   0        0        0    19148 2023-04-14 00:55:32.673181 python_ember_mug-0.6.1/tests/test_connection.py
--rw-r--r--   0        0        0      776 2023-04-14 00:55:32.673181 python_ember_mug-0.6.1/tests/test_consts.py
--rw-r--r--   0        0        0     1299 2023-04-14 00:55:32.673181 python_ember_mug-0.6.1/tests/test_data.py
--rw-r--r--   0        0        0      534 2023-04-14 00:55:32.673181 python_ember_mug-0.6.1/tests/test_formatting.py
--rw-r--r--   0        0        0     3294 2023-04-14 00:55:32.673181 python_ember_mug-0.6.1/tests/test_mug_data.py
--rw-r--r--   0        0        0     2012 2023-04-14 00:55:32.673181 python_ember_mug-0.6.1/tests/test_scanner.py
--rw-r--r--   0        0        0      801 2023-04-14 00:55:32.673181 python_ember_mug-0.6.1/tests/test_utils.py
--rw-r--r--   0        0        0     6425 1970-01-01 00:00:00.000000 python_ember_mug-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-15 03:17:36.080041 python_ember_mug-0.6.2/LICENSE
+-rw-r--r--   0        0        0     5219 2023-04-15 03:17:36.080041 python_ember_mug-0.6.2/README.md
+-rwxr-xr-x   0        0        0      187 2023-04-15 03:17:36.080041 python_ember_mug-0.6.2/ember_mug/__init__.py
+-rw-r--r--   0        0        0      106 2023-04-15 03:17:36.080041 python_ember_mug-0.6.2/ember_mug/__main__.py
+-rw-r--r--   0        0        0      296 2023-04-15 03:17:36.080041 python_ember_mug-0.6.2/ember_mug/cli/__init__.py
+-rw-r--r--   0        0        0     8471 2023-04-15 03:17:36.080041 python_ember_mug-0.6.2/ember_mug/cli/commands.py
+-rw-r--r--   0        0        0     2910 2023-04-15 03:17:36.080041 python_ember_mug-0.6.2/ember_mug/cli/helpers.py
+-rw-r--r--   0        0        0     4820 2023-04-15 03:17:36.084041 python_ember_mug-0.6.2/ember_mug/consts.py
+-rw-r--r--   0        0        0     7729 2023-04-15 03:17:36.084041 python_ember_mug-0.6.2/ember_mug/data.py
+-rw-r--r--   0        0        0      605 2023-04-15 03:17:36.084041 python_ember_mug-0.6.2/ember_mug/formatting.py
+-rw-r--r--   0        0        0    16978 2023-04-15 03:17:36.084041 python_ember_mug-0.6.2/ember_mug/mug.py
+-rw-r--r--   0        0        0     2112 2023-04-15 03:17:36.084041 python_ember_mug-0.6.2/ember_mug/scanner.py
+-rw-r--r--   0        0        0     1963 2023-04-15 03:17:36.084041 python_ember_mug-0.6.2/ember_mug/utils.py
+-rw-r--r--   0        0        0     2894 2023-04-15 03:17:36.084041 python_ember_mug-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0       46 2023-04-15 03:17:36.084041 python_ember_mug-0.6.2/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-15 03:17:36.084041 python_ember_mug-0.6.2/tests/cli/__init__.py
+-rw-r--r--   0        0        0     7846 2023-04-15 03:17:36.084041 python_ember_mug-0.6.2/tests/cli/test_commands.py
+-rw-r--r--   0        0        0     2663 2023-04-15 03:17:36.084041 python_ember_mug-0.6.2/tests/cli/test_helpers.py
+-rw-r--r--   0        0        0     1199 2023-04-15 03:17:36.084041 python_ember_mug-0.6.2/tests/conftest.py
+-rw-r--r--   0        0        0    19254 2023-04-15 03:17:36.084041 python_ember_mug-0.6.2/tests/test_connection.py
+-rw-r--r--   0        0        0      776 2023-04-15 03:17:36.084041 python_ember_mug-0.6.2/tests/test_consts.py
+-rw-r--r--   0        0        0     2343 2023-04-15 03:17:36.084041 python_ember_mug-0.6.2/tests/test_data.py
+-rw-r--r--   0        0        0      534 2023-04-15 03:17:36.084041 python_ember_mug-0.6.2/tests/test_formatting.py
+-rw-r--r--   0        0        0     3338 2023-04-15 03:17:36.084041 python_ember_mug-0.6.2/tests/test_mug_data.py
+-rw-r--r--   0        0        0     2012 2023-04-15 03:17:36.084041 python_ember_mug-0.6.2/tests/test_scanner.py
+-rw-r--r--   0        0        0      801 2023-04-15 03:17:36.084041 python_ember_mug-0.6.2/tests/test_utils.py
+-rw-r--r--   0        0        0     6425 1970-01-01 00:00:00.000000 python_ember_mug-0.6.2/PKG-INFO
```

### Comparing `python_ember_mug-0.6.1/LICENSE` & `python_ember_mug-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.6.1/README.md` & `python_ember_mug-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.6.1/ember_mug/cli/commands.py` & `python_ember_mug-0.6.2/ember_mug/cli/commands.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.6.1/ember_mug/cli/helpers.py` & `python_ember_mug-0.6.2/ember_mug/cli/helpers.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.6.1/ember_mug/consts.py` & `python_ember_mug-0.6.2/ember_mug/consts.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,20 +4,25 @@
 import platform
 import re
 from enum import Enum, IntEnum
 from functools import cached_property
 from typing import Literal
 from uuid import UUID
 
-# Bluetooth names of supported mugs
+# Bluetooth names of Ember devices
+EMBER_MUG = "Ember Ceramic Mug"
+EMBER_CUP = "Ember Cup"
+EMBER_CUP_2 = "Ember Cup 2"
+EMBER_TRAVEL_MUG = "Ember Travel Mug"
+
 EMBER_BLUETOOTH_NAMES: tuple[str, ...] = (
-    "Ember Ceramic Mug",
-    "Ember Travel Mug",
-    "Ember Cup",
-    "Ember Cup 2",
+    EMBER_MUG,
+    EMBER_CUP,
+    EMBER_CUP_2,
+    EMBER_TRAVEL_MUG,
 )
 
 # Format for all the mug's Bluetooth UUIDs
 UUID_TEMPLATE = "fc54{:0>4x}-236c-4c94-8fa9-944a3e5353fa"
 
 
 class TemperatureUnit(str, Enum):
@@ -169,16 +174,16 @@
     "led_colour",
     "current_temp",
     "target_temp",
     "temperature_unit",
     "battery",
     "liquid_level",
     "liquid_state",
-    "battery_voltage",
 }
+TRAVEL_MUG_ATTRS = {"battery_voltage"}
 EXTRA_ATTRS = {'dsk', 'udsk', 'battery_voltage', 'date_time_zone'}
 
 # Validation
 MUG_NAME_REGEX = re.compile(r"^[A-Za-z0-9,.\[\]#()!\"\';:|\-_+<>%= ]{1,16}$")
 MAC_ADDRESS_REGEX = re.compile(r"^([0-9A-Fa-f]{2}:){5}([0-9A-Fa-f]{2})$")
 
 IS_LINUX = platform.system() == "Linux"
```

### Comparing `python_ember_mug-0.6.1/ember_mug/data.py` & `python_ember_mug-0.6.2/ember_mug/data.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,25 @@
 """Classes for representing data from the mug."""
 from __future__ import annotations
 
 from dataclasses import asdict, dataclass, is_dataclass
+from functools import cached_property
 from typing import Any, NamedTuple
 
-from .consts import ATTR_LABELS, EXTRA_ATTRS, LiquidState, TemperatureUnit
+from .consts import (
+    ATTR_LABELS,
+    EMBER_CUP,
+    EMBER_TRAVEL_MUG,
+    EXTRA_ATTRS,
+    INITIAL_ATTRS,
+    TRAVEL_MUG_ATTRS,
+    UPDATE_ATTRS,
+    LiquidState,
+    TemperatureUnit,
+)
 from .formatting import format_led_colour, format_liquid_level, format_temp
 from .utils import bytes_to_little_int, decode_byte_string
 
 
 class Change(NamedTuple):
     """Helper for storing changes to attributes."""
 
@@ -92,14 +103,57 @@
                 f'Hardware: {self.hardware}',
                 f'Bootloader: {self.bootloader}',
             ),
         )
 
 
 @dataclass
+class Model:
+    """Model name and attributes based on mode."""
+
+    name: str
+    include_extra: bool = False
+
+    @cached_property
+    def is_cup(self) -> bool:
+        """Check if the model is a Cup."""
+        return self.name.startswith(EMBER_CUP)
+
+    @cached_property
+    def is_travel_mug(self) -> bool:
+        """Check if the model is a Travel mug."""
+        return self.name.startswith(EMBER_TRAVEL_MUG)
+
+    @cached_property
+    def attribute_labels(self) -> dict[str, str]:
+        """Calculated labels for includes attributes."""
+        all_attrs = self.initial_attributes | self.update_attributes | {'use_metric'}
+        return {attr: label for attr, label in ATTR_LABELS.items() if attr in all_attrs}
+
+    @cached_property
+    def initial_attributes(self) -> set[str]:
+        """Initial attributes based on model and extra."""
+        if self.include_extra is False:
+            return INITIAL_ATTRS - EXTRA_ATTRS
+        return INITIAL_ATTRS
+
+    @cached_property
+    def update_attributes(self) -> set[str]:
+        """Attributes to update based on model and extra."""
+        attributes = UPDATE_ATTRS
+        if self.include_extra is False:
+            attributes = attributes - EXTRA_ATTRS
+        if self.is_cup:
+            attributes = attributes - {'name'}
+        elif self.is_travel_mug:
+            attributes = attributes | TRAVEL_MUG_ATTRS
+        return attributes
+
+
+@dataclass
 class MugMeta:
     """Meta data for mug."""
 
     mug_id: str
     serial_number: str
 
     @classmethod
@@ -116,17 +170,16 @@
 
 
 @dataclass
 class MugData:
     """Class to store/display the state of the mug."""
 
     # Options
-    model: str
+    model: Model
     use_metric: bool = True
-    include_extra: bool = False
 
     # Attributes
     name: str = ""
     meta: MugMeta | None = None
     battery: BatteryInfo | None = None
     firmware: MugFirmwareInfo | None = None
     led_colour: Colour = Colour(255, 255, 255)
@@ -139,15 +192,15 @@
     udsk: str = ""
     date_time_zone: str = ""
     battery_voltage: str = ""
 
     @property
     def meta_display(self) -> str:
         """Return Meta infor based on preference."""
-        if self.meta and not self.include_extra:
+        if self.meta and not self.model.include_extra:
             return f'Serial Number: {self.meta.serial_number}'
         return str(self.meta)
 
     @property
     def led_colour_display(self) -> str:
         """Return colour as hex value."""
         return format_led_colour(self.led_colour)
@@ -186,19 +239,15 @@
         if display_value := getattr(self, f'{attr}_display', None):
             return display_value
         return getattr(self, attr)
 
     @property
     def formatted(self) -> dict[str, Any]:
         """Return human-readable names and values for all attributes for display."""
-        return {
-            label: self.get_formatted_attr(attr)
-            for attr, label in ATTR_LABELS.items()
-            if self.include_extra or attr not in EXTRA_ATTRS
-        }
+        return {label: self.get_formatted_attr(attr) for attr, label in self.model.attribute_labels.items()}
 
     def as_dict(self) -> dict[str, Any]:
         """Dump all attributes as dict for info/debugging."""
         data = {k: asdict(v) if is_dataclass(v) else v for k, v in asdict(self).items()}
         data.update(
             {
                 f'{attr}_display': getattr(self, f'{attr}_display')
```

### Comparing `python_ember_mug-0.6.1/ember_mug/formatting.py` & `python_ember_mug-0.6.2/ember_mug/formatting.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.6.1/ember_mug/mug.py` & `python_ember_mug-0.6.2/ember_mug/mug.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,26 +12,23 @@
 
 from bleak import BleakClient, BleakError
 from bleak.backends.characteristic import BleakGATTCharacteristic
 from bleak.backends.device import BLEDevice
 from bleak_retry_connector import establish_connection
 
 from .consts import (
-    EXTRA_ATTRS,
-    INITIAL_ATTRS,
     IS_LINUX,
     MUG_NAME_REGEX,
     PUSH_EVENT_BATTERY_IDS,
-    UPDATE_ATTRS,
     LiquidState,
     MugCharacteristic,
     PushEvent,
     TemperatureUnit,
 )
-from .data import BatteryInfo, Change, Colour, MugData, MugFirmwareInfo, MugMeta
+from .data import BatteryInfo, Change, Colour, Model, MugData, MugFirmwareInfo, MugMeta
 from .utils import (
     bytes_to_big_int,
     bytes_to_little_int,
     decode_byte_string,
     encode_byte_string,
     log_services,
     temp_from_bytes,
@@ -51,27 +48,28 @@
         include_extra: bool = False,
         use_metric: bool = True,
         debug: bool = False,
         **kwargs: Any,
     ) -> None:
         """Initialize connection manager."""
         self.device = ble_device
-        self.data = MugData(ble_device.name or 'EMBER', include_extra=include_extra, use_metric=use_metric)
+        self.data = MugData(
+            Model(ble_device.name or 'EMBER', include_extra),
+            use_metric=use_metric,
+        )
 
         self.debug = debug
         self._connect_lock = asyncio.Lock()
         self._operation_lock = asyncio.Lock()
         self._expected_disconnect = False
         self._callbacks: dict[Callable[[MugData], None], Callable[[], None]] = {}
         self._client: BleakClient = None  # type: ignore[assignment]
         self._queued_updates: set[str] = set()
         self._latest_events: dict[int, float] = {}
         self._client_kwargs: dict[str, str] = {}
-        self._initial_attrs = INITIAL_ATTRS if include_extra else (INITIAL_ATTRS - EXTRA_ATTRS)
-        self._update_attrs = UPDATE_ATTRS if include_extra else (UPDATE_ATTRS - EXTRA_ATTRS)
 
         logger.debug("New mug connection initialized.")
         self.set_client_options(**kwargs)
 
     def set_device(self, ble_device: BLEDevice) -> None:
         """Set the ble device."""
         logger.debug("Set new device from %s to %s", self.device, ble_device)
@@ -292,19 +290,19 @@
 
     async def get_firmware(self) -> MugFirmwareInfo:
         """Get firmware info."""
         return MugFirmwareInfo.from_bytes(await self._read(MugCharacteristic.FIRMWARE))
 
     async def update_initial(self) -> list[Change]:
         """Update attributes that don't normally change and don't need to be regularly updated."""
-        return await self._update_multiple(self._initial_attrs)
+        return await self._update_multiple(self.data.model.initial_attributes)
 
     async def update_all(self) -> list[Change]:
         """Update all standard attributes."""
-        return await self._update_multiple(self._update_attrs)
+        return await self._update_multiple(self.data.model.update_attributes)
 
     async def _update_multiple(self, attrs: set[str]) -> list[Change]:
         """Helper to update a list of attributes from the mug."""
         logger.debug('Updating the following attributes: %s', attrs)
         await self._ensure_connection()
         changes = self.data.update_info(**{attr: await getattr(self, f"get_{attr}")() for attr in attrs})
         if changes:
```

### Comparing `python_ember_mug-0.6.1/ember_mug/scanner.py` & `python_ember_mug-0.6.2/ember_mug/scanner.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.6.1/ember_mug/utils.py` & `python_ember_mug-0.6.2/ember_mug/utils.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.6.1/pyproject.toml` & `python_ember_mug-0.6.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "python-ember-mug"
-version = "0.6.1"
+version = "0.6.2"
 homepage = "https://github.com/sopelj/python-ember-mug"
 description = "Python Library for Ember Mugs."
 authors = ["Jesse Sopel <jesse.sopel@gmail.com>"]
 readme = "README.md"
 license =  "MIT"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
```

### Comparing `python_ember_mug-0.6.1/tests/cli/test_commands.py` & `python_ember_mug-0.6.2/tests/cli/test_commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 import pytest
 from bleak import BleakError, BLEDevice
 from pytest import CaptureFixture
 
 from ember_mug import EmberMug
 from ember_mug.cli.commands import EmberMugCli, discover, fetch_info, find_device, get_mug, get_mug_value
-from ember_mug.data import MugData
+from ember_mug.data import Model, MugData
 from tests.conftest import TEST_MAC
 
 from ..conftest import mock_connection
 
 
 @pytest.fixture()
 def mock_mug_with_connection() -> Generator[AsyncMock, None, None]:
@@ -165,15 +165,15 @@
 
 @patch('ember_mug.cli.commands.print_table')
 async def test_get_mug_value(
     mocked_print_table: Mock,
     mock_mug_with_connection: AsyncMock,
     capsys: CaptureFixture,
 ) -> None:
-    mock_mug_with_connection.data = MugData('test')
+    mock_mug_with_connection.data = MugData(Model('Test'))
     mock_mug_with_connection.data.get_formatted_attr = Mock(return_value='test')  # type: ignore[assignment]
     mock_mug_with_connection.get_target_temp.return_value = 55.5
     mock_mug_with_connection.get_name.return_value = 'test'
     args = mock_namespace(attributes=['target_temp', 'name'])
     await get_mug_value(args)
     mock_mug_with_connection.get_target_temp.assert_called_once()
     mocked_print_table.assert_called_once_with([('Target Temp', "test"), ('Mug Name', "test")])
```

### Comparing `python_ember_mug-0.6.1/tests/cli/test_helpers.py` & `python_ember_mug-0.6.2/tests/cli/test_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 from textwrap import dedent
 
 import pytest
 from pytest import CaptureFixture
 
 from ember_mug import EmberMug
 from ember_mug.cli.helpers import build_sub_rows, print_changes, print_info, print_table, validate_mac
-from ember_mug.consts import LiquidState
-from ember_mug.data import Change
+from ember_mug.consts import EMBER_MUG, LiquidState
+from ember_mug.data import Change, Model
 
 
 def test_validate_mac() -> None:
     with pytest.raises(ArgumentTypeError):
         validate_mac('potato')
     assert validate_mac('9C:DA:8C:19:27:DA') == '9c:da:8c:19:27:da'
```

### Comparing `python_ember_mug-0.6.1/tests/conftest.py` & `python_ember_mug-0.6.2/tests/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,18 +4,19 @@
 from unittest.mock import AsyncMock, MagicMock
 
 import pytest
 import pytest_asyncio
 from bleak.backends.device import BLEDevice
 
 from ember_mug import EmberMug
-from ember_mug.data import MugData
+from ember_mug.consts import EMBER_MUG
+from ember_mug.data import Model, MugData
 
 TEST_MAC = '32:36:a5:be:88:cb'
-TEST_MODEL_NAME = 'Ember Ceramic Mug'
+TEST_MODEL_NAME = EMBER_MUG
 
 
 class AsyncContextManager:
     """Stub for mocking."""
 
     async def __aenter__(self):
         """Return self."""
@@ -32,15 +33,15 @@
 @pytest.fixture(name='ble_device')
 def ble_device_fixture() -> Generator[BLEDevice, None, None]:
     yield BLEDevice(address=TEST_MAC, name=TEST_MODEL_NAME, details={}, rssi=1)
 
 
 @pytest.fixture
 def mug_data(ble_device: BLEDevice) -> Generator[MugData, None, None]:
-    yield MugData(ble_device.name or TEST_MODEL_NAME)
+    yield MugData(Model(ble_device.name or TEST_MODEL_NAME))
 
 
 @pytest_asyncio.fixture
 async def ember_mug(ble_device: BLEDevice) -> AsyncGenerator[EmberMug | AsyncMock, None]:
     mug = EmberMug(ble_device)
     mug._client = AsyncMock()
     yield mug
```

### Comparing `python_ember_mug-0.6.1/tests/test_connection.py` & `python_ember_mug-0.6.2/tests/test_connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 
 from unittest.mock import AsyncMock, Mock, patch
 
 import pytest
 from bleak import BleakError
 from bleak.backends.device import BLEDevice
 
-from ember_mug.consts import MugCharacteristic, TemperatureUnit
-from ember_mug.data import Colour
-from ember_mug.mug import EXTRA_ATTRS, INITIAL_ATTRS, UPDATE_ATTRS, EmberMug
+from ember_mug.consts import EMBER_MUG, EXTRA_ATTRS, INITIAL_ATTRS, UPDATE_ATTRS, MugCharacteristic, TemperatureUnit
+from ember_mug.data import Colour, Model
+from ember_mug.mug import EmberMug
 
 
 @patch('ember_mug.mug.IS_LINUX', True)
 async def test_adapter_with_bluez(ble_device: BLEDevice):
     mug = EmberMug(ble_device, adapter='hci0')
     assert mug._client_kwargs['adapter'] == 'hci0'
 
@@ -384,21 +384,22 @@
 
 
 async def test_mug_update_initial(ember_mug):
     no_extra = INITIAL_ATTRS - EXTRA_ATTRS
 
     with patch.object(ember_mug, '_ensure_connection', AsyncMock()):
         ember_mug._update_multiple = AsyncMock(return_value={})
+        ember_mug.data.model = Model(EMBER_MUG, include_extra=False)
         assert (await ember_mug.update_initial()) == {}
         ember_mug._update_multiple.assert_called_once_with(no_extra)
 
     # Try with extra
     with patch.object(ember_mug, '_ensure_connection', AsyncMock()):
         ember_mug._update_multiple.reset_mock()
-        ember_mug._initial_attrs = INITIAL_ATTRS
+        ember_mug.data.model = Model(EMBER_MUG, include_extra=True)
         assert (await ember_mug.update_initial()) == {}
         ember_mug._update_multiple.assert_called_once_with(INITIAL_ATTRS)
 
 
 async def test_mug_update_all(ember_mug):
     with patch.object(ember_mug, '_ensure_connection', AsyncMock()):
         ember_mug._update_multiple = AsyncMock(return_value={})
```

### Comparing `python_ember_mug-0.6.1/tests/test_consts.py` & `python_ember_mug-0.6.2/tests/test_consts.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.6.1/tests/test_formatting.py` & `python_ember_mug-0.6.2/tests/test_formatting.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.6.1/tests/test_mug_data.py` & `python_ember_mug-0.6.2/tests/test_mug_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Tests for `ember_mug.mug`."""
 from __future__ import annotations
 
 from typing import Any
 
-from ember_mug.consts import LiquidState, TemperatureUnit
-from ember_mug.data import BatteryInfo, Change, Colour, MugData, MugFirmwareInfo, MugMeta
+from ember_mug.consts import EMBER_MUG, LiquidState, TemperatureUnit
+from ember_mug.data import BatteryInfo, Change, Colour, Model, MugData, MugFirmwareInfo, MugMeta
 
 
 def test_mug_formatting(mug_data: MugData) -> None:
     meta = MugMeta('A', 'ABCDEF')
     battery = BatteryInfo(35.46, False)
     firmware = MugFirmwareInfo(12, 35, 55)
     colour = Colour(244, 0, 161)
@@ -24,15 +24,15 @@
         target_temp=55,
         dsk='dsk',
         udsk='udsk',
         date_time_zone=None,
         battery_voltage=0.1,
     )
     assert mug_data.meta_display == "Serial Number: ABCDEF"
-    mug_data.include_extra = True
+    mug_data.model = Model(EMBER_MUG, include_extra=True)
     assert mug_data.meta_display == "Mug ID: A, Serial Number: ABCDEF"
     assert mug_data.led_colour_display == "#f400a1"
     assert mug_data.liquid_state_display == "Heating"
     assert mug_data.liquid_level_display == "16.67%"
     assert mug_data.current_temp_display == "25.00°C"
     assert mug_data.target_temp_display == "55.00°C"
     basic_info: dict[str, Any] = {
@@ -49,17 +49,16 @@
     }
     assert mug_data.formatted == {
         **basic_info,
         'Meta': "Mug ID: A, Serial Number: ABCDEF",
         'DSK': "dsk",
         'UDSK': "udsk",
         'Date Time + Time Zone': None,
-        'Voltage': 0.1,
     }
-    mug_data.include_extra = False
+    mug_data.model = Model(EMBER_MUG, include_extra=False)
     assert mug_data.formatted == basic_info
 
 
 def test_update_info(mug_data: MugData) -> None:
     mug_data.current_temp = 55
     mug_data.target_temp = 55
     mug_data.led_colour = Colour(255, 0, 0)
@@ -73,16 +72,15 @@
         Change('led_colour', Colour(255, 0, 0), Colour(0, 255, 0)),
     ]
 
 
 def test_mug_dict(mug_data: MugData) -> None:
     mug_data.update_info(meta=MugMeta('test_id', 'serial number'))
     assert mug_data.as_dict() == {
-        'model': 'Ember Ceramic Mug',
-        'include_extra': False,
+        'model': {'include_extra': False, 'name': 'Ember Ceramic Mug'},
         'use_metric': True,
         'battery': None,
         'battery_voltage': '',
         'current_temp': 0.0,
         'current_temp_display': '0.00°C',
         'date_time_zone': '',
         'dsk': '',
```

### Comparing `python_ember_mug-0.6.1/tests/test_scanner.py` & `python_ember_mug-0.6.2/tests/test_scanner.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.6.1/tests/test_utils.py` & `python_ember_mug-0.6.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `python_ember_mug-0.6.1/PKG-INFO` & `python_ember_mug-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-ember-mug
-Version: 0.6.1
+Version: 0.6.2
 Summary: Python Library for Ember Mugs.
 Home-page: https://github.com/sopelj/python-ember-mug
 License: MIT
 Author: Jesse Sopel
 Author-email: jesse.sopel@gmail.com
 Requires-Python: >=3.9,<3.12
 Classifier: Development Status :: 2 - Pre-Alpha
```

