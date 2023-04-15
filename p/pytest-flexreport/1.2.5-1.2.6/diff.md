# Comparing `tmp/pytest-flexreport-1.2.5.tar.gz` & `tmp/pytest-flexreport-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-flexreport-1.2.5.tar", last modified: Wed Apr  5 14:40:02 2023, max compression
+gzip compressed data, was "pytest-flexreport-1.2.6.tar", last modified: Sat Apr 15 05:45:37 2023, max compression
```

## Comparing `pytest-flexreport-1.2.5.tar` & `pytest-flexreport-1.2.6.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2023-04-05 14:40:02.054342 pytest-flexreport-1.2.5/
--rw-rw-rw-   0        0        0     1928 2023-02-05 13:29:28.000000 pytest-flexreport-1.2.5/.gitignore
--rw-rw-rw-   0        0        0     1081 2023-02-05 13:29:28.000000 pytest-flexreport-1.2.5/LICENSE
--rw-rw-rw-   0        0        0      225 2023-02-05 13:29:28.000000 pytest-flexreport-1.2.5/MANIFEST.in
--rw-rw-rw-   0        0        0     3347 2023-04-05 14:40:02.054342 pytest-flexreport-1.2.5/PKG-INFO
--rw-rw-rw-   0        0        0     2141 2023-04-02 03:37:40.000000 pytest-flexreport-1.2.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-05 14:40:02.020719 pytest-flexreport-1.2.5/docs/
--rw-rw-rw-   0        0        0      193 2023-02-05 13:29:28.000000 pytest-flexreport-1.2.5/docs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-05 14:40:02.020719 pytest-flexreport-1.2.5/pytestFlexReport/
--rw-rw-rw-   0        0        0      193 2023-02-05 13:29:28.000000 pytest-flexreport-1.2.5/pytestFlexReport/__init__.py
--rw-rw-rw-   0        0        0     2592 2023-04-05 10:35:18.000000 pytest-flexreport-1.2.5/pytestFlexReport/module_define_init_.py
--rw-rw-rw-   0        0        0      187 2023-02-05 13:29:28.000000 pytest-flexreport-1.2.5/pytestFlexReport/plugin.py
--rw-rw-rw-   0        0        0    10401 2023-04-05 11:10:18.000000 pytest-flexreport-1.2.5/pytestFlexReport/pytest_flexreport.py
-drwxrwxrwx   0        0        0        0 2023-04-05 14:40:02.020719 pytest-flexreport-1.2.5/pytestFlexReport/templates/
--rw-rw-rw-   0        0        0      193 2023-02-05 13:29:28.000000 pytest-flexreport-1.2.5/pytestFlexReport/templates/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-05 14:40:02.020719 pytest-flexreport-1.2.5/pytestFlexReport/templates/static/
--rw-rw-rw-   0        0        0      192 2023-02-05 13:29:28.000000 pytest-flexreport-1.2.5/pytestFlexReport/templates/static/__init__.py
--rw-rw-rw-   0        0        0   160409 2023-02-05 13:29:28.000000 pytest-flexreport-1.2.5/pytestFlexReport/templates/static/bootstrap.min.css
--rw-rw-rw-   0        0        0   536575 2023-02-05 13:29:28.000000 pytest-flexreport-1.2.5/pytestFlexReport/templates/static/echarts.min.js
--rw-rw-rw-   0        0        0    72380 2023-02-05 13:29:28.000000 pytest-flexreport-1.2.5/pytestFlexReport/templates/static/jquery.slim.min.js
--rw-rw-rw-   0        0        0    15412 2023-04-02 03:06:27.000000 pytest-flexreport-1.2.5/pytestFlexReport/templates/template1.html
--rw-rw-rw-   0        0        0    23682 2023-04-02 03:06:23.000000 pytest-flexreport-1.2.5/pytestFlexReport/templates/template2.html
--rw-rw-rw-   0        0        0    11266 2023-04-05 14:20:04.000000 pytest-flexreport-1.2.5/pytestFlexReport/templates/template3.html
--rw-rw-rw-   0        0        0     1115 2023-04-05 14:39:18.000000 pytest-flexreport-1.2.5/pytestFlexReport/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-05 14:40:02.051974 pytest-flexreport-1.2.5/pytest_flexreport.egg-info/
--rw-rw-rw-   0        0        0     3347 2023-04-05 14:40:01.000000 pytest-flexreport-1.2.5/pytest_flexreport.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      983 2023-04-05 14:40:02.000000 pytest-flexreport-1.2.5/pytest_flexreport.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-05 14:40:01.000000 pytest-flexreport-1.2.5/pytest_flexreport.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-04-05 14:40:01.000000 pytest-flexreport-1.2.5/pytest_flexreport.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       23 2023-04-05 14:40:01.000000 pytest-flexreport-1.2.5/pytest_flexreport.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2023-04-05 14:40:01.000000 pytest-flexreport-1.2.5/pytest_flexreport.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       24 2023-02-05 13:29:28.000000 pytest-flexreport-1.2.5/requirements.txt
--rw-rw-rw-   0        0        0      142 2023-04-05 14:40:02.054342 pytest-flexreport-1.2.5/setup.cfg
--rw-rw-rw-   0        0        0     2879 2023-04-05 14:39:47.000000 pytest-flexreport-1.2.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-05 14:40:02.054342 pytest-flexreport-1.2.5/tests/
--rw-rw-rw-   0        0        0      220 2023-04-01 16:21:21.000000 pytest-flexreport-1.2.5/tests/__init__.py
--rw-rw-rw-   0        0        0      193 2023-02-05 13:29:28.000000 pytest-flexreport-1.2.5/tests/conftest.py
--rw-rw-rw-   0        0        0     1029 2023-04-05 11:09:35.000000 pytest-flexreport-1.2.5/tests/run.py
--rw-rw-rw-   0        0        0      765 2023-04-01 16:45:13.000000 pytest-flexreport-1.2.5/tests/test_demo1.py
--rw-rw-rw-   0        0        0     1011 2023-04-05 14:12:23.000000 pytest-flexreport-1.2.5/tests/test_demo2.py
--rw-rw-rw-   0        0        0      437 2023-04-01 15:25:08.000000 pytest-flexreport-1.2.5/tests/test_demo3.py
--rw-rw-rw-   0        0        0      307 2023-02-05 13:29:28.000000 pytest-flexreport-1.2.5/tox.ini
+drwxrwxrwx   0        0        0        0 2023-04-15 05:45:37.123493 pytest-flexreport-1.2.6/
+-rw-rw-rw-   0        0        0     1928 2023-02-05 13:29:28.000000 pytest-flexreport-1.2.6/.gitignore
+-rw-rw-rw-   0        0        0     1081 2023-02-05 13:29:28.000000 pytest-flexreport-1.2.6/LICENSE
+-rw-rw-rw-   0        0        0      225 2023-02-05 13:29:28.000000 pytest-flexreport-1.2.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     3347 2023-04-15 05:45:37.123493 pytest-flexreport-1.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2141 2023-04-02 03:37:40.000000 pytest-flexreport-1.2.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-15 05:45:36.998076 pytest-flexreport-1.2.6/docs/
+-rw-rw-rw-   0        0        0      193 2023-02-05 13:29:28.000000 pytest-flexreport-1.2.6/docs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-15 05:45:37.013706 pytest-flexreport-1.2.6/pytestFlexReport/
+-rw-rw-rw-   0        0        0      193 2023-02-05 13:29:28.000000 pytest-flexreport-1.2.6/pytestFlexReport/__init__.py
+-rw-rw-rw-   0        0        0     2592 2023-04-05 10:35:18.000000 pytest-flexreport-1.2.6/pytestFlexReport/module_define_init_.py
+-rw-rw-rw-   0        0        0      187 2023-02-05 13:29:28.000000 pytest-flexreport-1.2.6/pytestFlexReport/plugin.py
+-rw-rw-rw-   0        0        0    13075 2023-04-15 05:42:05.000000 pytest-flexreport-1.2.6/pytestFlexReport/pytest_flexreport.py
+drwxrwxrwx   0        0        0        0 2023-04-15 05:45:37.076607 pytest-flexreport-1.2.6/pytestFlexReport/templates/
+-rw-rw-rw-   0        0        0      193 2023-02-05 13:29:28.000000 pytest-flexreport-1.2.6/pytestFlexReport/templates/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-15 05:45:37.092249 pytest-flexreport-1.2.6/pytestFlexReport/templates/static/
+-rw-rw-rw-   0        0        0      192 2023-02-05 13:29:28.000000 pytest-flexreport-1.2.6/pytestFlexReport/templates/static/__init__.py
+-rw-rw-rw-   0        0        0   160409 2023-02-05 13:29:28.000000 pytest-flexreport-1.2.6/pytestFlexReport/templates/static/bootstrap.min.css
+-rw-rw-rw-   0        0        0   536575 2023-02-05 13:29:28.000000 pytest-flexreport-1.2.6/pytestFlexReport/templates/static/echarts.min.js
+-rw-rw-rw-   0        0        0    72380 2023-02-05 13:29:28.000000 pytest-flexreport-1.2.6/pytestFlexReport/templates/static/jquery.slim.min.js
+-rw-rw-rw-   0        0        0    15412 2023-04-02 03:06:27.000000 pytest-flexreport-1.2.6/pytestFlexReport/templates/template1.html
+-rw-rw-rw-   0        0        0    23682 2023-04-02 03:06:23.000000 pytest-flexreport-1.2.6/pytestFlexReport/templates/template2.html
+-rw-rw-rw-   0        0        0    11775 2023-04-15 05:43:42.000000 pytest-flexreport-1.2.6/pytestFlexReport/templates/template3.html
+-rw-rw-rw-   0        0        0     1115 2023-04-05 14:39:18.000000 pytest-flexreport-1.2.6/pytestFlexReport/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-15 05:45:37.107876 pytest-flexreport-1.2.6/pytest_flexreport.egg-info/
+-rw-rw-rw-   0        0        0     3347 2023-04-15 05:45:36.000000 pytest-flexreport-1.2.6/pytest_flexreport.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      983 2023-04-15 05:45:36.000000 pytest-flexreport-1.2.6/pytest_flexreport.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 05:45:36.000000 pytest-flexreport-1.2.6/pytest_flexreport.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2023-04-15 05:45:36.000000 pytest-flexreport-1.2.6/pytest_flexreport.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       23 2023-04-15 05:45:36.000000 pytest-flexreport-1.2.6/pytest_flexreport.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2023-04-15 05:45:36.000000 pytest-flexreport-1.2.6/pytest_flexreport.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       24 2023-02-05 13:29:28.000000 pytest-flexreport-1.2.6/requirements.txt
+-rw-rw-rw-   0        0        0      142 2023-04-15 05:45:37.123493 pytest-flexreport-1.2.6/setup.cfg
+-rw-rw-rw-   0        0        0     2879 2023-04-15 05:45:01.000000 pytest-flexreport-1.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 05:45:37.123493 pytest-flexreport-1.2.6/tests/
+-rw-rw-rw-   0        0        0      220 2023-04-01 16:21:21.000000 pytest-flexreport-1.2.6/tests/__init__.py
+-rw-rw-rw-   0        0        0      193 2023-02-05 13:29:28.000000 pytest-flexreport-1.2.6/tests/conftest.py
+-rw-rw-rw-   0        0        0     1029 2023-04-05 11:09:35.000000 pytest-flexreport-1.2.6/tests/run.py
+-rw-rw-rw-   0        0        0      955 2023-04-15 02:54:48.000000 pytest-flexreport-1.2.6/tests/test_demo1.py
+-rw-rw-rw-   0        0        0     2391 2023-04-15 05:41:13.000000 pytest-flexreport-1.2.6/tests/test_demo2.py
+-rw-rw-rw-   0        0        0      437 2023-04-15 05:40:32.000000 pytest-flexreport-1.2.6/tests/test_demo3.py
+-rw-rw-rw-   0        0        0      307 2023-02-05 13:29:28.000000 pytest-flexreport-1.2.6/tox.ini
```

### Comparing `pytest-flexreport-1.2.5/.gitignore` & `pytest-flexreport-1.2.6/.gitignore`

 * *Files identical despite different names*

### Comparing `pytest-flexreport-1.2.5/LICENSE` & `pytest-flexreport-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-flexreport-1.2.5/PKG-INFO` & `pytest-flexreport-1.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-flexreport
-Version: 1.2.5
+Version: 1.2.6
 Summary: UNKNOWN
 Home-page: https://github.com/txu2k8/pytest-flexreport
 Author: TXU
 Author-email: tao.xu2008@outlook.com
 Maintainer: flexreport
 Maintainer-email: tao.xu2008@outlook.com
 License: MIT
```

### Comparing `pytest-flexreport-1.2.5/README.md` & `pytest-flexreport-1.2.6/README.md`

 * *Files identical despite different names*

### Comparing `pytest-flexreport-1.2.5/pytestFlexReport/module_define_init_.py` & `pytest-flexreport-1.2.6/pytestFlexReport/module_define_init_.py`

 * *Files identical despite different names*

### Comparing `pytest-flexreport-1.2.5/pytestFlexReport/pytest_flexreport.py` & `pytest-flexreport-1.2.6/pytestFlexReport/pytest_flexreport.py`

 * *Files 25% similar despite different names*

```diff
@@ -29,60 +29,104 @@
     skipped: int = 0
     error: int = 0
     total: int = 0
     pass_rate: float = 0
     duration: int = 0  # 耗时 秒
 
 
+# 模块树统计测试结果
+class ModuleResult(BaseModel):
+    idx: int = 0  # 序号
+    name: Text = ''  # 模块名称
+    first: bool = False  # 标记是否第一个模块/子模块
+    subs_len: int = 0  # 子模块数量
+    subs_len_v3: int = 0  # 包含三级模块数量
+    subs: Dict = {}  # 子模块：name=StatisticsModule()
+    outcome: StatisticsOutcome = StatisticsOutcome()  # 结果统计
+
+
+# 测试结果
 class TestResult(StatisticsOutcome):
     """测试结果信息 - 数据模型"""
     title: Text = ''
     tester: Text = ''
     desc: Text = ''
     log_path: Text = ''
     report_path: Text = ''
 
     start_time: int = 0
     begin_time: Text = ''
 
     cases: Dict = {}
     modules: List = []
     history: List = []
+    module_result: Dict = defaultdict(dict)  # 按模块统计测试结果
     module_outcome: Dict = defaultdict(dict)  # 按模块统计测试结果
     report_sort: bool = False  # 参数报告中模块按名称排序
 
 
 result = TestResult()
 
 
+def format_module_result(module_result: ModuleResult) -> ModuleResult:
+    module_result.outcome.duration = utils.seconds_to_hms(module_result.outcome.duration)
+    if module_result.outcome.total != 0:
+        rate = module_result.outcome.passed / module_result.outcome.total * 100
+        module_result.outcome.pass_rate = utils.remove_decimal0(float('{:.1f}'.format(rate)))
+    else:
+        module_result.outcome.pass_rate = 0
+    return module_result
+
+
 def pytest_make_parametrize_id(config, val, argname):
     if isinstance(val, dict):
         return val.get('title') or val.get('desc')
 
 
 def pytest_runtest_logreport(report):
     if report.moduleName not in result.modules:
-        result.modules.append(report.moduleName)
-    if not result.module_outcome[report.moduleName]:
-        result.module_outcome[report.moduleName] = StatisticsOutcome()
+        result.modules.append(report.moduleName)  # template1/template2
+    m1, m2, m3 = report.module_name_v3
+    if m1 not in result.module_result:
+        result.module_result[m1] = ModuleResult(name=m1)
+        result.module_result[m1].idx = len(result.module_result)
+    if m2 not in result.module_result[m1].subs:
+        result.module_result[m1].subs_len += 1
+        result.module_result[m1].subs[m2] = ModuleResult(name=m2)
+        result.module_result[m1].subs[m2].idx = len(result.module_result[m1].subs)
+    if m3 not in result.module_result[m1].subs[m2].subs:
+        result.module_result[m1].subs[m2].subs_len += 1
+        result.module_result[m1].subs[m2].subs[m3] = ModuleResult(name=m3)
+        result.module_result[m1].subs[m2].subs[m3].idx = len(result.module_result[m1].subs[m2].subs)
+        # subs_len_v3
+        result.module_result[m1].subs_len_v3 += 1
+        result.module_result[m1].subs[m2].subs_len_v3 += 1
+
     if report.when == 'setup':
         result.total += 1
-        result.module_outcome[report.moduleName].total += 1
+        result.module_result[m1].outcome.total += 1
+        result.module_result[m1].subs[m2].outcome.total += 1
+        result.module_result[m1].subs[m2].subs[m3].outcome.total += 1
         if report.outcome != 'passed':
             result.error += 1
-            result.module_outcome[report.moduleName]["error"] += 1
+            result.module_result[m1].outcome.error += 1
+            result.module_result[m1].subs[m2].outcome.error += 1
+            result.module_result[m1].subs[m2].subs[m3].outcome.error += 1
     elif report.when == 'call':
         setattr(result, report.outcome, getattr(result, report.outcome)+1)
-        setattr(result.module_outcome[report.moduleName], report.outcome,
-                getattr(result.module_outcome[report.moduleName], report.outcome)+1)
-
-    result.module_outcome[report.moduleName].duration += report.duration
+        setattr(result.module_result[m1].outcome, report.outcome, getattr(result.module_result[m1].outcome, report.outcome)+1)
+        setattr(result.module_result[m1].subs[m2].outcome, report.outcome, getattr(result.module_result[m1].subs[m2].outcome, report.outcome)+1)
+        setattr(result.module_result[m1].subs[m2].subs[m3].outcome, report.outcome, getattr(result.module_result[m1].subs[m2].subs[m3].outcome, report.outcome)+1)
+
+    result.module_result[m1].outcome.duration += report.duration
+    result.module_result[m1].subs[m2].outcome.duration += report.duration
+    result.module_result[m1].subs[m2].subs[m3].outcome.duration += report.duration
     result.duration += report.duration
 
-    report.duration = '{:.2f}'.format(report.duration)
+    report.duration = '{:.2f}'.format(float(report.duration))
     result.cases[report.nodeid] = report
 
 
 def pytest_sessionstart(session):
     start_ts = datetime.datetime.now()
     result.start_time = start_ts.timestamp()
     result.begin_time = start_ts.strftime("%Y-%m-%d %H:%M:%S")
@@ -146,25 +190,20 @@
     if result.total != 0:
         rate = result.passed / result.total * 100
         result.pass_rate = utils.remove_decimal0(float('{:.1f}'.format(rate)))
     else:
         result.pass_rate = 0
 
     # 处理模块统计数据
-    for m in result.module_outcome.keys():
-        # result.module_outcome[m].duration = '{:.2f}'.format(result.module_outcome[m].duration)
-        result.module_outcome[m].duration = utils.seconds_to_hms(result.module_outcome[m].duration)
-        if result.module_outcome[m].total != 0:
-            rate = result.module_outcome[m].passed / result.module_outcome[m].total * 100
-            result.module_outcome[m].pass_rate = utils.remove_decimal0(float('{:.1f}'.format(rate)))
-        else:
-            result.module_outcome[m].pass_rate = 0
-    # 排序
-    if result.report_sort is True:
-        result.module_outcome = dict(sorted(result.module_outcome.items(), key=lambda x: x[0]))
+    for m1 in result.module_result.keys():
+        result.module_result[m1] = format_module_result(result.module_result[m1])
+        for m2 in result.module_result[m1].subs.keys():
+            result.module_result[m1].subs[m2] = format_module_result(result.module_result[m1].subs[m2])
+            for m3 in result.module_result[m1].subs[m2].subs.keys():
+                result.module_result[m1].subs[m2].subs[m3] = format_module_result(result.module_result[m1].subs[m2].subs[m3])
     # 保存历史数据
     result.history = handle_history_data(history_dir, result)
     # 渲染报告
     template_path = os.path.join(os.path.dirname(__file__), './templates')
     template_static_path = os.path.join(template_path, 'static')
     # 复制渲染文件 css、js
     shutil.copyfile(os.path.join(template_static_path, "bootstrap.min.css"), os.path.join(report_static_dir, "bootstrap.min.css"))
@@ -181,38 +220,51 @@
 def pytest_runtest_makereport(item, call):
     outcome = yield
     report = outcome.get_result()
     fixture_extras = getattr(item.config, "extras", [])
     plugin_extras = getattr(report, "extra", [])
     report.extra = fixture_extras + plugin_extras
 
-    # 获取模块名
+    # 获取用例模块名，例如：
+    # @allure.epic("对象存储")
+    # @allure.story("桶")
+    # @allure.feature("对象")
     module_dict = defaultdict(str)
     if hasattr(item.instance, 'pytestmark'):
         for pm in item.instance.pytestmark:
             if 'label_type' in pm.kwargs:
                 module_dict[pm.kwargs["label_type"]] = pm.args[0]
     for om in item.own_markers:
         if 'label_type' in om.kwargs:
             module_dict[om.kwargs["label_type"]] = om.args[0]
 
-    module_name_list = ['']
-    if module_dict['epic']:
-        module_name_list.append(module_dict['epic'])
-    if module_dict['story']:
-        module_name_list.append(module_dict['story'])
-    if module_dict['feature']:
-        module_name_list.append(module_dict['feature'])
-    if len(module_name_list) <= 1:
+    # 三级模块
+    module_name_v3 = [
+        module_dict['epic'],
+        module_dict['story'],
+        module_dict['feature'],
+    ]
+
+    # 未设置allure模块名，则获取__init__.py中定义的模块名称，例如：
+    # __module_zh__ = 'tests'
+    if not (module_dict['epic'] or module_dict['story'] or module_dict['feature']):
         testcase_basename = item.config.getoption('--testcase_basename')
-        module_name_list.extend(ModuleDefineInit().get_testcase_module_list(
+        test_case_modules = ModuleDefineInit().get_testcase_module_list(
             item.fspath.dirname, testcase_basename or item.config.rootdir.basename
-        ))
+        )
+        # 如果__init__.py中也未定义的模块名称，取py模块名称
+        if len(test_case_modules) == 0:
+            test_case_modules = [item.location[0]]
+        # 赋值到三级模块列表
+        for idx, m in enumerate(test_case_modules):
+            module_name_v3[idx] = m
+
     # print(module_name_list)
-    report.moduleName = '/'.join(module_name_list) if len(module_name_list) > 1 else item.location[0]
+    report.moduleName = '/'.join(module_name_v3)
+    report.module_name_v3 = module_name_v3
 
     if hasattr(item, 'callspec'):
         report.desc = item.callspec.id or item._obj.__doc__
     else:
         report.desc = item._obj.__doc__
     report.method = item.location[2].split('[')[0]
```

### Comparing `pytest-flexreport-1.2.5/pytestFlexReport/templates/static/bootstrap.min.css` & `pytest-flexreport-1.2.6/pytestFlexReport/templates/static/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `pytest-flexreport-1.2.5/pytestFlexReport/templates/static/echarts.min.js` & `pytest-flexreport-1.2.6/pytestFlexReport/templates/static/echarts.min.js`

 * *Files identical despite different names*

### Comparing `pytest-flexreport-1.2.5/pytestFlexReport/templates/static/jquery.slim.min.js` & `pytest-flexreport-1.2.6/pytestFlexReport/templates/static/jquery.slim.min.js`

 * *Files identical despite different names*

### Comparing `pytest-flexreport-1.2.5/pytestFlexReport/templates/template1.html` & `pytest-flexreport-1.2.6/pytestFlexReport/templates/template1.html`

 * *Files identical despite different names*

### Comparing `pytest-flexreport-1.2.5/pytestFlexReport/templates/template2.html` & `pytest-flexreport-1.2.6/pytestFlexReport/templates/template2.html`

 * *Files identical despite different names*

### Comparing `pytest-flexreport-1.2.5/pytestFlexReport/templates/template3.html` & `pytest-flexreport-1.2.6/pytestFlexReport/templates/template3.html`

 * *Files 10% similar despite different names*

```diff
@@ -292,29 +292,59 @@
 
   <div class="result_table">
     <h2>结果统计</h2>
     <div class="table_data">
       <table class="table" style="color: #fff">
         <thead class="text-light" style="background: rgba(3, 14, 70, 0.5)">
         <tr>
-          <th scope="col" style="width: 5%;padding: 0">ID</th>
-          <th scope="col" style="width: 25%;padding: 0">模块</th>
+          <th scope="col" style="width: 12%;padding: 0">一级模块</th>
+          <th scope="col" style="width: 12%;padding: 0">二级模块</th>
+          <th scope="col" style="width: 12%;padding: 0">三级模块</th>
           <th scope="col" style="width: 10%;padding: 0">耗时</th>
-          <th scope="col" style="width: 10%;padding: 0">总数</th>
-          <th scope="col" style="width: 10%;padding: 0">通过</th>
-          <th scope="col" style="width: 10%;padding: 0">失败</th>
-          <th scope="col" style="width: 10%;padding: 0">阻塞</th>
-          <th scope="col" style="width: 10%;padding: 0">跳过</th>
-          <th scope="col" style="width: 10%;padding: 0">通过率</th>
+          <th scope="col" style="width: 8%;padding: 0">总数</th>
+          <th scope="col" style="width: 8%;padding: 0">通过</th>
+          <th scope="col" style="width: 8%;padding: 0">失败</th>
+          <th scope="col" style="width: 8%;padding: 0">阻塞</th>
+          <th scope="col" style="width: 8%;padding: 0">跳过</th>
+          <th scope="col" style="width: 8%;padding: 0">通过率</th>
         </tr>
         </thead>
         <tbody>
+
+        {% for m1, foo1 in module_result.items() %}
+          {% for m2, foo2 in foo1.subs.items() %}
+            {% for m3, foo3 in foo2.subs.items() %}
+              <tr class="case_">
+                {% if foo2.idx == 1 and foo3.idx == 1 %}<td rowspan="{{ foo1.subs_len_v3 }}">{{ foo1.name }}</td>
+                {% endif %}
+                {% if foo3.idx == 1 %}<td rowspan="{{ foo2.subs_len_v3 }}">{{ foo2.name }}</td>
+                {% endif %}
+                <td>{{ foo3.name }}</td>
+                <td>{{ foo3.outcome.duration }}</td>
+                <td>{{ foo3.outcome.total }}</td>
+                <td>{{ foo3.outcome.passed }}</td>
+                <td>{{ foo3.outcome.failed }}</td>
+                <td>{{ foo3.outcome.error }}</td>
+                <td>{{ foo3.outcome.skipped }}</td>
+                {% if foo3.outcome.pass_rate < 70 %}
+                  <td style="color: rgb(245,108,108);">{{ foo3.outcome.pass_rate }}%</td>
+                {% elif foo3.outcome.pass_rate < 90 %}
+                  <td style="color: rgb(230,162,60);">{{ foo3.outcome.pass_rate }}%</td>
+                {% elif foo3.outcome.pass_rate == 100 %}
+                  <td style="color: rgb(103,194,58);">{{ foo3.outcome.pass_rate }}%</td>
+                {% else %}
+                  <td>{{ foo3.outcome.pass_rate }}%</td>
+                {% endif %}
+              </tr>
+            {% endfor %}
+          {% endfor %}
+        {% endfor %}
+        {#  合计 #}
         <tr>
-          <td>0</td>
-          <td>合计</td>
+          <td colspan="3">合计</td>
           <td>{{ duration }}</td>
           <td>{{ total }}</td>
           <td>{{ passed }}</td>
           <td>{{ failed }}</td>
           <td>{{ error }}</td>
           <td>{{ skipped }}</td>
           {% if pass_rate < 70 %}
@@ -323,37 +353,14 @@
             <td style="color: rgb(230,162,60);">{{ pass_rate }}%</td>
           {% elif pass_rate == 100 %}
             <td style="color: rgb(103,194,58);">{{ pass_rate }}%</td>
           {% else %}
             <td>{{ pass_rate }}%</td>
           {% endif %}
         </tr>
-        {% for name, foo in module_outcome.items() %}
-          <tr class="case_">
-            <td>{{ loop.index }}</td>
-            <td class="{{ name|replace('\\','')|replace('.','') }}"
-                style="text-align: left">{{ name.split("\\")[-1] }}</td>
-            <td>{{ foo.duration }}</td>
-            <td>{{ foo.total }}</td>
-            <td>{{ foo.passed }}</td>
-            <td>{{ foo.failed }}</td>
-            <td>{{ foo.error }}</td>
-            <td>{{ foo.skipped }}</td>
-            {#            <td>{{ foo.pass_rate }}%</td>#}
-            {% if foo.pass_rate < 70 %}
-              <td style="color: rgb(245,108,108);">{{ foo.pass_rate }}%</td>
-            {% elif foo.pass_rate < 90 %}
-              <td style="color: rgb(230,162,60);">{{ foo.pass_rate }}%</td>
-            {% elif foo.pass_rate == 100 %}
-              <td style="color: rgb(103,194,58);">{{ foo.pass_rate }}%</td>
-            {% else %}
-              <td>{{ foo.pass_rate }}%</td>
-            {% endif %}
-          </tr>
-        {% endfor %}
       </table>
     </div>
 
     <div style="height: 20px"></div>
   </div>
 
 </div>
```

#### html2text {}

```diff
@@ -11,15 +11,13 @@
 éè¿ç {{ pass_rate }}% ï¼{{ passed }}/{{ total }}ï¼ {% endif %}
 ***** åºæ¬ä¿¡æ¯ *****
 æµè¯æè¿° {{ desc }}
 æ¥å¿è¯¦æ {{_log_path_}}
 æ¥åè¯¦æ {{_report_path_}}
 ç¯å¢ä¿¡æ¯ {{_report_path_}}
 ***** ç»æç»è®¡ *****
-ID         æ¨¡å�èæ¶ æ»æéè¿�å¤±è´�é»å¡è·³è¿éè¿ç
-0          åè®�{{ duration  {{ total  {{ passed  {{ failed  {{ error  {{ skipped  {{ pass_rate  {{ pass_rate  {{ pass_rate  {{ pass_rate
-                      }}           }}        }}         }}         }}        }}          }}%           }}%           }}%           }}%
-{          {          {            {         {          {          {         {           {             {             {             {             {
-{          {          {            {         {          {          {         {           {             {             {             {             {
-loop.index name.split foo.duration foo.total foo.passed foo.failed foo.error foo.skipped foo.pass_rate foo.pass_rate foo.pass_rate foo.pass_rate foo.pass_rate
-}}         ("\\")[-1] }}           }}        }}         }}         }}        }}          }}%           }}%           }}%           }}%           }}%
-           }}
+ä¸çº§�äºçº§�ä¸çº§�èæ¶          æ»æ°       éè¿        å¤±è´¥        é»å¡       è·³è¿         éè¿ç
+                                       {                     {                  {                   {                   {                  {                    {                      {                      {                      {
+{{ foo1.name {{ foo2.name {{ foo3.name {                     {                  {                   {                   {                  {                    {                      {                      {                      {
+}}           }}           }}           foo3.outcome.duration foo3.outcome.total foo3.outcome.passed foo3.outcome.failed foo3.outcome.error foo3.outcome.skipped foo3.outcome.pass_rate foo3.outcome.pass_rate foo3.outcome.pass_rate foo3.outcome.pass_rate
+                                       }}                    }}                 }}                  }}                  }}                 }}                   }}%                    }}%                    }}%                    }}%
+åè®¡                           {{ duration }}        {{ total }}        {{ passed }}        {{ failed }}        {{ error }}        {{ skipped }}        {{ pass_rate }}%       {{ pass_rate }}%       {{ pass_rate }}%       {{ pass_rate }}%
```

### Comparing `pytest-flexreport-1.2.5/pytestFlexReport/utils.py` & `pytest-flexreport-1.2.6/pytestFlexReport/utils.py`

 * *Files identical despite different names*

### Comparing `pytest-flexreport-1.2.5/pytest_flexreport.egg-info/PKG-INFO` & `pytest-flexreport-1.2.6/pytest_flexreport.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-flexreport
-Version: 1.2.5
+Version: 1.2.6
 Summary: UNKNOWN
 Home-page: https://github.com/txu2k8/pytest-flexreport
 Author: TXU
 Author-email: tao.xu2008@outlook.com
 Maintainer: flexreport
 Maintainer-email: tao.xu2008@outlook.com
 License: MIT
```

### Comparing `pytest-flexreport-1.2.5/pytest_flexreport.egg-info/SOURCES.txt` & `pytest-flexreport-1.2.6/pytest_flexreport.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytest-flexreport-1.2.5/setup.py` & `pytest-flexreport-1.2.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
             if item is not None:
                 packages.append(item.lstrip('.'))
     return packages
 
 
 setup(
     name='pytest-flexreport',
-    version='1.2.5',
+    version='1.2.6',
     author='TXU',
     author_email='tao.xu2008@outlook.com',
     maintainer='flexreport',
     maintainer_email='tao.xu2008@outlook.com',
     license='MIT',
     url='https://github.com/txu2k8/pytest-flexreport',
     long_description=read_file('README.md'),
```

### Comparing `pytest-flexreport-1.2.5/tests/run.py` & `pytest-flexreport-1.2.6/tests/run.py`

 * *Files identical despite different names*

### Comparing `pytest-flexreport-1.2.5/tests/test_demo1.py` & `pytest-flexreport-1.2.6/tests/test_demo1.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,32 +9,44 @@
 """
 import time
 import allure
 
 
 @allure.epic("OM")
 @allure.story("登录")
-# @allure.feature("首页")
-@allure.suite("正常")
+@allure.feature("正常")
 class TestDemo1(object):
-
     def test_1(self):
-        allure.dynamic.feature("首页2")
         time.sleep(1)
         print("TestDemo1--->>> test_1")
         assert 3 + 2 == 5
 
-    @allure.feature("首页2")
     def test_2(self):
         assert 3 + 2 == 6
 
-    @allure.feature("首页1")
     def test_3(self):
         assert 3 + 2 == 5
 
-    @allure.feature("首页1")
     def test_4(self):
         assert 3 + 2 == 5
 
 
+@allure.epic("OM")
+@allure.story("首页")
+@allure.feature("正常")
+class TestDemo22(object):
+    def test_221(self):
+        print("TestDemo1--->>> test_1")
+        assert 3 + 2 == 5
+
+    def test_222(self):
+        assert 3 + 2 == 6
+
+    def test_223(self):
+        assert 3 + 2 == 5
+
+    def test_224(self):
+        assert 3 + 2 == 5
+
+
 if __name__ == '__main__':
     pass
```

