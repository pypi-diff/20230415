# Comparing `tmp/pebbles_bot-0.2.0.tar.gz` & `tmp/pebbles_bot-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pebbles_bot-0.2.0.tar", last modified: Sun Mar 12 22:10:23 2023, max compression
+gzip compressed data, was "pebbles_bot-0.3.0.tar", last modified: Sat Apr 15 18:33:31 2023, max compression
```

## Comparing `pebbles_bot-0.2.0.tar` & `pebbles_bot-0.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 22:10:23.129950 pebbles_bot-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-03-12 22:10:13.000000 pebbles_bot-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-03-12 22:10:23.129950 pebbles_bot-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-03-12 22:10:13.000000 pebbles_bot-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 22:10:23.129950 pebbles_bot-0.2.0/pebbles_bot/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-03-12 22:10:13.000000 pebbles_bot-0.2.0/pebbles_bot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11902 2023-03-12 22:10:13.000000 pebbles_bot-0.2.0/pebbles_bot/pb_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-03-12 22:10:13.000000 pebbles_bot-0.2.0/pebbles_bot/pb_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-03-12 22:10:13.000000 pebbles_bot-0.2.0/pebbles_bot/pebot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 22:10:23.129950 pebbles_bot-0.2.0/pebbles_bot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-03-12 22:10:23.000000 pebbles_bot-0.2.0/pebbles_bot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-03-12 22:10:23.000000 pebbles_bot-0.2.0/pebbles_bot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-12 22:10:23.000000 pebbles_bot-0.2.0/pebbles_bot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-03-12 22:10:23.000000 pebbles_bot-0.2.0/pebbles_bot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-12 22:10:23.000000 pebbles_bot-0.2.0/pebbles_bot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-12 22:10:23.000000 pebbles_bot-0.2.0/pebbles_bot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-03-12 22:10:13.000000 pebbles_bot-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-03-12 22:10:23.129950 pebbles_bot-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-12 22:10:13.000000 pebbles_bot-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:33:31.457166 pebbles_bot-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-15 18:33:22.000000 pebbles_bot-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-04-15 18:33:31.457166 pebbles_bot-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-04-15 18:33:22.000000 pebbles_bot-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:33:31.457166 pebbles_bot-0.3.0/pebbles_bot/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-15 18:33:22.000000 pebbles_bot-0.3.0/pebbles_bot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9839 2023-04-15 18:33:22.000000 pebbles_bot-0.3.0/pebbles_bot/pb_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-04-15 18:33:22.000000 pebbles_bot-0.3.0/pebbles_bot/pb_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-04-15 18:33:22.000000 pebbles_bot-0.3.0/pebbles_bot/pebot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:33:31.457166 pebbles_bot-0.3.0/pebbles_bot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-04-15 18:33:31.000000 pebbles_bot-0.3.0/pebbles_bot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-15 18:33:31.000000 pebbles_bot-0.3.0/pebbles_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 18:33:31.000000 pebbles_bot-0.3.0/pebbles_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-15 18:33:31.000000 pebbles_bot-0.3.0/pebbles_bot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-15 18:33:31.000000 pebbles_bot-0.3.0/pebbles_bot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-15 18:33:31.000000 pebbles_bot-0.3.0/pebbles_bot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-15 18:33:22.000000 pebbles_bot-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-15 18:33:31.457166 pebbles_bot-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 18:33:22.000000 pebbles_bot-0.3.0/setup.py
```

### Comparing `pebbles_bot-0.2.0/LICENSE` & `pebbles_bot-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pebbles_bot-0.2.0/PKG-INFO` & `pebbles_bot-0.3.0/pebbles_bot.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pebbles_bot
-Version: 0.2.0
+Name: pebbles-bot
+Version: 0.3.0
 Summary: Telegram bot that runs Linux shell commands
 Home-page: https://github.com/Lab-Brat/pyLookout
 Author: Lab-Brat
 Author-email: labbrat_social@pm.me
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
@@ -15,108 +15,94 @@
 
 ## Table of content
 - [Table of content](#table-of-content)
 - [Introduction](#introduction)
     - [What It Can Do Now](#what-it-can-do-now)
     - [What It Will Do In The Future](#what-it-will-do-in-the-future)
     - [Is it secure to run a public bot with direct access to a server?](#is-it-secure-to-run-a-public-bot-with-direct-access-to-a-server)
-- [Deployment](#deployment)
+- [Deploy](#deploy)
 - [Run Pebbles](#run-pebbles)
 - [Command Guide](#command-guide)
 - [Prefix](#prefix)
     - [Running Pebbles in a Docker container](#running-pebbles-in-a-docker-container)
+    - [Configuration file](#configuration-file)
 
 ## Introduction
 Pebbles is a bot which allows users to run shell commands on their Linux servers from Telegram.  
-It is designed to be self-hosted. To get it up and running clone repository on the server, 
-ask [BotFather](https://core.telegram.org/bots#6-botfather) to create a bot, 
-save its API hash to `./pebbles_api`, and just run it!
+There are only 3 steps to get it up and running:
+1. Ask [BotFather](https://core.telegram.org/bots#6-botfather) to create a bot and save its API key.
+2. Install the bot on the server where you wish to run commands using Python pip.
+3. Configure environment variables and run it!
 
 #### What It Can Do Now
 At this stage Pebbles is not very sophisticated, it can:
 - Run commands locally.
 - Establish a SSH connection to another host and run commands there.
 - Send a notification by piping stdout.
+- Users whitelist - only whitelisted users can run commands on the bot.
 
 #### What It Will Do In The Future
-- More built-in commands to do various tasks.
-- Public key authentication for SSH connections.
-- Add support for custom plugins, like monitoring etc.
+- More built-in commands to do various tasks without entering long commands.
+- Commands whitelist - only whitelisted commands can be run on the bot.
+- Log parser that will block users or even shut the bot down if it detects a malicious activity.
 
 #### Is it secure to run a public bot with direct access to a server?
-The bot's channel itself is encrypted and secure by default. 
-To verify this, run `/setprivacy` on `@BotFather`, then check if privacy settings are enabled.  
-However, the bot can still be found by its handle and access to the server could be compromised. 
-That is why Pebbles has a built-in whitelisting mechanism to only allow certain users to run 
-commands on it.  
-Example of `pebbles_whitelist`
-```
-0123456789
-3141592653
-0112358132
-...
-```
-There is no limit on how much user IDs can be allowed, but the list cannot be empty. User ID 
-can be obtained from a public bot `@userinfobot`, by calling `/start` command on it.  
-So yeah, I'd say it is pretty secure :)
+The bot's channel is encrypted via Telegram's proprietary protocol - MTProto, and the API 
+also uses appropriate security measures, therefore there are no issues from Telegram's side.
+However, the bot is still a public service, and anyone on the internet can attempt to use it 
+(if they find bot's handle). That is why Pebbles has a whitelisting mechanism to only allow 
+certain users to run commands on it.  
+In general I'd say it's pretty safe to use, but don't use it on important production servers 😅
 
 
-## Deployment
+## Deploy
 - Ask [BotFather](https://core.telegram.org/bots#6-botfather) to create a bot, then save it's API key
-
-- Create a configuration file and paste your API key and authorized user IDs to it
-```yaml
----
-pebbles:
-  api_key: '....................'
-
-  whitelist:
-    - '0123456789'
-    - '3141592653' 
-```
-
-- Install the bot with pip
-```bash
-python -m pip install pebbles_bot
-```
-**Note** Alternatively the bot can be ran in a container, see [Prefix](#prefix)
+- Install the bot with pip `python -m pip install pebbles_bot`
+  **Note** Alternatively the bot can be ran in a container, see [Prefix](#prefix)
+- Define 2 environment variables:
+  - `PEBBLES_BOT_TOKEN` - the API key of the bot
+  - `PEBBLES_BOT_USERS` - a comma-separated list of Telegram user IDs that will be whitelisted.
+    User ID can be obtained from a public bot `@userinfobot`, by calling `/start` command on it.  
+- **Optionally** a yaml configuration file can be used to list users and set other options.
+  See [Configuration file](#configuration-file) for more details.
 
 
 ## Run Pebbles
-- Run in SSH proxy mode:
+Pebbles provides two modes of operation: Proxy and Notification modes. 
+In Proxy mode, will run commands that users send from Telegram on the server it's deployed on. 
+And in Notification mode it will send a Linux command/service output to the user from the server.  
+
+Run in proxy mode:
 ```bash
 pebot
 ```
 
-- Send notifications with it:
+Send notifications with Pebbles:
 ```bash
 echo 'Testing Notifications!' | pebot --notify
 ```
 
 ## Command Guide
 - `/start` -> start interacting with Pebbles.
 - `/help` -> print all available commands.
 - `/mode` -> choose Pebbles mode
   - `local`: run commands on the server it's deployed
   - `remote`: run commands on the remote server. To use this option a connection must be first established by `/login`.
-- `/login` -> establish a SSH connection to a remote host. User will be prompted for:  
-  - IP address or hostname.  
-    If port is not specified (8.8.8.8:22) then port 22 will be used.
-  - username
-  - password  
-    If `~/.ssh/config` has connection information (key and/or user), connection will still be established if a wrond password is entered.
+- `/login` -> establish a SSH connection to a remote host using information from `~/.ssh/config`. User will be prompted for:
+  - hostname  
+    should be the same as in `~/.ssh/config`
   - confirmation  
     select `Yes` to establish a connection, `No` to cancel.
 - `/logout` -> to terminate the SSH connection
 - `/run` -> run a shell command, where it runs depends on `/mode`. After command call user will be prompted to enter a command, stdout or stderr will be returned
 
 
 ## Prefix
 #### Running Pebbles in a Docker container
-**Note** This is not the recommended installation method, more like a fun alternative :)
+**Note** This is not the recommended installation method, more like a fun alternative 😉
 
 Create a `$HOME/.pebbles/pebbles.yaml` configuration file first 
 (`.pebbles` will be mounted to the container) and run:
 ```bash
 docker run -d --name pebot \
               --volume $HOME/.pebbles:/root/.pebbles \
               labbratnet/pebbles:0.1.1
@@ -126,7 +112,17 @@
 which can be customized. To use it, navigrate to `Docker` and run:
 ```bash
 docker build -t pebbles .
 docker run -d --name pebot \
               --volume $HOME/.pebbles:/root/.pebbles \
               pebbles
 ```
+
+#### Configuration file
+The default location is `$HOME/pebbles.yaml`, but it can be changed by setting the `PEBBLES_CONFIG` environment variable.  
+Example of the configuration file:
+```yaml
+whitelist_ids:
+  - 123456789
+  - 987654321
+```
+**Note** If both environment variables and configuration file are defined, the environment variables will take precedence.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pebbles_bot-0.2.0/README.md` & `pebbles_bot-0.3.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,107 +1,108 @@
+Metadata-Version: 2.1
+Name: pebbles_bot
+Version: 0.3.0
+Summary: Telegram bot that runs Linux shell commands
+Home-page: https://github.com/Lab-Brat/pyLookout
+Author: Lab-Brat
+Author-email: labbrat_social@pm.me
+License: MIT
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Operating System :: POSIX :: Linux
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 ## Table of content
 - [Table of content](#table-of-content)
 - [Introduction](#introduction)
     - [What It Can Do Now](#what-it-can-do-now)
     - [What It Will Do In The Future](#what-it-will-do-in-the-future)
     - [Is it secure to run a public bot with direct access to a server?](#is-it-secure-to-run-a-public-bot-with-direct-access-to-a-server)
-- [Deployment](#deployment)
+- [Deploy](#deploy)
 - [Run Pebbles](#run-pebbles)
 - [Command Guide](#command-guide)
 - [Prefix](#prefix)
     - [Running Pebbles in a Docker container](#running-pebbles-in-a-docker-container)
+    - [Configuration file](#configuration-file)
 
 ## Introduction
 Pebbles is a bot which allows users to run shell commands on their Linux servers from Telegram.  
-It is designed to be self-hosted. To get it up and running clone repository on the server, 
-ask [BotFather](https://core.telegram.org/bots#6-botfather) to create a bot, 
-save its API hash to `./pebbles_api`, and just run it!
+There are only 3 steps to get it up and running:
+1. Ask [BotFather](https://core.telegram.org/bots#6-botfather) to create a bot and save its API key.
+2. Install the bot on the server where you wish to run commands using Python pip.
+3. Configure environment variables and run it!
 
 #### What It Can Do Now
 At this stage Pebbles is not very sophisticated, it can:
 - Run commands locally.
 - Establish a SSH connection to another host and run commands there.
 - Send a notification by piping stdout.
+- Users whitelist - only whitelisted users can run commands on the bot.
 
 #### What It Will Do In The Future
-- More built-in commands to do various tasks.
-- Public key authentication for SSH connections.
-- Add support for custom plugins, like monitoring etc.
+- More built-in commands to do various tasks without entering long commands.
+- Commands whitelist - only whitelisted commands can be run on the bot.
+- Log parser that will block users or even shut the bot down if it detects a malicious activity.
 
 #### Is it secure to run a public bot with direct access to a server?
-The bot's channel itself is encrypted and secure by default. 
-To verify this, run `/setprivacy` on `@BotFather`, then check if privacy settings are enabled.  
-However, the bot can still be found by its handle and access to the server could be compromised. 
-That is why Pebbles has a built-in whitelisting mechanism to only allow certain users to run 
-commands on it.  
-Example of `pebbles_whitelist`
-```
-0123456789
-3141592653
-0112358132
-...
-```
-There is no limit on how much user IDs can be allowed, but the list cannot be empty. User ID 
-can be obtained from a public bot `@userinfobot`, by calling `/start` command on it.  
-So yeah, I'd say it is pretty secure :)
+The bot's channel is encrypted via Telegram's proprietary protocol - MTProto, and the API 
+also uses appropriate security measures, therefore there are no issues from Telegram's side.
+However, the bot is still a public service, and anyone on the internet can attempt to use it 
+(if they find bot's handle). That is why Pebbles has a whitelisting mechanism to only allow 
+certain users to run commands on it.  
+In general I'd say it's pretty safe to use, but don't use it on important production servers 😅
 
 
-## Deployment
+## Deploy
 - Ask [BotFather](https://core.telegram.org/bots#6-botfather) to create a bot, then save it's API key
-
-- Create a configuration file and paste your API key and authorized user IDs to it
-```yaml
----
-pebbles:
-  api_key: '....................'
-
-  whitelist:
-    - '0123456789'
-    - '3141592653' 
-```
-
-- Install the bot with pip
-```bash
-python -m pip install pebbles_bot
-```
-**Note** Alternatively the bot can be ran in a container, see [Prefix](#prefix)
+- Install the bot with pip `python -m pip install pebbles_bot`
+  **Note** Alternatively the bot can be ran in a container, see [Prefix](#prefix)
+- Define 2 environment variables:
+  - `PEBBLES_BOT_TOKEN` - the API key of the bot
+  - `PEBBLES_BOT_USERS` - a comma-separated list of Telegram user IDs that will be whitelisted.
+    User ID can be obtained from a public bot `@userinfobot`, by calling `/start` command on it.  
+- **Optionally** a yaml configuration file can be used to list users and set other options.
+  See [Configuration file](#configuration-file) for more details.
 
 
 ## Run Pebbles
-- Run in SSH proxy mode:
+Pebbles provides two modes of operation: Proxy and Notification modes. 
+In Proxy mode, will run commands that users send from Telegram on the server it's deployed on. 
+And in Notification mode it will send a Linux command/service output to the user from the server.  
+
+Run in proxy mode:
 ```bash
 pebot
 ```
 
-- Send notifications with it:
+Send notifications with Pebbles:
 ```bash
 echo 'Testing Notifications!' | pebot --notify
 ```
 
 ## Command Guide
 - `/start` -> start interacting with Pebbles.
 - `/help` -> print all available commands.
 - `/mode` -> choose Pebbles mode
   - `local`: run commands on the server it's deployed
   - `remote`: run commands on the remote server. To use this option a connection must be first established by `/login`.
-- `/login` -> establish a SSH connection to a remote host. User will be prompted for:  
-  - IP address or hostname.  
-    If port is not specified (8.8.8.8:22) then port 22 will be used.
-  - username
-  - password  
-    If `~/.ssh/config` has connection information (key and/or user), connection will still be established if a wrond password is entered.
+- `/login` -> establish a SSH connection to a remote host using information from `~/.ssh/config`. User will be prompted for:
+  - hostname  
+    should be the same as in `~/.ssh/config`
   - confirmation  
     select `Yes` to establish a connection, `No` to cancel.
 - `/logout` -> to terminate the SSH connection
 - `/run` -> run a shell command, where it runs depends on `/mode`. After command call user will be prompted to enter a command, stdout or stderr will be returned
 
 
 ## Prefix
 #### Running Pebbles in a Docker container
-**Note** This is not the recommended installation method, more like a fun alternative :)
+**Note** This is not the recommended installation method, more like a fun alternative 😉
 
 Create a `$HOME/.pebbles/pebbles.yaml` configuration file first 
 (`.pebbles` will be mounted to the container) and run:
 ```bash
 docker run -d --name pebot \
               --volume $HOME/.pebbles:/root/.pebbles \
               labbratnet/pebbles:0.1.1
@@ -111,7 +112,17 @@
 which can be customized. To use it, navigrate to `Docker` and run:
 ```bash
 docker build -t pebbles .
 docker run -d --name pebot \
               --volume $HOME/.pebbles:/root/.pebbles \
               pebbles
 ```
+
+#### Configuration file
+The default location is `$HOME/pebbles.yaml`, but it can be changed by setting the `PEBBLES_CONFIG` environment variable.  
+Example of the configuration file:
+```yaml
+whitelist_ids:
+  - 123456789
+  - 987654321
+```
+**Note** If both environment variables and configuration file are defined, the environment variables will take precedence.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pebbles_bot-0.2.0/pebbles_bot/pb_main.py` & `pebbles_bot-0.3.0/pebbles_bot/pb_main.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import logging
 from pathlib import Path
-from socket import gethostbyname
 from .pb_tools import security_check, Tools, SSH_Tools
 
 from telebot import TeleBot
 from telebot.apihelper import ApiTelegramException
 from telebot.types import (
     InlineKeyboardMarkup as ik_markup,
     InlineKeyboardButton as ik_button,
@@ -20,17 +19,15 @@
 
         self.uid_whitelist = whitelist
 
         logging.basicConfig(
             format="%(asctime)s %(message)s",
             level=logging.INFO,
             handlers=[
-                logging.FileHandler(
-                    f"{str(Path.home())}/.pebbles/pebbles.log"
-                ),
+                logging.FileHandler(f"{str(Path.home())}/.pebbles.log"),
                 logging.StreamHandler(),
             ],
         )
         self.logger = logging.getLogger()
 
         @self.bot.message_handler(commands=["start"])
         def _start(message):
@@ -146,90 +143,29 @@
         """
         /login command
         Function: initialize SSH connection
         """
         self.log(message, log="/login")
         self.bot.send_message(
             message.from_user.id,
-            "Enter **IP address**  [format -> IP:port]",
+            "Enter *hostname*\n(as defined in `~/.ssh/config`)",
             parse_mode="markdown",
         )
-        self.bot.register_next_step_handler(message, self.get_ip)
+        self.bot.register_next_step_handler(message, self.get_hostname)
 
-    def _valid_ip_hn(self, ip):
+    def get_hostname(self, message):
         """
-        Check if input is a valid IP address,
-        or try to resolve it in case of a hostname.
-        Return a boolean.
+        Takes hostname (as defined in ~/.ssh/config),
         """
-        try:
-            gethostbyname(ip)
-            return True
-        except:
-            return False
-
-    def _parse_ip(self, message):
-        """
-        Takes <ip>:<port> as input,
-        validates IP and reads it and port into a dict.
-        If port is missing, default SSH port is assigned.
-        """
-        msg_split = message.text.split(":")
-        host = msg_split[0]
-        port = "22" if len(msg_split) == 1 else msg_split[1]
-        resolved = True if self._valid_ip_hn(host) else False
-        return {"host": host, "port": port, "resolved": resolved}
-
-    def get_ip(self, message):
-        """
-        Takes IP address and port of the remote host as input,
-        redirects to get_uname
-        """
-        self.log(message, "called get_ip method")
-        self.host = self._parse_ip(message)
-        if not self.host["resolved"]:
-            err_message = f"{self.host['host']} cannot be resolved"
-            self.bot.send_message(message.from_user.id, err_message)
-            self.log(message, err_message)
-        else:
-            self.bot.send_message(
-                message.from_user.id,
-                "Enter **username**",
-                parse_mode="markdown",
-            )
-            self.bot.register_next_step_handler(message, self.get_uname)
-
-    def get_uname(self, message):
-        """
-        Takes username of the remote host as input,
-        redirects to get_pass
-        """
-        self.log(message, "called get_uname method")
-        self.uname = message.text
-        self.bot.send_message(
-            message.from_user.id, "Enter **password**", parse_mode="markdown"
-        )
-        self.bot.register_next_step_handler(message, self.get_pass)
-
-    def get_pass(self, message):
-        """
-        Takes remote host's password as input,
-        displays confirmation message
-        """
-        self.log(message, "called get_pass method")
-        self.paswd = message.text
-
+        self.log(message, "called get_hostname method")
+        self.host = message.text
         keyboard = ik_markup()
         keyboard.add(ik_button(text="yes", callback_data="yes"))
         keyboard.add(ik_button(text="no", callback_data="no"))
-        question = (
-            f"Establish SSH connection to "
-            f"{self.host['host']}:{self.host['port']} "
-            f"with user `{self.uname}`?"
-        )
+        question = f"Establish SSH connection to {self.host}"
 
         self.bot.send_message(
             message.from_user.id,
             text=question,
             reply_markup=keyboard,
             parse_mode="markdown",
         )
@@ -296,34 +232,36 @@
     def _connect(self, chat_id, con_result):
         """
         Use Paramiko to connect to remote host,
         return connection status.
         """
         if con_result == True:
             self.bot.send_message(chat_id, "Login Success 🔗")
-        elif con_result == "pass":
-            self.bot.send_message(chat_id, "Login Failed, Wrong Password ❌")
-        elif con_result == "port":
-            self.bot.send_message(chat_id, "Login Failed, Wrong Port ❌")
-        elif con_result == "time":
+        elif con_result == "key_not_found":
+            self.bot.send_message(chat_id, "Login Failed, No Key In Config ❌")
+        elif con_result == "timeout":
             self.bot.send_message(
                 chat_id, "Login Failed, Connection Timed Out ❌"
             )
+        elif con_result == "config_not_found":
+            self.bot.send_message(
+                chat_id, "Login Failed, ~/.ssh/config File Not Found ❌"
+            )
+        else:
+            self.bot.send_message(chat_id, "Login Failed, Reason Unclear ❌")
 
     def callback_worker(self, call):
         """
         Process callback data from the confirmation message,
         if callback is yes - establish a SSH connection,
         if callback is no - suggest to run /login again
         """
         if call.data == "yes":
             self.log(call, "pressed YES on the keyboard")
-            con_result = self.ssh.ssh_connect(
-                self.host["host"], self.host["port"], self.uname, self.paswd
-            )
+            con_result = self.ssh.ssh_connect(self.host)
             self._connect(call.message.chat.id, con_result)
         elif call.data == "no":
             self.log(call, "pressed NO on the keyboard")
             self.bot.send_message(
                 call.message.chat.id, "To start over enter /login again ♻️"
             )
         elif call.data == "remote":
```

### Comparing `pebbles_bot-0.2.0/pebbles_bot/pb_tools.py` & `pebbles_bot-0.3.0/pebbles_bot/pb_tools.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,10 @@
+import os
 from subprocess import PIPE, STDOUT, Popen
-from paramiko import SSHClient, AutoAddPolicy
+from paramiko import SSHConfig, SSHClient, AutoAddPolicy
 from paramiko.ssh_exception import (
     AuthenticationException,
     NoValidConnectionsError,
 )
 
 
 def security_check(method):
@@ -27,30 +28,48 @@
             self.log(message, f">!< {uid} was BLOCKED")
 
     return wrapper
 
 
 class SSH_Tools:
     def __init__(self):
+        self.config = SSHConfig()
+        self.read_ssh_config()
+
         self.client = SSHClient()
         self.client.set_missing_host_key_policy(AutoAddPolicy())
 
-    def ssh_connect(self, host, port, uname, pwd):
+    def read_ssh_config(self):
+        """
+        Read SSH config file and return a dictionary
+        """
+        ssh_config_file = os.path.expanduser("~/.ssh/config")
+        with open(ssh_config_file) as f:
+            self.config.parse(f)
+
+    def ssh_connect(self, host):
         """
         Establish a SSH connection
         """
         try:
-            self.client.connect(host, port=port, username=uname, password=pwd)
-            return True
-        except AuthenticationException:
-            return "pass"
-        except NoValidConnectionsError:
-            return "port"
+            host_config = self.config.lookup(host)
+            if "identityfile" not in host_config:
+                return "key_not_found"
+            else:
+                self.client.connect(
+                    host_config["hostname"],
+                    username=host_config.get("user"),
+                    port=host_config.get("port"),
+                    key_filename=host_config.get("identityfile"),
+                )
+                return True
         except TimeoutError:
-            return "time"
+            return "timeout"
+        except:
+            return "config_not_found"
 
     def ssh_disconnect(self):
         """
         Terminate a SSH connection
         """
         self.client.close()
```

### Comparing `pebbles_bot-0.2.0/pebbles_bot.egg-info/PKG-INFO` & `pebbles_bot-0.3.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,122 +1,93 @@
-Metadata-Version: 2.1
-Name: pebbles-bot
-Version: 0.2.0
-Summary: Telegram bot that runs Linux shell commands
-Home-page: https://github.com/Lab-Brat/pyLookout
-Author: Lab-Brat
-Author-email: labbrat_social@pm.me
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Operating System :: POSIX :: Linux
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ## Table of content
 - [Table of content](#table-of-content)
 - [Introduction](#introduction)
     - [What It Can Do Now](#what-it-can-do-now)
     - [What It Will Do In The Future](#what-it-will-do-in-the-future)
     - [Is it secure to run a public bot with direct access to a server?](#is-it-secure-to-run-a-public-bot-with-direct-access-to-a-server)
-- [Deployment](#deployment)
+- [Deploy](#deploy)
 - [Run Pebbles](#run-pebbles)
 - [Command Guide](#command-guide)
 - [Prefix](#prefix)
     - [Running Pebbles in a Docker container](#running-pebbles-in-a-docker-container)
+    - [Configuration file](#configuration-file)
 
 ## Introduction
 Pebbles is a bot which allows users to run shell commands on their Linux servers from Telegram.  
-It is designed to be self-hosted. To get it up and running clone repository on the server, 
-ask [BotFather](https://core.telegram.org/bots#6-botfather) to create a bot, 
-save its API hash to `./pebbles_api`, and just run it!
+There are only 3 steps to get it up and running:
+1. Ask [BotFather](https://core.telegram.org/bots#6-botfather) to create a bot and save its API key.
+2. Install the bot on the server where you wish to run commands using Python pip.
+3. Configure environment variables and run it!
 
 #### What It Can Do Now
 At this stage Pebbles is not very sophisticated, it can:
 - Run commands locally.
 - Establish a SSH connection to another host and run commands there.
 - Send a notification by piping stdout.
+- Users whitelist - only whitelisted users can run commands on the bot.
 
 #### What It Will Do In The Future
-- More built-in commands to do various tasks.
-- Public key authentication for SSH connections.
-- Add support for custom plugins, like monitoring etc.
+- More built-in commands to do various tasks without entering long commands.
+- Commands whitelist - only whitelisted commands can be run on the bot.
+- Log parser that will block users or even shut the bot down if it detects a malicious activity.
 
 #### Is it secure to run a public bot with direct access to a server?
-The bot's channel itself is encrypted and secure by default. 
-To verify this, run `/setprivacy` on `@BotFather`, then check if privacy settings are enabled.  
-However, the bot can still be found by its handle and access to the server could be compromised. 
-That is why Pebbles has a built-in whitelisting mechanism to only allow certain users to run 
-commands on it.  
-Example of `pebbles_whitelist`
-```
-0123456789
-3141592653
-0112358132
-...
-```
-There is no limit on how much user IDs can be allowed, but the list cannot be empty. User ID 
-can be obtained from a public bot `@userinfobot`, by calling `/start` command on it.  
-So yeah, I'd say it is pretty secure :)
+The bot's channel is encrypted via Telegram's proprietary protocol - MTProto, and the API 
+also uses appropriate security measures, therefore there are no issues from Telegram's side.
+However, the bot is still a public service, and anyone on the internet can attempt to use it 
+(if they find bot's handle). That is why Pebbles has a whitelisting mechanism to only allow 
+certain users to run commands on it.  
+In general I'd say it's pretty safe to use, but don't use it on important production servers 😅
 
 
-## Deployment
+## Deploy
 - Ask [BotFather](https://core.telegram.org/bots#6-botfather) to create a bot, then save it's API key
-
-- Create a configuration file and paste your API key and authorized user IDs to it
-```yaml
----
-pebbles:
-  api_key: '....................'
-
-  whitelist:
-    - '0123456789'
-    - '3141592653' 
-```
-
-- Install the bot with pip
-```bash
-python -m pip install pebbles_bot
-```
-**Note** Alternatively the bot can be ran in a container, see [Prefix](#prefix)
+- Install the bot with pip `python -m pip install pebbles_bot`
+  **Note** Alternatively the bot can be ran in a container, see [Prefix](#prefix)
+- Define 2 environment variables:
+  - `PEBBLES_BOT_TOKEN` - the API key of the bot
+  - `PEBBLES_BOT_USERS` - a comma-separated list of Telegram user IDs that will be whitelisted.
+    User ID can be obtained from a public bot `@userinfobot`, by calling `/start` command on it.  
+- **Optionally** a yaml configuration file can be used to list users and set other options.
+  See [Configuration file](#configuration-file) for more details.
 
 
 ## Run Pebbles
-- Run in SSH proxy mode:
+Pebbles provides two modes of operation: Proxy and Notification modes. 
+In Proxy mode, will run commands that users send from Telegram on the server it's deployed on. 
+And in Notification mode it will send a Linux command/service output to the user from the server.  
+
+Run in proxy mode:
 ```bash
 pebot
 ```
 
-- Send notifications with it:
+Send notifications with Pebbles:
 ```bash
 echo 'Testing Notifications!' | pebot --notify
 ```
 
 ## Command Guide
 - `/start` -> start interacting with Pebbles.
 - `/help` -> print all available commands.
 - `/mode` -> choose Pebbles mode
   - `local`: run commands on the server it's deployed
   - `remote`: run commands on the remote server. To use this option a connection must be first established by `/login`.
-- `/login` -> establish a SSH connection to a remote host. User will be prompted for:  
-  - IP address or hostname.  
-    If port is not specified (8.8.8.8:22) then port 22 will be used.
-  - username
-  - password  
-    If `~/.ssh/config` has connection information (key and/or user), connection will still be established if a wrond password is entered.
+- `/login` -> establish a SSH connection to a remote host using information from `~/.ssh/config`. User will be prompted for:
+  - hostname  
+    should be the same as in `~/.ssh/config`
   - confirmation  
     select `Yes` to establish a connection, `No` to cancel.
 - `/logout` -> to terminate the SSH connection
 - `/run` -> run a shell command, where it runs depends on `/mode`. After command call user will be prompted to enter a command, stdout or stderr will be returned
 
 
 ## Prefix
 #### Running Pebbles in a Docker container
-**Note** This is not the recommended installation method, more like a fun alternative :)
+**Note** This is not the recommended installation method, more like a fun alternative 😉
 
 Create a `$HOME/.pebbles/pebbles.yaml` configuration file first 
 (`.pebbles` will be mounted to the container) and run:
 ```bash
 docker run -d --name pebot \
               --volume $HOME/.pebbles:/root/.pebbles \
               labbratnet/pebbles:0.1.1
@@ -126,7 +97,17 @@
 which can be customized. To use it, navigrate to `Docker` and run:
 ```bash
 docker build -t pebbles .
 docker run -d --name pebot \
               --volume $HOME/.pebbles:/root/.pebbles \
               pebbles
 ```
+
+#### Configuration file
+The default location is `$HOME/pebbles.yaml`, but it can be changed by setting the `PEBBLES_CONFIG` environment variable.  
+Example of the configuration file:
+```yaml
+whitelist_ids:
+  - 123456789
+  - 987654321
+```
+**Note** If both environment variables and configuration file are defined, the environment variables will take precedence.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pebbles_bot-0.2.0/setup.cfg` & `pebbles_bot-0.3.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pebbles_bot
-version = 0.2.0
+version = 0.3.0
 description = Telegram bot that runs Linux shell commands
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Lab-Brat
 author_email = labbrat_social@pm.me
 url = https://github.com/Lab-Brat/pyLookout
 license = MIT
```

