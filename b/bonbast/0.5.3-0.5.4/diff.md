# Comparing `tmp/bonbast-0.5.3.tar.gz` & `tmp/bonbast-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bonbast-0.5.3.tar", last modified: Sat Jan 28 08:58:37 2023, max compression
+gzip compressed data, was "bonbast-0.5.4.tar", last modified: Sat Apr 15 17:25:37 2023, max compression
```

## Comparing `bonbast-0.5.3.tar` & `bonbast-0.5.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-28 08:58:37.511776 bonbast-0.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-01-28 08:58:18.000000 bonbast-0.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7907 2023-01-28 08:58:37.511776 bonbast-0.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6009 2023-01-28 08:58:18.000000 bonbast-0.5.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-01-28 08:58:18.000000 bonbast-0.5.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-28 08:58:37.511776 bonbast-0.5.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)       38 2023-01-28 08:58:18.000000 bonbast-0.5.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-28 08:58:37.507776 bonbast-0.5.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-28 08:58:37.511776 bonbast-0.5.3/src/bonbast/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-01-28 08:58:18.000000 bonbast-0.5.3/src/bonbast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-01-28 08:58:18.000000 bonbast-0.5.3/src/bonbast/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-28 08:58:37.511776 bonbast-0.5.3/src/bonbast/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-28 08:58:18.000000 bonbast-0.5.3/src/bonbast/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-01-28 08:58:18.000000 bonbast-0.5.3/src/bonbast/helpers/click_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-01-28 08:58:18.000000 bonbast-0.5.3/src/bonbast/helpers/currency_flags.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-01-28 08:58:18.000000 bonbast-0.5.3/src/bonbast/helpers/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9893 2023-01-28 08:58:18.000000 bonbast-0.5.3/src/bonbast/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-28 08:58:37.511776 bonbast-0.5.3/src/bonbast/managers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-28 08:58:18.000000 bonbast-0.5.3/src/bonbast/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-01-28 08:58:18.000000 bonbast-0.5.3/src/bonbast/managers/storage_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-01-28 08:58:18.000000 bonbast-0.5.3/src/bonbast/managers/token_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-28 08:58:37.511776 bonbast-0.5.3/src/bonbast/models/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-01-28 08:58:18.000000 bonbast-0.5.3/src/bonbast/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-01-28 08:58:18.000000 bonbast-0.5.3/src/bonbast/models/coin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-01-28 08:58:18.000000 bonbast-0.5.3/src/bonbast/models/currency.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-01-28 08:58:18.000000 bonbast-0.5.3/src/bonbast/models/gold.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-01-28 08:58:18.000000 bonbast-0.5.3/src/bonbast/models/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-01-28 08:58:18.000000 bonbast-0.5.3/src/bonbast/models/token.py
--rw-r--r--   0 runner    (1001) docker     (123)     9064 2023-01-28 08:58:18.000000 bonbast-0.5.3/src/bonbast/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-01-28 08:58:18.000000 bonbast-0.5.3/src/bonbast/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-28 08:58:37.511776 bonbast-0.5.3/src/bonbast.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7907 2023-01-28 08:58:37.000000 bonbast-0.5.3/src/bonbast.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-01-28 08:58:37.000000 bonbast-0.5.3/src/bonbast.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-28 08:58:37.000000 bonbast-0.5.3/src/bonbast.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-01-28 08:58:37.000000 bonbast-0.5.3/src/bonbast.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-01-28 08:58:37.000000 bonbast-0.5.3/src/bonbast.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-01-28 08:58:37.000000 bonbast-0.5.3/src/bonbast.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:25:37.498376 bonbast-0.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-15 17:25:16.000000 bonbast-0.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10454 2023-04-15 17:25:37.498376 bonbast-0.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-04-15 17:25:16.000000 bonbast-0.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-15 17:25:16.000000 bonbast-0.5.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 17:25:37.498376 bonbast-0.5.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)       38 2023-04-15 17:25:16.000000 bonbast-0.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:25:37.494376 bonbast-0.5.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:25:37.494376 bonbast-0.5.4/src/bonbast/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-15 17:25:16.000000 bonbast-0.5.4/src/bonbast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-15 17:25:16.000000 bonbast-0.5.4/src/bonbast/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:25:37.498376 bonbast-0.5.4/src/bonbast/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 17:25:16.000000 bonbast-0.5.4/src/bonbast/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-15 17:25:16.000000 bonbast-0.5.4/src/bonbast/helpers/click_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-15 17:25:16.000000 bonbast-0.5.4/src/bonbast/helpers/currency_flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-04-15 17:25:16.000000 bonbast-0.5.4/src/bonbast/helpers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9902 2023-04-15 17:25:16.000000 bonbast-0.5.4/src/bonbast/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:25:37.498376 bonbast-0.5.4/src/bonbast/managers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 17:25:16.000000 bonbast-0.5.4/src/bonbast/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-04-15 17:25:16.000000 bonbast-0.5.4/src/bonbast/managers/storage_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-04-15 17:25:16.000000 bonbast-0.5.4/src/bonbast/managers/token_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:25:37.498376 bonbast-0.5.4/src/bonbast/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-15 17:25:16.000000 bonbast-0.5.4/src/bonbast/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-15 17:25:16.000000 bonbast-0.5.4/src/bonbast/models/coin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-04-15 17:25:16.000000 bonbast-0.5.4/src/bonbast/models/currency.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-04-15 17:25:16.000000 bonbast-0.5.4/src/bonbast/models/gold.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-15 17:25:16.000000 bonbast-0.5.4/src/bonbast/models/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-15 17:25:16.000000 bonbast-0.5.4/src/bonbast/models/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9298 2023-04-15 17:25:16.000000 bonbast-0.5.4/src/bonbast/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-04-15 17:25:16.000000 bonbast-0.5.4/src/bonbast/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:25:37.498376 bonbast-0.5.4/src/bonbast.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10454 2023-04-15 17:25:37.000000 bonbast-0.5.4/src/bonbast.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-15 17:25:37.000000 bonbast-0.5.4/src/bonbast.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 17:25:37.000000 bonbast-0.5.4/src/bonbast.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-15 17:25:37.000000 bonbast-0.5.4/src/bonbast.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-15 17:25:37.000000 bonbast-0.5.4/src/bonbast.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-15 17:25:37.000000 bonbast-0.5.4/src/bonbast.egg-info/top_level.txt
```

### Comparing `bonbast-0.5.3/LICENSE` & `bonbast-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bonbast-0.5.3/PKG-INFO` & `bonbast-0.5.4/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bonbast
-Version: 0.5.3
+Version: 0.5.4
 Summary: Get currencies exchange rates for IRR from Bonbast.com
 Author-email: Amir Hossein SamadiPour <samadipoor2@gmail.com>, Alireza Azadi <alireza_azadi@hotmail.com>, Iliya Aghamajidi <dozheiny@gmail.com>, Parsa Shahmaleki <parsampsh@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Amir Hossein SamadiPour
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -38,16 +38,53 @@
 
 [bonbast.com](https://bonbast.com) offers accurate and reliable gold prices and IRR exchange rates for businesses.
 Bonbast is the most accurate and reputable foreign exchange trading data collector of the Iranian market.
 
 I don't alter any of the data in this tool; it all comes from bonbast. The sole purpose of this tool is to offer a
 different method of obtaining bonbast prices.
 
+## Contents
+1. [Installation](#installation)
+   * [Brew](#brew)
+   * [Python](#python)
+   * [Raycast](#setup-for-raycast)
+2. [Usage](#usage)
+   1. [Command Line](#command-line)
+      * [Main mode](#main-mode)
+      * [Live](#live)
+      * [Simple](#simple)
+      * [Currency](#currency)
+      * [History](#history)
+      * [Convert](#convert)
+      * [Json Output](#json-output)
+      * [Pretty Print Json](#pretty-print-json)
+      * [List of supported currencies](#list-of-supported-currencies)
+   2. [Usage in other programs](#usage-in-other-programs)
+   3. [Mac Shortcuts](#mac-shortcuts)
+   4. [Raycast](#raycast)
+3. [Development](#development)
+
 ## Installation
 
+### Brew
+
+```
+brew install samadipour/bonbast/bonbast
+```
+
+or
+
+```
+brew tap samadipour/bonbast
+brew update
+brew install bonbast
+```
+
+### Python
+
 To install this program, you can to use pip:
 
 ```shell
 $ pip install bonbast
 # Or
 $ python -m pip install bonbast
 ```
@@ -66,80 +103,139 @@
 pip install -U bonbast
 #or
 python -m pip install -U bonbast
 ```
 
 ---
 
-# Usage
+## Usage
 
 I tried my best to display the price data in a variety of ways that would be useful in a variety of circumstances.
 
-## Main mode
+### Command Line
+
+#### Main mode
 
 This will be the default mode if you run the program without any arguments. It will show the current prices for gold,
 coins, and the IRR exchange rate in separate tables.
 
 ![bonbast](https://user-images.githubusercontent.com/24422125/194708514-e7b76a69-0671-4a6c-a025-51f29558f087.png)
 
-## Live
+#### Live
 
 In live mode, the program tries to update the prices in a specified interval. This is useful if you want to keep an eye
 on the prices.
 
 The website updates the prices every 30 seconds and the default value is 30 seconds as well. You can change this value
 by using the `-i` or `--interval` argument.
 
-### Simple
+```shell
+$ bonbast -i 60
+# Or
+$ python -m bonbast -i 60
+```
+
+#### Simple
 
 In this mode, the program will show the prices as text in the terminal.
 
+```shell
+$ bonbast live simple --show-only usd,eur,gbp,cad -i 300
+# Or
+$ python -m bonbast live simple --show-only usd,eur,gbp,cad -i 300
+```
+
 ![bonbast_live_simple](https://user-images.githubusercontent.com/24422125/194708537-09f98a47-a6b2-4489-a106-9bf22db6d527.png)
 
-### Currency
+#### Currency
 
 In this mode, the program will show the prices in a table. It can only show one currency at a time.
 
+```shell
+$ bonbast live currency --show-only usd,eur,gbp,cad -i 300
+# Or
+$ python -m bonbast live currency --show-only usd,eur,gbp,cad -i 300
+```
+
 ![bonbast_live_currency](https://user-images.githubusercontent.com/24422125/194708542-241d2e11-35ec-4868-91ec-30ff7ca5e6e0.png)
 
-## History
+#### History
 
 This is useful if you want to see the prices for a specific date. You can use the `-d` or `--date` argument to specify
 the date. The date must be in the format `YYYY-MM-DD` or `YYYY/MM/DD`. Also, the date needs to be Gregorian.
 
 The date is valid from 2012-10-09 to one day before the current date.
 
+```shell
+$ bonbast history --date 2020/10/10
+# Or
+$ python -m bonbast history --date 2020/10/10
+```
+
 ![bonbast_history](https://user-images.githubusercontent.com/24422125/194708555-fb5ada09-8e74-497d-8b61-74f27dea9220.png)
 
-## Convert
+#### Convert
 
 This is useful if you want to convert a value from one currency to Rial or from Rial to another currency.
+If you want to convert from a currency to Rial, you need to use `-s` or `--source` argument to specify the currency you
+want to convert from.
+
+```shell
+$ bonbast convert -s EUR 12.5
+# Or
+$ python -m bonbast convert -s EUR 12.5
+```
 
 If you want to convert from Rial to another currency, you need to use the `-d` or `--destination` argument to specify
 the currency you want to convert to.
 
-If you want to convert from a currency to Rial, you need to use `-s` or `--source` argument to specify the currency you
-want to convert from.
+```shell
+$ bonbast convert -d USD 1837850
+# Or
+$ python -m bonbast convert -d USD 1837850
+```
+
+You can also use `--only-buy` or `--only-sell` to specify which price you want to use.
+
+```shell
+$ bonbast convert -d USD 1837850 --only-buy
+$ bonbast convert -d USD 1837850 --only-sell
+# Or
+$ python -m bonbast convert -d USD 1837850 --only-buy
+$ python -m bonbast convert -d USD 1837850 --only-sell
+```
 
 ![bonbast_convert](https://user-images.githubusercontent.com/24422125/194708562-38f9f08c-9bc7-41d0-9889-04f38007b7f3.png)
 
-## Json Output
+#### Json Output
 
 It can be useful if you want to use the result of the program in another program. You can also pipe the output in
 terminal to another program like `JQ`.
 
+```shell
+$ bonbast export
+# Or
+$ python -m bonbast export
+```
+
 ![bonbast_export](https://user-images.githubusercontent.com/24422125/194708575-58fc19a5-9aa9-4e6d-b020-a40835d9d55d.png)
 
-### Pretty Print Json
+#### Pretty Print Json
 
 There is also a way to pretty print the json output. You can use the `--pretty` argument to do that. It helps to see the
 output in a more readable way.
+
+```shell
+$ bonbast export --pretty
+# Or
+$ python -m bonbast export --pretty
+```
 ![bonbast_export_pretty](https://user-images.githubusercontent.com/24422125/194708592-471a189b-e3f4-4a29-b36c-ad536d93822e.png)
 
-## List of supported currencies
+#### List of supported currencies
 
 | Flag | Currency          | Code |
 |:----:|-------------------|:----:|
 | 🇺🇸 | US Dollar         | USD  |
 | 🇪🇺 | Euro              | EUR  |
 | 🇬🇧 | British Pound     | GBP  |
 | 🇨🇭 | Swiss Franc       | CHF  |
@@ -166,51 +262,71 @@
 | 🇮🇶 | 100 Iraqi Dinar   | IQD  |
 | 🇧🇭 | Bahraini Dinar    | BHD  |
 | 🇴🇲 | Omani Rial        | OMR  |
 | 🇶🇦 | Qatari Rial       | QAR  |
 
 ---
 
-# Usage in other programs
+### Usage in other programs
 
 There are few ways to use the program in other programs. The best way is to use the json output.
 
-## Mac Shortcuts
+### Mac Shortcuts
 
 You can use the json output or the convert function to create a shortcut in Mac. You can use the shortcut to show the
 currency price as a notification.
 
-## [Raycast](https://www.raycast.com/)
+### [Raycast](https://www.raycast.com/)
 
 Raycast is a tool for searching your Mac, launching applications, and controlling your computer, and it is far superior
 to Spotlight. You can use the json output to create a script command in Raycast. In this way, you can easily access the
 prices in Raycast.
 
 I included an example script command in the `raycast` folder. You can use it to create your own script.
 
 ![bonbast_raycast](https://user-images.githubusercontent.com/24422125/194708612-a5f5557c-aab3-4ded-b500-9e08b594949c.png)
 
+#### Setup for Raycast
+
+You can use this [setup-raycast.sh](./raycast_script/setup-raycast.sh) script to setup the script command in Raycast. Then Follow the instructions in below image or read Raycast docs.
+
+```shell
+$ chmod +x setup-raycast.sh
+
+$ ./setup-raycast.sh standalone
+or
+$ ./setup-raycast.sh python
+```
+
+or manually:
+
+1. Enable the script command in Raycast.
+2. Copy [bonbast.sh](./raycast_script/bonbast.sh) file to the Raycast `script-commands` folder.
+3. Follow the instructions below or read Raycast docs.
+
+![raycast-setup](https://github.com/SamadiPour/bonbast/blob/master/.github/setup-raycast.png?raw=true)
+
 ---
 
-# Development
+## Development
 
-## Setup
+### Setup
 
 1. Clone the repo
 2. Install the dependencies
 3. Run it with python
 
 ```shell
 git clone https://github.com/SamadiPour/bonbast.git
 cd bonbast
 pip install .
 python -m src.bonbast.main
 ```
 
-## Building the package
+### Building the package
 
 1. Install build dependencies
 2. Build the package
 3. install it locally if you want (or you can use `local_install` script)
 
 ```shell
 python -m pip install ".[build]"
```

### Comparing `bonbast-0.5.3/pyproject.toml` & `bonbast-0.5.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bonbast"
-version = "0.5.3"
+version = "0.5.4"
 description = "Get currencies exchange rates for IRR from Bonbast.com"
 readme = "README.md"
 authors = [
     { name = "Amir Hossein SamadiPour", email = "samadipoor2@gmail.com" },
     { name = "Alireza Azadi", email = "alireza_azadi@hotmail.com" },
     { name = "Iliya Aghamajidi", email = "dozheiny@gmail.com" },
     { name = "Parsa Shahmaleki", email = "parsampsh@gmail.com" },
@@ -37,15 +37,15 @@
 
 [project.urls]
 repository = "https://github.com/SamadiPour/bonbast"
 #documentation = ""
 
 
 [tool.bumpver]
-current_version = "0.5.3"
+current_version = "0.5.4"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `bonbast-0.5.3/src/bonbast/helpers/click_callbacks.py` & `bonbast-0.5.4/src/bonbast/helpers/click_callbacks.py`

 * *Files identical despite different names*

### Comparing `bonbast-0.5.3/src/bonbast/helpers/currency_flags.py` & `bonbast-0.5.4/src/bonbast/helpers/currency_flags.py`

 * *Files identical despite different names*

### Comparing `bonbast-0.5.3/src/bonbast/helpers/utils.py` & `bonbast-0.5.4/src/bonbast/helpers/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,22 +20,31 @@
     return TOMAN_FORMATTER.format(price)
 
 
 def format_price(price: float) -> str:
     return PRICE_FORMATTER.format(price)
 
 
+class RetryError(Exception):
+    def __init__(self, message):
+        self.message = message
+        super().__init__(message)
+
+
 def retry(retry_count=3, retry_delay=None, message=''):
     def decorator_retry(func):
         @functools.wraps(func)
         def wrapper_retry(*args, **kwargs):
-            for _ in range(retry_count):
+            for i in range(retry_count):
                 try:
                     return func(*args, **kwargs)
-                except:  # noqa
+                except RetryError as e:
+                    if i == retry_count - 1:
+                        raise SystemExit(e.message)
+                except Exception as e:  # noqa
                     if retry_delay is not None:
                         time.sleep(retry_delay)
 
             raise SystemExit(message)
 
         return wrapper_retry
```

### Comparing `bonbast-0.5.3/src/bonbast/main.py` & `bonbast-0.5.4/src/bonbast/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     from tables import *
     from managers.token_manager import *
     from managers.storage_manager import *
     from helpers.click_callbacks import *
     from helpers.utils import *
 
 
-@retry(message='Error: token is expired. Try again later.')
+@retry(message='Error: The operation failed for an unknown reason.')
 def get_prices(show_only: List[str] = None):
     token = token_manager.generate()
     try:
         response = get_prices_from_api(token.value)
         if show_only is not None and len(show_only) > 0:
             response = list(response)
             for index, item in enumerate(response):
```

### Comparing `bonbast-0.5.3/src/bonbast/managers/storage_manager.py` & `bonbast-0.5.4/src/bonbast/managers/storage_manager.py`

 * *Files identical despite different names*

### Comparing `bonbast-0.5.3/src/bonbast/managers/token_manager.py` & `bonbast-0.5.4/src/bonbast/managers/token_manager.py`

 * *Files identical despite different names*

### Comparing `bonbast-0.5.3/src/bonbast/models/coin.py` & `bonbast-0.5.4/src/bonbast/models/coin.py`

 * *Files identical despite different names*

### Comparing `bonbast-0.5.3/src/bonbast/models/currency.py` & `bonbast-0.5.4/src/bonbast/models/currency.py`

 * *Files identical despite different names*

### Comparing `bonbast-0.5.3/src/bonbast/models/gold.py` & `bonbast-0.5.4/src/bonbast/models/gold.py`

 * *Files identical despite different names*

### Comparing `bonbast-0.5.3/src/bonbast/models/token.py` & `bonbast-0.5.4/src/bonbast/models/token.py`

 * *Files identical despite different names*

### Comparing `bonbast-0.5.3/src/bonbast/server.py` & `bonbast-0.5.4/src/bonbast/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,16 @@
     }
 
     try:
         r = requests.get(BASE_URL, headers=headers)
         r.raise_for_status()
     except requests.exceptions.HTTPError as err:
         raise SystemExit(err)
+    except requests.exceptions.ConnectionError as _:
+        raise SystemExit('Error: Failed to connect to bonbast')
 
     search = re.search(r"param\s*=\s*\"(.+)\"", r.text, re.MULTILINE)
     if search is None or search.group(1) is None:
         raise SystemExit('Error: token not found in the main page')
 
     return search.group(1)
 
@@ -95,14 +97,16 @@
 
     try:
         r = requests.post(f'{BASE_URL}/json', headers=headers, data=data)
         r.raise_for_status()
         r = r.json()
     except requests.exceptions.HTTPError as err:
         raise SystemExit(err)
+    except requests.exceptions.ConnectionError as _:
+        raise SystemExit('Error: Failed to connect to bonbast')
 
     if 'reset' in r:
         raise ResetAPIError('Error: token is expired')
 
     currencies: List[Currency] = []
     coins: List[Coin] = []
     golds: List[Gold] = []
```

### Comparing `bonbast-0.5.3/src/bonbast/tables.py` & `bonbast-0.5.4/src/bonbast/tables.py`

 * *Files identical despite different names*

### Comparing `bonbast-0.5.3/src/bonbast.egg-info/PKG-INFO` & `bonbast-0.5.4/src/bonbast.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bonbast
-Version: 0.5.3
+Version: 0.5.4
 Summary: Get currencies exchange rates for IRR from Bonbast.com
 Author-email: Amir Hossein SamadiPour <samadipoor2@gmail.com>, Alireza Azadi <alireza_azadi@hotmail.com>, Iliya Aghamajidi <dozheiny@gmail.com>, Parsa Shahmaleki <parsampsh@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Amir Hossein SamadiPour
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -38,16 +38,53 @@
 
 [bonbast.com](https://bonbast.com) offers accurate and reliable gold prices and IRR exchange rates for businesses.
 Bonbast is the most accurate and reputable foreign exchange trading data collector of the Iranian market.
 
 I don't alter any of the data in this tool; it all comes from bonbast. The sole purpose of this tool is to offer a
 different method of obtaining bonbast prices.
 
+## Contents
+1. [Installation](#installation)
+   * [Brew](#brew)
+   * [Python](#python)
+   * [Raycast](#setup-for-raycast)
+2. [Usage](#usage)
+   1. [Command Line](#command-line)
+      * [Main mode](#main-mode)
+      * [Live](#live)
+      * [Simple](#simple)
+      * [Currency](#currency)
+      * [History](#history)
+      * [Convert](#convert)
+      * [Json Output](#json-output)
+      * [Pretty Print Json](#pretty-print-json)
+      * [List of supported currencies](#list-of-supported-currencies)
+   2. [Usage in other programs](#usage-in-other-programs)
+   3. [Mac Shortcuts](#mac-shortcuts)
+   4. [Raycast](#raycast)
+3. [Development](#development)
+
 ## Installation
 
+### Brew
+
+```
+brew install samadipour/bonbast/bonbast
+```
+
+or
+
+```
+brew tap samadipour/bonbast
+brew update
+brew install bonbast
+```
+
+### Python
+
 To install this program, you can to use pip:
 
 ```shell
 $ pip install bonbast
 # Or
 $ python -m pip install bonbast
 ```
@@ -66,80 +103,139 @@
 pip install -U bonbast
 #or
 python -m pip install -U bonbast
 ```
 
 ---
 
-# Usage
+## Usage
 
 I tried my best to display the price data in a variety of ways that would be useful in a variety of circumstances.
 
-## Main mode
+### Command Line
+
+#### Main mode
 
 This will be the default mode if you run the program without any arguments. It will show the current prices for gold,
 coins, and the IRR exchange rate in separate tables.
 
 ![bonbast](https://user-images.githubusercontent.com/24422125/194708514-e7b76a69-0671-4a6c-a025-51f29558f087.png)
 
-## Live
+#### Live
 
 In live mode, the program tries to update the prices in a specified interval. This is useful if you want to keep an eye
 on the prices.
 
 The website updates the prices every 30 seconds and the default value is 30 seconds as well. You can change this value
 by using the `-i` or `--interval` argument.
 
-### Simple
+```shell
+$ bonbast -i 60
+# Or
+$ python -m bonbast -i 60
+```
+
+#### Simple
 
 In this mode, the program will show the prices as text in the terminal.
 
+```shell
+$ bonbast live simple --show-only usd,eur,gbp,cad -i 300
+# Or
+$ python -m bonbast live simple --show-only usd,eur,gbp,cad -i 300
+```
+
 ![bonbast_live_simple](https://user-images.githubusercontent.com/24422125/194708537-09f98a47-a6b2-4489-a106-9bf22db6d527.png)
 
-### Currency
+#### Currency
 
 In this mode, the program will show the prices in a table. It can only show one currency at a time.
 
+```shell
+$ bonbast live currency --show-only usd,eur,gbp,cad -i 300
+# Or
+$ python -m bonbast live currency --show-only usd,eur,gbp,cad -i 300
+```
+
 ![bonbast_live_currency](https://user-images.githubusercontent.com/24422125/194708542-241d2e11-35ec-4868-91ec-30ff7ca5e6e0.png)
 
-## History
+#### History
 
 This is useful if you want to see the prices for a specific date. You can use the `-d` or `--date` argument to specify
 the date. The date must be in the format `YYYY-MM-DD` or `YYYY/MM/DD`. Also, the date needs to be Gregorian.
 
 The date is valid from 2012-10-09 to one day before the current date.
 
+```shell
+$ bonbast history --date 2020/10/10
+# Or
+$ python -m bonbast history --date 2020/10/10
+```
+
 ![bonbast_history](https://user-images.githubusercontent.com/24422125/194708555-fb5ada09-8e74-497d-8b61-74f27dea9220.png)
 
-## Convert
+#### Convert
 
 This is useful if you want to convert a value from one currency to Rial or from Rial to another currency.
+If you want to convert from a currency to Rial, you need to use `-s` or `--source` argument to specify the currency you
+want to convert from.
+
+```shell
+$ bonbast convert -s EUR 12.5
+# Or
+$ python -m bonbast convert -s EUR 12.5
+```
 
 If you want to convert from Rial to another currency, you need to use the `-d` or `--destination` argument to specify
 the currency you want to convert to.
 
-If you want to convert from a currency to Rial, you need to use `-s` or `--source` argument to specify the currency you
-want to convert from.
+```shell
+$ bonbast convert -d USD 1837850
+# Or
+$ python -m bonbast convert -d USD 1837850
+```
+
+You can also use `--only-buy` or `--only-sell` to specify which price you want to use.
+
+```shell
+$ bonbast convert -d USD 1837850 --only-buy
+$ bonbast convert -d USD 1837850 --only-sell
+# Or
+$ python -m bonbast convert -d USD 1837850 --only-buy
+$ python -m bonbast convert -d USD 1837850 --only-sell
+```
 
 ![bonbast_convert](https://user-images.githubusercontent.com/24422125/194708562-38f9f08c-9bc7-41d0-9889-04f38007b7f3.png)
 
-## Json Output
+#### Json Output
 
 It can be useful if you want to use the result of the program in another program. You can also pipe the output in
 terminal to another program like `JQ`.
 
+```shell
+$ bonbast export
+# Or
+$ python -m bonbast export
+```
+
 ![bonbast_export](https://user-images.githubusercontent.com/24422125/194708575-58fc19a5-9aa9-4e6d-b020-a40835d9d55d.png)
 
-### Pretty Print Json
+#### Pretty Print Json
 
 There is also a way to pretty print the json output. You can use the `--pretty` argument to do that. It helps to see the
 output in a more readable way.
+
+```shell
+$ bonbast export --pretty
+# Or
+$ python -m bonbast export --pretty
+```
 ![bonbast_export_pretty](https://user-images.githubusercontent.com/24422125/194708592-471a189b-e3f4-4a29-b36c-ad536d93822e.png)
 
-## List of supported currencies
+#### List of supported currencies
 
 | Flag | Currency          | Code |
 |:----:|-------------------|:----:|
 | 🇺🇸 | US Dollar         | USD  |
 | 🇪🇺 | Euro              | EUR  |
 | 🇬🇧 | British Pound     | GBP  |
 | 🇨🇭 | Swiss Franc       | CHF  |
@@ -166,51 +262,71 @@
 | 🇮🇶 | 100 Iraqi Dinar   | IQD  |
 | 🇧🇭 | Bahraini Dinar    | BHD  |
 | 🇴🇲 | Omani Rial        | OMR  |
 | 🇶🇦 | Qatari Rial       | QAR  |
 
 ---
 
-# Usage in other programs
+### Usage in other programs
 
 There are few ways to use the program in other programs. The best way is to use the json output.
 
-## Mac Shortcuts
+### Mac Shortcuts
 
 You can use the json output or the convert function to create a shortcut in Mac. You can use the shortcut to show the
 currency price as a notification.
 
-## [Raycast](https://www.raycast.com/)
+### [Raycast](https://www.raycast.com/)
 
 Raycast is a tool for searching your Mac, launching applications, and controlling your computer, and it is far superior
 to Spotlight. You can use the json output to create a script command in Raycast. In this way, you can easily access the
 prices in Raycast.
 
 I included an example script command in the `raycast` folder. You can use it to create your own script.
 
 ![bonbast_raycast](https://user-images.githubusercontent.com/24422125/194708612-a5f5557c-aab3-4ded-b500-9e08b594949c.png)
 
+#### Setup for Raycast
+
+You can use this [setup-raycast.sh](./raycast_script/setup-raycast.sh) script to setup the script command in Raycast. Then Follow the instructions in below image or read Raycast docs.
+
+```shell
+$ chmod +x setup-raycast.sh
+
+$ ./setup-raycast.sh standalone
+or
+$ ./setup-raycast.sh python
+```
+
+or manually:
+
+1. Enable the script command in Raycast.
+2. Copy [bonbast.sh](./raycast_script/bonbast.sh) file to the Raycast `script-commands` folder.
+3. Follow the instructions below or read Raycast docs.
+
+![raycast-setup](https://github.com/SamadiPour/bonbast/blob/master/.github/setup-raycast.png?raw=true)
+
 ---
 
-# Development
+## Development
 
-## Setup
+### Setup
 
 1. Clone the repo
 2. Install the dependencies
 3. Run it with python
 
 ```shell
 git clone https://github.com/SamadiPour/bonbast.git
 cd bonbast
 pip install .
 python -m src.bonbast.main
 ```
 
-## Building the package
+### Building the package
 
 1. Install build dependencies
 2. Build the package
 3. install it locally if you want (or you can use `local_install` script)
 
 ```shell
 python -m pip install ".[build]"
```

### Comparing `bonbast-0.5.3/src/bonbast.egg-info/SOURCES.txt` & `bonbast-0.5.4/src/bonbast.egg-info/SOURCES.txt`

 * *Files identical despite different names*

