# Comparing `tmp/pysolarfocus-3.6.3.tar.gz` & `tmp/pysolarfocus-3.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysolarfocus-3.6.3.tar", max compression
+gzip compressed data, was "pysolarfocus-3.6.4.tar", max compression
```

## Comparing `pysolarfocus-3.6.3.tar` & `pysolarfocus-3.6.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    11357 2023-04-14 14:53:14.745483 pysolarfocus-3.6.3/LICENSE
--rw-r--r--   0        0        0     3183 2023-04-14 14:53:14.745483 pysolarfocus-3.6.3/README.md
--rw-r--r--   0        0        0      580 2023-04-14 14:53:14.745483 pysolarfocus-3.6.3/pyproject.toml
--rw-r--r--   0        0        0     5469 2023-04-14 14:53:14.745483 pysolarfocus-3.6.3/pysolarfocus/__init__.py
--rw-r--r--   0        0        0     3495 2023-04-14 14:53:14.745483 pysolarfocus-3.6.3/pysolarfocus/component_factory.py
--rw-r--r--   0        0        0        0 2023-04-14 14:53:14.745483 pysolarfocus-3.6.3/pysolarfocus/components/__init__.py
--rw-r--r--   0        0        0        0 2023-04-14 14:53:14.745483 pysolarfocus-3.6.3/pysolarfocus/components/base/__init__.py
--rw-r--r--   0        0        0     9390 2023-04-14 14:53:14.745483 pysolarfocus-3.6.3/pysolarfocus/components/base/component.py
--rw-r--r--   0        0        0     2840 2023-04-14 14:53:14.745483 pysolarfocus-3.6.3/pysolarfocus/components/base/data_value.py
--rw-r--r--   0        0        0      159 2023-04-14 14:53:14.745483 pysolarfocus-3.6.3/pysolarfocus/components/base/enums.py
--rw-r--r--   0        0        0      205 2023-04-14 14:53:14.745483 pysolarfocus-3.6.3/pysolarfocus/components/base/part.py
--rw-r--r--   0        0        0      784 2023-04-14 14:53:14.745483 pysolarfocus-3.6.3/pysolarfocus/components/base/performance_calculator.py
--rw-r--r--   0        0        0      133 2023-04-14 14:53:14.745483 pysolarfocus-3.6.3/pysolarfocus/components/base/register_slice.py
--rw-r--r--   0        0        0      872 2023-04-14 14:53:14.745483 pysolarfocus-3.6.3/pysolarfocus/components/boiler.py
--rw-r--r--   0        0        0     1474 2023-04-14 14:53:14.745483 pysolarfocus-3.6.3/pysolarfocus/components/buffer.py
--rw-r--r--   0        0        0      292 2023-04-14 14:53:14.745483 pysolarfocus-3.6.3/pysolarfocus/components/fresh_water_module.py
--rw-r--r--   0        0        0     2650 2023-04-14 14:53:14.745483 pysolarfocus-3.6.3/pysolarfocus/components/heat_pump.py
--rw-r--r--   0        0        0     1827 2023-04-14 14:53:14.745483 pysolarfocus-3.6.3/pysolarfocus/components/heating_circuit.py
--rw-r--r--   0        0        0     1877 2023-04-14 14:53:14.745483 pysolarfocus-3.6.3/pysolarfocus/components/pellets_boiler.py
--rw-r--r--   0        0        0      800 2023-04-14 14:53:14.745483 pysolarfocus-3.6.3/pysolarfocus/components/photovoltaic.py
--rw-r--r--   0        0        0     1054 2023-04-14 14:53:14.745483 pysolarfocus-3.6.3/pysolarfocus/components/solar.py
--rw-r--r--   0        0        0     2965 2023-04-14 14:53:14.745483 pysolarfocus-3.6.3/pysolarfocus/const.py
--rw-r--r--   0        0        0     4027 2023-04-14 14:53:14.745483 pysolarfocus-3.6.3/pysolarfocus/modbus_wrapper.py
--rw-r--r--   0        0        0     3881 1970-01-01 00:00:00.000000 pysolarfocus-3.6.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-15 17:26:38.619168 pysolarfocus-3.6.4/LICENSE
+-rw-r--r--   0        0        0     4514 2023-04-15 17:26:38.619168 pysolarfocus-3.6.4/README.md
+-rw-r--r--   0        0        0      580 2023-04-15 17:26:38.623168 pysolarfocus-3.6.4/pyproject.toml
+-rw-r--r--   0        0        0     5469 2023-04-15 17:26:38.623168 pysolarfocus-3.6.4/pysolarfocus/__init__.py
+-rw-r--r--   0        0        0     3495 2023-04-15 17:26:38.623168 pysolarfocus-3.6.4/pysolarfocus/component_factory.py
+-rw-r--r--   0        0        0        0 2023-04-15 17:26:38.623168 pysolarfocus-3.6.4/pysolarfocus/components/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-15 17:26:38.623168 pysolarfocus-3.6.4/pysolarfocus/components/base/__init__.py
+-rw-r--r--   0        0        0     9390 2023-04-15 17:26:38.623168 pysolarfocus-3.6.4/pysolarfocus/components/base/component.py
+-rw-r--r--   0        0        0     2840 2023-04-15 17:26:38.623168 pysolarfocus-3.6.4/pysolarfocus/components/base/data_value.py
+-rw-r--r--   0        0        0      159 2023-04-15 17:26:38.623168 pysolarfocus-3.6.4/pysolarfocus/components/base/enums.py
+-rw-r--r--   0        0        0      205 2023-04-15 17:26:38.623168 pysolarfocus-3.6.4/pysolarfocus/components/base/part.py
+-rw-r--r--   0        0        0      784 2023-04-15 17:26:38.623168 pysolarfocus-3.6.4/pysolarfocus/components/base/performance_calculator.py
+-rw-r--r--   0        0        0      133 2023-04-15 17:26:38.623168 pysolarfocus-3.6.4/pysolarfocus/components/base/register_slice.py
+-rw-r--r--   0        0        0      872 2023-04-15 17:26:38.623168 pysolarfocus-3.6.4/pysolarfocus/components/boiler.py
+-rw-r--r--   0        0        0     1480 2023-04-15 17:26:38.623168 pysolarfocus-3.6.4/pysolarfocus/components/buffer.py
+-rw-r--r--   0        0        0      292 2023-04-15 17:26:38.623168 pysolarfocus-3.6.4/pysolarfocus/components/fresh_water_module.py
+-rw-r--r--   0        0        0     2650 2023-04-15 17:26:38.623168 pysolarfocus-3.6.4/pysolarfocus/components/heat_pump.py
+-rw-r--r--   0        0        0     1827 2023-04-15 17:26:38.623168 pysolarfocus-3.6.4/pysolarfocus/components/heating_circuit.py
+-rw-r--r--   0        0        0     1877 2023-04-15 17:26:38.623168 pysolarfocus-3.6.4/pysolarfocus/components/pellets_boiler.py
+-rw-r--r--   0        0        0      800 2023-04-15 17:26:38.623168 pysolarfocus-3.6.4/pysolarfocus/components/photovoltaic.py
+-rw-r--r--   0        0        0     1054 2023-04-15 17:26:38.623168 pysolarfocus-3.6.4/pysolarfocus/components/solar.py
+-rw-r--r--   0        0        0     2965 2023-04-15 17:26:38.623168 pysolarfocus-3.6.4/pysolarfocus/const.py
+-rw-r--r--   0        0        0     4027 2023-04-15 17:26:38.623168 pysolarfocus-3.6.4/pysolarfocus/modbus_wrapper.py
+-rw-r--r--   0        0        0     5212 1970-01-01 00:00:00.000000 pysolarfocus-3.6.4/PKG-INFO
```

### Comparing `pysolarfocus-3.6.3/LICENSE` & `pysolarfocus-3.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pysolarfocus-3.6.3/pyproject.toml` & `pysolarfocus-3.6.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pysolarfocus"
-version = "3.6.3"
+version = "3.6.4"
 description = "Unofficial, local Solarfocus client"
 authors = ["Jeroen Laverman <jjlaverman@web.de>"]
 license = "Apache-2.0"
 homepage = "https://github.com/lavermanjj/pysolarfocus"
 repository = "https://github.com/lavermanjj/pysolarfocus"
 keywords = ["solarfocus", "api client"]
 include = ["LICENSE"]
```

### Comparing `pysolarfocus-3.6.3/pysolarfocus/__init__.py` & `pysolarfocus-3.6.4/pysolarfocus/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Python client lib for Solarfocus"""
-__version__ = "3.6.3"
+__version__ = "3.6.4"
 
 from enum import Enum
 from packaging import version
 
 #Default port for modbus
 PORT = 502
```

### Comparing `pysolarfocus-3.6.3/pysolarfocus/component_factory.py` & `pysolarfocus-3.6.4/pysolarfocus/component_factory.py`

 * *Files identical despite different names*

### Comparing `pysolarfocus-3.6.3/pysolarfocus/components/base/component.py` & `pysolarfocus-3.6.4/pysolarfocus/components/base/component.py`

 * *Files identical despite different names*

### Comparing `pysolarfocus-3.6.3/pysolarfocus/components/base/data_value.py` & `pysolarfocus-3.6.4/pysolarfocus/components/base/data_value.py`

 * *Files identical despite different names*

### Comparing `pysolarfocus-3.6.3/pysolarfocus/components/base/performance_calculator.py` & `pysolarfocus-3.6.4/pysolarfocus/components/base/performance_calculator.py`

 * *Files identical despite different names*

### Comparing `pysolarfocus-3.6.3/pysolarfocus/components/boiler.py` & `pysolarfocus-3.6.4/pysolarfocus/components/boiler.py`

 * *Files identical despite different names*

### Comparing `pysolarfocus-3.6.3/pysolarfocus/components/buffer.py` & `pysolarfocus-3.6.4/pysolarfocus/components/buffer.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,13 +18,13 @@
             self.external_top_temperature_x44 = DataValue(address=0,multiplier=10,register_type=RegisterTypes.Holding)
             self.external_middle_temperature_x36 = DataValue(address=1,multiplier=10,register_type=RegisterTypes.Holding)
             self.external_bottom_temperature_x35 = DataValue(address=2,multiplier=10,register_type=RegisterTypes.Holding)
         
         
 class TherminatorBuffer(Buffer):
     def __init__(self,address:int=1900) -> None:
-        super().__init__(address=address)
+        super().__init__(input_address=address)
         self.x35_temperature = DataValue(address=2,multiplier=0.1)
         self.pump = DataValue(address=3)
         self.state = DataValue(address=4,type=DataTypes.UINT)
         self.mode = DataValue(address=5,type=DataTypes.UINT)
```

### Comparing `pysolarfocus-3.6.3/pysolarfocus/components/heat_pump.py` & `pysolarfocus-3.6.4/pysolarfocus/components/heat_pump.py`

 * *Files identical despite different names*

### Comparing `pysolarfocus-3.6.3/pysolarfocus/components/heating_circuit.py` & `pysolarfocus-3.6.4/pysolarfocus/components/heating_circuit.py`

 * *Files identical despite different names*

### Comparing `pysolarfocus-3.6.3/pysolarfocus/components/pellets_boiler.py` & `pysolarfocus-3.6.4/pysolarfocus/components/pellets_boiler.py`

 * *Files identical despite different names*

### Comparing `pysolarfocus-3.6.3/pysolarfocus/components/photovoltaic.py` & `pysolarfocus-3.6.4/pysolarfocus/components/photovoltaic.py`

 * *Files identical despite different names*

### Comparing `pysolarfocus-3.6.3/pysolarfocus/components/solar.py` & `pysolarfocus-3.6.4/pysolarfocus/components/solar.py`

 * *Files identical despite different names*

### Comparing `pysolarfocus-3.6.3/pysolarfocus/const.py` & `pysolarfocus-3.6.4/pysolarfocus/const.py`

 * *Files identical despite different names*

### Comparing `pysolarfocus-3.6.3/pysolarfocus/modbus_wrapper.py` & `pysolarfocus-3.6.4/pysolarfocus/modbus_wrapper.py`

 * *Files identical despite different names*

### Comparing `pysolarfocus-3.6.3/PKG-INFO` & `pysolarfocus-3.6.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysolarfocus
-Version: 3.6.3
+Version: 3.6.4
 Summary: Unofficial, local Solarfocus client
 Home-page: https://github.com/lavermanjj/pysolarfocus
 License: Apache-2.0
 Keywords: solarfocus,api client
 Author: Jeroen Laverman
 Author-email: jjlaverman@web.de
 Requires-Python: >=3.9,<4.0
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pymodbus (==3.2.2)
 Project-URL: Repository, https://github.com/lavermanjj/pysolarfocus
 Description-Content-Type: text/markdown
 
-# pysolarfocus: Python Client for Solarfocus eco<sup>_manager-touch_</sup>
+# pysolarfocus: Python Client for Solarfocus eco<sup>_manager-touch_</sup> via Modbus TCP
 
 Python client library to interact with heating systems of [Solarfocus](https://www.solarfocus.com/) (eco<sup>_manager-touch_</sup> and thermi<sup>nator</sup> II) via Modbus TCP. This library has been developed for the integration into [Home-Assistant](https://www.home-assistant.io/) via a [custom integration](https://github.com/LavermanJJ/home-assistant-solarfocus), but can be used indepdently.
 
 ## What's Supported 
 
 ### Software Version
 
@@ -38,37 +38,81 @@
 |---|---|
 | Heating Circuits (_Heizkreis_) 1-8 | :white_check_mark: |
 | Buffers (_Puffer_) 1-4 | :white_check_mark: |
 | Solar (_Solar_)| :white_check_mark:|
 | Boilers (_Boiler_) 1-4 | :white_check_mark: |
 | Heatpump (_Wärmepumpe_) | :white_check_mark: |
 | Biomassboiler (_Kessel_) | :white_check_mark: | 
-| Fresh Water Module (_Frishwasser Modul_) 1-4 | :white_check_mark: | 
+| Photvoltaic (_Photovoltaik_) | :white_check_mark: | 
+| Fresh Water Module (_Frischwasser Modul_) 1-4 | :white_check_mark: | 
 
 ## How To
 
 ### Basic Example 
 
 ```python
-from pysolarfocus import SolarfocusAPI,Systems
+from pysolarfocus import SolarfocusAPI,Systems,ApiVersions
 
 # Create the Solarfocus API client
-solarfocus = SolarfocusAPI(ip="[Your-IP]",system=Systems.Vampair)
-# Connect to the heating system
-solarfocus.connect() 
+solarfocus = SolarfocusAPI(
+    ip="solarfocus",                    # adapt IP-Address 
+    system=Systems.Vampair,             # for biomass boiler change to Systems.Therminator 
+    api_version=ApiVersions.V_23_020)   # select Solarfocus version
+
+solarfocus.connect()
 # Fetch the values
 solarfocus.update()
 
 # Print the values
-print(solarfocus.buffers[0])
-print(solarfocus.heating_circuit[0])
+print(solarfocus)
+print(solarfocus.heating_circuits[0])
+```
+
+Output: 
+
+```
+--------------------------------------------------
+SolarfocusAPI, v3.6.4
+--------------------------------------------------
++ API Version: 23.020
++ System: Vampair
++ Components:
+  + Heat pump: True
+  + Biomass boiler: False
+  + Heating circuit: 1
+  + Buffer: 1
+  + Boiler: 1
+  + Fresh water module: 1
+  + Solar: False
+  + Photovoltaic: False
+--------------------------------------------------
+
+
+============
+HeatingCircuit
+============
+---Input:
+supply_temperature| raw:258 scaled:25.8
+room_temperature| raw:222 scaled:22.2
+humidity| raw:480 scaled:48.0
+limit_thermostat| raw:1 scaled:1
+circulator_pump| raw:1 scaled:1
+mixer_valve| raw:34 scaled:34
+state| raw:12 scaled:12
+---Holding:
+target_supply_temperature | raw:0 scaled:0.0
+cooling | raw:0 scaled:0
+mode | raw:0 scaled:0
+target_room_temperatur | raw:0 scaled:0.0
+indoor_temperatur_external | raw:222 scaled:22.2
+indoor_humidity_external | raw:480 scaled:48.0
 ```
 
 ### Handling multiple components e.g. heating circuits
-Solarfocus systems allow the use of multiple heating circuits, buffers and boilers. The api can be configured to interact with multiple components.
+Solarfocus systems allow the use of multiple heating circuits, buffers, boilers, and fresh water modules. The api can be configured to interact with multiple components.
 
 ```python 
 # Create the Solarfocus API client with 2 Heating Circuits
 solarfocus = SolarfocusAPI(ip="[Your-IP]",heating_circuit_count=2,system=Systems.Vampair)
 # Connect to the heating system
 solarfocus.connect()
 
@@ -87,21 +131,25 @@
 ```
 
 ### API-Version specification
 By default, the integration uses API-Version`21.140`. If your system is newer, you can specify
 the version by using the `api_version` parameter. 
 
 ```python
-solarfocus = SolarfocusAPI(ip="[Your-IP]", system=Systems.Vampair, api_version=ApiVersions.V_23_010)
+solarfocus = SolarfocusAPI(ip="[Your-IP]", system=Systems.Vampair, api_version=ApiVersions.V_23_020)
 ```
 
+You can find the API-Version displayed in the header of the screen of your Solarfocus system:
+
+<img src="images/sf-version.png?raw=true" width="500">
+
 ## Changelog of API-Versions
 > **Note**
 > The API-Version of Solarfocus is independent of the versions of this library. Below list refers to to 
-> the Solarfocus versions. See [releases](https://github.com/LavermanJJ/pysolarfocus/releases)for the changelog
+> the Solarfocus versions. See [releases](https://github.com/LavermanJJ/pysolarfocus/releases) for the changelog
 > of this library.
 
 
 #### 23.020
 * Add fresh water module state.
 
 #### 23.010
```

