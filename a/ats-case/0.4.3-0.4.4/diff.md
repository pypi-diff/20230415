# Comparing `tmp/ats_case-0.4.3.tar.gz` & `tmp/ats_case-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ats_case-0.4.3.tar", last modified: Thu Apr 13 02:22:15 2023, max compression
+gzip compressed data, was "ats_case-0.4.4.tar", last modified: Sat Apr 15 06:07:03 2023, max compression
```

## Comparing `ats_case-0.4.3.tar` & `ats_case-0.4.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 02:22:15.707571 ats_case-0.4.3/
--rw-rw-rw-   0        0        0      116 2022-09-15 08:18:29.000000 ats_case-0.4.3/LICENSE
--rw-rw-rw-   0        0        0        0 2023-03-03 08:23:26.000000 ats_case-0.4.3/MANIFEST.in
--rw-rw-rw-   0        0        0     1042 2023-04-13 02:22:15.704976 ats_case-0.4.3/PKG-INFO
--rw-rw-rw-   0        0        0      532 2022-06-13 07:56:24.000000 ats_case-0.4.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 02:22:15.293085 ats_case-0.4.3/ats_case/
--rw-rw-rw-   0        0        0        0 2023-01-04 02:21:31.000000 ats_case-0.4.3/ats_case/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 02:22:15.508533 ats_case-0.4.3/ats_case/case/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:13:48.000000 ats_case-0.4.3/ats_case/case/__init__.py
--rw-rw-rw-   0        0        0    16964 2023-04-13 02:21:54.000000 ats_case-0.4.3/ats_case/case/command.py
--rw-rw-rw-   0        0        0    10103 2023-04-07 01:41:51.000000 ats_case-0.4.3/ats_case/case/context.py
--rw-rw-rw-   0        0        0     5143 2023-04-12 01:07:14.000000 ats_case-0.4.3/ats_case/case/executor.py
--rw-rw-rw-   0        0        0     5437 2023-04-12 01:16:48.000000 ats_case-0.4.3/ats_case/case/translator.py
-drwxrwxrwx   0        0        0        0 2023-04-13 02:22:15.573135 ats_case-0.4.3/ats_case/common/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:22:45.000000 ats_case-0.4.3/ats_case/common/__init__.py
--rw-rw-rw-   0        0        0      381 2023-04-10 07:20:19.000000 ats_case-0.4.3/ats_case/common/enum.py
--rw-rw-rw-   0        0        0      628 2023-04-11 03:13:44.000000 ats_case-0.4.3/ats_case/common/error.py
-drwxrwxrwx   0        0        0        0 2023-04-13 02:22:15.637332 ats_case-0.4.3/ats_case/manage/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.4.3/ats_case/manage/__init__.py
--rw-rw-rw-   0        0        0     1434 2023-03-03 01:15:16.000000 ats_case-0.4.3/ats_case/manage/core.py
--rw-rw-rw-   0        0        0     2586 2023-04-12 01:16:48.000000 ats_case-0.4.3/ats_case/manage/start.py
-drwxrwxrwx   0        0        0        0 2023-04-13 02:22:15.693851 ats_case-0.4.3/ats_case/template/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.4.3/ats_case/template/__init__.py
--rw-rw-rw-   0        0        0     2089 2023-04-12 01:03:34.000000 ats_case-0.4.3/ats_case/template/testcase_v1.tmp
-drwxrwxrwx   0        0        0        0 2023-04-13 02:22:15.393919 ats_case-0.4.3/ats_case.egg-info/
--rw-rw-rw-   0        0        0     1042 2023-04-13 02:22:14.000000 ats_case-0.4.3/ats_case.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      566 2023-04-13 02:22:14.000000 ats_case-0.4.3/ats_case.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 02:22:14.000000 ats_case-0.4.3/ats_case.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-04-13 02:22:14.000000 ats_case-0.4.3/ats_case.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-13 02:22:14.000000 ats_case-0.4.3/ats_case.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-13 02:22:15.707571 ats_case-0.4.3/setup.cfg
--rw-rw-rw-   0        0        0      935 2023-04-13 02:21:54.000000 ats_case-0.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 06:07:03.789340 ats_case-0.4.4/
+-rw-rw-rw-   0        0        0      116 2022-09-15 08:18:29.000000 ats_case-0.4.4/LICENSE
+-rw-rw-rw-   0        0        0        0 2023-03-03 08:23:26.000000 ats_case-0.4.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     1042 2023-04-15 06:07:03.786341 ats_case-0.4.4/PKG-INFO
+-rw-rw-rw-   0        0        0      532 2022-06-13 07:56:24.000000 ats_case-0.4.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-15 06:07:03.415243 ats_case-0.4.4/ats_case/
+-rw-rw-rw-   0        0        0        0 2023-01-04 02:21:31.000000 ats_case-0.4.4/ats_case/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-15 06:07:03.618074 ats_case-0.4.4/ats_case/case/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:13:48.000000 ats_case-0.4.4/ats_case/case/__init__.py
+-rw-rw-rw-   0        0        0    17491 2023-04-15 06:06:14.000000 ats_case-0.4.4/ats_case/case/command.py
+-rw-rw-rw-   0        0        0    10103 2023-04-07 01:41:51.000000 ats_case-0.4.4/ats_case/case/context.py
+-rw-rw-rw-   0        0        0     5317 2023-04-15 05:22:12.000000 ats_case-0.4.4/ats_case/case/executor.py
+-rw-rw-rw-   0        0        0     5437 2023-04-12 01:16:48.000000 ats_case-0.4.4/ats_case/case/translator.py
+drwxrwxrwx   0        0        0        0 2023-04-15 06:07:03.682517 ats_case-0.4.4/ats_case/common/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:22:45.000000 ats_case-0.4.4/ats_case/common/__init__.py
+-rw-rw-rw-   0        0        0      381 2023-04-10 07:20:19.000000 ats_case-0.4.4/ats_case/common/enum.py
+-rw-rw-rw-   0        0        0      646 2023-04-15 05:21:08.000000 ats_case-0.4.4/ats_case/common/error.py
+drwxrwxrwx   0        0        0        0 2023-04-15 06:07:03.743947 ats_case-0.4.4/ats_case/manage/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.4.4/ats_case/manage/__init__.py
+-rw-rw-rw-   0        0        0     1434 2023-03-03 01:15:16.000000 ats_case-0.4.4/ats_case/manage/core.py
+-rw-rw-rw-   0        0        0     2586 2023-04-12 01:16:48.000000 ats_case-0.4.4/ats_case/manage/start.py
+drwxrwxrwx   0        0        0        0 2023-04-15 06:07:03.777185 ats_case-0.4.4/ats_case/template/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.4.4/ats_case/template/__init__.py
+-rw-rw-rw-   0        0        0     2089 2023-04-12 01:03:34.000000 ats_case-0.4.4/ats_case/template/testcase_v1.tmp
+drwxrwxrwx   0        0        0        0 2023-04-15 06:07:03.502130 ats_case-0.4.4/ats_case.egg-info/
+-rw-rw-rw-   0        0        0     1042 2023-04-15 06:07:02.000000 ats_case-0.4.4/ats_case.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      566 2023-04-15 06:07:03.000000 ats_case-0.4.4/ats_case.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 06:07:02.000000 ats_case-0.4.4/ats_case.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-04-15 06:07:02.000000 ats_case-0.4.4/ats_case.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-15 06:07:02.000000 ats_case-0.4.4/ats_case.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-15 06:07:03.789340 ats_case-0.4.4/setup.cfg
+-rw-rw-rw-   0        0        0      935 2023-04-15 06:06:40.000000 ats_case-0.4.4/setup.py
```

### Comparing `ats_case-0.4.3/PKG-INFO` & `ats_case-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ats_case
-Version: 0.4.3
+Version: 0.4.4
 Summary: Test Script Development Library
 Home-page: https://gitee.com/henry9000/ats_case
 Author: zhangyue
 Author-email: zhangyue@techen.cn
 Project-URL: Bug Tracker, https://gitee.com/henry9000/ats_case/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ats_case-0.4.3/README.md` & `ats_case-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `ats_case-0.4.3/ats_case/case/command.py` & `ats_case-0.4.4/ats_case/case/command.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from ats_base.common import func
 from ats_base.log.logger import logger
 from ats_base.service import app, pro, em, udm
 
 from ats_case.case.context import Context
 from ats_case.common.enum import ProClazz, OperationClazz
-from ats_case.common.error import APIError, ClientReturnError
+from ats_case.common.error import APIError, ClientReturnError, MeterOperationError
 
 """
     常用操作命令
 """
 
 
 def send(context: Context, todo: dict, types=2, retry_times: int = 3):
@@ -65,15 +65,15 @@
     time.sleep(seconds)
 
 
 def offbench(context: Context, disabled=1):
     """
     脱表台
     :param context:
-    :param disabled:     秒
+    :param disabled:     使能
     :return:
     """
     clazz = OperationClazz(context.case.steps[str(context.runtime.step)].get('type'))
 
     if disabled == 1:
         if clazz == OperationClazz.BENCH:
             return True
@@ -209,51 +209,65 @@
                                                                                       self._operation,
                                                                                       self._element))
         if type(self._parameter) is dict:
             self._parameter = _replace(context, self._parameter)
 
         parse = pro.encode(func.to_dict(protocol=self._protocol.name, comm_addr=self._comm_addr,
                                         operation=self._operation, element=self._element, parameter=self._parameter,
-                                        addition=self._addition, security=self._security, session_key=context.session.basename))
+                                        addition=self._addition, security=self._security,
+                                        session_key=context.session.basename))
         logger.info('~ @PRO-ENCODE<- protocol:{} frame:{}'.format(self._protocol, parse.get('frame')))
 
         self._frame = parse.get('frame')
         return self._frame
 
-    def decode(self, context: Context):
+    def decode(self, context: Context, index=0):
+        # 异常判断 - 客户端返回结果
         if self._frame is None or len(self._frame) <= 0:
             raise ClientReturnError(self._frame)
 
         logger.info('~ @PRO-DECODE-> protocol:{} frame:{}'.format(self._protocol, self._frame))
-        data = pro.decode(func.to_dict(protocol=self._protocol.name, frame=self._frame, session_key=context.session.basename))
+        data = pro.decode(
+            func.to_dict(protocol=self._protocol.name, frame=self._frame, session_key=context.session.basename))
         logger.info('~ @PRO-DECODE<- protocol:{} parse:{}'.format(self._protocol, data))
 
-        self._handle_framing(context, data)
+        # 异常判断 - 协议服务返回结果
+        if data.get('error') == 1:
+            raise MeterOperationError(data.get('result'))
 
-        self._parse = data.get('parse').get('link_data').get('mission').get('result')
-        self._flush(context)
-        return self._parse
+        # 分帧处理开始
+        next_frame = data.get('next_frame', None)
+        if next_frame is not None:
+            result = send(context,
+                          todo={
+                              'meter:comm': {'channel': {'type': 'RS485', 'baudrate': 9600}, 'frame': next_frame}})
+            self._frame = result.get('result')
+            self.decode(context, index+1)
+        # 分帧处理结束
+
+        if index == 0:
+            self._parse = data.get('result')
+            self._flush(context)
+            return self._parse
 
     def _handle_framing(self, context: Context, data: dict, index=0):
         try:
-            next_frame = data['parse']['next_frame']
+            next_frame = data.get('next_frame', None)
         except:
             next_frame = None
 
         if next_frame is not None:
-            part_frame = data['parse']['session']['part_frame']
-            pfs = context.session.set('part_frame', str(index), part_frame)
-
             result = send(context,
                           todo={
                               'meter:comm': {'channel': {'type': 'RS485', 'baudrate': 9600}, 'frame': next_frame}})
             self._frame = result.get('result')
-            data = pro.decode(func.to_dict(protocol=self._protocol.name, frame=self._frame, session_key=context.session.basename))
+            data = pro.decode(
+                func.to_dict(protocol=self._protocol.name, frame=self._frame, session_key=context.session.basename))
 
-            self.handle_framing(context, data, index + 1)
+            self._handle_framing(context, data, index + 1)
 
     def _flush(self, context: Context):
         context.runtime.steps.update({context.runtime.step: func.to_dict(obj='meter', op=self._operation
                                                                          , element=self._element
                                                                          , parameter=self._parameter,
                                                                          result=self._parse)})
 
@@ -518,9 +532,7 @@
     def parameter(self, param=None):
         self._parameter = param
         return self
 
     def exec(self, context: Context):
         logger.info('~ @ATS-> operation:{} parameter:{}'.format(self._operation, self._parameter))
         return eval('{}(context, {})'.format(self._operation, self._parameter))
-
-
```

### Comparing `ats_case-0.4.3/ats_case/case/context.py` & `ats_case-0.4.4/ats_case/case/context.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.4.3/ats_case/case/executor.py` & `ats_case-0.4.4/ats_case/case/executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,18 @@
     except APIError as ae:
         logger.info(str(ae))
         raise AssertionError(str(ae))
     except ClientReturnError as ce:
         logger.info(str(ce))
         command.client().operation("app:error").message(str(ce))
         raise AssertionError(str(ce))
+    except MeterOperationError as pe:
+        logger.info(str(pe))
+        command.client().operation("app:error").message(str(pe))
+        raise AssertionError(str(pe))
     except Exception as e:
         logger.error(str(e))
         command.client().operation("app:error").message(str(e))
         raise AssertionError(str(e))
 
 
 class Executor(object):
```

### Comparing `ats_case-0.4.3/ats_case/case/translator.py` & `ats_case-0.4.4/ats_case/case/translator.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.4.3/ats_case/common/error.py` & `ats_case-0.4.4/ats_case/common/error.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,20 +2,20 @@
     def __init__(self, value):
         self.value = value
 
     def __str__(self):
         return "APIError - API服务接口[{}], 连接失败.".format(repr(self.value))
 
 
-class ProtocolError(Exception):
+class MeterOperationError(Exception):
     def __init__(self, value):
         self.value = value
 
     def __str__(self):
-        return "ProtocolError - 协议错误. {}".format(repr(self.value))
+        return "MeterOperationError - 电表操作错误, {}".format(repr(self.value))
 
 
 class ClientReturnError(Exception):
     def __init__(self, value):
         self.value = value
 
     def __str__(self):
```

### Comparing `ats_case-0.4.3/ats_case/manage/core.py` & `ats_case-0.4.4/ats_case/manage/core.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.4.3/ats_case/manage/start.py` & `ats_case-0.4.4/ats_case/manage/start.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.4.3/ats_case/template/testcase_v1.tmp` & `ats_case-0.4.4/ats_case/template/testcase_v1.tmp`

 * *Files identical despite different names*

### Comparing `ats_case-0.4.3/ats_case.egg-info/PKG-INFO` & `ats_case-0.4.4/ats_case.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ats-case
-Version: 0.4.3
+Version: 0.4.4
 Summary: Test Script Development Library
 Home-page: https://gitee.com/henry9000/ats_case
 Author: zhangyue
 Author-email: zhangyue@techen.cn
 Project-URL: Bug Tracker, https://gitee.com/henry9000/ats_case/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ats_case-0.4.3/ats_case.egg-info/SOURCES.txt` & `ats_case-0.4.4/ats_case.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ats_case-0.4.3/setup.py` & `ats_case-0.4.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ats_case",
-    version="0.4.3",
+    version="0.4.4",
     py_modules=['ats_case'],
     author="zhangyue",
     author_email="zhangyue@techen.cn",
     description="Test Script Development Library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitee.com/henry9000/ats_case",
```

