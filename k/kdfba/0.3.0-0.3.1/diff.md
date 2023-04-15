# Comparing `tmp/kdfba-0.3.0.tar.gz` & `tmp/kdfba-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\kdfba-0.3.0.tar", last modified: Sun Apr  2 13:58:50 2023, max compression
+gzip compressed data, was "dist\kdfba-0.3.1.tar", last modified: Sat Apr 15 08:22:32 2023, max compression
```

## Comparing `kdfba-0.3.0.tar` & `kdfba-0.3.1.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-02 13:58:50.000000 kdfba-0.3.0/
--rw-rw-rw-   0        0        0     8638 2023-04-02 13:58:50.000000 kdfba-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     7076 2023-03-17 10:44:11.000000 kdfba-0.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-02 13:58:50.000000 kdfba-0.3.0/kdfba/
--rw-rw-rw-   0        0        0      131 2023-03-06 11:38:30.000000 kdfba-0.3.0/kdfba/__init__.py
--rw-rw-rw-   0        0        0     1929 2023-04-02 13:55:27.000000 kdfba-0.3.0/kdfba/dio.py
--rw-rw-rw-   0        0        0     9080 2023-04-02 13:55:27.000000 kdfba-0.3.0/kdfba/model.py
--rw-rw-rw-   0        0        0      626 2023-04-02 13:55:27.000000 kdfba-0.3.0/kdfba/reactions.py
--rw-rw-rw-   0        0        0     3065 2023-04-02 13:55:27.000000 kdfba-0.3.0/kdfba/solver.py
--rw-rw-rw-   0        0        0    12015 2023-04-02 13:55:27.000000 kdfba-0.3.0/kdfba/tool.py
-drwxrwxrwx   0        0        0        0 2023-04-02 13:58:50.000000 kdfba-0.3.0/kdfba.egg-info/
--rw-rw-rw-   0        0        0     8638 2023-04-02 13:58:50.000000 kdfba-0.3.0/kdfba.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      257 2023-04-02 13:58:50.000000 kdfba-0.3.0/kdfba.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-02 13:58:50.000000 kdfba-0.3.0/kdfba.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-04-02 13:58:50.000000 kdfba-0.3.0/kdfba.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-02 13:58:50.000000 kdfba-0.3.0/kdfba.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-02 13:58:50.000000 kdfba-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0      674 2023-04-02 13:58:16.000000 kdfba-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 08:22:32.000000 kdfba-0.3.1/
+-rw-rw-rw-   0        0        0     8853 2023-04-15 08:22:32.000000 kdfba-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     7291 2023-04-03 08:05:27.000000 kdfba-0.3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-15 08:22:32.000000 kdfba-0.3.1/kdfba/
+-rw-rw-rw-   0        0        0      119 2023-04-15 08:18:39.000000 kdfba-0.3.1/kdfba/__init__.py
+-rw-rw-rw-   0        0        0     1548 2023-04-10 06:49:33.000000 kdfba-0.3.1/kdfba/dio.py
+-rw-rw-rw-   0        0        0     7138 2023-04-10 06:49:33.000000 kdfba-0.3.1/kdfba/model.py
+-rw-rw-rw-   0        0        0      626 2023-04-02 13:55:27.000000 kdfba-0.3.1/kdfba/reactions.py
+-rw-rw-rw-   0        0        0     8983 2023-04-15 08:22:08.000000 kdfba-0.3.1/kdfba/solver.py
+drwxrwxrwx   0        0        0        0 2023-04-15 08:22:32.000000 kdfba-0.3.1/kdfba.egg-info/
+-rw-rw-rw-   0        0        0     8853 2023-04-15 08:22:32.000000 kdfba-0.3.1/kdfba.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2023-04-15 08:22:32.000000 kdfba-0.3.1/kdfba.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 08:22:32.000000 kdfba-0.3.1/kdfba.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-04-15 08:22:32.000000 kdfba-0.3.1/kdfba.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-15 08:22:32.000000 kdfba-0.3.1/kdfba.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-15 08:22:32.000000 kdfba-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      674 2023-04-15 08:22:23.000000 kdfba-0.3.1/setup.py
```

### Comparing `kdfba-0.3.0/PKG-INFO` & `kdfba-0.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kdfba
-Version: 0.3.0
+Version: 0.3.1
 Summary: dfba algorithm with kinetics to simulate metabolic activities of microbiota
 Home-page: https://gitee.com/Xu_Billy/d-fba-package
 Author: Xu Billy
 Author-email: xu_tian@stu.scu.edu.cn
 License: MIT License
 Description: # dFBApy - 动态通量平衡分析&&酶动力学模型 in Python
         
@@ -126,28 +126,28 @@
         
         #### 3. 使用求解器对共培养条件进行模拟
         
         ```
         solver = solver()
         model_dict = {'ec1': Ec1, 'ec2': Ec2}
         states_dict = {'x_ec1': 0.5, 'x_ec2': 1, 'glc': 10, 'o2': 20}
-        derivatives = {'o2':'ec1_EX_o2_e+ec2_EX_o2_e', 'glc': 'ec1_EX_glc__D_e+ec2_EX_glc__D_e'}
+        derivatives = {'ec1':'BIOMASS_Ec_iAF1260_core_59p81M', 'ec2': 'BIOMASS_Ec_iAF1260_core_59p81M', 'o2':'ec1_EX_o2_e+ec2_EX_o2_e', 'glc': 'ec1_EX_glc__D_e+ec2_EX_glc__D_e'}
         result = solver.simulate(model_dict, states_dict, derivatives, 5)
         ```
         
         根据dModel对象，初始物质浓度参数以及时间导数参数使用solver对象的simulate函数进行动态模拟。返回多维数组，包含一系列时间点下的不同物质浓度。
         
         **· simulate(models_dict, states_dict, derivatives_description, times, steps, loopless)->scipy.integrate._ivp.ivp.OdeResult**
         
           simulate函数对参与反应的dModel代谢网络优化后不断迭代，而整合的酶动力学模型可描述一段时间范围内物质浓度变化情况。在求解微分方程组的同时即可获得细胞浓度以及各种物质浓度的动态变化情况。
         
             参数：
             · models_dict：参与共培养的所有dModel，字典数据类型，键为给dModel对象取的变量名，值为dModel对象
             · states_dict：参与细胞物质交换反应的反应物，字典数据类型，键为给每种物质取的变量名，值为反应一开始的初始浓度，单位mmol/L（注，每种微生物初始浓度的变量名应命名为x_(dModel变量名，即models_dict中的变量名)，如x_ec)
-            · derivatives_description：时间导数，字典数据类型，键为物质的变量名，值为不同微生物参与到对该物质交换的反应通量之和(注，反应通量变量命名按照(model变量名)+_+reaction_id命名，如ec_EX_o2_e)
+            · derivatives_description：时间导数，字典数据类型，键为物质的变量名，值为不同微生物参与到对该物质交换的反应通量之和(注，反应通量变量命名按照(model变量名)+_+reaction_id命名，如ec_EX_o2_e)；另外，必须输入微生物的生长通量，键为参与模拟的微生物dModel对象变量，值为对应的生物量反应id
             · times：模拟反应的时长，单位h
             · steps：模拟步数，步数越多模拟结果越精确，但时间消耗更大，默认为100
             · loopless：开启后可以消除FVA算法中包含的通量循环使结果更精确，但开启后时间消耗更大，默认为False
         
         ## 参考文献
         
         <p id="1"></p>
```

### Comparing `kdfba-0.3.0/README.md` & `kdfba-0.3.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -118,28 +118,28 @@
 
 #### 3. 使用求解器对共培养条件进行模拟
 
 ```
 solver = solver()
 model_dict = {'ec1': Ec1, 'ec2': Ec2}
 states_dict = {'x_ec1': 0.5, 'x_ec2': 1, 'glc': 10, 'o2': 20}
-derivatives = {'o2':'ec1_EX_o2_e+ec2_EX_o2_e', 'glc': 'ec1_EX_glc__D_e+ec2_EX_glc__D_e'}
+derivatives = {'ec1':'BIOMASS_Ec_iAF1260_core_59p81M', 'ec2': 'BIOMASS_Ec_iAF1260_core_59p81M', 'o2':'ec1_EX_o2_e+ec2_EX_o2_e', 'glc': 'ec1_EX_glc__D_e+ec2_EX_glc__D_e'}
 result = solver.simulate(model_dict, states_dict, derivatives, 5)
 ```
 
 根据dModel对象，初始物质浓度参数以及时间导数参数使用solver对象的simulate函数进行动态模拟。返回多维数组，包含一系列时间点下的不同物质浓度。
 
 **· simulate(models_dict, states_dict, derivatives_description, times, steps, loopless)->scipy.integrate._ivp.ivp.OdeResult**
 
   simulate函数对参与反应的dModel代谢网络优化后不断迭代，而整合的酶动力学模型可描述一段时间范围内物质浓度变化情况。在求解微分方程组的同时即可获得细胞浓度以及各种物质浓度的动态变化情况。
 
     参数：
     · models_dict：参与共培养的所有dModel，字典数据类型，键为给dModel对象取的变量名，值为dModel对象
     · states_dict：参与细胞物质交换反应的反应物，字典数据类型，键为给每种物质取的变量名，值为反应一开始的初始浓度，单位mmol/L（注，每种微生物初始浓度的变量名应命名为x_(dModel变量名，即models_dict中的变量名)，如x_ec)
-    · derivatives_description：时间导数，字典数据类型，键为物质的变量名，值为不同微生物参与到对该物质交换的反应通量之和(注，反应通量变量命名按照(model变量名)+_+reaction_id命名，如ec_EX_o2_e)
+    · derivatives_description：时间导数，字典数据类型，键为物质的变量名，值为不同微生物参与到对该物质交换的反应通量之和(注，反应通量变量命名按照(model变量名)+_+reaction_id命名，如ec_EX_o2_e)；另外，必须输入微生物的生长通量，键为参与模拟的微生物dModel对象变量，值为对应的生物量反应id
     · times：模拟反应的时长，单位h
     · steps：模拟步数，步数越多模拟结果越精确，但时间消耗更大，默认为100
     · loopless：开启后可以消除FVA算法中包含的通量循环使结果更精确，但开启后时间消耗更大，默认为False
 
 ## 参考文献
 
 <p id="1"></p>
```

### Comparing `kdfba-0.3.0/kdfba/reactions.py` & `kdfba-0.3.1/kdfba/reactions.py`

 * *Files identical despite different names*

### Comparing `kdfba-0.3.0/kdfba.egg-info/PKG-INFO` & `kdfba-0.3.1/kdfba.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kdfba
-Version: 0.3.0
+Version: 0.3.1
 Summary: dfba algorithm with kinetics to simulate metabolic activities of microbiota
 Home-page: https://gitee.com/Xu_Billy/d-fba-package
 Author: Xu Billy
 Author-email: xu_tian@stu.scu.edu.cn
 License: MIT License
 Description: # dFBApy - 动态通量平衡分析&&酶动力学模型 in Python
         
@@ -126,28 +126,28 @@
         
         #### 3. 使用求解器对共培养条件进行模拟
         
         ```
         solver = solver()
         model_dict = {'ec1': Ec1, 'ec2': Ec2}
         states_dict = {'x_ec1': 0.5, 'x_ec2': 1, 'glc': 10, 'o2': 20}
-        derivatives = {'o2':'ec1_EX_o2_e+ec2_EX_o2_e', 'glc': 'ec1_EX_glc__D_e+ec2_EX_glc__D_e'}
+        derivatives = {'ec1':'BIOMASS_Ec_iAF1260_core_59p81M', 'ec2': 'BIOMASS_Ec_iAF1260_core_59p81M', 'o2':'ec1_EX_o2_e+ec2_EX_o2_e', 'glc': 'ec1_EX_glc__D_e+ec2_EX_glc__D_e'}
         result = solver.simulate(model_dict, states_dict, derivatives, 5)
         ```
         
         根据dModel对象，初始物质浓度参数以及时间导数参数使用solver对象的simulate函数进行动态模拟。返回多维数组，包含一系列时间点下的不同物质浓度。
         
         **· simulate(models_dict, states_dict, derivatives_description, times, steps, loopless)->scipy.integrate._ivp.ivp.OdeResult**
         
           simulate函数对参与反应的dModel代谢网络优化后不断迭代，而整合的酶动力学模型可描述一段时间范围内物质浓度变化情况。在求解微分方程组的同时即可获得细胞浓度以及各种物质浓度的动态变化情况。
         
             参数：
             · models_dict：参与共培养的所有dModel，字典数据类型，键为给dModel对象取的变量名，值为dModel对象
             · states_dict：参与细胞物质交换反应的反应物，字典数据类型，键为给每种物质取的变量名，值为反应一开始的初始浓度，单位mmol/L（注，每种微生物初始浓度的变量名应命名为x_(dModel变量名，即models_dict中的变量名)，如x_ec)
-            · derivatives_description：时间导数，字典数据类型，键为物质的变量名，值为不同微生物参与到对该物质交换的反应通量之和(注，反应通量变量命名按照(model变量名)+_+reaction_id命名，如ec_EX_o2_e)
+            · derivatives_description：时间导数，字典数据类型，键为物质的变量名，值为不同微生物参与到对该物质交换的反应通量之和(注，反应通量变量命名按照(model变量名)+_+reaction_id命名，如ec_EX_o2_e)；另外，必须输入微生物的生长通量，键为参与模拟的微生物dModel对象变量，值为对应的生物量反应id
             · times：模拟反应的时长，单位h
             · steps：模拟步数，步数越多模拟结果越精确，但时间消耗更大，默认为100
             · loopless：开启后可以消除FVA算法中包含的通量循环使结果更精确，但开启后时间消耗更大，默认为False
         
         ## 参考文献
         
         <p id="1"></p>
```

### Comparing `kdfba-0.3.0/setup.py` & `kdfba-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name = 'kdfba',
-    version = '0.3.0',
+    version = '0.3.1',
     keywords='dfba with kinetics',
     install_requires=['cobra>=0.26.0', 'scipy', 'numpy', 'pandas'],
     description = 'dfba algorithm with kinetics to simulate metabolic activities of microbiota',
     long_description = open('README.md', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     license = 'MIT License',
     url = 'https://gitee.com/Xu_Billy/d-fba-package',
```

