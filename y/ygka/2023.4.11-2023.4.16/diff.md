# Comparing `tmp/ygka-2023.4.11.tar.gz` & `tmp/ygka-2023.4.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ygka-2023.4.11.tar", max compression
+gzip compressed data, was "ygka-2023.4.16.tar", max compression
```

## Comparing `ygka-2023.4.11.tar` & `ygka-2023.4.16.tar`

### file list

```diff
@@ -1,31 +1,28 @@
--rw-r--r--   0        0        0     1068 2023-04-11 08:06:45.484779 ygka-2023.4.11/LICENSE
--rw-r--r--   0        0        0     2810 2023-04-11 08:06:45.484779 ygka-2023.4.11/README.md
--rw-r--r--   0        0        0     1409 2023-04-11 08:07:11.336987 ygka-2023.4.11/pyproject.toml
--rw-r--r--   0        0        0       53 2023-04-11 08:06:45.496778 ygka-2023.4.11/ygka/__init__.py
--rw-r--r--   0        0        0      119 2023-04-11 08:06:45.496778 ygka-2023.4.11/ygka/__main__.py
--rw-r--r--   0        0        0       78 2023-04-11 08:06:45.496778 ygka-2023.4.11/ygka/adapters/__init__.py
--rw-r--r--   0        0        0     1151 2023-04-11 08:06:45.496778 ygka-2023.4.11/ygka/adapters/openai_cookie_adapter.py
--rw-r--r--   0        0        0      704 2023-04-11 08:06:45.496778 ygka-2023.4.11/ygka/adapters/test/test_openai_cookie_adapter.py
--rw-r--r--   0        0        0       84 2023-04-11 08:06:45.496778 ygka-2023.4.11/ygka/cli/__init__.py
--rw-r--r--   0        0        0       43 2023-04-11 08:06:45.496778 ygka-2023.4.11/ygka/cli/cli_app.py
--rw-r--r--   0        0        0     2824 2023-04-11 08:06:45.496778 ygka-2023.4.11/ygka/cli/config_ygka.py
--rw-r--r--   0        0        0      112 2023-04-11 08:06:45.496778 ygka-2023.4.11/ygka/cli/retrieve_stdin.py
--rw-r--r--   0        0        0     1751 2023-04-11 08:06:45.496778 ygka-2023.4.11/ygka/cli/ygka.py
--rw-r--r--   0        0        0       90 2023-04-11 08:06:45.496778 ygka-2023.4.11/ygka/exceptions/__init__.py
--rw-r--r--   0        0        0       51 2023-04-11 08:06:45.496778 ygka-2023.4.11/ygka/exceptions/unauthorized_access_error.py
--rw-r--r--   0        0        0      234 2023-04-11 08:06:45.496778 ygka-2023.4.11/ygka/models/__init__.py
--rw-r--r--   0        0        0      155 2023-04-11 08:06:45.496778 ygka-2023.4.11/ygka/models/language_model.py
--rw-r--r--   0        0        0      705 2023-04-11 08:06:45.496778 ygka-2023.4.11/ygka/models/revchatgpt_chatbot_config_model.py
--rw-r--r--   0        0        0      403 2023-04-11 08:06:45.496778 ygka-2023.4.11/ygka/models/str_enum.py
--rw-r--r--   0        0        0     1038 2023-04-11 08:06:45.496778 ygka-2023.4.11/ygka/models/ygka_config_model.py
--rw-r--r--   0        0        0      324 2023-04-11 08:06:45.496778 ygka-2023.4.11/ygka/query_clients/__init__.py
--rw-r--r--   0        0        0      714 2023-04-11 08:06:45.496778 ygka-2023.4.11/ygka/query_clients/official_chatgpt_client.py
--rw-r--r--   0        0        0      155 2023-04-11 08:06:45.496778 ygka-2023.4.11/ygka/query_clients/query_client.py
--rw-r--r--   0        0        0      868 2023-04-11 08:06:45.496778 ygka-2023.4.11/ygka/query_clients/query_client_factory.py
--rw-r--r--   0        0        0     1661 2023-04-11 08:06:45.496778 ygka-2023.4.11/ygka/query_clients/reverse_engineered_chatgpt_client.py
--rw-r--r--   0        0        0        0 2023-04-11 08:06:45.496778 ygka-2023.4.11/ygka/tests/__init__.py
--rw-r--r--   0        0        0       58 2023-04-11 08:06:45.496778 ygka-2023.4.11/ygka/tests/test_sample.py
--rw-r--r--   0        0        0       73 2023-04-11 08:06:45.496778 ygka-2023.4.11/ygka/utils/__init__.py
--rw-r--r--   0        0        0      334 2023-04-11 08:06:45.496778 ygka-2023.4.11/ygka/utils/test/test_ygka_config_manager.py
--rw-r--r--   0        0        0     1669 2023-04-11 08:06:45.496778 ygka-2023.4.11/ygka/utils/ygka_config_manager.py
--rw-r--r--   0        0        0     3384 1970-01-01 00:00:00.000000 ygka-2023.4.11/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-04-15 16:01:50.252825 ygka-2023.4.16/LICENSE
+-rw-r--r--   0        0        0     2810 2023-04-15 16:01:50.252825 ygka-2023.4.16/README.md
+-rw-r--r--   0        0        0     1435 2023-04-15 16:02:44.005442 ygka-2023.4.16/pyproject.toml
+-rw-r--r--   0        0        0       53 2023-04-15 16:01:50.264825 ygka-2023.4.16/ygka/__init__.py
+-rw-r--r--   0        0        0      119 2023-04-15 16:01:50.264825 ygka-2023.4.16/ygka/__main__.py
+-rw-r--r--   0        0        0       84 2023-04-15 16:01:50.264825 ygka-2023.4.16/ygka/cli/__init__.py
+-rw-r--r--   0        0        0       43 2023-04-15 16:01:50.264825 ygka-2023.4.16/ygka/cli/cli_app.py
+-rw-r--r--   0        0        0     2112 2023-04-15 16:01:50.264825 ygka-2023.4.16/ygka/cli/config_ygka.py
+-rw-r--r--   0        0        0      112 2023-04-15 16:01:50.264825 ygka-2023.4.16/ygka/cli/retrieve_stdin.py
+-rw-r--r--   0        0        0     1424 2023-04-15 16:01:50.264825 ygka-2023.4.16/ygka/cli/ygka.py
+-rw-r--r--   0        0        0       90 2023-04-15 16:01:50.264825 ygka-2023.4.16/ygka/exceptions/__init__.py
+-rw-r--r--   0        0        0       51 2023-04-15 16:01:50.264825 ygka-2023.4.16/ygka/exceptions/unauthorized_access_error.py
+-rw-r--r--   0        0        0      234 2023-04-15 16:01:50.264825 ygka-2023.4.16/ygka/models/__init__.py
+-rw-r--r--   0        0        0      155 2023-04-15 16:01:50.264825 ygka-2023.4.16/ygka/models/language_model.py
+-rw-r--r--   0        0        0      705 2023-04-15 16:01:50.264825 ygka-2023.4.16/ygka/models/revchatgpt_chatbot_config_model.py
+-rw-r--r--   0        0        0      403 2023-04-15 16:01:50.264825 ygka-2023.4.16/ygka/models/str_enum.py
+-rw-r--r--   0        0        0      933 2023-04-15 16:01:50.264825 ygka-2023.4.16/ygka/models/ygka_config_model.py
+-rw-r--r--   0        0        0      324 2023-04-15 16:01:50.264825 ygka-2023.4.16/ygka/query_clients/__init__.py
+-rw-r--r--   0        0        0      714 2023-04-15 16:01:50.264825 ygka-2023.4.16/ygka/query_clients/official_chatgpt_client.py
+-rw-r--r--   0        0        0      155 2023-04-15 16:01:50.264825 ygka-2023.4.16/ygka/query_clients/query_client.py
+-rw-r--r--   0        0        0     1266 2023-04-15 16:01:50.264825 ygka-2023.4.16/ygka/query_clients/query_client_factory.py
+-rw-r--r--   0        0        0     1661 2023-04-15 16:01:50.264825 ygka-2023.4.16/ygka/query_clients/reverse_engineered_chatgpt_client.py
+-rw-r--r--   0        0        0        0 2023-04-15 16:01:50.264825 ygka-2023.4.16/ygka/tests/__init__.py
+-rw-r--r--   0        0        0       58 2023-04-15 16:01:50.264825 ygka-2023.4.16/ygka/tests/test_sample.py
+-rw-r--r--   0        0        0       73 2023-04-15 16:01:50.264825 ygka-2023.4.16/ygka/utils/__init__.py
+-rw-r--r--   0        0        0      334 2023-04-15 16:01:50.264825 ygka-2023.4.16/ygka/utils/test/test_ygka_config_manager.py
+-rw-r--r--   0        0        0     1683 2023-04-15 16:01:50.264825 ygka-2023.4.16/ygka/utils/ygka_config_manager.py
+-rw-r--r--   0        0        0     3393 1970-01-01 00:00:00.000000 ygka-2023.4.16/PKG-INFO
```

### Comparing `ygka-2023.4.11/LICENSE` & `ygka-2023.4.16/LICENSE`

 * *Files identical despite different names*

### Comparing `ygka-2023.4.11/README.md` & `ygka-2023.4.16/README.md`

 * *Files identical despite different names*

### Comparing `ygka-2023.4.11/pyproject.toml` & `ygka-2023.4.16/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "ygka"
-version = "2023.04.11"
+version = "v2023.04.16"
 description = ""
 authors = []
 readme = "README.md"
 
 [tool.pyright]
 typeCheckingMode = "strict"
 pythonPlatform = "All"
@@ -27,23 +27,23 @@
 spaces_before_comment = 2
 split_before_logical_operator = true
 column_limit = 119
 allow_split_before_dict_value = false
 
 [tool.ruff]
 line-length = 119
-select = [ "PLE", "PLR", "PLW", "E", "W", "F", "I", "Q",]
+select = [ "PLE", "PLW", "E", "W", "F", "I", "Q",]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 poetry = "^1.4.0"
 rich = "<13.0.0"
-revchatgpt = "^4.1.6"
-pydantic = "^1.10.5"
-yt-dlp = "^2023.3.4"
+revchatgpt = "^4.2.2"
+pydantic = "^1.10.7"
+revchatgptauth = "^2023.4.16"
 
 [tool.poetry.scripts]
 ygka = "ygka:main"
 
 [tool.ruff.flake8-quotes]
 inline-quotes = "single"
 docstring-quotes = "single"
@@ -54,15 +54,16 @@
 
 [tool.poetry.dependencies.typer]
 extras = [ "all",]
 version = "^0.7.0"
 
 [tool.poetry.group.dev.dependencies]
 toml = "^0.10.2"
+types-toml = "^0.10.8.6"
+invoke = "^2.0.0"
+types-invoke = "^2.0.0.6"
+ruff = "^0.0.261"
 yapf = "^0.32.0"
+pyright = "^1.1.302"
 pytest = "^7.2.2"
 pytest-cov = "^4.0.0"
-invoke = "^1.7.3"
-ruff = "^0.0.199"
-types-invoke = "^1.7.3.16"
-types-toml = "^0.10.8.5"
-pyright = "^1.1.296"
+pytest-sugar = "^0.9.7"
```

### Comparing `ygka-2023.4.11/ygka/cli/config_ygka.py` & `ygka-2023.4.16/ygka/cli/config_ygka.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import sys
 
 import rich
 import typer
-from yt_dlp.cookies import SUPPORTED_BROWSERS
+from revChatGPTAuth import SupportedBrowser
 
-from ygka.adapters.openai_cookie_adapter import OpenAICookieAdapter
-from ygka.models import RevChatGPTChatbotConfigModel
 from ygka.models.ygka_config_model import YGKAConfigModel
 from ygka.utils import YGKAConfigManager
 
 
 def config_ygka():
+    SUPPORTED_BROWSERS = [browser.value for browser in SupportedBrowser]
     rich.print('''
 Hi! 🙌 I am [bold blue]YGKA[/bold blue]!
 [yellow][blue bold underline]Y[/blue bold underline]our
 [blue bold underline]G[/blue bold underline]enius,
 [blue bold underline]K[/blue bold underline]nowledgeable assistant
 [blue bold underline]A[/blue bold underline]n advanced ChatGPT client[/yellow] 🔥
 I am here to assist you with configuring YGKA. 💪
@@ -29,43 +28,33 @@
 
 We support the following browsers: [{SUPPORTED_BROWSERS}]'''[1:])
     browser_name = typer.prompt('Please enter your choice here: ')
     if browser_name not in SUPPORTED_BROWSERS:
         rich.print(f'Browser {browser_name} is not supported. Supported browsers are: {SUPPORTED_BROWSERS}')
         sys.exit(1)
 
-    adapter = OpenAICookieAdapter(browser_name)
-    session_token = adapter.get_openai_session_token()
-    if not session_token:
-        rich.print('Failed to get session token. 😓 Can you check if you are logged in to https://chat.openai.com?')
-        sys.exit(1)
-
-    config_manager = save_config(session_token)
+    config_manager = save_config(browser_name)
 
     rich.print(f'''
 [green bold]Excellent![/green bold] You are now ready to use [bold blue]YGKA[/bold blue] 🚀
 
 Enjoy your AI powered terminal assistant! 🎉
 
 [dim]To check your settings file, it's at: {config_manager.config_path}[/dim]
 
 '''[1:])
     return config_manager
 
 
-def save_config(session_token: str):
+def save_config(browser_name: str):
+    config_manager: YGKAConfigManager = YGKAConfigManager()
+
     is_config_file_available = YGKAConfigManager.is_config_file_available(YGKAConfigManager.DEFAULT_CONFIG_PATH)
     if is_config_file_available:
         config_manager = YGKAConfigManager(load_config=True)
-        is_chatgpt_config_available = config_manager.config_model.chatgpt_config is not None
-        if is_chatgpt_config_available:
-            assert config_manager.config_model.chatgpt_config  # for type hinting
-            config_manager.config_model.chatgpt_config.session_token = session_token
-        else:
-            config_manager.config_model.chatgpt_config = RevChatGPTChatbotConfigModel(session_token=session_token)
+        config_manager.config_model.browser_name = browser_name
     else:
-        chatgpt_config = RevChatGPTChatbotConfigModel(session_token=session_token)
-        YGKA_config = YGKAConfigModel(chatgpt_config=chatgpt_config)
+        YGKA_config = YGKAConfigModel(browser_name=browser_name)
         config_manager = YGKAConfigManager(config_model=YGKA_config)
 
     config_manager.save_config()
     return config_manager
```

### Comparing `ygka-2023.4.11/ygka/models/revchatgpt_chatbot_config_model.py` & `ygka-2023.4.16/ygka/models/revchatgpt_chatbot_config_model.py`

 * *Files identical despite different names*

### Comparing `ygka-2023.4.11/ygka/models/ygka_config_model.py` & `ygka-2023.4.16/ygka/models/ygka_config_model.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 from typing import Optional
 
 from pydantic import BaseModel, root_validator
 
 from .language_model import LanguageModel
-from .revchatgpt_chatbot_config_model import RevChatGPTChatbotConfigModel
 
 
 class YGKAConfigModel(BaseModel):
     language_model: LanguageModel = LanguageModel.REVERSE_ENGINEERED_CHATGPT
-    chatgpt_config: Optional[RevChatGPTChatbotConfigModel] = None
+    browser_name: Optional[str] = None
     openai_api_key: Optional[str] = None
 
     @root_validator
     def check_required_info_provided(cls, values: dict[str, Optional[str]]):
         language_model = values.get('language_model')
         if language_model == LanguageModel.REVERSE_ENGINEERED_CHATGPT:
-            if not values.get('chatgpt_config'):
-                raise ValueError(f'chatgpt_config should not be none if language_model is {language_model}')
+            if not values.get('browser_name'):
+                raise ValueError(f'browser_name should not be none if language_model is {language_model}')
         elif language_model == LanguageModel.OFFICIAL_CHATGPT:
             if not values.get('openai_api_key'):
                 raise ValueError(f'openai_api_key should not be none if language_model is {language_model}')
 
         return values
```

### Comparing `ygka-2023.4.11/ygka/query_clients/official_chatgpt_client.py` & `ygka-2023.4.16/ygka/query_clients/official_chatgpt_client.py`

 * *Files identical despite different names*

### Comparing `ygka-2023.4.11/ygka/query_clients/query_client_factory.py` & `ygka-2023.4.16/ygka/query_clients/query_client_factory.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,27 @@
-from ygka.models import LanguageModel, YGKAConfigModel
+from typing import cast
+
+from revChatGPTAuth import get_access_token
+
+from ygka.models import LanguageModel, RevChatGPTChatbotConfigModel, YGKAConfigModel
 
 
 class QueryClientFactory:
     '''Factory for creating query clients.'''
 
     def __init__(self, config_model: YGKAConfigModel):
         self.config_model = config_model
 
     def create(self):
         '''Create a query client.'''
         if self.config_model.language_model == LanguageModel.REVERSE_ENGINEERED_CHATGPT:
             from .reverse_engineered_chatgpt_client import ReverseEngineeredChatGPTClient
-            return ReverseEngineeredChatGPTClient(config=self.config_model.chatgpt_config)
+            browser_name: str = \
+                cast(str, self.config_model.browser_name)  # REVERSE_ENGINEERED_CHATGPT means browser_name is not None
+            access_token = get_access_token(browser_name)
+            rev_chatgpt_config_model = RevChatGPTChatbotConfigModel(access_token=access_token)
+            return ReverseEngineeredChatGPTClient(config=rev_chatgpt_config_model)
         elif self.config_model.language_model == LanguageModel.OFFICIAL_CHATGPT:
             from .official_chatgpt_client import OfficialChatGPTClient
             return OfficialChatGPTClient(openai_api_key=self.config_model.openai_api_key)
         else:
             raise ValueError('Invalid language model.')
```

### Comparing `ygka-2023.4.11/ygka/query_clients/reverse_engineered_chatgpt_client.py` & `ygka-2023.4.16/ygka/query_clients/reverse_engineered_chatgpt_client.py`

 * *Files identical despite different names*

### Comparing `ygka-2023.4.11/ygka/utils/ygka_config_manager.py` & `ygka-2023.4.16/ygka/utils/ygka_config_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 from typing import Optional
 
 from ygka.models import YGKAConfigModel
 
 
 class YGKAConfigManager:
-    DEFAULT_CONFIG_PATH = os.path.expanduser('~/.ygka_config.json')
+    DEFAULT_CONFIG_PATH = os.path.expanduser('~/.ygka_openai_config.json')
 
     def __init__(
         self,
         config_model: Optional[YGKAConfigModel] = None,
         config_path: Optional[str] = None,
         load_config: bool = False,
     ):
@@ -18,15 +18,15 @@
         Initialize an instance of YGKAConfigManager
 
         Args:
             config_model: \
                     An instance of YGKAConfigManager to use as the configuration.\
                     If None and load_config is True, loads the configuration from the configuration file.
             config_path: Path to the configuration file. \
-                If None, uses the default path "~/.ygka_config.json".
+                If None, uses the default path "~/.ygka_openai_config.json".
             load_config: If True and config_model is None, loads the configuration from the configuration file.
         '''
         self.config_path = config_path or YGKAConfigManager.DEFAULT_CONFIG_PATH
 
         if config_model:
             self.update_config(config_model)
         elif load_config:
```

### Comparing `ygka-2023.4.11/PKG-INFO` & `ygka-2023.4.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: ygka
-Version: 2023.4.11
+Version: 2023.4.16
 Summary: 
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: poetry (>=1.4.0,<2.0.0)
-Requires-Dist: pydantic (>=1.10.5,<2.0.0)
-Requires-Dist: revchatgpt (>=4.1.6,<5.0.0)
+Requires-Dist: pydantic (>=1.10.7,<2.0.0)
+Requires-Dist: revchatgpt (>=4.2.2,<5.0.0)
+Requires-Dist: revchatgptauth (>=2023.4.16,<2024.0.0)
 Requires-Dist: rich (<13.0.0)
 Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
-Requires-Dist: yt-dlp (>=2023.3.4,<2024.0.0)
 Description-Content-Type: text/markdown
 
 # YGKA 🤖
 
 [![codecov](https://codecov.io/gh/code-yeongyu/YGK-a/branch/master/graph/badge.svg?token=GB79Y7PEHU)](https://codecov.io/gh/code-yeongyu/YGK-a)
 [![Release Package to PyPI](https://github.com/code-yeongyu/YGK-a/actions/workflows/release.yml/badge.svg)](https://github.com/code-yeongyu/YGK-a/actions/workflows/release.yml)
 [![PyPI version](https://badge.fury.io/py/ygka.svg)](https://badge.fury.io/py/ygka)
```

