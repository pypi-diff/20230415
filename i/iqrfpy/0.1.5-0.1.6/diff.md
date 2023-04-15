# Comparing `tmp/iqrfpy-0.1.5.tar.gz` & `tmp/iqrfpy-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iqrfpy-0.1.5.tar", last modified: Fri Apr  7 16:12:51 2023, max compression
+gzip compressed data, was "iqrfpy-0.1.6.tar", last modified: Sat Apr 15 08:21:22 2023, max compression
```

## Comparing `iqrfpy-0.1.5.tar` & `iqrfpy-0.1.6.tar`

### file list

```diff
@@ -1,194 +1,198 @@
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.686399 iqrfpy-0.1.5/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      309 2023-03-12 10:44:36.000000 iqrfpy-0.1.5/.editorconfig
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      113 2023-03-27 06:23:13.000000 iqrfpy-0.1.5/.gitignore
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      937 2023-03-22 19:16:00.000000 iqrfpy-0.1.5/.gitlab-ci.yml
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      203 2023-03-22 19:16:00.000000 iqrfpy-0.1.5/.pylintrc
--rw-rw-r--   0 khanak    (1000) khanak    (1000)    11346 2023-03-24 07:47:59.000000 iqrfpy-0.1.5/LICENSE
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      663 2023-03-25 07:04:37.000000 iqrfpy-0.1.5/Makefile
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      859 2023-04-07 16:12:51.686399 iqrfpy-0.1.5/PKG-INFO
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        9 2023-03-07 12:47:49.000000 iqrfpy-0.1.5/README.md
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      671 2023-04-06 07:28:51.000000 iqrfpy-0.1.5/example.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.678399 iqrfpy-0.1.5/examples/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2081 2023-03-25 07:08:59.000000 iqrfpy-0.1.5/examples/response_factories.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.678399 iqrfpy-0.1.5/iqrfpy/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)       44 2023-04-07 16:12:26.000000 iqrfpy-0.1.5/iqrfpy/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.682399 iqrfpy-0.1.5/iqrfpy/enums/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     5379 2023-03-24 10:38:31.000000 iqrfpy-0.1.5/iqrfpy/enums/Commands.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4646 2023-03-24 10:31:05.000000 iqrfpy-0.1.5/iqrfpy/enums/MessageTypes.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)       90 2023-03-24 10:27:58.000000 iqrfpy-0.1.5/iqrfpy/enums/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      708 2023-03-24 10:49:19.000000 iqrfpy-0.1.5/iqrfpy/enums/peripherals.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4173 2023-04-07 15:58:03.000000 iqrfpy-0.1.5/iqrfpy/exceptions.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.682399 iqrfpy-0.1.5/iqrfpy/messages/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)       61 2023-03-24 07:14:54.000000 iqrfpy-0.1.5/iqrfpy/messages/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.682399 iqrfpy-0.1.5/iqrfpy/messages/requests/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2370 2023-04-07 15:07:14.000000 iqrfpy-0.1.5/iqrfpy/messages/requests/IRequest.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-08 11:54:48.000000 iqrfpy-0.1.5/iqrfpy/messages/requests/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.682399 iqrfpy-0.1.5/iqrfpy/messages/requests/binaryoutput/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:45:27.000000 iqrfpy-0.1.5/iqrfpy/messages/requests/binaryoutput/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.682399 iqrfpy-0.1.5/iqrfpy/messages/requests/coordinator/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      988 2023-03-24 10:31:41.000000 iqrfpy-0.1.5/iqrfpy/messages/requests/coordinator/AddrInfo.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2617 2023-04-07 15:11:45.000000 iqrfpy-0.1.5/iqrfpy/messages/requests/coordinator/AuthorizeBond.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1521 2023-04-07 15:13:22.000000 iqrfpy-0.1.5/iqrfpy/messages/requests/coordinator/Backup.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2268 2023-04-07 15:14:15.000000 iqrfpy-0.1.5/iqrfpy/messages/requests/coordinator/BondNode.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1008 2023-03-24 10:31:41.000000 iqrfpy-0.1.5/iqrfpy/messages/requests/coordinator/BondedDevices.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1010 2023-03-24 10:31:41.000000 iqrfpy-0.1.5/iqrfpy/messages/requests/coordinator/ClearAllBonds.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1024 2023-03-24 10:31:41.000000 iqrfpy-0.1.5/iqrfpy/messages/requests/coordinator/DiscoveredDevices.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1922 2023-04-07 15:14:51.000000 iqrfpy-0.1.5/iqrfpy/messages/requests/coordinator/Discovery.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1593 2023-04-07 15:15:04.000000 iqrfpy-0.1.5/iqrfpy/messages/requests/coordinator/RemoveBond.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1778 2023-04-07 15:15:27.000000 iqrfpy-0.1.5/iqrfpy/messages/requests/coordinator/Restore.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1429 2023-04-07 15:16:51.000000 iqrfpy-0.1.5/iqrfpy/messages/requests/coordinator/SetDpaParams.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2116 2023-04-07 15:17:08.000000 iqrfpy-0.1.5/iqrfpy/messages/requests/coordinator/SetHops.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2022 2023-04-07 15:17:22.000000 iqrfpy-0.1.5/iqrfpy/messages/requests/coordinator/SetMID.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4922 2023-04-07 15:18:37.000000 iqrfpy-0.1.5/iqrfpy/messages/requests/coordinator/SmartConnect.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      955 2023-03-16 15:28:35.000000 iqrfpy-0.1.5/iqrfpy/messages/requests/coordinator/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.682399 iqrfpy-0.1.5/iqrfpy/messages/requests/dali/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:45:18.000000 iqrfpy-0.1.5/iqrfpy/messages/requests/dali/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.682399 iqrfpy-0.1.5/iqrfpy/messages/requests/eeeprom/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:43:26.000000 iqrfpy-0.1.5/iqrfpy/messages/requests/eeeprom/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.682399 iqrfpy-0.1.5/iqrfpy/messages/requests/eeprom/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:43:21.000000 iqrfpy-0.1.5/iqrfpy/messages/requests/eeprom/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.682399 iqrfpy-0.1.5/iqrfpy/messages/requests/exploration/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-14 15:30:10.000000 iqrfpy-0.1.5/iqrfpy/messages/requests/exploration/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.682399 iqrfpy-0.1.5/iqrfpy/messages/requests/frc/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:44:40.000000 iqrfpy-0.1.5/iqrfpy/messages/requests/frc/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.682399 iqrfpy-0.1.5/iqrfpy/messages/requests/generic/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-14 15:30:10.000000 iqrfpy-0.1.5/iqrfpy/messages/requests/generic/Raw.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-14 15:30:10.000000 iqrfpy-0.1.5/iqrfpy/messages/requests/generic/RawHdp.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-14 15:30:10.000000 iqrfpy-0.1.5/iqrfpy/messages/requests/generic/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.682399 iqrfpy-0.1.5/iqrfpy/messages/requests/io/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:44:21.000000 iqrfpy-0.1.5/iqrfpy/messages/requests/io/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.682399 iqrfpy-0.1.5/iqrfpy/messages/requests/ledg/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:44:15.000000 iqrfpy-0.1.5/iqrfpy/messages/requests/ledg/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.682399 iqrfpy-0.1.5/iqrfpy/messages/requests/ledr/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:44:11.000000 iqrfpy-0.1.5/iqrfpy/messages/requests/ledr/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.682399 iqrfpy-0.1.5/iqrfpy/messages/requests/light/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:45:37.000000 iqrfpy-0.1.5/iqrfpy/messages/requests/light/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.682399 iqrfpy-0.1.5/iqrfpy/messages/requests/node/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      949 2023-03-24 10:31:41.000000 iqrfpy-0.1.5/iqrfpy/messages/requests/node/Read.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:41:43.000000 iqrfpy-0.1.5/iqrfpy/messages/requests/node/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.682399 iqrfpy-0.1.5/iqrfpy/messages/requests/os/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:43:14.000000 iqrfpy-0.1.5/iqrfpy/messages/requests/os/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.682399 iqrfpy-0.1.5/iqrfpy/messages/requests/ram/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:43:31.000000 iqrfpy-0.1.5/iqrfpy/messages/requests/ram/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.682399 iqrfpy-0.1.5/iqrfpy/messages/requests/sensor/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:45:31.000000 iqrfpy-0.1.5/iqrfpy/messages/requests/sensor/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.682399 iqrfpy-0.1.5/iqrfpy/messages/requests/thermometer/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:44:27.000000 iqrfpy-0.1.5/iqrfpy/messages/requests/thermometer/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.682399 iqrfpy-0.1.5/iqrfpy/messages/requests/uart/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:44:32.000000 iqrfpy-0.1.5/iqrfpy/messages/requests/uart/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     8216 2023-04-07 15:00:59.000000 iqrfpy-0.1.5/iqrfpy/messages/response_factory.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.682399 iqrfpy-0.1.5/iqrfpy/messages/responses/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2202 2023-03-24 12:37:34.000000 iqrfpy-0.1.5/iqrfpy/messages/responses/AsyncResponse.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2074 2023-04-07 15:36:21.000000 iqrfpy-0.1.5/iqrfpy/messages/responses/Confirmation.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3269 2023-04-07 15:34:42.000000 iqrfpy-0.1.5/iqrfpy/messages/responses/IResponse.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-17 10:12:06.000000 iqrfpy-0.1.5/iqrfpy/messages/responses/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.682399 iqrfpy-0.1.5/iqrfpy/messages/responses/binaryoutput/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:08:04.000000 iqrfpy-0.1.5/iqrfpy/messages/responses/binaryoutput/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.682399 iqrfpy-0.1.5/iqrfpy/messages/responses/coordinator/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2238 2023-04-07 15:21:57.000000 iqrfpy-0.1.5/iqrfpy/messages/responses/coordinator/AddrInfo.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2323 2023-04-07 15:23:07.000000 iqrfpy-0.1.5/iqrfpy/messages/responses/coordinator/AuthorizeBond.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2169 2023-04-07 15:23:36.000000 iqrfpy-0.1.5/iqrfpy/messages/responses/coordinator/Backup.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2283 2023-04-07 15:24:18.000000 iqrfpy-0.1.5/iqrfpy/messages/responses/coordinator/BondNode.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2230 2023-04-07 15:23:59.000000 iqrfpy-0.1.5/iqrfpy/messages/responses/coordinator/BondedDevices.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1902 2023-04-07 15:24:33.000000 iqrfpy-0.1.5/iqrfpy/messages/responses/coordinator/ClearAllBonds.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2286 2023-04-07 15:24:47.000000 iqrfpy-0.1.5/iqrfpy/messages/responses/coordinator/DiscoveredDevices.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2143 2023-04-07 15:25:03.000000 iqrfpy-0.1.5/iqrfpy/messages/responses/coordinator/Discovery.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2147 2023-04-07 15:25:14.000000 iqrfpy-0.1.5/iqrfpy/messages/responses/coordinator/RemoveBond.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1777 2023-04-07 15:25:30.000000 iqrfpy-0.1.5/iqrfpy/messages/responses/coordinator/Restore.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2287 2023-04-07 15:26:28.000000 iqrfpy-0.1.5/iqrfpy/messages/responses/coordinator/SetDpaParams.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2335 2023-04-07 15:26:40.000000 iqrfpy-0.1.5/iqrfpy/messages/responses/coordinator/SetHops.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1771 2023-04-07 15:26:51.000000 iqrfpy-0.1.5/iqrfpy/messages/responses/coordinator/SetMID.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2315 2023-04-07 15:27:01.000000 iqrfpy-0.1.5/iqrfpy/messages/responses/coordinator/SmartConnect.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      983 2023-03-24 07:27:46.000000 iqrfpy-0.1.5/iqrfpy/messages/responses/coordinator/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.682399 iqrfpy-0.1.5/iqrfpy/messages/responses/dali/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:07:58.000000 iqrfpy-0.1.5/iqrfpy/messages/responses/dali/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.682399 iqrfpy-0.1.5/iqrfpy/messages/responses/eeeprom/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:07:01.000000 iqrfpy-0.1.5/iqrfpy/messages/responses/eeeprom/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.682399 iqrfpy-0.1.5/iqrfpy/messages/responses/eeprom/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:06:56.000000 iqrfpy-0.1.5/iqrfpy/messages/responses/eeprom/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.682399 iqrfpy-0.1.5/iqrfpy/messages/responses/frc/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:07:43.000000 iqrfpy-0.1.5/iqrfpy/messages/responses/frc/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.682399 iqrfpy-0.1.5/iqrfpy/messages/responses/io/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:07:27.000000 iqrfpy-0.1.5/iqrfpy/messages/responses/io/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.686399 iqrfpy-0.1.5/iqrfpy/messages/responses/ledg/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:07:23.000000 iqrfpy-0.1.5/iqrfpy/messages/responses/ledg/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.686399 iqrfpy-0.1.5/iqrfpy/messages/responses/ledr/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:07:19.000000 iqrfpy-0.1.5/iqrfpy/messages/responses/ledr/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.686399 iqrfpy-0.1.5/iqrfpy/messages/responses/light/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:08:14.000000 iqrfpy-0.1.5/iqrfpy/messages/responses/light/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.686399 iqrfpy-0.1.5/iqrfpy/messages/responses/node/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2578 2023-04-07 15:29:01.000000 iqrfpy-0.1.5/iqrfpy/messages/responses/node/Read.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:06:49.000000 iqrfpy-0.1.5/iqrfpy/messages/responses/node/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.686399 iqrfpy-0.1.5/iqrfpy/messages/responses/os/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:06:52.000000 iqrfpy-0.1.5/iqrfpy/messages/responses/os/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.686399 iqrfpy-0.1.5/iqrfpy/messages/responses/ram/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:07:05.000000 iqrfpy-0.1.5/iqrfpy/messages/responses/ram/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.686399 iqrfpy-0.1.5/iqrfpy/messages/responses/sensor/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:08:09.000000 iqrfpy-0.1.5/iqrfpy/messages/responses/sensor/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.686399 iqrfpy-0.1.5/iqrfpy/messages/responses/thermometer/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:07:32.000000 iqrfpy-0.1.5/iqrfpy/messages/responses/thermometer/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.686399 iqrfpy-0.1.5/iqrfpy/messages/responses/uart/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:07:37.000000 iqrfpy-0.1.5/iqrfpy/messages/responses/uart/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.686399 iqrfpy-0.1.5/iqrfpy/transports/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      300 2023-03-22 19:16:00.000000 iqrfpy-0.1.5/iqrfpy/transports/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2133 2023-04-06 09:43:24.000000 iqrfpy-0.1.5/iqrfpy/transports/itransport.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2076 2023-03-24 09:57:48.000000 iqrfpy-0.1.5/iqrfpy/transports/mqtt_transport.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3788 2023-03-24 09:57:48.000000 iqrfpy-0.1.5/iqrfpy/transports/udp_transport.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.686399 iqrfpy-0.1.5/iqrfpy/utils/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)       50 2023-03-24 11:33:36.000000 iqrfpy-0.1.5/iqrfpy/utils/__init__.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)    20336 2023-04-07 15:58:34.000000 iqrfpy-0.1.5/iqrfpy/utils/common.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      343 2023-03-24 11:01:36.000000 iqrfpy-0.1.5/iqrfpy/utils/enums.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.682399 iqrfpy-0.1.5/iqrfpy.egg-info/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      859 2023-04-07 16:12:51.000000 iqrfpy-0.1.5/iqrfpy.egg-info/PKG-INFO
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     6112 2023-04-07 16:12:51.000000 iqrfpy-0.1.5/iqrfpy.egg-info/SOURCES.txt
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        1 2023-04-07 16:12:51.000000 iqrfpy-0.1.5/iqrfpy.egg-info/dependency_links.txt
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      159 2023-04-07 16:12:51.000000 iqrfpy-0.1.5/iqrfpy.egg-info/requires.txt
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        7 2023-04-07 16:12:51.000000 iqrfpy-0.1.5/iqrfpy.egg-info/top_level.txt
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      138 2023-03-24 09:25:00.000000 iqrfpy-0.1.5/pyproject.toml
--rw-rw-r--   0 khanak    (1000) khanak    (1000)       85 2023-03-24 07:40:43.000000 iqrfpy-0.1.5/requirements.txt
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1162 2023-04-07 16:12:51.686399 iqrfpy-0.1.5/setup.cfg
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      102 2023-03-22 19:16:00.000000 iqrfpy-0.1.5/test_requirements.txt
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.686399 iqrfpy-0.1.5/tests/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-07 12:49:34.000000 iqrfpy-0.1.5/tests/__init__.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.686399 iqrfpy-0.1.5/tests/enums/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1241 2023-03-24 10:31:41.000000 iqrfpy-0.1.5/tests/enums/Peripherals_test.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.686399 iqrfpy-0.1.5/tests/messages/
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.686399 iqrfpy-0.1.5/tests/messages/requests/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1292 2023-03-18 09:19:32.000000 iqrfpy-0.1.5/tests/messages/requests/IRequest_test.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.686399 iqrfpy-0.1.5/tests/messages/requests/coordinator/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      869 2023-03-18 09:24:49.000000 iqrfpy-0.1.5/tests/messages/requests/coordinator/AddrInfoRequest_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4015 2023-04-02 10:26:13.000000 iqrfpy-0.1.5/tests/messages/requests/coordinator/AuthorizeBondRequest_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2194 2023-03-18 09:44:00.000000 iqrfpy-0.1.5/tests/messages/requests/coordinator/BackupRequest_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3758 2023-03-18 09:50:37.000000 iqrfpy-0.1.5/tests/messages/requests/coordinator/BondNodeRequest_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      903 2023-03-18 09:24:46.000000 iqrfpy-0.1.5/tests/messages/requests/coordinator/BondedDevicesRequest_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      904 2023-03-18 09:57:38.000000 iqrfpy-0.1.5/tests/messages/requests/coordinator/ClearAllBondsRequest_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)      925 2023-03-18 09:59:43.000000 iqrfpy-0.1.5/tests/messages/requests/coordinator/DiscoveredDevicesRequest_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3445 2023-03-18 10:11:35.000000 iqrfpy-0.1.5/tests/messages/requests/coordinator/DiscoveryRequest_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2322 2023-03-18 10:17:19.000000 iqrfpy-0.1.5/tests/messages/requests/coordinator/RemoveBondRequest_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4241 2023-03-18 10:45:18.000000 iqrfpy-0.1.5/tests/messages/requests/coordinator/RestoreRequest_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2257 2023-03-18 10:55:51.000000 iqrfpy-0.1.5/tests/messages/requests/coordinator/SetDpaParamsRequest_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3672 2023-03-18 11:08:56.000000 iqrfpy-0.1.5/tests/messages/requests/coordinator/SetHopsRequest_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3511 2023-03-18 11:37:09.000000 iqrfpy-0.1.5/tests/messages/requests/coordinator/SetMIDRequest_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)    11030 2023-03-19 07:20:25.000000 iqrfpy-0.1.5/tests/messages/requests/coordinator/SmartConnectRequest_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4826 2023-04-07 16:08:13.000000 iqrfpy-0.1.5/tests/messages/response_factory_test.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.686399 iqrfpy-0.1.5/tests/messages/responses/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     2161 2023-03-24 10:31:41.000000 iqrfpy-0.1.5/tests/messages/responses/AsyncResponse_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     1280 2023-03-24 12:50:58.000000 iqrfpy-0.1.5/tests/messages/responses/Confirmation_test.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.686399 iqrfpy-0.1.5/tests/messages/responses/coordinator/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4324 2023-03-24 10:31:41.000000 iqrfpy-0.1.5/tests/messages/responses/coordinator/AddrInfoResponse_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4513 2023-04-02 10:41:56.000000 iqrfpy-0.1.5/tests/messages/responses/coordinator/AuthorizeBondResponse_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4764 2023-03-24 10:31:41.000000 iqrfpy-0.1.5/tests/messages/responses/coordinator/BackupResponse_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4390 2023-03-24 10:31:41.000000 iqrfpy-0.1.5/tests/messages/responses/coordinator/BondNodeResponse_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4211 2023-03-24 10:31:41.000000 iqrfpy-0.1.5/tests/messages/responses/coordinator/BondedDevicesResponse_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3154 2023-03-24 10:31:41.000000 iqrfpy-0.1.5/tests/messages/responses/coordinator/ClearAllBondsResponse_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4343 2023-03-24 10:31:41.000000 iqrfpy-0.1.5/tests/messages/responses/coordinator/DiscoveredDevicesResponse_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3784 2023-03-24 10:31:41.000000 iqrfpy-0.1.5/tests/messages/responses/coordinator/DiscoveryResponse_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3794 2023-03-24 10:31:41.000000 iqrfpy-0.1.5/tests/messages/responses/coordinator/RemoveNodeResponse_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3054 2023-03-24 10:31:41.000000 iqrfpy-0.1.5/tests/messages/responses/coordinator/RestoreResponse_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3930 2023-03-24 10:31:41.000000 iqrfpy-0.1.5/tests/messages/responses/coordinator/SetDpaParamsResponse_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4490 2023-03-24 10:31:41.000000 iqrfpy-0.1.5/tests/messages/responses/coordinator/SetHopsResponse_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     3052 2023-03-24 10:31:41.000000 iqrfpy-0.1.5/tests/messages/responses/coordinator/SetMIDResponse_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)     4486 2023-03-24 10:47:04.000000 iqrfpy-0.1.5/tests/messages/responses/coordinator/SmartConnectResponse_test.py
-drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-07 16:12:51.686399 iqrfpy-0.1.5/tests/utils/
--rw-rw-r--   0 khanak    (1000) khanak    (1000)    16222 2023-04-07 16:02:36.000000 iqrfpy-0.1.5/tests/utils/Common_test.py
--rw-rw-r--   0 khanak    (1000) khanak    (1000)       78 2023-03-22 19:16:00.000000 iqrfpy-0.1.5/tox.ini
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.231226 iqrfpy-0.1.6/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      309 2023-03-12 10:44:36.000000 iqrfpy-0.1.6/.editorconfig
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      113 2023-03-27 06:23:13.000000 iqrfpy-0.1.6/.gitignore
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      937 2023-03-22 19:16:00.000000 iqrfpy-0.1.6/.gitlab-ci.yml
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      203 2023-03-22 19:16:00.000000 iqrfpy-0.1.6/.pylintrc
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)    11346 2023-03-24 07:47:59.000000 iqrfpy-0.1.6/LICENSE
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      699 2023-04-15 05:33:58.000000 iqrfpy-0.1.6/Makefile
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      859 2023-04-15 08:21:22.231226 iqrfpy-0.1.6/PKG-INFO
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        9 2023-03-07 12:47:49.000000 iqrfpy-0.1.6/README.md
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.223226 iqrfpy-0.1.6/examples/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2081 2023-03-25 07:08:59.000000 iqrfpy-0.1.6/examples/response_factories.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.223226 iqrfpy-0.1.6/iqrfpy/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      111 2023-04-15 08:21:05.000000 iqrfpy-0.1.6/iqrfpy/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.227226 iqrfpy-0.1.6/iqrfpy/enums/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)       90 2023-03-24 10:27:58.000000 iqrfpy-0.1.6/iqrfpy/enums/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     5379 2023-03-24 10:38:31.000000 iqrfpy-0.1.6/iqrfpy/enums/commands.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4646 2023-03-24 10:31:05.000000 iqrfpy-0.1.6/iqrfpy/enums/message_types.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      708 2023-03-24 10:49:19.000000 iqrfpy-0.1.6/iqrfpy/enums/peripherals.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4173 2023-04-07 15:58:03.000000 iqrfpy-0.1.6/iqrfpy/exceptions.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.227226 iqrfpy-0.1.6/iqrfpy/messages/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)       61 2023-03-24 07:14:54.000000 iqrfpy-0.1.6/iqrfpy/messages/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.227226 iqrfpy-0.1.6/iqrfpy/messages/requests/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2454 2023-04-15 07:42:07.000000 iqrfpy-0.1.6/iqrfpy/messages/requests/IRequest.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      184 2023-04-15 05:52:25.000000 iqrfpy-0.1.6/iqrfpy/messages/requests/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.227226 iqrfpy-0.1.6/iqrfpy/messages/requests/binaryoutput/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:45:27.000000 iqrfpy-0.1.6/iqrfpy/messages/requests/binaryoutput/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.227226 iqrfpy-0.1.6/iqrfpy/messages/requests/coordinator/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1024 2023-04-15 07:16:20.000000 iqrfpy-0.1.6/iqrfpy/messages/requests/coordinator/AddrInfo.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2730 2023-04-15 07:17:50.000000 iqrfpy-0.1.6/iqrfpy/messages/requests/coordinator/AuthorizeBond.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1595 2023-04-15 07:21:20.000000 iqrfpy-0.1.6/iqrfpy/messages/requests/coordinator/Backup.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2400 2023-04-15 07:23:56.000000 iqrfpy-0.1.6/iqrfpy/messages/requests/coordinator/BondNode.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1044 2023-04-15 07:22:26.000000 iqrfpy-0.1.6/iqrfpy/messages/requests/coordinator/BondedDevices.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1046 2023-04-15 07:24:16.000000 iqrfpy-0.1.6/iqrfpy/messages/requests/coordinator/ClearAllBonds.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1060 2023-04-15 07:24:30.000000 iqrfpy-0.1.6/iqrfpy/messages/requests/coordinator/DiscoveredDevices.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2044 2023-04-15 07:26:04.000000 iqrfpy-0.1.6/iqrfpy/messages/requests/coordinator/Discovery.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1677 2023-04-15 07:26:47.000000 iqrfpy-0.1.6/iqrfpy/messages/requests/coordinator/RemoveBond.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1879 2023-04-15 07:28:01.000000 iqrfpy-0.1.6/iqrfpy/messages/requests/coordinator/Restore.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1465 2023-04-15 07:28:26.000000 iqrfpy-0.1.6/iqrfpy/messages/requests/coordinator/SetDpaParams.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2389 2023-04-15 08:13:58.000000 iqrfpy-0.1.6/iqrfpy/messages/requests/coordinator/SetHops.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2135 2023-04-15 07:33:11.000000 iqrfpy-0.1.6/iqrfpy/messages/requests/coordinator/SetMID.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     5293 2023-04-15 07:39:44.000000 iqrfpy-0.1.6/iqrfpy/messages/requests/coordinator/SmartConnect.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      955 2023-03-16 15:28:35.000000 iqrfpy-0.1.6/iqrfpy/messages/requests/coordinator/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.227226 iqrfpy-0.1.6/iqrfpy/messages/requests/dali/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:45:18.000000 iqrfpy-0.1.6/iqrfpy/messages/requests/dali/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.227226 iqrfpy-0.1.6/iqrfpy/messages/requests/eeeprom/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:43:26.000000 iqrfpy-0.1.6/iqrfpy/messages/requests/eeeprom/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.227226 iqrfpy-0.1.6/iqrfpy/messages/requests/eeprom/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:43:21.000000 iqrfpy-0.1.6/iqrfpy/messages/requests/eeprom/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.227226 iqrfpy-0.1.6/iqrfpy/messages/requests/exploration/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-14 15:30:10.000000 iqrfpy-0.1.6/iqrfpy/messages/requests/exploration/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.227226 iqrfpy-0.1.6/iqrfpy/messages/requests/frc/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:44:40.000000 iqrfpy-0.1.6/iqrfpy/messages/requests/frc/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.227226 iqrfpy-0.1.6/iqrfpy/messages/requests/generic/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-14 15:30:10.000000 iqrfpy-0.1.6/iqrfpy/messages/requests/generic/Raw.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-14 15:30:10.000000 iqrfpy-0.1.6/iqrfpy/messages/requests/generic/RawHdp.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-14 15:30:10.000000 iqrfpy-0.1.6/iqrfpy/messages/requests/generic/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.227226 iqrfpy-0.1.6/iqrfpy/messages/requests/io/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:44:21.000000 iqrfpy-0.1.6/iqrfpy/messages/requests/io/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.227226 iqrfpy-0.1.6/iqrfpy/messages/requests/ledg/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:44:15.000000 iqrfpy-0.1.6/iqrfpy/messages/requests/ledg/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.227226 iqrfpy-0.1.6/iqrfpy/messages/requests/ledr/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:44:11.000000 iqrfpy-0.1.6/iqrfpy/messages/requests/ledr/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.227226 iqrfpy-0.1.6/iqrfpy/messages/requests/light/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:45:37.000000 iqrfpy-0.1.6/iqrfpy/messages/requests/light/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.227226 iqrfpy-0.1.6/iqrfpy/messages/requests/node/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      957 2023-04-15 07:43:28.000000 iqrfpy-0.1.6/iqrfpy/messages/requests/node/Read.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:41:43.000000 iqrfpy-0.1.6/iqrfpy/messages/requests/node/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.227226 iqrfpy-0.1.6/iqrfpy/messages/requests/os/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:43:14.000000 iqrfpy-0.1.6/iqrfpy/messages/requests/os/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.227226 iqrfpy-0.1.6/iqrfpy/messages/requests/ram/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:43:31.000000 iqrfpy-0.1.6/iqrfpy/messages/requests/ram/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.227226 iqrfpy-0.1.6/iqrfpy/messages/requests/sensor/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:45:31.000000 iqrfpy-0.1.6/iqrfpy/messages/requests/sensor/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.227226 iqrfpy-0.1.6/iqrfpy/messages/requests/thermometer/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:44:27.000000 iqrfpy-0.1.6/iqrfpy/messages/requests/thermometer/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.227226 iqrfpy-0.1.6/iqrfpy/messages/requests/uart/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 09:44:32.000000 iqrfpy-0.1.6/iqrfpy/messages/requests/uart/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     8383 2023-04-15 07:00:07.000000 iqrfpy-0.1.6/iqrfpy/messages/response_factory.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.227226 iqrfpy-0.1.6/iqrfpy/messages/responses/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2735 2023-04-15 08:08:05.000000 iqrfpy-0.1.6/iqrfpy/messages/responses/AsyncResponse.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2484 2023-04-15 08:09:36.000000 iqrfpy-0.1.6/iqrfpy/messages/responses/Confirmation.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3277 2023-04-15 08:09:43.000000 iqrfpy-0.1.6/iqrfpy/messages/responses/IResponse.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      214 2023-04-15 05:57:36.000000 iqrfpy-0.1.6/iqrfpy/messages/responses/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.227226 iqrfpy-0.1.6/iqrfpy/messages/responses/binaryoutput/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:08:04.000000 iqrfpy-0.1.6/iqrfpy/messages/responses/binaryoutput/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.227226 iqrfpy-0.1.6/iqrfpy/messages/responses/coordinator/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2548 2023-04-15 07:49:09.000000 iqrfpy-0.1.6/iqrfpy/messages/responses/coordinator/AddrInfo.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2659 2023-04-15 07:51:29.000000 iqrfpy-0.1.6/iqrfpy/messages/responses/coordinator/AuthorizeBond.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2468 2023-04-15 07:52:33.000000 iqrfpy-0.1.6/iqrfpy/messages/responses/coordinator/Backup.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2582 2023-04-15 07:55:01.000000 iqrfpy-0.1.6/iqrfpy/messages/responses/coordinator/BondNode.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2567 2023-04-15 07:54:09.000000 iqrfpy-0.1.6/iqrfpy/messages/responses/coordinator/BondedDevices.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2231 2023-04-15 07:56:16.000000 iqrfpy-0.1.6/iqrfpy/messages/responses/coordinator/ClearAllBonds.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2627 2023-04-15 07:57:08.000000 iqrfpy-0.1.6/iqrfpy/messages/responses/coordinator/DiscoveredDevices.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2475 2023-04-15 07:58:02.000000 iqrfpy-0.1.6/iqrfpy/messages/responses/coordinator/Discovery.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2480 2023-04-15 07:58:52.000000 iqrfpy-0.1.6/iqrfpy/messages/responses/coordinator/RemoveBond.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2039 2023-04-15 07:59:57.000000 iqrfpy-0.1.6/iqrfpy/messages/responses/coordinator/Restore.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2622 2023-04-15 08:01:05.000000 iqrfpy-0.1.6/iqrfpy/messages/responses/coordinator/SetDpaParams.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2634 2023-04-15 08:02:04.000000 iqrfpy-0.1.6/iqrfpy/messages/responses/coordinator/SetHops.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2033 2023-04-15 08:03:57.000000 iqrfpy-0.1.6/iqrfpy/messages/responses/coordinator/SetMID.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2650 2023-04-15 08:04:34.000000 iqrfpy-0.1.6/iqrfpy/messages/responses/coordinator/SmartConnect.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      983 2023-03-24 07:27:46.000000 iqrfpy-0.1.6/iqrfpy/messages/responses/coordinator/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.227226 iqrfpy-0.1.6/iqrfpy/messages/responses/dali/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:07:58.000000 iqrfpy-0.1.6/iqrfpy/messages/responses/dali/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.227226 iqrfpy-0.1.6/iqrfpy/messages/responses/eeeprom/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:07:01.000000 iqrfpy-0.1.6/iqrfpy/messages/responses/eeeprom/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.227226 iqrfpy-0.1.6/iqrfpy/messages/responses/eeprom/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:06:56.000000 iqrfpy-0.1.6/iqrfpy/messages/responses/eeprom/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.227226 iqrfpy-0.1.6/iqrfpy/messages/responses/exploration/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-04-15 05:56:54.000000 iqrfpy-0.1.6/iqrfpy/messages/responses/exploration/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.227226 iqrfpy-0.1.6/iqrfpy/messages/responses/frc/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:07:43.000000 iqrfpy-0.1.6/iqrfpy/messages/responses/frc/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.227226 iqrfpy-0.1.6/iqrfpy/messages/responses/generic/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-04-15 05:56:49.000000 iqrfpy-0.1.6/iqrfpy/messages/responses/generic/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.227226 iqrfpy-0.1.6/iqrfpy/messages/responses/io/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:07:27.000000 iqrfpy-0.1.6/iqrfpy/messages/responses/io/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.227226 iqrfpy-0.1.6/iqrfpy/messages/responses/ledg/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:07:23.000000 iqrfpy-0.1.6/iqrfpy/messages/responses/ledg/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.231226 iqrfpy-0.1.6/iqrfpy/messages/responses/ledr/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:07:19.000000 iqrfpy-0.1.6/iqrfpy/messages/responses/ledr/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.231226 iqrfpy-0.1.6/iqrfpy/messages/responses/light/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:08:14.000000 iqrfpy-0.1.6/iqrfpy/messages/responses/light/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.231226 iqrfpy-0.1.6/iqrfpy/messages/responses/node/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2579 2023-04-15 05:36:55.000000 iqrfpy-0.1.6/iqrfpy/messages/responses/node/Read.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:06:49.000000 iqrfpy-0.1.6/iqrfpy/messages/responses/node/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.231226 iqrfpy-0.1.6/iqrfpy/messages/responses/os/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:06:52.000000 iqrfpy-0.1.6/iqrfpy/messages/responses/os/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.231226 iqrfpy-0.1.6/iqrfpy/messages/responses/ram/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:07:05.000000 iqrfpy-0.1.6/iqrfpy/messages/responses/ram/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.231226 iqrfpy-0.1.6/iqrfpy/messages/responses/sensor/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:08:09.000000 iqrfpy-0.1.6/iqrfpy/messages/responses/sensor/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.231226 iqrfpy-0.1.6/iqrfpy/messages/responses/thermometer/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:07:32.000000 iqrfpy-0.1.6/iqrfpy/messages/responses/thermometer/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.231226 iqrfpy-0.1.6/iqrfpy/messages/responses/uart/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-11 10:07:37.000000 iqrfpy-0.1.6/iqrfpy/messages/responses/uart/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.231226 iqrfpy-0.1.6/iqrfpy/transports/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      300 2023-03-22 19:16:00.000000 iqrfpy-0.1.6/iqrfpy/transports/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2133 2023-04-06 09:43:24.000000 iqrfpy-0.1.6/iqrfpy/transports/itransport.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2076 2023-03-24 09:57:48.000000 iqrfpy-0.1.6/iqrfpy/transports/mqtt_transport.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3788 2023-03-24 09:57:48.000000 iqrfpy-0.1.6/iqrfpy/transports/udp_transport.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.231226 iqrfpy-0.1.6/iqrfpy/utils/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)       50 2023-03-24 11:33:36.000000 iqrfpy-0.1.6/iqrfpy/utils/__init__.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)    20492 2023-04-15 08:13:29.000000 iqrfpy-0.1.6/iqrfpy/utils/common.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1810 2023-04-15 07:47:59.000000 iqrfpy-0.1.6/iqrfpy/utils/dpa.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      343 2023-04-15 06:15:47.000000 iqrfpy-0.1.6/iqrfpy/utils/enums.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.223226 iqrfpy-0.1.6/iqrfpy.egg-info/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      859 2023-04-15 08:21:22.000000 iqrfpy-0.1.6/iqrfpy.egg-info/PKG-INFO
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     6218 2023-04-15 08:21:22.000000 iqrfpy-0.1.6/iqrfpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        1 2023-04-15 08:21:22.000000 iqrfpy-0.1.6/iqrfpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      159 2023-04-15 08:21:22.000000 iqrfpy-0.1.6/iqrfpy.egg-info/requires.txt
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        7 2023-04-15 08:21:22.000000 iqrfpy-0.1.6/iqrfpy.egg-info/top_level.txt
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      138 2023-03-24 09:25:00.000000 iqrfpy-0.1.6/pyproject.toml
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)       85 2023-03-24 07:40:43.000000 iqrfpy-0.1.6/requirements.txt
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1162 2023-04-15 08:21:22.231226 iqrfpy-0.1.6/setup.cfg
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      102 2023-03-22 19:16:00.000000 iqrfpy-0.1.6/test_requirements.txt
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.231226 iqrfpy-0.1.6/tests/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)        0 2023-03-07 12:49:34.000000 iqrfpy-0.1.6/tests/__init__.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.231226 iqrfpy-0.1.6/tests/enums/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1241 2023-03-24 10:31:41.000000 iqrfpy-0.1.6/tests/enums/Peripherals_test.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.231226 iqrfpy-0.1.6/tests/messages/
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.231226 iqrfpy-0.1.6/tests/messages/requests/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1292 2023-03-18 09:19:32.000000 iqrfpy-0.1.6/tests/messages/requests/IRequest_test.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.231226 iqrfpy-0.1.6/tests/messages/requests/coordinator/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      869 2023-03-18 09:24:49.000000 iqrfpy-0.1.6/tests/messages/requests/coordinator/AddrInfoRequest_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4015 2023-04-02 10:26:13.000000 iqrfpy-0.1.6/tests/messages/requests/coordinator/AuthorizeBondRequest_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2194 2023-03-18 09:44:00.000000 iqrfpy-0.1.6/tests/messages/requests/coordinator/BackupRequest_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3758 2023-03-18 09:50:37.000000 iqrfpy-0.1.6/tests/messages/requests/coordinator/BondNodeRequest_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      903 2023-03-18 09:24:46.000000 iqrfpy-0.1.6/tests/messages/requests/coordinator/BondedDevicesRequest_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      904 2023-03-18 09:57:38.000000 iqrfpy-0.1.6/tests/messages/requests/coordinator/ClearAllBondsRequest_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)      925 2023-03-18 09:59:43.000000 iqrfpy-0.1.6/tests/messages/requests/coordinator/DiscoveredDevicesRequest_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3445 2023-03-18 10:11:35.000000 iqrfpy-0.1.6/tests/messages/requests/coordinator/DiscoveryRequest_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2322 2023-03-18 10:17:19.000000 iqrfpy-0.1.6/tests/messages/requests/coordinator/RemoveBondRequest_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4241 2023-03-18 10:45:18.000000 iqrfpy-0.1.6/tests/messages/requests/coordinator/RestoreRequest_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2257 2023-03-18 10:55:51.000000 iqrfpy-0.1.6/tests/messages/requests/coordinator/SetDpaParamsRequest_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3672 2023-03-18 11:08:56.000000 iqrfpy-0.1.6/tests/messages/requests/coordinator/SetHopsRequest_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3511 2023-03-18 11:37:09.000000 iqrfpy-0.1.6/tests/messages/requests/coordinator/SetMIDRequest_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)    11030 2023-03-19 07:20:25.000000 iqrfpy-0.1.6/tests/messages/requests/coordinator/SmartConnectRequest_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4827 2023-04-15 05:36:55.000000 iqrfpy-0.1.6/tests/messages/response_factory_test.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.231226 iqrfpy-0.1.6/tests/messages/responses/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     2162 2023-04-15 05:36:55.000000 iqrfpy-0.1.6/tests/messages/responses/AsyncResponse_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     1280 2023-04-15 05:36:55.000000 iqrfpy-0.1.6/tests/messages/responses/Confirmation_test.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.231226 iqrfpy-0.1.6/tests/messages/responses/coordinator/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4325 2023-04-15 05:36:55.000000 iqrfpy-0.1.6/tests/messages/responses/coordinator/AddrInfoResponse_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4514 2023-04-15 05:36:55.000000 iqrfpy-0.1.6/tests/messages/responses/coordinator/AuthorizeBondResponse_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4765 2023-04-15 05:36:55.000000 iqrfpy-0.1.6/tests/messages/responses/coordinator/BackupResponse_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4391 2023-04-15 05:36:55.000000 iqrfpy-0.1.6/tests/messages/responses/coordinator/BondNodeResponse_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4212 2023-04-15 05:36:55.000000 iqrfpy-0.1.6/tests/messages/responses/coordinator/BondedDevicesResponse_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3155 2023-04-15 05:36:55.000000 iqrfpy-0.1.6/tests/messages/responses/coordinator/ClearAllBondsResponse_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4344 2023-04-15 05:36:55.000000 iqrfpy-0.1.6/tests/messages/responses/coordinator/DiscoveredDevicesResponse_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3785 2023-04-15 05:36:55.000000 iqrfpy-0.1.6/tests/messages/responses/coordinator/DiscoveryResponse_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3795 2023-04-15 05:36:55.000000 iqrfpy-0.1.6/tests/messages/responses/coordinator/RemoveNodeResponse_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3055 2023-04-15 05:36:55.000000 iqrfpy-0.1.6/tests/messages/responses/coordinator/RestoreResponse_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3931 2023-04-15 05:36:55.000000 iqrfpy-0.1.6/tests/messages/responses/coordinator/SetDpaParamsResponse_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4491 2023-04-15 05:36:55.000000 iqrfpy-0.1.6/tests/messages/responses/coordinator/SetHopsResponse_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     3053 2023-04-15 05:36:55.000000 iqrfpy-0.1.6/tests/messages/responses/coordinator/SetMIDResponse_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)     4487 2023-04-15 05:36:55.000000 iqrfpy-0.1.6/tests/messages/responses/coordinator/SmartConnectResponse_test.py
+drwxrwxr-x   0 khanak    (1000) khanak    (1000)        0 2023-04-15 08:21:22.231226 iqrfpy-0.1.6/tests/utils/
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)    16223 2023-04-15 05:36:55.000000 iqrfpy-0.1.6/tests/utils/Common_test.py
+-rw-rw-r--   0 khanak    (1000) khanak    (1000)       78 2023-03-22 19:16:00.000000 iqrfpy-0.1.6/tox.ini
```

### Comparing `iqrfpy-0.1.5/.gitlab-ci.yml` & `iqrfpy-0.1.6/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.5/LICENSE` & `iqrfpy-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.5/Makefile` & `iqrfpy-0.1.6/Makefile`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 build:
 	python3 -m pip install --upgrade build
 	python3 -m build
 
+install:
+	python3 -m pip install .
+
 upload-test:
 	python3 -m pip install --upgrade twine
 	python3 -m twine upload --repository testpypi dist/*
 
 upload:
 	python3 -m pip install --upgrade twine
 	python3 -m twine upload dist/*
```

### Comparing `iqrfpy-0.1.5/PKG-INFO` & `iqrfpy-0.1.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iqrfpy
-Version: 0.1.5
+Version: 0.1.6
 Summary: A python library for communication with IQRF Network
 Home-page: https://gitlab.iqrf.org/microrisc/libiqrf-python
 Author: Karel Hanák
 Author-email: karel.hanak@iqrf.org
 License: Apache-2.0
 Keywords: iqrf,dpa
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `iqrfpy-0.1.5/examples/response_factories.py` & `iqrfpy-0.1.6/examples/response_factories.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.5/iqrfpy/enums/Commands.py` & `iqrfpy-0.1.6/iqrfpy/enums/commands.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.5/iqrfpy/enums/MessageTypes.py` & `iqrfpy-0.1.6/iqrfpy/enums/message_types.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.5/iqrfpy/enums/peripherals.py` & `iqrfpy-0.1.6/iqrfpy/enums/peripherals.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.5/iqrfpy/exceptions.py` & `iqrfpy-0.1.6/iqrfpy/exceptions.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.5/iqrfpy/messages/requests/IRequest.py` & `iqrfpy-0.1.6/iqrfpy/messages/requests/IRequest.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 from __future__ import annotations
 from typeguard import typechecked
 from abc import ABC, abstractmethod
 from typing import List, Optional, Union
 from uuid import uuid4
-from iqrfpy.utils.common import Common
-from iqrfpy.enums.Commands import Command
-from iqrfpy.enums.MessageTypes import MessageType
+import iqrfpy.utils.dpa as DpaConstants
+from iqrfpy.enums.commands import Command
+from iqrfpy.enums.message_types import MessageType
 from iqrfpy.enums.peripherals import Peripheral
 from iqrfpy.exceptions import RequestNadrInvalidError, RequestHwpidInvalidError
 
 __all__ = ['IRequest']
 
 
 @typechecked
 class IRequest(ABC):
     __slots__ = '_nadr', '_pnum', '_pcmd', '_m_type', '_hwpid', '_pdata', '_msgid', '_params'
 
-    def __init__(self, nadr: int, pnum: Peripheral, pcmd: Command, hwpid: int = Common.HWPID_MAX,
+    def __init__(self, nadr: int, pnum: Peripheral, pcmd: Command, hwpid: int = DpaConstants.HWPID_MAX,
                  pdata: Optional[List[int]] = None, m_type: Optional[MessageType] = None, params: Optional[dict] = None,
                  msgid: str = str(uuid4())):
         self._nadr: int = nadr
         self._pnum: Peripheral = pnum
         self._pcmd: Command = pcmd
         self._hwpid: int = hwpid
         self._pdata: Optional[List[int]] = pdata
         self._m_type: Optional[str] = m_type.value if m_type is not None else m_type
         self._msgid: str = msgid
         self._params: Optional[dict] = params if params is not None else {}
         self._validate_base()
 
     def _validate_base(self) -> None:
-        if self._nadr < 0 or self._nadr > 239:
+        if self._nadr < DpaConstants.NADR_MIN or self._nadr > DpaConstants.NADR_MAX:
             raise RequestNadrInvalidError('NADR should be between 0 and 239.')
-        if self._hwpid < 0 or self._hwpid > 65535:
+        if self._hwpid < DpaConstants.HWPID_MIN or self._hwpid > DpaConstants.HWPID_MAX:
             raise RequestHwpidInvalidError('HWPID should be between 0 and 65535.')
 
     @abstractmethod
     def to_dpa(self, mutable: bool = False) -> Union[bytes, bytearray]:
         self._validate_base()
         dpa: List[int] = [0, self._nadr, self._pnum, self._pcmd, self._hwpid & 0xFF, (self._hwpid >> 8) & 0xFF]
         if self._pdata is not None:
```

### Comparing `iqrfpy-0.1.5/iqrfpy/messages/requests/coordinator/AddrInfo.py` & `iqrfpy-0.1.6/iqrfpy/messages/requests/coordinator/BondedDevices.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from __future__ import annotations
 from typeguard import typechecked
 from uuid import uuid4
 from typing import Union
-from iqrfpy.enums.Commands import CoordinatorRequestCommands
-from iqrfpy.enums.MessageTypes import CoordinatorMessages
+from iqrfpy.enums.commands import CoordinatorRequestCommands
+from iqrfpy.enums.message_types import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
-from iqrfpy.utils.common import Common
+import iqrfpy.utils.dpa as DpaConstants
 from iqrfpy.messages.requests.IRequest import IRequest
 
-__all__ = ['AddrInfoRequest']
+__all__ = ['BondedDevicesRequest']
 
 
 @typechecked
-class AddrInfoRequest(IRequest):
+class BondedDevicesRequest(IRequest):
 
-    def __init__(self, hwpid: int = Common.HWPID_MAX, msgid: str = str(uuid4())):
+    def __init__(self, hwpid: int = DpaConstants.HWPID_MAX, msgid: str = str(uuid4())):
         super().__init__(
-            nadr=0,
+            nadr=DpaConstants.COORDINATOR_NADR,
             pnum=EmbedPeripherals.COORDINATOR,
-            pcmd=CoordinatorRequestCommands.ADDR_INFO,
-            m_type=CoordinatorMessages.ADDR_INFO,
+            pcmd=CoordinatorRequestCommands.BONDED_DEVICES,
+            m_type=CoordinatorMessages.BONDED_DEVICES,
             hwpid=hwpid,
             msgid=msgid
         )
 
     def to_dpa(self, mutable: bool = False) -> Union[bytes, bytearray]:
         return super().to_dpa(mutable=mutable)
```

### Comparing `iqrfpy-0.1.5/iqrfpy/messages/requests/coordinator/AuthorizeBond.py` & `iqrfpy-0.1.6/iqrfpy/messages/requests/coordinator/AuthorizeBond.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from __future__ import annotations
 from dataclasses import dataclass
 from typeguard import typechecked
 from uuid import uuid4
 from typing import List, Union
-from iqrfpy.enums.Commands import CoordinatorRequestCommands
-from iqrfpy.enums.MessageTypes import CoordinatorMessages
+from iqrfpy.enums.commands import CoordinatorRequestCommands
+from iqrfpy.enums.message_types import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
 from iqrfpy.exceptions import RequestParameterInvalidValueError
-from iqrfpy.utils.common import Common
+import iqrfpy.utils.dpa as DpaConstants
 from iqrfpy.messages.requests.IRequest import IRequest
 
 __all__ = ['AuthorizeBondRequest', 'AuthorizeBondParams']
 
 
 @dataclass(slots=True)
 @typechecked
@@ -21,17 +21,17 @@
 
 
 @typechecked
 class AuthorizeBondRequest(IRequest):
 
     __slots__ = '_nodes'
 
-    def __init__(self, nodes: List[AuthorizeBondParams], hwpid: int = Common.HWPID_MAX, msgid: str = str(uuid4())):
+    def __init__(self, nodes: List[AuthorizeBondParams], hwpid: int = DpaConstants.HWPID_MAX, msgid: str = str(uuid4())):
         super().__init__(
-            nadr=0,
+            nadr=DpaConstants.COORDINATOR_NADR,
             pnum=EmbedPeripherals.COORDINATOR,
             pcmd=CoordinatorRequestCommands.AUTHORIZE_BOND,
             m_type=CoordinatorMessages.AUTHORIZE_BOND,
             hwpid=hwpid,
             msgid=msgid
         ),
         self._nodes: List[AuthorizeBondParams] = nodes
@@ -39,17 +39,17 @@
 
     def _validate(self) -> None:
         if len(self._nodes) == 0:
             raise RequestParameterInvalidValueError('At least one pair of requested address and MID is required.')
         if len(self._nodes) > 11:
             raise RequestParameterInvalidValueError('Request can carry at most 11 pairs of address and MID.')
         for node in self._nodes:
-            if node.reqAddr < 1 or node.reqAddr > 239:
+            if node.reqAddr < DpaConstants.NODE_NADR_MIN or node.reqAddr > DpaConstants.NODE_NADR_MAX:
                 raise RequestParameterInvalidValueError('Requested address value should be between 1 and 239.')
-            if node.mid < 0 or node.mid > 0xFFFFFFFF:
+            if node.mid < DpaConstants.MID_MIN or node.mid > DpaConstants.MID_MAX:
                 raise RequestParameterInvalidValueError('MID value should be an unsigned 32bit integer.')
 
     def set_nodes(self, nodes: List[AuthorizeBondParams]) -> None:
         self._nodes = nodes
 
     def to_dpa(self, mutable: bool = False) -> Union[bytes, bytearray]:
         self._validate()
```

### Comparing `iqrfpy-0.1.5/iqrfpy/messages/requests/coordinator/Backup.py` & `iqrfpy-0.1.6/iqrfpy/messages/requests/coordinator/Backup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 from __future__ import annotations
 from typeguard import typechecked
 from uuid import uuid4
 from typing import Union
-from iqrfpy.enums.Commands import CoordinatorRequestCommands
-from iqrfpy.enums.MessageTypes import CoordinatorMessages
+from iqrfpy.enums.commands import CoordinatorRequestCommands
+from iqrfpy.enums.message_types import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
 from iqrfpy.exceptions import RequestParameterInvalidValueError
-from iqrfpy.utils.common import Common
+import iqrfpy.utils.dpa as DpaConstants
 from iqrfpy.messages.requests.IRequest import IRequest
 
 __all__ = ['BackupRequest']
 
 
 @typechecked
 class BackupRequest(IRequest):
     __slots__ = '_index'
 
-    def __init__(self, index: int = 0, hwpid: int = Common.HWPID_MAX, msgid: str = str(uuid4())):
+    def __init__(self, index: int = 0, hwpid: int = DpaConstants.HWPID_MAX, msgid: str = str(uuid4())):
         super().__init__(
-            nadr=0,
+            nadr=DpaConstants.COORDINATOR_NADR,
             pnum=EmbedPeripherals.COORDINATOR,
             pcmd=CoordinatorRequestCommands.BACKUP,
             m_type=CoordinatorMessages.BACKUP,
             hwpid=hwpid,
             msgid=msgid
         )
         self._index = index
         self._validate()
 
     def _validate(self) -> None:
-        if self._index < 0 or self._index > 255:
+        if self._index < DpaConstants.BYTE_MIN or self._index > DpaConstants.BYTE_MAX:
             raise RequestParameterInvalidValueError('Index value should be between 0 and 255.')
 
     def set_index(self, index: int) -> None:
         self._index = index
 
     def to_dpa(self, mutable: bool = False) -> Union[bytes, bytearray]:
         self._validate()
```

### Comparing `iqrfpy-0.1.5/iqrfpy/messages/requests/coordinator/BondNode.py` & `iqrfpy-0.1.6/iqrfpy/messages/requests/coordinator/BondNode.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 from __future__ import annotations
 from typeguard import typechecked
 from uuid import uuid4
 from typing import Union
-from iqrfpy.enums.Commands import CoordinatorRequestCommands
-from iqrfpy.enums.MessageTypes import CoordinatorMessages
+from iqrfpy.enums.commands import CoordinatorRequestCommands
+from iqrfpy.enums.message_types import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
 from iqrfpy.exceptions import RequestParameterInvalidValueError
-from iqrfpy.utils.common import Common
+import iqrfpy.utils.dpa as DpaConstants
 from iqrfpy.messages.requests.IRequest import IRequest
 
 __all__ = ['BondNodeRequest']
 
 
 @typechecked
 class BondNodeRequest(IRequest):
     __slots__ = '_req_addr', '_bonding_test_retries'
 
-    def __init__(self, req_addr: int, bonding_test_retries: int, hwpid: int = Common.HWPID_MAX,
+    def __init__(self, req_addr: int, bonding_test_retries: int, hwpid: int = DpaConstants.HWPID_MAX,
                  msgid: str = str(uuid4())) -> None:
         super().__init__(
-            nadr=0,
+            nadr=DpaConstants.COORDINATOR_NADR,
             pnum=EmbedPeripherals.COORDINATOR,
             pcmd=CoordinatorRequestCommands.BOND_NODE,
             m_type=CoordinatorMessages.BOND_NODE,
             hwpid=hwpid,
             msgid=msgid
         )
         self._req_addr = req_addr
         self._bonding_test_retries = bonding_test_retries
         self._validate()
 
     def _validate(self) -> None:
-        if self._req_addr == 240 and self._bonding_test_retries == 0:
+        if self._req_addr == DpaConstants.IQUIP_NADR and self._bonding_test_retries == 0:
             return
-        if self._req_addr < 0 or self._req_addr > 239:
+        if self._req_addr < DpaConstants.NADR_MIN or self._req_addr > DpaConstants.NADR_MAX:
             raise RequestParameterInvalidValueError('Address value should be between 0 and 239. Value 240 is allowed \
             combination with bonding test retries value 0.')
-        if self._bonding_test_retries < 0 or self._bonding_test_retries > 255:
+        if self._bonding_test_retries < DpaConstants.BYTE_MIN or self._bonding_test_retries > DpaConstants.BYTE_MAX:
             raise RequestParameterInvalidValueError('Bonding test retries value should be between 0 and 255.')
 
     def set_req_addr(self, req_addr: int) -> None:
         self._req_addr = req_addr
 
     def set_bonding_test_retries(self, bonding_test_retries: int) -> None:
         self._bonding_test_retries = bonding_test_retries
```

### Comparing `iqrfpy-0.1.5/iqrfpy/messages/requests/coordinator/BondedDevices.py` & `iqrfpy-0.1.6/iqrfpy/messages/requests/coordinator/DiscoveredDevices.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from __future__ import annotations
 from typeguard import typechecked
 from uuid import uuid4
 from typing import Union
-from iqrfpy.enums.Commands import CoordinatorRequestCommands
-from iqrfpy.enums.MessageTypes import CoordinatorMessages
+from iqrfpy.enums.commands import CoordinatorRequestCommands
+from iqrfpy.enums.message_types import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
-from iqrfpy.utils.common import Common
+import iqrfpy.utils.dpa as DpaConstants
 from iqrfpy.messages.requests.IRequest import IRequest
 
-__all__ = ['BondedDevicesRequest']
+__all__ = ['DiscoveredDevicesRequest']
 
 
 @typechecked
-class BondedDevicesRequest(IRequest):
+class DiscoveredDevicesRequest(IRequest):
 
-    def __init__(self, hwpid: int = Common.HWPID_MAX, msgid: str = str(uuid4())):
+    def __init__(self, hwpid: int = DpaConstants.HWPID_MAX, msgid: str = str(uuid4())):
         super().__init__(
-            nadr=0,
+            nadr=DpaConstants.COORDINATOR_NADR,
             pnum=EmbedPeripherals.COORDINATOR,
-            pcmd=CoordinatorRequestCommands.BONDED_DEVICES,
-            m_type=CoordinatorMessages.BONDED_DEVICES,
+            pcmd=CoordinatorRequestCommands.DISCOVERED_DEVICES,
+            m_type=CoordinatorMessages.DISCOVERED_DEVICES,
             hwpid=hwpid,
             msgid=msgid
         )
 
     def to_dpa(self, mutable: bool = False) -> Union[bytes, bytearray]:
         return super().to_dpa(mutable=mutable)
```

### Comparing `iqrfpy-0.1.5/iqrfpy/messages/requests/coordinator/ClearAllBonds.py` & `iqrfpy-0.1.6/iqrfpy/messages/requests/coordinator/ClearAllBonds.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from __future__ import annotations
 from typeguard import typechecked
 from uuid import uuid4
 from typing import Union
-from iqrfpy.enums.Commands import CoordinatorRequestCommands
-from iqrfpy.enums.MessageTypes import CoordinatorMessages
+from iqrfpy.enums.commands import CoordinatorRequestCommands
+from iqrfpy.enums.message_types import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
-from iqrfpy.utils.common import Common
+import iqrfpy.utils.dpa as DpaConstants
 from iqrfpy.messages.requests.IRequest import IRequest
 
 __all__ = ['ClearAllBondsRequest']
 
 
 @typechecked
 class ClearAllBondsRequest(IRequest):
 
-    def __init__(self, hwpid: int = Common.HWPID_MAX, msgid: str = str(uuid4())):
+    def __init__(self, hwpid: int = DpaConstants.HWPID_MAX, msgid: str = str(uuid4())):
         super().__init__(
-            nadr=0,
+            nadr=DpaConstants.COORDINATOR_NADR,
             pnum=EmbedPeripherals.COORDINATOR,
             pcmd=CoordinatorRequestCommands.CLEAR_ALL_BONDS,
             m_type=CoordinatorMessages.CLEAR_ALL_BONDS,
             hwpid=hwpid,
             msgid=msgid
         )
```

### Comparing `iqrfpy-0.1.5/iqrfpy/messages/requests/coordinator/DiscoveredDevices.py` & `iqrfpy-0.1.6/iqrfpy/messages/requests/coordinator/AddrInfo.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from __future__ import annotations
 from typeguard import typechecked
 from uuid import uuid4
 from typing import Union
-from iqrfpy.enums.Commands import CoordinatorRequestCommands
-from iqrfpy.enums.MessageTypes import CoordinatorMessages
+from iqrfpy.enums.commands import CoordinatorRequestCommands
+from iqrfpy.enums.message_types import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
-from iqrfpy.utils.common import Common
+import iqrfpy.utils.dpa as DpaConstants
 from iqrfpy.messages.requests.IRequest import IRequest
 
-__all__ = ['DiscoveredDevicesRequest']
+__all__ = ['AddrInfoRequest']
 
 
 @typechecked
-class DiscoveredDevicesRequest(IRequest):
+class AddrInfoRequest(IRequest):
 
-    def __init__(self, hwpid: int = Common.HWPID_MAX, msgid: str = str(uuid4())):
+    def __init__(self, hwpid: int = DpaConstants.HWPID_MAX, msgid: str = str(uuid4())):
         super().__init__(
-            nadr=0,
+            nadr=DpaConstants.COORDINATOR_NADR,
             pnum=EmbedPeripherals.COORDINATOR,
-            pcmd=CoordinatorRequestCommands.DISCOVERED_DEVICES,
-            m_type=CoordinatorMessages.DISCOVERED_DEVICES,
+            pcmd=CoordinatorRequestCommands.ADDR_INFO,
+            m_type=CoordinatorMessages.ADDR_INFO,
             hwpid=hwpid,
             msgid=msgid
         )
 
     def to_dpa(self, mutable: bool = False) -> Union[bytes, bytearray]:
         return super().to_dpa(mutable=mutable)
```

### Comparing `iqrfpy-0.1.5/iqrfpy/messages/requests/coordinator/Discovery.py` & `iqrfpy-0.1.6/iqrfpy/messages/requests/coordinator/Discovery.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 from __future__ import annotations
 from typeguard import typechecked
 from uuid import uuid4
 from typing import Union
-from iqrfpy.enums.Commands import CoordinatorRequestCommands
-from iqrfpy.enums.MessageTypes import CoordinatorMessages
+from iqrfpy.enums.commands import CoordinatorRequestCommands
+from iqrfpy.enums.message_types import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
 from iqrfpy.exceptions import RequestParameterInvalidValueError
-from iqrfpy.utils.common import Common
+import iqrfpy.utils.dpa as DpaConstants
 from iqrfpy.messages.requests.IRequest import IRequest
 
 __all__ = ['DiscoveryRequest']
 
 
 @typechecked
 class DiscoveryRequest(IRequest):
     __slots__ = '_tx_power', '_max_addr'
 
-    def __init__(self, tx_power: int, max_addr: int, hwpid: int = Common.HWPID_MAX, msgid: str = str(uuid4())) -> None:
+    def __init__(self, tx_power: int, max_addr: int, hwpid: int = DpaConstants.HWPID_MAX, msgid: str = str(uuid4())) -> None:
         super().__init__(
-            nadr=0,
+            nadr=DpaConstants.COORDINATOR_NADR,
             pnum=EmbedPeripherals.COORDINATOR,
             pcmd=CoordinatorRequestCommands.DISCOVERY,
             m_type=CoordinatorMessages.DISCOVERY,
             hwpid=hwpid,
             msgid=msgid
         )
         self._tx_power = tx_power
         self._max_addr = max_addr
         self._validate()
 
     def _validate(self) -> None:
-        if self._tx_power < 0 or self._tx_power > 7:
+        if self._tx_power < DpaConstants.TX_POWER_MIN or self._tx_power > DpaConstants.TX_POWER_MAX:
             raise RequestParameterInvalidValueError('TX power value should be between 0 and 7.')
-        if self._max_addr < 0 or self._max_addr > 239:
+        if self._max_addr < DpaConstants.NADR_MIN or self._max_addr > DpaConstants.NADR_MAX:
             raise RequestParameterInvalidValueError('Max address value should be between 0 and 239.')
 
     def set_tx_power(self, tx_power: int) -> None:
         self._tx_power = tx_power
 
     def set_max_addr(self, max_addr: int) -> None:
         self._max_addr = max_addr
```

### Comparing `iqrfpy-0.1.5/iqrfpy/messages/requests/coordinator/RemoveBond.py` & `iqrfpy-0.1.6/iqrfpy/messages/requests/coordinator/RemoveBond.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 from __future__ import annotations
 from typeguard import typechecked
 from uuid import uuid4
 from typing import Union
-from iqrfpy.enums.Commands import CoordinatorRequestCommands
-from iqrfpy.enums.MessageTypes import CoordinatorMessages
+from iqrfpy.enums.commands import CoordinatorRequestCommands
+from iqrfpy.enums.message_types import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
 from iqrfpy.exceptions import RequestParameterInvalidValueError
-from iqrfpy.utils.common import Common
+import iqrfpy.utils.dpa as DpaConstants
 from iqrfpy.messages.requests.IRequest import IRequest
 
 __all__ = ['RemoveBondRequest']
 
 
 @typechecked
 class RemoveBondRequest(IRequest):
     __slots__ = '_bond_addr'
 
-    def __init__(self, bond_addr: int, hwpid: int = Common.HWPID_MAX, msgid: str = str(uuid4())):
+    def __init__(self, bond_addr: int, hwpid: int = DpaConstants.HWPID_MAX, msgid: str = str(uuid4())):
         super().__init__(
-            nadr=0,
+            nadr=DpaConstants.COORDINATOR_NADR,
             pnum=EmbedPeripherals.COORDINATOR,
             pcmd=CoordinatorRequestCommands.REMOVE_BOND,
             m_type=CoordinatorMessages.REMOVE_BOND,
             hwpid=hwpid,
             msgid=msgid
         )
         self._bond_addr = bond_addr
         self._validate()
 
     def _validate(self) -> None:
-        if self._bond_addr < 1 or self._bond_addr > 239:
+        if self._bond_addr < DpaConstants.NODE_NADR_MIN or self._bond_addr > DpaConstants.NODE_NADR_MAX:
             raise RequestParameterInvalidValueError('Bond address value should be between 1 and 239.')
 
     def set_bond_addr(self, bond_addr: int) -> None:
         self._bond_addr = bond_addr
 
     def to_dpa(self, mutable: bool = False) -> Union[bytes, bytearray]:
         self._validate()
```

### Comparing `iqrfpy-0.1.5/iqrfpy/messages/requests/coordinator/Restore.py` & `iqrfpy-0.1.6/iqrfpy/messages/requests/coordinator/Restore.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 from __future__ import annotations
 from typeguard import typechecked
 from uuid import uuid4
 from typing import List, Union
-from iqrfpy.enums.Commands import CoordinatorRequestCommands
-from iqrfpy.enums.MessageTypes import CoordinatorMessages
+from iqrfpy.enums.commands import CoordinatorRequestCommands
+from iqrfpy.enums.message_types import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
 from iqrfpy.exceptions import RequestParameterInvalidValueError
 from iqrfpy.utils.common import Common
+import iqrfpy.utils.dpa as DpaConstants
 from iqrfpy.messages.requests.IRequest import IRequest
 
 __all__ = ['RestoreRequest']
 
 
 @typechecked
 class RestoreRequest(IRequest):
     __slots__ = '_network_data'
 
-    def __init__(self, network_data: List[int], hwpid: int = Common.HWPID_MAX, msgid: str = str(uuid4())):
+    def __init__(self, network_data: List[int], hwpid: int = DpaConstants.HWPID_MAX, msgid: str = str(uuid4())):
         super().__init__(
-            nadr=0,
+            nadr=DpaConstants.COORDINATOR_NADR,
             pnum=EmbedPeripherals.COORDINATOR,
             pcmd=CoordinatorRequestCommands.RESTORE,
             m_type=CoordinatorMessages.RESTORE,
             hwpid=hwpid,
             msgid=msgid
         )
         self._network_data = network_data
         self._validate()
 
     def _validate(self) -> None:
         if not Common.values_in_byte_range(self._network_data):
             raise RequestParameterInvalidValueError('Network data block values should be between 0 and 255.')
-        if len(self._network_data) != 49:
+        if len(self._network_data) != DpaConstants.BACKUP_DATA_LEN:
             raise RequestParameterInvalidValueError('Network data should be 49 blocks long.')
 
     def set_network_data(self, network_data: List[int]) -> None:
         self._network_data = network_data
 
     def to_dpa(self, mutable: bool = False) -> Union[bytes, bytearray]:
         self._validate()
```

### Comparing `iqrfpy-0.1.5/iqrfpy/messages/requests/coordinator/SetDpaParams.py` & `iqrfpy-0.1.6/iqrfpy/messages/requests/coordinator/SetDpaParams.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import annotations
 from typeguard import typechecked
 from enum import IntEnum
 from uuid import uuid4
 from typing import Union
-from iqrfpy.enums.Commands import CoordinatorRequestCommands
-from iqrfpy.enums.MessageTypes import CoordinatorMessages
+from iqrfpy.enums.commands import CoordinatorRequestCommands
+from iqrfpy.enums.message_types import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
-from iqrfpy.utils.common import Common
+import iqrfpy.utils.dpa as DpaConstants
 from iqrfpy.messages.requests.IRequest import IRequest
 
 __all__ = ['SetDpaParamsRequest', 'DpaParam']
 
 
 @typechecked
 class DpaParam(IntEnum):
@@ -20,17 +20,17 @@
     USER_SPECIFIED = 3
 
 
 @typechecked
 class SetDpaParamsRequest(IRequest):
     __slots__ = '_dpa_param'
 
-    def __init__(self, dpa_param: DpaParam, hwpid: int = Common.HWPID_MAX, msgid: str = str(uuid4())):
+    def __init__(self, dpa_param: DpaParam, hwpid: int = DpaConstants.HWPID_MAX, msgid: str = str(uuid4())):
         super().__init__(
-            nadr=0,
+            nadr=DpaConstants.COORDINATOR_NADR,
             pnum=EmbedPeripherals.COORDINATOR,
             pcmd=CoordinatorRequestCommands.SET_DPA_PARAMS,
             m_type=CoordinatorMessages.SET_DPA_PARAMS,
             hwpid=hwpid,
             msgid=msgid
         )
         self._dpa_param = dpa_param
```

### Comparing `iqrfpy-0.1.5/iqrfpy/messages/requests/coordinator/SetHops.py` & `iqrfpy-0.1.6/iqrfpy/messages/requests/coordinator/SetHops.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,42 +1,49 @@
 from __future__ import annotations
 from typeguard import typechecked
 from uuid import uuid4
 from typing import Union
-from iqrfpy.enums.Commands import CoordinatorRequestCommands
-from iqrfpy.enums.MessageTypes import CoordinatorMessages
+from iqrfpy.enums.commands import CoordinatorRequestCommands
+from iqrfpy.enums.message_types import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
 from iqrfpy.exceptions import RequestParameterInvalidValueError
-from iqrfpy.utils.common import Common
+import iqrfpy.utils.dpa as DpaConstants
 from iqrfpy.messages.requests.IRequest import IRequest
 
 __all__ = ['SetHopsRequest']
 
+REQUEST_HOPS_DRM = 0
+REQUEST_HOPS_DOM = 0xFF
+RESPONSE_HOPS_DOM = 0xFF
+
 
 @typechecked
 class SetHopsRequest(IRequest):
     __slots__ = '_request_hops', '_response_hops'
 
-    def __init__(self, request_hops: int, response_hops: int, hwpid: int = Common.HWPID_MAX, msgid: str = str(uuid4())):
+    def __init__(self, request_hops: int, response_hops: int, hwpid: int = DpaConstants.HWPID_MAX,
+                 msgid: str = str(uuid4())):
         super().__init__(
-            nadr=0,
+            nadr=DpaConstants.COORDINATOR_NADR,
             pnum=EmbedPeripherals.COORDINATOR,
             pcmd=CoordinatorRequestCommands.SET_HOPS,
             m_type=CoordinatorMessages.SET_HOPS,
             hwpid=hwpid,
             msgid=msgid
         )
         self._request_hops = request_hops
         self._response_hops = response_hops
         self._validate()
 
     def _validate(self) -> None:
-        if (self._request_hops < 0 or self._request_hops > 239) and self._request_hops != 255:
+        if (self._request_hops < REQUEST_HOPS_DRM or self._request_hops > DpaConstants.NODE_NADR_MAX) \
+                and self._request_hops != REQUEST_HOPS_DOM:
             raise RequestParameterInvalidValueError('Request hops value should be between 0 and 239, or 255.')
-        if (self._response_hops < 1 or self._response_hops > 239) and self._response_hops != 255:
+        if (self._response_hops < DpaConstants.NODE_NADR_MIN or self._response_hops > DpaConstants.NODE_NADR_MAX) \
+                and self._response_hops != RESPONSE_HOPS_DOM:
             raise RequestParameterInvalidValueError('Response hops value should be between 1 and 239, or 255.')
 
     def set_request_hops(self, request_hops: int) -> None:
         self._request_hops = request_hops
 
     def set_response_hops(self, response_hops: int) -> None:
         self._response_hops = response_hops
```

### Comparing `iqrfpy-0.1.5/iqrfpy/messages/requests/coordinator/SetMID.py` & `iqrfpy-0.1.6/iqrfpy/messages/requests/coordinator/SetMID.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 from __future__ import annotations
 from typeguard import typechecked
 from uuid import uuid4
 from typing import Union
-from iqrfpy.enums.Commands import CoordinatorRequestCommands
-from iqrfpy.enums.MessageTypes import CoordinatorMessages
+from iqrfpy.enums.commands import CoordinatorRequestCommands
+from iqrfpy.enums.message_types import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
 from iqrfpy.exceptions import RequestParameterInvalidValueError
-from iqrfpy.utils.common import Common
+import iqrfpy.utils.dpa as DpaConstants
 from iqrfpy.messages.requests.IRequest import IRequest
 
 __all__ = ['SetMIDRequest']
 
 
 @typechecked
 class SetMIDRequest(IRequest):
     __slots__ = '_bond_addr', '_mid'
 
-    def __init__(self, bond_addr: int, mid: int, hwpid: int = Common.HWPID_MAX, msgid: str = str(uuid4())):
+    def __init__(self, bond_addr: int, mid: int, hwpid: int = DpaConstants.HWPID_MAX, msgid: str = str(uuid4())):
         super().__init__(
-            nadr=0,
+            nadr=DpaConstants.COORDINATOR_NADR,
             pnum=EmbedPeripherals.COORDINATOR,
             pcmd=CoordinatorRequestCommands.SET_MID,
             m_type=CoordinatorMessages.SET_MID,
             hwpid=hwpid,
             msgid=msgid
         )
         self._bond_addr = bond_addr
         self._mid = mid
         self._validate()
 
     def _validate(self) -> None:
-        if self._bond_addr < 1 or self._bond_addr > 239:
+        if self._bond_addr < DpaConstants.NODE_NADR_MIN or self._bond_addr > DpaConstants.NODE_NADR_MAX:
             raise RequestParameterInvalidValueError('Bond address value should be between 1 and 239.')
-        if self._mid < 0 or self._mid > 0xFFFFFFFF:
+        if self._mid < DpaConstants.MID_MIN or self._mid > DpaConstants.MID_MAX:
             raise RequestParameterInvalidValueError('MID value should be an unsigned 32bit integer.')
 
     def set_bond_addr(self, bond_addr: int) -> None:
         self._bond_addr = bond_addr
 
     def set_mid(self, mid: int) -> None:
         self._mid = mid
```

### Comparing `iqrfpy-0.1.5/iqrfpy/messages/requests/coordinator/SmartConnect.py` & `iqrfpy-0.1.6/iqrfpy/messages/requests/coordinator/SmartConnect.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,68 +1,70 @@
 from __future__ import annotations
 from typeguard import typechecked
 from uuid import uuid4
 from typing import List, Union
-from iqrfpy.enums.Commands import CoordinatorRequestCommands
-from iqrfpy.enums.MessageTypes import CoordinatorMessages
+from iqrfpy.enums.commands import CoordinatorRequestCommands
+from iqrfpy.enums.message_types import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
 from iqrfpy.exceptions import RequestParameterInvalidValueError
 from iqrfpy.utils.common import Common
+import iqrfpy.utils.dpa as DpaConstants
 from iqrfpy.messages.requests.IRequest import IRequest
 
 __all__ = ['SmartConnectRequest']
 
 
 @typechecked
 class SmartConnectRequest(IRequest):
     __slots__ = '_req_addr', '_bonding_test_retries', '_ibk', '_mid', '_virtual_device_address'
 
     def __init__(self, req_addr: int, bonding_test_retries: int, ibk: Union[str, List[int]], mid: int,
-                 virtual_device_address: int = 0xFF, hwpid: int = Common.HWPID_MAX, msgid: str = str(uuid4())):
+                 virtual_device_address: int = 0xFF, hwpid: int = DpaConstants.HWPID_MAX, msgid: str = str(uuid4())):
         super().__init__(
-            nadr=0,
+            nadr=DpaConstants.COORDINATOR_NADR,
             pnum=EmbedPeripherals.COORDINATOR,
             pcmd=CoordinatorRequestCommands.SMART_CONNECT,
             m_type=CoordinatorMessages.SMART_CONNECT,
             hwpid=hwpid,
             msgid=msgid
         )
         self._req_addr = req_addr
         self._bonding_test_retries = bonding_test_retries
         self._ibk = ibk
         self._mid = mid
         self._virtual_device_address = virtual_device_address
         self._validate()
 
     def _validate(self) -> None:
-        if self._req_addr == Common.IQMESH_TEMP_ADDR:
-            if self._bonding_test_retries != 0:
+        if self._req_addr == DpaConstants.IQMESH_TEMP_ADDR:
+            if self._bonding_test_retries != DpaConstants.BYTE_MIN:
                 raise RequestParameterInvalidValueError('Bonding test value must be zero if requested address \
                 set to 254.')
-            if len(self._ibk) != 32:
+            if len(self._ibk) != DpaConstants.IBK_LEN:
                 raise RequestParameterInvalidValueError('IBK should be a string of 32 hex characters.')
             # if set(self._ibk) - set('0'):
             #    raise RequestParameterInvalidValueError('IBK values must be zero if requested address is set to 254.')
-            if self._mid != 0:
+            if self._mid != DpaConstants.MID_MIN:
                 raise RequestParameterInvalidValueError('MID value must be zero if requested address is set to 254.')
-            if self._virtual_device_address != 0:
+            if self._virtual_device_address != DpaConstants.NADR_MIN:
                 raise RequestParameterInvalidValueError('VRN value must be zero if requested address is set to 254.')
             return
-        if self._req_addr < 1 or self._req_addr > 239:
+        if self._req_addr < DpaConstants.NODE_NADR_MIN or self._req_addr > DpaConstants.NODE_NADR_MAX:
             raise RequestParameterInvalidValueError('Requested address value should be between 1 and 239, or 254.')
-        if self._bonding_test_retries < 0 or self._bonding_test_retries > 255:
+        if self._bonding_test_retries < DpaConstants.BYTE_MIN or self._bonding_test_retries > DpaConstants.BYTE_MAX:
             raise RequestParameterInvalidValueError('Bonding test retries value should be between 0 and 255.')
-        if len(self._ibk) != 32:
+        if len(self._ibk) != DpaConstants.IBK_LEN:
             raise RequestParameterInvalidValueError('IBK should be a string of 32 hex characters.')
         if not Common.is_hex_string(self._ibk):
             raise RequestParameterInvalidValueError('IBK string should only contain hexadecimal characters.')
-        if self._mid < 0 or self._mid > 0xFFFFFFFF:
+        if self._mid < DpaConstants.MID_MIN or self._mid > DpaConstants.MID_MAX:
             raise RequestParameterInvalidValueError('MID value should be an unsigned 32bit integer.')
-        if (self._virtual_device_address < 1 or self._virtual_device_address > 239) \
-                and self._virtual_device_address != 255:
+        if (self._virtual_device_address < DpaConstants.NODE_NADR_MIN
+            or self._virtual_device_address > DpaConstants.NODE_NADR_MAX) \
+                and self._virtual_device_address != DpaConstants.VDA_UNUSED:
             raise RequestParameterInvalidValueError('VRN value should be between 1 and 239, or 255.')
 
     def set_req_addr(self, req_addr: int) -> None:
         self._req_addr = req_addr
 
     def set_bonding_test_retries(self, bonding_test_retries: int) -> None:
         self._bonding_test_retries = bonding_test_retries
```

### Comparing `iqrfpy-0.1.5/iqrfpy/messages/requests/coordinator/__init__.py` & `iqrfpy-0.1.6/iqrfpy/messages/requests/coordinator/__init__.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.5/iqrfpy/messages/response_factory.py` & `iqrfpy-0.1.6/iqrfpy/messages/response_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from abc import ABC, abstractmethod
-from ..enums.MessageTypes import *
+from ..enums.message_types import *
 from .responses.AsyncResponse import AsyncResponse
 from .responses.Confirmation import Confirmation
 from .responses.IResponse import IResponse
 from .responses.coordinator import *
 from ..utils.common import Common
+from ..utils.dpa import *
 from ..exceptions import UnsupportedMessageTypeError
 
 __all__ = [
     'ResponseFactory',
     '_get_factory_from_mtype',
     'AsyncResponseFactory',
     'ConfirmationFactory',
@@ -30,20 +31,20 @@
 
 
 class ResponseFactory:
 
     @staticmethod
     def get_response_from_dpa(dpa: bytes) -> IResponse:
         IResponse.validate_dpa_response(dpa)
-        pnum = dpa[2]
-        pcmd = dpa[3]
-        rcode = dpa[6]
-        if rcode == 0xFF and len(dpa) == 11:
+        pnum = dpa[ResponsePacketMembers.PNUM]
+        pcmd = dpa[ResponsePacketMembers.PCMD]
+        rcode = dpa[ResponsePacketMembers.RCODE]
+        if rcode == CONFIRMATION_RCODE and len(dpa) == CONFIRMATION_PACKET_LEN:
             factory = ConfirmationFactory()
-        elif pcmd <= 127 and rcode >= 128:
+        elif pcmd <= REQUEST_PCMD_MAX and rcode >= ASYNC_RESPONSE_CODE:
             factory = AsyncResponseFactory()
         else:
             mtype = Common.mtype_from_dpa_response(pnum, pcmd)
             factory = _get_factory_from_mtype(mtype)
         return factory.create_from_dpa(dpa)
 
     @staticmethod
```

### Comparing `iqrfpy-0.1.5/iqrfpy/messages/responses/AsyncResponse.py` & `iqrfpy-0.1.6/iqrfpy/messages/responses/coordinator/SetMID.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,57 +1,48 @@
 from __future__ import annotations
 from typeguard import typechecked
 from typing import Optional
-from iqrfpy.enums.peripherals import Peripheral
-from iqrfpy.enums.Commands import Command
-from iqrfpy.enums.MessageTypes import GenericMessages
-from .IResponse import IResponse, IResponseGetterMixin
+from iqrfpy.messages.responses.IResponse import IResponse, IResponseGetterMixin
+from iqrfpy.enums.commands import CoordinatorResponseCommands
+from iqrfpy.enums.message_types import CoordinatorMessages
+from iqrfpy.enums.peripherals import EmbedPeripherals
+from iqrfpy.exceptions import DpaResponsePacketLengthError
 from iqrfpy.utils.common import Common
+import iqrfpy.utils.dpa as DpaConstants
+from iqrfpy.utils.dpa import ResponsePacketMembers
 
-__all__ = ['AsyncResponse']
+__all__ = ['SetMIDResponse']
 
 
 @typechecked
-class AsyncResponse(IResponseGetterMixin):
+class SetMIDResponse(IResponseGetterMixin):
 
-    def __init__(self, nadr: int, pnum: Peripheral, pcmd: Command, hwpid: int = Common.HWPID_MAX, rcode: int = 0x80,
-                 dpa_value: int = 0, pdata: Optional[bytes] = None, msgid: Optional[str] = None,
-                 result: Optional[dict] = None):
+    def __init__(self, hwpid: int = DpaConstants.HWPID_MAX, rcode: int = 0, dpa_value: int = 0,
+                 msgid: Optional[str] = None, result: Optional[dict] = None):
         super().__init__(
-            nadr=nadr,
-            pnum=pnum,
-            pcmd=pcmd,
-            m_type=GenericMessages.RAW,
+            nadr=DpaConstants.COORDINATOR_NADR,
+            pnum=EmbedPeripherals.COORDINATOR,
+            pcmd=CoordinatorResponseCommands.SET_MID,
+            m_type=CoordinatorMessages.SET_MID,
             hwpid=hwpid,
             rcode=rcode,
             dpa_value=dpa_value,
-            pdata=pdata,
             msgid=msgid,
             result=result
         )
 
     @staticmethod
-    def from_dpa(dpa: bytes) -> AsyncResponse:
+    def from_dpa(dpa: bytes) -> SetMIDResponse:
         IResponse.validate_dpa_response(dpa)
-        hwpid = Common.hwpid_from_dpa(dpa[5], dpa[4])
-        pnum = Common.pnum_from_dpa(dpa[2])
-        pcmd = Common.request_pcmd_from_dpa(pnum, dpa[3])
-        rcode = dpa[6]
-        result = None
-        if rcode == 0x80:
-            if len(dpa) > 8:
-                result = {'rData': list(dpa)}
-        return AsyncResponse(nadr=dpa[0], pnum=pnum, pcmd=pcmd, hwpid=hwpid, rcode=rcode,
-                             dpa_value=dpa[7], pdata=dpa, result=result)
+        hwpid = Common.hwpid_from_dpa(dpa[ResponsePacketMembers.HWPID_HI], dpa[ResponsePacketMembers.HWPID_LO])
+        rcode = dpa[ResponsePacketMembers.RCODE]
+        if len(dpa) != 8:
+            raise DpaResponsePacketLengthError('Invalid DPA response packet length.')
+        return SetMIDResponse(hwpid=hwpid, rcode=rcode, dpa_value=dpa[ResponsePacketMembers.DPA_VALUE], result=None)
 
     @staticmethod
-    def from_json(json: dict) -> AsyncResponse:
+    def from_json(json: dict) -> SetMIDResponse:
         msgid = Common.msgid_from_json(json)
-        result = json['data']['rsp']
-        packet = result['rData'].replace('.', '')
-        pdata = bytes.fromhex(packet)
-        ldata = Common.hex_string_to_list(packet)
-        hwpid = Common.hwpid_from_dpa(ldata[5], ldata[4])
-        pnum = Common.pnum_from_dpa(ldata[2])
-        pcmd = Common.request_pcmd_from_dpa(pnum, ldata[3])
-        return AsyncResponse(nadr=ldata[0], pnum=pnum, pcmd=pcmd, hwpid=hwpid, rcode=ldata[6],
-                             dpa_value=ldata[7], pdata=pdata, msgid=msgid, result=result)
+        hwpid = Common.hwpid_from_json(json)
+        dpa_value = Common.dpa_value_from_json(json)
+        rcode = Common.rcode_from_json(json)
+        return SetMIDResponse(msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode, result=None)
```

### Comparing `iqrfpy-0.1.5/iqrfpy/messages/responses/Confirmation.py` & `iqrfpy-0.1.6/iqrfpy/messages/responses/Confirmation.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from __future__ import annotations
 from typing import Optional
-from iqrfpy.enums.Commands import Command
+from iqrfpy.enums.commands import Command
 from iqrfpy.enums.peripherals import Peripheral
 from iqrfpy.exceptions import DpaConfirmationPacketError, DpaConfirmationPacketLengthError
 from iqrfpy.utils.common import Common
+import iqrfpy.utils.dpa as DpaConstants
+from iqrfpy.utils.dpa import ResponseCodes, ResponsePacketMembers
 from iqrfpy.messages.responses.IResponse import IResponseGetterMixin
 
 __all__ = ['Confirmation']
 
 
 class Confirmation(IResponseGetterMixin):
     __slots__ = '_request_hops', '_response_hops', '_timeslot'
@@ -34,21 +36,22 @@
         return self._response_hops
 
     def get_timeslot(self) -> int:
         return self._timeslot
 
     @staticmethod
     def from_dpa(dpa: bytes) -> Confirmation:
-        if len(dpa) != 11:
+        if len(dpa) != DpaConstants.CONFIRMATION_PACKET_LEN:
             raise DpaConfirmationPacketLengthError('Invalid DPA confirmation packet length.')
-        if dpa[6] != 0xFF:
+        if dpa[ResponsePacketMembers.RCODE] != DpaConstants.CONFIRMATION_RCODE:
             raise DpaConfirmationPacketError('Invalid DPA confirmation packet error code.')
-        pnum = Common.pnum_from_dpa(dpa[2])
-        pcmd = Common.request_pcmd_from_dpa(pnum, dpa[3])
-        hwpid = Common.hwpid_from_dpa(dpa[5], dpa[4])
+        pnum = Common.pnum_from_dpa(dpa[ResponsePacketMembers.PNUM])
+        pcmd = Common.request_pcmd_from_dpa(pnum, dpa[ResponsePacketMembers.PCMD])
+        hwpid = Common.hwpid_from_dpa(dpa[ResponsePacketMembers.HWPID_HI], dpa[ResponsePacketMembers.HWPID_LO])
         result = {'requestHops': dpa[8], 'responseHops': dpa[10], 'timeslot': dpa[9]}
-        return Confirmation(nadr=dpa[0], pnum=pnum, pcmd=pcmd, hwpid=hwpid, rcode=dpa[6], dpa_value=dpa[7],
+        return Confirmation(nadr=dpa[ResponsePacketMembers.NADR], pnum=pnum, pcmd=pcmd, hwpid=hwpid,
+                            rcode=dpa[ResponsePacketMembers.RCODE], dpa_value=dpa[ResponsePacketMembers.DPA_VALUE],
                             result=result)
 
     @staticmethod
     def from_json(json: dict) -> Confirmation:
         raise NotImplementedError('from_json() method not implemented.')
```

### Comparing `iqrfpy-0.1.5/iqrfpy/messages/responses/IResponse.py` & `iqrfpy-0.1.6/iqrfpy/messages/responses/IResponse.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from __future__ import annotations
 from abc import ABC, abstractmethod
 from typing import Optional
-from iqrfpy.enums.Commands import Command
-from iqrfpy.enums.MessageTypes import MessageType
+from iqrfpy.enums.commands import Command
+from iqrfpy.enums.message_types import MessageType
 from iqrfpy.enums.peripherals import Peripheral
 from iqrfpy.exceptions import DpaResponsePacketLengthError
-from iqrfpy.utils.common import Common
+import iqrfpy.utils.dpa as DpaConstants
 
 __all__ = ['IResponse', 'IResponseGetterMixin']
 
 
 class IResponse(ABC):
 
     ASYNC_MSGID = 'async'
 
-    def __init__(self, nadr: int, pnum: Peripheral, pcmd: Command, hwpid: int = Common.HWPID_MAX, rcode: int = 0,
+    def __init__(self, nadr: int, pnum: Peripheral, pcmd: Command, hwpid: int = DpaConstants.HWPID_MAX, rcode: int = 0,
                  dpa_value: int = 0, pdata: Optional[bytes] = None, m_type: Optional[MessageType] = None,
                  msgid: Optional[str] = None, result: Optional[dict] = None):
         self._nadr: int = nadr
         self._pnum: Peripheral = pnum
         self._pcmd: Command = pcmd
         self._mtype = m_type
         self._hwpid: int = hwpid
```

### Comparing `iqrfpy-0.1.5/iqrfpy/messages/responses/coordinator/AddrInfo.py` & `iqrfpy-0.1.6/iqrfpy/messages/responses/coordinator/AddrInfo.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,60 +1,62 @@
 from __future__ import annotations
 from typeguard import typechecked
 from typing import Optional
 from iqrfpy.messages.responses.IResponse import IResponse, IResponseGetterMixin
-from iqrfpy.enums.Commands import CoordinatorResponseCommands
-from iqrfpy.enums.MessageTypes import CoordinatorMessages
+from iqrfpy.enums.commands import CoordinatorResponseCommands
+from iqrfpy.enums.message_types import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
 from iqrfpy.exceptions import DpaResponsePacketLengthError
 from iqrfpy.utils.common import Common
+import iqrfpy.utils.dpa as DpaConstants
+from iqrfpy.utils.dpa import ResponseCodes, ResponsePacketMembers
 
 __all__ = ['AddrInfoResponse']
 
 
 @typechecked
 class AddrInfoResponse(IResponseGetterMixin):
     __slots__ = '_dev_nr', '_did'
 
-    def __init__(self, hwpid: int = 0xFFFF, rcode: int = 0, dpa_value: int = 0,
+    def __init__(self, hwpid: int = DpaConstants.HWPID_MAX, rcode: int = 0, dpa_value: int = 0,
                  msgid: Optional[str] = None, result: Optional[dict] = None):
         super().__init__(
-            nadr=0,
+            nadr=DpaConstants.COORDINATOR_NADR,
             pnum=EmbedPeripherals.COORDINATOR,
             pcmd=CoordinatorResponseCommands.ADDR_INFO,
             m_type=CoordinatorMessages.ADDR_INFO,
             hwpid=hwpid,
             rcode=rcode,
             dpa_value=dpa_value,
             msgid=msgid,
             result=result
         )
-        if rcode == 0:
+        if rcode == ResponseCodes.OK:
             self._dev_nr = result['devNr']
             self._did = result['did']
 
     def get_dev_nr(self) -> int:
         return self._dev_nr
 
     def get_did(self) -> int:
         return self._did
 
     @staticmethod
     def from_dpa(dpa: bytes) -> AddrInfoResponse:
         IResponse.validate_dpa_response(dpa)
-        hwpid = Common.hwpid_from_dpa(dpa[5], dpa[4])
-        rcode = dpa[6]
+        hwpid = Common.hwpid_from_dpa(dpa[ResponsePacketMembers.HWPID_HI], dpa[ResponsePacketMembers.HWPID_LO])
+        rcode = dpa[ResponsePacketMembers.RCODE]
         result = None
-        if rcode == 0:
+        if rcode == ResponseCodes.OK:
             if len(dpa) != 10:
                 raise DpaResponsePacketLengthError('Invalid DPA response packet length.')
             result = {'devNr': dpa[8], 'did': dpa[9]}
-        return AddrInfoResponse(hwpid=hwpid, rcode=rcode, dpa_value=dpa[7], result=result)
+        return AddrInfoResponse(hwpid=hwpid, rcode=rcode, dpa_value=dpa[ResponsePacketMembers.DPA_VALUE], result=result)
 
     @staticmethod
     def from_json(json: dict) -> AddrInfoResponse:
         msgid = Common.msgid_from_json(json)
         hwpid = Common.hwpid_from_json(json)
         dpa_value = Common.dpa_value_from_json(json)
         rcode = Common.rcode_from_json(json)
-        result = Common.result_from_json(json) if rcode == 0 else None
+        result = Common.result_from_json(json) if rcode == ResponseCodes.OK else None
         return AddrInfoResponse(msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode, result=result)
```

### Comparing `iqrfpy-0.1.5/iqrfpy/messages/responses/coordinator/AuthorizeBond.py` & `iqrfpy-0.1.6/iqrfpy/messages/responses/coordinator/RemoveBond.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,60 +1,59 @@
 from __future__ import annotations
 from typeguard import typechecked
 from typing import Optional
 from iqrfpy.messages.responses.IResponse import IResponse, IResponseGetterMixin
-from iqrfpy.enums.Commands import CoordinatorResponseCommands
-from iqrfpy.enums.MessageTypes import CoordinatorMessages
+from iqrfpy.enums.commands import CoordinatorResponseCommands
+from iqrfpy.enums.message_types import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
 from iqrfpy.exceptions import DpaResponsePacketLengthError
 from iqrfpy.utils.common import Common
+import iqrfpy.utils.dpa as DpaConstants
+from iqrfpy.utils.dpa import ResponseCodes, ResponsePacketMembers
 
-__all__ = ['AuthorizeBondResponse']
+__all__ = ['RemoveBondResponse']
 
 
 @typechecked
-class AuthorizeBondResponse(IResponseGetterMixin):
-    __slots__ = '_bond_addr', '_dev_nr'
+class RemoveBondResponse(IResponseGetterMixin):
+    __slots__ = '_dev_nr'
 
-    def __init__(self, hwpid: int = Common.HWPID_MAX, rcode: int = 0, dpa_value: int = 0,
+    def __init__(self, hwpid: int = DpaConstants.HWPID_MAX, rcode: int = 0, dpa_value: int = 0,
                  msgid: Optional[str] = None, result: Optional[dict] = None):
         super().__init__(
-            nadr=0,
+            nadr=DpaConstants.COORDINATOR_NADR,
             pnum=EmbedPeripherals.COORDINATOR,
-            pcmd=CoordinatorResponseCommands.AUTHORIZE_BOND,
-            m_type=CoordinatorMessages.AUTHORIZE_BOND,
+            pcmd=CoordinatorResponseCommands.REMOVE_BOND,
+            m_type=CoordinatorMessages.REMOVE_BOND,
             hwpid=hwpid,
             rcode=rcode,
             dpa_value=dpa_value,
             msgid=msgid,
             result=result
         )
-        if rcode == 0:
-            self._bond_addr = result['bondAddr']
+        if rcode == ResponseCodes.OK:
             self._dev_nr = result['devNr']
 
-    def get_bond_addr(self) -> int:
-        return self._bond_addr
-
     def get_dev_nr(self) -> int:
         return self._dev_nr
 
     @staticmethod
-    def from_dpa(dpa: bytes) -> AuthorizeBondResponse:
+    def from_dpa(dpa: bytes) -> RemoveBondResponse:
         IResponse.validate_dpa_response(dpa)
-        hwpid = Common.hwpid_from_dpa(dpa[5], dpa[4])
-        rcode = dpa[6]
+        hwpid = Common.hwpid_from_dpa(dpa[ResponsePacketMembers.HWPID_HI], dpa[ResponsePacketMembers.HWPID_LO])
+        rcode = dpa[ResponsePacketMembers.RCODE]
         result = None
-        if rcode == 0:
-            if len(dpa) != 10:
+        if rcode == ResponseCodes.OK:
+            if len(dpa) != 9:
                 raise DpaResponsePacketLengthError('Invalid DPA response packet length.')
-            result = {'bondAddr': dpa[8], 'devNr': dpa[9]}
-        return AuthorizeBondResponse(hwpid=hwpid, rcode=dpa[6], dpa_value=dpa[7], result=result)
+            result = {'devNr': dpa[8]}
+        return RemoveBondResponse(hwpid=hwpid, rcode=rcode, dpa_value=dpa[ResponsePacketMembers.DPA_VALUE],
+                                  result=result)
 
     @staticmethod
-    def from_json(json: dict) -> AuthorizeBondResponse:
+    def from_json(json: dict) -> RemoveBondResponse:
         msgid = Common.msgid_from_json(json)
         hwpid = Common.hwpid_from_json(json)
         dpa_value = Common.dpa_value_from_json(json)
         rcode = Common.rcode_from_json(json)
-        result = Common.result_from_json(json) if rcode == 0 else None
-        return AuthorizeBondResponse(msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode, result=result)
+        result = Common.result_from_json(json) if rcode == ResponseCodes.OK else None
+        return RemoveBondResponse(msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode, result=result)
```

### Comparing `iqrfpy-0.1.5/iqrfpy/messages/responses/coordinator/Backup.py` & `iqrfpy-0.1.6/iqrfpy/messages/responses/coordinator/Backup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,56 +1,58 @@
 from __future__ import annotations
 from typeguard import typechecked
 from typing import List, Optional
 from iqrfpy.messages.responses.IResponse import IResponse, IResponseGetterMixin
-from iqrfpy.enums.Commands import CoordinatorResponseCommands
-from iqrfpy.enums.MessageTypes import CoordinatorMessages
+from iqrfpy.enums.commands import CoordinatorResponseCommands
+from iqrfpy.enums.message_types import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
 from iqrfpy.exceptions import DpaResponsePacketLengthError
 from iqrfpy.utils.common import Common
+import iqrfpy.utils.dpa as DpaConstants
+from iqrfpy.utils.dpa import ResponseCodes, ResponsePacketMembers
 
 __all__ = ['BackupResponse']
 
 
 @typechecked
 class BackupResponse(IResponseGetterMixin):
     __slots__ = '_network_data'
 
-    def __init__(self, hwpid: int = Common.HWPID_MAX, rcode: int = 0, dpa_value: int = 0,
+    def __init__(self, hwpid: int = DpaConstants.HWPID_MAX, rcode: int = 0, dpa_value: int = 0,
                  msgid: Optional[str] = None, result: Optional[dict] = None):
         super().__init__(
-            nadr=0,
+            nadr=DpaConstants.COORDINATOR_NADR,
             pnum=EmbedPeripherals.COORDINATOR,
             pcmd=CoordinatorResponseCommands.BACKUP,
             m_type=CoordinatorMessages.BACKUP,
             hwpid=hwpid,
             rcode=rcode,
             dpa_value=dpa_value,
             msgid=msgid,
             result=result
         )
-        if rcode == 0:
+        if rcode == ResponseCodes.OK:
             self._network_data = result['networkData']
 
     def get_network_data(self) -> List[int]:
         return self._network_data
 
     @staticmethod
     def from_dpa(dpa: bytes) -> BackupResponse:
         IResponse.validate_dpa_response(dpa)
-        hwpid = Common.hwpid_from_dpa(dpa[5], dpa[4])
-        rcode = dpa[6]
+        hwpid = Common.hwpid_from_dpa(dpa[ResponsePacketMembers.HWPID_HI], dpa[ResponsePacketMembers.HWPID_LO])
+        rcode = dpa[ResponsePacketMembers.RCODE]
         result = None
-        if rcode == 0:
+        if rcode == ResponseCodes.OK:
             if len(dpa) != 57:
                 raise DpaResponsePacketLengthError('Invalid DPA response packet length.')
             result = {'networkData': list(dpa[8:])}
-        return BackupResponse(hwpid=hwpid, rcode=dpa[6], dpa_value=dpa[7], result=result)
+        return BackupResponse(hwpid=hwpid, rcode=rcode, dpa_value=dpa[ResponsePacketMembers.DPA_VALUE], result=result)
 
     @staticmethod
     def from_json(json: dict) -> BackupResponse:
         msgid = Common.msgid_from_json(json)
         hwpid = Common.hwpid_from_json(json)
         dpa_value = Common.dpa_value_from_json(json)
         rcode = Common.rcode_from_json(json)
-        result = Common.result_from_json(json) if rcode == 0 else None
+        result = Common.result_from_json(json) if rcode == ResponseCodes.OK else None
         return BackupResponse(msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode, result=result)
```

### Comparing `iqrfpy-0.1.5/iqrfpy/messages/responses/coordinator/BondNode.py` & `iqrfpy-0.1.6/iqrfpy/messages/responses/coordinator/Discovery.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,60 +1,59 @@
 from __future__ import annotations
 from typeguard import typechecked
 from typing import Optional
 from iqrfpy.messages.responses.IResponse import IResponse, IResponseGetterMixin
-from iqrfpy.enums.Commands import CoordinatorResponseCommands
-from iqrfpy.enums.MessageTypes import CoordinatorMessages
+from iqrfpy.enums.commands import CoordinatorResponseCommands
+from iqrfpy.enums.message_types import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
 from iqrfpy.exceptions import DpaResponsePacketLengthError
 from iqrfpy.utils.common import Common
+import iqrfpy.utils.dpa as DpaConstants
+from iqrfpy.utils.dpa import ResponseCodes, ResponsePacketMembers
 
-__all__ = ['BondNodeResponse']
+__all__ = ['DiscoveryResponse']
 
 
 @typechecked
-class BondNodeResponse(IResponseGetterMixin):
-    __slots__ = '_bond_addr', '_dev_nr'
+class DiscoveryResponse(IResponseGetterMixin):
+    __slots__ = '_disc_nr'
 
-    def __init__(self, hwpid: int = Common.HWPID_MAX, rcode: int = 0, dpa_value: int = 0,
+    def __init__(self, hwpid: int = DpaConstants.HWPID_MAX, rcode: int = 0, dpa_value: int = 0,
                  msgid: Optional[str] = None, result: Optional[dict] = None):
         super().__init__(
-            nadr=0,
+            nadr=DpaConstants.COORDINATOR_NADR,
             pnum=EmbedPeripherals.COORDINATOR,
-            pcmd=CoordinatorResponseCommands.BOND_NODE,
-            m_type=CoordinatorMessages.BOND_NODE,
+            pcmd=CoordinatorResponseCommands.DISCOVERY,
+            m_type=CoordinatorMessages.DISCOVERY,
             hwpid=hwpid,
             rcode=rcode,
             dpa_value=dpa_value,
             msgid=msgid,
             result=result
         )
-        if rcode == 0:
-            self._bond_addr = result['bondAddr']
-            self._dev_nr = result['devNr']
+        if rcode == ResponseCodes.OK:
+            self._disc_nr = result['discNr']
 
-    def get_bond_addr(self) -> int:
-        return self._bond_addr
-
-    def get_dev_nr(self) -> int:
-        return self._dev_nr
+    def get_disc_nr(self) -> int:
+        return self._disc_nr
 
     @staticmethod
-    def from_dpa(dpa: bytes) -> BondNodeResponse:
+    def from_dpa(dpa: bytes) -> DiscoveryResponse:
         IResponse.validate_dpa_response(dpa)
-        hwpid = Common.hwpid_from_dpa(dpa[5], dpa[4])
-        rcode = dpa[6]
+        hwpid = Common.hwpid_from_dpa(dpa[ResponsePacketMembers.HWPID_HI], dpa[ResponsePacketMembers.HWPID_LO])
+        rcode = dpa[ResponsePacketMembers.RCODE]
         result = None
-        if rcode == 0:
-            if len(dpa) != 10:
+        if rcode == ResponseCodes.OK:
+            if len(dpa) != 9:
                 raise DpaResponsePacketLengthError('Invalid DPA response packet length.')
-            result = {'bondAddr': dpa[8], 'devNr': dpa[9]}
-        return BondNodeResponse(hwpid=hwpid, rcode=dpa[6], dpa_value=dpa[7], result=result)
+            result = {'discNr': dpa[8]}
+        return DiscoveryResponse(hwpid=hwpid, rcode=rcode, dpa_value=dpa[ResponsePacketMembers.DPA_VALUE],
+                                 result=result)
 
     @staticmethod
-    def from_json(json: dict) -> BondNodeResponse:
+    def from_json(json: dict) -> DiscoveryResponse:
         msgid = Common.msgid_from_json(json)
         hwpid = Common.hwpid_from_json(json)
         dpa_value = Common.dpa_value_from_json(json)
         rcode = Common.rcode_from_json(json)
-        result = Common.result_from_json(json) if rcode == 0 else None
-        return BondNodeResponse(msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode, result=result)
+        result = Common.result_from_json(json) if rcode == ResponseCodes.OK else None
+        return DiscoveryResponse(msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode, result=result)
```

### Comparing `iqrfpy-0.1.5/iqrfpy/messages/responses/coordinator/BondedDevices.py` & `iqrfpy-0.1.6/iqrfpy/messages/responses/coordinator/SmartConnect.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,56 +1,63 @@
 from __future__ import annotations
 from typeguard import typechecked
-from typing import List, Optional
-from iqrfpy.enums.Commands import CoordinatorResponseCommands
-from iqrfpy.enums.MessageTypes import CoordinatorMessages
+from typing import Optional
+from iqrfpy.messages.responses.IResponse import IResponse, IResponseGetterMixin
+from iqrfpy.enums.commands import CoordinatorResponseCommands
+from iqrfpy.enums.message_types import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
 from iqrfpy.exceptions import DpaResponsePacketLengthError
 from iqrfpy.utils.common import Common
-from iqrfpy.messages.responses.IResponse import IResponse, IResponseGetterMixin
+import iqrfpy.utils.dpa as DpaConstants
+from iqrfpy.utils.dpa import ResponseCodes, ResponsePacketMembers
 
-__all__ = ['BondedDevicesResponse']
+__all__ = ['SmartConnectResponse']
 
 
 @typechecked
-class BondedDevicesResponse(IResponseGetterMixin):
-    __slots__ = '_bonded'
+class SmartConnectResponse(IResponseGetterMixin):
+    __slots__ = '_bond_addr', '_dev_nr'
 
-    def __init__(self, hwpid: int = Common.HWPID_MAX, rcode: int = 0, dpa_value: int = 0,
+    def __init__(self, hwpid: int = DpaConstants.HWPID_MAX, rcode: int = 0, dpa_value: int = 0,
                  msgid: Optional[str] = None, result: Optional[dict] = None):
         super().__init__(
-            nadr=0,
+            nadr=DpaConstants.COORDINATOR_NADR,
             pnum=EmbedPeripherals.COORDINATOR,
-            pcmd=CoordinatorResponseCommands.BONDED_DEVICES,
-            m_type=CoordinatorMessages.BONDED_DEVICES,
+            pcmd=CoordinatorResponseCommands.SMART_CONNECT,
+            m_type=CoordinatorMessages.SMART_CONNECT,
             hwpid=hwpid,
             rcode=rcode,
             dpa_value=dpa_value,
             msgid=msgid,
             result=result
         )
-        if rcode == 0:
-            self._bonded = result['bondedDevices']
+        if rcode == ResponseCodes.OK:
+            self._bond_addr = result['bondAddr']
+            self._dev_nr = result['devNr']
+
+    def get_bond_addr(self) -> int:
+        return self._bond_addr
 
-    def get_bonded(self) -> List[int]:
-        return self._bonded
+    def get_dev_nr(self) -> int:
+        return self._dev_nr
 
     @staticmethod
-    def from_dpa(dpa: bytes) -> BondedDevicesResponse:
+    def from_dpa(dpa: bytes) -> SmartConnectResponse:
         IResponse.validate_dpa_response(dpa)
-        hwpid = Common.hwpid_from_dpa(dpa[5], dpa[4])
-        rcode = dpa[6]
+        hwpid = Common.hwpid_from_dpa(dpa[ResponsePacketMembers.HWPID_HI], dpa[ResponsePacketMembers.HWPID_LO])
+        rcode = dpa[ResponsePacketMembers.RCODE]
         result = None
-        if rcode == 0:
-            if len(dpa) != 40:
+        if rcode == ResponseCodes.OK:
+            if len(dpa) != 10:
                 raise DpaResponsePacketLengthError('Invalid DPA response packet length.')
-            result = {'bondedDevices': Common.bitmap_to_nodes(list(dpa[8:]))}
-        return BondedDevicesResponse(hwpid=hwpid, rcode=rcode, dpa_value=dpa[7], result=result)
+            result = {'bondAddr': dpa[8], 'devNr': dpa[9]}
+        return SmartConnectResponse(hwpid=hwpid, rcode=rcode, dpa_value=dpa[ResponsePacketMembers.DPA_VALUE],
+                                    result=result)
 
     @staticmethod
-    def from_json(json: dict) -> BondedDevicesResponse:
+    def from_json(json: dict) -> SmartConnectResponse:
         msgid = Common.msgid_from_json(json)
         hwpid = Common.hwpid_from_json(json)
         dpa_value = Common.dpa_value_from_json(json)
         rcode = Common.rcode_from_json(json)
-        result = Common.result_from_json(json) if rcode == 0 else None
-        return BondedDevicesResponse(msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode, result=result)
+        result = Common.result_from_json(json) if rcode == ResponseCodes.OK else None
+        return SmartConnectResponse(msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode, result=result)
```

### Comparing `iqrfpy-0.1.5/iqrfpy/messages/responses/coordinator/ClearAllBonds.py` & `iqrfpy-0.1.6/iqrfpy/messages/responses/coordinator/ClearAllBonds.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,46 +1,50 @@
 from __future__ import annotations
 from typeguard import typechecked
 from typing import Optional
 from iqrfpy.messages.responses.IResponse import IResponse, IResponseGetterMixin
-from iqrfpy.enums.Commands import CoordinatorResponseCommands
-from iqrfpy.enums.MessageTypes import CoordinatorMessages
+from iqrfpy.enums.commands import CoordinatorResponseCommands
+from iqrfpy.enums.message_types import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
 from iqrfpy.exceptions import DpaResponsePacketLengthError
 from iqrfpy.utils.common import Common
+import iqrfpy.utils.dpa as DpaConstants
+from iqrfpy.utils.dpa import ResponseCodes, ResponsePacketMembers
 
 __all__ = ['ClearAllBondsResponse']
 
 
 @typechecked
 class ClearAllBondsResponse(IResponseGetterMixin):
 
-    def __init__(self, hwpid: int = Common.HWPID_MAX, rcode: int = 0, dpa_value: int = 0,
+    def __init__(self, hwpid: int = DpaConstants.HWPID_MAX, rcode: int = 0, dpa_value: int = 0,
                  msgid: Optional[str] = None, result: Optional[dict] = None):
         super().__init__(
-            nadr=0,
+            nadr=DpaConstants.COORDINATOR_NADR,
             pnum=EmbedPeripherals.COORDINATOR,
             pcmd=CoordinatorResponseCommands.CLEAR_ALL_BONDS,
             m_type=CoordinatorMessages.CLEAR_ALL_BONDS,
             hwpid=hwpid,
             rcode=rcode,
             dpa_value=dpa_value,
             msgid=msgid,
             result=result
         )
 
     @staticmethod
     def from_dpa(dpa: bytes) -> ClearAllBondsResponse:
         IResponse.validate_dpa_response(dpa)
-        hwpid = Common.hwpid_from_dpa(dpa[5], dpa[4])
+        hwpid = Common.hwpid_from_dpa(dpa[ResponsePacketMembers.HWPID_HI], dpa[ResponsePacketMembers.HWPID_LO])
+        rcode = dpa[ResponsePacketMembers.RCODE]
         if len(dpa) != 8:
             raise DpaResponsePacketLengthError('Invalid DPA response packet length.')
-        return ClearAllBondsResponse(hwpid=hwpid, rcode=dpa[6], dpa_value=dpa[7], result=None)
+        return ClearAllBondsResponse(hwpid=hwpid, rcode=rcode, dpa_value=dpa[ResponsePacketMembers.DPA_VALUE],
+                                     result=None)
 
     @staticmethod
     def from_json(json: dict) -> ClearAllBondsResponse:
         msgid = Common.msgid_from_json(json)
         hwpid = Common.hwpid_from_json(json)
         dpa_value = Common.dpa_value_from_json(json)
         rcode = Common.rcode_from_json(json)
-        result = Common.result_from_json(json) if rcode == 0 else None
+        result = Common.result_from_json(json) if rcode == ResponseCodes.OK else None
         return ClearAllBondsResponse(msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode, result=result)
```

### Comparing `iqrfpy-0.1.5/iqrfpy/messages/responses/coordinator/DiscoveredDevices.py` & `iqrfpy-0.1.6/iqrfpy/messages/responses/coordinator/DiscoveredDevices.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,56 +1,59 @@
 from __future__ import annotations
 from typeguard import typechecked
 from typing import List, Optional
-from iqrfpy.enums.Commands import CoordinatorResponseCommands
-from iqrfpy.enums.MessageTypes import CoordinatorMessages
+from iqrfpy.enums.commands import CoordinatorResponseCommands
+from iqrfpy.enums.message_types import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
 from iqrfpy.exceptions import DpaResponsePacketLengthError
 from iqrfpy.utils.common import Common
+import iqrfpy.utils.dpa as DpaConstants
+from iqrfpy.utils.dpa import ResponseCodes, ResponsePacketMembers
 from iqrfpy.messages.responses.IResponse import IResponse, IResponseGetterMixin
 
 __all__ = ['DiscoveredDevicesResponse']
 
 
 @typechecked
 class DiscoveredDevicesResponse(IResponseGetterMixin):
     __slots__ = '_discovered'
 
-    def __init__(self, hwpid: int = Common.HWPID_MAX, rcode: int = 0, dpa_value: int = 0,
+    def __init__(self, hwpid: int = DpaConstants.HWPID_MAX, rcode: int = 0, dpa_value: int = 0,
                  msgid: Optional[str] = None, result: Optional[dict] = None):
         super().__init__(
-            nadr=0,
+            nadr=DpaConstants.COORDINATOR_NADR,
             pnum=EmbedPeripherals.COORDINATOR,
             pcmd=CoordinatorResponseCommands.DISCOVERED_DEVICES,
             m_type=CoordinatorMessages.DISCOVERED_DEVICES,
             hwpid=hwpid,
             rcode=rcode,
             dpa_value=dpa_value,
             msgid=msgid,
             result=result
         )
-        if rcode == 0:
+        if rcode == ResponseCodes.OK:
             self._discovered = result['discoveredDevices']
 
     def get_discovered(self) -> List[int]:
         return self._discovered
 
     @staticmethod
     def from_dpa(dpa: bytes) -> DiscoveredDevicesResponse:
         IResponse.validate_dpa_response(dpa)
-        hwpid = Common.hwpid_from_dpa(dpa[5], dpa[4])
-        rcode = dpa[6]
+        hwpid = Common.hwpid_from_dpa(dpa[ResponsePacketMembers.HWPID_HI], dpa[ResponsePacketMembers.HWPID_LO])
+        rcode = dpa[ResponsePacketMembers.RCODE]
         result = None
-        if rcode == 0:
+        if rcode == ResponseCodes.OK:
             if len(dpa) != 40:
                 raise DpaResponsePacketLengthError('Invalid DPA response packet length.')
             result = {'discoveredDevices': Common.bitmap_to_nodes(list(dpa[8:]))}
-        return DiscoveredDevicesResponse(hwpid=hwpid, rcode=rcode, dpa_value=dpa[7], result=result)
+        return DiscoveredDevicesResponse(hwpid=hwpid, rcode=rcode, dpa_value=dpa[ResponsePacketMembers.DPA_VALUE],
+                                         result=result)
 
     @staticmethod
     def from_json(json: dict) -> DiscoveredDevicesResponse:
         msgid = Common.msgid_from_json(json)
         hwpid = Common.hwpid_from_json(json)
         dpa_value = Common.dpa_value_from_json(json)
         rcode = Common.rcode_from_json(json)
-        result = Common.result_from_json(json) if rcode == 0 else None
+        result = Common.result_from_json(json) if rcode == ResponseCodes.OK else None
         return DiscoveredDevicesResponse(msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode, result=result)
```

### Comparing `iqrfpy-0.1.5/iqrfpy/messages/responses/coordinator/Discovery.py` & `iqrfpy-0.1.6/iqrfpy/messages/responses/coordinator/BondNode.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,56 +1,62 @@
 from __future__ import annotations
 from typeguard import typechecked
 from typing import Optional
 from iqrfpy.messages.responses.IResponse import IResponse, IResponseGetterMixin
-from iqrfpy.enums.Commands import CoordinatorResponseCommands
-from iqrfpy.enums.MessageTypes import CoordinatorMessages
+from iqrfpy.enums.commands import CoordinatorResponseCommands
+from iqrfpy.enums.message_types import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
 from iqrfpy.exceptions import DpaResponsePacketLengthError
 from iqrfpy.utils.common import Common
+import iqrfpy.utils.dpa as DpaConstants
+from iqrfpy.utils.dpa import ResponseCodes, ResponsePacketMembers
 
-__all__ = ['DiscoveryResponse']
+__all__ = ['BondNodeResponse']
 
 
 @typechecked
-class DiscoveryResponse(IResponseGetterMixin):
-    __slots__ = '_disc_nr'
+class BondNodeResponse(IResponseGetterMixin):
+    __slots__ = '_bond_addr', '_dev_nr'
 
-    def __init__(self, hwpid: int = Common.HWPID_MAX, rcode: int = 0, dpa_value: int = 0,
+    def __init__(self, hwpid: int = DpaConstants.HWPID_MAX, rcode: int = 0, dpa_value: int = 0,
                  msgid: Optional[str] = None, result: Optional[dict] = None):
         super().__init__(
-            nadr=0,
+            nadr=DpaConstants.COORDINATOR_NADR,
             pnum=EmbedPeripherals.COORDINATOR,
-            pcmd=CoordinatorResponseCommands.DISCOVERY,
-            m_type=CoordinatorMessages.DISCOVERY,
+            pcmd=CoordinatorResponseCommands.BOND_NODE,
+            m_type=CoordinatorMessages.BOND_NODE,
             hwpid=hwpid,
             rcode=rcode,
             dpa_value=dpa_value,
             msgid=msgid,
             result=result
         )
-        if rcode == 0:
-            self._disc_nr = result['discNr']
+        if rcode == ResponseCodes.OK:
+            self._bond_addr = result['bondAddr']
+            self._dev_nr = result['devNr']
 
-    def get_disc_nr(self) -> int:
-        return self._disc_nr
+    def get_bond_addr(self) -> int:
+        return self._bond_addr
+
+    def get_dev_nr(self) -> int:
+        return self._dev_nr
 
     @staticmethod
-    def from_dpa(dpa: bytes) -> DiscoveryResponse:
+    def from_dpa(dpa: bytes) -> BondNodeResponse:
         IResponse.validate_dpa_response(dpa)
-        hwpid = Common.hwpid_from_dpa(dpa[5], dpa[4])
-        rcode = dpa[6]
+        hwpid = Common.hwpid_from_dpa(dpa[ResponsePacketMembers.HWPID_HI], dpa[ResponsePacketMembers.HWPID_LO])
+        rcode = dpa[ResponsePacketMembers.RCODE]
         result = None
-        if rcode == 0:
-            if len(dpa) != 9:
+        if rcode == ResponseCodes.OK:
+            if len(dpa) != 10:
                 raise DpaResponsePacketLengthError('Invalid DPA response packet length.')
-            result = {'discNr': dpa[8]}
-        return DiscoveryResponse(hwpid=hwpid, rcode=dpa[6], dpa_value=dpa[7], result=result)
+            result = {'bondAddr': dpa[8], 'devNr': dpa[9]}
+        return BondNodeResponse(hwpid=hwpid, rcode=rcode, dpa_value=dpa[ResponsePacketMembers.DPA_VALUE], result=result)
 
     @staticmethod
-    def from_json(json: dict) -> DiscoveryResponse:
+    def from_json(json: dict) -> BondNodeResponse:
         msgid = Common.msgid_from_json(json)
         hwpid = Common.hwpid_from_json(json)
         dpa_value = Common.dpa_value_from_json(json)
         rcode = Common.rcode_from_json(json)
-        result = Common.result_from_json(json) if rcode == 0 else None
-        return DiscoveryResponse(msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode, result=result)
+        result = Common.result_from_json(json) if rcode == ResponseCodes.OK else None
+        return BondNodeResponse(msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode, result=result)
```

### Comparing `iqrfpy-0.1.5/iqrfpy/messages/responses/coordinator/RemoveBond.py` & `iqrfpy-0.1.6/iqrfpy/messages/responses/coordinator/SetDpaParams.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,56 +1,60 @@
 from __future__ import annotations
 from typeguard import typechecked
 from typing import Optional
 from iqrfpy.messages.responses.IResponse import IResponse, IResponseGetterMixin
-from iqrfpy.enums.Commands import CoordinatorResponseCommands
-from iqrfpy.enums.MessageTypes import CoordinatorMessages
+from iqrfpy.messages.requests.coordinator.SetDpaParams import DpaParam
+from iqrfpy.enums.commands import CoordinatorResponseCommands
+from iqrfpy.enums.message_types import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
 from iqrfpy.exceptions import DpaResponsePacketLengthError
 from iqrfpy.utils.common import Common
+import iqrfpy.utils.dpa as DpaConstants
+from iqrfpy.utils.dpa import ResponseCodes, ResponsePacketMembers
 
-__all__ = ['RemoveBondResponse']
+__all__ = ['SetDpaParamsResponse']
 
 
 @typechecked
-class RemoveBondResponse(IResponseGetterMixin):
-    __slots__ = '_dev_nr'
+class SetDpaParamsResponse(IResponseGetterMixin):
+    __slots__ = '_dpa_param'
 
-    def __init__(self, hwpid: int = Common.HWPID_MAX, rcode: int = 0, dpa_value: int = 0,
+    def __init__(self, hwpid: int = DpaConstants.HWPID_MAX, rcode: int = 0, dpa_value: int = 0,
                  msgid: Optional[str] = None, result: Optional[dict] = None):
         super().__init__(
-            nadr=0,
+            nadr=DpaConstants.COORDINATOR_NADR,
             pnum=EmbedPeripherals.COORDINATOR,
-            pcmd=CoordinatorResponseCommands.REMOVE_BOND,
-            m_type=CoordinatorMessages.REMOVE_BOND,
+            pcmd=CoordinatorResponseCommands.SET_DPA_PARAMS,
+            m_type=CoordinatorMessages.SET_DPA_PARAMS,
             hwpid=hwpid,
             rcode=rcode,
             dpa_value=dpa_value,
             msgid=msgid,
             result=result
         )
-        if rcode == 0:
-            self._dev_nr = result['devNr']
+        if rcode == ResponseCodes.OK:
+            self._dpa_param: DpaParam = DpaParam(result['prevDpaParam'])
 
-    def get_dev_nr(self) -> int:
-        return self._dev_nr
+    def get_dpa_param(self) -> DpaParam:
+        return self._dpa_param
 
     @staticmethod
-    def from_dpa(dpa: bytes) -> RemoveBondResponse:
+    def from_dpa(dpa: bytes) -> SetDpaParamsResponse:
         IResponse.validate_dpa_response(dpa)
-        hwpid = Common.hwpid_from_dpa(dpa[5], dpa[4])
-        rcode = dpa[6]
+        hwpid = Common.hwpid_from_dpa(dpa[ResponsePacketMembers.HWPID_HI], dpa[ResponsePacketMembers.HWPID_LO])
+        rcode = dpa[ResponsePacketMembers.RCODE]
         result = None
-        if rcode == 0:
+        if rcode == ResponseCodes.OK:
             if len(dpa) != 9:
                 raise DpaResponsePacketLengthError('Invalid DPA response packet length.')
-            result = {'devNr': dpa[8]}
-        return RemoveBondResponse(hwpid=hwpid, rcode=dpa[6], dpa_value=dpa[7], result=result)
+            result = {'prevDpaParam': dpa[8]}
+        return SetDpaParamsResponse(hwpid=hwpid, rcode=rcode, dpa_value=dpa[ResponsePacketMembers.DPA_VALUE],
+                                    result=result)
 
     @staticmethod
-    def from_json(json: dict) -> RemoveBondResponse:
+    def from_json(json: dict) -> SetDpaParamsResponse:
         msgid = Common.msgid_from_json(json)
         hwpid = Common.hwpid_from_json(json)
         dpa_value = Common.dpa_value_from_json(json)
         rcode = Common.rcode_from_json(json)
-        result = Common.result_from_json(json) if rcode == 0 else None
-        return RemoveBondResponse(msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode, result=result)
+        result = Common.result_from_json(json) if rcode == ResponseCodes.OK else None
+        return SetDpaParamsResponse(msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode, result=result)
```

### Comparing `iqrfpy-0.1.5/iqrfpy/messages/responses/coordinator/Restore.py` & `iqrfpy-0.1.6/iqrfpy/messages/responses/coordinator/Restore.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,47 @@
 from __future__ import annotations
 from typeguard import typechecked
 from typing import Optional
 from iqrfpy.messages.responses.IResponse import IResponse, IResponseGetterMixin
-from iqrfpy.enums.Commands import CoordinatorResponseCommands
-from iqrfpy.enums.MessageTypes import CoordinatorMessages
+from iqrfpy.enums.commands import CoordinatorResponseCommands
+from iqrfpy.enums.message_types import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
 from iqrfpy.exceptions import DpaResponsePacketLengthError
 from iqrfpy.utils.common import Common
+import iqrfpy.utils.dpa as DpaConstants
+from iqrfpy.utils.dpa import ResponsePacketMembers
 
 __all__ = ['RestoreResponse']
 
 
 @typechecked
 class RestoreResponse(IResponseGetterMixin):
 
-    def __init__(self, hwpid: int = Common.HWPID_MAX, rcode: int = 0, dpa_value: int = 0,
+    def __init__(self, hwpid: int = DpaConstants.HWPID_MAX, rcode: int = 0, dpa_value: int = 0,
                  msgid: Optional[str] = None, result: Optional[dict] = None):
         super().__init__(
-            nadr=0,
+            nadr=DpaConstants.COORDINATOR_NADR,
             pnum=EmbedPeripherals.COORDINATOR,
             pcmd=CoordinatorResponseCommands.RESTORE,
             m_type=CoordinatorMessages.RESTORE,
             hwpid=hwpid,
             rcode=rcode,
             dpa_value=dpa_value,
             msgid=msgid,
             result=result
         )
 
     @staticmethod
     def from_dpa(dpa: bytes) -> RestoreResponse:
         IResponse.validate_dpa_response(dpa)
-        hwpid = Common.hwpid_from_dpa(dpa[5], dpa[4])
+        hwpid = Common.hwpid_from_dpa(dpa[ResponsePacketMembers.HWPID_HI], dpa[ResponsePacketMembers.HWPID_LO])
+        rcode = dpa[ResponsePacketMembers.RCODE]
         if len(dpa) != 8:
             raise DpaResponsePacketLengthError('Invalid DPA response packet length.')
-        return RestoreResponse(hwpid=hwpid, rcode=dpa[6], dpa_value=dpa[7], result=None)
+        return RestoreResponse(hwpid=hwpid, rcode=rcode, dpa_value=dpa[ResponsePacketMembers.DPA_VALUE], result=None)
 
     @staticmethod
     def from_json(json: dict) -> RestoreResponse:
         msgid = Common.msgid_from_json(json)
         hwpid = Common.hwpid_from_json(json)
         dpa_value = Common.dpa_value_from_json(json)
         rcode = Common.rcode_from_json(json)
```

### Comparing `iqrfpy-0.1.5/iqrfpy/messages/responses/coordinator/SetDpaParams.py` & `iqrfpy-0.1.6/iqrfpy/messages/responses/coordinator/SetHops.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,57 +1,62 @@
 from __future__ import annotations
 from typeguard import typechecked
 from typing import Optional
 from iqrfpy.messages.responses.IResponse import IResponse, IResponseGetterMixin
-from iqrfpy.messages.requests.coordinator.SetDpaParams import DpaParam
-from iqrfpy.enums.Commands import CoordinatorResponseCommands
-from iqrfpy.enums.MessageTypes import CoordinatorMessages
+from iqrfpy.enums.commands import CoordinatorResponseCommands
+from iqrfpy.enums.message_types import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
 from iqrfpy.exceptions import DpaResponsePacketLengthError
 from iqrfpy.utils.common import Common
+import iqrfpy.utils.dpa as DpaConstants
+from iqrfpy.utils.dpa import ResponseCodes, ResponsePacketMembers
 
-__all__ = ['SetDpaParamsResponse']
+__all__ = ['SetHopsResponse']
 
 
 @typechecked
-class SetDpaParamsResponse(IResponseGetterMixin):
-    __slots__ = '_dpa_param'
+class SetHopsResponse(IResponseGetterMixin):
+    __slots__ = '_request_hops', '_response_hops'
 
-    def __init__(self, hwpid: int = Common.HWPID_MAX, rcode: int = 0, dpa_value: int = 0,
+    def __init__(self, hwpid: int = DpaConstants.HWPID_MAX, rcode: int = 0, dpa_value: int = 0,
                  msgid: Optional[str] = None, result: Optional[dict] = None):
         super().__init__(
-            nadr=0,
+            nadr=DpaConstants.COORDINATOR_NADR,
             pnum=EmbedPeripherals.COORDINATOR,
-            pcmd=CoordinatorResponseCommands.SET_DPA_PARAMS,
-            m_type=CoordinatorMessages.SET_DPA_PARAMS,
+            pcmd=CoordinatorResponseCommands.SET_HOPS,
+            m_type=CoordinatorMessages.SET_HOPS,
             hwpid=hwpid,
             rcode=rcode,
             dpa_value=dpa_value,
             msgid=msgid,
             result=result
         )
-        if rcode == 0:
-            self._dpa_param: DpaParam = DpaParam(result['prevDpaParam'])
+        if rcode == ResponseCodes.OK:
+            self._request_hops = result['requestHops']
+            self._response_hops = result['responseHops']
 
-    def get_dpa_param(self) -> DpaParam:
-        return self._dpa_param
+    def get_request_hops(self) -> int:
+        return self._request_hops
+
+    def get_response_hops(self) -> int:
+        return self._response_hops
 
     @staticmethod
-    def from_dpa(dpa: bytes) -> SetDpaParamsResponse:
+    def from_dpa(dpa: bytes) -> SetHopsResponse:
         IResponse.validate_dpa_response(dpa)
-        hwpid = Common.hwpid_from_dpa(dpa[5], dpa[4])
-        rcode = dpa[6]
+        hwpid = Common.hwpid_from_dpa(dpa[ResponsePacketMembers.HWPID_HI], dpa[ResponsePacketMembers.HWPID_LO])
+        rcode = dpa[ResponsePacketMembers.RCODE]
         result = None
-        if rcode == 0:
-            if len(dpa) != 9:
+        if rcode == ResponseCodes.OK:
+            if len(dpa) != 10:
                 raise DpaResponsePacketLengthError('Invalid DPA response packet length.')
-            result = {'prevDpaParam': dpa[8]}
-        return SetDpaParamsResponse(hwpid=hwpid, rcode=dpa[6], dpa_value=dpa[7], result=result)
+            result = {'requestHops': dpa[8], 'responseHops': dpa[9]}
+        return SetHopsResponse(hwpid=hwpid, rcode=rcode, dpa_value=dpa[ResponsePacketMembers.DPA_VALUE], result=result)
 
     @staticmethod
-    def from_json(json: dict) -> SetDpaParamsResponse:
+    def from_json(json: dict) -> SetHopsResponse:
         msgid = Common.msgid_from_json(json)
         hwpid = Common.hwpid_from_json(json)
         dpa_value = Common.dpa_value_from_json(json)
         rcode = Common.rcode_from_json(json)
-        result = Common.result_from_json(json) if rcode == 0 else None
-        return SetDpaParamsResponse(msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode, result=result)
+        result = Common.result_from_json(json) if rcode == ResponseCodes.OK else None
+        return SetHopsResponse(msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode, result=result)
```

### Comparing `iqrfpy-0.1.5/iqrfpy/messages/responses/coordinator/SetHops.py` & `iqrfpy-0.1.6/iqrfpy/messages/responses/node/Read.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,60 +1,64 @@
 from __future__ import annotations
-from typeguard import typechecked
 from typing import Optional
 from iqrfpy.messages.responses.IResponse import IResponse, IResponseGetterMixin
-from iqrfpy.enums.Commands import CoordinatorResponseCommands
-from iqrfpy.enums.MessageTypes import CoordinatorMessages
+from iqrfpy.enums.commands import NodeResponseCommands
+from iqrfpy.enums.message_types import NodeMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
 from iqrfpy.exceptions import DpaResponsePacketLengthError
 from iqrfpy.utils.common import Common
 
-__all__ = ['SetHopsResponse']
+__all__ = ['ReadResponse']
 
 
-@typechecked
-class SetHopsResponse(IResponseGetterMixin):
-    __slots__ = '_request_hops', '_response_hops'
+class ReadResponse(IResponseGetterMixin):
+    __slots__ = '_ntw_addr', '_ntw_vrn', '_ntw_zin', '_ntw_did', '_ntw_pvrn', '_ntw_useraddr', '_ntw_id', \
+        '_ntw_vrnfnz', '_ntw_cfg', '_flags'
 
-    def __init__(self, hwpid: int = Common.HWPID_MAX, rcode: int = 0, dpa_value: int = 0,
+    def __init__(self, nadr: int, hwpid: Common.HWPID_MAX, rcode: int = 0, dpa_value: int = 0,
                  msgid: Optional[str] = None, result: Optional[dict] = None):
         super().__init__(
-            nadr=0,
-            pnum=EmbedPeripherals.COORDINATOR,
-            pcmd=CoordinatorResponseCommands.SET_HOPS,
-            m_type=CoordinatorMessages.SET_HOPS,
+            nadr=nadr,
+            pnum=EmbedPeripherals.NODE,
+            pcmd=NodeResponseCommands.READ,
+            m_type=NodeMessages.READ,
             hwpid=hwpid,
             rcode=rcode,
             dpa_value=dpa_value,
             msgid=msgid,
             result=result
         )
         if rcode == 0:
-            self._request_hops = result['requestHops']
-            self._response_hops = result['responseHops']
-
-    def get_request_hops(self) -> int:
-        return self._request_hops
-
-    def get_response_hops(self) -> int:
-        return self._response_hops
+            self._ntw_addr = result['ntwADDR']
+            self._ntw_vrn = result['ntwVRN']
+            self._ntw_zin = result['ntwZIN']
+            self._ntw_did = result['ntwDID']
+            self._ntw_pvrn = result['ntwPVRN']
+            self._ntw_useraddr = result['ntwUSERADDRESS']
+            self._ntw_id = result['ntwID']
+            self._ntw_vrnfnz = result['ntwVRNFNZ']
+            self._ntw_cfg = result['ntwCFG']
+            self._flags = result['flags']
 
     @staticmethod
-    def from_dpa(dpa: bytes) -> SetHopsResponse:
+    def from_dpa(dpa: bytes) -> ReadResponse:
         IResponse.validate_dpa_response(dpa)
         hwpid = Common.hwpid_from_dpa(dpa[5], dpa[4])
         rcode = dpa[6]
         result = None
         if rcode == 0:
             if len(dpa) != 10:
                 raise DpaResponsePacketLengthError('Invalid DPA response packet length.')
-            result = {'requestHops': dpa[8], 'responseHops': dpa[9]}
-        return SetHopsResponse(hwpid=hwpid, rcode=dpa[6], dpa_value=dpa[7], result=result)
+            result = {
+
+            }
+        return ReadResponse(nadr=dpa[0], hwpid=hwpid, rcode=rcode, dpa_value=dpa[7], result=result)
 
     @staticmethod
-    def from_json(json: dict) -> SetHopsResponse:
+    def from_json(json: dict) -> ReadResponse:
+        nadr = Common.nadr_from_json(json)
         msgid = Common.msgid_from_json(json)
         hwpid = Common.hwpid_from_json(json)
         dpa_value = Common.dpa_value_from_json(json)
         rcode = Common.rcode_from_json(json)
         result = Common.result_from_json(json) if rcode == 0 else None
-        return SetHopsResponse(msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode, result=result)
+        return ReadResponse(nadr=nadr, msgid=msgid, hwpid=hwpid, rcode=rcode, dpa_value=dpa_value, result=result)
```

### Comparing `iqrfpy-0.1.5/iqrfpy/messages/responses/coordinator/SetMID.py` & `iqrfpy-0.1.6/iqrfpy/messages/responses/coordinator/BondedDevices.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,45 +1,59 @@
 from __future__ import annotations
 from typeguard import typechecked
-from typing import Optional
-from iqrfpy.messages.responses.IResponse import IResponse, IResponseGetterMixin
-from iqrfpy.enums.Commands import CoordinatorResponseCommands
-from iqrfpy.enums.MessageTypes import CoordinatorMessages
+from typing import List, Optional
+from iqrfpy.enums.commands import CoordinatorResponseCommands
+from iqrfpy.enums.message_types import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
 from iqrfpy.exceptions import DpaResponsePacketLengthError
 from iqrfpy.utils.common import Common
+import iqrfpy.utils.dpa as DpaConstants
+from iqrfpy.utils.dpa import ResponseCodes, ResponsePacketMembers
+from iqrfpy.messages.responses.IResponse import IResponse, IResponseGetterMixin
 
-__all__ = ['SetMIDResponse']
+__all__ = ['BondedDevicesResponse']
 
 
 @typechecked
-class SetMIDResponse(IResponseGetterMixin):
+class BondedDevicesResponse(IResponseGetterMixin):
+    __slots__ = '_bonded'
 
-    def __init__(self, hwpid: int = Common.HWPID_MAX, rcode: int = 0, dpa_value: int = 0,
+    def __init__(self, hwpid: int = DpaConstants.HWPID_MAX, rcode: int = 0, dpa_value: int = 0,
                  msgid: Optional[str] = None, result: Optional[dict] = None):
         super().__init__(
-            nadr=0,
+            nadr=DpaConstants.COORDINATOR_NADR,
             pnum=EmbedPeripherals.COORDINATOR,
-            pcmd=CoordinatorResponseCommands.SET_MID,
-            m_type=CoordinatorMessages.SET_MID,
+            pcmd=CoordinatorResponseCommands.BONDED_DEVICES,
+            m_type=CoordinatorMessages.BONDED_DEVICES,
             hwpid=hwpid,
             rcode=rcode,
             dpa_value=dpa_value,
             msgid=msgid,
             result=result
         )
+        if rcode == ResponseCodes.OK:
+            self._bonded = result['bondedDevices']
+
+    def get_bonded(self) -> List[int]:
+        return self._bonded
 
     @staticmethod
-    def from_dpa(dpa: bytes) -> SetMIDResponse:
+    def from_dpa(dpa: bytes) -> BondedDevicesResponse:
         IResponse.validate_dpa_response(dpa)
-        hwpid = Common.hwpid_from_dpa(dpa[5], dpa[4])
-        if len(dpa) != 8:
-            raise DpaResponsePacketLengthError('Invalid DPA response packet length.')
-        return SetMIDResponse(hwpid=hwpid, rcode=dpa[6], dpa_value=dpa[7], result=None)
+        hwpid = Common.hwpid_from_dpa(dpa[ResponsePacketMembers.HWPID_HI], dpa[ResponsePacketMembers.HWPID_LO])
+        rcode = dpa[ResponsePacketMembers.RCODE]
+        result = None
+        if rcode == ResponseCodes.OK:
+            if len(dpa) != 40:
+                raise DpaResponsePacketLengthError('Invalid DPA response packet length.')
+            result = {'bondedDevices': Common.bitmap_to_nodes(list(dpa[8:]))}
+        return BondedDevicesResponse(hwpid=hwpid, rcode=rcode, dpa_value=dpa[ResponsePacketMembers.DPA_VALUE],
+                                     result=result)
 
     @staticmethod
-    def from_json(json: dict) -> SetMIDResponse:
+    def from_json(json: dict) -> BondedDevicesResponse:
         msgid = Common.msgid_from_json(json)
         hwpid = Common.hwpid_from_json(json)
         dpa_value = Common.dpa_value_from_json(json)
         rcode = Common.rcode_from_json(json)
-        return SetMIDResponse(msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode, result=None)
+        result = Common.result_from_json(json) if rcode == ResponseCodes.OK else None
+        return BondedDevicesResponse(msgid=msgid, hwpid=hwpid, dpa_value=dpa_value, rcode=rcode, result=result)
```

### Comparing `iqrfpy-0.1.5/iqrfpy/messages/responses/coordinator/__init__.py` & `iqrfpy-0.1.6/iqrfpy/messages/responses/coordinator/__init__.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.5/iqrfpy/transports/itransport.py` & `iqrfpy-0.1.6/iqrfpy/transports/itransport.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.5/iqrfpy/transports/mqtt_transport.py` & `iqrfpy-0.1.6/iqrfpy/transports/mqtt_transport.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.5/iqrfpy/transports/udp_transport.py` & `iqrfpy-0.1.6/iqrfpy/transports/udp_transport.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.5/iqrfpy/utils/common.py` & `iqrfpy-0.1.6/iqrfpy/utils/common.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,21 +8,22 @@
 """
 
 __all__ = ['Common']
 
 import math
 from typing import List
 from typeguard import typechecked
-from iqrfpy.enums.Commands import *
-from iqrfpy.enums.MessageTypes import *
+from iqrfpy.enums.commands import *
+from iqrfpy.enums.message_types import *
 from iqrfpy.enums.peripherals import *
 from iqrfpy.exceptions import InvalidPeripheralValueError, InvalidPeripheralCommandValueError, \
     JsonMsgidMissingError, JsonMTypeMissingError, JsonNadrMissingError, JsonHwpidMissingError, JsonRCodeMissingError, \
     JsonDpaValueMissingError, JsonResultMissingError, JsonStatusMissingError, UnsupportedMessageTypeError, \
     UnsupportedPeripheralError, UnsupportedPeripheralCommandError
+import iqrfpy.utils.dpa as DpaConstants
 
 
 @typechecked
 class Common:
     """
     Common class provides static methods for handling, modification and extraction of information
     from DPA and Daemon API JSON messages.
@@ -65,18 +66,14 @@
         Check if string contains only hexadecimal characters.
     hex_string_to_list(string: str) -> List[int]:
         Convert hexadecimal string to list of unsigned integers.
     values_in_byte_range(values: List[int]) -> bool:
         Check if list elements are within unsigned integer byte range.
     """
 
-    IQMESH_TEMP_ADDR = 0xFE
-    PNUM_MAX = 0x7F
-    HWPID_MAX = 0xFFFF
-
     # DPA
 
     @staticmethod
     def hwpid_from_dpa(upper: int, lower: int) -> int:
         """
         Convert DPA HWPID bytes to a single 16bit unsigned integer.
 
@@ -93,17 +90,17 @@
             16bit unsigned integer HWPID value
 
         Raises
         ------
         ValueError
             Raised if input values are not between 0 and 255
         """
-        if upper > 255 or lower > 255:
+        if upper > DpaConstants.BYTE_MAX or lower > DpaConstants.BYTE_MAX:
             raise ValueError('Argument value exceeds maximum allowed value of 255.')
-        if upper < 0 or lower < 0:
+        if upper < DpaConstants.BYTE_MIN or lower < DpaConstants.BYTE_MIN:
             raise ValueError('Negative argument values are not allowed.')
         return (upper << 8) + lower
 
     @staticmethod
     def pnum_from_dpa(pnum: int) -> Peripheral:
         """
         Return peripheral enum value based on DPA peripheral data byte.
@@ -153,17 +150,17 @@
         ------
         ValueError
             Raised if pcmd is a negative value
             Raised if pcmd is not a value between 0 and 127
             Raised if peripheral is not a recognized peripheral value
             Raised if pcmd is not a recognized peripheral command
         """
-        if pcmd < 0:
+        if pcmd < DpaConstants.REQUEST_PCMD_MIN:
             raise InvalidPeripheralCommandValueError('Negative peripheral command values are not allowed.')
-        if pcmd > Common.PNUM_MAX:
+        if pcmd > DpaConstants.REQUEST_PCMD_MAX:
             raise InvalidPeripheralCommandValueError('Peripheral command value exceeds maximum allowed value of 127.')
         commands = None
         match pnum:
             case EmbedPeripherals.COORDINATOR:
                 commands = CoordinatorRequestCommands
             case EmbedPeripherals.NODE:
                 commands = NodeRequestCommands
@@ -221,17 +218,17 @@
         ------
         ValueError
             Raised if pcmd is a negative value
             Raised if pcmd is not a value between 128 and 255
             Raised if peripheral is not a recognized peripheral value
             Raised if pcmd is not a recognized peripheral command
         """
-        if pcmd < 0:
+        if pcmd < DpaConstants.REQUEST_PCMD_MIN:
             raise InvalidPeripheralCommandValueError('Negative peripheral command values are not allowed.')
-        if pcmd <= Common.PNUM_MAX or pcmd > 255:
+        if pcmd <= DpaConstants.REQUEST_PCMD_MAX or pcmd > DpaConstants.RESPONSE_PCMD_MAX:
             raise InvalidPeripheralCommandValueError('Response peripheral command should be value between 128 and 255.')
         commands = None
         match pnum:
             case EmbedPeripherals.COORDINATOR:
                 commands = CoordinatorResponseCommands
             case EmbedPeripherals.NODE:
                 commands = NodeResponseCommands
```

### Comparing `iqrfpy-0.1.5/iqrfpy.egg-info/PKG-INFO` & `iqrfpy-0.1.6/iqrfpy.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iqrfpy
-Version: 0.1.5
+Version: 0.1.6
 Summary: A python library for communication with IQRF Network
 Home-page: https://gitlab.iqrf.org/microrisc/libiqrf-python
 Author: Karel Hanák
 Author-email: karel.hanak@iqrf.org
 License: Apache-2.0
 Keywords: iqrf,dpa
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `iqrfpy-0.1.5/iqrfpy.egg-info/SOURCES.txt` & `iqrfpy-0.1.6/iqrfpy.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 .editorconfig
 .gitignore
 .gitlab-ci.yml
 .pylintrc
 LICENSE
 Makefile
 README.md
-example.py
 pyproject.toml
 requirements.txt
 setup.cfg
 test_requirements.txt
 tox.ini
 examples/response_factories.py
 iqrfpy/__init__.py
 iqrfpy/exceptions.py
 iqrfpy.egg-info/PKG-INFO
 iqrfpy.egg-info/SOURCES.txt
 iqrfpy.egg-info/dependency_links.txt
 iqrfpy.egg-info/requires.txt
 iqrfpy.egg-info/top_level.txt
-iqrfpy/enums/Commands.py
-iqrfpy/enums/MessageTypes.py
 iqrfpy/enums/__init__.py
+iqrfpy/enums/commands.py
+iqrfpy/enums/message_types.py
 iqrfpy/enums/peripherals.py
 iqrfpy/messages/__init__.py
 iqrfpy/messages/response_factory.py
 iqrfpy/messages/requests/IRequest.py
 iqrfpy/messages/requests/__init__.py
 iqrfpy/messages/requests/binaryoutput/__init__.py
 iqrfpy/messages/requests/coordinator/AddrInfo.py
@@ -81,15 +80,17 @@
 iqrfpy/messages/responses/coordinator/SetHops.py
 iqrfpy/messages/responses/coordinator/SetMID.py
 iqrfpy/messages/responses/coordinator/SmartConnect.py
 iqrfpy/messages/responses/coordinator/__init__.py
 iqrfpy/messages/responses/dali/__init__.py
 iqrfpy/messages/responses/eeeprom/__init__.py
 iqrfpy/messages/responses/eeprom/__init__.py
+iqrfpy/messages/responses/exploration/__init__.py
 iqrfpy/messages/responses/frc/__init__.py
+iqrfpy/messages/responses/generic/__init__.py
 iqrfpy/messages/responses/io/__init__.py
 iqrfpy/messages/responses/ledg/__init__.py
 iqrfpy/messages/responses/ledr/__init__.py
 iqrfpy/messages/responses/light/__init__.py
 iqrfpy/messages/responses/node/Read.py
 iqrfpy/messages/responses/node/__init__.py
 iqrfpy/messages/responses/os/__init__.py
@@ -99,14 +100,15 @@
 iqrfpy/messages/responses/uart/__init__.py
 iqrfpy/transports/__init__.py
 iqrfpy/transports/itransport.py
 iqrfpy/transports/mqtt_transport.py
 iqrfpy/transports/udp_transport.py
 iqrfpy/utils/__init__.py
 iqrfpy/utils/common.py
+iqrfpy/utils/dpa.py
 iqrfpy/utils/enums.py
 tests/__init__.py
 tests/enums/Peripherals_test.py
 tests/messages/response_factory_test.py
 tests/messages/requests/IRequest_test.py
 tests/messages/requests/coordinator/AddrInfoRequest_test.py
 tests/messages/requests/coordinator/AuthorizeBondRequest_test.py
```

### Comparing `iqrfpy-0.1.5/setup.cfg` & `iqrfpy-0.1.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.5/tests/enums/Peripherals_test.py` & `iqrfpy-0.1.6/tests/enums/Peripherals_test.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.5/tests/messages/requests/IRequest_test.py` & `iqrfpy-0.1.6/tests/messages/requests/IRequest_test.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.5/tests/messages/requests/coordinator/AddrInfoRequest_test.py` & `iqrfpy-0.1.6/tests/messages/requests/coordinator/AddrInfoRequest_test.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.5/tests/messages/requests/coordinator/AuthorizeBondRequest_test.py` & `iqrfpy-0.1.6/tests/messages/requests/coordinator/AuthorizeBondRequest_test.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.5/tests/messages/requests/coordinator/BackupRequest_test.py` & `iqrfpy-0.1.6/tests/messages/requests/coordinator/BackupRequest_test.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.5/tests/messages/requests/coordinator/BondNodeRequest_test.py` & `iqrfpy-0.1.6/tests/messages/requests/coordinator/BondNodeRequest_test.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.5/tests/messages/requests/coordinator/BondedDevicesRequest_test.py` & `iqrfpy-0.1.6/tests/messages/requests/coordinator/BondedDevicesRequest_test.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.5/tests/messages/requests/coordinator/ClearAllBondsRequest_test.py` & `iqrfpy-0.1.6/tests/messages/requests/coordinator/ClearAllBondsRequest_test.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.5/tests/messages/requests/coordinator/DiscoveredDevicesRequest_test.py` & `iqrfpy-0.1.6/tests/messages/requests/coordinator/DiscoveredDevicesRequest_test.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.5/tests/messages/requests/coordinator/DiscoveryRequest_test.py` & `iqrfpy-0.1.6/tests/messages/requests/coordinator/DiscoveryRequest_test.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.5/tests/messages/requests/coordinator/RemoveBondRequest_test.py` & `iqrfpy-0.1.6/tests/messages/requests/coordinator/RemoveBondRequest_test.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.5/tests/messages/requests/coordinator/RestoreRequest_test.py` & `iqrfpy-0.1.6/tests/messages/requests/coordinator/RestoreRequest_test.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.5/tests/messages/requests/coordinator/SetDpaParamsRequest_test.py` & `iqrfpy-0.1.6/tests/messages/requests/coordinator/SetDpaParamsRequest_test.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.5/tests/messages/requests/coordinator/SetHopsRequest_test.py` & `iqrfpy-0.1.6/tests/messages/requests/coordinator/SetHopsRequest_test.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.5/tests/messages/requests/coordinator/SetMIDRequest_test.py` & `iqrfpy-0.1.6/tests/messages/requests/coordinator/SetMIDRequest_test.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.5/tests/messages/requests/coordinator/SmartConnectRequest_test.py` & `iqrfpy-0.1.6/tests/messages/requests/coordinator/SmartConnectRequest_test.py`

 * *Files identical despite different names*

### Comparing `iqrfpy-0.1.5/tests/messages/response_factory_test.py` & `iqrfpy-0.1.6/tests/messages/response_factory_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import unittest
 from parameterized import parameterized
-from iqrfpy.enums.MessageTypes import *
+from iqrfpy.enums.message_types import *
 from iqrfpy.exceptions import JsonMsgidMissingError, JsonMTypeMissingError, UnsupportedMessageTypeError
 from iqrfpy.messages.response_factory import *
 from iqrfpy.messages.responses.AsyncResponse import AsyncResponse
 from iqrfpy.messages.responses.Confirmation import Confirmation
 from iqrfpy.messages.responses.coordinator import *
```

### Comparing `iqrfpy-0.1.5/tests/messages/responses/AsyncResponse_test.py` & `iqrfpy-0.1.6/tests/messages/responses/AsyncResponse_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import unittest
 from parameterized import parameterized
-from iqrfpy.enums.Commands import ExplorationRequestCommands
-from iqrfpy.enums.MessageTypes import GenericMessages
+from iqrfpy.enums.commands import ExplorationRequestCommands
+from iqrfpy.enums.message_types import GenericMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
 from iqrfpy.messages.responses.AsyncResponse import AsyncResponse
 
 data_ok: dict = {
     'msgid': 'async',
     'nadr': 0,
     'hwpid': 0,
```

### Comparing `iqrfpy-0.1.5/tests/messages/responses/Confirmation_test.py` & `iqrfpy-0.1.6/tests/messages/responses/Confirmation_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import unittest
-from iqrfpy.enums.Commands import NodeRequestCommands
+from iqrfpy.enums.commands import NodeRequestCommands
 from iqrfpy.enums.peripherals import EmbedPeripherals
 from iqrfpy.messages.responses.Confirmation import Confirmation
 
 
 class ConfirmationTestCase(unittest.TestCase):
 
     def test_from_dpa_ok(self):
```

### Comparing `iqrfpy-0.1.5/tests/messages/responses/coordinator/AddrInfoResponse_test.py` & `iqrfpy-0.1.6/tests/messages/responses/coordinator/AddrInfoResponse_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import unittest
 from parameterized import parameterized
-from iqrfpy.enums.Commands import CoordinatorResponseCommands
-from iqrfpy.enums.MessageTypes import CoordinatorMessages
+from iqrfpy.enums.commands import CoordinatorResponseCommands
+from iqrfpy.enums.message_types import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
 from iqrfpy.messages.responses.coordinator.AddrInfo import AddrInfoResponse
 
 data_ok: dict = {
     'msgid': 'addrInfoTest',
     'nadr': 0,
     'hwpid': 0,
```

### Comparing `iqrfpy-0.1.5/tests/messages/responses/coordinator/AuthorizeBondResponse_test.py` & `iqrfpy-0.1.6/tests/messages/responses/coordinator/AuthorizeBondResponse_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import unittest
 from parameterized import parameterized
-from iqrfpy.enums.Commands import CoordinatorResponseCommands
-from iqrfpy.enums.MessageTypes import CoordinatorMessages
+from iqrfpy.enums.commands import CoordinatorResponseCommands
+from iqrfpy.enums.message_types import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
 from iqrfpy.messages.responses.coordinator.AuthorizeBond import AuthorizeBondResponse
 
 data_ok: dict = {
     'msgid': 'authorizeBondTest',
     'nadr': 0,
     'hwpid': 0,
```

### Comparing `iqrfpy-0.1.5/tests/messages/responses/coordinator/BackupResponse_test.py` & `iqrfpy-0.1.6/tests/messages/responses/coordinator/BackupResponse_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import unittest
 from parameterized import parameterized
-from iqrfpy.enums.Commands import CoordinatorResponseCommands
-from iqrfpy.enums.MessageTypes import CoordinatorMessages
+from iqrfpy.enums.commands import CoordinatorResponseCommands
+from iqrfpy.enums.message_types import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
 from iqrfpy.messages.responses.coordinator.Backup import BackupResponse
 
 data_ok: dict = {
     'msgid': 'backupTest',
     'nadr': 0,
     'hwpid': 0,
```

### Comparing `iqrfpy-0.1.5/tests/messages/responses/coordinator/BondNodeResponse_test.py` & `iqrfpy-0.1.6/tests/messages/responses/coordinator/BondNodeResponse_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import unittest
 from parameterized import parameterized
-from iqrfpy.enums.Commands import CoordinatorResponseCommands
-from iqrfpy.enums.MessageTypes import CoordinatorMessages
+from iqrfpy.enums.commands import CoordinatorResponseCommands
+from iqrfpy.enums.message_types import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
 from iqrfpy.messages.responses.coordinator.BondNode import BondNodeResponse
 
 data_ok: dict = {
     'msgid': 'bondNodeTest',
     'nadr': 0,
     'hwpid': 0,
```

### Comparing `iqrfpy-0.1.5/tests/messages/responses/coordinator/BondedDevicesResponse_test.py` & `iqrfpy-0.1.6/tests/messages/responses/coordinator/BondedDevicesResponse_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import unittest
 from parameterized import parameterized
-from iqrfpy.enums.Commands import CoordinatorResponseCommands
-from iqrfpy.enums.MessageTypes import CoordinatorMessages
+from iqrfpy.enums.commands import CoordinatorResponseCommands
+from iqrfpy.enums.message_types import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
 from iqrfpy.messages.responses.coordinator.BondedDevices import BondedDevicesResponse
 
 data_ok: dict = {
     'msgid': 'bondedDevicesTest',
     'nadr': 0,
     'hwpid': 0,
```

### Comparing `iqrfpy-0.1.5/tests/messages/responses/coordinator/ClearAllBondsResponse_test.py` & `iqrfpy-0.1.6/tests/messages/responses/coordinator/ClearAllBondsResponse_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import unittest
 from parameterized import parameterized
-from iqrfpy.enums.Commands import CoordinatorResponseCommands
-from iqrfpy.enums.MessageTypes import CoordinatorMessages
+from iqrfpy.enums.commands import CoordinatorResponseCommands
+from iqrfpy.enums.message_types import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
 from iqrfpy.messages.responses.coordinator.ClearAllBonds import ClearAllBondsResponse
 
 data_ok: dict = {
     'msgid': 'clearAllBondsTest',
     'nadr': 0,
     'hwpid': 0,
```

### Comparing `iqrfpy-0.1.5/tests/messages/responses/coordinator/DiscoveredDevicesResponse_test.py` & `iqrfpy-0.1.6/tests/messages/responses/coordinator/DiscoveredDevicesResponse_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import unittest
 from parameterized import parameterized
-from iqrfpy.enums.Commands import CoordinatorResponseCommands
-from iqrfpy.enums.MessageTypes import CoordinatorMessages
+from iqrfpy.enums.commands import CoordinatorResponseCommands
+from iqrfpy.enums.message_types import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
 from iqrfpy.messages.responses.coordinator.DiscoveredDevices import DiscoveredDevicesResponse
 
 data_ok: dict = {
     'msgid': 'discoveredDevicesTest',
     'nadr': 0,
     'hwpid': 0,
```

### Comparing `iqrfpy-0.1.5/tests/messages/responses/coordinator/DiscoveryResponse_test.py` & `iqrfpy-0.1.6/tests/messages/responses/coordinator/DiscoveryResponse_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import unittest
 from parameterized import parameterized
-from iqrfpy.enums.Commands import CoordinatorResponseCommands
-from iqrfpy.enums.MessageTypes import CoordinatorMessages
+from iqrfpy.enums.commands import CoordinatorResponseCommands
+from iqrfpy.enums.message_types import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
 from iqrfpy.messages.responses.coordinator.Discovery import DiscoveryResponse
 
 data_ok: dict = {
     'msgid': 'discoveryTest',
     'nadr': 0,
     'hwpid': 0,
```

### Comparing `iqrfpy-0.1.5/tests/messages/responses/coordinator/RemoveNodeResponse_test.py` & `iqrfpy-0.1.6/tests/messages/responses/coordinator/RemoveNodeResponse_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import unittest
 from parameterized import parameterized
-from iqrfpy.enums.Commands import CoordinatorResponseCommands
-from iqrfpy.enums.MessageTypes import CoordinatorMessages
+from iqrfpy.enums.commands import CoordinatorResponseCommands
+from iqrfpy.enums.message_types import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
 from iqrfpy.messages.responses.coordinator.RemoveBond import RemoveBondResponse
 
 data_ok: dict = {
     'msgid': 'removeBondTest',
     'nadr': 0,
     'hwpid': 0,
```

### Comparing `iqrfpy-0.1.5/tests/messages/responses/coordinator/RestoreResponse_test.py` & `iqrfpy-0.1.6/tests/messages/responses/coordinator/RestoreResponse_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import unittest
 from parameterized import parameterized
-from iqrfpy.enums.Commands import CoordinatorResponseCommands
-from iqrfpy.enums.MessageTypes import CoordinatorMessages
+from iqrfpy.enums.commands import CoordinatorResponseCommands
+from iqrfpy.enums.message_types import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
 from iqrfpy.messages.responses.coordinator.Restore import RestoreResponse
 
 data_ok: dict = {
     'msgid': 'restoreTest',
     'nadr': 0,
     'hwpid': 0,
```

### Comparing `iqrfpy-0.1.5/tests/messages/responses/coordinator/SetDpaParamsResponse_test.py` & `iqrfpy-0.1.6/tests/messages/responses/coordinator/SetDpaParamsResponse_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import unittest
 from parameterized import parameterized
-from iqrfpy.enums.Commands import CoordinatorResponseCommands
-from iqrfpy.enums.MessageTypes import CoordinatorMessages
+from iqrfpy.enums.commands import CoordinatorResponseCommands
+from iqrfpy.enums.message_types import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
 from iqrfpy.messages.responses.coordinator.SetDpaParams import SetDpaParamsResponse, DpaParam
 
 data_ok: dict = {
     'msgid': 'setDpaParamsTest',
     'nadr': 0,
     'hwpid': 0,
```

### Comparing `iqrfpy-0.1.5/tests/messages/responses/coordinator/SetHopsResponse_test.py` & `iqrfpy-0.1.6/tests/messages/responses/coordinator/SetHopsResponse_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import unittest
 from parameterized import parameterized
-from iqrfpy.enums.Commands import CoordinatorResponseCommands
-from iqrfpy.enums.MessageTypes import CoordinatorMessages
+from iqrfpy.enums.commands import CoordinatorResponseCommands
+from iqrfpy.enums.message_types import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
 from iqrfpy.messages.responses.coordinator.SetHops import SetHopsResponse
 
 data_ok: dict = {
     'msgid': 'setHopsTest',
     'nadr': 0,
     'hwpid': 0,
```

### Comparing `iqrfpy-0.1.5/tests/messages/responses/coordinator/SetMIDResponse_test.py` & `iqrfpy-0.1.6/tests/messages/responses/coordinator/SetMIDResponse_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import unittest
 from parameterized import parameterized
-from iqrfpy.enums.Commands import CoordinatorResponseCommands
-from iqrfpy.enums.MessageTypes import CoordinatorMessages
+from iqrfpy.enums.commands import CoordinatorResponseCommands
+from iqrfpy.enums.message_types import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
 from iqrfpy.messages.responses.coordinator.SetMID import SetMIDResponse
 
 data_ok: dict = {
     'msgid': 'setMidResponse',
     'nadr': 0,
     'hwpid': 0,
```

### Comparing `iqrfpy-0.1.5/tests/messages/responses/coordinator/SmartConnectResponse_test.py` & `iqrfpy-0.1.6/tests/messages/responses/coordinator/SmartConnectResponse_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import unittest
 from parameterized import parameterized
-from iqrfpy.enums.Commands import CoordinatorResponseCommands
-from iqrfpy.enums.MessageTypes import CoordinatorMessages
+from iqrfpy.enums.commands import CoordinatorResponseCommands
+from iqrfpy.enums.message_types import CoordinatorMessages
 from iqrfpy.enums.peripherals import EmbedPeripherals
 from iqrfpy.messages.responses.coordinator.SmartConnect import SmartConnectResponse
 
 data_ok: dict = {
     'msgid': 'smartConnectTest',
     'nadr': 0,
     'hwpid': 0,
```

### Comparing `iqrfpy-0.1.5/tests/utils/Common_test.py` & `iqrfpy-0.1.6/tests/utils/Common_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from parameterized import parameterized
 import unittest
 from iqrfpy.utils.common import *
-from iqrfpy.enums.Commands import *
-from iqrfpy.enums.MessageTypes import *
+from iqrfpy.enums.commands import *
+from iqrfpy.enums.message_types import *
 from iqrfpy.enums.peripherals import *
 from iqrfpy.exceptions import JsonMsgidMissingError, JsonDpaValueMissingError, JsonHwpidMissingError, \
     JsonMTypeMissingError, JsonNadrMissingError, JsonRCodeMissingError, JsonResultMissingError, \
     JsonStatusMissingError, UnsupportedMessageTypeError
 
 
 class CommonTestCase(unittest.TestCase):
```

