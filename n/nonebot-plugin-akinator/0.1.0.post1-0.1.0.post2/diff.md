# Comparing `tmp/nonebot-plugin-akinator-0.1.0.post1.tar.gz` & `tmp/nonebot-plugin-akinator-0.1.0.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-akinator-0.1.0.post1.tar", last modified: Fri Apr 14 22:53:16 2023, max compression
+gzip compressed data, was "nonebot-plugin-akinator-0.1.0.post2.tar", last modified: Fri Apr 14 22:57:48 2023, max compression
```

## Comparing `nonebot-plugin-akinator-0.1.0.post1.tar` & `nonebot-plugin-akinator-0.1.0.post2.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0     1069 2023-04-14 22:53:05.896664 nonebot-plugin-akinator-0.1.0.post1/LICENSE
--rw-r--r--   0        0        0     4133 2023-04-14 22:53:05.896664 nonebot-plugin-akinator-0.1.0.post1/README.md
--rw-r--r--   0        0        0      292 2023-04-14 22:53:05.896664 nonebot-plugin-akinator-0.1.0.post1/nonebot_plugin_akinator/__init__.py
--rw-r--r--   0        0        0     4396 2023-04-14 22:53:05.896664 nonebot-plugin-akinator-0.1.0.post1/nonebot_plugin_akinator/__main__.py
--rw-r--r--   0        0        0       39 2023-04-14 22:53:06.584681 nonebot-plugin-akinator-0.1.0.post1/nonebot_plugin_akinator/akinator/.git
--rw-r--r--   0        0        0     1873 2023-04-14 22:53:06.592681 nonebot-plugin-akinator-0.1.0.post1/nonebot_plugin_akinator/akinator/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0        0        0      200 2023-04-14 22:53:06.592681 nonebot-plugin-akinator-0.1.0.post1/nonebot_plugin_akinator/akinator/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0     1103 2023-04-14 22:53:06.592681 nonebot-plugin-akinator-0.1.0.post1/nonebot_plugin_akinator/akinator/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0        0        0      749 2023-04-14 22:53:06.592681 nonebot-plugin-akinator-0.1.0.post1/nonebot_plugin_akinator/akinator/.github/workflows/codeql.yml
--rw-r--r--   0        0        0     1128 2023-04-14 22:53:06.592681 nonebot-plugin-akinator-0.1.0.post1/nonebot_plugin_akinator/akinator/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     1799 2023-04-14 22:53:06.592681 nonebot-plugin-akinator-0.1.0.post1/nonebot_plugin_akinator/akinator/.gitignore
--rw-r--r--   0        0        0      173 2023-04-14 22:53:06.592681 nonebot-plugin-akinator-0.1.0.post1/nonebot_plugin_akinator/akinator/.readthedocs.yml
--rw-r--r--   0        0        0     5328 2023-04-14 22:53:06.592681 nonebot-plugin-akinator-0.1.0.post1/nonebot_plugin_akinator/akinator/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1082 2023-04-14 22:53:06.592681 nonebot-plugin-akinator-0.1.0.post1/nonebot_plugin_akinator/akinator/LICENSE
--rw-r--r--   0        0        0       34 2023-04-14 22:53:06.592681 nonebot-plugin-akinator-0.1.0.post1/nonebot_plugin_akinator/akinator/MANIFEST.in
--rw-r--r--   0        0        0     1994 2023-04-14 22:53:06.592681 nonebot-plugin-akinator-0.1.0.post1/nonebot_plugin_akinator/akinator/README.rst
--rw-r--r--   0        0        0      380 2023-04-14 22:53:06.592681 nonebot-plugin-akinator-0.1.0.post1/nonebot_plugin_akinator/akinator/akinator/__init__.py
--rw-r--r--   0        0        0    12713 2023-04-14 22:53:06.592681 nonebot-plugin-akinator-0.1.0.post1/nonebot_plugin_akinator/akinator/akinator/akinator.py
--rw-r--r--   0        0        0      356 2023-04-14 22:53:06.592681 nonebot-plugin-akinator-0.1.0.post1/nonebot_plugin_akinator/akinator/akinator/async_aki/__init__.py
--rw-r--r--   0        0        0    14044 2023-04-14 22:53:06.592681 nonebot-plugin-akinator-0.1.0.post1/nonebot_plugin_akinator/akinator/akinator/async_aki/async_akinator.py
--rw-r--r--   0        0        0     2510 2023-04-14 22:53:06.592681 nonebot-plugin-akinator-0.1.0.post1/nonebot_plugin_akinator/akinator/akinator/exceptions.py
--rw-r--r--   0        0        0     5559 2023-04-14 22:53:06.592681 nonebot-plugin-akinator-0.1.0.post1/nonebot_plugin_akinator/akinator/akinator/utils.py
--rw-r--r--   0        0        0      319 2023-04-14 22:53:06.592681 nonebot-plugin-akinator-0.1.0.post1/nonebot_plugin_akinator/akinator/docs/conf.py
--rw-r--r--   0        0        0    11653 2023-04-14 22:53:06.592681 nonebot-plugin-akinator-0.1.0.post1/nonebot_plugin_akinator/akinator/docs/index.rst
--rw-r--r--   0        0        0        6 2023-04-14 22:53:06.592681 nonebot-plugin-akinator-0.1.0.post1/nonebot_plugin_akinator/akinator/docs/requirements.txt
--rw-r--r--   0        0        0      612 2023-04-14 22:53:06.592681 nonebot-plugin-akinator-0.1.0.post1/nonebot_plugin_akinator/akinator/examples/aki.py
--rw-r--r--   0        0        0      887 2023-04-14 22:53:06.592681 nonebot-plugin-akinator-0.1.0.post1/nonebot_plugin_akinator/akinator/examples/async_aki.py
--rw-r--r--   0        0        0      681 2023-04-14 22:53:06.592681 nonebot-plugin-akinator-0.1.0.post1/nonebot_plugin_akinator/akinator/pyproject.toml
--rw-r--r--   0        0        0       18 2023-04-14 22:53:06.592681 nonebot-plugin-akinator-0.1.0.post1/nonebot_plugin_akinator/akinator/requirements.txt
--rw-r--r--   0        0        0     1496 2023-04-14 22:53:06.592681 nonebot-plugin-akinator-0.1.0.post1/nonebot_plugin_akinator/akinator/setup.py
--rw-r--r--   0        0        0      302 2023-04-14 22:53:05.896664 nonebot-plugin-akinator-0.1.0.post1/nonebot_plugin_akinator/config.py
--rw-r--r--   0        0        0    10648 2023-04-14 22:53:05.896664 nonebot-plugin-akinator-0.1.0.post1/nonebot_plugin_akinator/game.py
--rw-r--r--   0        0        0    11528 2023-04-14 22:53:05.896664 nonebot-plugin-akinator-0.1.0.post1/nonebot_plugin_akinator/res/bg.jpg
--rw-r--r--   0        0        0    43524 2023-04-14 22:53:05.896664 nonebot-plugin-akinator-0.1.0.post1/nonebot_plugin_akinator/res/concentration_intense.webp
--rw-r--r--   0        0        0    46462 2023-04-14 22:53:05.896664 nonebot-plugin-akinator-0.1.0.post1/nonebot_plugin_akinator/res/confiant.webp
--rw-r--r--   0        0        0    45550 2023-04-14 22:53:05.896664 nonebot-plugin-akinator-0.1.0.post1/nonebot_plugin_akinator/res/etonnement.webp
--rw-r--r--   0        0        0    49318 2023-04-14 22:53:05.900664 nonebot-plugin-akinator-0.1.0.post1/nonebot_plugin_akinator/res/inspiration_forte.webp
--rw-r--r--   0        0        0    45300 2023-04-14 22:53:05.900664 nonebot-plugin-akinator-0.1.0.post1/nonebot_plugin_akinator/res/inspiration_legere.webp
--rw-r--r--   0        0        0    50740 2023-04-14 22:53:05.900664 nonebot-plugin-akinator-0.1.0.post1/nonebot_plugin_akinator/res/leger_decouragement.webp
--rw-r--r--   0        0        0    40432 2023-04-14 22:53:05.900664 nonebot-plugin-akinator-0.1.0.post1/nonebot_plugin_akinator/res/mobile.webp
--rw-r--r--   0        0        0    36506 2023-04-14 22:53:05.900664 nonebot-plugin-akinator-0.1.0.post1/nonebot_plugin_akinator/res/serein.webp
--rw-r--r--   0        0        0    45464 2023-04-14 22:53:05.900664 nonebot-plugin-akinator-0.1.0.post1/nonebot_plugin_akinator/res/surprise.webp
--rw-r--r--   0        0        0    42668 2023-04-14 22:53:05.900664 nonebot-plugin-akinator-0.1.0.post1/nonebot_plugin_akinator/res/tension.webp
--rw-r--r--   0        0        0    54230 2023-04-14 22:53:05.900664 nonebot-plugin-akinator-0.1.0.post1/nonebot_plugin_akinator/res/vrai_decouragement.webp
--rw-r--r--   0        0        0     1410 2023-04-14 22:53:05.904664 nonebot-plugin-akinator-0.1.0.post1/pyproject.toml
--rw-r--r--   0        0        0     4483 1970-01-01 00:00:00.000000 nonebot-plugin-akinator-0.1.0.post1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-14 22:57:39.672828 nonebot-plugin-akinator-0.1.0.post2/LICENSE
+-rw-r--r--   0        0        0     4133 2023-04-14 22:57:39.672828 nonebot-plugin-akinator-0.1.0.post2/README.md
+-rw-r--r--   0        0        0      337 2023-04-14 22:57:39.672828 nonebot-plugin-akinator-0.1.0.post2/nonebot_plugin_akinator/__init__.py
+-rw-r--r--   0        0        0     4396 2023-04-14 22:57:39.672828 nonebot-plugin-akinator-0.1.0.post2/nonebot_plugin_akinator/__main__.py
+-rw-r--r--   0        0        0       39 2023-04-14 22:57:40.000833 nonebot-plugin-akinator-0.1.0.post2/nonebot_plugin_akinator/akinator/.git
+-rw-r--r--   0        0        0     1873 2023-04-14 22:57:40.008833 nonebot-plugin-akinator-0.1.0.post2/nonebot_plugin_akinator/akinator/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0        0        0      200 2023-04-14 22:57:40.008833 nonebot-plugin-akinator-0.1.0.post2/nonebot_plugin_akinator/akinator/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0     1103 2023-04-14 22:57:40.008833 nonebot-plugin-akinator-0.1.0.post2/nonebot_plugin_akinator/akinator/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0        0        0      749 2023-04-14 22:57:40.008833 nonebot-plugin-akinator-0.1.0.post2/nonebot_plugin_akinator/akinator/.github/workflows/codeql.yml
+-rw-r--r--   0        0        0     1128 2023-04-14 22:57:40.008833 nonebot-plugin-akinator-0.1.0.post2/nonebot_plugin_akinator/akinator/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     1799 2023-04-14 22:57:40.008833 nonebot-plugin-akinator-0.1.0.post2/nonebot_plugin_akinator/akinator/.gitignore
+-rw-r--r--   0        0        0      173 2023-04-14 22:57:40.008833 nonebot-plugin-akinator-0.1.0.post2/nonebot_plugin_akinator/akinator/.readthedocs.yml
+-rw-r--r--   0        0        0     5328 2023-04-14 22:57:40.008833 nonebot-plugin-akinator-0.1.0.post2/nonebot_plugin_akinator/akinator/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1082 2023-04-14 22:57:40.008833 nonebot-plugin-akinator-0.1.0.post2/nonebot_plugin_akinator/akinator/LICENSE
+-rw-r--r--   0        0        0       34 2023-04-14 22:57:40.008833 nonebot-plugin-akinator-0.1.0.post2/nonebot_plugin_akinator/akinator/MANIFEST.in
+-rw-r--r--   0        0        0     1994 2023-04-14 22:57:40.008833 nonebot-plugin-akinator-0.1.0.post2/nonebot_plugin_akinator/akinator/README.rst
+-rw-r--r--   0        0        0      380 2023-04-14 22:57:40.008833 nonebot-plugin-akinator-0.1.0.post2/nonebot_plugin_akinator/akinator/akinator/__init__.py
+-rw-r--r--   0        0        0    12713 2023-04-14 22:57:40.008833 nonebot-plugin-akinator-0.1.0.post2/nonebot_plugin_akinator/akinator/akinator/akinator.py
+-rw-r--r--   0        0        0      356 2023-04-14 22:57:40.008833 nonebot-plugin-akinator-0.1.0.post2/nonebot_plugin_akinator/akinator/akinator/async_aki/__init__.py
+-rw-r--r--   0        0        0    14044 2023-04-14 22:57:40.008833 nonebot-plugin-akinator-0.1.0.post2/nonebot_plugin_akinator/akinator/akinator/async_aki/async_akinator.py
+-rw-r--r--   0        0        0     2510 2023-04-14 22:57:40.008833 nonebot-plugin-akinator-0.1.0.post2/nonebot_plugin_akinator/akinator/akinator/exceptions.py
+-rw-r--r--   0        0        0     5559 2023-04-14 22:57:40.008833 nonebot-plugin-akinator-0.1.0.post2/nonebot_plugin_akinator/akinator/akinator/utils.py
+-rw-r--r--   0        0        0      319 2023-04-14 22:57:40.008833 nonebot-plugin-akinator-0.1.0.post2/nonebot_plugin_akinator/akinator/docs/conf.py
+-rw-r--r--   0        0        0    11653 2023-04-14 22:57:40.008833 nonebot-plugin-akinator-0.1.0.post2/nonebot_plugin_akinator/akinator/docs/index.rst
+-rw-r--r--   0        0        0        6 2023-04-14 22:57:40.008833 nonebot-plugin-akinator-0.1.0.post2/nonebot_plugin_akinator/akinator/docs/requirements.txt
+-rw-r--r--   0        0        0      612 2023-04-14 22:57:40.008833 nonebot-plugin-akinator-0.1.0.post2/nonebot_plugin_akinator/akinator/examples/aki.py
+-rw-r--r--   0        0        0      887 2023-04-14 22:57:40.008833 nonebot-plugin-akinator-0.1.0.post2/nonebot_plugin_akinator/akinator/examples/async_aki.py
+-rw-r--r--   0        0        0      681 2023-04-14 22:57:40.008833 nonebot-plugin-akinator-0.1.0.post2/nonebot_plugin_akinator/akinator/pyproject.toml
+-rw-r--r--   0        0        0       18 2023-04-14 22:57:40.008833 nonebot-plugin-akinator-0.1.0.post2/nonebot_plugin_akinator/akinator/requirements.txt
+-rw-r--r--   0        0        0     1496 2023-04-14 22:57:40.008833 nonebot-plugin-akinator-0.1.0.post2/nonebot_plugin_akinator/akinator/setup.py
+-rw-r--r--   0        0        0      302 2023-04-14 22:57:39.676828 nonebot-plugin-akinator-0.1.0.post2/nonebot_plugin_akinator/config.py
+-rw-r--r--   0        0        0    10648 2023-04-14 22:57:39.676828 nonebot-plugin-akinator-0.1.0.post2/nonebot_plugin_akinator/game.py
+-rw-r--r--   0        0        0    11528 2023-04-14 22:57:39.676828 nonebot-plugin-akinator-0.1.0.post2/nonebot_plugin_akinator/res/bg.jpg
+-rw-r--r--   0        0        0    43524 2023-04-14 22:57:39.676828 nonebot-plugin-akinator-0.1.0.post2/nonebot_plugin_akinator/res/concentration_intense.webp
+-rw-r--r--   0        0        0    46462 2023-04-14 22:57:39.676828 nonebot-plugin-akinator-0.1.0.post2/nonebot_plugin_akinator/res/confiant.webp
+-rw-r--r--   0        0        0    45550 2023-04-14 22:57:39.676828 nonebot-plugin-akinator-0.1.0.post2/nonebot_plugin_akinator/res/etonnement.webp
+-rw-r--r--   0        0        0    49318 2023-04-14 22:57:39.676828 nonebot-plugin-akinator-0.1.0.post2/nonebot_plugin_akinator/res/inspiration_forte.webp
+-rw-r--r--   0        0        0    45300 2023-04-14 22:57:39.676828 nonebot-plugin-akinator-0.1.0.post2/nonebot_plugin_akinator/res/inspiration_legere.webp
+-rw-r--r--   0        0        0    50740 2023-04-14 22:57:39.676828 nonebot-plugin-akinator-0.1.0.post2/nonebot_plugin_akinator/res/leger_decouragement.webp
+-rw-r--r--   0        0        0    40432 2023-04-14 22:57:39.676828 nonebot-plugin-akinator-0.1.0.post2/nonebot_plugin_akinator/res/mobile.webp
+-rw-r--r--   0        0        0    36506 2023-04-14 22:57:39.676828 nonebot-plugin-akinator-0.1.0.post2/nonebot_plugin_akinator/res/serein.webp
+-rw-r--r--   0        0        0    45464 2023-04-14 22:57:39.676828 nonebot-plugin-akinator-0.1.0.post2/nonebot_plugin_akinator/res/surprise.webp
+-rw-r--r--   0        0        0    42668 2023-04-14 22:57:39.676828 nonebot-plugin-akinator-0.1.0.post2/nonebot_plugin_akinator/res/tension.webp
+-rw-r--r--   0        0        0    54230 2023-04-14 22:57:39.676828 nonebot-plugin-akinator-0.1.0.post2/nonebot_plugin_akinator/res/vrai_decouragement.webp
+-rw-r--r--   0        0        0     1410 2023-04-14 22:57:39.680828 nonebot-plugin-akinator-0.1.0.post2/pyproject.toml
+-rw-r--r--   0        0        0     4483 1970-01-01 00:00:00.000000 nonebot-plugin-akinator-0.1.0.post2/PKG-INFO
```

### Comparing `nonebot-plugin-akinator-0.1.0.post1/LICENSE` & `nonebot-plugin-akinator-0.1.0.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-akinator-0.1.0.post1/README.md` & `nonebot-plugin-akinator-0.1.0.post2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -100,15 +100,15 @@
 ## ⚙️ 配置
 
 在 nonebot2 项目的`.env`文件中添加下表中的必填配置
 
 |        配置项         | 必填 | 默认值  |                          说明                          |
 | :-------------------: | :--: | :-----: | :----------------------------------------------------: |
 |        `PROXY`        |  否  |   无    |                访问 Akinator 使用的代理                |
-| `AKINATOR_CHILD_MODE` |  否  | `False` | 是否启用 Akinator 的儿童模式（结果不会出现 NSFW 角色） |
+| `AKINATOR_CHILD_MODE` |  否  | `False` | 是否启用 Akinator 的儿童模式（结果不会出现 NSFW 人物） |
 |  `AKINATOR_LANGUAGE`  |  否  |  `cn`   |                    Akinator 的语言                     |
 
 ## 🎉 使用
 
 发送指令 `akinator` / `aki` 即可开始游戏
 
 开始游戏后，直接发送你的答案即可（序号和文字均可）
```

#### html2text {}

```diff
@@ -14,15 +14,15 @@
 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åç
 `plugins` é¡¹éè¿½å åå¥ ```toml [tool.nonebot] plugins = [ # ...
 "nonebot_plugin_akinator" ] ```  ## âï¸ éç½® å¨ nonebot2
 é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½® | éç½®é¡¹ | å¿å¡« |
 é»è®¤å¼ | è¯´æ | | :-------------------: | :--: | :-----: | :--------------
 --------------------------------------: | | `PROXY` | å¦ | æ  | è®¿é®
 Akinator ä½¿ç¨çä»£ç | | `AKINATOR_CHILD_MODE` | å¦ | `False` |
-æ¯å¦å¯ç¨ Akinator çå¿ç«¥æ¨¡å¼ï¼ç»æä¸ä¼åºç° NSFW è§è²ï¼ | |
+æ¯å¦å¯ç¨ Akinator çå¿ç«¥æ¨¡å¼ï¼ç»æä¸ä¼åºç° NSFW äººç©ï¼ | |
 `AKINATOR_LANGUAGE` | å¦ | `cn` | Akinator çè¯­è¨ | ## ð ä½¿ç¨
 åéæä»¤ `akinator` / `aki` å³å¯å¼å§æ¸¸æ
 å¼å§æ¸¸æåï¼ç´æ¥åéä½ çç­æ¡å³å¯ï¼åºå·åæå­åå¯ï¼ ###
 ææå¾  ç¹å»å±å¼ ![Alt text](readme/
 QQ%E5%9B%BE%E7%89%8720230415063509.png) ![Alt text](readme/
 QQ%E5%9B%BE%E7%89%8720230415063607.png)  ## ð èç³» QQï¼3076823485
 Telegramï¼[@lgc2333](https://t.me/lgc2333) å¹æ°´ç¾¤ï¼[1105946125](https://
```

### Comparing `nonebot-plugin-akinator-0.1.0.post1/nonebot_plugin_akinator/__main__.py` & `nonebot-plugin-akinator-0.1.0.post2/nonebot_plugin_akinator/__main__.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-akinator-0.1.0.post1/nonebot_plugin_akinator/akinator/.github/ISSUE_TEMPLATE/bug_report.yml` & `nonebot-plugin-akinator-0.1.0.post2/nonebot_plugin_akinator/akinator/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-akinator-0.1.0.post1/nonebot_plugin_akinator/akinator/.github/ISSUE_TEMPLATE/feature_request.yml` & `nonebot-plugin-akinator-0.1.0.post2/nonebot_plugin_akinator/akinator/.github/ISSUE_TEMPLATE/feature_request.yml`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-akinator-0.1.0.post1/nonebot_plugin_akinator/akinator/.github/workflows/codeql.yml` & `nonebot-plugin-akinator-0.1.0.post2/nonebot_plugin_akinator/akinator/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-akinator-0.1.0.post1/nonebot_plugin_akinator/akinator/.github/workflows/python-publish.yml` & `nonebot-plugin-akinator-0.1.0.post2/nonebot_plugin_akinator/akinator/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-akinator-0.1.0.post1/nonebot_plugin_akinator/akinator/.gitignore` & `nonebot-plugin-akinator-0.1.0.post2/nonebot_plugin_akinator/akinator/.gitignore`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-akinator-0.1.0.post1/nonebot_plugin_akinator/akinator/CODE_OF_CONDUCT.md` & `nonebot-plugin-akinator-0.1.0.post2/nonebot_plugin_akinator/akinator/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-akinator-0.1.0.post1/nonebot_plugin_akinator/akinator/LICENSE` & `nonebot-plugin-akinator-0.1.0.post2/nonebot_plugin_akinator/akinator/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-akinator-0.1.0.post1/nonebot_plugin_akinator/akinator/README.rst` & `nonebot-plugin-akinator-0.1.0.post2/nonebot_plugin_akinator/akinator/README.rst`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-akinator-0.1.0.post1/nonebot_plugin_akinator/akinator/akinator/akinator.py` & `nonebot-plugin-akinator-0.1.0.post2/nonebot_plugin_akinator/akinator/akinator/akinator.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-akinator-0.1.0.post1/nonebot_plugin_akinator/akinator/akinator/async_aki/async_akinator.py` & `nonebot-plugin-akinator-0.1.0.post2/nonebot_plugin_akinator/akinator/akinator/async_aki/async_akinator.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-akinator-0.1.0.post1/nonebot_plugin_akinator/akinator/akinator/exceptions.py` & `nonebot-plugin-akinator-0.1.0.post2/nonebot_plugin_akinator/akinator/akinator/exceptions.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-akinator-0.1.0.post1/nonebot_plugin_akinator/akinator/akinator/utils.py` & `nonebot-plugin-akinator-0.1.0.post2/nonebot_plugin_akinator/akinator/akinator/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-akinator-0.1.0.post1/nonebot_plugin_akinator/akinator/docs/index.rst` & `nonebot-plugin-akinator-0.1.0.post2/nonebot_plugin_akinator/akinator/docs/index.rst`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-akinator-0.1.0.post1/nonebot_plugin_akinator/akinator/examples/aki.py` & `nonebot-plugin-akinator-0.1.0.post2/nonebot_plugin_akinator/akinator/examples/aki.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-akinator-0.1.0.post1/nonebot_plugin_akinator/akinator/examples/async_aki.py` & `nonebot-plugin-akinator-0.1.0.post2/nonebot_plugin_akinator/akinator/examples/async_aki.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-akinator-0.1.0.post1/nonebot_plugin_akinator/akinator/pyproject.toml` & `nonebot-plugin-akinator-0.1.0.post2/nonebot_plugin_akinator/akinator/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-akinator-0.1.0.post1/nonebot_plugin_akinator/akinator/setup.py` & `nonebot-plugin-akinator-0.1.0.post2/nonebot_plugin_akinator/akinator/setup.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-akinator-0.1.0.post1/nonebot_plugin_akinator/game.py` & `nonebot-plugin-akinator-0.1.0.post2/nonebot_plugin_akinator/game.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-akinator-0.1.0.post1/nonebot_plugin_akinator/res/bg.jpg` & `nonebot-plugin-akinator-0.1.0.post2/nonebot_plugin_akinator/res/bg.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-akinator-0.1.0.post1/nonebot_plugin_akinator/res/concentration_intense.webp` & `nonebot-plugin-akinator-0.1.0.post2/nonebot_plugin_akinator/res/concentration_intense.webp`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-akinator-0.1.0.post1/nonebot_plugin_akinator/res/confiant.webp` & `nonebot-plugin-akinator-0.1.0.post2/nonebot_plugin_akinator/res/confiant.webp`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-akinator-0.1.0.post1/nonebot_plugin_akinator/res/etonnement.webp` & `nonebot-plugin-akinator-0.1.0.post2/nonebot_plugin_akinator/res/etonnement.webp`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-akinator-0.1.0.post1/nonebot_plugin_akinator/res/inspiration_forte.webp` & `nonebot-plugin-akinator-0.1.0.post2/nonebot_plugin_akinator/res/inspiration_forte.webp`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-akinator-0.1.0.post1/nonebot_plugin_akinator/res/inspiration_legere.webp` & `nonebot-plugin-akinator-0.1.0.post2/nonebot_plugin_akinator/res/inspiration_legere.webp`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-akinator-0.1.0.post1/nonebot_plugin_akinator/res/leger_decouragement.webp` & `nonebot-plugin-akinator-0.1.0.post2/nonebot_plugin_akinator/res/leger_decouragement.webp`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-akinator-0.1.0.post1/nonebot_plugin_akinator/res/mobile.webp` & `nonebot-plugin-akinator-0.1.0.post2/nonebot_plugin_akinator/res/mobile.webp`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-akinator-0.1.0.post1/nonebot_plugin_akinator/res/serein.webp` & `nonebot-plugin-akinator-0.1.0.post2/nonebot_plugin_akinator/res/serein.webp`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-akinator-0.1.0.post1/nonebot_plugin_akinator/res/surprise.webp` & `nonebot-plugin-akinator-0.1.0.post2/nonebot_plugin_akinator/res/surprise.webp`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-akinator-0.1.0.post1/nonebot_plugin_akinator/res/tension.webp` & `nonebot-plugin-akinator-0.1.0.post2/nonebot_plugin_akinator/res/tension.webp`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-akinator-0.1.0.post1/nonebot_plugin_akinator/res/vrai_decouragement.webp` & `nonebot-plugin-akinator-0.1.0.post2/nonebot_plugin_akinator/res/vrai_decouragement.webp`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-akinator-0.1.0.post1/pyproject.toml` & `nonebot-plugin-akinator-0.1.0.post2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-akinator"
-version = "0.1.0.post1"
+version = "0.1.0.post2"
 description = "Template plugin project"
 authors = [
     { name = "student_2333", email = "lgc2333@126.com" },
 ]
 dependencies = [
     "nonebot2>=2.0.0-rc.1",
     "nonebot-adapter-onebot>=2.2.0",
```

### Comparing `nonebot-plugin-akinator-0.1.0.post1/PKG-INFO` & `nonebot-plugin-akinator-0.1.0.post2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-akinator
-Version: 0.1.0.post1
+Version: 0.1.0.post2
 Summary: Template plugin project
 License: MIT
 Author-email: student_2333 <lgc2333@126.com>
 Requires-Python: >=3.8,<4.0
 Provides-Extra: dev
 Provides-Extra: extra
 Project-URL: homepage, https://github.com/lgc2333/nonebot-plugin-akinator
@@ -112,15 +112,15 @@
 ## ⚙️ 配置
 
 在 nonebot2 项目的`.env`文件中添加下表中的必填配置
 
 |        配置项         | 必填 | 默认值  |                          说明                          |
 | :-------------------: | :--: | :-----: | :----------------------------------------------------: |
 |        `PROXY`        |  否  |   无    |                访问 Akinator 使用的代理                |
-| `AKINATOR_CHILD_MODE` |  否  | `False` | 是否启用 Akinator 的儿童模式（结果不会出现 NSFW 角色） |
+| `AKINATOR_CHILD_MODE` |  否  | `False` | 是否启用 Akinator 的儿童模式（结果不会出现 NSFW 人物） |
 |  `AKINATOR_LANGUAGE`  |  否  |  `cn`   |                    Akinator 的语言                     |
 
 ## 🎉 使用
 
 发送指令 `akinator` / `aki` 即可开始游戏
 
 开始游戏后，直接发送你的答案即可（序号和文字均可）
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-akinator Version: 0.1.0.post1
+Metadata-Version: 2.1 Name: nonebot-plugin-akinator Version: 0.1.0.post2
 Summary: Template plugin project License: MIT Author-email: student_2333
 126.com> Requires-Python: >=3.8,<4.0 Provides-Extra: dev Provides-Extra: extra
 Project-URL: homepage, https://github.com/lgc2333/nonebot-plugin-akinator
 Description-Content-Type: text/markdown
                               [NoneBotPluginLogo]
                               [NoneBotPluginText]
   # NoneBot-Plugin-Akinator _â¨ ç½ç»å¤©æ â¨_ [license] [pypi] [python]
@@ -19,15 +19,15 @@
 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åç
 `plugins` é¡¹éè¿½å åå¥ ```toml [tool.nonebot] plugins = [ # ...
 "nonebot_plugin_akinator" ] ```  ## âï¸ éç½® å¨ nonebot2
 é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½® | éç½®é¡¹ | å¿å¡« |
 é»è®¤å¼ | è¯´æ | | :-------------------: | :--: | :-----: | :--------------
 --------------------------------------: | | `PROXY` | å¦ | æ  | è®¿é®
 Akinator ä½¿ç¨çä»£ç | | `AKINATOR_CHILD_MODE` | å¦ | `False` |
-æ¯å¦å¯ç¨ Akinator çå¿ç«¥æ¨¡å¼ï¼ç»æä¸ä¼åºç° NSFW è§è²ï¼ | |
+æ¯å¦å¯ç¨ Akinator çå¿ç«¥æ¨¡å¼ï¼ç»æä¸ä¼åºç° NSFW äººç©ï¼ | |
 `AKINATOR_LANGUAGE` | å¦ | `cn` | Akinator çè¯­è¨ | ## ð ä½¿ç¨
 åéæä»¤ `akinator` / `aki` å³å¯å¼å§æ¸¸æ
 å¼å§æ¸¸æåï¼ç´æ¥åéä½ çç­æ¡å³å¯ï¼åºå·åæå­åå¯ï¼ ###
 ææå¾  ç¹å»å±å¼ ![Alt text](readme/
 QQ%E5%9B%BE%E7%89%8720230415063509.png) ![Alt text](readme/
 QQ%E5%9B%BE%E7%89%8720230415063607.png)  ## ð èç³» QQï¼3076823485
 Telegramï¼[@lgc2333](https://t.me/lgc2333) å¹æ°´ç¾¤ï¼[1105946125](https://
```

