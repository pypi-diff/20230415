# Comparing `tmp/weather_command-5.2.2.tar.gz` & `tmp/weather_command-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weather_command-5.2.2.tar", max compression
+gzip compressed data, was "weather_command-6.0.0.tar", max compression
```

## Comparing `weather_command-5.2.2.tar` & `weather_command-6.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1069 2023-04-13 23:35:31.339075 weather_command-5.2.2/LICENSE
--rw-r--r--   0        0        0     2881 2023-04-13 23:35:31.339075 weather_command-5.2.2/README.md
--rw-r--r--   0        0        0     1849 2023-04-13 23:35:31.339075 weather_command-5.2.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-13 23:35:31.343075 weather_command-5.2.2/weather_command/__init__.py
--rw-r--r--   0        0        0       95 2023-04-13 23:35:31.343075 weather_command-5.2.2/weather_command/__main__.py
--rw-r--r--   0        0        0    18640 2023-04-13 23:35:31.343075 weather_command-5.2.2/weather_command/_builder.py
--rw-r--r--   0        0        0     5260 2023-04-13 23:35:31.343075 weather_command-5.2.2/weather_command/_cache.py
--rw-r--r--   0        0        0     5262 2023-04-13 23:35:31.343075 weather_command-5.2.2/weather_command/_config.py
--rw-r--r--   0        0        0     2546 2023-04-13 23:35:31.343075 weather_command-5.2.2/weather_command/_location.py
--rw-r--r--   0        0        0      473 2023-04-13 23:35:31.343075 weather_command-5.2.2/weather_command/_utils.py
--rw-r--r--   0        0        0     2921 2023-04-13 23:35:31.343075 weather_command-5.2.2/weather_command/_weather.py
--rw-r--r--   0        0        0      459 2023-04-13 23:35:31.343075 weather_command-5.2.2/weather_command/errors.py
--rw-r--r--   0        0        0     9000 2023-04-13 23:35:31.343075 weather_command-5.2.2/weather_command/main.py
--rw-r--r--   0        0        0        0 2023-04-13 23:35:31.343075 weather_command-5.2.2/weather_command/models/__init__.py
--rw-r--r--   0        0        0      133 2023-04-13 23:35:31.343075 weather_command-5.2.2/weather_command/models/location.py
--rw-r--r--   0        0        0     3053 2023-04-13 23:35:31.343075 weather_command-5.2.2/weather_command/models/weather.py
--rw-r--r--   0        0        0        0 2023-04-13 23:35:31.343075 weather_command-5.2.2/weather_command/py.typed
--rw-r--r--   0        0        0     2816 2023-04-13 23:35:31.343075 weather_command-5.2.2/weather_command/settings_commands.py
--rw-r--r--   0        0        0     3928 1970-01-01 00:00:00.000000 weather_command-5.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-15 18:13:07.333191 weather_command-6.0.0/LICENSE
+-rw-r--r--   0        0        0     2849 2023-04-15 18:13:07.333191 weather_command-6.0.0/README.md
+-rw-r--r--   0        0        0     1841 2023-04-15 18:13:07.333191 weather_command-6.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-15 18:13:07.337191 weather_command-6.0.0/weather_command/__init__.py
+-rw-r--r--   0        0        0       95 2023-04-15 18:13:07.337191 weather_command-6.0.0/weather_command/__main__.py
+-rw-r--r--   0        0        0    18640 2023-04-15 18:13:07.337191 weather_command-6.0.0/weather_command/_builder.py
+-rw-r--r--   0        0        0     5260 2023-04-15 18:13:07.337191 weather_command-6.0.0/weather_command/_cache.py
+-rw-r--r--   0        0        0     5262 2023-04-15 18:13:07.337191 weather_command-6.0.0/weather_command/_config.py
+-rw-r--r--   0        0        0     2546 2023-04-15 18:13:07.337191 weather_command-6.0.0/weather_command/_location.py
+-rw-r--r--   0        0        0      473 2023-04-15 18:13:07.337191 weather_command-6.0.0/weather_command/_utils.py
+-rw-r--r--   0        0        0     2921 2023-04-15 18:13:07.337191 weather_command-6.0.0/weather_command/_weather.py
+-rw-r--r--   0        0        0      459 2023-04-15 18:13:07.337191 weather_command-6.0.0/weather_command/errors.py
+-rw-r--r--   0        0        0     9000 2023-04-15 18:13:07.337191 weather_command-6.0.0/weather_command/main.py
+-rw-r--r--   0        0        0        0 2023-04-15 18:13:07.337191 weather_command-6.0.0/weather_command/models/__init__.py
+-rw-r--r--   0        0        0      133 2023-04-15 18:13:07.337191 weather_command-6.0.0/weather_command/models/location.py
+-rw-r--r--   0        0        0     3053 2023-04-15 18:13:07.337191 weather_command-6.0.0/weather_command/models/weather.py
+-rw-r--r--   0        0        0        0 2023-04-15 18:13:07.337191 weather_command-6.0.0/weather_command/py.typed
+-rw-r--r--   0        0        0     2816 2023-04-15 18:13:07.337191 weather_command-6.0.0/weather_command/settings_commands.py
+-rw-r--r--   0        0        0     3896 1970-01-01 00:00:00.000000 weather_command-6.0.0/PKG-INFO
```

### Comparing `weather_command-5.2.2/LICENSE` & `weather_command-6.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `weather_command-5.2.2/README.md` & `weather_command-6.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -35,24 +35,24 @@
 Each time the shell is restarted this variable will be cleared. To avoid this it can be added to your
 profile. For example if your shell is zsh the API key can be added to the `~/.zshenv` file. Doing this
 will prevent the need to re-add the key each time the shell is started.
 
 To get the weather for a city:
 
 ```sh
-weather-command city seattle
+weather city seattle
 ```
 
 Once installed you can also add aliases to your shell to make it quick to get a forecast. For example
 if your shell is zsh you can add something like the following to your `~/.zshrc` file:
 
 ```sh
-alias we="weather-command zip 98109 -i --am-pm"
-alias wed="weather-command zip 98109 -i --am-pm -f daily"
-alias weh="weather-command zip 98109 -i --am-pm -f hourly"
+alias we="weather zip 98109 -i --am-pm"
+alias wed="weather zip 98109 -i --am-pm -f daily"
+alias weh="weather zip 98109 -i --am-pm -f hourly"
 ```
 
 After adding this to the `~/.zshrc` you will need to restart your terminal. After that typing `we`
 will get the current forecast, `wed` will get the daily forecast and `weh` will get the hourly forecast.
 
 ## Examples
```

### Comparing `weather_command-5.2.2/pyproject.toml` & `weather_command-6.0.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "weather-command"
-version = "5.2.2"
+version = "6.0.0"
 description = "Command line weather app"
 authors = ["Paul Sanders <psanders1@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/sanders41/weather-command"
 homepage = "https://github.com/sanders41/weather-command"
 documentation = "https://github.com/sanders41/weather-command"
@@ -20,28 +20,28 @@
 tenacity = "8.2.2"
 pyyaml = "6.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "23.3.0"
 mypy = "1.2.0"
 pre-commit = "2.21.0"
-pytest = "7.3.0"
+pytest = "7.3.1"
 pytest-cov = "4.0.0"
 tox = "4.4.12"
 ruff = "0.0.261"
 tomli = {version = "2.0.1", python = "<3.11"}
 types-pyyaml = "6.0.12.9"
 pytest-asyncio = "0.21.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
-weather-command = "weather_command.main:app"
+weather = "weather_command.main:app"
 
 [tool.black]
 line-length = 100
 include = '\.pyi?$'
 exclude = '''
 /(
     \.egg
```

### Comparing `weather_command-5.2.2/weather_command/_builder.py` & `weather_command-6.0.0/weather_command/_builder.py`

 * *Files identical despite different names*

### Comparing `weather_command-5.2.2/weather_command/_cache.py` & `weather_command-6.0.0/weather_command/_cache.py`

 * *Files identical despite different names*

### Comparing `weather_command-5.2.2/weather_command/_config.py` & `weather_command-6.0.0/weather_command/_config.py`

 * *Files identical despite different names*

### Comparing `weather_command-5.2.2/weather_command/_location.py` & `weather_command-6.0.0/weather_command/_location.py`

 * *Files identical despite different names*

### Comparing `weather_command-5.2.2/weather_command/_weather.py` & `weather_command-6.0.0/weather_command/_weather.py`

 * *Files identical despite different names*

### Comparing `weather_command-5.2.2/weather_command/main.py` & `weather_command-6.0.0/weather_command/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from weather_command._builder import show_current, show_daily, show_hourly
 from weather_command._cache import Cache
 from weather_command._config import console, load_settings
 from weather_command._location import get_location_details
 from weather_command._utils import build_weather_url
 from weather_command._weather import get_current_weather, get_one_call_weather
 
-__version__ = "5.2.2"
+__version__ = "6.0.0"
 
 app = Typer()
 app.add_typer(settings_commands.app, name="settings", help="Manage saved settings.")
 
 
 class ForecastType(str, Enum):
     CURRENT = "current"
```

### Comparing `weather_command-5.2.2/weather_command/models/weather.py` & `weather_command-6.0.0/weather_command/models/weather.py`

 * *Files identical despite different names*

### Comparing `weather_command-5.2.2/weather_command/settings_commands.py` & `weather_command-6.0.0/weather_command/settings_commands.py`

 * *Files identical despite different names*

### Comparing `weather_command-5.2.2/PKG-INFO` & `weather_command-6.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weather-command
-Version: 5.2.2
+Version: 6.0.0
 Summary: Command line weather app
 Home-page: https://github.com/sanders41/weather-command
 License: MIT
 Keywords: weather,cli
 Author: Paul Sanders
 Author-email: psanders1@gmail.com
 Requires-Python: >=3.7,<4.0
@@ -63,24 +63,24 @@
 Each time the shell is restarted this variable will be cleared. To avoid this it can be added to your
 profile. For example if your shell is zsh the API key can be added to the `~/.zshenv` file. Doing this
 will prevent the need to re-add the key each time the shell is started.
 
 To get the weather for a city:
 
 ```sh
-weather-command city seattle
+weather city seattle
 ```
 
 Once installed you can also add aliases to your shell to make it quick to get a forecast. For example
 if your shell is zsh you can add something like the following to your `~/.zshrc` file:
 
 ```sh
-alias we="weather-command zip 98109 -i --am-pm"
-alias wed="weather-command zip 98109 -i --am-pm -f daily"
-alias weh="weather-command zip 98109 -i --am-pm -f hourly"
+alias we="weather zip 98109 -i --am-pm"
+alias wed="weather zip 98109 -i --am-pm -f daily"
+alias weh="weather zip 98109 -i --am-pm -f hourly"
 ```
 
 After adding this to the `~/.zshrc` you will need to restart your terminal. After that typing `we`
 will get the current forecast, `wed` will get the daily forecast and `weh` will get the hourly forecast.
 
 ## Examples
```

