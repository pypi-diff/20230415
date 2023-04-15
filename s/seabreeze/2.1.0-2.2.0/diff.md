# Comparing `tmp/seabreeze-2.1.0.tar.gz` & `tmp/seabreeze-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seabreeze-2.1.0.tar", last modified: Tue Mar 28 10:48:12 2023, max compression
+gzip compressed data, was "seabreeze-2.2.0.tar", last modified: Sat Apr 15 17:57:29 2023, max compression
```

## Comparing `seabreeze-2.1.0.tar` & `seabreeze-2.2.0.tar`

### file list

```diff
@@ -1,1196 +1,1198 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.163887 seabreeze-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-03-28 10:47:34.000000 seabreeze-2.1.0/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-03-28 10:47:34.000000 seabreeze-2.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7308 2023-03-28 10:47:34.000000 seabreeze-2.1.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-03-28 10:47:34.000000 seabreeze-2.1.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-03-28 10:47:34.000000 seabreeze-2.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-03-28 10:48:12.163887 seabreeze-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6278 2023-03-28 10:47:34.000000 seabreeze-2.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.039888 seabreeze-2.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-03-28 10:47:34.000000 seabreeze-2.1.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-03-28 10:47:34.000000 seabreeze-2.1.0/docs/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.043888 seabreeze-2.1.0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.043888 seabreeze-2.1.0/docs/source/_extensions/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-03-28 10:47:34.000000 seabreeze-2.1.0/docs/source/_extensions/repo_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.043888 seabreeze-2.1.0/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    36848 2023-03-28 10:47:34.000000 seabreeze-2.1.0/docs/source/_static/overview.png
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-03-28 10:47:34.000000 seabreeze-2.1.0/docs/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9624 2023-03-28 10:47:34.000000 seabreeze-2.1.0/docs/source/backend_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6040 2023-03-28 10:47:34.000000 seabreeze-2.1.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    10234 2023-03-28 10:47:34.000000 seabreeze-2.1.0/docs/source/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4616 2023-03-28 10:47:34.000000 seabreeze-2.1.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-03-28 10:47:34.000000 seabreeze-2.1.0/docs/source/install.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-03-28 10:47:34.000000 seabreeze-2.1.0/docs/source/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-03-28 10:47:34.000000 seabreeze-2.1.0/docs/source/tldr.rst
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-03-28 10:47:34.000000 seabreeze-2.1.0/docs/source/troubleshoot.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.043888 seabreeze-2.1.0/os_support/
--rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-03-28 10:47:34.000000 seabreeze-2.1.0/os_support/10-oceanoptics.rules
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-03-28 10:47:34.000000 seabreeze-2.1.0/os_support/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)  7255559 2023-03-28 10:47:35.000000 seabreeze-2.1.0/os_support/windows-driver-files.zip
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-03-28 10:47:35.000000 seabreeze-2.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-28 10:47:35.000000 seabreeze-2.1.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-28 10:47:35.000000 seabreeze-2.1.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-28 10:48:12.163887 seabreeze-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     8039 2023-03-28 10:47:35.000000 seabreeze-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.039888 seabreeze-2.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.035889 seabreeze-2.1.0/src/libseabreeze/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.031889 seabreeze-2.1.0/src/libseabreeze/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.051888 seabreeze-2.1.0/src/libseabreeze/include/api/
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/api/DeviceFactory.h
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/api/USBEndpointTypes.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.055888 seabreeze-2.1.0/src/libseabreeze/include/api/seabreezeapi/
--rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/api/seabreezeapi/AcquisitionDelayFeatureAdapter.h
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/api/seabreezeapi/ContinuousStrobeFeatureAdapter.h
--rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/api/seabreezeapi/DHCPServerFeatureAdapter.h
--rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/api/seabreezeapi/DataBufferFeatureAdapter.h
--rw-r--r--   0 runner    (1001) docker     (123)    28448 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/api/seabreezeapi/DeviceAdapter.h
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/api/seabreezeapi/EEPROMFeatureAdapter.h
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/api/seabreezeapi/EthernetConfigurationFeatureAdapter.h
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/api/seabreezeapi/FastBufferFeatureAdapter.h
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/api/seabreezeapi/FeatureAdapterInterface.h
--rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/api/seabreezeapi/FeatureAdapterTemplate.h
--rw-r--r--   0 runner    (1001) docker     (123)     9272 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/api/seabreezeapi/FeatureFamilies.h
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/api/seabreezeapi/I2CMasterFeatureAdapter.h
--rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/api/seabreezeapi/IPv4FeatureAdapter.h
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/api/seabreezeapi/IntrospectionFeatureAdapter.h
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/api/seabreezeapi/IrradCalFeatureAdapter.h
--rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/api/seabreezeapi/LightSourceFeatureAdapter.h
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/api/seabreezeapi/MulticastFeatureAdapter.h
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/api/seabreezeapi/NetworkConfigurationFeatureAdapter.h
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/api/seabreezeapi/NonlinearityCoeffsFeatureAdapter.h
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/api/seabreezeapi/OpticalBenchFeatureAdapter.h
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/api/seabreezeapi/PixelBinningFeatureAdapter.h
--rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/api/seabreezeapi/ProtocolFamilies.h
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/api/seabreezeapi/RawUSBBusAccessFeatureAdapter.h
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/api/seabreezeapi/RevisionFeatureAdapter.h
--rw-r--r--   0 runner    (1001) docker     (123)    29520 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/api/seabreezeapi/SeaBreezeAPI.h
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/api/seabreezeapi/SeaBreezeAPIConstants.h
--rw-r--r--   0 runner    (1001) docker     (123)    26268 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/api/seabreezeapi/SeaBreezeAPI_Impl.h
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/api/seabreezeapi/SerialNumberFeatureAdapter.h
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/api/seabreezeapi/ShutterFeatureAdapter.h
--rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/api/seabreezeapi/SpectrometerFeatureAdapter.h
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/api/seabreezeapi/SpectrumProcessingFeatureAdapter.h
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/api/seabreezeapi/StrayLightCoeffsFeatureAdapter.h
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/api/seabreezeapi/StrobeLampFeatureAdapter.h
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/api/seabreezeapi/TemperatureFeatureAdapter.h
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/api/seabreezeapi/ThermoElectricCoolerFeatureAdapter.h
--rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/api/seabreezeapi/WifiConfigurationFeatureAdapter.h
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/api/seabreezeapi/gpioFeatureAdapter.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.055888 seabreeze-2.1.0/src/libseabreeze/include/common/
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/common/ByteVector.h
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/common/Data.h
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/common/DoubleVector.h
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/common/FloatVector.h
--rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/common/Log.h
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/common/SeaBreeze.h
--rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/common/U32Vector.h
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/common/UShortVector.h
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/common/UnitDescriptor.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.055888 seabreeze-2.1.0/src/libseabreeze/include/common/buses/
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/common/buses/Bus.h
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/common/buses/BusFamilies.h
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/common/buses/BusFamily.h
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/common/buses/DeviceLocationProberInterface.h
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/common/buses/DeviceLocatorInterface.h
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/common/buses/TransferHelper.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.055888 seabreeze-2.1.0/src/libseabreeze/include/common/buses/network/
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/common/buses/network/IPv4NetworkProtocol.h
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/common/buses/network/IPv4SocketDeviceLocator.h
--rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/common/buses/network/TCPIPv4SocketBus.h
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/common/buses/network/TCPIPv4SocketTransferHelper.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.055888 seabreeze-2.1.0/src/libseabreeze/include/common/buses/rs232/
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/common/buses/rs232/RS232DeviceLocator.h
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/common/buses/rs232/RS232Interface.h
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/common/buses/rs232/RS232TransferHelper.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.055888 seabreeze-2.1.0/src/libseabreeze/include/common/buses/usb/
--rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/common/buses/usb/USBDeviceLocator.h
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/common/buses/usb/USBInterface.h
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/common/buses/usb/USBTransferHelper.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.055888 seabreeze-2.1.0/src/libseabreeze/include/common/devices/
--rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/common/devices/Device.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.059888 seabreeze-2.1.0/src/libseabreeze/include/common/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/common/exceptions/BusConnectException.h
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/common/exceptions/BusException.h
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/common/exceptions/BusTransferException.h
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/common/exceptions/FeatureControlException.h
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/common/exceptions/FeatureException.h
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/common/exceptions/FeatureProtocolNotFoundException.h
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/common/exceptions/IllegalArgumentException.h
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/common/exceptions/NumberFormatException.h
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/common/exceptions/ProtocolBusMismatchException.h
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/common/exceptions/ProtocolException.h
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/common/exceptions/ProtocolFormatException.h
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/common/exceptions/ProtocolTransactionException.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.059888 seabreeze-2.1.0/src/libseabreeze/include/common/features/
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/common/features/Feature.h
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/common/features/FeatureFamily.h
--rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/common/features/FeatureImpl.h
--rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/common/globals.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.059888 seabreeze-2.1.0/src/libseabreeze/include/common/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/common/protocols/Exchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/common/protocols/Protocol.h
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/common/protocols/ProtocolFamily.h
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/common/protocols/ProtocolHelper.h
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/common/protocols/ProtocolHint.h
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/common/protocols/Transaction.h
--rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/common/protocols/Transfer.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.031889 seabreeze-2.1.0/src/libseabreeze/include/native/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.059888 seabreeze-2.1.0/src/libseabreeze/include/native/network/
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/native/network/Inet4Address.h
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/native/network/Socket.h
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/native/network/SocketException.h
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/native/network/SocketTimeoutException.h
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/native/network/UnknownHostException.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.059888 seabreeze-2.1.0/src/libseabreeze/include/native/network/posix/
--rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/native/network/posix/NativeSocketPOSIX.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.059888 seabreeze-2.1.0/src/libseabreeze/include/native/network/windows/
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/native/network/windows/NativeSocketWindows.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.059888 seabreeze-2.1.0/src/libseabreeze/include/native/rs232/
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/native/rs232/NativeRS232.h
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/native/rs232/RS232.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.059888 seabreeze-2.1.0/src/libseabreeze/include/native/rs232/windows/
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/native/rs232/windows/NativeRS232Windows.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.059888 seabreeze-2.1.0/src/libseabreeze/include/native/system/
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/native/system/NativeSystem.h
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/native/system/System.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.059888 seabreeze-2.1.0/src/libseabreeze/include/native/usb/
--rw-r--r--   0 runner    (1001) docker     (123)     8474 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/native/usb/NativeUSB.h
--rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/native/usb/USB.h
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/native/usb/USBDiscovery.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.059888 seabreeze-2.1.0/src/libseabreeze/include/native/usb/winusb/
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/native/usb/winusb/WindowsGUID.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.031889 seabreeze-2.1.0/src/libseabreeze/include/vendors/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.031889 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.031889 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/buses/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.059888 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/buses/network/
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/buses/network/FlameXTCPIPv4.h
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/buses/network/JazTCPIPv4.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.059888 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/buses/rs232/
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/buses/rs232/OOIRS232Interface.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.063888 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/ApexUSB.h
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/FlameNIRUSB.h
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/FlameXUSB.h
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/FlameXUSBTransferHelper.h
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/HR2000PlusUSB.h
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/HR2000USB.h
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/HR4000USB.h
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/JazUSB.h
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/Maya2000ProUSB.h
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/Maya2000USB.h
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/MayaLSLUSB.h
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/NIRQuest256USB.h
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/NIRQuest512USB.h
--rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/OOIUSB4KSpectrumTransferHelper.h
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/OOIUSBControlTransferHelper.h
--rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/OOIUSBEndpointMaps.h
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/OOIUSBInterface.h
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/OOIUSBProductID.h
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/OOIUSBSpectrumTransferHelper.h
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/OOIUSBTrivialTransferHelper.h
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/QE65000USB.h
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/QEProUSB.h
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/STSUSB.h
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/SparkUSB.h
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/TorusUSB.h
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/USB2000PlusUSB.h
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/USB2000USB.h
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/USB4000USB.h
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/VentanaUSB.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.067888 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/devices/
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/devices/Apex.h
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/devices/FlameNIR.h
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/devices/FlameX.h
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/devices/HR2000.h
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/devices/HR2000Plus.h
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/devices/HR4000.h
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/devices/Jaz.h
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/devices/Maya2000.h
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/devices/Maya2000Pro.h
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/devices/MayaLSL.h
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/devices/NIRQuest256.h
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/devices/NIRQuest512.h
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/devices/QE65000.h
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/devices/QEPro.h
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/devices/STS.h
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/devices/Spark.h
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/devices/Torus.h
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/devices/USB2000.h
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/devices/USB2000Plus.h
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/devices/USB4000.h
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/devices/Ventana.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.031889 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.067888 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/acquisition_delay/
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/acquisition_delay/AcquisitionDelayFeature.h
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/acquisition_delay/AcquisitionDelayFeatureInterface.h
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/acquisition_delay/AcquisitionDelayFeature_FPGA.h
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/acquisition_delay/STSAcquisitionDelayFeature.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.067888 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/continuous_strobe/
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/continuous_strobe/ContinuousStrobeFeature.h
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/continuous_strobe/ContinuousStrobeFeatureInterface.h
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/continuous_strobe/ContinuousStrobeFeature_FPGA.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.067888 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/data_buffer/
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/data_buffer/DataBufferFeatureBase.h
--rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/data_buffer/DataBufferFeatureInterface.h
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/data_buffer/FlameXDataBufferFeature.h
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/data_buffer/QEProDataBufferFeature.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.067888 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/dhcp_server/
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/dhcp_server/DHCPServerFeature.h
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/dhcp_server/DHCPServerFeatureInterface.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.071888 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/EEPROMSlotFeature.h
--rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/EEPROMSlotFeatureBase.h
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/EEPROMSlotFeatureInterface.h
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/NonlinearityEEPROMSlotFeature.h
--rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/SaturationEEPROMSlotFeature.h
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/SaturationEEPROMSlotFeatureBase.h
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/SaturationEEPROMSlotFeature_MayaPro.h
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/SaturationEEPROMSlotFeature_NIRQuest.h
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/SerialNumberEEPROMSlotFeature.h
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/StrayLightEEPROMSlotFeature.h
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/WavelengthEEPROMSlotFeature.h
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/WavelengthEEPROMSlotFeature_QE65000.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.071888 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/ethernet_configuration/
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/ethernet_configuration/EthernetConfigurationFeature.h
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/ethernet_configuration/EthernetConfigurationFeatureInterface.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.071888 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/fast_buffer/
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/fast_buffer/FastBufferFeatureBase.h
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/fast_buffer/FastBufferFeatureInterface.h
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/fast_buffer/FlameXFastBufferFeature.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.071888 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/fpga_register/
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/fpga_register/FPGARegisterFeature.h
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/fpga_register/FPGARegisterFeatureInterface.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.071888 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/gpio/
--rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/gpio/gpioFeature.h
--rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/gpio/gpioFeatureInterface.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.071888 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/i2c_master/
--rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/i2c_master/i2cMasterFeature.h
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/i2c_master/i2cMasterFeatureInterface.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.071888 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/introspection/
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/introspection/IntrospectionFeature.h
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/introspection/IntrospectionFeatureInterface.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.071888 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/ipv4/
--rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/ipv4/IPv4Feature.h
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/ipv4/IPv4FeatureInterface.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.071888 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/irradcal/
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/irradcal/IrradCalFeature.h
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/irradcal/IrradCalFeatureInterface.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.071888 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/light_source/
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/light_source/LightSourceFeatureBase.h
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/light_source/LightSourceFeatureImpl.h
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/light_source/LightSourceFeatureInterface.h
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/light_source/StrobeLampFeature.h
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/light_source/StrobeLampFeatureInterface.h
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/light_source/VentanaLightSourceFeature.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.071888 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/multicast/
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/multicast/MulticastFeature.h
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/multicast/MulticastFeatureInterface.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.071888 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/network_configuration/
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/network_configuration/NetworkConfigurationFeature.h
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/network_configuration/NetworkConfigurationFeatureInterface.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.071888 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/nonlinearity/
--rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/nonlinearity/NonlinearityCoeffsFeature.h
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/nonlinearity/NonlinearityCoeffsFeatureInterface.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.071888 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/optical_bench/
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/optical_bench/OpticalBenchFeature.h
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/optical_bench/OpticalBenchFeatureInterface.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.075888 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/pixel_binning/
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/pixel_binning/PixelBinningFeatureInterface.h
--rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/pixel_binning/STSPixelBinningFeature.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.075888 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/raw_bus_access/
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/raw_bus_access/RawUSBBusAccessFeature.h
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/raw_bus_access/RawUSBBusAccessFeatureInterface.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.075888 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/revision/
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/revision/RevisionFeature.h
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/revision/RevisionFeatureInterface.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.075888 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/serial_number/
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/serial_number/SerialNumberFeature.h
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/serial_number/SerialNumberFeatureInterface.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.075888 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/shutter/
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/shutter/ShutterFeature.h
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/shutter/ShutterFeatureInterface.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.079888 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/ApexSpectrometerFeature.h
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/FlameNIRSpectrometerFeature.h
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/FlameXSpectrometerFeature.h
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/GainAdjustedSpectrometerFeature.h
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/HR2000PlusSpectrometerFeature.h
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/HR2000SpectrometerFeature.h
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/HR4000SpectrometerFeature.h
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/JazSpectrometerFeature.h
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/Maya2000ProSpectrometerFeature.h
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/Maya2000SpectrometerFeature.h
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/MayaLSLSpectrometerFeature.h
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/NIRQuest256SpectrometerFeature.h
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/NIRQuest512SpectrometerFeature.h
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/NIRQuestSpectrometerFeature.h
--rw-r--r--   0 runner    (1001) docker     (123)     5579 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/OOISpectrometerFeature.h
--rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/OOISpectrometerFeatureInterface.h
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/ProgrammableSaturationFeature.h
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/ProgrammableSaturationFeatureBase.h
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/ProgrammableSaturationFeatureImpl.h
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/ProgrammableSaturationFeatureInterface.h
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/QE65000SpectrometerFeature.h
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/QEProSpectrometerFeature.h
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/STSSpectrometerFeature.h
--rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/SparkSpectrometerFeature.h
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/SpectrometerTriggerMode.h
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/USB2000PlusSpectrometerFeature.h
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/USB2000SpectrometerFeature.h
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/USB4000SpectrometerFeature.h
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/VentanaSpectrometerFeature.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.079888 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrum_processing/
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrum_processing/SpectrumProcessingFeature.h
--rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrum_processing/SpectrumProcessingFeatureInterface.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.079888 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/stray_light/
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/stray_light/StrayLightCoeffsFeature.h
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/stray_light/StrayLightCoeffsFeatureInterface.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.079888 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/temperature/
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/temperature/TemperatureFeature.h
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/temperature/TemperatureFeatureInterface.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.079888 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/thermoelectric/
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/thermoelectric/QEProThermoElectricFeature.h
--rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/thermoelectric/ThermoElectricFeatureBase.h
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/thermoelectric/ThermoElectricFeatureInterface.h
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/thermoelectric/ThermoElectricQEFeature.h
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/thermoelectric/VentanaThermoElectricFeature.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.079888 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/wavecal/
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/wavecal/WaveCalFeature.h
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/wavecal/WaveCalFeatureInterface.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.079888 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/wifi_configuration/
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/wifi_configuration/WifiConfigurationFeature.h
--rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/wifi_configuration/WifiConfigurationFeatureInterface.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.031889 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.083888 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/AcquisitionDelayProtocolInterface.h
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/ContinuousStrobeProtocolInterface.h
--rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/DHCPServerProtocolInterface.h
--rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/DataBufferProtocolInterface.h
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/EEPROMProtocolInterface.h
--rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/EthernetConfigurationProtocolInterface.h
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/FPGARegisterProtocolInterface.h
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/FastBufferProtocolInterface.h
--rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/GPIOProtocolInterface.h
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/I2CMasterProtocolInterface.h
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/IPv4ProtocolInterface.h
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/IntrospectionProtocolInterface.h
--rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/IrradCalProtocolInterface.h
--rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/LightSourceProtocolInterface.h
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/MulticastProtocolInterface.h
--rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/NetworkConfigurationProtocolInterface.h
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/NonlinearityCoeffsProtocolInterface.h
--rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/OpticalBenchProtocolInterface.h
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/PixelBinningProtocolInterface.h
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/ProgrammableSaturationProtocolInterface.h
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/RevisionProtocolInterface.h
--rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/SerialNumberProtocolInterface.h
--rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/ShutterProtocolInterface.h
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/SpectrometerProtocolInterface.h
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/SpectrumProcessingProtocolInterface.h
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/StrayLightCoeffsProtocolInterface.h
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/StrobeLampProtocolInterface.h
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/TemperatureProtocolInterface.h
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/ThermoElectricProtocolInterface.h
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/WaveCalProtocolInterface.h
--rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/WifiConfigurationProtocolInterface.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.031889 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.083888 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/constants/
--rw-r--r--   0 runner    (1001) docker     (123)    21778 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/constants/OBPMessageTypes.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.095888 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPAddIPv4AddressExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPCommand.h
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPContinuousStrobeEnableExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPContinuousStrobePeriodExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPDataBufferClearExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPDataBufferRemoveOldestExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPDeleteIPv4AddressExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetActivePixelRangesExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetAllTemperaturesExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetBoxcarWidthExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetConsecutiveSampleCountExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDHCPServerAddressExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDHCPServerEnableExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDataBufferCapacityExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDataBufferElementCountExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDataBufferMaximumCapacityExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDefaultPixelBinningExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetElectricDarkPixelRangesExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetEthernetConfigurationGbEEnableExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetEthernetConfigurationMACAddressExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetFastBufferingEnableExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetFirmwareRevisionExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOExtensionAvailableModesExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOExtensionCurrentModeExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOExtensionNumberOfPinsExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOExtensionOutputVectorExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOExtensionValueExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIONumberOfPinsExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOOutputEnableVectorExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOValueVectorExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetHardwareRevisionExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetI2CMasterNumberOfBusesExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIPv4AddressExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIPv4DHCPEnableStateExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIPv4DefaultGatewayExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIPv4NumberOfAddressesExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIrradCalExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIrradCollectionAreaExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetMaxPixelBinningExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetMulticastEnableExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNetworkInterfaceConnectionTypeExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNetworkInterfaceEnableStateExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNonlinearityCoeffExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNonlinearityCoeffsCountExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNumberOfNetworkInterfacesExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNumberOfPixelsExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchCoatingExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchFiberDiameterMicronsExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchFilterExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchGratingExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchIDExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchSerialNumberExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchSlitWidthMicronsExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalDarkPixelRangesExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetPixelBinningExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetSaturationExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetScansToAverageExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetSerialNumberExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetSerialNumberMaximumLengthExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetStrayLightCoeffExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetStrayLightCoeffsCountExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetTemperatureCountExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetTemperatureExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetThermoElectricTemperatureExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetWaveCalExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetWifiConfigurationModeExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetWifiConfigurationSSIDExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetWifiConfigurationSecurityExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPIntegrationTimeExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPLampEnableCommand.h
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPLightSourceEnableCommand.h
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPLightSourceEnabledQuery.h
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPLightSourceIntensityCommand.h
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPLightSourceIntensityQuery.h
--rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPMessage.h
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPQuery.h
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPReadI2CMasterBusExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPReadNumberOfRawSpectraWithMetadataExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPReadRawSpectrum32AndMetadataExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPReadRawSpectrumExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPReadSpectrum32AndMetadataExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPReadSpectrumExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPReadSpectrumWithGainExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPRequestBufferedSpectrum32AndMetadataExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPRequestNumberOfBufferedSpectraWithMetadataExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPRequestRawSpectrumExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPRequestSpectrumExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPRunNetworkInterfaceSelfTestExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSaveNetworkInterfaceConnectionSettingsExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetAcquisitionDelayExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetBoxcarWidthExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetConsecutiveSampleCountExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetDHCPServerAddressExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetDHCPServerEnableExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetDataBufferCapacityExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetDefaultPixelBinningExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetEthernetConfigurationGbEEnableExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetEthernetConfigurationMACAddressExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetFastBufferingEnableExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetGPIOExtensionModeExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetGPIOExtensionOutputVectorExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetGPIOExtensionValueExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetGPIOExtensionVectorExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetGPIOOutputEnableVectorExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetGPIOValueVectorExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetIPv4DHCPEnableStateExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetIPv4DefaultGatewayExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetIrradCalExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetIrradCollectionAreaExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetMulticastEnableExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetNetworkInterfaceEnableStateExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetPixelBinningExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetScansToAverageExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetThermoElectricEnableExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetThermoElectricSetpointExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetWifiConfigurationModeExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetWifiConfigurationPassPhraseExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetWifiConfigurationSSIDExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetWifiConfigurationSecurityExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPShutterExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPTransaction.h
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPTriggerModeExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPWriteI2CMasterBusExchange.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.095888 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/hints/
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/hints/OBPControlHint.h
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/hints/OBPSpectrumHint.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.099888 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPAcquisitionDelayProtocol.h
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPContinuousStrobeProtocol.h
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPDHCPServerProtocol.h
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPDataBufferProtocol.h
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPEthernetConfigurationProtocol.h
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPFastBufferProtocol.h
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPGPIOProtocol.h
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPI2CMasterProtocol.h
--rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPIPv4Protocol.h
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPIntrospectionProtocol.h
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPIrradCalProtocol.h
--rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPLightSourceProtocol.h
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPLightSourceProtocol_Ventana.h
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPMulticastProtocol.h
--rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPNetworkConfigurationProtocol.h
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPNonlinearityCoeffsProtocol.h
--rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPOpticalBenchProtocol.h
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPPixelBinningProtocol.h
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPProgrammableSaturationProtocol.h
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPRevisionProtocol.h
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPSerialNumberProtocol.h
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPShutterProtocol.h
--rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPSpectrometerProtocol.h
--rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPSpectrumProcessingProtocol.h
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPStrayLightCoeffsProtocol.h
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPStrobeLampProtocol.h
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPTemperatureProtocol.h
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPThermoElectricProtocol.h
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPWaveCalProtocol.h
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPWifiConfigurationProtocol.h
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OceanBinaryProtocol.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.031889 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.099888 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/constants/
--rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/constants/FPGARegisterCodes.h
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/constants/OpCodes.h
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/constants/QETECConstants.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.103888 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/FPGARegisterReadExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/FPGARegisterWriteExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/FPGASpectrumExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/FlameNIRSpectrumExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/HRFPGASpectrumExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/IntegrationTimeExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/JazSpectrumExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/MayaProSpectrumExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/NIRQuestSpectrumExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/OOI2KSpectrumExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/OOIIrradCalExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/OOIReadIrradCalExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/OOIWriteIrradCalExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/QESpectrumExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/ReadEEPROMSlotExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/ReadSpectrumExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/ReadTECQETemperatureExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/ReadTECTemperatureExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/RequestSpectrumExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/StrobeEnableExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/TECEnableExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/TECQEEnableExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/TriggerModeExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/USBFPGASpectrumExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/WriteEEPROMSlotExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/WriteTECQESetPointExchange.h
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/WriteTECSetPointExchange.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.103888 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/hints/
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/hints/ControlHint.h
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/hints/SpectrumHint.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.103888 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/impls/
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/impls/FPGARegisterProtocol.h
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/impls/OOIEEPROMProtocol.h
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/impls/OOIIrradCalProtocol.h
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/impls/OOIProtocol.h
--rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/impls/OOISpectrometerProtocol.h
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/impls/OOIStrobeLampProtocol.h
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/impls/OOITECProtocol.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.103888 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/utils/Polynomial.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.035889 seabreeze-2.1.0/src/libseabreeze/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.103888 seabreeze-2.1.0/src/libseabreeze/src/api/
--rw-r--r--   0 runner    (1001) docker     (123)     6249 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/api/DeviceFactory.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.107888 seabreeze-2.1.0/src/libseabreeze/src/api/seabreezeapi/
--rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/api/seabreezeapi/AcquisitionDelayFeatureAdapter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/api/seabreezeapi/ContinuousStrobeFeatureAdapter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/api/seabreezeapi/DHCPServerFeatureAdapter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/api/seabreezeapi/DataBufferFeatureAdapter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    80076 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/api/seabreezeapi/DeviceAdapter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/api/seabreezeapi/EEPROMFeatureAdapter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4306 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/api/seabreezeapi/EthernetConfigurationFeatureAdapter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/api/seabreezeapi/FastBufferFeatureAdapter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    12485 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/api/seabreezeapi/FeatureFamilies.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/api/seabreezeapi/I2CMasterFeatureAdapter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6106 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/api/seabreezeapi/IPv4FeatureAdapter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5019 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/api/seabreezeapi/IntrospectionFeatureAdapter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/api/seabreezeapi/IrradCalFeatureAdapter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/api/seabreezeapi/LightSourceFeatureAdapter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/api/seabreezeapi/MulticastFeatureAdapter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4770 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/api/seabreezeapi/NetworkConfigurationFeatureAdapter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/api/seabreezeapi/NonlinearityCoeffsFeatureAdapter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7338 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/api/seabreezeapi/OpticalBenchFeatureAdapter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/api/seabreezeapi/PixelBinningFeatureAdapter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/api/seabreezeapi/ProtocolFamilies.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4371 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/api/seabreezeapi/RawUSBBusAccessFeatureAdapter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/api/seabreezeapi/RevisionFeatureAdapter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/api/seabreezeapi/SeaBreezeAPI.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    87831 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/api/seabreezeapi/SeaBreezeAPI_Impl.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/api/seabreezeapi/SerialNumberFeatureAdapter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/api/seabreezeapi/ShutterFeatureAdapter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    12647 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/api/seabreezeapi/SpectrometerFeatureAdapter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4445 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/api/seabreezeapi/SpectrumProcessingFeatureAdapter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/api/seabreezeapi/StrayLightCoeffsFeatureAdapter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/api/seabreezeapi/StrobeLampFeatureAdapter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/api/seabreezeapi/TemperatureFeatureAdapter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/api/seabreezeapi/ThermoElectricCoolerFeatureAdapter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5946 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/api/seabreezeapi/WifiConfigurationFeatureAdapter.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6995 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/api/seabreezeapi/gpioFeatureAdapter.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.111888 seabreeze-2.1.0/src/libseabreeze/src/common/
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/common/ByteVector.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/common/Data.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/common/DoubleVector.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/common/FloatVector.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6490 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/common/Log.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/common/U32Vector.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/common/UShortVector.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/common/UnitDescriptor.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.111888 seabreeze-2.1.0/src/libseabreeze/src/common/buses/
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/common/buses/Bus.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/common/buses/BusFamilies.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/common/buses/BusFamily.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/common/buses/DeviceLocationProberInterface.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/common/buses/TransferHelper.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.111888 seabreeze-2.1.0/src/libseabreeze/src/common/buses/network/
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/common/buses/network/IPv4NetworkProtocol.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/common/buses/network/IPv4SocketDeviceLocator.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/common/buses/network/TCPIPv4SocketBus.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/common/buses/network/TCPIPv4SocketTransferHelper.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.111888 seabreeze-2.1.0/src/libseabreeze/src/common/buses/rs232/
--rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/common/buses/rs232/RS232DeviceLocator.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/common/buses/rs232/RS232Interface.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/common/buses/rs232/RS232TransferHelper.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.111888 seabreeze-2.1.0/src/libseabreeze/src/common/buses/usb/
--rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/common/buses/usb/USBDeviceLocator.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/common/buses/usb/USBInterface.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/common/buses/usb/USBTransferHelper.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.111888 seabreeze-2.1.0/src/libseabreeze/src/common/devices/
--rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/common/devices/Device.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.111888 seabreeze-2.1.0/src/libseabreeze/src/common/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/common/exceptions/BusConnectException.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/common/exceptions/BusException.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/common/exceptions/BusTransferException.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/common/exceptions/FeatureControlException.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/common/exceptions/FeatureException.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/common/exceptions/FeatureProtocolNotFoundException.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/common/exceptions/IllegalArgumentException.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/common/exceptions/NumberFormatException.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/common/exceptions/ProtocolBusMismatchException.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/common/exceptions/ProtocolException.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/common/exceptions/ProtocolFormatException.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/common/exceptions/ProtocolTransactionException.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.111888 seabreeze-2.1.0/src/libseabreeze/src/common/features/
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/common/features/FeatureFamily.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/common/features/FeatureImpl.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.115888 seabreeze-2.1.0/src/libseabreeze/src/common/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/common/protocols/Exchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/common/protocols/Protocol.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/common/protocols/ProtocolFamily.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/common/protocols/ProtocolHelper.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/common/protocols/ProtocolHint.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/common/protocols/Transaction.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/common/protocols/Transfer.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.035889 seabreeze-2.1.0/src/libseabreeze/src/native/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.115888 seabreeze-2.1.0/src/libseabreeze/src/native/network/
--rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/native/network/Inet4Address.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/native/network/SocketException.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/native/network/SocketTimeoutException.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/native/network/UnknownHostException.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.115888 seabreeze-2.1.0/src/libseabreeze/src/native/network/posix/
--rw-r--r--   0 runner    (1001) docker     (123)     7271 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/native/network/posix/NativeSocketPOSIX.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.115888 seabreeze-2.1.0/src/libseabreeze/src/native/network/windows/
--rw-r--r--   0 runner    (1001) docker     (123)     7149 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/native/network/windows/NativeSocketWindows.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.115888 seabreeze-2.1.0/src/libseabreeze/src/native/rs232/
--rw-r--r--   0 runner    (1001) docker     (123)     6555 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/native/rs232/RS232.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.115888 seabreeze-2.1.0/src/libseabreeze/src/native/rs232/posix/
--rw-r--r--   0 runner    (1001) docker     (123)    12360 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/native/rs232/posix/NativeRS232POSIX.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.115888 seabreeze-2.1.0/src/libseabreeze/src/native/rs232/windows/
--rw-r--r--   0 runner    (1001) docker     (123)     7796 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/native/rs232/windows/NativeRS232Windows.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.115888 seabreeze-2.1.0/src/libseabreeze/src/native/system/
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/native/system/System.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.115888 seabreeze-2.1.0/src/libseabreeze/src/native/system/posix/
--rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/native/system/posix/NativeSystemPOSIX.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.115888 seabreeze-2.1.0/src/libseabreeze/src/native/system/windows/
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/native/system/windows/NativeSystemWindows.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.115888 seabreeze-2.1.0/src/libseabreeze/src/native/usb/
--rw-r--r--   0 runner    (1001) docker     (123)     9909 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/native/usb/USB.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/native/usb/USBDiscovery.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.115888 seabreeze-2.1.0/src/libseabreeze/src/native/usb/linux/
--rw-r--r--   0 runner    (1001) docker     (123)    22561 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/native/usb/linux/NativeUSBLinux.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.115888 seabreeze-2.1.0/src/libseabreeze/src/native/usb/osx/
--rw-r--r--   0 runner    (1001) docker     (123)    38021 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/native/usb/osx/NativeUSBMacOSX.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.115888 seabreeze-2.1.0/src/libseabreeze/src/native/usb/winusb/
--rw-r--r--   0 runner    (1001) docker     (123)    28911 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/native/usb/winusb/NativeUSBWinUSB.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.035889 seabreeze-2.1.0/src/libseabreeze/src/vendors/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.039888 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.035889 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/buses/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.115888 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/buses/network/
--rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/buses/network/FlameXTCPIPv4.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/buses/network/JazTCPIPv4.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.115888 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/buses/rs232/
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/buses/rs232/OOIRS232Interface.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.119888 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/ApexUSB.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/FlameNIRUSB.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/FlameXUSB.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/FlameXUSBTransferHelper.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/HR2000PlusUSB.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/HR2000USB.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/HR4000USB.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/JazUSB.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/Maya2000ProUSB.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/Maya2000USB.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/MayaLSLUSB.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/NIRQuest256USB.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/NIRQuest512USB.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/OOIUSB4KSpectrumTransferHelper.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/OOIUSBControlTransferHelper.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/OOIUSBEndpointMaps.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5452 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/OOIUSBInterface.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/OOIUSBSpectrumTransferHelper.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/OOIUSBTrivialTransferHelper.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/QE65000USB.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/QEProUSB.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/STSUSB.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/SparkUSB.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/TorusUSB.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/USB2000PlusUSB.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/USB2000USB.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/USB4000USB.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/VentanaUSB.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.123888 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/devices/
--rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/devices/Apex.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/devices/FlameNIR.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9704 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/devices/FlameX.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/devices/HR2000.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/devices/HR2000Plus.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/devices/HR4000.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/devices/Jaz.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4951 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/devices/Maya2000.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/devices/Maya2000Pro.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4799 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/devices/MayaLSL.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/devices/NIRQuest256.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/devices/NIRQuest512.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5081 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/devices/QE65000.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6351 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/devices/QEPro.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8466 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/devices/STS.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7144 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/devices/Spark.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/devices/Torus.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/devices/USB2000.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5072 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/devices/USB2000Plus.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4797 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/devices/USB4000.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7724 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/devices/Ventana.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.039888 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.123888 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/acquisition_delay/
--rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/acquisition_delay/AcquisitionDelayFeature.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5221 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/acquisition_delay/AcquisitionDelayFeature_FPGA.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/acquisition_delay/STSAcquisitionDelayFeature.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.123888 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/continuous_strobe/
--rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/continuous_strobe/ContinuousStrobeFeature.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/continuous_strobe/ContinuousStrobeFeature_FPGA.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.123888 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/data_buffer/
--rw-r--r--   0 runner    (1001) docker     (123)    10049 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/data_buffer/DataBufferFeatureBase.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/data_buffer/FlameXDataBufferFeature.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/data_buffer/QEProDataBufferFeature.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.123888 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/dhcp_server/
--rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/dhcp_server/DHCPServerFeature.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.123888 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/
--rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/EEPROMSlotFeature.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6938 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/EEPROMSlotFeatureBase.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/NonlinearityEEPROMSlotFeature.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/SaturationEEPROMSlotFeature.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/SaturationEEPROMSlotFeatureBase.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/SaturationEEPROMSlotFeature_MayaPro.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/SaturationEEPROMSlotFeature_NIRQuest.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/SerialNumberEEPROMSlotFeature.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/StrayLightEEPROMSlotFeature.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3774 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/WavelengthEEPROMSlotFeature.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/WavelengthEEPROMSlotFeature_QE65000.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.123888 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/ethernet_configuration/
--rw-r--r--   0 runner    (1001) docker     (123)     6763 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/ethernet_configuration/EthernetConfigurationFeature.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.123888 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/fast_buffer/
--rw-r--r--   0 runner    (1001) docker     (123)     6310 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/fast_buffer/FastBufferFeatureBase.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/fast_buffer/FlameXFastBufferFeature.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.123888 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/fpga_register/
--rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/fpga_register/FPGARegisterFeature.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.123888 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/gpio/
--rw-r--r--   0 runner    (1001) docker     (123)    13793 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/gpio/gpioFeature.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.123888 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/i2c_master/
--rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/i2c_master/i2cFeature.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.123888 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/introspection/
--rw-r--r--   0 runner    (1001) docker     (123)     6646 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/introspection/IntrospectionFeature.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.123888 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/ipv4/
--rw-r--r--   0 runner    (1001) docker     (123)     9822 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/ipv4/IPv4Feature.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.123888 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/irradcal/
--rw-r--r--   0 runner    (1001) docker     (123)     6711 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/irradcal/IrradCalFeature.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.127888 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/light_source/
--rw-r--r--   0 runner    (1001) docker     (123)    14844 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/light_source/LightSourceFeatureBase.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/light_source/LightSourceFeatureImpl.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/light_source/StrobeLampFeature.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/light_source/VentanaLightSourceFeature.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.127888 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/multicast/
--rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/multicast/MulticastFeature.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.127888 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/network_configuration/
--rw-r--r--   0 runner    (1001) docker     (123)     8675 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/network_configuration/NetworkConfigurationFeature.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.127888 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/nonlinearity/
--rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/nonlinearity/NonlinearityCoeffsFeature.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.127888 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/optical_bench/
--rw-r--r--   0 runner    (1001) docker     (123)     9817 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/optical_bench/OpticalBenchFeature.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.127888 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/pixel_binning/
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/pixel_binning/PixelBinningFeatureInterface.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9620 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/pixel_binning/STSPixelBinningFeature.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.127888 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/raw_bus_access/
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/raw_bus_access/RawUSBBusAccessFeature.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.127888 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/revision/
--rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/revision/RevisionFeature.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.127888 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/serial_number/
--rw-r--r--   0 runner    (1001) docker     (123)     4465 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/serial_number/SerialNumberFeature.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.127888 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/shutter/
--rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/shutter/ShutterFeature.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.131888 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/
--rw-r--r--   0 runner    (1001) docker     (123)     4708 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/ApexSpectrometerFeature.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/FlameNIRSpectrometerFeature.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7869 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/FlameXSpectrometerFeature.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/GainAdjustedSpectrometerFeature.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/HR2000PlusSpectrometerFeature.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4348 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/HR2000SpectrometerFeature.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4390 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/HR4000SpectrometerFeature.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/JazSpectrometerFeature.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/Maya2000ProSpectrometerFeature.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4465 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/Maya2000SpectrometerFeature.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/MayaLSLSpectrometerFeature.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/NIRQuest256SpectrometerFeature.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/NIRQuest512SpectrometerFeature.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/NIRQuestSpectrometerFeature.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    14571 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/OOISpectrometerFeature.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/ProgrammableSaturationFeature.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/ProgrammableSaturationFeatureBase.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/ProgrammableSaturationFeatureImpl.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/QE65000SpectrometerFeature.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/QEProSpectrometerFeature.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5874 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/STSSpectrometerFeature.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/SparkSpectrometerFeature.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/SpectrometerTriggerMode.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4713 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/USB2000PlusSpectrometerFeature.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/USB2000SpectrometerFeature.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/USB4000SpectrometerFeature.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/VentanaSpectrometerFeature.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.131888 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrum_processing/
--rw-r--r--   0 runner    (1001) docker     (123)     6867 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrum_processing/SpectrumProcessingFeature.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.131888 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/stray_light/
--rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/stray_light/StrayLightCoeffsFeature.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.131888 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/temperature/
--rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/temperature/TemperatureFeature.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.131888 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/thermoelectric/
--rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/thermoelectric/QEProThermoElectricFeature.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/thermoelectric/ThermoElectricFeatureBase.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/thermoelectric/ThermoElectricQEFeature.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/thermoelectric/VentanaThermoElectricFeature.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.131888 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/wavecal/
--rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/wavecal/WaveCalFeature.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.131888 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/wifi_configuration/
--rw-r--r--   0 runner    (1001) docker     (123)     9640 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/wifi_configuration/WifiConfigurationFeature.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.039888 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.135887 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/AcquisitionDelayProtocolInterface.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/ContinuousStrobeProtocolInterface.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/DHCPServerProtocolInterface.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/DataBufferProtocolInterface.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/EEPROMProtocolInterface.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/EthernetConfigurationProtocolInterface.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/FPGARegisterProtocolInterface.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/FastBufferProtocolInterface.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/GPIOProtocolInterface.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/I2CMasterProtocolInterface.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/IPv4ProtocolInterface.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/IntrospectionProtocolInterface.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/IrradCalProtocolInterface.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/LightSourceProtocolInterface.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/MulticastProtocolInterface.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/NetworkConfigurationProtocolInterface.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/NonlinearityCoeffsProtocolInterface.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/OpticalBenchProtocolInteface.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/PixelBinningProtocolInterface.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/ProgrammableSaturationProtocolInteface.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/RevisionProtocolInteface.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/SerialNumberProtocolInterface.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/ShutterProtocolInterface.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/SpectrometerProtocolInterface.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/SpectrumProcessingProtocolInteface.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/StrayLightCoeffsProtocolInterface.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/StrobeLampProtocolInterface.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/TemperatureProtocolInteface.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/ThermoElectricProtocolInterface.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/WaveCalProtocolInterface.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/WifiConfigurationProtocolInterface.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.039888 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.147887 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPAddIPv4AddressExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPCommand.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPContinuousStrobeEnableExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPContinuousStrobePeriodExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPDataBufferClearExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPDataBufferRemoveOldestExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPDeleteIPv4AddressExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetActivePixelRangesExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetAllTemperaturesExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetBoxcarWidthExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetConsecutiveSampleCountExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDHCPServerAddressExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDHCPServerEnableExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDataBufferCapacityExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDataBufferCountExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDataBufferMaximumCapacityExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDefaultPixelBinningExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetElectricDarkPixelRangesExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetEthernetConfigurationGbEEnableExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetEthernetConfigurationMACAddressExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetFastBufferingEnableExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetFirmwareRevisionExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOExtensionAvailableModesExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOExtensionCurrentModeExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOExtensionNumberOfPinsExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOExtensionOutputVectorExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOExtensionValueExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIONumberOfPinsExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOOutputEnableVectorExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOValueVectorExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetHardwareRevisionExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetI2CMasterNumberOfBusesExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIPv4AddressExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIPv4DHCPEnableStateExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIPv4DefaultGatewayExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIPv4NumberOfAddressesExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIrradCalExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIrradCollectionAreaExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetMaxPixelBinningExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetMulticastEnableExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNetworkInterfaceConnectionTypeExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNetworkInterfaceEnableStateExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNonlinearityCoeffExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNonlinearityCoeffsCountExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNumberOfNetworkInterfacesExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNumberOfPixelsExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchCoatingExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchFiberDiameterMicronsExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchFilterExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchGratingExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchIDExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchSerialNumberExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchSlitWidthMicronsExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalDarkPixelRangesExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetPixelBinningExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetSaturationExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetScansToAverageExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetSerialNumberExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetSerialNumberMaximumLengthExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetStrayLightCoeffExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetStrayLightCoeffsCountExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetTemperatureCountExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetTemperatureExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetThermoElectricTemperatureExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetWaveCalExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetWifiConfigurationModeExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetWifiConfigurationSSIDExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetWifiConfigurationSecurityExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPIntegrationTimeExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPLampEnableCommand.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPLightSourceEnableCommand.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPLightSourceEnabledQuery.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPLightSourceIntensityCommand.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPLightSourceIntensityQuery.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    12839 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPMessage.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPQuery.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPReadI2CMasterBusExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5658 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPReadNumberOfRawSpectraWithMetadataExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5017 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPReadRawSpectrum32AndMetadataExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4616 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPReadRawSpectrumExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPReadSpectrum32AndMetadataExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPReadSpectrumExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPReadSpectrumWithGainExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPRequestBufferedSpectrum32AndMetadata.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPRequestNumberOfBufferedSpectraWithMetadata.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPRequestRawSpectrumExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPRequestSpectrumExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPRunNetworkInterfaceSelfTestExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSaveNetworkInterfaceConnectionSettingsExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetAcquisitionDelayExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetBoxcarWidthExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetConsecutiveSampleCountExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetDHCPServerAddressExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetDHCPServerEnableExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetDataBufferCapacityExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetDefaultPixelBinningFactorExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetEthernetConfigurationGbEEnableExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetEthernetConfigurationMACAddressExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetFastBufferingEnableExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetGPIOExtensionModeExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetGPIOExtensionOutputVectorExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetGPIOExtensionValueExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetGPIOOutputEnableVectorExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetGPIOValueVectorExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetIPv4DHCPEnableStateExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetIPv4DefaultGatewayExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetIrradCalExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetIrradCollectionAreaExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetMulticastEnableExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetNetworkInterfaceEnableStateExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetPixelBinningExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetScansToAverageExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetThermoElectricEnableExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetThermoElectricSetpointExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetWifiConfigurationModeExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetWifiConfigurationPassPhraseExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetWifiConfigurationSSIDExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetWifiConfigurationSecurityExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPShutterExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    10484 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPTransaction.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPTriggerModeExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPWriteI2CMasterBusExchange.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.147887 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/hints/
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/hints/OBPControlHint.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/hints/OBPSpectrumHint.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.151887 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/
--rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPAcquisitionDelayProtocol.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPContinuousStrobeProtocol.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6070 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPDHCPServerProtocol.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9129 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPDataBufferProtocol.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPEthernetConfigurationProtocol.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPFastBufferProtocol.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    13773 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPGPIOProtocol.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5371 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPI2CMasterProtocol.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9506 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPIPv4Protocol.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPIntrospectionProtocol.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6699 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPIrradCalProtocol.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPLightSourceProtocol.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPLightSourceProtocol_Ventana.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5637 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPMulticastProtocol.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7815 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPNetworkConfigurationProtocol.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPNonlinearityCoeffsProtocol.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11491 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPOpticalBenchProtocol.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPPixelBinningProtocol.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPProgrammableSaturationProtocol.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPRevisionProtocol.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPSerialNumberProtocol.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPShutterProtocol.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    12416 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPSpectrometerProtocol.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5673 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPSpectrumProcessingProtocol.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPStrayLightCoeffsProtocol.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPStrobeLampProtocol.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6471 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPTemperatureProtocol.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4770 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPThermoElectricProtocol.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPWaveCalProtocol.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8531 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPWifiConfigurationProtocol.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OceanBinaryProtocol.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.039888 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.151887 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/constants/
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/constants/FPGARegisterCodes.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/constants/OpCodes.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.155887 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/
--rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/FPGARegisterReadExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/FPGARegisterWriteExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/FPGASpectrumExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/FlameNIRSpectrumExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/HRFPGASpectrumExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/IntegrationTimeExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/JazSpectrumExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/MayaProSpectrumExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/NIRQuestSpectrumExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/OOI2KSpectrumExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/OOIIrradCalExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5363 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/OOIReadIrradCalExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5049 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/OOIWriteIrradCalExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/QESpectrumExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/ReadEEPROMSlotExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/ReadSpectrumExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/ReadTECQETemperatureExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/ReadTECTemperatureExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/RequestSpectrumExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/StrobeEnableExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/TECEnableExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/TECQEEnableExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/TriggerModeExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/USBFPGASpectrumExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/WriteEEPROMSlotExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/WriteTECQESetPointExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/WriteTECSetPointExchange.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.155887 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/hints/
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/hints/ControlHint.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/hints/SpectrumHint.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.155887 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/impls/
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/impls/FPGARegisterProtocol.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/impls/OOIEEPROMProtocol.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/impls/OOIIrradCalProtocol.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/impls/OOIProtocol.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    10685 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/impls/OOISpectrometerProtocol.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/impls/OOIStrobeLampProtocol.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4319 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/impls/OOITECProtocol.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.159887 seabreeze-2.1.0/src/seabreeze/
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/seabreeze/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/seabreeze/_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-28 10:48:11.000000 seabreeze-2.1.0/src/seabreeze/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/seabreeze/backends.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.159887 seabreeze-2.1.0/src/seabreeze/cseabreeze/
--rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/seabreeze/cseabreeze/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24316 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/seabreeze/cseabreeze/c_seabreeze.pxd
--rw-r--r--   0 runner    (1001) docker     (123)   142956 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/seabreeze/cseabreeze/c_seabreeze_wrapper.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     7815 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/seabreeze/os_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/seabreeze/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.159887 seabreeze-2.1.0/src/seabreeze/pyseabreeze/
--rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/seabreeze/pyseabreeze/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4879 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/seabreeze/pyseabreeze/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/seabreeze/pyseabreeze/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    39264 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/seabreeze/pyseabreeze/devices.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/seabreeze/pyseabreeze/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.163887 seabreeze-2.1.0/src/seabreeze/pyseabreeze/features/
--rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/seabreeze/pyseabreeze/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/seabreeze/pyseabreeze/features/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/seabreeze/pyseabreeze/features/acquisitiondelay.py
--rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/seabreeze/pyseabreeze/features/continuousstrobe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/seabreeze/pyseabreeze/features/databuffer.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/seabreeze/pyseabreeze/features/dhcpserver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/seabreeze/pyseabreeze/features/eeprom.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/seabreeze/pyseabreeze/features/ethernetconfiguration.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/seabreeze/pyseabreeze/features/fastbuffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/seabreeze/pyseabreeze/features/fpga.py
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/seabreeze/pyseabreeze/features/gpio.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/seabreeze/pyseabreeze/features/i2cmaster.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/seabreeze/pyseabreeze/features/introspection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/seabreeze/pyseabreeze/features/ipv4.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/seabreeze/pyseabreeze/features/irradcal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/seabreeze/pyseabreeze/features/lightsource.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/seabreeze/pyseabreeze/features/multicast.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/seabreeze/pyseabreeze/features/networkconfiguration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/seabreeze/pyseabreeze/features/nonlinearity.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/seabreeze/pyseabreeze/features/opticalbench.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/seabreeze/pyseabreeze/features/pixelbinning.py
--rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/seabreeze/pyseabreeze/features/rawusb.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/seabreeze/pyseabreeze/features/revision.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/seabreeze/pyseabreeze/features/shutter.py
--rw-r--r--   0 runner    (1001) docker     (123)    23387 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/seabreeze/pyseabreeze/features/spectrometer.py
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/seabreeze/pyseabreeze/features/spectrumprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/seabreeze/pyseabreeze/features/straylightcoefficients.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/seabreeze/pyseabreeze/features/strobelamp.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/seabreeze/pyseabreeze/features/temperature.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/seabreeze/pyseabreeze/features/thermoelectric.py
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/seabreeze/pyseabreeze/features/wificonfiguration.py
--rw-r--r--   0 runner    (1001) docker     (123)    24310 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/seabreeze/pyseabreeze/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)    11657 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/seabreeze/pyseabreeze/transport.py
--rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/seabreeze/pyseabreeze/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    13623 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/seabreeze/spectrometers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18768 2023-03-28 10:47:35.000000 seabreeze-2.1.0/src/seabreeze/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.159887 seabreeze-2.1.0/src/seabreeze.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-03-28 10:48:11.000000 seabreeze-2.1.0/src/seabreeze.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    84487 2023-03-28 10:48:12.000000 seabreeze-2.1.0/src/seabreeze.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 10:48:11.000000 seabreeze-2.1.0/src/seabreeze.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-03-28 10:48:11.000000 seabreeze-2.1.0/src/seabreeze.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-03-28 10:48:11.000000 seabreeze-2.1.0/src/seabreeze.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-28 10:48:11.000000 seabreeze-2.1.0/src/seabreeze.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 10:48:12.163887 seabreeze-2.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-03-28 10:47:35.000000 seabreeze-2.1.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-03-28 10:47:35.000000 seabreeze-2.1.0/tests/test_backends.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-03-28 10:47:35.000000 seabreeze-2.1.0/tests/test_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)    11725 2023-03-28 10:47:35.000000 seabreeze-2.1.0/tests/test_spectrometers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.259852 seabreeze-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-15 17:57:02.000000 seabreeze-2.2.0/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-15 17:57:02.000000 seabreeze-2.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7579 2023-04-15 17:57:02.000000 seabreeze-2.2.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-04-15 17:57:02.000000 seabreeze-2.2.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-15 17:57:02.000000 seabreeze-2.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-04-15 17:57:29.259852 seabreeze-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6278 2023-04-15 17:57:02.000000 seabreeze-2.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:28.971848 seabreeze-2.2.0/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)    10263 2023-04-15 17:57:02.000000 seabreeze-2.2.0/dev/pretty_print_obp_pcapng.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:28.971848 seabreeze-2.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-15 17:57:02.000000 seabreeze-2.2.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-15 17:57:02.000000 seabreeze-2.2.0/docs/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:28.975848 seabreeze-2.2.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:28.975848 seabreeze-2.2.0/docs/source/_extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-15 17:57:02.000000 seabreeze-2.2.0/docs/source/_extensions/repo_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:28.975848 seabreeze-2.2.0/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    36848 2023-04-15 17:57:02.000000 seabreeze-2.2.0/docs/source/_static/overview.png
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-15 17:57:02.000000 seabreeze-2.2.0/docs/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9624 2023-04-15 17:57:02.000000 seabreeze-2.2.0/docs/source/backend_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6040 2023-04-15 17:57:02.000000 seabreeze-2.2.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10234 2023-04-15 17:57:02.000000 seabreeze-2.2.0/docs/source/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4616 2023-04-15 17:57:02.000000 seabreeze-2.2.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-04-15 17:57:02.000000 seabreeze-2.2.0/docs/source/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-04-15 17:57:02.000000 seabreeze-2.2.0/docs/source/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-15 17:57:02.000000 seabreeze-2.2.0/docs/source/tldr.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-04-15 17:57:02.000000 seabreeze-2.2.0/docs/source/troubleshoot.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:28.975848 seabreeze-2.2.0/os_support/
+-rw-r--r--   0 runner    (1001) docker     (123)     4811 2023-04-15 17:57:02.000000 seabreeze-2.2.0/os_support/10-oceanoptics.rules
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-15 17:57:02.000000 seabreeze-2.2.0/os_support/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)  7255559 2023-04-15 17:57:02.000000 seabreeze-2.2.0/os_support/windows-driver-files.zip
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-04-15 17:57:02.000000 seabreeze-2.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-15 17:57:02.000000 seabreeze-2.2.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-15 17:57:02.000000 seabreeze-2.2.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 17:57:29.259852 seabreeze-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     8039 2023-04-15 17:57:02.000000 seabreeze-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:28.971848 seabreeze-2.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:28.955848 seabreeze-2.2.0/src/libseabreeze/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:28.947848 seabreeze-2.2.0/src/libseabreeze/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:28.987848 seabreeze-2.2.0/src/libseabreeze/include/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/api/DeviceFactory.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/api/USBEndpointTypes.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:28.995849 seabreeze-2.2.0/src/libseabreeze/include/api/seabreezeapi/
+-rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/api/seabreezeapi/AcquisitionDelayFeatureAdapter.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/api/seabreezeapi/ContinuousStrobeFeatureAdapter.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/api/seabreezeapi/DHCPServerFeatureAdapter.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/api/seabreezeapi/DataBufferFeatureAdapter.h
+-rw-r--r--   0 runner    (1001) docker     (123)    28448 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/api/seabreezeapi/DeviceAdapter.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/api/seabreezeapi/EEPROMFeatureAdapter.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/api/seabreezeapi/EthernetConfigurationFeatureAdapter.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/api/seabreezeapi/FastBufferFeatureAdapter.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/api/seabreezeapi/FeatureAdapterInterface.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/api/seabreezeapi/FeatureAdapterTemplate.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9272 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/api/seabreezeapi/FeatureFamilies.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/api/seabreezeapi/I2CMasterFeatureAdapter.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/api/seabreezeapi/IPv4FeatureAdapter.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/api/seabreezeapi/IntrospectionFeatureAdapter.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/api/seabreezeapi/IrradCalFeatureAdapter.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/api/seabreezeapi/LightSourceFeatureAdapter.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/api/seabreezeapi/MulticastFeatureAdapter.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/api/seabreezeapi/NetworkConfigurationFeatureAdapter.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/api/seabreezeapi/NonlinearityCoeffsFeatureAdapter.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/api/seabreezeapi/OpticalBenchFeatureAdapter.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/api/seabreezeapi/PixelBinningFeatureAdapter.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/api/seabreezeapi/ProtocolFamilies.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/api/seabreezeapi/RawUSBBusAccessFeatureAdapter.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/api/seabreezeapi/RevisionFeatureAdapter.h
+-rw-r--r--   0 runner    (1001) docker     (123)    29520 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/api/seabreezeapi/SeaBreezeAPI.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/api/seabreezeapi/SeaBreezeAPIConstants.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26268 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/api/seabreezeapi/SeaBreezeAPI_Impl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/api/seabreezeapi/SerialNumberFeatureAdapter.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/api/seabreezeapi/ShutterFeatureAdapter.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/api/seabreezeapi/SpectrometerFeatureAdapter.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/api/seabreezeapi/SpectrumProcessingFeatureAdapter.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/api/seabreezeapi/StrayLightCoeffsFeatureAdapter.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/api/seabreezeapi/StrobeLampFeatureAdapter.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/api/seabreezeapi/TemperatureFeatureAdapter.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/api/seabreezeapi/ThermoElectricCoolerFeatureAdapter.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/api/seabreezeapi/WifiConfigurationFeatureAdapter.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/api/seabreezeapi/gpioFeatureAdapter.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:28.999848 seabreeze-2.2.0/src/libseabreeze/include/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/common/ByteVector.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/common/Data.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/common/DoubleVector.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/common/FloatVector.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/common/Log.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/common/SeaBreeze.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/common/U32Vector.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/common/UShortVector.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/common/UnitDescriptor.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:28.999848 seabreeze-2.2.0/src/libseabreeze/include/common/buses/
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/common/buses/Bus.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/common/buses/BusFamilies.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/common/buses/BusFamily.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/common/buses/DeviceLocationProberInterface.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/common/buses/DeviceLocatorInterface.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/common/buses/TransferHelper.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:28.999848 seabreeze-2.2.0/src/libseabreeze/include/common/buses/network/
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/common/buses/network/IPv4NetworkProtocol.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/common/buses/network/IPv4SocketDeviceLocator.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/common/buses/network/TCPIPv4SocketBus.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/common/buses/network/TCPIPv4SocketTransferHelper.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:28.999848 seabreeze-2.2.0/src/libseabreeze/include/common/buses/rs232/
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/common/buses/rs232/RS232DeviceLocator.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/common/buses/rs232/RS232Interface.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/common/buses/rs232/RS232TransferHelper.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:28.999848 seabreeze-2.2.0/src/libseabreeze/include/common/buses/usb/
+-rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/common/buses/usb/USBDeviceLocator.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/common/buses/usb/USBInterface.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/common/buses/usb/USBTransferHelper.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.003848 seabreeze-2.2.0/src/libseabreeze/include/common/devices/
+-rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/common/devices/Device.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.003848 seabreeze-2.2.0/src/libseabreeze/include/common/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/common/exceptions/BusConnectException.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/common/exceptions/BusException.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/common/exceptions/BusTransferException.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/common/exceptions/FeatureControlException.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/common/exceptions/FeatureException.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/common/exceptions/FeatureProtocolNotFoundException.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/common/exceptions/IllegalArgumentException.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/common/exceptions/NumberFormatException.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/common/exceptions/ProtocolBusMismatchException.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/common/exceptions/ProtocolException.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/common/exceptions/ProtocolFormatException.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/common/exceptions/ProtocolTransactionException.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.003848 seabreeze-2.2.0/src/libseabreeze/include/common/features/
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/common/features/Feature.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/common/features/FeatureFamily.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/common/features/FeatureImpl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/common/globals.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.007849 seabreeze-2.2.0/src/libseabreeze/include/common/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/common/protocols/Exchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/common/protocols/Protocol.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/common/protocols/ProtocolFamily.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/common/protocols/ProtocolHelper.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/common/protocols/ProtocolHint.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/common/protocols/Transaction.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/common/protocols/Transfer.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:28.947848 seabreeze-2.2.0/src/libseabreeze/include/native/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.007849 seabreeze-2.2.0/src/libseabreeze/include/native/network/
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/native/network/Inet4Address.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/native/network/Socket.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/native/network/SocketException.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/native/network/SocketTimeoutException.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/native/network/UnknownHostException.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.007849 seabreeze-2.2.0/src/libseabreeze/include/native/network/posix/
+-rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/native/network/posix/NativeSocketPOSIX.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.007849 seabreeze-2.2.0/src/libseabreeze/include/native/network/windows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/native/network/windows/NativeSocketWindows.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.007849 seabreeze-2.2.0/src/libseabreeze/include/native/rs232/
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/native/rs232/NativeRS232.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/native/rs232/RS232.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.007849 seabreeze-2.2.0/src/libseabreeze/include/native/rs232/windows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/native/rs232/windows/NativeRS232Windows.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.007849 seabreeze-2.2.0/src/libseabreeze/include/native/system/
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/native/system/NativeSystem.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/native/system/System.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.011849 seabreeze-2.2.0/src/libseabreeze/include/native/usb/
+-rw-r--r--   0 runner    (1001) docker     (123)     8474 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/native/usb/NativeUSB.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/native/usb/USB.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/native/usb/USBDiscovery.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.011849 seabreeze-2.2.0/src/libseabreeze/include/native/usb/winusb/
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/native/usb/winusb/WindowsGUID.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:28.947848 seabreeze-2.2.0/src/libseabreeze/include/vendors/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:28.955848 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:28.947848 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/buses/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.011849 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/buses/network/
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/buses/network/FlameXTCPIPv4.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/buses/network/JazTCPIPv4.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.011849 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/buses/rs232/
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/buses/rs232/OOIRS232Interface.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.015849 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/ApexUSB.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/FlameNIRUSB.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/FlameXUSB.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/FlameXUSBTransferHelper.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/HR2000PlusUSB.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/HR2000USB.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/HR4000USB.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/JazUSB.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/Maya2000ProUSB.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/Maya2000USB.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/MayaLSLUSB.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/NIRQuest256USB.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/NIRQuest512USB.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/OOIUSB4KSpectrumTransferHelper.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/OOIUSBControlTransferHelper.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/OOIUSBEndpointMaps.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/OOIUSBInterface.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/OOIUSBProductID.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/OOIUSBSpectrumTransferHelper.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/OOIUSBTrivialTransferHelper.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/QE65000USB.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/QEProUSB.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/STSUSB.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/SparkUSB.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/TorusUSB.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/USB2000PlusUSB.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/USB2000USB.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/USB4000USB.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/VentanaUSB.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.019849 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/devices/
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/devices/Apex.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/devices/FlameNIR.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/devices/FlameX.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/devices/HR2000.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/devices/HR2000Plus.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/devices/HR4000.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/devices/Jaz.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/devices/Maya2000.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/devices/Maya2000Pro.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/devices/MayaLSL.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/devices/NIRQuest256.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/devices/NIRQuest512.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/devices/QE65000.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/devices/QEPro.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/devices/STS.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/devices/Spark.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/devices/Torus.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/devices/USB2000.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/devices/USB2000Plus.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/devices/USB4000.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/devices/Ventana.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:28.955848 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.023849 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/acquisition_delay/
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/acquisition_delay/AcquisitionDelayFeature.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/acquisition_delay/AcquisitionDelayFeatureInterface.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/acquisition_delay/AcquisitionDelayFeature_FPGA.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/acquisition_delay/STSAcquisitionDelayFeature.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.023849 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/continuous_strobe/
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/continuous_strobe/ContinuousStrobeFeature.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/continuous_strobe/ContinuousStrobeFeatureInterface.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/continuous_strobe/ContinuousStrobeFeature_FPGA.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.023849 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/data_buffer/
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/data_buffer/DataBufferFeatureBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/data_buffer/DataBufferFeatureInterface.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/data_buffer/FlameXDataBufferFeature.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/data_buffer/QEProDataBufferFeature.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.023849 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/dhcp_server/
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/dhcp_server/DHCPServerFeature.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/dhcp_server/DHCPServerFeatureInterface.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.027849 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/EEPROMSlotFeature.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/EEPROMSlotFeatureBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/EEPROMSlotFeatureInterface.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/NonlinearityEEPROMSlotFeature.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/SaturationEEPROMSlotFeature.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/SaturationEEPROMSlotFeatureBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/SaturationEEPROMSlotFeature_MayaPro.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/SaturationEEPROMSlotFeature_NIRQuest.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/SerialNumberEEPROMSlotFeature.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/StrayLightEEPROMSlotFeature.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/WavelengthEEPROMSlotFeature.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/WavelengthEEPROMSlotFeature_QE65000.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.027849 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/ethernet_configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/ethernet_configuration/EthernetConfigurationFeature.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/ethernet_configuration/EthernetConfigurationFeatureInterface.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.027849 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/fast_buffer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/fast_buffer/FastBufferFeatureBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/fast_buffer/FastBufferFeatureInterface.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/fast_buffer/FlameXFastBufferFeature.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.027849 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/fpga_register/
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/fpga_register/FPGARegisterFeature.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/fpga_register/FPGARegisterFeatureInterface.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.027849 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/gpio/
+-rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/gpio/gpioFeature.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/gpio/gpioFeatureInterface.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.027849 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/i2c_master/
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/i2c_master/i2cMasterFeature.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/i2c_master/i2cMasterFeatureInterface.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.027849 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/introspection/
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/introspection/IntrospectionFeature.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/introspection/IntrospectionFeatureInterface.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.027849 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/ipv4/
+-rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/ipv4/IPv4Feature.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/ipv4/IPv4FeatureInterface.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.031849 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/irradcal/
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/irradcal/IrradCalFeature.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/irradcal/IrradCalFeatureInterface.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.031849 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/light_source/
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/light_source/LightSourceFeatureBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/light_source/LightSourceFeatureImpl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/light_source/LightSourceFeatureInterface.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/light_source/StrobeLampFeature.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/light_source/StrobeLampFeatureInterface.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/light_source/VentanaLightSourceFeature.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.031849 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/multicast/
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/multicast/MulticastFeature.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/multicast/MulticastFeatureInterface.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.031849 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/network_configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/network_configuration/NetworkConfigurationFeature.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/network_configuration/NetworkConfigurationFeatureInterface.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.031849 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/nonlinearity/
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/nonlinearity/NonlinearityCoeffsFeature.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/nonlinearity/NonlinearityCoeffsFeatureInterface.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.031849 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/optical_bench/
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/optical_bench/OpticalBenchFeature.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/optical_bench/OpticalBenchFeatureInterface.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.035849 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/pixel_binning/
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/pixel_binning/PixelBinningFeatureInterface.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/pixel_binning/STSPixelBinningFeature.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.035849 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/raw_bus_access/
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/raw_bus_access/RawUSBBusAccessFeature.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/raw_bus_access/RawUSBBusAccessFeatureInterface.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.035849 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/revision/
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/revision/RevisionFeature.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/revision/RevisionFeatureInterface.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.035849 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/serial_number/
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/serial_number/SerialNumberFeature.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/serial_number/SerialNumberFeatureInterface.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.035849 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/shutter/
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/shutter/ShutterFeature.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/shutter/ShutterFeatureInterface.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.039849 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/ApexSpectrometerFeature.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/FlameNIRSpectrometerFeature.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/FlameXSpectrometerFeature.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/GainAdjustedSpectrometerFeature.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/HR2000PlusSpectrometerFeature.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/HR2000SpectrometerFeature.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/HR4000SpectrometerFeature.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/JazSpectrometerFeature.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/Maya2000ProSpectrometerFeature.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/Maya2000SpectrometerFeature.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/MayaLSLSpectrometerFeature.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/NIRQuest256SpectrometerFeature.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/NIRQuest512SpectrometerFeature.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/NIRQuestSpectrometerFeature.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5579 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/OOISpectrometerFeature.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/OOISpectrometerFeatureInterface.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/ProgrammableSaturationFeature.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/ProgrammableSaturationFeatureBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/ProgrammableSaturationFeatureImpl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/ProgrammableSaturationFeatureInterface.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/QE65000SpectrometerFeature.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/QEProSpectrometerFeature.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/STSSpectrometerFeature.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/SparkSpectrometerFeature.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/SpectrometerTriggerMode.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/USB2000PlusSpectrometerFeature.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/USB2000SpectrometerFeature.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/USB4000SpectrometerFeature.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/VentanaSpectrometerFeature.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.043849 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrum_processing/
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrum_processing/SpectrumProcessingFeature.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrum_processing/SpectrumProcessingFeatureInterface.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.043849 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/stray_light/
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/stray_light/StrayLightCoeffsFeature.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/stray_light/StrayLightCoeffsFeatureInterface.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.043849 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/temperature/
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/temperature/TemperatureFeature.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/temperature/TemperatureFeatureInterface.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.043849 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/thermoelectric/
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/thermoelectric/QEProThermoElectricFeature.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/thermoelectric/ThermoElectricFeatureBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/thermoelectric/ThermoElectricFeatureInterface.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/thermoelectric/ThermoElectricQEFeature.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/thermoelectric/VentanaThermoElectricFeature.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.043849 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/wavecal/
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/wavecal/WaveCalFeature.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/wavecal/WaveCalFeatureInterface.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.043849 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/wifi_configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/wifi_configuration/WifiConfigurationFeature.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/wifi_configuration/WifiConfigurationFeatureInterface.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:28.955848 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.051849 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/AcquisitionDelayProtocolInterface.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/ContinuousStrobeProtocolInterface.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/DHCPServerProtocolInterface.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/DataBufferProtocolInterface.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/EEPROMProtocolInterface.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/EthernetConfigurationProtocolInterface.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/FPGARegisterProtocolInterface.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/FastBufferProtocolInterface.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/GPIOProtocolInterface.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/I2CMasterProtocolInterface.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/IPv4ProtocolInterface.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/IntrospectionProtocolInterface.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/IrradCalProtocolInterface.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/LightSourceProtocolInterface.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/MulticastProtocolInterface.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/NetworkConfigurationProtocolInterface.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/NonlinearityCoeffsProtocolInterface.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/OpticalBenchProtocolInterface.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/PixelBinningProtocolInterface.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/ProgrammableSaturationProtocolInterface.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/RevisionProtocolInterface.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/SerialNumberProtocolInterface.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/ShutterProtocolInterface.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/SpectrometerProtocolInterface.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/SpectrumProcessingProtocolInterface.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/StrayLightCoeffsProtocolInterface.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/StrobeLampProtocolInterface.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/TemperatureProtocolInterface.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/ThermoElectricProtocolInterface.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/WaveCalProtocolInterface.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/WifiConfigurationProtocolInterface.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:28.955848 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.051849 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/constants/
+-rw-r--r--   0 runner    (1001) docker     (123)    21778 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/constants/OBPMessageTypes.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.075849 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPAddIPv4AddressExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPCommand.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPContinuousStrobeEnableExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPContinuousStrobePeriodExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPDataBufferClearExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPDataBufferRemoveOldestExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPDeleteIPv4AddressExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetActivePixelRangesExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetAllTemperaturesExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetBoxcarWidthExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetConsecutiveSampleCountExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDHCPServerAddressExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDHCPServerEnableExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDataBufferCapacityExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDataBufferElementCountExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDataBufferMaximumCapacityExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDefaultPixelBinningExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetElectricDarkPixelRangesExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetEthernetConfigurationGbEEnableExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetEthernetConfigurationMACAddressExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetFastBufferingEnableExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetFirmwareRevisionExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOExtensionAvailableModesExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOExtensionCurrentModeExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOExtensionNumberOfPinsExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOExtensionOutputVectorExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOExtensionValueExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIONumberOfPinsExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOOutputEnableVectorExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOValueVectorExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetHardwareRevisionExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetI2CMasterNumberOfBusesExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIPv4AddressExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIPv4DHCPEnableStateExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIPv4DefaultGatewayExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIPv4NumberOfAddressesExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIrradCalExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIrradCollectionAreaExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetMaxPixelBinningExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetMulticastEnableExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNetworkInterfaceConnectionTypeExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNetworkInterfaceEnableStateExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNonlinearityCoeffExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNonlinearityCoeffsCountExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNumberOfNetworkInterfacesExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNumberOfPixelsExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchCoatingExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchFiberDiameterMicronsExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchFilterExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchGratingExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchIDExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchSerialNumberExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchSlitWidthMicronsExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalDarkPixelRangesExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetPixelBinningExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetSaturationExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetScansToAverageExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetSerialNumberExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetSerialNumberMaximumLengthExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetStrayLightCoeffExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetStrayLightCoeffsCountExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetTemperatureCountExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetTemperatureExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetThermoElectricTemperatureExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetWaveCalExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetWifiConfigurationModeExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetWifiConfigurationSSIDExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetWifiConfigurationSecurityExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPIntegrationTimeExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPLampEnableCommand.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPLightSourceEnableCommand.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPLightSourceEnabledQuery.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPLightSourceIntensityCommand.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPLightSourceIntensityQuery.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPMessage.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPQuery.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPReadI2CMasterBusExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPReadNumberOfRawSpectraWithMetadataExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPReadRawSpectrum32AndMetadataExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPReadRawSpectrumExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPReadSpectrum32AndMetadataExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPReadSpectrumExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPReadSpectrumWithGainExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPRequestBufferedSpectrum32AndMetadataExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPRequestNumberOfBufferedSpectraWithMetadataExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPRequestRawSpectrumExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPRequestSpectrumExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPRunNetworkInterfaceSelfTestExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSaveNetworkInterfaceConnectionSettingsExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetAcquisitionDelayExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetBoxcarWidthExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetConsecutiveSampleCountExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetDHCPServerAddressExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetDHCPServerEnableExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetDataBufferCapacityExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetDefaultPixelBinningExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetEthernetConfigurationGbEEnableExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetEthernetConfigurationMACAddressExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetFastBufferingEnableExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetGPIOExtensionModeExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetGPIOExtensionOutputVectorExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetGPIOExtensionValueExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetGPIOExtensionVectorExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetGPIOOutputEnableVectorExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetGPIOValueVectorExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetIPv4DHCPEnableStateExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetIPv4DefaultGatewayExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetIrradCalExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetIrradCollectionAreaExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetMulticastEnableExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetNetworkInterfaceEnableStateExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetPixelBinningExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetScansToAverageExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetThermoElectricEnableExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetThermoElectricSetpointExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetWifiConfigurationModeExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetWifiConfigurationPassPhraseExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetWifiConfigurationSSIDExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetWifiConfigurationSecurityExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPShutterExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPTransaction.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPTriggerModeExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPWriteI2CMasterBusExchange.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.075849 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/hints/
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/hints/OBPControlHint.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/hints/OBPSpectrumHint.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.083850 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPAcquisitionDelayProtocol.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPContinuousStrobeProtocol.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPDHCPServerProtocol.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPDataBufferProtocol.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPEthernetConfigurationProtocol.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPFastBufferProtocol.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPGPIOProtocol.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPI2CMasterProtocol.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPIPv4Protocol.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPIntrospectionProtocol.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPIrradCalProtocol.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPLightSourceProtocol.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPLightSourceProtocol_Ventana.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPMulticastProtocol.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPNetworkConfigurationProtocol.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPNonlinearityCoeffsProtocol.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPOpticalBenchProtocol.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPPixelBinningProtocol.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPProgrammableSaturationProtocol.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPRevisionProtocol.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPSerialNumberProtocol.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPShutterProtocol.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPSpectrometerProtocol.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPSpectrumProcessingProtocol.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPStrayLightCoeffsProtocol.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPStrobeLampProtocol.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPTemperatureProtocol.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPThermoElectricProtocol.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPWaveCalProtocol.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPWifiConfigurationProtocol.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OceanBinaryProtocol.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:28.955848 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.083850 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/constants/
+-rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/constants/FPGARegisterCodes.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/constants/OpCodes.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/constants/QETECConstants.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.087849 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/FPGARegisterReadExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/FPGARegisterWriteExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/FPGASpectrumExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/FlameNIRSpectrumExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/HRFPGASpectrumExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/IntegrationTimeExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/JazSpectrumExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/MayaProSpectrumExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/NIRQuestSpectrumExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/OOI2KSpectrumExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/OOIIrradCalExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/OOIReadIrradCalExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/OOIWriteIrradCalExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/QESpectrumExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/ReadEEPROMSlotExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/ReadSpectrumExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/ReadTECQETemperatureExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/ReadTECTemperatureExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/RequestSpectrumExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/StrobeEnableExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/TECEnableExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/TECQEEnableExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/TriggerModeExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/USBFPGASpectrumExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/WriteEEPROMSlotExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/WriteTECQESetPointExchange.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/WriteTECSetPointExchange.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.087849 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/hints/
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/hints/ControlHint.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/hints/SpectrumHint.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.091850 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/impls/
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/impls/FPGARegisterProtocol.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/impls/OOIEEPROMProtocol.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/impls/OOIIrradCalProtocol.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/impls/OOIProtocol.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/impls/OOISpectrometerProtocol.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/impls/OOIStrobeLampProtocol.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/impls/OOITECProtocol.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.091850 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/utils/Polynomial.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:28.959848 seabreeze-2.2.0/src/libseabreeze/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.091850 seabreeze-2.2.0/src/libseabreeze/src/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     6249 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/api/DeviceFactory.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.099850 seabreeze-2.2.0/src/libseabreeze/src/api/seabreezeapi/
+-rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/api/seabreezeapi/AcquisitionDelayFeatureAdapter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/api/seabreezeapi/ContinuousStrobeFeatureAdapter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/api/seabreezeapi/DHCPServerFeatureAdapter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/api/seabreezeapi/DataBufferFeatureAdapter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    80076 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/api/seabreezeapi/DeviceAdapter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/api/seabreezeapi/EEPROMFeatureAdapter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4306 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/api/seabreezeapi/EthernetConfigurationFeatureAdapter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/api/seabreezeapi/FastBufferFeatureAdapter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12485 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/api/seabreezeapi/FeatureFamilies.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/api/seabreezeapi/I2CMasterFeatureAdapter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6106 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/api/seabreezeapi/IPv4FeatureAdapter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5019 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/api/seabreezeapi/IntrospectionFeatureAdapter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/api/seabreezeapi/IrradCalFeatureAdapter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/api/seabreezeapi/LightSourceFeatureAdapter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/api/seabreezeapi/MulticastFeatureAdapter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4770 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/api/seabreezeapi/NetworkConfigurationFeatureAdapter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/api/seabreezeapi/NonlinearityCoeffsFeatureAdapter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7338 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/api/seabreezeapi/OpticalBenchFeatureAdapter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/api/seabreezeapi/PixelBinningFeatureAdapter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/api/seabreezeapi/ProtocolFamilies.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4371 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/api/seabreezeapi/RawUSBBusAccessFeatureAdapter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/api/seabreezeapi/RevisionFeatureAdapter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/api/seabreezeapi/SeaBreezeAPI.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    87831 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/api/seabreezeapi/SeaBreezeAPI_Impl.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/api/seabreezeapi/SerialNumberFeatureAdapter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/api/seabreezeapi/ShutterFeatureAdapter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12647 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/api/seabreezeapi/SpectrometerFeatureAdapter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4445 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/api/seabreezeapi/SpectrumProcessingFeatureAdapter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/api/seabreezeapi/StrayLightCoeffsFeatureAdapter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/api/seabreezeapi/StrobeLampFeatureAdapter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/api/seabreezeapi/TemperatureFeatureAdapter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/api/seabreezeapi/ThermoElectricCoolerFeatureAdapter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5946 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/api/seabreezeapi/WifiConfigurationFeatureAdapter.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6995 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/api/seabreezeapi/gpioFeatureAdapter.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.099850 seabreeze-2.2.0/src/libseabreeze/src/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/common/ByteVector.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/common/Data.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/common/DoubleVector.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/common/FloatVector.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6490 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/common/Log.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/common/U32Vector.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/common/UShortVector.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/common/UnitDescriptor.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.099850 seabreeze-2.2.0/src/libseabreeze/src/common/buses/
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/common/buses/Bus.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/common/buses/BusFamilies.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/common/buses/BusFamily.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/common/buses/DeviceLocationProberInterface.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/common/buses/TransferHelper.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.103850 seabreeze-2.2.0/src/libseabreeze/src/common/buses/network/
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/common/buses/network/IPv4NetworkProtocol.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/common/buses/network/IPv4SocketDeviceLocator.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/common/buses/network/TCPIPv4SocketBus.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/common/buses/network/TCPIPv4SocketTransferHelper.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.103850 seabreeze-2.2.0/src/libseabreeze/src/common/buses/rs232/
+-rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/common/buses/rs232/RS232DeviceLocator.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/common/buses/rs232/RS232Interface.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/common/buses/rs232/RS232TransferHelper.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.103850 seabreeze-2.2.0/src/libseabreeze/src/common/buses/usb/
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/common/buses/usb/USBDeviceLocator.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/common/buses/usb/USBInterface.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/common/buses/usb/USBTransferHelper.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.103850 seabreeze-2.2.0/src/libseabreeze/src/common/devices/
+-rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/common/devices/Device.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.107850 seabreeze-2.2.0/src/libseabreeze/src/common/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/common/exceptions/BusConnectException.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/common/exceptions/BusException.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/common/exceptions/BusTransferException.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/common/exceptions/FeatureControlException.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/common/exceptions/FeatureException.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/common/exceptions/FeatureProtocolNotFoundException.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/common/exceptions/IllegalArgumentException.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/common/exceptions/NumberFormatException.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/common/exceptions/ProtocolBusMismatchException.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/common/exceptions/ProtocolException.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/common/exceptions/ProtocolFormatException.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/common/exceptions/ProtocolTransactionException.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.111850 seabreeze-2.2.0/src/libseabreeze/src/common/features/
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/common/features/FeatureFamily.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/common/features/FeatureImpl.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.111850 seabreeze-2.2.0/src/libseabreeze/src/common/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/common/protocols/Exchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/common/protocols/Protocol.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/common/protocols/ProtocolFamily.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/common/protocols/ProtocolHelper.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/common/protocols/ProtocolHint.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/common/protocols/Transaction.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/common/protocols/Transfer.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:28.959848 seabreeze-2.2.0/src/libseabreeze/src/native/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.115850 seabreeze-2.2.0/src/libseabreeze/src/native/network/
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/native/network/Inet4Address.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/native/network/SocketException.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/native/network/SocketTimeoutException.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/native/network/UnknownHostException.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.115850 seabreeze-2.2.0/src/libseabreeze/src/native/network/posix/
+-rw-r--r--   0 runner    (1001) docker     (123)     7271 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/native/network/posix/NativeSocketPOSIX.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.115850 seabreeze-2.2.0/src/libseabreeze/src/native/network/windows/
+-rw-r--r--   0 runner    (1001) docker     (123)     7149 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/native/network/windows/NativeSocketWindows.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.115850 seabreeze-2.2.0/src/libseabreeze/src/native/rs232/
+-rw-r--r--   0 runner    (1001) docker     (123)     6555 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/native/rs232/RS232.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.115850 seabreeze-2.2.0/src/libseabreeze/src/native/rs232/posix/
+-rw-r--r--   0 runner    (1001) docker     (123)    12360 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/native/rs232/posix/NativeRS232POSIX.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.115850 seabreeze-2.2.0/src/libseabreeze/src/native/rs232/windows/
+-rw-r--r--   0 runner    (1001) docker     (123)     7796 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/native/rs232/windows/NativeRS232Windows.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.115850 seabreeze-2.2.0/src/libseabreeze/src/native/system/
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/native/system/System.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.115850 seabreeze-2.2.0/src/libseabreeze/src/native/system/posix/
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/native/system/posix/NativeSystemPOSIX.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.115850 seabreeze-2.2.0/src/libseabreeze/src/native/system/windows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/native/system/windows/NativeSystemWindows.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.115850 seabreeze-2.2.0/src/libseabreeze/src/native/usb/
+-rw-r--r--   0 runner    (1001) docker     (123)     9909 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/native/usb/USB.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/native/usb/USBDiscovery.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.115850 seabreeze-2.2.0/src/libseabreeze/src/native/usb/linux/
+-rw-r--r--   0 runner    (1001) docker     (123)    22561 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/native/usb/linux/NativeUSBLinux.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.115850 seabreeze-2.2.0/src/libseabreeze/src/native/usb/osx/
+-rw-r--r--   0 runner    (1001) docker     (123)    38021 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/native/usb/osx/NativeUSBMacOSX.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.115850 seabreeze-2.2.0/src/libseabreeze/src/native/usb/winusb/
+-rw-r--r--   0 runner    (1001) docker     (123)    28911 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/native/usb/winusb/NativeUSBWinUSB.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:28.959848 seabreeze-2.2.0/src/libseabreeze/src/vendors/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:28.967848 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:28.963848 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/buses/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.119850 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/buses/network/
+-rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/buses/network/FlameXTCPIPv4.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/buses/network/JazTCPIPv4.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.119850 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/buses/rs232/
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/buses/rs232/OOIRS232Interface.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.123850 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/ApexUSB.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/FlameNIRUSB.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/FlameXUSB.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/FlameXUSBTransferHelper.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/HR2000PlusUSB.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/HR2000USB.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/HR4000USB.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/JazUSB.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/Maya2000ProUSB.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/Maya2000USB.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/MayaLSLUSB.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/NIRQuest256USB.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/NIRQuest512USB.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/OOIUSB4KSpectrumTransferHelper.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/OOIUSBControlTransferHelper.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/OOIUSBEndpointMaps.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5452 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/OOIUSBInterface.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/OOIUSBSpectrumTransferHelper.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/OOIUSBTrivialTransferHelper.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/QE65000USB.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/QEProUSB.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/STSUSB.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/SparkUSB.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/TorusUSB.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/USB2000PlusUSB.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/USB2000USB.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/USB4000USB.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/VentanaUSB.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.131850 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/devices/
+-rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/devices/Apex.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/devices/FlameNIR.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9704 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/devices/FlameX.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/devices/HR2000.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/devices/HR2000Plus.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/devices/HR4000.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/devices/Jaz.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4951 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/devices/Maya2000.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/devices/Maya2000Pro.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4799 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/devices/MayaLSL.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/devices/NIRQuest256.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/devices/NIRQuest512.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5081 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/devices/QE65000.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6351 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/devices/QEPro.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8466 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/devices/STS.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7144 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/devices/Spark.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/devices/Torus.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/devices/USB2000.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5072 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/devices/USB2000Plus.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4797 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/devices/USB4000.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7724 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/devices/Ventana.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:28.967848 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.131850 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/acquisition_delay/
+-rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/acquisition_delay/AcquisitionDelayFeature.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5221 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/acquisition_delay/AcquisitionDelayFeature_FPGA.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/acquisition_delay/STSAcquisitionDelayFeature.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.131850 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/continuous_strobe/
+-rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/continuous_strobe/ContinuousStrobeFeature.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/continuous_strobe/ContinuousStrobeFeature_FPGA.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.131850 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/data_buffer/
+-rw-r--r--   0 runner    (1001) docker     (123)    10049 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/data_buffer/DataBufferFeatureBase.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/data_buffer/FlameXDataBufferFeature.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/data_buffer/QEProDataBufferFeature.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.131850 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/dhcp_server/
+-rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/dhcp_server/DHCPServerFeature.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.135850 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/
+-rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/EEPROMSlotFeature.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6938 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/EEPROMSlotFeatureBase.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/NonlinearityEEPROMSlotFeature.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/SaturationEEPROMSlotFeature.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/SaturationEEPROMSlotFeatureBase.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/SaturationEEPROMSlotFeature_MayaPro.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/SaturationEEPROMSlotFeature_NIRQuest.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/SerialNumberEEPROMSlotFeature.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/StrayLightEEPROMSlotFeature.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3774 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/WavelengthEEPROMSlotFeature.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/WavelengthEEPROMSlotFeature_QE65000.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.135850 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/ethernet_configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)     6763 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/ethernet_configuration/EthernetConfigurationFeature.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.135850 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/fast_buffer/
+-rw-r--r--   0 runner    (1001) docker     (123)     6310 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/fast_buffer/FastBufferFeatureBase.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/fast_buffer/FlameXFastBufferFeature.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.135850 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/fpga_register/
+-rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/fpga_register/FPGARegisterFeature.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.135850 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/gpio/
+-rw-r--r--   0 runner    (1001) docker     (123)    13793 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/gpio/gpioFeature.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.135850 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/i2c_master/
+-rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/i2c_master/i2cFeature.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.135850 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/introspection/
+-rw-r--r--   0 runner    (1001) docker     (123)     6646 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/introspection/IntrospectionFeature.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.135850 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/ipv4/
+-rw-r--r--   0 runner    (1001) docker     (123)     9822 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/ipv4/IPv4Feature.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.135850 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/irradcal/
+-rw-r--r--   0 runner    (1001) docker     (123)     6711 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/irradcal/IrradCalFeature.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.135850 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/light_source/
+-rw-r--r--   0 runner    (1001) docker     (123)    14844 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/light_source/LightSourceFeatureBase.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/light_source/LightSourceFeatureImpl.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/light_source/StrobeLampFeature.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/light_source/VentanaLightSourceFeature.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.139850 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/multicast/
+-rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/multicast/MulticastFeature.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.139850 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/network_configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)     8675 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/network_configuration/NetworkConfigurationFeature.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.139850 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/nonlinearity/
+-rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/nonlinearity/NonlinearityCoeffsFeature.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.139850 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/optical_bench/
+-rw-r--r--   0 runner    (1001) docker     (123)     9817 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/optical_bench/OpticalBenchFeature.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.139850 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/pixel_binning/
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/pixel_binning/PixelBinningFeatureInterface.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9620 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/pixel_binning/STSPixelBinningFeature.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.139850 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/raw_bus_access/
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/raw_bus_access/RawUSBBusAccessFeature.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.139850 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/revision/
+-rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/revision/RevisionFeature.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.139850 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/serial_number/
+-rw-r--r--   0 runner    (1001) docker     (123)     4465 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/serial_number/SerialNumberFeature.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.139850 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/shutter/
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/shutter/ShutterFeature.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.151850 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/
+-rw-r--r--   0 runner    (1001) docker     (123)     4708 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/ApexSpectrometerFeature.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/FlameNIRSpectrometerFeature.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7869 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/FlameXSpectrometerFeature.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/GainAdjustedSpectrometerFeature.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/HR2000PlusSpectrometerFeature.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4348 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/HR2000SpectrometerFeature.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4390 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/HR4000SpectrometerFeature.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/JazSpectrometerFeature.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/Maya2000ProSpectrometerFeature.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4465 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/Maya2000SpectrometerFeature.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/MayaLSLSpectrometerFeature.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/NIRQuest256SpectrometerFeature.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/NIRQuest512SpectrometerFeature.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/NIRQuestSpectrometerFeature.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14571 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/OOISpectrometerFeature.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/ProgrammableSaturationFeature.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/ProgrammableSaturationFeatureBase.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/ProgrammableSaturationFeatureImpl.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/QE65000SpectrometerFeature.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/QEProSpectrometerFeature.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5874 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/STSSpectrometerFeature.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/SparkSpectrometerFeature.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/SpectrometerTriggerMode.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4713 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/USB2000PlusSpectrometerFeature.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/USB2000SpectrometerFeature.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/USB4000SpectrometerFeature.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/VentanaSpectrometerFeature.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.151850 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrum_processing/
+-rw-r--r--   0 runner    (1001) docker     (123)     6867 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrum_processing/SpectrumProcessingFeature.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.151850 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/stray_light/
+-rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/stray_light/StrayLightCoeffsFeature.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.151850 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/temperature/
+-rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/temperature/TemperatureFeature.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.151850 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/thermoelectric/
+-rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/thermoelectric/QEProThermoElectricFeature.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/thermoelectric/ThermoElectricFeatureBase.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/thermoelectric/ThermoElectricQEFeature.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/thermoelectric/VentanaThermoElectricFeature.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.151850 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/wavecal/
+-rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/wavecal/WaveCalFeature.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.155851 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/wifi_configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)     9640 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/wifi_configuration/WifiConfigurationFeature.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:28.967848 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.167851 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/AcquisitionDelayProtocolInterface.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/ContinuousStrobeProtocolInterface.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/DHCPServerProtocolInterface.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/DataBufferProtocolInterface.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/EEPROMProtocolInterface.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/EthernetConfigurationProtocolInterface.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/FPGARegisterProtocolInterface.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/FastBufferProtocolInterface.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/GPIOProtocolInterface.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/I2CMasterProtocolInterface.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/IPv4ProtocolInterface.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/IntrospectionProtocolInterface.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/IrradCalProtocolInterface.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/LightSourceProtocolInterface.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/MulticastProtocolInterface.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/NetworkConfigurationProtocolInterface.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/NonlinearityCoeffsProtocolInterface.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/OpticalBenchProtocolInteface.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/PixelBinningProtocolInterface.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/ProgrammableSaturationProtocolInteface.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/RevisionProtocolInteface.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/SerialNumberProtocolInterface.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/ShutterProtocolInterface.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/SpectrometerProtocolInterface.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/SpectrumProcessingProtocolInteface.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/StrayLightCoeffsProtocolInterface.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/StrobeLampProtocolInterface.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/TemperatureProtocolInteface.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/ThermoElectricProtocolInterface.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/WaveCalProtocolInterface.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/WifiConfigurationProtocolInterface.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:28.967848 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.215851 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPAddIPv4AddressExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPCommand.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPContinuousStrobeEnableExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPContinuousStrobePeriodExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPDataBufferClearExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPDataBufferRemoveOldestExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPDeleteIPv4AddressExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetActivePixelRangesExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetAllTemperaturesExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetBoxcarWidthExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetConsecutiveSampleCountExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDHCPServerAddressExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDHCPServerEnableExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDataBufferCapacityExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDataBufferCountExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDataBufferMaximumCapacityExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDefaultPixelBinningExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetElectricDarkPixelRangesExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetEthernetConfigurationGbEEnableExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetEthernetConfigurationMACAddressExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetFastBufferingEnableExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetFirmwareRevisionExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOExtensionAvailableModesExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOExtensionCurrentModeExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOExtensionNumberOfPinsExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOExtensionOutputVectorExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOExtensionValueExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIONumberOfPinsExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOOutputEnableVectorExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOValueVectorExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetHardwareRevisionExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetI2CMasterNumberOfBusesExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIPv4AddressExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIPv4DHCPEnableStateExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIPv4DefaultGatewayExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIPv4NumberOfAddressesExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIrradCalExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIrradCollectionAreaExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetMaxPixelBinningExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetMulticastEnableExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNetworkInterfaceConnectionTypeExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNetworkInterfaceEnableStateExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNonlinearityCoeffExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNonlinearityCoeffsCountExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNumberOfNetworkInterfacesExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNumberOfPixelsExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchCoatingExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchFiberDiameterMicronsExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchFilterExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchGratingExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchIDExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchSerialNumberExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchSlitWidthMicronsExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalDarkPixelRangesExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetPixelBinningExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetSaturationExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetScansToAverageExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetSerialNumberExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetSerialNumberMaximumLengthExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetStrayLightCoeffExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetStrayLightCoeffsCountExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetTemperatureCountExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetTemperatureExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetThermoElectricTemperatureExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetWaveCalExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetWifiConfigurationModeExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetWifiConfigurationSSIDExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetWifiConfigurationSecurityExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPIntegrationTimeExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPLampEnableCommand.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPLightSourceEnableCommand.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPLightSourceEnabledQuery.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPLightSourceIntensityCommand.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPLightSourceIntensityQuery.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12839 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPMessage.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPQuery.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPReadI2CMasterBusExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5658 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPReadNumberOfRawSpectraWithMetadataExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5017 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPReadRawSpectrum32AndMetadataExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4616 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPReadRawSpectrumExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPReadSpectrum32AndMetadataExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPReadSpectrumExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPReadSpectrumWithGainExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPRequestBufferedSpectrum32AndMetadata.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPRequestNumberOfBufferedSpectraWithMetadata.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPRequestRawSpectrumExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPRequestSpectrumExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPRunNetworkInterfaceSelfTestExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSaveNetworkInterfaceConnectionSettingsExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetAcquisitionDelayExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetBoxcarWidthExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetConsecutiveSampleCountExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetDHCPServerAddressExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetDHCPServerEnableExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetDataBufferCapacityExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetDefaultPixelBinningFactorExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetEthernetConfigurationGbEEnableExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetEthernetConfigurationMACAddressExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetFastBufferingEnableExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetGPIOExtensionModeExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetGPIOExtensionOutputVectorExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetGPIOExtensionValueExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetGPIOOutputEnableVectorExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetGPIOValueVectorExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetIPv4DHCPEnableStateExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetIPv4DefaultGatewayExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetIrradCalExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetIrradCollectionAreaExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetMulticastEnableExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetNetworkInterfaceEnableStateExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetPixelBinningExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetScansToAverageExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetThermoElectricEnableExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetThermoElectricSetpointExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetWifiConfigurationModeExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetWifiConfigurationPassPhraseExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetWifiConfigurationSSIDExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetWifiConfigurationSecurityExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPShutterExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10484 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPTransaction.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPTriggerModeExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPWriteI2CMasterBusExchange.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.215851 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/hints/
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/hints/OBPControlHint.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/hints/OBPSpectrumHint.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.227851 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/
+-rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPAcquisitionDelayProtocol.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPContinuousStrobeProtocol.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6070 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPDHCPServerProtocol.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9129 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPDataBufferProtocol.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPEthernetConfigurationProtocol.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPFastBufferProtocol.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    13773 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPGPIOProtocol.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5371 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPI2CMasterProtocol.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9506 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPIPv4Protocol.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPIntrospectionProtocol.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6699 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPIrradCalProtocol.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPLightSourceProtocol.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPLightSourceProtocol_Ventana.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5637 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPMulticastProtocol.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7815 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPNetworkConfigurationProtocol.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPNonlinearityCoeffsProtocol.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11491 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPOpticalBenchProtocol.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPPixelBinningProtocol.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPProgrammableSaturationProtocol.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPRevisionProtocol.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPSerialNumberProtocol.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPShutterProtocol.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12416 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPSpectrometerProtocol.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5673 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPSpectrumProcessingProtocol.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPStrayLightCoeffsProtocol.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPStrobeLampProtocol.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6471 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPTemperatureProtocol.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4770 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPThermoElectricProtocol.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPWaveCalProtocol.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8531 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPWifiConfigurationProtocol.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OceanBinaryProtocol.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:28.971848 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.227851 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/constants/
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/constants/FPGARegisterCodes.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/constants/OpCodes.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.235851 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/FPGARegisterReadExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/FPGARegisterWriteExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/FPGASpectrumExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/FlameNIRSpectrumExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/HRFPGASpectrumExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/IntegrationTimeExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/JazSpectrumExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/MayaProSpectrumExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/NIRQuestSpectrumExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/OOI2KSpectrumExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/OOIIrradCalExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5363 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/OOIReadIrradCalExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5049 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/OOIWriteIrradCalExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/QESpectrumExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/ReadEEPROMSlotExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/ReadSpectrumExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/ReadTECQETemperatureExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/ReadTECTemperatureExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/RequestSpectrumExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/StrobeEnableExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/TECEnableExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/TECQEEnableExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/TriggerModeExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/USBFPGASpectrumExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/WriteEEPROMSlotExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/WriteTECQESetPointExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/WriteTECSetPointExchange.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.235851 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/hints/
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/hints/ControlHint.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/hints/SpectrumHint.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.239852 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/impls/
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/impls/FPGARegisterProtocol.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/impls/OOIEEPROMProtocol.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/impls/OOIIrradCalProtocol.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/impls/OOIProtocol.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10685 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/impls/OOISpectrometerProtocol.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/impls/OOIStrobeLampProtocol.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4319 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/impls/OOITECProtocol.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.243852 seabreeze-2.2.0/src/seabreeze/
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/seabreeze/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/seabreeze/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-15 17:57:28.000000 seabreeze-2.2.0/src/seabreeze/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/seabreeze/backends.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.247852 seabreeze-2.2.0/src/seabreeze/cseabreeze/
+-rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/seabreeze/cseabreeze/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24316 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/seabreeze/cseabreeze/c_seabreeze.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)   142956 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/seabreeze/cseabreeze/c_seabreeze_wrapper.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     7815 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/seabreeze/os_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/seabreeze/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.247852 seabreeze-2.2.0/src/seabreeze/pyseabreeze/
+-rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/seabreeze/pyseabreeze/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4879 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/seabreeze/pyseabreeze/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/seabreeze/pyseabreeze/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40797 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/seabreeze/pyseabreeze/devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/seabreeze/pyseabreeze/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.259852 seabreeze-2.2.0/src/seabreeze/pyseabreeze/features/
+-rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/seabreeze/pyseabreeze/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/seabreeze/pyseabreeze/features/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/seabreeze/pyseabreeze/features/acquisitiondelay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/seabreeze/pyseabreeze/features/continuousstrobe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/seabreeze/pyseabreeze/features/databuffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/seabreeze/pyseabreeze/features/dhcpserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/seabreeze/pyseabreeze/features/eeprom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/seabreeze/pyseabreeze/features/ethernetconfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/seabreeze/pyseabreeze/features/fastbuffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/seabreeze/pyseabreeze/features/fpga.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/seabreeze/pyseabreeze/features/gpio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/seabreeze/pyseabreeze/features/i2cmaster.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/seabreeze/pyseabreeze/features/introspection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/seabreeze/pyseabreeze/features/ipv4.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/seabreeze/pyseabreeze/features/irradcal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/seabreeze/pyseabreeze/features/lightsource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/seabreeze/pyseabreeze/features/multicast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/seabreeze/pyseabreeze/features/networkconfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/seabreeze/pyseabreeze/features/nonlinearity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/seabreeze/pyseabreeze/features/opticalbench.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/seabreeze/pyseabreeze/features/pixelbinning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/seabreeze/pyseabreeze/features/rawusb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/seabreeze/pyseabreeze/features/revision.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/seabreeze/pyseabreeze/features/shutter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25320 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/seabreeze/pyseabreeze/features/spectrometer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/seabreeze/pyseabreeze/features/spectrumprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/seabreeze/pyseabreeze/features/straylightcoefficients.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/seabreeze/pyseabreeze/features/strobelamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/seabreeze/pyseabreeze/features/temperature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/seabreeze/pyseabreeze/features/thermoelectric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/seabreeze/pyseabreeze/features/wificonfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25063 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/seabreeze/pyseabreeze/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12211 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/seabreeze/pyseabreeze/transport.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/seabreeze/pyseabreeze/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13623 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/seabreeze/spectrometers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18768 2023-04-15 17:57:02.000000 seabreeze-2.2.0/src/seabreeze/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.243852 seabreeze-2.2.0/src/seabreeze.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-04-15 17:57:28.000000 seabreeze-2.2.0/src/seabreeze.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    84518 2023-04-15 17:57:28.000000 seabreeze-2.2.0/src/seabreeze.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 17:57:28.000000 seabreeze-2.2.0/src/seabreeze.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-15 17:57:28.000000 seabreeze-2.2.0/src/seabreeze.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-15 17:57:28.000000 seabreeze-2.2.0/src/seabreeze.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-15 17:57:28.000000 seabreeze-2.2.0/src/seabreeze.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:57:29.259852 seabreeze-2.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-04-15 17:57:02.000000 seabreeze-2.2.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-04-15 17:57:02.000000 seabreeze-2.2.0/tests/test_backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-15 17:57:02.000000 seabreeze-2.2.0/tests/test_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11725 2023-04-15 17:57:02.000000 seabreeze-2.2.0/tests/test_spectrometers.py
```

### Comparing `seabreeze-2.1.0/.pre-commit-config.yaml` & `seabreeze-2.2.0/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     rev: v4.4.0
     hooks:
     -   id: trailing-whitespace
     -   id: end-of-file-fixer
     -   id: check-yaml
     -   id: check-added-large-files
 -   repo: https://github.com/psf/black
-    rev: '23.1.0'
+    rev: '23.3.0'
     hooks:
     -   id: black
         language_version: python3
 -   repo: https://github.com/pycqa/isort
     rev: 5.12.0
     hooks:
     -   id: isort
@@ -24,15 +24,15 @@
     hooks:
     -   id: flake8
         additional_dependencies:
         -    flake8-typing-imports==1.14.0
         language_version: python3
         exclude: "^(build|docs|tests|setup.py)"
 -   repo: https://github.com/pre-commit/mirrors-mypy
-    rev: 'v1.1.1'
+    rev: 'v1.2.0'
     hooks:
     -   id: mypy
         additional_dependencies: [numpy<1.22, pyusb>=1.0]
         exclude: "^(build|docs|tests|setup.py)"
 -   repo: https://github.com/asottile/pyupgrade
     rev: v3.3.1
     hooks:
```

### Comparing `seabreeze-2.1.0/CHANGELOG.md` & `seabreeze-2.2.0/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,19 @@
 | *psb*  | refers to `seabreeze.pyseabreeze`   |
 | *spec* | refers to `seabreeze.spectrometers` |
 
 
 ## [Unreleased]
 ...
 
+## [2.2.0] - 2023-04-15
+### Added
+- *repo* build aarch64 and osx arm64 wheels
+- *psb* basic support for SR4 spectrometers
+
 ## [2.1.0] - 2023-03-28
 ### Added
 - *psb* allow configuration of OBP protocol version checks
 - *psb* EXPERIMENTAL support for ADC1000-USB
 
 ### Fixed
 - *repo* multiple pre-commit updates
@@ -186,15 +191,17 @@
 ## [0.5.3] - 2016-02-16
 ### Added
 - oldest version I'll go back to in this changelog
 
 ### Changed
 - Don't require numpy during build of cseabreeze cython extension
 
-[Unreleased]: https://github.com/ap--/python-seabreeze/compare/v2.0.3...HEAD
+[Unreleased]: https://github.com/ap--/python-seabreeze/compare/v2.2.0...HEAD
+[2.2.0]: https://github.com/ap--/python-seabreeze/compare/v2.1.0...v2.2.0
+[2.1.0]: https://github.com/ap--/python-seabreeze/compare/v2.0.3...v2.1.0
 [2.0.3]: https://github.com/ap--/python-seabreeze/compare/v2.0.2...v2.0.3
 [2.0.2]: https://github.com/ap--/python-seabreeze/compare/v2.0.1...v2.0.2
 [2.0.1]: https://github.com/ap--/python-seabreeze/compare/v2.0.0...v2.0.1
 [2.0.0]: https://github.com/ap--/python-seabreeze/compare/v1.3.0...v2.0.0
 [1.3.0]: https://github.com/ap--/python-seabreeze/compare/v1.2.0...v1.3.0
 [1.2.0]: https://github.com/ap--/python-seabreeze/compare/v1.1.0...v1.2.0
 [1.1.0]: https://github.com/ap--/python-seabreeze/compare/v1.0.2...v1.1.0
```

### Comparing `seabreeze-2.1.0/LICENSE.md` & `seabreeze-2.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/PKG-INFO` & `seabreeze-2.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seabreeze
-Version: 2.1.0
+Version: 2.2.0
 Summary: Python interface module for Ocean Optics spectrometers. This software is not associated with Ocean Optics. Use it at your own risk.
 Home-page: https://github.com/ap--/python-seabreeze
 Author: Andreas Poehlmann
 Author-email: andreas@poehlmann.io
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `seabreeze-2.1.0/README.md` & `seabreeze-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/docs/Makefile` & `seabreeze-2.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/docs/source/_extensions/repo_file.py` & `seabreeze-2.2.0/docs/source/_extensions/repo_file.py`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/docs/source/_static/overview.png` & `seabreeze-2.2.0/docs/source/_static/overview.png`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/docs/source/api.rst` & `seabreeze-2.2.0/docs/source/api.rst`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/docs/source/backend_api.rst` & `seabreeze-2.2.0/docs/source/backend_api.rst`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/docs/source/conf.py` & `seabreeze-2.2.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/docs/source/contributing.rst` & `seabreeze-2.2.0/docs/source/contributing.rst`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/docs/source/index.rst` & `seabreeze-2.2.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/docs/source/install.rst` & `seabreeze-2.2.0/docs/source/install.rst`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/docs/source/quickstart.rst` & `seabreeze-2.2.0/docs/source/quickstart.rst`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/docs/source/tldr.rst` & `seabreeze-2.2.0/docs/source/tldr.rst`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/docs/source/troubleshoot.rst` & `seabreeze-2.2.0/docs/source/troubleshoot.rst`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/os_support/10-oceanoptics.rules` & `seabreeze-2.2.0/os_support/10-oceanoptics.rules`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 # udev rules file for Ocean Optics, Inc. spectrometers
 # ====================================================
 #
-# version: 2.3
-# updated: 2020-08-09
+# version: 2.4
+# updated: 2023-04-15
 # maintainer: Andreas Poehlmann <andreas@poehlmann.io>
 #
 # [info] Previous versions are missing this header.
 #
 # Ships with [python-seabreeze](https://github.com/ap--/python-seabreeze/)
 # Only USB spectrometers are supported. When using the newest version (1.0+)
 # of python-seabreeze you can install the rules via running:
 #
 #   $ seabreeze_os_setup
 #
 # Changes:
+# - [2.4] added support for SR4 spectrometer
 # - added support for HDX spectrometer
 # - added support for QE-PRO class of OceanOptics spectrometers
 # - set MODE instead of group (Fedora doesn't use `plugdev`)
 # - match parent SUBSYSTEMS for compatibility with older udev versions
 # - match both actions 'add' and 'bind' (fixes https://github.com/systemd/systemd/issues/8221)
 # - do not allow overriding MODE setting (fixes https://github.com/ap--/python-seabreeze/issues/78)
 #
@@ -80,9 +81,11 @@
 ATTR{idVendor}=="0547", ATTR{idProduct}=="2131", SYMLINK+="ezUSB-%n", MODE:="0666"
 # unprogrammed EzUSB-FX
 ATTR{idVendor}=="0547", ATTR{idProduct}=="2235", SYMLINK+="ezUSB-FX-%n", MODE:="0666"
 # unprogrammed EzUSB-FX2
 ATTR{idVendor}=="04b4", ATTR{idProduct}=="8613", SYMLINK+="ezUSB-FX2-%n", MODE:="0666"
 # Ocean Insight Inc. HDX spectrometer
 ATTR{idVendor}=="2457", ATTR{idProduct}=="2003", SYMLINK+="oceanhdx-%n", MODE:="0666"
+# Ocean Insight Inc. SR4 spectrometer
+ATTR{idVendor}=="0999", ATTR{idProduct}=="1002", SYMLINK+="sr4-%n", MODE:="0666"
 
 LABEL="oceanoptics_rules_end"
```

### Comparing `seabreeze-2.1.0/os_support/readme.md` & `seabreeze-2.2.0/os_support/readme.md`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/os_support/windows-driver-files.zip` & `seabreeze-2.2.0/os_support/windows-driver-files.zip`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/pyproject.toml` & `seabreeze-2.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/setup.py` & `seabreeze-2.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/api/DeviceFactory.h` & `seabreeze-2.2.0/src/libseabreeze/include/api/DeviceFactory.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/api/USBEndpointTypes.h` & `seabreeze-2.2.0/src/libseabreeze/include/api/USBEndpointTypes.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/api/seabreezeapi/AcquisitionDelayFeatureAdapter.h` & `seabreeze-2.2.0/src/libseabreeze/include/api/seabreezeapi/AcquisitionDelayFeatureAdapter.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/api/seabreezeapi/ContinuousStrobeFeatureAdapter.h` & `seabreeze-2.2.0/src/libseabreeze/include/api/seabreezeapi/ContinuousStrobeFeatureAdapter.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/api/seabreezeapi/DHCPServerFeatureAdapter.h` & `seabreeze-2.2.0/src/libseabreeze/include/api/seabreezeapi/DHCPServerFeatureAdapter.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/api/seabreezeapi/DataBufferFeatureAdapter.h` & `seabreeze-2.2.0/src/libseabreeze/include/api/seabreezeapi/DataBufferFeatureAdapter.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/api/seabreezeapi/DeviceAdapter.h` & `seabreeze-2.2.0/src/libseabreeze/include/api/seabreezeapi/DeviceAdapter.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/api/seabreezeapi/EEPROMFeatureAdapter.h` & `seabreeze-2.2.0/src/libseabreeze/include/api/seabreezeapi/EEPROMFeatureAdapter.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/api/seabreezeapi/EthernetConfigurationFeatureAdapter.h` & `seabreeze-2.2.0/src/libseabreeze/include/api/seabreezeapi/EthernetConfigurationFeatureAdapter.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/api/seabreezeapi/FastBufferFeatureAdapter.h` & `seabreeze-2.2.0/src/libseabreeze/include/api/seabreezeapi/FastBufferFeatureAdapter.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/api/seabreezeapi/FeatureAdapterInterface.h` & `seabreeze-2.2.0/src/libseabreeze/include/api/seabreezeapi/FeatureAdapterInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/api/seabreezeapi/FeatureAdapterTemplate.h` & `seabreeze-2.2.0/src/libseabreeze/include/api/seabreezeapi/FeatureAdapterTemplate.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/api/seabreezeapi/FeatureFamilies.h` & `seabreeze-2.2.0/src/libseabreeze/include/api/seabreezeapi/FeatureFamilies.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/api/seabreezeapi/I2CMasterFeatureAdapter.h` & `seabreeze-2.2.0/src/libseabreeze/include/api/seabreezeapi/I2CMasterFeatureAdapter.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/api/seabreezeapi/IPv4FeatureAdapter.h` & `seabreeze-2.2.0/src/libseabreeze/include/api/seabreezeapi/IPv4FeatureAdapter.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/api/seabreezeapi/IntrospectionFeatureAdapter.h` & `seabreeze-2.2.0/src/libseabreeze/include/api/seabreezeapi/IntrospectionFeatureAdapter.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/api/seabreezeapi/IrradCalFeatureAdapter.h` & `seabreeze-2.2.0/src/libseabreeze/include/api/seabreezeapi/IrradCalFeatureAdapter.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/api/seabreezeapi/LightSourceFeatureAdapter.h` & `seabreeze-2.2.0/src/libseabreeze/include/api/seabreezeapi/LightSourceFeatureAdapter.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/api/seabreezeapi/MulticastFeatureAdapter.h` & `seabreeze-2.2.0/src/libseabreeze/include/api/seabreezeapi/MulticastFeatureAdapter.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/api/seabreezeapi/NetworkConfigurationFeatureAdapter.h` & `seabreeze-2.2.0/src/libseabreeze/include/api/seabreezeapi/NetworkConfigurationFeatureAdapter.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/api/seabreezeapi/NonlinearityCoeffsFeatureAdapter.h` & `seabreeze-2.2.0/src/libseabreeze/include/api/seabreezeapi/NonlinearityCoeffsFeatureAdapter.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/api/seabreezeapi/OpticalBenchFeatureAdapter.h` & `seabreeze-2.2.0/src/libseabreeze/include/api/seabreezeapi/OpticalBenchFeatureAdapter.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/api/seabreezeapi/PixelBinningFeatureAdapter.h` & `seabreeze-2.2.0/src/libseabreeze/include/api/seabreezeapi/PixelBinningFeatureAdapter.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/api/seabreezeapi/ProtocolFamilies.h` & `seabreeze-2.2.0/src/libseabreeze/include/api/seabreezeapi/ProtocolFamilies.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/api/seabreezeapi/RawUSBBusAccessFeatureAdapter.h` & `seabreeze-2.2.0/src/libseabreeze/include/api/seabreezeapi/RawUSBBusAccessFeatureAdapter.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/api/seabreezeapi/RevisionFeatureAdapter.h` & `seabreeze-2.2.0/src/libseabreeze/include/api/seabreezeapi/RevisionFeatureAdapter.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/api/seabreezeapi/SeaBreezeAPI.h` & `seabreeze-2.2.0/src/libseabreeze/include/api/seabreezeapi/SeaBreezeAPI.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/api/seabreezeapi/SeaBreezeAPIConstants.h` & `seabreeze-2.2.0/src/libseabreeze/include/api/seabreezeapi/SeaBreezeAPIConstants.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/api/seabreezeapi/SeaBreezeAPI_Impl.h` & `seabreeze-2.2.0/src/libseabreeze/include/api/seabreezeapi/SeaBreezeAPI_Impl.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/api/seabreezeapi/SerialNumberFeatureAdapter.h` & `seabreeze-2.2.0/src/libseabreeze/include/api/seabreezeapi/SerialNumberFeatureAdapter.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/api/seabreezeapi/ShutterFeatureAdapter.h` & `seabreeze-2.2.0/src/libseabreeze/include/api/seabreezeapi/ShutterFeatureAdapter.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/api/seabreezeapi/SpectrometerFeatureAdapter.h` & `seabreeze-2.2.0/src/libseabreeze/include/api/seabreezeapi/SpectrometerFeatureAdapter.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/api/seabreezeapi/SpectrumProcessingFeatureAdapter.h` & `seabreeze-2.2.0/src/libseabreeze/include/api/seabreezeapi/SpectrumProcessingFeatureAdapter.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/api/seabreezeapi/StrayLightCoeffsFeatureAdapter.h` & `seabreeze-2.2.0/src/libseabreeze/include/api/seabreezeapi/StrayLightCoeffsFeatureAdapter.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/api/seabreezeapi/StrobeLampFeatureAdapter.h` & `seabreeze-2.2.0/src/libseabreeze/include/api/seabreezeapi/StrobeLampFeatureAdapter.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/api/seabreezeapi/TemperatureFeatureAdapter.h` & `seabreeze-2.2.0/src/libseabreeze/include/api/seabreezeapi/TemperatureFeatureAdapter.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/api/seabreezeapi/ThermoElectricCoolerFeatureAdapter.h` & `seabreeze-2.2.0/src/libseabreeze/include/api/seabreezeapi/ThermoElectricCoolerFeatureAdapter.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/api/seabreezeapi/WifiConfigurationFeatureAdapter.h` & `seabreeze-2.2.0/src/libseabreeze/include/api/seabreezeapi/WifiConfigurationFeatureAdapter.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/api/seabreezeapi/gpioFeatureAdapter.h` & `seabreeze-2.2.0/src/libseabreeze/include/api/seabreezeapi/gpioFeatureAdapter.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/common/ByteVector.h` & `seabreeze-2.2.0/src/libseabreeze/include/common/ByteVector.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/common/Data.h` & `seabreeze-2.2.0/src/libseabreeze/include/common/Data.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/common/DoubleVector.h` & `seabreeze-2.2.0/src/libseabreeze/include/common/DoubleVector.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/common/FloatVector.h` & `seabreeze-2.2.0/src/libseabreeze/include/common/FloatVector.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/common/Log.h` & `seabreeze-2.2.0/src/libseabreeze/include/common/Log.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/common/SeaBreeze.h` & `seabreeze-2.2.0/src/libseabreeze/include/common/SeaBreeze.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/common/U32Vector.h` & `seabreeze-2.2.0/src/libseabreeze/include/common/U32Vector.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/common/UShortVector.h` & `seabreeze-2.2.0/src/libseabreeze/include/common/UShortVector.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/common/UnitDescriptor.h` & `seabreeze-2.2.0/src/libseabreeze/include/common/UnitDescriptor.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/common/buses/Bus.h` & `seabreeze-2.2.0/src/libseabreeze/include/common/buses/Bus.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/common/buses/BusFamilies.h` & `seabreeze-2.2.0/src/libseabreeze/include/common/buses/BusFamilies.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/common/buses/BusFamily.h` & `seabreeze-2.2.0/src/libseabreeze/include/common/buses/BusFamily.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/common/buses/DeviceLocationProberInterface.h` & `seabreeze-2.2.0/src/libseabreeze/include/common/buses/DeviceLocationProberInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/common/buses/DeviceLocatorInterface.h` & `seabreeze-2.2.0/src/libseabreeze/include/common/buses/DeviceLocatorInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/common/buses/TransferHelper.h` & `seabreeze-2.2.0/src/libseabreeze/include/common/buses/TransferHelper.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/common/buses/network/IPv4NetworkProtocol.h` & `seabreeze-2.2.0/src/libseabreeze/include/common/buses/network/IPv4NetworkProtocol.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/common/buses/network/IPv4SocketDeviceLocator.h` & `seabreeze-2.2.0/src/libseabreeze/include/common/buses/network/IPv4SocketDeviceLocator.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/common/buses/network/TCPIPv4SocketBus.h` & `seabreeze-2.2.0/src/libseabreeze/include/common/buses/network/TCPIPv4SocketBus.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/common/buses/network/TCPIPv4SocketTransferHelper.h` & `seabreeze-2.2.0/src/libseabreeze/include/common/buses/network/TCPIPv4SocketTransferHelper.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/common/buses/rs232/RS232DeviceLocator.h` & `seabreeze-2.2.0/src/libseabreeze/include/common/buses/rs232/RS232DeviceLocator.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/common/buses/rs232/RS232Interface.h` & `seabreeze-2.2.0/src/libseabreeze/include/common/buses/rs232/RS232Interface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/common/buses/rs232/RS232TransferHelper.h` & `seabreeze-2.2.0/src/libseabreeze/include/common/buses/rs232/RS232TransferHelper.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/common/buses/usb/USBDeviceLocator.h` & `seabreeze-2.2.0/src/libseabreeze/include/common/buses/usb/USBDeviceLocator.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/common/buses/usb/USBInterface.h` & `seabreeze-2.2.0/src/libseabreeze/include/common/buses/usb/USBInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/common/buses/usb/USBTransferHelper.h` & `seabreeze-2.2.0/src/libseabreeze/include/common/buses/usb/USBTransferHelper.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/common/devices/Device.h` & `seabreeze-2.2.0/src/libseabreeze/include/common/devices/Device.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/common/exceptions/BusConnectException.h` & `seabreeze-2.2.0/src/libseabreeze/include/common/exceptions/BusConnectException.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/common/exceptions/BusException.h` & `seabreeze-2.2.0/src/libseabreeze/include/common/exceptions/BusException.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/common/exceptions/BusTransferException.h` & `seabreeze-2.2.0/src/libseabreeze/include/common/exceptions/BusTransferException.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/common/exceptions/FeatureControlException.h` & `seabreeze-2.2.0/src/libseabreeze/include/common/exceptions/FeatureControlException.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/common/exceptions/FeatureException.h` & `seabreeze-2.2.0/src/libseabreeze/include/common/exceptions/FeatureException.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/common/exceptions/FeatureProtocolNotFoundException.h` & `seabreeze-2.2.0/src/libseabreeze/include/common/exceptions/FeatureProtocolNotFoundException.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/common/exceptions/IllegalArgumentException.h` & `seabreeze-2.2.0/src/libseabreeze/include/common/exceptions/IllegalArgumentException.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/common/exceptions/NumberFormatException.h` & `seabreeze-2.2.0/src/libseabreeze/include/common/exceptions/NumberFormatException.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/common/exceptions/ProtocolBusMismatchException.h` & `seabreeze-2.2.0/src/libseabreeze/include/common/exceptions/ProtocolBusMismatchException.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/common/exceptions/ProtocolException.h` & `seabreeze-2.2.0/src/libseabreeze/include/common/exceptions/ProtocolException.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/common/exceptions/ProtocolFormatException.h` & `seabreeze-2.2.0/src/libseabreeze/include/common/exceptions/ProtocolFormatException.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/common/exceptions/ProtocolTransactionException.h` & `seabreeze-2.2.0/src/libseabreeze/include/common/exceptions/ProtocolTransactionException.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/common/features/Feature.h` & `seabreeze-2.2.0/src/libseabreeze/include/common/features/Feature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/common/features/FeatureFamily.h` & `seabreeze-2.2.0/src/libseabreeze/include/common/features/FeatureFamily.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/common/features/FeatureImpl.h` & `seabreeze-2.2.0/src/libseabreeze/include/common/features/FeatureImpl.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/common/globals.h` & `seabreeze-2.2.0/src/libseabreeze/include/common/globals.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/common/protocols/Exchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/common/protocols/Exchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/common/protocols/Protocol.h` & `seabreeze-2.2.0/src/libseabreeze/include/common/protocols/Protocol.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/common/protocols/ProtocolFamily.h` & `seabreeze-2.2.0/src/libseabreeze/include/common/protocols/ProtocolFamily.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/common/protocols/ProtocolHelper.h` & `seabreeze-2.2.0/src/libseabreeze/include/common/protocols/ProtocolHelper.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/common/protocols/ProtocolHint.h` & `seabreeze-2.2.0/src/libseabreeze/include/common/protocols/ProtocolHint.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/common/protocols/Transaction.h` & `seabreeze-2.2.0/src/libseabreeze/include/common/protocols/Transaction.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/common/protocols/Transfer.h` & `seabreeze-2.2.0/src/libseabreeze/include/common/protocols/Transfer.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/native/network/Inet4Address.h` & `seabreeze-2.2.0/src/libseabreeze/include/native/network/Inet4Address.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/native/network/Socket.h` & `seabreeze-2.2.0/src/libseabreeze/include/native/network/Socket.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/native/network/SocketException.h` & `seabreeze-2.2.0/src/libseabreeze/include/native/network/SocketException.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/native/network/SocketTimeoutException.h` & `seabreeze-2.2.0/src/libseabreeze/include/native/network/SocketTimeoutException.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/native/network/UnknownHostException.h` & `seabreeze-2.2.0/src/libseabreeze/include/native/network/UnknownHostException.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/native/network/posix/NativeSocketPOSIX.h` & `seabreeze-2.2.0/src/libseabreeze/include/native/network/posix/NativeSocketPOSIX.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/native/network/windows/NativeSocketWindows.h` & `seabreeze-2.2.0/src/libseabreeze/include/native/network/windows/NativeSocketWindows.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/native/rs232/NativeRS232.h` & `seabreeze-2.2.0/src/libseabreeze/include/native/rs232/NativeRS232.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/native/rs232/RS232.h` & `seabreeze-2.2.0/src/libseabreeze/include/native/rs232/RS232.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/native/rs232/windows/NativeRS232Windows.h` & `seabreeze-2.2.0/src/libseabreeze/include/native/rs232/windows/NativeRS232Windows.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/native/system/NativeSystem.h` & `seabreeze-2.2.0/src/libseabreeze/include/native/system/NativeSystem.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/native/system/System.h` & `seabreeze-2.2.0/src/libseabreeze/include/native/system/System.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/native/usb/NativeUSB.h` & `seabreeze-2.2.0/src/libseabreeze/include/native/usb/NativeUSB.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/native/usb/USB.h` & `seabreeze-2.2.0/src/libseabreeze/include/native/usb/USB.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/native/usb/USBDiscovery.h` & `seabreeze-2.2.0/src/libseabreeze/include/native/usb/USBDiscovery.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/native/usb/winusb/WindowsGUID.h` & `seabreeze-2.2.0/src/libseabreeze/include/native/usb/winusb/WindowsGUID.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/buses/network/FlameXTCPIPv4.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/buses/network/FlameXTCPIPv4.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/buses/network/JazTCPIPv4.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/buses/network/JazTCPIPv4.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/buses/rs232/OOIRS232Interface.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/buses/rs232/OOIRS232Interface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/ApexUSB.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/ApexUSB.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/FlameNIRUSB.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/FlameNIRUSB.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/FlameXUSB.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/FlameXUSB.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/FlameXUSBTransferHelper.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/FlameXUSBTransferHelper.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/HR2000PlusUSB.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/HR2000PlusUSB.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/HR2000USB.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/HR2000USB.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/HR4000USB.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/HR4000USB.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/JazUSB.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/JazUSB.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/Maya2000ProUSB.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/Maya2000ProUSB.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/Maya2000USB.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/Maya2000USB.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/MayaLSLUSB.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/MayaLSLUSB.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/NIRQuest256USB.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/NIRQuest256USB.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/NIRQuest512USB.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/NIRQuest512USB.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/OOIUSB4KSpectrumTransferHelper.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/OOIUSB4KSpectrumTransferHelper.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/OOIUSBControlTransferHelper.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/OOIUSBControlTransferHelper.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/OOIUSBEndpointMaps.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/OOIUSBEndpointMaps.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/OOIUSBInterface.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/OOIUSBInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/OOIUSBProductID.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/OOIUSBProductID.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/OOIUSBSpectrumTransferHelper.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/OOIUSBSpectrumTransferHelper.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/OOIUSBTrivialTransferHelper.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/OOIUSBTrivialTransferHelper.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/QE65000USB.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/QE65000USB.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/QEProUSB.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/QEProUSB.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/STSUSB.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/STSUSB.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/SparkUSB.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/SparkUSB.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/TorusUSB.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/TorusUSB.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/USB2000PlusUSB.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/USB2000PlusUSB.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/USB2000USB.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/USB2000USB.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/USB4000USB.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/USB4000USB.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/VentanaUSB.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/VentanaUSB.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/devices/Apex.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/devices/Apex.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/devices/FlameNIR.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/devices/FlameNIR.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/devices/FlameX.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/devices/FlameX.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/devices/HR2000.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/devices/HR2000.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/devices/HR2000Plus.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/devices/HR2000Plus.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/devices/HR4000.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/devices/HR4000.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/devices/Jaz.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/devices/Jaz.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/devices/Maya2000.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/devices/Maya2000.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/devices/Maya2000Pro.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/devices/Maya2000Pro.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/devices/MayaLSL.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/devices/MayaLSL.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/devices/NIRQuest256.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/devices/NIRQuest256.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/devices/NIRQuest512.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/devices/NIRQuest512.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/devices/QE65000.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/devices/QE65000.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/devices/QEPro.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/devices/QEPro.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/devices/STS.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/devices/STS.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/devices/Spark.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/devices/Spark.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/devices/Torus.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/devices/Torus.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/devices/USB2000.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/devices/USB2000.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/devices/USB2000Plus.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/devices/USB2000Plus.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/devices/USB4000.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/devices/USB4000.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/devices/Ventana.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/devices/Ventana.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/acquisition_delay/AcquisitionDelayFeature.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/acquisition_delay/AcquisitionDelayFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/acquisition_delay/AcquisitionDelayFeatureInterface.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/acquisition_delay/AcquisitionDelayFeatureInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/acquisition_delay/AcquisitionDelayFeature_FPGA.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/acquisition_delay/AcquisitionDelayFeature_FPGA.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/acquisition_delay/STSAcquisitionDelayFeature.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/acquisition_delay/STSAcquisitionDelayFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/continuous_strobe/ContinuousStrobeFeature.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/continuous_strobe/ContinuousStrobeFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/continuous_strobe/ContinuousStrobeFeatureInterface.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/continuous_strobe/ContinuousStrobeFeatureInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/continuous_strobe/ContinuousStrobeFeature_FPGA.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/continuous_strobe/ContinuousStrobeFeature_FPGA.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/data_buffer/DataBufferFeatureBase.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/data_buffer/DataBufferFeatureBase.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/data_buffer/DataBufferFeatureInterface.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/data_buffer/DataBufferFeatureInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/data_buffer/FlameXDataBufferFeature.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/data_buffer/FlameXDataBufferFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/data_buffer/QEProDataBufferFeature.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/data_buffer/QEProDataBufferFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/dhcp_server/DHCPServerFeature.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/dhcp_server/DHCPServerFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/dhcp_server/DHCPServerFeatureInterface.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/dhcp_server/DHCPServerFeatureInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/EEPROMSlotFeature.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/EEPROMSlotFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/EEPROMSlotFeatureBase.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/EEPROMSlotFeatureBase.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/EEPROMSlotFeatureInterface.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/EEPROMSlotFeatureInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/NonlinearityEEPROMSlotFeature.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/NonlinearityEEPROMSlotFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/SaturationEEPROMSlotFeature.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/SaturationEEPROMSlotFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/SaturationEEPROMSlotFeatureBase.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/SaturationEEPROMSlotFeatureBase.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/SaturationEEPROMSlotFeature_MayaPro.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/SaturationEEPROMSlotFeature_MayaPro.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/SaturationEEPROMSlotFeature_NIRQuest.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/SaturationEEPROMSlotFeature_NIRQuest.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/SerialNumberEEPROMSlotFeature.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/SerialNumberEEPROMSlotFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/StrayLightEEPROMSlotFeature.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/StrayLightEEPROMSlotFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/WavelengthEEPROMSlotFeature.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/WavelengthEEPROMSlotFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/WavelengthEEPROMSlotFeature_QE65000.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/WavelengthEEPROMSlotFeature_QE65000.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/ethernet_configuration/EthernetConfigurationFeature.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/ethernet_configuration/EthernetConfigurationFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/ethernet_configuration/EthernetConfigurationFeatureInterface.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/ethernet_configuration/EthernetConfigurationFeatureInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/fast_buffer/FastBufferFeatureBase.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/fast_buffer/FastBufferFeatureBase.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/fast_buffer/FastBufferFeatureInterface.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/fast_buffer/FastBufferFeatureInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/fast_buffer/FlameXFastBufferFeature.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/fast_buffer/FlameXFastBufferFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/fpga_register/FPGARegisterFeature.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/fpga_register/FPGARegisterFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/fpga_register/FPGARegisterFeatureInterface.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/fpga_register/FPGARegisterFeatureInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/gpio/gpioFeature.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/gpio/gpioFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/gpio/gpioFeatureInterface.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/gpio/gpioFeatureInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/i2c_master/i2cMasterFeature.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/i2c_master/i2cMasterFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/i2c_master/i2cMasterFeatureInterface.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/i2c_master/i2cMasterFeatureInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/introspection/IntrospectionFeature.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/introspection/IntrospectionFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/introspection/IntrospectionFeatureInterface.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/introspection/IntrospectionFeatureInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/ipv4/IPv4Feature.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/ipv4/IPv4Feature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/ipv4/IPv4FeatureInterface.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/ipv4/IPv4FeatureInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/irradcal/IrradCalFeature.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/irradcal/IrradCalFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/irradcal/IrradCalFeatureInterface.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/irradcal/IrradCalFeatureInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/light_source/LightSourceFeatureBase.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/light_source/LightSourceFeatureBase.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/light_source/LightSourceFeatureImpl.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/light_source/LightSourceFeatureImpl.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/light_source/LightSourceFeatureInterface.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/light_source/LightSourceFeatureInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/light_source/StrobeLampFeature.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/light_source/StrobeLampFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/light_source/StrobeLampFeatureInterface.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/light_source/StrobeLampFeatureInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/light_source/VentanaLightSourceFeature.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/light_source/VentanaLightSourceFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/multicast/MulticastFeature.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/multicast/MulticastFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/multicast/MulticastFeatureInterface.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/multicast/MulticastFeatureInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/network_configuration/NetworkConfigurationFeature.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/network_configuration/NetworkConfigurationFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/network_configuration/NetworkConfigurationFeatureInterface.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/network_configuration/NetworkConfigurationFeatureInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/nonlinearity/NonlinearityCoeffsFeature.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/nonlinearity/NonlinearityCoeffsFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/nonlinearity/NonlinearityCoeffsFeatureInterface.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/nonlinearity/NonlinearityCoeffsFeatureInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/optical_bench/OpticalBenchFeature.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/optical_bench/OpticalBenchFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/optical_bench/OpticalBenchFeatureInterface.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/optical_bench/OpticalBenchFeatureInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/pixel_binning/PixelBinningFeatureInterface.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/pixel_binning/PixelBinningFeatureInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/pixel_binning/STSPixelBinningFeature.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/pixel_binning/STSPixelBinningFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/raw_bus_access/RawUSBBusAccessFeature.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/raw_bus_access/RawUSBBusAccessFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/raw_bus_access/RawUSBBusAccessFeatureInterface.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/raw_bus_access/RawUSBBusAccessFeatureInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/revision/RevisionFeature.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/revision/RevisionFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/revision/RevisionFeatureInterface.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/revision/RevisionFeatureInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/serial_number/SerialNumberFeature.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/serial_number/SerialNumberFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/serial_number/SerialNumberFeatureInterface.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/serial_number/SerialNumberFeatureInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/shutter/ShutterFeature.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/shutter/ShutterFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/shutter/ShutterFeatureInterface.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/shutter/ShutterFeatureInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/ApexSpectrometerFeature.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/ApexSpectrometerFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/FlameNIRSpectrometerFeature.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/FlameNIRSpectrometerFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/FlameXSpectrometerFeature.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/FlameXSpectrometerFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/GainAdjustedSpectrometerFeature.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/GainAdjustedSpectrometerFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/HR2000PlusSpectrometerFeature.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/HR2000PlusSpectrometerFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/HR2000SpectrometerFeature.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/HR2000SpectrometerFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/HR4000SpectrometerFeature.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/HR4000SpectrometerFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/JazSpectrometerFeature.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/JazSpectrometerFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/Maya2000ProSpectrometerFeature.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/Maya2000ProSpectrometerFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/Maya2000SpectrometerFeature.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/Maya2000SpectrometerFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/MayaLSLSpectrometerFeature.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/MayaLSLSpectrometerFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/NIRQuest256SpectrometerFeature.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/NIRQuest256SpectrometerFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/NIRQuest512SpectrometerFeature.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/NIRQuest512SpectrometerFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/NIRQuestSpectrometerFeature.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/NIRQuestSpectrometerFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/OOISpectrometerFeature.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/OOISpectrometerFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/OOISpectrometerFeatureInterface.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/OOISpectrometerFeatureInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/ProgrammableSaturationFeature.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/ProgrammableSaturationFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/ProgrammableSaturationFeatureBase.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/ProgrammableSaturationFeatureBase.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/ProgrammableSaturationFeatureImpl.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/ProgrammableSaturationFeatureImpl.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/ProgrammableSaturationFeatureInterface.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/ProgrammableSaturationFeatureInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/QE65000SpectrometerFeature.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/QE65000SpectrometerFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/QEProSpectrometerFeature.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/QEProSpectrometerFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/STSSpectrometerFeature.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/STSSpectrometerFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/SparkSpectrometerFeature.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/SparkSpectrometerFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/SpectrometerTriggerMode.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/SpectrometerTriggerMode.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/USB2000PlusSpectrometerFeature.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/USB2000PlusSpectrometerFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/USB2000SpectrometerFeature.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/USB2000SpectrometerFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/USB4000SpectrometerFeature.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/USB4000SpectrometerFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/VentanaSpectrometerFeature.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/VentanaSpectrometerFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrum_processing/SpectrumProcessingFeature.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrum_processing/SpectrumProcessingFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrum_processing/SpectrumProcessingFeatureInterface.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrum_processing/SpectrumProcessingFeatureInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/stray_light/StrayLightCoeffsFeature.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/stray_light/StrayLightCoeffsFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/stray_light/StrayLightCoeffsFeatureInterface.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/stray_light/StrayLightCoeffsFeatureInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/temperature/TemperatureFeature.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/temperature/TemperatureFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/temperature/TemperatureFeatureInterface.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/temperature/TemperatureFeatureInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/thermoelectric/QEProThermoElectricFeature.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/thermoelectric/QEProThermoElectricFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/thermoelectric/ThermoElectricFeatureBase.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/thermoelectric/ThermoElectricFeatureBase.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/thermoelectric/ThermoElectricFeatureInterface.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/thermoelectric/ThermoElectricFeatureInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/thermoelectric/ThermoElectricQEFeature.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/thermoelectric/ThermoElectricQEFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/thermoelectric/VentanaThermoElectricFeature.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/thermoelectric/VentanaThermoElectricFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/wavecal/WaveCalFeature.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/wavecal/WaveCalFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/wavecal/WaveCalFeatureInterface.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/wavecal/WaveCalFeatureInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/wifi_configuration/WifiConfigurationFeature.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/wifi_configuration/WifiConfigurationFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/features/wifi_configuration/WifiConfigurationFeatureInterface.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/features/wifi_configuration/WifiConfigurationFeatureInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/AcquisitionDelayProtocolInterface.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/AcquisitionDelayProtocolInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/ContinuousStrobeProtocolInterface.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/ContinuousStrobeProtocolInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/DHCPServerProtocolInterface.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/DHCPServerProtocolInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/DataBufferProtocolInterface.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/DataBufferProtocolInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/EEPROMProtocolInterface.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/EEPROMProtocolInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/EthernetConfigurationProtocolInterface.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/EthernetConfigurationProtocolInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/FPGARegisterProtocolInterface.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/FPGARegisterProtocolInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/FastBufferProtocolInterface.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/FastBufferProtocolInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/GPIOProtocolInterface.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/GPIOProtocolInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/I2CMasterProtocolInterface.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/I2CMasterProtocolInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/IPv4ProtocolInterface.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/IPv4ProtocolInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/IntrospectionProtocolInterface.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/IntrospectionProtocolInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/IrradCalProtocolInterface.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/IrradCalProtocolInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/LightSourceProtocolInterface.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/LightSourceProtocolInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/MulticastProtocolInterface.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/MulticastProtocolInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/NetworkConfigurationProtocolInterface.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/NetworkConfigurationProtocolInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/NonlinearityCoeffsProtocolInterface.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/NonlinearityCoeffsProtocolInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/OpticalBenchProtocolInterface.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/OpticalBenchProtocolInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/PixelBinningProtocolInterface.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/PixelBinningProtocolInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/ProgrammableSaturationProtocolInterface.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/ProgrammableSaturationProtocolInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/RevisionProtocolInterface.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/RevisionProtocolInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/SerialNumberProtocolInterface.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/SerialNumberProtocolInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/ShutterProtocolInterface.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/ShutterProtocolInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/SpectrometerProtocolInterface.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/SpectrometerProtocolInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/SpectrumProcessingProtocolInterface.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/SpectrumProcessingProtocolInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/StrayLightCoeffsProtocolInterface.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/StrayLightCoeffsProtocolInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/StrobeLampProtocolInterface.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/StrobeLampProtocolInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/TemperatureProtocolInterface.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/TemperatureProtocolInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/ThermoElectricProtocolInterface.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/ThermoElectricProtocolInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/WaveCalProtocolInterface.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/WaveCalProtocolInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/WifiConfigurationProtocolInterface.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/WifiConfigurationProtocolInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/constants/OBPMessageTypes.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/constants/OBPMessageTypes.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPAddIPv4AddressExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPAddIPv4AddressExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPCommand.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPCommand.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPContinuousStrobeEnableExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPContinuousStrobeEnableExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPContinuousStrobePeriodExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPContinuousStrobePeriodExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPDataBufferClearExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPDataBufferClearExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPDataBufferRemoveOldestExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPDataBufferRemoveOldestExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPDeleteIPv4AddressExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPDeleteIPv4AddressExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetActivePixelRangesExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetActivePixelRangesExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetAllTemperaturesExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetAllTemperaturesExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetBoxcarWidthExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetBoxcarWidthExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetConsecutiveSampleCountExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetConsecutiveSampleCountExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDHCPServerAddressExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDHCPServerAddressExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDHCPServerEnableExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDHCPServerEnableExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDataBufferCapacityExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDataBufferCapacityExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDataBufferElementCountExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDataBufferElementCountExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDataBufferMaximumCapacityExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDataBufferMaximumCapacityExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDefaultPixelBinningExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDefaultPixelBinningExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetElectricDarkPixelRangesExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetElectricDarkPixelRangesExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetEthernetConfigurationGbEEnableExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetEthernetConfigurationGbEEnableExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetEthernetConfigurationMACAddressExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetEthernetConfigurationMACAddressExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetFastBufferingEnableExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetFastBufferingEnableExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetFirmwareRevisionExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetFirmwareRevisionExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOExtensionAvailableModesExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOExtensionAvailableModesExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOExtensionCurrentModeExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOExtensionCurrentModeExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOExtensionNumberOfPinsExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOExtensionNumberOfPinsExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOExtensionOutputVectorExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOExtensionOutputVectorExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOExtensionValueExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOExtensionValueExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIONumberOfPinsExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIONumberOfPinsExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOOutputEnableVectorExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOOutputEnableVectorExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOValueVectorExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOValueVectorExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetHardwareRevisionExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetHardwareRevisionExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetI2CMasterNumberOfBusesExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetI2CMasterNumberOfBusesExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIPv4AddressExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIPv4AddressExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIPv4DHCPEnableStateExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIPv4DHCPEnableStateExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIPv4DefaultGatewayExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIPv4DefaultGatewayExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIPv4NumberOfAddressesExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIPv4NumberOfAddressesExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIrradCalExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIrradCalExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIrradCollectionAreaExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIrradCollectionAreaExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetMaxPixelBinningExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetMaxPixelBinningExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetMulticastEnableExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetMulticastEnableExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNetworkInterfaceConnectionTypeExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNetworkInterfaceConnectionTypeExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNetworkInterfaceEnableStateExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNetworkInterfaceEnableStateExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNonlinearityCoeffExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNonlinearityCoeffExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNonlinearityCoeffsCountExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNonlinearityCoeffsCountExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNumberOfNetworkInterfacesExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNumberOfNetworkInterfacesExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNumberOfPixelsExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNumberOfPixelsExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchCoatingExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchCoatingExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchFiberDiameterMicronsExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchFiberDiameterMicronsExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchFilterExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchFilterExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchGratingExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchGratingExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchIDExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchIDExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchSerialNumberExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchSerialNumberExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchSlitWidthMicronsExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchSlitWidthMicronsExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalDarkPixelRangesExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalDarkPixelRangesExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetPixelBinningExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetPixelBinningExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetSaturationExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetSaturationExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetScansToAverageExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetScansToAverageExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetSerialNumberExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetSerialNumberExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetSerialNumberMaximumLengthExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetSerialNumberMaximumLengthExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetStrayLightCoeffExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetStrayLightCoeffExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetStrayLightCoeffsCountExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetStrayLightCoeffsCountExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetTemperatureCountExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetTemperatureCountExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetTemperatureExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetTemperatureExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetThermoElectricTemperatureExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetThermoElectricTemperatureExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetWaveCalExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetWaveCalExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetWifiConfigurationModeExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetWifiConfigurationModeExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetWifiConfigurationSSIDExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetWifiConfigurationSSIDExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetWifiConfigurationSecurityExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetWifiConfigurationSecurityExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPIntegrationTimeExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPIntegrationTimeExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPLampEnableCommand.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPLampEnableCommand.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPLightSourceEnableCommand.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPLightSourceEnableCommand.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPLightSourceEnabledQuery.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPLightSourceEnabledQuery.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPLightSourceIntensityCommand.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPLightSourceIntensityCommand.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPLightSourceIntensityQuery.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPLightSourceIntensityQuery.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPMessage.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPMessage.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPQuery.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPQuery.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPReadI2CMasterBusExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPReadI2CMasterBusExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPReadNumberOfRawSpectraWithMetadataExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPReadNumberOfRawSpectraWithMetadataExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPReadRawSpectrum32AndMetadataExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPReadRawSpectrum32AndMetadataExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPReadRawSpectrumExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPReadRawSpectrumExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPReadSpectrum32AndMetadataExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPReadSpectrum32AndMetadataExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPReadSpectrumExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPReadSpectrumExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPReadSpectrumWithGainExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPReadSpectrumWithGainExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPRequestBufferedSpectrum32AndMetadataExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPRequestBufferedSpectrum32AndMetadataExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPRequestNumberOfBufferedSpectraWithMetadataExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPRequestNumberOfBufferedSpectraWithMetadataExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPRequestRawSpectrumExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPRequestRawSpectrumExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPRequestSpectrumExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPRequestSpectrumExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPRunNetworkInterfaceSelfTestExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPRunNetworkInterfaceSelfTestExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSaveNetworkInterfaceConnectionSettingsExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSaveNetworkInterfaceConnectionSettingsExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetAcquisitionDelayExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetAcquisitionDelayExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetBoxcarWidthExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetBoxcarWidthExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetConsecutiveSampleCountExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetConsecutiveSampleCountExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetDHCPServerAddressExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetDHCPServerAddressExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetDHCPServerEnableExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetDHCPServerEnableExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetDataBufferCapacityExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetDataBufferCapacityExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetDefaultPixelBinningExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetDefaultPixelBinningExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetEthernetConfigurationGbEEnableExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetEthernetConfigurationGbEEnableExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetEthernetConfigurationMACAddressExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetEthernetConfigurationMACAddressExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetFastBufferingEnableExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetFastBufferingEnableExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetGPIOExtensionModeExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetGPIOExtensionModeExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetGPIOExtensionOutputVectorExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetGPIOExtensionOutputVectorExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetGPIOExtensionValueExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetGPIOExtensionValueExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetGPIOExtensionVectorExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetGPIOExtensionVectorExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetGPIOOutputEnableVectorExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetGPIOOutputEnableVectorExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetGPIOValueVectorExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetGPIOValueVectorExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetIPv4DHCPEnableStateExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetIPv4DHCPEnableStateExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetIPv4DefaultGatewayExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetIPv4DefaultGatewayExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetIrradCalExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetIrradCalExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetIrradCollectionAreaExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetIrradCollectionAreaExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetMulticastEnableExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetMulticastEnableExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetNetworkInterfaceEnableStateExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetNetworkInterfaceEnableStateExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetPixelBinningExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetPixelBinningExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetScansToAverageExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetScansToAverageExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetThermoElectricEnableExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetThermoElectricEnableExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetThermoElectricSetpointExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetThermoElectricSetpointExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetWifiConfigurationModeExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetWifiConfigurationModeExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetWifiConfigurationPassPhraseExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetWifiConfigurationPassPhraseExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetWifiConfigurationSSIDExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetWifiConfigurationSSIDExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetWifiConfigurationSecurityExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetWifiConfigurationSecurityExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPShutterExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPShutterExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPTransaction.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPTransaction.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPTriggerModeExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPTriggerModeExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPWriteI2CMasterBusExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPWriteI2CMasterBusExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/hints/OBPControlHint.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/hints/OBPControlHint.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/hints/OBPSpectrumHint.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/hints/OBPSpectrumHint.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPAcquisitionDelayProtocol.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPAcquisitionDelayProtocol.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPContinuousStrobeProtocol.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPContinuousStrobeProtocol.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPDHCPServerProtocol.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPDHCPServerProtocol.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPDataBufferProtocol.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPDataBufferProtocol.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPEthernetConfigurationProtocol.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPEthernetConfigurationProtocol.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPFastBufferProtocol.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPFastBufferProtocol.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPGPIOProtocol.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPGPIOProtocol.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPI2CMasterProtocol.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPI2CMasterProtocol.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPIPv4Protocol.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPIPv4Protocol.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPIntrospectionProtocol.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPIntrospectionProtocol.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPIrradCalProtocol.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPIrradCalProtocol.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPLightSourceProtocol.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPLightSourceProtocol.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPLightSourceProtocol_Ventana.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPLightSourceProtocol_Ventana.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPMulticastProtocol.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPMulticastProtocol.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPNetworkConfigurationProtocol.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPNetworkConfigurationProtocol.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPNonlinearityCoeffsProtocol.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPNonlinearityCoeffsProtocol.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPOpticalBenchProtocol.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPOpticalBenchProtocol.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPPixelBinningProtocol.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPPixelBinningProtocol.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPProgrammableSaturationProtocol.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPProgrammableSaturationProtocol.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPRevisionProtocol.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPRevisionProtocol.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPSerialNumberProtocol.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPSerialNumberProtocol.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPShutterProtocol.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPShutterProtocol.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPSpectrometerProtocol.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPSpectrometerProtocol.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPSpectrumProcessingProtocol.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPSpectrumProcessingProtocol.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPStrayLightCoeffsProtocol.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPStrayLightCoeffsProtocol.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPStrobeLampProtocol.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPStrobeLampProtocol.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPTemperatureProtocol.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPTemperatureProtocol.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPThermoElectricProtocol.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPThermoElectricProtocol.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPWaveCalProtocol.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPWaveCalProtocol.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPWifiConfigurationProtocol.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPWifiConfigurationProtocol.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OceanBinaryProtocol.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OceanBinaryProtocol.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/constants/FPGARegisterCodes.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/constants/FPGARegisterCodes.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/constants/OpCodes.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/constants/OpCodes.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/constants/QETECConstants.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/constants/QETECConstants.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/FPGARegisterReadExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/FPGARegisterReadExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/FPGARegisterWriteExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/FPGARegisterWriteExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/FPGASpectrumExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/FPGASpectrumExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/FlameNIRSpectrumExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/FlameNIRSpectrumExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/HRFPGASpectrumExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/HRFPGASpectrumExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/IntegrationTimeExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/IntegrationTimeExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/JazSpectrumExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/JazSpectrumExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/MayaProSpectrumExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/MayaProSpectrumExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/NIRQuestSpectrumExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/NIRQuestSpectrumExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/OOI2KSpectrumExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/OOI2KSpectrumExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/OOIIrradCalExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/OOIIrradCalExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/OOIReadIrradCalExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/OOIReadIrradCalExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/OOIWriteIrradCalExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/OOIWriteIrradCalExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/QESpectrumExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/QESpectrumExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/ReadEEPROMSlotExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/ReadEEPROMSlotExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/ReadSpectrumExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/ReadSpectrumExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/ReadTECQETemperatureExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/ReadTECQETemperatureExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/ReadTECTemperatureExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/ReadTECTemperatureExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/RequestSpectrumExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/RequestSpectrumExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/StrobeEnableExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/StrobeEnableExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/TECEnableExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/TECEnableExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/TECQEEnableExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/TECQEEnableExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/TriggerModeExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/TriggerModeExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/USBFPGASpectrumExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/USBFPGASpectrumExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/WriteEEPROMSlotExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/WriteEEPROMSlotExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/WriteTECQESetPointExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/WriteTECQESetPointExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/WriteTECSetPointExchange.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/WriteTECSetPointExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/hints/ControlHint.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/hints/ControlHint.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/hints/SpectrumHint.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/hints/SpectrumHint.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/impls/FPGARegisterProtocol.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/impls/FPGARegisterProtocol.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/impls/OOIEEPROMProtocol.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/impls/OOIEEPROMProtocol.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/impls/OOIIrradCalProtocol.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/impls/OOIIrradCalProtocol.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/impls/OOIProtocol.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/impls/OOIProtocol.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/impls/OOISpectrometerProtocol.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/impls/OOISpectrometerProtocol.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/impls/OOIStrobeLampProtocol.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/impls/OOIStrobeLampProtocol.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/impls/OOITECProtocol.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/impls/OOITECProtocol.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/include/vendors/OceanOptics/utils/Polynomial.h` & `seabreeze-2.2.0/src/libseabreeze/include/vendors/OceanOptics/utils/Polynomial.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/api/DeviceFactory.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/api/DeviceFactory.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/api/seabreezeapi/AcquisitionDelayFeatureAdapter.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/api/seabreezeapi/AcquisitionDelayFeatureAdapter.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/api/seabreezeapi/ContinuousStrobeFeatureAdapter.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/api/seabreezeapi/ContinuousStrobeFeatureAdapter.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/api/seabreezeapi/DHCPServerFeatureAdapter.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/api/seabreezeapi/DHCPServerFeatureAdapter.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/api/seabreezeapi/DataBufferFeatureAdapter.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/api/seabreezeapi/DataBufferFeatureAdapter.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/api/seabreezeapi/DeviceAdapter.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/api/seabreezeapi/DeviceAdapter.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/api/seabreezeapi/EEPROMFeatureAdapter.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/api/seabreezeapi/EEPROMFeatureAdapter.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/api/seabreezeapi/EthernetConfigurationFeatureAdapter.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/api/seabreezeapi/EthernetConfigurationFeatureAdapter.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/api/seabreezeapi/FastBufferFeatureAdapter.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/api/seabreezeapi/FastBufferFeatureAdapter.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/api/seabreezeapi/FeatureFamilies.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/api/seabreezeapi/FeatureFamilies.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/api/seabreezeapi/I2CMasterFeatureAdapter.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/api/seabreezeapi/I2CMasterFeatureAdapter.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/api/seabreezeapi/IPv4FeatureAdapter.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/api/seabreezeapi/IPv4FeatureAdapter.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/api/seabreezeapi/IntrospectionFeatureAdapter.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/api/seabreezeapi/IntrospectionFeatureAdapter.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/api/seabreezeapi/IrradCalFeatureAdapter.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/api/seabreezeapi/IrradCalFeatureAdapter.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/api/seabreezeapi/LightSourceFeatureAdapter.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/api/seabreezeapi/LightSourceFeatureAdapter.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/api/seabreezeapi/MulticastFeatureAdapter.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/api/seabreezeapi/MulticastFeatureAdapter.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/api/seabreezeapi/NetworkConfigurationFeatureAdapter.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/api/seabreezeapi/NetworkConfigurationFeatureAdapter.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/api/seabreezeapi/NonlinearityCoeffsFeatureAdapter.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/api/seabreezeapi/NonlinearityCoeffsFeatureAdapter.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/api/seabreezeapi/OpticalBenchFeatureAdapter.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/api/seabreezeapi/OpticalBenchFeatureAdapter.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/api/seabreezeapi/PixelBinningFeatureAdapter.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/api/seabreezeapi/PixelBinningFeatureAdapter.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/api/seabreezeapi/ProtocolFamilies.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/api/seabreezeapi/ProtocolFamilies.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/api/seabreezeapi/RawUSBBusAccessFeatureAdapter.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/api/seabreezeapi/RawUSBBusAccessFeatureAdapter.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/api/seabreezeapi/RevisionFeatureAdapter.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/api/seabreezeapi/RevisionFeatureAdapter.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/api/seabreezeapi/SeaBreezeAPI.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/api/seabreezeapi/SeaBreezeAPI.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/api/seabreezeapi/SeaBreezeAPI_Impl.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/api/seabreezeapi/SeaBreezeAPI_Impl.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/api/seabreezeapi/SerialNumberFeatureAdapter.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/api/seabreezeapi/SerialNumberFeatureAdapter.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/api/seabreezeapi/ShutterFeatureAdapter.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/api/seabreezeapi/ShutterFeatureAdapter.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/api/seabreezeapi/SpectrometerFeatureAdapter.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/api/seabreezeapi/SpectrometerFeatureAdapter.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/api/seabreezeapi/SpectrumProcessingFeatureAdapter.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/api/seabreezeapi/SpectrumProcessingFeatureAdapter.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/api/seabreezeapi/StrayLightCoeffsFeatureAdapter.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/api/seabreezeapi/StrayLightCoeffsFeatureAdapter.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/api/seabreezeapi/StrobeLampFeatureAdapter.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/api/seabreezeapi/StrobeLampFeatureAdapter.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/api/seabreezeapi/TemperatureFeatureAdapter.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/api/seabreezeapi/TemperatureFeatureAdapter.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/api/seabreezeapi/ThermoElectricCoolerFeatureAdapter.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/api/seabreezeapi/ThermoElectricCoolerFeatureAdapter.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/api/seabreezeapi/WifiConfigurationFeatureAdapter.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/api/seabreezeapi/WifiConfigurationFeatureAdapter.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/api/seabreezeapi/gpioFeatureAdapter.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/api/seabreezeapi/gpioFeatureAdapter.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/common/ByteVector.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/common/ByteVector.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/common/Data.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/common/Data.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/common/DoubleVector.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/common/DoubleVector.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/common/FloatVector.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/common/FloatVector.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/common/Log.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/common/Log.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/common/U32Vector.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/common/U32Vector.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/common/UShortVector.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/common/UShortVector.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/common/UnitDescriptor.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/common/UnitDescriptor.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/common/buses/Bus.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/common/buses/Bus.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/common/buses/BusFamilies.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/common/buses/BusFamilies.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/common/buses/BusFamily.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/common/buses/BusFamily.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/common/buses/DeviceLocationProberInterface.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/common/buses/DeviceLocationProberInterface.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/common/buses/TransferHelper.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/common/buses/TransferHelper.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/common/buses/network/IPv4NetworkProtocol.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/common/buses/network/IPv4NetworkProtocol.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/common/buses/network/IPv4SocketDeviceLocator.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/common/buses/network/IPv4SocketDeviceLocator.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/common/buses/network/TCPIPv4SocketBus.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/common/buses/network/TCPIPv4SocketBus.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/common/buses/network/TCPIPv4SocketTransferHelper.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/common/buses/network/TCPIPv4SocketTransferHelper.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/common/buses/rs232/RS232DeviceLocator.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/common/buses/rs232/RS232DeviceLocator.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/common/buses/rs232/RS232Interface.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/common/buses/rs232/RS232Interface.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/common/buses/rs232/RS232TransferHelper.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/common/buses/rs232/RS232TransferHelper.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/common/buses/usb/USBDeviceLocator.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/common/buses/usb/USBDeviceLocator.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/common/buses/usb/USBInterface.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/common/buses/usb/USBInterface.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/common/buses/usb/USBTransferHelper.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/common/buses/usb/USBTransferHelper.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/common/devices/Device.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/common/devices/Device.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/common/exceptions/BusConnectException.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/common/exceptions/BusConnectException.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/common/exceptions/BusException.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/common/exceptions/BusException.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/common/exceptions/BusTransferException.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/common/exceptions/BusTransferException.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/common/exceptions/FeatureControlException.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/common/exceptions/FeatureControlException.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/common/exceptions/FeatureException.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/common/exceptions/FeatureException.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/common/exceptions/FeatureProtocolNotFoundException.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/common/exceptions/FeatureProtocolNotFoundException.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/common/exceptions/IllegalArgumentException.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/common/exceptions/IllegalArgumentException.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/common/exceptions/NumberFormatException.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/common/exceptions/NumberFormatException.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/common/exceptions/ProtocolBusMismatchException.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/common/exceptions/ProtocolBusMismatchException.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/common/exceptions/ProtocolException.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/common/exceptions/ProtocolException.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/common/exceptions/ProtocolFormatException.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/common/exceptions/ProtocolFormatException.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/common/exceptions/ProtocolTransactionException.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/common/exceptions/ProtocolTransactionException.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/common/features/FeatureFamily.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/common/features/FeatureFamily.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/common/features/FeatureImpl.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/common/features/FeatureImpl.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/common/protocols/Exchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/common/protocols/Exchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/common/protocols/Protocol.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/common/protocols/Protocol.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/common/protocols/ProtocolFamily.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/common/protocols/ProtocolFamily.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/common/protocols/ProtocolHelper.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/common/protocols/ProtocolHelper.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/common/protocols/ProtocolHint.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/common/protocols/ProtocolHint.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/common/protocols/Transaction.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/common/protocols/Transaction.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/common/protocols/Transfer.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/common/protocols/Transfer.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/native/network/Inet4Address.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/native/network/Inet4Address.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/native/network/SocketException.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/native/network/SocketException.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/native/network/SocketTimeoutException.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/native/network/SocketTimeoutException.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/native/network/UnknownHostException.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/native/network/UnknownHostException.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/native/network/posix/NativeSocketPOSIX.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/native/network/posix/NativeSocketPOSIX.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/native/network/windows/NativeSocketWindows.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/native/network/windows/NativeSocketWindows.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/native/rs232/RS232.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/native/rs232/RS232.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/native/rs232/posix/NativeRS232POSIX.c` & `seabreeze-2.2.0/src/libseabreeze/src/native/rs232/posix/NativeRS232POSIX.c`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/native/rs232/windows/NativeRS232Windows.c` & `seabreeze-2.2.0/src/libseabreeze/src/native/rs232/windows/NativeRS232Windows.c`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/native/system/System.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/native/system/System.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/native/system/posix/NativeSystemPOSIX.c` & `seabreeze-2.2.0/src/libseabreeze/src/native/system/posix/NativeSystemPOSIX.c`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/native/system/windows/NativeSystemWindows.c` & `seabreeze-2.2.0/src/libseabreeze/src/native/system/windows/NativeSystemWindows.c`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/native/usb/USB.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/native/usb/USB.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/native/usb/USBDiscovery.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/native/usb/USBDiscovery.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/native/usb/linux/NativeUSBLinux.c` & `seabreeze-2.2.0/src/libseabreeze/src/native/usb/linux/NativeUSBLinux.c`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/native/usb/osx/NativeUSBMacOSX.c` & `seabreeze-2.2.0/src/libseabreeze/src/native/usb/osx/NativeUSBMacOSX.c`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/native/usb/winusb/NativeUSBWinUSB.c` & `seabreeze-2.2.0/src/libseabreeze/src/native/usb/winusb/NativeUSBWinUSB.c`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/buses/network/FlameXTCPIPv4.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/buses/network/FlameXTCPIPv4.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/buses/network/JazTCPIPv4.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/buses/network/JazTCPIPv4.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/buses/rs232/OOIRS232Interface.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/buses/rs232/OOIRS232Interface.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/ApexUSB.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/ApexUSB.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/FlameNIRUSB.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/FlameNIRUSB.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/FlameXUSB.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/FlameXUSB.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/FlameXUSBTransferHelper.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/FlameXUSBTransferHelper.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/HR2000PlusUSB.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/HR2000PlusUSB.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/HR2000USB.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/HR2000USB.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/HR4000USB.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/HR4000USB.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/JazUSB.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/JazUSB.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/Maya2000ProUSB.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/Maya2000ProUSB.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/Maya2000USB.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/Maya2000USB.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/MayaLSLUSB.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/MayaLSLUSB.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/NIRQuest256USB.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/NIRQuest256USB.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/NIRQuest512USB.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/NIRQuest512USB.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/OOIUSB4KSpectrumTransferHelper.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/OOIUSB4KSpectrumTransferHelper.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/OOIUSBControlTransferHelper.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/OOIUSBControlTransferHelper.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/OOIUSBEndpointMaps.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/OOIUSBEndpointMaps.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/OOIUSBInterface.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/OOIUSBInterface.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/OOIUSBSpectrumTransferHelper.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/OOIUSBSpectrumTransferHelper.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/OOIUSBTrivialTransferHelper.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/OOIUSBTrivialTransferHelper.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/QE65000USB.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/QE65000USB.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/QEProUSB.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/QEProUSB.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/STSUSB.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/STSUSB.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/SparkUSB.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/SparkUSB.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/TorusUSB.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/TorusUSB.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/USB2000PlusUSB.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/USB2000PlusUSB.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/USB2000USB.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/USB2000USB.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/USB4000USB.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/USB4000USB.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/VentanaUSB.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/VentanaUSB.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/devices/Apex.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/devices/Apex.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/devices/FlameNIR.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/devices/FlameNIR.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/devices/FlameX.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/devices/FlameX.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/devices/HR2000.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/devices/HR2000.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/devices/HR2000Plus.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/devices/HR2000Plus.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/devices/HR4000.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/devices/HR4000.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/devices/Jaz.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/devices/Jaz.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/devices/Maya2000.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/devices/Maya2000.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/devices/Maya2000Pro.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/devices/Maya2000Pro.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/devices/MayaLSL.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/devices/MayaLSL.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/devices/NIRQuest256.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/devices/NIRQuest256.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/devices/NIRQuest512.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/devices/NIRQuest512.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/devices/QE65000.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/devices/QE65000.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/devices/QEPro.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/devices/QEPro.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/devices/STS.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/devices/STS.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/devices/Spark.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/devices/Spark.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/devices/Torus.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/devices/Torus.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/devices/USB2000.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/devices/USB2000.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/devices/USB2000Plus.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/devices/USB2000Plus.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/devices/USB4000.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/devices/USB4000.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/devices/Ventana.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/devices/Ventana.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/acquisition_delay/AcquisitionDelayFeature.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/acquisition_delay/AcquisitionDelayFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/acquisition_delay/AcquisitionDelayFeature_FPGA.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/acquisition_delay/AcquisitionDelayFeature_FPGA.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/acquisition_delay/STSAcquisitionDelayFeature.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/acquisition_delay/STSAcquisitionDelayFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/continuous_strobe/ContinuousStrobeFeature.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/continuous_strobe/ContinuousStrobeFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/continuous_strobe/ContinuousStrobeFeature_FPGA.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/continuous_strobe/ContinuousStrobeFeature_FPGA.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/data_buffer/DataBufferFeatureBase.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/data_buffer/DataBufferFeatureBase.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/data_buffer/FlameXDataBufferFeature.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/data_buffer/FlameXDataBufferFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/data_buffer/QEProDataBufferFeature.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/data_buffer/QEProDataBufferFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/dhcp_server/DHCPServerFeature.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/dhcp_server/DHCPServerFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/EEPROMSlotFeature.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/EEPROMSlotFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/EEPROMSlotFeatureBase.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/EEPROMSlotFeatureBase.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/NonlinearityEEPROMSlotFeature.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/NonlinearityEEPROMSlotFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/SaturationEEPROMSlotFeature.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/SaturationEEPROMSlotFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/SaturationEEPROMSlotFeatureBase.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/SaturationEEPROMSlotFeatureBase.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/SaturationEEPROMSlotFeature_MayaPro.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/SaturationEEPROMSlotFeature_MayaPro.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/SaturationEEPROMSlotFeature_NIRQuest.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/SaturationEEPROMSlotFeature_NIRQuest.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/SerialNumberEEPROMSlotFeature.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/SerialNumberEEPROMSlotFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/StrayLightEEPROMSlotFeature.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/StrayLightEEPROMSlotFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/WavelengthEEPROMSlotFeature.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/WavelengthEEPROMSlotFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/WavelengthEEPROMSlotFeature_QE65000.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/WavelengthEEPROMSlotFeature_QE65000.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/ethernet_configuration/EthernetConfigurationFeature.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/ethernet_configuration/EthernetConfigurationFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/fast_buffer/FastBufferFeatureBase.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/fast_buffer/FastBufferFeatureBase.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/fast_buffer/FlameXFastBufferFeature.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/fast_buffer/FlameXFastBufferFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/fpga_register/FPGARegisterFeature.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/fpga_register/FPGARegisterFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/gpio/gpioFeature.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/gpio/gpioFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/i2c_master/i2cFeature.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/i2c_master/i2cFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/introspection/IntrospectionFeature.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/introspection/IntrospectionFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/ipv4/IPv4Feature.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/ipv4/IPv4Feature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/irradcal/IrradCalFeature.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/irradcal/IrradCalFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/light_source/LightSourceFeatureBase.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/light_source/LightSourceFeatureBase.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/light_source/LightSourceFeatureImpl.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/light_source/LightSourceFeatureImpl.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/light_source/StrobeLampFeature.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/light_source/StrobeLampFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/light_source/VentanaLightSourceFeature.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/light_source/VentanaLightSourceFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/multicast/MulticastFeature.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/multicast/MulticastFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/network_configuration/NetworkConfigurationFeature.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/network_configuration/NetworkConfigurationFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/nonlinearity/NonlinearityCoeffsFeature.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/nonlinearity/NonlinearityCoeffsFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/optical_bench/OpticalBenchFeature.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/optical_bench/OpticalBenchFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/pixel_binning/PixelBinningFeatureInterface.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/pixel_binning/PixelBinningFeatureInterface.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/pixel_binning/STSPixelBinningFeature.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/pixel_binning/STSPixelBinningFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/raw_bus_access/RawUSBBusAccessFeature.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/raw_bus_access/RawUSBBusAccessFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/revision/RevisionFeature.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/revision/RevisionFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/serial_number/SerialNumberFeature.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/serial_number/SerialNumberFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/shutter/ShutterFeature.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/shutter/ShutterFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/ApexSpectrometerFeature.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/ApexSpectrometerFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/FlameNIRSpectrometerFeature.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/FlameNIRSpectrometerFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/FlameXSpectrometerFeature.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/FlameXSpectrometerFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/GainAdjustedSpectrometerFeature.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/GainAdjustedSpectrometerFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/HR2000PlusSpectrometerFeature.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/HR2000PlusSpectrometerFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/HR2000SpectrometerFeature.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/HR2000SpectrometerFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/HR4000SpectrometerFeature.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/HR4000SpectrometerFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/JazSpectrometerFeature.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/JazSpectrometerFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/Maya2000ProSpectrometerFeature.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/Maya2000ProSpectrometerFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/Maya2000SpectrometerFeature.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/Maya2000SpectrometerFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/MayaLSLSpectrometerFeature.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/MayaLSLSpectrometerFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/NIRQuest256SpectrometerFeature.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/NIRQuest256SpectrometerFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/NIRQuest512SpectrometerFeature.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/NIRQuest512SpectrometerFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/NIRQuestSpectrometerFeature.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/NIRQuestSpectrometerFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/OOISpectrometerFeature.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/OOISpectrometerFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/ProgrammableSaturationFeature.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/ProgrammableSaturationFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/ProgrammableSaturationFeatureBase.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/ProgrammableSaturationFeatureBase.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/ProgrammableSaturationFeatureImpl.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/ProgrammableSaturationFeatureImpl.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/QE65000SpectrometerFeature.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/QE65000SpectrometerFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/QEProSpectrometerFeature.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/QEProSpectrometerFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/STSSpectrometerFeature.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/STSSpectrometerFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/SparkSpectrometerFeature.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/SparkSpectrometerFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/SpectrometerTriggerMode.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/SpectrometerTriggerMode.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/USB2000PlusSpectrometerFeature.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/USB2000PlusSpectrometerFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/USB2000SpectrometerFeature.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/USB2000SpectrometerFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/USB4000SpectrometerFeature.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/USB4000SpectrometerFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/VentanaSpectrometerFeature.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/VentanaSpectrometerFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrum_processing/SpectrumProcessingFeature.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrum_processing/SpectrumProcessingFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/stray_light/StrayLightCoeffsFeature.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/stray_light/StrayLightCoeffsFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/temperature/TemperatureFeature.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/temperature/TemperatureFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/thermoelectric/QEProThermoElectricFeature.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/thermoelectric/QEProThermoElectricFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/thermoelectric/ThermoElectricFeatureBase.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/thermoelectric/ThermoElectricFeatureBase.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/thermoelectric/ThermoElectricQEFeature.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/thermoelectric/ThermoElectricQEFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/thermoelectric/VentanaThermoElectricFeature.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/thermoelectric/VentanaThermoElectricFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/wavecal/WaveCalFeature.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/wavecal/WaveCalFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/features/wifi_configuration/WifiConfigurationFeature.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/features/wifi_configuration/WifiConfigurationFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/AcquisitionDelayProtocolInterface.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/AcquisitionDelayProtocolInterface.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/ContinuousStrobeProtocolInterface.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/ContinuousStrobeProtocolInterface.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/DHCPServerProtocolInterface.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/DHCPServerProtocolInterface.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/DataBufferProtocolInterface.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/DataBufferProtocolInterface.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/EEPROMProtocolInterface.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/EEPROMProtocolInterface.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/EthernetConfigurationProtocolInterface.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/EthernetConfigurationProtocolInterface.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/FPGARegisterProtocolInterface.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/FPGARegisterProtocolInterface.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/FastBufferProtocolInterface.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/FastBufferProtocolInterface.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/GPIOProtocolInterface.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/GPIOProtocolInterface.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/I2CMasterProtocolInterface.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/I2CMasterProtocolInterface.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/IPv4ProtocolInterface.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/IPv4ProtocolInterface.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/IntrospectionProtocolInterface.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/IntrospectionProtocolInterface.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/IrradCalProtocolInterface.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/IrradCalProtocolInterface.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/LightSourceProtocolInterface.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/LightSourceProtocolInterface.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/MulticastProtocolInterface.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/MulticastProtocolInterface.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/NetworkConfigurationProtocolInterface.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/NetworkConfigurationProtocolInterface.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/NonlinearityCoeffsProtocolInterface.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/NonlinearityCoeffsProtocolInterface.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/OpticalBenchProtocolInteface.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/OpticalBenchProtocolInteface.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/PixelBinningProtocolInterface.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/PixelBinningProtocolInterface.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/ProgrammableSaturationProtocolInteface.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/ProgrammableSaturationProtocolInteface.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/RevisionProtocolInteface.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/RevisionProtocolInteface.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/SerialNumberProtocolInterface.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/SerialNumberProtocolInterface.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/ShutterProtocolInterface.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/ShutterProtocolInterface.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/SpectrometerProtocolInterface.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/SpectrometerProtocolInterface.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/SpectrumProcessingProtocolInteface.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/SpectrumProcessingProtocolInteface.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/StrayLightCoeffsProtocolInterface.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/StrayLightCoeffsProtocolInterface.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/StrobeLampProtocolInterface.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/StrobeLampProtocolInterface.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/TemperatureProtocolInteface.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/TemperatureProtocolInteface.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/ThermoElectricProtocolInterface.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/ThermoElectricProtocolInterface.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/WaveCalProtocolInterface.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/WaveCalProtocolInterface.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/WifiConfigurationProtocolInterface.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/WifiConfigurationProtocolInterface.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPAddIPv4AddressExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPAddIPv4AddressExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPCommand.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPCommand.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPContinuousStrobeEnableExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPContinuousStrobeEnableExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPContinuousStrobePeriodExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPContinuousStrobePeriodExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPDataBufferClearExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPDataBufferClearExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPDataBufferRemoveOldestExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPDataBufferRemoveOldestExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPDeleteIPv4AddressExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPDeleteIPv4AddressExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetActivePixelRangesExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetActivePixelRangesExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetAllTemperaturesExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetAllTemperaturesExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetBoxcarWidthExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetBoxcarWidthExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetConsecutiveSampleCountExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetConsecutiveSampleCountExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDHCPServerAddressExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDHCPServerAddressExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDHCPServerEnableExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDHCPServerEnableExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDataBufferCapacityExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDataBufferCapacityExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDataBufferCountExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDataBufferCountExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDataBufferMaximumCapacityExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDataBufferMaximumCapacityExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDefaultPixelBinningExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDefaultPixelBinningExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetElectricDarkPixelRangesExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetElectricDarkPixelRangesExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetEthernetConfigurationGbEEnableExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetEthernetConfigurationGbEEnableExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetEthernetConfigurationMACAddressExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetEthernetConfigurationMACAddressExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetFastBufferingEnableExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetFastBufferingEnableExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetFirmwareRevisionExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetFirmwareRevisionExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOExtensionAvailableModesExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOExtensionAvailableModesExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOExtensionCurrentModeExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOExtensionCurrentModeExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOExtensionNumberOfPinsExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOExtensionNumberOfPinsExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOExtensionOutputVectorExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOExtensionOutputVectorExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOExtensionValueExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOExtensionValueExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIONumberOfPinsExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIONumberOfPinsExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOOutputEnableVectorExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOOutputEnableVectorExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOValueVectorExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOValueVectorExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetHardwareRevisionExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetHardwareRevisionExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetI2CMasterNumberOfBusesExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetI2CMasterNumberOfBusesExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIPv4AddressExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIPv4AddressExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIPv4DHCPEnableStateExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIPv4DHCPEnableStateExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIPv4DefaultGatewayExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIPv4DefaultGatewayExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIPv4NumberOfAddressesExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIPv4NumberOfAddressesExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIrradCalExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIrradCalExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIrradCollectionAreaExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIrradCollectionAreaExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetMaxPixelBinningExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetMaxPixelBinningExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetMulticastEnableExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetMulticastEnableExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNetworkInterfaceConnectionTypeExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNetworkInterfaceConnectionTypeExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNetworkInterfaceEnableStateExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNetworkInterfaceEnableStateExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNonlinearityCoeffExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNonlinearityCoeffExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNonlinearityCoeffsCountExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNonlinearityCoeffsCountExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNumberOfNetworkInterfacesExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNumberOfNetworkInterfacesExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNumberOfPixelsExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNumberOfPixelsExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchCoatingExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchCoatingExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchFiberDiameterMicronsExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchFiberDiameterMicronsExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchFilterExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchFilterExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchGratingExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchGratingExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchIDExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchIDExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchSerialNumberExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchSerialNumberExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchSlitWidthMicronsExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchSlitWidthMicronsExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalDarkPixelRangesExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalDarkPixelRangesExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetPixelBinningExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetPixelBinningExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetSaturationExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetSaturationExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetScansToAverageExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetScansToAverageExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetSerialNumberExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetSerialNumberExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetSerialNumberMaximumLengthExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetSerialNumberMaximumLengthExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetStrayLightCoeffExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetStrayLightCoeffExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetStrayLightCoeffsCountExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetStrayLightCoeffsCountExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetTemperatureCountExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetTemperatureCountExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetTemperatureExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetTemperatureExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetThermoElectricTemperatureExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetThermoElectricTemperatureExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetWaveCalExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetWaveCalExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetWifiConfigurationModeExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetWifiConfigurationModeExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetWifiConfigurationSSIDExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetWifiConfigurationSSIDExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetWifiConfigurationSecurityExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetWifiConfigurationSecurityExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPIntegrationTimeExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPIntegrationTimeExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPLampEnableCommand.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPLampEnableCommand.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPLightSourceEnableCommand.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPLightSourceEnableCommand.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPLightSourceEnabledQuery.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPLightSourceEnabledQuery.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPLightSourceIntensityCommand.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPLightSourceIntensityCommand.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPLightSourceIntensityQuery.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPLightSourceIntensityQuery.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPMessage.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPMessage.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPQuery.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPQuery.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPReadI2CMasterBusExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPReadI2CMasterBusExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPReadNumberOfRawSpectraWithMetadataExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPReadNumberOfRawSpectraWithMetadataExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPReadRawSpectrum32AndMetadataExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPReadRawSpectrum32AndMetadataExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPReadRawSpectrumExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPReadRawSpectrumExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPReadSpectrum32AndMetadataExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPReadSpectrum32AndMetadataExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPReadSpectrumExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPReadSpectrumExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPReadSpectrumWithGainExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPReadSpectrumWithGainExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPRequestBufferedSpectrum32AndMetadata.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPRequestBufferedSpectrum32AndMetadata.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPRequestNumberOfBufferedSpectraWithMetadata.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPRequestNumberOfBufferedSpectraWithMetadata.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPRequestRawSpectrumExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPRequestRawSpectrumExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPRequestSpectrumExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPRequestSpectrumExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPRunNetworkInterfaceSelfTestExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPRunNetworkInterfaceSelfTestExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSaveNetworkInterfaceConnectionSettingsExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSaveNetworkInterfaceConnectionSettingsExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetAcquisitionDelayExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetAcquisitionDelayExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetBoxcarWidthExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetBoxcarWidthExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetConsecutiveSampleCountExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetConsecutiveSampleCountExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetDHCPServerAddressExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetDHCPServerAddressExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetDHCPServerEnableExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetDHCPServerEnableExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetDataBufferCapacityExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetDataBufferCapacityExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetDefaultPixelBinningFactorExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetDefaultPixelBinningFactorExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetEthernetConfigurationGbEEnableExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetEthernetConfigurationGbEEnableExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetEthernetConfigurationMACAddressExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetEthernetConfigurationMACAddressExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetFastBufferingEnableExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetFastBufferingEnableExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetGPIOExtensionModeExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetGPIOExtensionModeExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetGPIOExtensionOutputVectorExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetGPIOExtensionOutputVectorExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetGPIOExtensionValueExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetGPIOExtensionValueExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetGPIOOutputEnableVectorExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetGPIOOutputEnableVectorExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetGPIOValueVectorExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetGPIOValueVectorExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetIPv4DHCPEnableStateExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetIPv4DHCPEnableStateExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetIPv4DefaultGatewayExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetIPv4DefaultGatewayExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetIrradCalExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetIrradCalExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetIrradCollectionAreaExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetIrradCollectionAreaExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetMulticastEnableExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetMulticastEnableExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetNetworkInterfaceEnableStateExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetNetworkInterfaceEnableStateExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetPixelBinningExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetPixelBinningExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetScansToAverageExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetScansToAverageExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetThermoElectricEnableExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetThermoElectricEnableExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetThermoElectricSetpointExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetThermoElectricSetpointExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetWifiConfigurationModeExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetWifiConfigurationModeExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetWifiConfigurationPassPhraseExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetWifiConfigurationPassPhraseExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetWifiConfigurationSSIDExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetWifiConfigurationSSIDExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetWifiConfigurationSecurityExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetWifiConfigurationSecurityExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPShutterExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPShutterExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPTransaction.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPTransaction.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPTriggerModeExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPTriggerModeExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPWriteI2CMasterBusExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPWriteI2CMasterBusExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/hints/OBPControlHint.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/hints/OBPControlHint.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/hints/OBPSpectrumHint.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/hints/OBPSpectrumHint.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPAcquisitionDelayProtocol.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPAcquisitionDelayProtocol.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPContinuousStrobeProtocol.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPContinuousStrobeProtocol.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPDHCPServerProtocol.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPDHCPServerProtocol.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPDataBufferProtocol.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPDataBufferProtocol.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPEthernetConfigurationProtocol.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPEthernetConfigurationProtocol.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPFastBufferProtocol.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPFastBufferProtocol.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPGPIOProtocol.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPGPIOProtocol.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPI2CMasterProtocol.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPI2CMasterProtocol.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPIPv4Protocol.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPIPv4Protocol.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPIntrospectionProtocol.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPIntrospectionProtocol.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPIrradCalProtocol.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPIrradCalProtocol.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPLightSourceProtocol.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPLightSourceProtocol.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPLightSourceProtocol_Ventana.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPLightSourceProtocol_Ventana.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPMulticastProtocol.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPMulticastProtocol.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPNetworkConfigurationProtocol.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPNetworkConfigurationProtocol.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPNonlinearityCoeffsProtocol.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPNonlinearityCoeffsProtocol.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPOpticalBenchProtocol.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPOpticalBenchProtocol.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPPixelBinningProtocol.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPPixelBinningProtocol.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPProgrammableSaturationProtocol.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPProgrammableSaturationProtocol.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPRevisionProtocol.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPRevisionProtocol.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPSerialNumberProtocol.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPSerialNumberProtocol.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPShutterProtocol.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPShutterProtocol.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPSpectrometerProtocol.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPSpectrometerProtocol.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPSpectrumProcessingProtocol.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPSpectrumProcessingProtocol.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPStrayLightCoeffsProtocol.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPStrayLightCoeffsProtocol.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPStrobeLampProtocol.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPStrobeLampProtocol.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPTemperatureProtocol.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPTemperatureProtocol.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPThermoElectricProtocol.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPThermoElectricProtocol.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPWaveCalProtocol.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPWaveCalProtocol.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPWifiConfigurationProtocol.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPWifiConfigurationProtocol.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OceanBinaryProtocol.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OceanBinaryProtocol.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/constants/FPGARegisterCodes.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/constants/FPGARegisterCodes.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/constants/OpCodes.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/constants/OpCodes.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/FPGARegisterReadExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/FPGARegisterReadExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/FPGARegisterWriteExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/FPGARegisterWriteExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/FPGASpectrumExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/FPGASpectrumExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/FlameNIRSpectrumExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/FlameNIRSpectrumExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/HRFPGASpectrumExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/HRFPGASpectrumExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/IntegrationTimeExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/IntegrationTimeExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/JazSpectrumExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/JazSpectrumExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/MayaProSpectrumExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/MayaProSpectrumExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/NIRQuestSpectrumExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/NIRQuestSpectrumExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/OOI2KSpectrumExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/OOI2KSpectrumExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/OOIIrradCalExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/OOIIrradCalExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/OOIReadIrradCalExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/OOIReadIrradCalExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/OOIWriteIrradCalExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/OOIWriteIrradCalExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/QESpectrumExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/QESpectrumExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/ReadEEPROMSlotExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/ReadEEPROMSlotExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/ReadSpectrumExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/ReadSpectrumExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/ReadTECQETemperatureExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/ReadTECQETemperatureExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/ReadTECTemperatureExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/ReadTECTemperatureExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/RequestSpectrumExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/RequestSpectrumExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/StrobeEnableExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/StrobeEnableExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/TECEnableExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/TECEnableExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/TECQEEnableExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/TECQEEnableExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/TriggerModeExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/TriggerModeExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/USBFPGASpectrumExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/USBFPGASpectrumExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/WriteEEPROMSlotExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/WriteEEPROMSlotExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/WriteTECQESetPointExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/WriteTECQESetPointExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/WriteTECSetPointExchange.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/WriteTECSetPointExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/hints/ControlHint.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/hints/ControlHint.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/hints/SpectrumHint.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/hints/SpectrumHint.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/impls/FPGARegisterProtocol.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/impls/FPGARegisterProtocol.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/impls/OOIEEPROMProtocol.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/impls/OOIEEPROMProtocol.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/impls/OOIIrradCalProtocol.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/impls/OOIIrradCalProtocol.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/impls/OOIProtocol.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/impls/OOIProtocol.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/impls/OOISpectrometerProtocol.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/impls/OOISpectrometerProtocol.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/impls/OOIStrobeLampProtocol.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/impls/OOIStrobeLampProtocol.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/impls/OOITECProtocol.cpp` & `seabreeze-2.2.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/impls/OOITECProtocol.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/seabreeze/__init__.py` & `seabreeze-2.2.0/src/seabreeze/__init__.py`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/seabreeze/_cli.py` & `seabreeze-2.2.0/src/seabreeze/_cli.py`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/seabreeze/backends.py` & `seabreeze-2.2.0/src/seabreeze/backends.py`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/seabreeze/cseabreeze/__init__.py` & `seabreeze-2.2.0/src/seabreeze/cseabreeze/__init__.py`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/seabreeze/cseabreeze/c_seabreeze.pxd` & `seabreeze-2.2.0/src/seabreeze/cseabreeze/c_seabreeze.pxd`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/seabreeze/cseabreeze/c_seabreeze_wrapper.pyx` & `seabreeze-2.2.0/src/seabreeze/cseabreeze/c_seabreeze_wrapper.pyx`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/seabreeze/os_setup.py` & `seabreeze-2.2.0/src/seabreeze/os_setup.py`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/seabreeze/pyseabreeze/__init__.py` & `seabreeze-2.2.0/src/seabreeze/pyseabreeze/__init__.py`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/seabreeze/pyseabreeze/api.py` & `seabreeze-2.2.0/src/seabreeze/pyseabreeze/api.py`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/seabreeze/pyseabreeze/config.py` & `seabreeze-2.2.0/src/seabreeze/pyseabreeze/config.py`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/seabreeze/pyseabreeze/devices.py` & `seabreeze-2.2.0/src/seabreeze/pyseabreeze/devices.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from typing import Tuple
 from typing import TypeVar
 
 from seabreeze.pyseabreeze import features as sbf
 from seabreeze.pyseabreeze.exceptions import SeaBreezeError
 from seabreeze.pyseabreeze.features import SeaBreezeFeature
 from seabreeze.pyseabreeze.protocol import ADCProtocol
+from seabreeze.pyseabreeze.protocol import OBP2Protocol
 from seabreeze.pyseabreeze.protocol import OBPProtocol
 from seabreeze.pyseabreeze.protocol import OOIProtocol
 from seabreeze.pyseabreeze.transport import USBTransport
 from seabreeze.pyseabreeze.types import PySeaBreezeTransport
 from seabreeze.types import SeaBreezeFeatureAccessor
 
 # class registry for all spectrometer models
@@ -410,14 +411,18 @@
         except RuntimeError:
             raise SeaBreezeError("device not open")
 
         if isinstance(protocol, OOIProtocol) or isinstance(protocol, ADCProtocol):
             # The serial is stored in slot 0
             return self.f.eeprom.eeprom_read_slot(0)
 
+        elif isinstance(protocol, OBP2Protocol):
+            serial_str = protocol.query(0x00000100).strip()
+            return serial_str.decode("utf8")
+
         elif isinstance(protocol, OBPProtocol):
             serial_len = ord(protocol.query(0x00000101))
             serial_str = protocol.query(0x00000100)[:serial_len]
             return serial_str.decode("utf8")
 
         else:
             raise NotImplementedError(
@@ -477,14 +482,15 @@
 # ========================
 #
 class USB2000PLUS(SeaBreezeDevice):
     model_name = "USB2000PLUS"
 
     # communication config
     transport = (USBTransport,)
+    usb_vendor_id = 0x2457
     usb_product_id = 0x101E
     usb_endpoint_map = EndPointMap(
         ep_out=0x01, lowspeed_in=0x81, highspeed_in=0x82, highspeed_in2=0x86
     )
     usb_protocol = OOIProtocol
 
     # spectrometer config
@@ -554,14 +560,15 @@
 
 
 class USB2000(SeaBreezeDevice):
     model_name = "USB2000"
 
     # communication config
     transport = (USBTransport,)
+    usb_vendor_id = 0x2457
     usb_product_id = 0x1002
     usb_endpoint_map = EndPointMap(ep_out=0x02, lowspeed_in=0x87, highspeed_in=0x82)
     usb_protocol = OOIProtocol
 
     # spectrometer config
     dark_pixel_indices = DarkPixelIndices.from_ranges((2, 24))
     integration_time_min = 3000
@@ -581,14 +588,15 @@
 
 
 class HR2000(SeaBreezeDevice):
     model_name = "HR2000"
 
     # communication config
     transport = (USBTransport,)
+    usb_vendor_id = 0x2457
     usb_product_id = 0x100A
     usb_endpoint_map = EndPointMap(ep_out=0x02, lowspeed_in=0x87, highspeed_in=0x82)
     usb_protocol = OOIProtocol
 
     # spectrometer config
     dark_pixel_indices = DarkPixelIndices.from_ranges((2, 24))
     integration_time_min = 3000
@@ -608,14 +616,15 @@
 
 
 class HR4000(SeaBreezeDevice):
     model_name = "HR4000"
 
     # communication config
     transport = (USBTransport,)
+    usb_vendor_id = 0x2457
     usb_product_id = 0x1012
     usb_endpoint_map = EndPointMap(
         ep_out=0x01, lowspeed_in=0x81, highspeed_in=0x82, highspeed_in2=0x86
     )
     usb_protocol = OOIProtocol
 
     # spectrometer config
@@ -639,14 +648,15 @@
 
 
 class HR2000PLUS(SeaBreezeDevice):
     model_name = "HR2000PLUS"
 
     # communication config
     transport = (USBTransport,)
+    usb_vendor_id = 0x2457
     usb_product_id = 0x1016
     usb_endpoint_map = EndPointMap(
         ep_out=0x01, lowspeed_in=0x81, highspeed_in=0x82, highspeed_in2=0x86
     )
     usb_protocol = OOIProtocol
 
     # spectrometer config
@@ -670,14 +680,15 @@
 
 
 class USB650(SeaBreezeDevice):
     model_name = "USB650"
 
     # communication config
     transport = (USBTransport,)
+    usb_vendor_id = 0x2457
     usb_product_id = 0x1014
     usb_endpoint_map = EndPointMap(ep_out=0x02, lowspeed_in=0x87, highspeed_in=0x82)
     usb_protocol = OOIProtocol
 
     # spectrometer config
     dark_pixel_indices = DarkPixelIndices.from_ranges()
     integration_time_min = 3000
@@ -698,14 +709,15 @@
 
 
 class QE65000(SeaBreezeDevice):
     model_name = "QE65000"
 
     # communication config
     transport = (USBTransport,)
+    usb_vendor_id = 0x2457
     usb_product_id = 0x1018
     usb_endpoint_map = EndPointMap(
         ep_out=0x01, lowspeed_in=0x81, highspeed_in=0x82, highspeed_in2=0x86
     )
     usb_protocol = OOIProtocol
 
     # spectrometer config
@@ -729,14 +741,15 @@
 
 
 class USB4000(SeaBreezeDevice):
     model_name = "USB4000"
 
     # communication config
     transport = (USBTransport,)
+    usb_vendor_id = 0x2457
     usb_product_id = 0x1022
     usb_endpoint_map = EndPointMap(
         ep_out=0x01, lowspeed_in=0x81, highspeed_in=0x82, highspeed_in2=0x86
     )
     usb_protocol = OOIProtocol
 
     # spectrometer config
@@ -762,14 +775,15 @@
 
 
 class NIRQUEST512(SeaBreezeDevice):
     model_name = "NIRQUEST512"
 
     # communication config
     transport = (USBTransport,)
+    usb_vendor_id = 0x2457
     usb_product_id = 0x1026
     usb_endpoint_map = EndPointMap(
         ep_out=0x01, lowspeed_in=0x81, highspeed_in=0x82, highspeed_in2=0x86
     )
     usb_protocol = OOIProtocol
 
     # spectrometer config
@@ -793,14 +807,15 @@
 
 
 class NIRQUEST256(SeaBreezeDevice):
     model_name = "NIRQUEST256"
 
     # communication config
     transport = (USBTransport,)
+    usb_vendor_id = 0x2457
     usb_product_id = 0x1028
     usb_endpoint_map = EndPointMap(
         ep_out=0x01, lowspeed_in=0x81, highspeed_in=0x82, highspeed_in2=0x86
     )
     usb_protocol = OOIProtocol
 
     # spectrometer config
@@ -824,14 +839,15 @@
 
 
 class MAYA2000PRO(SeaBreezeDevice):
     model_name = "MAYA2000PRO"
 
     # communication config
     transport = (USBTransport,)
+    usb_vendor_id = 0x2457
     usb_product_id = 0x102A
     usb_endpoint_map = EndPointMap(
         ep_out=0x01, lowspeed_in=0x81, highspeed_in=0x82, highspeed_in2=0x86
     )
     usb_protocol = OOIProtocol
 
     # spectrometer config
@@ -855,14 +871,15 @@
 
 
 class MAYA2000(SeaBreezeDevice):
     model_name = "MAYA2000"
 
     # communication config
     transport = (USBTransport,)
+    usb_vendor_id = 0x2457
     usb_product_id = 0x102C
     usb_endpoint_map = EndPointMap(
         ep_out=0x01, lowspeed_in=0x81, highspeed_in=0x82, highspeed_in2=0x86
     )
     usb_protocol = OOIProtocol
 
     # spectrometer config
@@ -884,14 +901,15 @@
 
 
 class TORUS(SeaBreezeDevice):
     model_name = "TORUS"
 
     # communication config
     transport = (USBTransport,)
+    usb_vendor_id = 0x2457
     usb_product_id = 0x1040
     usb_endpoint_map = EndPointMap(
         ep_out=0x01, lowspeed_in=0x81, highspeed_in=0x82, highspeed_in2=0x86
     )
     usb_protocol = OOIProtocol
 
     # spectrometer config
@@ -915,14 +933,15 @@
 
 
 class APEX(SeaBreezeDevice):
     model_name = "APEX"
 
     # communication config
     transport = (USBTransport,)
+    usb_vendor_id = 0x2457
     usb_product_id = 0x1044
     usb_endpoint_map = EndPointMap(
         ep_out=0x01, lowspeed_in=0x81, highspeed_in=0x82, highspeed_in2=0x86
     )
     usb_protocol = OOIProtocol
 
     # spectrometer config
@@ -946,14 +965,15 @@
 
 
 class MAYALSL(SeaBreezeDevice):
     model_name = "MAYALSL"
 
     # communication config
     transport = (USBTransport,)
+    usb_vendor_id = 0x2457
     usb_product_id = 0x1046
     usb_endpoint_map = EndPointMap(
         ep_out=0x01, lowspeed_in=0x81, highspeed_in=0x82, highspeed_in2=0x86
     )
     usb_protocol = OOIProtocol
 
     # spectrometer config
@@ -977,14 +997,15 @@
 
 
 class JAZ(SeaBreezeDevice):
     model_name = "JAZ"
 
     # communication config
     transport = (USBTransport,)
+    usb_vendor_id = 0x2457
     usb_product_id = 0x2000
     usb_endpoint_map = EndPointMap(ep_out=0x01, lowspeed_in=0x81, highspeed_in=0x82)
     usb_protocol = OOIProtocol
 
     # spectrometer config
     dark_pixel_indices = DarkPixelIndices.from_ranges((2, 24))
     integration_time_min = 1000
@@ -1006,14 +1027,15 @@
 
 
 class STS(SeaBreezeDevice):
     model_name = "STS"
 
     # communication config
     transport = (USBTransport,)
+    usb_vendor_id = 0x2457
     usb_product_id = 0x4000
     usb_endpoint_map = EndPointMap(
         ep_out=0x01, lowspeed_in=0x81
     )  # XXX: we'll ignore the alternative EPs
     usb_protocol = OBPProtocol
 
     # spectrometer config
@@ -1034,14 +1056,15 @@
 
 
 class QEPRO(SeaBreezeDevice):
     model_name = "QEPRO"
 
     # communication config
     transport = (USBTransport,)
+    usb_vendor_id = 0x2457
     usb_product_id = 0x4004
     usb_endpoint_map = EndPointMap(
         ep_out=0x01, lowspeed_in=0x81
     )  # XXX: we'll ignore the alternative EPs
     usb_protocol = OBPProtocol
 
     # spectrometer config
@@ -1062,14 +1085,15 @@
 
 
 class VENTANA(SeaBreezeDevice):
     model_name = "VENTANA"
 
     # communication config
     transport = (USBTransport,)
+    usb_vendor_id = 0x2457
     usb_product_id = 0x5000
     usb_endpoint_map = EndPointMap(ep_out=0x01, lowspeed_in=0x82)
     usb_protocol = OBPProtocol
 
     # spectrometer config
     dark_pixel_indices = DarkPixelIndices.from_ranges()
     integration_time_min = 22000
@@ -1088,14 +1112,15 @@
 
 
 class SPARK(SeaBreezeDevice):
     model_name = "SPARK"
 
     # communication config
     transport = (USBTransport,)
+    usb_vendor_id = 0x2457
     usb_product_id = 0x4200
     usb_endpoint_map = EndPointMap(
         ep_out=0x01, lowspeed_in=0x81
     )  # XXX: we'll ignore the alternative EPs
     usb_protocol = OBPProtocol
 
     # spectrometer config
@@ -1116,14 +1141,15 @@
 
 
 class HDX(SeaBreezeDevice):
     model_name = "HDX"
 
     # communication config
     transport = (USBTransport,)
+    usb_vendor_id = 0x2457
     usb_product_id = 0x2003
     usb_endpoint_map = EndPointMap(
         ep_out=0x01, lowspeed_in=0x81, highspeed_in=0x82, highspeed_in2=0x86
     )
     usb_protocol = OBPProtocol
 
     # spectrometer config
@@ -1147,14 +1173,15 @@
 
 
 class ADC1000USB(SeaBreezeDevice):
     model_name = "ADC1000-USB"
 
     # communication config
     transport = (USBTransport,)
+    usb_vendor_id = 0x2457
     usb_product_id = 0x1004
     usb_endpoint_map = EndPointMap(ep_out=0x02, lowspeed_in=0x87, highspeed_in=0x82)
     usb_protocol = ADCProtocol
 
     # spectrometer config
     dark_pixel_indices = DarkPixelIndices.from_ranges((2, 24))
     integration_time_min = 5000
@@ -1169,7 +1196,31 @@
 
     # features
     feature_classes = (
         sbf.eeprom.SeaBreezeEEPromFeatureADC,
         sbf.spectrometer.SeaBreezeSpectrometerFeatureADC,
         sbf.rawusb.SeaBreezeRawUSBBusAccessFeature,
     )
+
+
+class SR4(SeaBreezeDevice):
+    model_name = "SR4"
+
+    # communication config
+    transport = (USBTransport,)
+    usb_vendor_id = 0x0999
+    usb_product_id = 0x1002
+    usb_endpoint_map = EndPointMap(ep_out=0x01, highspeed_in=0x81)
+    usb_protocol = OBP2Protocol
+
+    # spectrometer config
+    dark_pixel_indices = DarkPixelIndices.from_ranges()
+    integration_time_min = 6000  # ???
+    integration_time_max = 10000000  # ???
+    integration_time_base = 1
+    spectrum_num_pixel = 3648
+    spectrum_raw_length = (3648 * 2) + 32  # XXX: Metadata
+    spectrum_max_value = 65535
+    trigger_modes = TriggerMode.supported("OBP_NORMAL")
+
+    # features
+    feature_classes = (sbf.spectrometer.SeaBreezeSpectrometerFeatureSR4,)
```

### Comparing `seabreeze-2.1.0/src/seabreeze/pyseabreeze/features/__init__.py` & `seabreeze-2.2.0/src/seabreeze/pyseabreeze/features/__init__.py`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/seabreeze/pyseabreeze/features/_base.py` & `seabreeze-2.2.0/src/seabreeze/pyseabreeze/features/_base.py`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/seabreeze/pyseabreeze/features/acquisitiondelay.py` & `seabreeze-2.2.0/src/seabreeze/pyseabreeze/features/acquisitiondelay.py`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/seabreeze/pyseabreeze/features/continuousstrobe.py` & `seabreeze-2.2.0/src/seabreeze/pyseabreeze/features/continuousstrobe.py`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/seabreeze/pyseabreeze/features/databuffer.py` & `seabreeze-2.2.0/src/seabreeze/pyseabreeze/features/databuffer.py`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/seabreeze/pyseabreeze/features/dhcpserver.py` & `seabreeze-2.2.0/src/seabreeze/pyseabreeze/features/dhcpserver.py`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/seabreeze/pyseabreeze/features/eeprom.py` & `seabreeze-2.2.0/src/seabreeze/pyseabreeze/features/eeprom.py`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/seabreeze/pyseabreeze/features/ethernetconfiguration.py` & `seabreeze-2.2.0/src/seabreeze/pyseabreeze/features/ethernetconfiguration.py`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/seabreeze/pyseabreeze/features/fastbuffer.py` & `seabreeze-2.2.0/src/seabreeze/pyseabreeze/features/fastbuffer.py`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/seabreeze/pyseabreeze/features/fpga.py` & `seabreeze-2.2.0/src/seabreeze/pyseabreeze/features/fpga.py`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/seabreeze/pyseabreeze/features/gpio.py` & `seabreeze-2.2.0/src/seabreeze/pyseabreeze/features/gpio.py`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/seabreeze/pyseabreeze/features/i2cmaster.py` & `seabreeze-2.2.0/src/seabreeze/pyseabreeze/features/i2cmaster.py`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/seabreeze/pyseabreeze/features/introspection.py` & `seabreeze-2.2.0/src/seabreeze/pyseabreeze/features/introspection.py`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/seabreeze/pyseabreeze/features/ipv4.py` & `seabreeze-2.2.0/src/seabreeze/pyseabreeze/features/ipv4.py`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/seabreeze/pyseabreeze/features/irradcal.py` & `seabreeze-2.2.0/src/seabreeze/pyseabreeze/features/irradcal.py`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/seabreeze/pyseabreeze/features/lightsource.py` & `seabreeze-2.2.0/src/seabreeze/pyseabreeze/features/lightsource.py`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/seabreeze/pyseabreeze/features/multicast.py` & `seabreeze-2.2.0/src/seabreeze/pyseabreeze/features/multicast.py`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/seabreeze/pyseabreeze/features/networkconfiguration.py` & `seabreeze-2.2.0/src/seabreeze/pyseabreeze/features/networkconfiguration.py`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/seabreeze/pyseabreeze/features/nonlinearity.py` & `seabreeze-2.2.0/src/seabreeze/pyseabreeze/features/nonlinearity.py`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/seabreeze/pyseabreeze/features/opticalbench.py` & `seabreeze-2.2.0/src/seabreeze/pyseabreeze/features/opticalbench.py`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/seabreeze/pyseabreeze/features/pixelbinning.py` & `seabreeze-2.2.0/src/seabreeze/pyseabreeze/features/pixelbinning.py`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/seabreeze/pyseabreeze/features/rawusb.py` & `seabreeze-2.2.0/src/seabreeze/pyseabreeze/features/rawusb.py`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/seabreeze/pyseabreeze/features/spectrometer.py` & `seabreeze-2.2.0/src/seabreeze/pyseabreeze/features/spectrometer.py`

 * *Files 2% similar despite different names*

```diff
@@ -623,7 +623,51 @@
         N_raw = self._spectrum_raw_length - 1
         N_pix = self._spectrum_length
         idx = [(i // 2) % 64 + (i % 2) * 64 + (i // 128) * 128 for i in range(N_raw)]
         tsorted = tmp[idx]
         ret = numpy.array(struct.unpack("<" + "H" * N_pix, tsorted), dtype=numpy.double)
         # sorted and parsed
         return ret * self._normalization_value
+
+
+class SeaBreezeSpectrometerFeatureSR4(SeaBreezeSpectrometerFeatureOBP):
+    def _get_spectrum_raw(self) -> NDArray[np.uint8]:
+        timeout = int(
+            self._integration_time_max * 1e-3
+            + self.protocol.transport.default_timeout_ms
+        )
+        datastring = self.protocol.query(0x000_01C_00, timeout_ms=timeout)
+        return numpy.frombuffer(datastring, dtype=numpy.uint8)  # type: ignore
+
+    def get_intensities(self) -> NDArray[np.float_]:
+        tmp = self._get_spectrum_raw()
+        # 32byte metadata block at beginning
+        ret = numpy.array(
+            struct.unpack("<" + "H" * self._spectrum_length, tmp[32:]),
+            dtype=numpy.double,
+        )
+        return ret * self._normalization_value
+
+    def set_trigger_mode(self, mode: int) -> None:
+        if mode in self._trigger_modes:
+            self.protocol.send(0x000_00D_01, mode, request_ack=True)
+        else:
+            raise SeaBreezeError("Only supports: %s" % str(self._trigger_modes))
+
+    def set_integration_time_micros(self, integration_time_micros: int) -> None:
+        t_min = self._integration_time_min
+        t_max = self._integration_time_max
+        if t_min <= integration_time_micros < t_max:
+            i_time = int(integration_time_micros / self._integration_time_base)
+            self.protocol.send(0x000_00C_01, i_time)
+        else:
+            raise SeaBreezeError(f"Integration not in [{t_min:d}, {t_max:d}]")
+
+    def get_wavelengths(self) -> NDArray[np.float_]:
+        data = self.protocol.query(0x000_011_00)
+        num_coeffs = len(data) // 4
+        assert len(data) % 4 == 0  # ???
+        assert num_coeffs > 1  # ???
+        coeffs = struct.unpack("<" + "f" * num_coeffs, data)[1:]
+        # and generate the wavelength array
+        indices = numpy.arange(self._spectrum_length, dtype=numpy.float64)
+        return sum(wl * (indices**i) for i, wl in enumerate(coeffs))  # type: ignore
```

### Comparing `seabreeze-2.1.0/src/seabreeze/pyseabreeze/features/spectrumprocessing.py` & `seabreeze-2.2.0/src/seabreeze/pyseabreeze/features/spectrumprocessing.py`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/seabreeze/pyseabreeze/features/temperature.py` & `seabreeze-2.2.0/src/seabreeze/pyseabreeze/features/temperature.py`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/seabreeze/pyseabreeze/features/thermoelectric.py` & `seabreeze-2.2.0/src/seabreeze/pyseabreeze/features/thermoelectric.py`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/seabreeze/pyseabreeze/features/wificonfiguration.py` & `seabreeze-2.2.0/src/seabreeze/pyseabreeze/features/wificonfiguration.py`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/seabreeze/pyseabreeze/protocol.py` & `seabreeze-2.2.0/src/seabreeze/pyseabreeze/protocol.py`

 * *Files 3% similar despite different names*

```diff
@@ -146,14 +146,74 @@
         data:
             data returned from the spectrometer
         """
         self.send(msg_type, payload, timeout_ms=timeout_ms)
         return self.receive(size=size, timeout_ms=timeout_ms, mode=mode, **kwargs)
 
 
+class _OBP:
+    """All relevant constants are stored here"""
+
+    HEADER_START_BYTES = 0xC0C1
+    HEADER_PROTOCOL_VERSION = 0x1100  # XXX: seems to be the newest protocol version
+
+    FLAG_RESPONSE_TO_REQUEST = 0x0001
+    FLAG_ACK = 0x0002
+    FLAG_REQUEST_ACK = 0x0004
+    FLAG_NACK = 0x0008
+    FLAG_HW_EXCEPTION = 0x0010
+    FLAG_PROTOCOL_DEPRECATED = 0x0020
+
+    ERROR_CODES = {
+        0: "Success (no detectable errors)",
+        1: "Invalid/unsupported protocol",
+        2: "Unknown message type",
+        3: "Bad checksum",
+        4: "Message too large",
+        5: "Payload length does not match message type",
+        6: "Payload data invalid",
+        7: "Device not ready for given message type",
+        8: "Unknown checksum type",
+        9: "Device reset unexpectedly",
+        10: "Too many buses (Commands have come from too many bus interfaces)",
+        11: "Out of memory. Failed to allocate enough space to complete request.",
+        12: "Command is valid, but desired information does not exist.",
+        13: "Int Device Error. May be unrecoverable.",
+        100: "Could not decrypt properly",
+        101: "Firmware layout invalid",
+        102: "Data packet was wrong size",
+        103: "hardware revision not compatible with firmware",
+        104: "Existing flash map not compatible with firmware",
+        255: "Operation/Response Deferred. Will take some time. Do not ACK or NACK yet.",
+    }
+
+    NO_ERROR = 0x0000
+    RESERVED = b""
+    CHECKSUM_TYPE_NONE = 0x00
+    CHECKSUM_TYPE_MD5 = 0x01
+    NO_CHECKSUM = b""
+    FOOTER = 0xC2C3C4C5  # the datasheet specifies it in this order...
+
+    HEADER_FMT = (
+        "<H"  # start_bytes
+        "H"  # protocol_version
+        "H"  # flags
+        "H"  # error number
+        "L"  # message type
+        "L"  # regarding
+        "6s"  # reserved
+        "B"  # checksum type
+        "B"  # immediate length
+        "16s"  # immediate data
+        "L"  # bytes remaining
+    )
+
+    FOOTER_FMT = "16s" "L"  # checksum  # footer
+
+
 class OBPProtocol(PySeaBreezeProtocol):
     msgs = {
         code: struct.Struct(msg).pack
         for code, msg in {
             0x00000100: "",  # GET_SERIAL
             0x00000101: "",  # GET_SERIAL_LENGTH
             0x00100928: "",  # GET_BUF_SPEC32_META
@@ -167,72 +227,15 @@
             0x00181101: "<B",  # GET_NL_COEFF
             0x00420004: "",  # GET_TE_TEMPERATURE
             0x00420010: "<B",  # SET_TE_ENABLE
             0x00420011: "<f",  # SET_TE_SETPOINT
         }.items()
     }  # add more here if you implement new features
 
-    class OBP:
-        """All relevant constants are stored here"""
-
-        HEADER_START_BYTES = 0xC0C1
-        HEADER_PROTOCOL_VERSION = 0x1100  # XXX: seems to be the newest protocol version
-
-        FLAG_RESPONSE_TO_REQUEST = 0x0001
-        FLAG_ACK = 0x0002
-        FLAG_REQUEST_ACK = 0x0004
-        FLAG_NACK = 0x0008
-        FLAG_HW_EXCEPTION = 0x0010
-        FLAG_PROTOCOL_DEPRECATED = 0x0020
-
-        ERROR_CODES = {
-            0: "Success (no detectable errors)",
-            1: "Invalid/unsupported protocol",
-            2: "Unknown message type",
-            3: "Bad checksum",
-            4: "Message too large",
-            5: "Payload length does not match message type",
-            6: "Payload data invalid",
-            7: "Device not ready for given message type",
-            8: "Unknown checksum type",
-            9: "Device reset unexpectedly",
-            10: "Too many buses (Commands have come from too many bus interfaces)",
-            11: "Out of memory. Failed to allocate enough space to complete request.",
-            12: "Command is valid, but desired information does not exist.",
-            13: "Int Device Error. May be unrecoverable.",
-            100: "Could not decrypt properly",
-            101: "Firmware layout invalid",
-            102: "Data packet was wrong size",
-            103: "hardware revision not compatible with firmware",
-            104: "Existing flash map not compatible with firmware",
-            255: "Operation/Response Deferred. Will take some time. Do not ACK or NACK yet.",
-        }
-
-        NO_ERROR = 0x0000
-        RESERVED = b""
-        CHECKSUM_TYPE_NONE = 0x00
-        CHECKSUM_TYPE_MD5 = 0x01
-        NO_CHECKSUM = b""
-        FOOTER = 0xC2C3C4C5  # the datasheet specifies it in this order...
-
-        HEADER_FMT = (
-            "<H"  # start_bytes
-            "H"  # protocol_version
-            "H"  # flags
-            "H"  # error number
-            "L"  # message type
-            "L"  # regarding
-            "6s"  # reserved
-            "B"  # checksum type
-            "B"  # immediate length
-            "16s"  # immediate data
-            "L"  # bytes remaining
-        )
-
-        FOOTER_FMT = "16s" "L"  # checksum  # footer
+    OBP = _OBP
 
     # noinspection DuplicatedCode
     def send(
         self,
         msg_type: int,
         payload: tuple[int | str | float, ...] | str | int | float = (),
         timeout_ms: int | None = None,
@@ -315,15 +318,15 @@
             ignored and only present to provide compatible caller interfaces
 
         Returns
         -------
         data : str
             data returned from the spectrometer
         """
-        response = self.transport.read(size=64, timeout_ms=timeout_ms)
+        response = self.transport.read(size=None, timeout_ms=timeout_ms)
         try:
             remaining_bytes, checksum_type = self._check_incoming_message_header(
                 response[:44]
             )
         except SeaBreezeError:
             # empty buffer if error raised
             self.transport.read(size=None, timeout_ms=500)
@@ -449,15 +452,20 @@
             bytes_remaining,
             payload_string,
             self.OBP.NO_CHECKSUM,
             self.OBP.FOOTER,
         )
         return msg
 
-    def _check_incoming_message_header(self, header: bytes) -> tuple[int, int]:
+    def _check_incoming_message_header(
+        self,
+        header: bytes,
+        *,
+        _raw: bool = False,
+    ) -> tuple[int, int]:
         """check the incoming message header
 
         Parameters
         ----------
         header:
             a obp header of length 44
 
@@ -471,17 +479,23 @@
             raise SeaBreezeError(
                 "header has wrong length! len(header): %d" % len(header)
             )
 
         data = struct.unpack(self.OBP.HEADER_FMT, header)
 
         if data[0] != self.OBP.HEADER_START_BYTES and config.obp_protocol_checks:
-            raise SeaBreezeError('Header start_bytes wrong: "%d"' % data[0])
+            if _raw:
+                warnings.warn(f"Header start_bytes wrong: 0x{data[0]:04x}")
+            else:
+                raise SeaBreezeError('Header start_bytes wrong: "%d"' % data[0])
         if data[1] != self.OBP.HEADER_PROTOCOL_VERSION and config.obp_protocol_checks:
-            raise SeaBreezeError("Header protocol version wrong: %d" % data[1])
+            if _raw:
+                warnings.warn(f"Header protocol version wrong: 0x{data[1]:04x}")
+            else:
+                raise SeaBreezeError("Header protocol version wrong: %d" % data[1])
 
         flags = data[2]
         if flags == 0:
             pass
         if flags & self.OBP.FLAG_RESPONSE_TO_REQUEST:
             pass  # TODO: propagate?
         if flags & self.OBP.FLAG_ACK:
@@ -511,14 +525,17 @@
         ):
             raise SeaBreezeError('the checksum type is unknown: "%d"' % checksum_type)
 
         # immediate_length = data[8]
         # immediate_data = data[9]
         bytes_remaining = data[10]
 
+        if _raw:
+            return data  # type: ignore
+
         return bytes_remaining, checksum_type
 
     def _check_incoming_message_footer(self, footer: bytes) -> bytes:
         """check the incoming message header
 
         Parameters
         ----------
@@ -576,14 +593,34 @@
             return immediate_data[:immediate_length]
         elif payload_length > 0:
             return payload
         else:
             return b""
 
 
+class _OBP2(_OBP):
+    HEADER_PROTOCOL_VERSION = 0x2000
+
+
+class OBP2Protocol(OBPProtocol):
+    msgs = {
+        code: struct.Struct(msg).pack
+        for code, msg in {
+            0x000_001_00: "",  # GET_SERIAL
+            0x000_001_01: "",  # GET_SERIAL_LENGTH  ??? not sure if this works
+            0x000_01C_00: "",  # GET_SPECTRUM ???
+            0x000_00C_01: "<L",  # SET_ITIME_USEC
+            0x000_00D_01: "<B",  # SET_TRIG_MODE
+            0x000_011_00: "",  # GET_WL_COEFFS
+        }.items()
+    }  # add more here if you implement new features
+
+    OBP = _OBP2
+
+
 class ADCProtocol(PySeaBreezeProtocol):
     msgs = {
         code: functools.partial(struct.Struct(msg).pack, code)
         for code, msg in {
             0x01: "<B",  # Reset
             0x02: "<BH",  # Set Integration Time
             0x03: "<BH",  # Set Strobe Enable Status
```

### Comparing `seabreeze-2.1.0/src/seabreeze/pyseabreeze/transport.py` & `seabreeze-2.2.0/src/seabreeze/pyseabreeze/transport.py`

 * *Files 7% similar despite different names*

```diff
@@ -90,43 +90,52 @@
             self.close()
         self.pyusb_device = None
 
 
 class USBTransport(PySeaBreezeTransport[USBTransportHandle]):
     """implementation of the usb transport interface for spectrometers"""
 
-    _required_init_kwargs = ("usb_product_id", "usb_endpoint_map", "usb_protocol")
-    vendor_id = 0x2457
-    product_ids: dict[int, str] = {}
+    _required_init_kwargs = (
+        "usb_vendor_id",
+        "usb_product_id",
+        "usb_endpoint_map",
+        "usb_protocol",
+    )
+    vendor_product_ids: dict[tuple[int, int], str] = {}
 
     # add logging
     _log = logging.getLogger(__name__)
 
     def __init__(
         self,
+        usb_vendor_id: int,
         usb_product_id: int,
         usb_endpoint_map: EndPointMap,
         usb_protocol: type[PySeaBreezeProtocol],
     ) -> None:
         super().__init__()
+        self._vendor_id = usb_vendor_id
         self._product_id = usb_product_id
         self._endpoint_map = usb_endpoint_map
         self._protocol_cls = usb_protocol
         # internal settings
         self._default_read_size = {
             "low_speed": 64,
             "high_speed": 512,
             "high_speed_alt": 512,
         }
         self._read_endpoints = {
             "low_speed": "lowspeed_in",
             "high_speed": "highspeed_in",
             "high_speed_alt": "highspeed_in2",
         }
-        self._default_read_endpoint = "low_speed"
+        if self._endpoint_map.lowspeed_in is not None:
+            self._default_read_endpoint = "low_speed"
+        else:
+            self._default_read_endpoint = "high_speed"
         self._default_read_spectrum_endpoint = "high_speed"
         # internal state
         self._device: USBTransportHandle | None = None
         self._opened: bool | None = None
         self._protocol: PySeaBreezeProtocol | None = None
 
     def open_device(self, device: USBTransportHandle) -> None:
@@ -223,45 +232,52 @@
         # check if a specific pyusb backend is requested
         _pyusb_backend = kwargs.get("pyusb_backend", None)
         # get all matching devices
         try:
             pyusb_devices = usb.core.find(
                 find_all=True,
                 custom_match=lambda dev: (
-                    dev.idVendor == cls.vendor_id and dev.idProduct in cls.product_ids
+                    (dev.idVendor, dev.idProduct) in cls.vendor_product_ids
                 ),
                 backend=get_pyusb_backend_from_name(name=_pyusb_backend),
             )
         except usb.core.NoBackendError:
             raise RuntimeError("No pyusb backend found")
         # encapsulate
         for pyusb_device in pyusb_devices:
             yield USBTransportHandle(pyusb_device)
 
     @classmethod
     def register_model(cls, model_name: str, **kwargs: Any) -> None:
+        vendor_id = kwargs.get("usb_vendor_id")
+        if not isinstance(vendor_id, int):
+            raise TypeError(f"vendor_id {vendor_id:r} not an integer")
         product_id = kwargs.get("usb_product_id")
         if not isinstance(product_id, int):
             raise TypeError(f"product_id {product_id:r} not an integer")
-        if product_id in cls.product_ids:
-            raise ValueError(f"product_id 0x{product_id:04x} already in registry")
-        cls.product_ids[product_id] = model_name
+        if (vendor_id, product_id) in cls.vendor_product_ids:
+            raise ValueError(
+                f"vendor_id:product_id {vendor_id:04x}:{product_id:04x} already in registry"
+            )
+        cls.vendor_product_ids[(vendor_id, product_id)] = model_name
 
     @classmethod
     def supported_model(cls, device: USBTransportHandle) -> str | None:
         """return supported model
 
         Parameters
         ----------
         device : USBTransportHandle
         """
         if not isinstance(device, USBTransportHandle):
             return None
         # noinspection PyUnresolvedReferences
-        return cls.product_ids[device.pyusb_device.idProduct]
+        return cls.vendor_product_ids[
+            (device.pyusb_device.idVendor, device.pyusb_device.idProduct)
+        ]
 
     @classmethod
     def specialize(cls, model_name: str, **kwargs: Any) -> type[USBTransport]:
         assert set(kwargs) == set(cls._required_init_kwargs)
         # usb transport register automatically on registration
         cls.register_model(model_name, **kwargs)
         specialized_class = type(
```

### Comparing `seabreeze-2.1.0/src/seabreeze/pyseabreeze/types.py` & `seabreeze-2.2.0/src/seabreeze/pyseabreeze/types.py`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/seabreeze/spectrometers.py` & `seabreeze-2.2.0/src/seabreeze/spectrometers.py`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/seabreeze/types.py` & `seabreeze-2.2.0/src/seabreeze/types.py`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/src/seabreeze.egg-info/PKG-INFO` & `seabreeze-2.2.0/src/seabreeze.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seabreeze
-Version: 2.1.0
+Version: 2.2.0
 Summary: Python interface module for Ocean Optics spectrometers. This software is not associated with Ocean Optics. Use it at your own risk.
 Home-page: https://github.com/ap--/python-seabreeze
 Author: Andreas Poehlmann
 Author-email: andreas@poehlmann.io
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `seabreeze-2.1.0/src/seabreeze.egg-info/SOURCES.txt` & `seabreeze-2.2.0/src/seabreeze.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 LICENSE.md
 MANIFEST.in
 README.md
 pyproject.toml
 pytest.ini
 requirements-dev.txt
 setup.py
+dev/pretty_print_obp_pcapng.py
 docs/Makefile
 docs/environment.yml
 docs/source/api.rst
 docs/source/backend_api.rst
 docs/source/conf.py
 docs/source/contributing.rst
 docs/source/index.rst
```

### Comparing `seabreeze-2.1.0/tests/conftest.py` & `seabreeze-2.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/tests/test_backends.py` & `seabreeze-2.2.0/tests/test_backends.py`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/tests/test_protocol.py` & `seabreeze-2.2.0/tests/test_protocol.py`

 * *Files identical despite different names*

### Comparing `seabreeze-2.1.0/tests/test_spectrometers.py` & `seabreeze-2.2.0/tests/test_spectrometers.py`

 * *Files identical despite different names*

