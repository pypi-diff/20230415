# Comparing `tmp/a_pandas_ex_easy_loc-0.13.tar.gz` & `tmp/a_pandas_ex_easy_loc-0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "a_pandas_ex_easy_loc-0.13.tar", last modified: Fri Apr 14 23:38:45 2023, max compression
+gzip compressed data, was "a_pandas_ex_easy_loc-0.14.tar", last modified: Fri Apr 14 23:43:31 2023, max compression
```

## Comparing `a_pandas_ex_easy_loc-0.13.tar` & `a_pandas_ex_easy_loc-0.14.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 23:38:45.485807 a_pandas_ex_easy_loc-0.13/
--rw-rw-rw-   0        0        0     1148 2023-04-14 23:38:41.000000 a_pandas_ex_easy_loc-0.13/LICENSE.rst
--rw-rw-rw-   0        0        0      131 2023-04-14 23:38:41.000000 a_pandas_ex_easy_loc-0.13/MANIFEST.in
--rw-rw-rw-   0        0        0    55576 2023-04-14 23:38:45.486805 a_pandas_ex_easy_loc-0.13/PKG-INFO
--rw-rw-rw-   0        0        0    54417 2023-04-14 23:15:39.000000 a_pandas_ex_easy_loc-0.13/README.md
-drwxrwxrwx   0        0        0        0 2023-04-14 23:38:45.481817 a_pandas_ex_easy_loc-0.13/a_pandas_ex_easy_loc/
--rw-rw-rw-   0        0        0    54417 2023-04-14 23:15:39.000000 a_pandas_ex_easy_loc-0.13/a_pandas_ex_easy_loc/README.md
--rw-rw-rw-   0        0        0    22528 2023-04-14 23:17:13.000000 a_pandas_ex_easy_loc-0.13/a_pandas_ex_easy_loc/__init__.py
--rw-rw-rw-   0        0        0      103 2023-04-14 23:38:44.000000 a_pandas_ex_easy_loc-0.13/a_pandas_ex_easy_loc/requirements.txt
--rw-rw-rw-   0        0        0     5332 2023-04-14 23:38:44.000000 a_pandas_ex_easy_loc-0.13/a_pandas_ex_easy_loc/thirdparty.json
-drwxrwxrwx   0        0        0        0 2023-04-14 23:38:45.484810 a_pandas_ex_easy_loc-0.13/a_pandas_ex_easy_loc.egg-info/
--rw-rw-rw-   0        0        0    55576 2023-04-14 23:38:45.000000 a_pandas_ex_easy_loc-0.13/a_pandas_ex_easy_loc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      410 2023-04-14 23:38:45.000000 a_pandas_ex_easy_loc-0.13/a_pandas_ex_easy_loc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 23:38:45.000000 a_pandas_ex_easy_loc-0.13/a_pandas_ex_easy_loc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       99 2023-04-14 23:38:45.000000 a_pandas_ex_easy_loc-0.13/a_pandas_ex_easy_loc.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-04-14 23:38:45.000000 a_pandas_ex_easy_loc-0.13/a_pandas_ex_easy_loc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2023-04-14 23:38:45.486805 a_pandas_ex_easy_loc-0.13/setup.cfg
--rw-rw-rw-   0        0        0     1466 2023-04-14 23:38:44.000000 a_pandas_ex_easy_loc-0.13/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 23:43:31.825339 a_pandas_ex_easy_loc-0.14/
+-rw-rw-rw-   0        0        0     1148 2023-04-14 23:43:27.000000 a_pandas_ex_easy_loc-0.14/LICENSE.rst
+-rw-rw-rw-   0        0        0      131 2023-04-14 23:43:27.000000 a_pandas_ex_easy_loc-0.14/MANIFEST.in
+-rw-rw-rw-   0        0        0    55124 2023-04-14 23:43:31.825339 a_pandas_ex_easy_loc-0.14/PKG-INFO
+-rw-rw-rw-   0        0        0    54417 2023-04-14 23:15:39.000000 a_pandas_ex_easy_loc-0.14/README.md
+drwxrwxrwx   0        0        0        0 2023-04-14 23:43:31.820352 a_pandas_ex_easy_loc-0.14/a_pandas_ex_easy_loc/
+-rw-rw-rw-   0        0        0    54417 2023-04-14 23:15:39.000000 a_pandas_ex_easy_loc-0.14/a_pandas_ex_easy_loc/README.md
+-rw-rw-rw-   0        0        0    22528 2023-04-14 23:17:13.000000 a_pandas_ex_easy_loc-0.14/a_pandas_ex_easy_loc/__init__.py
+-rw-rw-rw-   0        0        0      103 2023-04-14 23:43:31.000000 a_pandas_ex_easy_loc-0.14/a_pandas_ex_easy_loc/requirements.txt
+-rw-rw-rw-   0        0        0     5332 2023-04-14 23:43:31.000000 a_pandas_ex_easy_loc-0.14/a_pandas_ex_easy_loc/thirdparty.json
+drwxrwxrwx   0        0        0        0 2023-04-14 23:43:31.824342 a_pandas_ex_easy_loc-0.14/a_pandas_ex_easy_loc.egg-info/
+-rw-rw-rw-   0        0        0    55124 2023-04-14 23:43:31.000000 a_pandas_ex_easy_loc-0.14/a_pandas_ex_easy_loc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      410 2023-04-14 23:43:31.000000 a_pandas_ex_easy_loc-0.14/a_pandas_ex_easy_loc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 23:43:31.000000 a_pandas_ex_easy_loc-0.14/a_pandas_ex_easy_loc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       99 2023-04-14 23:43:31.000000 a_pandas_ex_easy_loc-0.14/a_pandas_ex_easy_loc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-04-14 23:43:31.000000 a_pandas_ex_easy_loc-0.14/a_pandas_ex_easy_loc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2023-04-14 23:43:31.826336 a_pandas_ex_easy_loc-0.14/setup.cfg
+-rw-rw-rw-   0        0        0     1606 2023-04-14 23:43:31.000000 a_pandas_ex_easy_loc-0.14/setup.py
```

### Comparing `a_pandas_ex_easy_loc-0.13/LICENSE.rst` & `a_pandas_ex_easy_loc-0.14/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `a_pandas_ex_easy_loc-0.13/PKG-INFO` & `a_pandas_ex_easy_loc-0.14/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,469 +1,468 @@
 Metadata-Version: 2.1
 Name: a_pandas_ex_easy_loc
-Version: 0.13
+Version: 0.14
 Summary: Search and replace values with df.loc without Exceptions due to dtype incompatibility
 Home-page: https://github.com/hansalemaos/a_pandas_ex_easy_loc
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: loc,iloc,df.at,df.iat,pandas,DataFrame,Series
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE.rst
 
+### A tolerant version of df.loc
 
-### A tolerant version of df.loc
-
-Search and replace values with df.loc without Exceptions due to dtype incompatibility.  If the dtypes of 2 variables don't match, they will be converted until they match. 
-
-```python
-pip install a_pandas_ex_easy_loc
-```
-
-Some examples
-
-```python
-import pandas as pd
-df = pd.read_csv("https://github.com/pandas-dev/pandas/raw/main/doc/data/titanic.csv")
-# df.loc[df.Ticket >20000]
-from random import randrange
-getrandomlist = lambda x: [
-  [[randrange(1, 100), randrange(1, 100)] * 1] * randrange(1, 10)
-]
-df["listtest"] = df.PassengerId.map(getrandomlist)
-
-
-getrandomdict = lambda x: {
-  randrange(1, 100):randrange(1, 100) for _ in range(randrange(1, 10))
-}
-df["dicttest"] = df.PassengerId.map(getrandomdict)
-from a_easy_loc import pd_add_easy_loc
-pd_add_easy_loc()
-df.shortloc_greater_replace('Pclass', 2,3000)
-
-df.shortloc_equal('Pclass', 3)
-     PassengerId  Survived  Pclass       Name     Sex    Age  SibSp  Parch     Ticket     Fare  Cabin Embarked   listtest   dicttest
-0            1           0       3  Braund...    male  22.00      1      0  A/5 21171   7.2500    NaN        S  [[[44,...  {5: 8,...
-2            3           1       3  Heikki...  female  26.00      0      0  STON/O...   7.9250    NaN        S  [[[60,...  {33: 3...
-4            5           0       3  Allen,...    male  35.00      0      0     373450   8.0500    NaN        S  [[[99,...  {96: 1...
-5            6           0       3  Moran,...    male    NaN      0      0     330877   8.4583    NaN        Q  [[[82,...  {23: 1...
-7            8           0       3  Palsso...    male   2.00      3      1     349909  21.0750    NaN        S  [[[14,...  {20: 8...
-8            9           1       3  Johnso...  female  27.00      0      2     347742  11.1333    NaN        S  [[[12,...  {96: 5...
-
-
-df.shortloc_equal('Ticket', 373450)
-   PassengerId  Survived  Pclass       Name   Sex   Age  SibSp  Parch  Ticket  Fare Cabin Embarked   listtest   dicttest
-4          5           0       3  Allen,...  male  35.0      0      0  373450  8.05   NaN        S  [[[99,...  {96: 1...
-
-
-df.shortloc_greater('Pclass', 2)
-     PassengerId  Survived  Pclass       Name     Sex    Age  SibSp  Parch     Ticket     Fare  Cabin Embarked   listtest   dicttest
-0            1           0       3  Braund...    male  22.00      1      0  A/5 21171   7.2500    NaN        S  [[[44,...  {5: 8,...
-2            3           1       3  Heikki...  female  26.00      0      0  STON/O...   7.9250    NaN        S  [[[60,...  {33: 3...
-4            5           0       3  Allen,...    male  35.00      0      0     373450   8.0500    NaN        S  [[[99,...  {96: 1...
-5            6           0       3  Moran,...    male    NaN      0      0     330877   8.4583    NaN        Q  [[[82,...  {23: 1...
-
-df.shortloc_greater('Ticket', 373450)
-     PassengerId  Survived  Pclass       Name     Sex   Age  SibSp  Parch   Ticket     Fare Cabin Embarked   listtest   dicttest
-16          17           0       3  Rice, ...    male   2.0      4      1   382652  29.1250   NaN        Q  [[[17,...  {46: 7...
-50          51           0       3  Panula...    male   7.0      4      1  3101295  39.6875   NaN        S  [[[30,...  {64: 2...
-68          69           1       3  Anders...  female  17.0      4      2  3101281   7.9250   NaN        S  [[[4, ...  {92: 3...
-77          78           0       3  Moutal...    male   NaN      0      0   374746   8.0500   NaN        S  [[[65,...  {47: 9...
-85          86           1       3  Backst...  female  33.0      3      0  3101278  15.8500   NaN        S  [[[55,...  {5: 22...
-
-
-df.shortloc_greater_or_equal('Age', 43)
-     PassengerId  Survived  Pclass       Name     Sex   Age  SibSp  Parch     Ticket      Fare      Cabin Embarked   listtest   dicttest
-6            7           0       1  McCart...    male  54.0      0      0      17463   51.8625        E46        S  [[[47,...   {22: 17}
-11          12           1       1  Bonnel...  female  58.0      0      0     113783   26.5500       C103        S  [[[1, ...    {35: 9}
-15          16           1       2  Hewlet...  female  55.0      0      0     248706   16.0000        NaN        S  [[[43,...  {40: 6...
-33          34           0       2  Wheado...    male  66.0      0      0  C.A. 2...   10.5000        NaN        S  [[[6, ...   {50: 28}
-52          53           1       1  Harper...  female  49.0      1      0   PC 17572   76.7292        D33        C  [[[41,...  {54: 6...
-
-
-df.shortloc_greater_replace('Pclass', 2,3000)
-     PassengerId  Survived  Pclass       Name     Sex    Age  SibSp  Parch     Ticket      Fare      Cabin Embarked   listtest   dicttest
-0            1           0    3000  Braund...    male  22.00      1      0  A/5 21171    7.2500        NaN        S  [[[65,...  {76: 3...
-1            2           1       1  Cuming...  female  38.00      1      0   PC 17599   71.2833        C85        C  [[[1, ...  {55: 3...
-2            3           1    3000  Heikki...  female  26.00      0      0  STON/O...    7.9250        NaN        S  [[[56,...  {7: 54...
-3            4           1       1  Futrel...  female  35.00      1      0     113803   53.1000       C123        S  [[[91,...   {51: 89}
-4            5           0    3000  Allen,...    male  35.00      0      0     373450    8.0500        NaN        S  [[[20,...  {39: 5...
-5            6           0    3000  Moran,...    male    NaN      0      0     330877    8.4583        NaN        Q  [[[60,...  {63: 2...
-6            7           0       1  McCart...    male  54.00      0      0      17463   51.8625        E46        S  [[[51,...  {1: 90...
-
-
-
-df.shortloc_greater_replace('Ticket', 5000, 888000)
-     PassengerId  Survived  Pclass       Name     Sex    Age  SibSp  Parch     Ticket      Fare      Cabin Embarked   listtest   dicttest
-0            1           0       3  Braund...    male  22.00      1      0  A/5 21171    7.2500        NaN        S  [[[74,...  {40: 3...
-1            2           1       1  Cuming...  female  38.00      1      0   PC 17599   71.2833        C85        C  [[[67,...     {1: 8}
-2            3           1       3  Heikki...  female  26.00      0      0  STON/O...    7.9250        NaN        S  [[[62,...   {39: 79}
-3            4           1       1  Futrel...  female  35.00      1      0     888000   53.1000       C123        S  [[[15,...  {13: 2...
-4            5           0       3  Allen,...    male  35.00      0      0     888000    8.0500        NaN        S  [[[81,...   {60: 90}
-5            6           0       3  Moran,...    male    NaN      0      0     888000    8.4583        NaN        Q  [[[58,...    {20: 4}
-6            7           0       1  McCart...    male  54.00      0      0     888000   51.8625        E46        S  [[[28,...  {21: 8...
-7            8           0       3  Palsso...    male   2.00      3      1     888000   21.0750        NaN        S  [[[25,...  {53: 8...
-8            9           1       3  Johnso...  female  27.00      0      2     888000   11.1333        NaN        S  [[[47,...  {19: 3...
-
-
-df.shortloc_greater_replace('Cabin','C123', pd.NA)
-     PassengerId  Survived  Pclass       Name     Sex    Age  SibSp  Parch     Ticket      Fare      Cabin Embarked   listtest   dicttest
-0            1           0       3  Braund...    male  22.00      1      0  A/5 21171    7.2500        NaN        S  [[[74,...  {40: 3...
-1            2           1       1  Cuming...  female  38.00      1      0   PC 17599   71.2833       <NA>        C  [[[67,...     {1: 8}
-2            3           1       3  Heikki...  female  26.00      0      0  STON/O...    7.9250        NaN        S  [[[62,...   {39: 79}
-3            4           1       1  Futrel...  female  35.00      1      0     113803   53.1000       C123        S  [[[15,...  {13: 2...
-4            5           0       3  Allen,...    male  35.00      0      0     373450    8.0500        NaN        S  [[[81,...   {60: 90}
-5            6           0       3  Moran,...    male    NaN      0      0     330877    8.4583        NaN        Q  [[[58,...    {20: 4}
-6            7           0       1  McCart...    male  54.00      0      0      17463   51.8625       <NA>        S  [[[28,...  {21: 8...
-7            8           0       3  Palsso...    male   2.00      3      1     349909   21.0750        NaN        S  [[[25,...  {53: 8...
-
-df.shortloc_in_iter('listtest', 3)
-     PassengerId  Survived  Pclass                 Name     Sex   Age  SibSp  Parch        Ticket     Fare Cabin Embarked             listtest             dicttest
-19            20         1       3  Masselmani, Mrs....  female   NaN      0      0          2649   7.2250   NaN        C  [[[32, 3], [32, ...  {98: 75, 69: 39,...
-66            67         1       2  Nye, Mrs. (Eliza...  female  29.0      0      0    C.A. 29395  10.5000   F33        S  [[[3, 98], [3, 9...             {60: 81}
-92            93         0       1  Chaffee, Mr. Her...    male  46.0      1      0   W.E.P. 5734  61.1750   E31        S  [[[52, 3], [52, ...             {80: 25}
-106          107         1       3  Salkjelsvik, Mis...  female  21.0      0      0        343120   7.6500   NaN        S  [[[85, 3], [85, ...             {62: 49}
-120          121         0       2  Hickman, Mr. Sta...    male  21.0      2      0  S.O.C. 14879  73.5000   NaN        S  [[[40, 3], [40, ...  {28: 85, 60: 72,...
-129          130         0       3   Ekstrom, Mr. Johan    male  45.0      0      0        347061   6.9750   NaN        S  [[[3, 76], [3, 7...  {79: 2, 30: 18, ...
-132          133         0       3  Robins, Mrs. Ale...  female  47.0      1      0     A/5. 3337  14.5000   NaN        S  [[[3, 68], [3, 6...  {69: 90, 1: 23, ...
-184          185         1       3  Kink-Heilmann, M...  female   4.0      0      2        315153  22.0250   NaN        S  [[[3, 88], [3, 8...  {24: 74, 30: 11,...
-
-df.shortloc_in_iter('listtest', [3,4,10])
-     PassengerId  Survived  Pclass                 Name     Sex    Age  SibSp  Parch           Ticket      Fare        Cabin Embarked             listtest             dicttest
-19            20         1       3  Masselmani, Mrs....  female    NaN      0      0             2649    7.2250          NaN        C  [[[32, 3], [32, ...  {98: 75, 69: 39,...
-22            23         1       3  McGowan, Miss. A...  female  15.00      0      0           330923    8.0292          NaN        Q  [[[13, 4], [13, ...  {56: 86, 30: 5, ...
-27            28         0       1  Fortune, Mr. Cha...    male  19.00      3      2            19950  263.0000  C23 C25 C27        S  [[[4, 66], [4, 6...  {58: 98, 32: 55,...
-66            67         1       2  Nye, Mrs. (Eliza...  female  29.00      0      0       C.A. 29395   10.5000          F33        S  [[[3, 98], [3, 9...             {60: 81}
-74            75         1       3        Bing, Mr. Lee    male  32.00      0      0             1601   56.4958          NaN        S  [[[14, 4], [14, ...  {31: 31, 64: 38,...
-84            85         1       2  Ilett, Miss. Bertha  female  17.00      0      0       SO/C 14885   10.5000          NaN        S  [[[18, 10], [18,...  {81: 64, 10: 80,...
-
-
-df.shortloc_in_iter('dicttest', [3,4,10])
-     PassengerId  Survived  Pclass                           Name     Sex    Age  SibSp  Parch             Ticket      Fare            Cabin Embarked                       listtest                       dicttest
-5              6         0       3               Moran, Mr. James    male    NaN      0      0             330877    8.4583              NaN        Q         [[[58, 72], [58, 72]]]                        {20: 4}
-8              9         1       3  Johnson, Mrs. Oscar W (Eli...  female  27.00      0      2             347742   11.1333              NaN        S         [[[47, 12], [47, 12]]]         {19: 3, 60: 24, 9: 38}
-
-
-df.shortloc_in_iter('dicttest', [3,4,10])
-     PassengerId  Survived  Pclass                          Name     Sex   Age  SibSp  Parch         Ticket     Fare Cabin Embarked                                                           listtest                                                               dicttest
-96            97         0       1     Goldschmidt, Mr. George B    male  71.0      0      0       PC 17754  34.6542    A5        C           [[[94, 4], [94, 4], [94, 4], [94, 4], [94, 4], [94, 4]]]       {67: 92, 24: 19, 53: 40, 66: 53, 44: 81, 94: 10, 34: 63, 61: 45}
-103          104         0       3    Johansson, Mr. Gustaf Joel    male  33.0      0      0           7540   8.6542   NaN        S               [[[89, 10], [89, 10], [89, 10], [89, 10], [89, 10]]]                                        {92: 23, 32: 17, 53: 3, 98: 94}
-129          130         0       3            Ekstrom, Mr. Johan    male  45.0      0      0         347061   6.9750   NaN        S  [[[3, 76], [3, 76], [3, 76], [3, 76], [3, 76], [3, 76], [3, 76]]]   {79: 2, 30: 18, 63: 10, 62: 26, 91: 58, 11: 44, 8: 81, 6: 93, 97: 5}
-
-
-df.shortloc_in_iter_replace('dicttest', [3,4,10], 15151515)
-     PassengerId  Survived  Pclass                           Name     Sex    Age  SibSp  Parch              Ticket      Fare            Cabin Embarked                       listtest                       dicttest
-0              1         0       3        Braund, Mr. Owen Harris    male  22.00      1      0           A/5 21171    7.2500              NaN        S  [[[74, 68], [74, 68], [74,...  {40: 30, 93: 84, 24: 92, 7...
-1              2         1       1  Cumings, Mrs. John Bradley...  female  38.00      1      0            PC 17599   71.2833              C85        C  [[[67, 64], [67, 64], [67,...                         {1: 8}
-2              3         1       3         Heikkinen, Miss. Laina  female  26.00      0      0    STON/O2. 3101282    7.9250              NaN        S  [[[62, 65], [62, 65], [62,...                       {39: 79}
-3              4         1       1  Futrelle, Mrs. Jacques Hea...  female  35.00      1      0              113803   53.1000             C123        S  [[[15, 96], [15, 96], [15,...       {13: 29, 65: 59, 99: 31}
-4              5         0       3       Allen, Mr. William Henry    male  35.00      0      0              373450    8.0500              NaN        S                   [[[81, 13]]]                       {60: 90}
-5              6         0       3               Moran, Mr. James    male    NaN      0      0              330877    8.4583              NaN        Q         [[[58, 72], [58, 72]]]                       15151515
-6              7         0       1        McCarthy, Mr. Timothy J    male  54.00      0      0               17463   51.8625              E46        S  [[[28, 98], [28, 98], [28,...  {21: 8, 31: 42, 9: 40, 93:...
-7              8         0       3  Palsson, Master. Gosta Leo...    male   2.00      3      1              349909   21.0750              NaN        S  [[[25, 88], [25, 88], [25,...  {53: 83, 49: 66, 57: 95, 4...
-8              9         1       3  Johnson, Mrs. Oscar W (Eli...  female  27.00      0      2              347742   11.1333              NaN        S         [[[47, 12], [47, 12]]]                       15151515
-
-df.shortloc_isin('Embarked', ['C', 'S'])
-     PassengerId  Survived  Pclass                           Name     Sex    Age  SibSp  Parch              Ticket      Fare            Cabin Embarked                       listtest                       dicttest
-0              1         0       3        Braund, Mr. Owen Harris    male  22.00      1      0           A/5 21171    7.2500              NaN        S  [[[74, 68], [74, 68], [74,...  {40: 30, 93: 84, 24: 92, 7...
-1              2         1       1  Cumings, Mrs. John Bradley...  female  38.00      1      0            PC 17599   71.2833              C85        C  [[[67, 64], [67, 64], [67,...                         {1: 8}
-2              3         1       3         Heikkinen, Miss. Laina  female  26.00      0      0    STON/O2. 3101282    7.9250              NaN        S  [[[62, 65], [62, 65], [62,...                       {39: 79}
-3              4         1       1  Futrelle, Mrs. Jacques Hea...  female  35.00      1      0              113803   53.1000             C123        S  [[[15, 96], [15, 96], [15,...       {13: 29, 65: 59, 99: 31}
-4              5         0       3       Allen, Mr. William Henry    male  35.00      0      0              373450    8.0500              NaN        S                   [[[81, 13]]]                       {60: 90}
-6              7         0       1        McCarthy, Mr. Timothy J    male  54.00      0      0               17463   51.8625              E46        S  [[[28, 98], [28, 98], [28,...  {21: 8, 31: 42, 9: 40, 93:...
-7              8         0       3  Palsson, Master. Gosta Leo...    male   2.00      3      1              349909   21.0750              NaN        S  [[[25, 88], [25, 88], [25,...  {53: 83, 49: 66, 57: 95, 4...
-8              9         1       3  Johnson, Mrs. Oscar W (Eli...  female  27.00      0      2              347742   11.1333              NaN        S         [[[47, 12], [47, 12]]]         {19: 3, 60: 24, 9: 38}
-
-df.shortloc_isin_replace('Embarked', ['C', 'S'], 'CCCCCCCCCCCCCCCCCCCSSSSSSSSSSSSSSSSSSSSSSSSSSSSS')
-     PassengerId  Survived  Pclass       Name     Sex    Age  SibSp  Parch     Ticket      Fare      Cabin   Embarked   listtest   dicttest
-0            1           0       3  Braund...    male  22.00      1      0  A/5 21171    7.2500        NaN  CCCCCC...  [[[74,...  {40: 3...
-1            2           1       1  Cuming...  female  38.00      1      0   PC 17599   71.2833        C85  CCCCCC...  [[[67,...     {1: 8}
-2            3           1       3  Heikki...  female  26.00      0      0  STON/O...    7.9250        NaN  CCCCCC...  [[[62,...   {39: 79}
-3            4           1       1  Futrel...  female  35.00      1      0     113803   53.1000       C123  CCCCCC...  [[[15,...  {13: 2...
-4            5           0       3  Allen,...    male  35.00      0      0     373450    8.0500        NaN  CCCCCC...  [[[81,...   {60: 90}
-5            6           0       3  Moran,...    male    NaN      0      0     330877    8.4583        NaN          Q  [[[58,...    {20: 4}
-
-
-df.shortloc_isna('Age')
-     PassengerId  Survived  Pclass                           Name     Sex  Age  SibSp  Parch              Ticket      Fare  Cabin Embarked                       listtest                       dicttest
-5              6         0       3               Moran, Mr. James    male  NaN      0      0              330877    8.4583    NaN        Q         [[[25, 39], [25, 39]]]       {97: 78, 85: 88, 42: 34}
-17            18         1       2   Williams, Mr. Charles Eugene    male  NaN      0      0              244373   13.0000    NaN        S  [[[17, 6], [17, 6], [17, 6...                 {41: 6, 2: 82}
-19            20         1       3        Masselmani, Mrs. Fatima  female  NaN      0      0                2649    7.2250    NaN        C  [[[11, 37], [11, 37], [11,...  {43: 73, 50: 28, 38: 47, 4...
-26            27         0       3        Emir, Mr. Farred Chehab    male  NaN      0      0                2631    7.2250    NaN        C  [[[48, 66], [48, 66], [48,...               {33: 45, 82: 90}
-28            29         1       3  O'Dwyer, Miss. Ellen "Nellie"  female  NaN      0      0              330959    7.8792    NaN        Q           [[[3, 53], [3, 53]]]               {29: 90, 84: 86}
-29            30         0       3            Todoroff, Mr. Lalio    male  NaN      0      0              349216    7.8958    NaN        S  [[[67, 3], [67, 3], [67, 3...  {57: 49, 23: 71, 64: 45, 1...
-31            32         1       1  Spencer, Mrs. William Augu...  female  NaN      1      0            PC 17569  146.5208    B78        C  [[[88, 94], [88, 94], [88,...  {4: 42, 98: 58, 94: 7, 39:...
-
-
-df.shortloc_isna_replace('Age',16541)
-     PassengerId  Survived  Pclass                           Name     Sex       Age  SibSp  Parch              Ticket      Fare            Cabin Embarked                       listtest                       dicttest
-0              1         0       3        Braund, Mr. Owen Harris    male     22.00      1      0           A/5 21171    7.2500              NaN        S  [[[27, 71], [27, 71], [27,...  {36: 67, 73: 54, 56: 48, 8...
-1              2         1       1  Cumings, Mrs. John Bradley...  female     38.00      1      0            PC 17599   71.2833              C85        C  [[[31, 68], [31, 68], [31,...                        {9: 77}
-2              3         1       3         Heikkinen, Miss. Laina  female     26.00      0      0    STON/O2. 3101282    7.9250              NaN        S                   [[[31, 23]]]  {49: 6, 76: 22, 52: 18, 6:...
-3              4         1       1  Futrelle, Mrs. Jacques Hea...  female     35.00      1      0              113803   53.1000             C123        S  [[[96, 48], [96, 48], [96,...  {27: 90, 9: 38, 18: 94, 67...
-4              5         0       3       Allen, Mr. William Henry    male     35.00      0      0              373450    8.0500              NaN        S  [[[60, 84], [60, 84], [60,...  {8: 61, 37: 4, 25: 43, 21:...
-5              6         0       3               Moran, Mr. James    male  16541.00      0      0              330877    8.4583              NaN        Q         [[[25, 39], [25, 39]]]       {97: 78, 85: 88, 42: 34}
-6              7         0       1        McCarthy, Mr. Timothy J    male     54.00      0      0               17463   51.8625              E46        S  [[[76, 5], [76, 5], [76, 5...  {56: 51, 13: 24, 84: 24, 9...
-
-df.shortloc_less('Ticket', 7534)
-
-     PassengerId  Survived  Pclass                           Name     Sex    Age  SibSp  Parch Ticket     Fare        Cabin Embarked                       listtest                       dicttest
-19            20         1       3        Masselmani, Mrs. Fatima  female    NaN      0      0   2649   7.2250          NaN        C  [[[11, 37], [11, 37], [11,...  {43: 73, 50: 28, 38: 47, 4...
-26            27         0       3        Emir, Mr. Farred Chehab    male    NaN      0      0   2631   7.2250          NaN        C  [[[48, 66], [48, 66], [48,...               {33: 45, 82: 90}
-36            37         1       3               Mamee, Mr. Hanna    male    NaN      0      0   2677   7.2292          NaN        C  [[[84, 24], [84, 24], [84,...  {39: 19, 88: 50, 23: 7, 53...
-39            40         1       3    Nicola-Yarred, Miss. Jamila  female  14.00      1      0   2651  11.2417          NaN        C  [[[20, 72], [20, 72], [20,...  {72: 91, 81: 15, 89: 24, 9...
-48            49         0       3            Samaan, Mr. Youssef    male    NaN      2      0   2662  21.6792          NaN        C  [[[79, 85], [79, 85], [79,...                       {35: 61}
-53            54         1       2  Faunthorpe, Mrs. Lizzie (E...  female  29.00      1      0   2926  26.0000          NaN        S         [[[62, 79], [62, 79]]]  {36: 53, 38: 70, 6: 1, 89:...
-57            58         0       3            Novel, Mr. Mansouer    male  28.50      0      0   2697   7.2292          NaN        C         [[[86, 78], [86, 78]]]                {28: 5, 49: 22}
-60            61         0       3          Sirayanian, Mr. Orsen    male  22.00      0      0   2669   7.2292          NaN        C                   [[[24, 72]]]  {74: 59, 16: 44, 30: 17, 5...
-65            66         1       3       Moubarek, Master. Gerios    male    NaN      1      1   2661  15.2458          NaN        C  [[[56, 96], [56, 96], [56,...  {5: 34, 59: 97, 78: 15, 76...
-73            74         0       3    Chronopoulos, Mr. Apostolos    male  26.00      1      0   2680  14.4542          NaN        C         [[[78, 24], [78, 24]]]  {96: 26, 87: 73, 58: 49, 3...
-74            75         1       3                  Bing, Mr. Lee    male  32.00      0      0   1601  56.4958          NaN        S  [[[86, 20], [86, 20], [86,...  {84: 87, 18: 40, 17: 28, 7...
-
-
-df.shortloc_less_replace('Age', 30, 'less 30')
-     PassengerId  Survived  Pclass                           Name     Sex      Age  SibSp  Parch              Ticket      Fare            Cabin Embarked                       listtest                       dicttest
-0              1         0       3        Braund, Mr. Owen Harris    male  less 30      1      0           A/5 21171    7.2500              NaN        S  [[[27, 71], [27, 71], [27,...  {36: 67, 73: 54, 56: 48, 8...
-1              2         1       1  Cumings, Mrs. John Bradley...  female     38.0      1      0            PC 17599   71.2833              C85        C  [[[31, 68], [31, 68], [31,...                        {9: 77}
-2              3         1       3         Heikkinen, Miss. Laina  female  less 30      0      0    STON/O2. 3101282    7.9250              NaN        S                   [[[31, 23]]]  {49: 6, 76: 22, 52: 18, 6:...
-3              4         1       1  Futrelle, Mrs. Jacques Hea...  female     35.0      1      0              113803   53.1000             C123        S  [[[96, 48], [96, 48], [96,...  {27: 90, 9: 38, 18: 94, 67...
-
-
-df.shortloc_less_or_equal_replace('Survived', 0, 'DEAD')
-     PassengerId Survived  Pclass                           Name     Sex    Age  SibSp  Parch              Ticket      Fare            Cabin Embarked                       listtest                       dicttest
-0              1     DEAD       3        Braund, Mr. Owen Harris    male  22.00      1      0           A/5 21171    7.2500              NaN        S  [[[27, 71], [27, 71], [27,...  {36: 67, 73: 54, 56: 48, 8...
-1              2        1       1  Cumings, Mrs. John Bradley...  female  38.00      1      0            PC 17599   71.2833              C85        C  [[[31, 68], [31, 68], [31,...                        {9: 77}
-2              3        1       3         Heikkinen, Miss. Laina  female  26.00      0      0    STON/O2. 3101282    7.9250              NaN        S                   [[[31, 23]]]  {49: 6, 76: 22, 52: 18, 6:...
-3              4        1       1  Futrelle, Mrs. Jacques Hea...  female  35.00      1      0              113803   53.1000             C123        S  [[[96, 48], [96, 48], [96,...  {27: 90, 9: 38, 18: 94, 67...
-4              5     DEAD       3       Allen, Mr. William Henry    male  35.00      0      0              373450    8.0500              NaN        S  [[[60, 84], [60, 84], [60,...  {8: 61, 37: 4, 25: 43, 21:...
-5              6     DEAD       3               Moran, Mr. James    male    NaN      0      0              330877    8.4583              NaN        Q         [[[25, 39], [25, 39]]]       {97: 78, 85: 88, 42: 34}
-6              7     DEAD       1        McCarthy, Mr. Timothy J    male  54.00      0      0               17463   51.8625              E46        S  [[[76, 5], [76, 5], [76, 5...  {56: 51, 13: 24, 84: 24, 9...
-7              8     DEAD       3  Palsson, Master. Gosta Leo...    male   2.00      3      1              349909   21.0750              NaN        S  [[[42, 52], [42, 52], [42,...               {71: 69, 44: 14}
-
-
-
-df.shortloc_not_equal_replace('Survived', 0, True)
-     PassengerId Survived  Pclass                           Name     Sex    Age  SibSp  Parch              Ticket      Fare            Cabin Embarked                       listtest                       dicttest
-0              1        0       3        Braund, Mr. Owen Harris    male  22.00      1      0           A/5 21171    7.2500              NaN        S  [[[27, 71], [27, 71], [27,...  {36: 67, 73: 54, 56: 48, 8...
-1              2     True       1  Cumings, Mrs. John Bradley...  female  38.00      1      0            PC 17599   71.2833              C85        C  [[[31, 68], [31, 68], [31,...                        {9: 77}
-2              3     True       3         Heikkinen, Miss. Laina  female  26.00      0      0    STON/O2. 3101282    7.9250              NaN        S                   [[[31, 23]]]  {49: 6, 76: 22, 52: 18, 6:...
-3              4     True       1  Futrelle, Mrs. Jacques Hea...  female  35.00      1      0              113803   53.1000             C123        S  [[[96, 48], [96, 48], [96,...  {27: 90, 9: 38, 18: 94, 67...
-4              5        0       3       Allen, Mr. William Henry    male  35.00      0      0              373450    8.0500              NaN        S  [[[60, 84], [60, 84], [60,...  {8: 61, 37: 4, 25: 43, 21:...
-5              6        0       3               Moran, Mr. James    male    NaN      0      0              330877    8.4583              NaN        Q         [[[25, 39], [25, 39]]]       {97: 78, 85: 88, 42: 34}
-
-
-
-df.shortloc_not_in_iter('listtest', list(range(0,90)))
-     PassengerId  Survived  Pclass                           Name     Sex   Age  SibSp  Parch      Ticket      Fare Cabin Embarked                       listtest                       dicttest
-832          833         0       3                 Saad, Mr. Amin    male   NaN      0      0        2671    7.2292   NaN        C  [[[95, 94], [95, 94], [95,...                {82: 66, 84: 5}
-484          485         1       1        Bishop, Mr. Dickinson H    male  25.0      1      0       11967   91.0792   B49        C  [[[97, 92], [97, 92], [97,...  {20: 34, 2: 23, 98: 37, 1:...
-581          582         1       1  Thayer, Mrs. John Borland ...  female  39.0      1      1       17421  110.8833   C68        C         [[[91, 90], [91, 90]]]  {48: 98, 3: 98, 93: 4, 97:...
-336          337         0       1      Pears, Mr. Thomas Clinton    male  29.0      1      0      113776   66.6000    C2        S         [[[90, 98], [90, 98]]]                         {6: 7}
-116          117         0       3           Connors, Mr. Patrick    male  70.5      0      0      370369    7.7500   NaN        Q  [[[92, 99], [92, 99], [92,...  {60: 79, 75: 71, 28: 68, 5...
-52            53         1       1  Harper, Mrs. Henry Sleeper...  female  49.0      1      0    PC 17572   76.7292   D33        C  [[[96, 94], [96, 94], [96,...  {20: 53, 93: 11, 83: 79, 5...
-439          440         0       2  Kvillner, Mr. Johan Henrik...    male  31.0      0      0  C.A. 18723   10.5000   NaN        S  [[[95, 98], [95, 98], [95,...  {58: 11, 89: 23, 22: 66, 1...
-56            57         1       2              Rugg, Miss. Emily  female  21.0      0      0  C.A. 31026   10.5000   NaN        S  [[[92, 92], [92, 92], [92,...                {45: 1, 37: 98}
-
-
-
-df.shortloc_not_in_iter_replace('listtest', list(range(0,20)), 27)
-     PassengerId  Survived  Pclass                           Name     Sex    Age  SibSp  Parch              Ticket      Fare            Cabin Embarked                       listtest                       dicttest
-0              1         0       3        Braund, Mr. Owen Harris    male  22.00      1      0           A/5 21171    7.2500              NaN        S                             27  {36: 67, 73: 54, 56: 48, 8...
-1              2         1       1  Cumings, Mrs. John Bradley...  female  38.00      1      0            PC 17599   71.2833              C85        C                             27                        {9: 77}
-2              3         1       3         Heikkinen, Miss. Laina  female  26.00      0      0    STON/O2. 3101282    7.9250              NaN        S                             27  {49: 6, 76: 22, 52: 18, 6:...
-3              4         1       1  Futrelle, Mrs. Jacques Hea...  female  35.00      1      0              113803   53.1000             C123        S                             27  {27: 90, 9: 38, 18: 94, 67...
-4              5         0       3       Allen, Mr. William Henry    male  35.00      0      0              373450    8.0500              NaN        S                             27  {8: 61, 37: 4, 25: 43, 21:...
-5              6         0       3               Moran, Mr. James    male    NaN      0      0              330877    8.4583              NaN        Q                             27       {97: 78, 85: 88, 42: 34}
-6              7         0       1        McCarthy, Mr. Timothy J    male  54.00      0      0               17463   51.8625              E46        S  [[[76, 5], [76, 5], [76, 5...  {56: 51, 13: 24, 84: 24, 9...
-
-
-df.shortloc_regex('Fare', r'^\d?7\.').to_string(max_colwidth=30)
-     PassengerId  Survived  Pclass                           Name     Sex   Age  SibSp  Parch              Ticket     Fare  Cabin Embarked                       listtest                       dicttest
-0              1         0       3        Braund, Mr. Owen Harris    male  22.0      1      0           A/5 21171   7.2500    NaN        S  [[[27, 71], [27, 71], [27,...  {36: 67, 73: 54, 56: 48, 8...
-2              3         1       3         Heikkinen, Miss. Laina  female  26.0      0      0    STON/O2. 3101282   7.9250    NaN        S                   [[[31, 23]]]  {49: 6, 76: 22, 52: 18, 6:...
-14            15         0       3  Vestrom, Miss. Hulda Amand...  female  14.0      0      0              350406   7.8542    NaN        S  [[[40, 57], [40, 57], [40,...  {54: 39, 8: 35, 76: 84, 20...
-19            20         1       3        Masselmani, Mrs. Fatima  female   NaN      0      0                2649   7.2250    NaN        C  [[[11, 37], [11, 37], [11,...  {43: 73, 50: 28, 38: 47, 4...
-26            27         0       3        Emir, Mr. Farred Chehab    male   NaN      0      0                2631   7.2250    NaN        C  [[[48, 66], [48, 66], [48,...               {33: 45, 82: 90}
-28            29         1       3  O'Dwyer, Miss. Ellen "Nellie"  female   NaN      0      0              330959   7.8792    NaN        Q           [[[3, 53], [3, 53]]]               {29: 90, 84: 86}
-29            30         0       3            Todoroff, Mr. Lalio    male   NaN      0      0              349216   7.8958    NaN        S  [[[67, 3], [67, 3], [67, 3...  {57: 49, 23: 71, 64: 45, 1...
-30            31         0       1       Uruchurtu, Don. Manuel E    male  40.0      0      0            PC 17601  27.7208    NaN        C  [[[91, 32], [91, 32], [91,...         {1: 29, 54: 93, 96: 7}
-
-
-
-df.shortloc_not_regex('Fare', r'^\d?7\.').to_string(max_colwidth=30)
-     PassengerId  Survived  Pclass                           Name     Sex    Age  SibSp  Parch             Ticket      Fare            Cabin Embarked                       listtest                       dicttest
-1              2         1       1  Cumings, Mrs. John Bradley...  female  38.00      1      0           PC 17599   71.2833              C85        C  [[[31, 68], [31, 68], [31,...                        {9: 77}
-3              4         1       1  Futrelle, Mrs. Jacques Hea...  female  35.00      1      0             113803   53.1000             C123        S  [[[96, 48], [96, 48], [96,...  {27: 90, 9: 38, 18: 94, 67...
-4              5         0       3       Allen, Mr. William Henry    male  35.00      0      0             373450    8.0500              NaN        S  [[[60, 84], [60, 84], [60,...  {8: 61, 37: 4, 25: 43, 21:...
-5              6         0       3               Moran, Mr. James    male    NaN      0      0             330877    8.4583              NaN        Q         [[[25, 39], [25, 39]]]       {97: 78, 85: 88, 42: 34}
-6              7         0       1        McCarthy, Mr. Timothy J    male  54.00      0      0              17463   51.8625              E46        S  [[[76, 5], [76, 5], [76, 5...  {56: 51, 13: 24, 84: 24, 9...
-7              8         0       3  Palsson, Master. Gosta Leo...    male   2.00      3      1             349909   21.0750              NaN        S  [[[42, 52], [42, 52], [42,...               {71: 69, 44: 14}
-8              9         1       3  Johnson, Mrs. Oscar W (Eli...  female  27.00      0      2             347742   11.1333              NaN        S  [[[92, 21], [92, 21], [92,...  {61: 17, 72: 44, 81: 74, 3...
-9             10         1       2  Nasser, Mrs. Nicholas (Ade...  female  14.00      1      0             237736   30.0708              NaN        C  [[[88, 97], [88, 97], [88,...                       {69: 43}
-
-
-df.shortloc_str('Pclass', r'3').to_string(max_colwidth=30)
-     PassengerId  Survived  Pclass                           Name     Sex    Age  SibSp  Parch              Ticket     Fare  Cabin Embarked                       listtest                       dicttest
-0              1         0       3        Braund, Mr. Owen Harris    male  22.00      1      0           A/5 21171   7.2500    NaN        S  [[[27, 71], [27, 71], [27,...  {36: 67, 73: 54, 56: 48, 8...
-2              3         1       3         Heikkinen, Miss. Laina  female  26.00      0      0    STON/O2. 3101282   7.9250    NaN        S                   [[[31, 23]]]  {49: 6, 76: 22, 52: 18, 6:...
-4              5         0       3       Allen, Mr. William Henry    male  35.00      0      0              373450   8.0500    NaN        S  [[[60, 84], [60, 84], [60,...  {8: 61, 37: 4, 25: 43, 21:...
-5              6         0       3               Moran, Mr. James    male    NaN      0      0              330877   8.4583    NaN        Q         [[[25, 39], [25, 39]]]       {97: 78, 85: 88, 42: 34}
-7              8         0       3  Palsson, Master. Gosta Leo...    male   2.00      3      1              349909  21.0750    NaN        S  [[[42, 52], [42, 52], [42,...               {71: 69, 44: 14}
-8              9         1       3  Johnson, Mrs. Oscar W (Eli...  female  27.00      0      2              347742  11.1333    NaN        S  [[[92, 21], [92, 21], [92,...  {61: 17, 72: 44, 81: 74, 3...
-10            11         1       3  Sandstrom, Miss. Marguerit...  female   4.00      1      1             PP 9549  16.7000     G6        S  [[[28, 63], [28, 63], [28,...  {12: 80, 63: 96, 79: 99, 5...
-12            13         0       3  Saundercock, Mr. William H...    male  20.00      0      0           A/5. 2151   8.0500    NaN        S  [[[34, 91], [34, 91], [34,...  {42: 68, 46: 90, 66: 96, 3...
-13            14         0       3    Andersson, Mr. Anders Johan    male  39.00      1      5              347082  31.2750    NaN        S  [[[3, 47], [3, 47], [3, 47...  {94: 60, 73: 33, 59: 32, 3...
-14            15         0       3  Vestrom, Miss. Hulda Amand...  female  14.00      0      0              350406   7.8542    NaN        S  [[[40, 57], [40, 57], [40,...  {54: 39, 8: 35, 76: 84, 20...
-16            17         0       3           Rice, Master. Eugene    male   2.00      4      1              382652  29.1250    NaN        Q  [[[24, 8], [24, 8], [24, 8...  {20: 91, 56: 55, 11: 16, 3...
-
-
-
-df.shortloc_str_replace('Pclass', r'3',4).to_string(max_colwidth=30)
-     PassengerId  Survived  Pclass                           Name     Sex    Age  SibSp  Parch              Ticket      Fare            Cabin Embarked                       listtest                       dicttest
-0              1         0       4        Braund, Mr. Owen Harris    male  22.00      1      0           A/5 21171    7.2500              NaN        S  [[[27, 71], [27, 71], [27,...  {36: 67, 73: 54, 56: 48, 8...
-1              2         1       1  Cumings, Mrs. John Bradley...  female  38.00      1      0            PC 17599   71.2833              C85        C  [[[31, 68], [31, 68], [31,...                        {9: 77}
-2              3         1       4         Heikkinen, Miss. Laina  female  26.00      0      0    STON/O2. 3101282    7.9250              NaN        S                   [[[31, 23]]]  {49: 6, 76: 22, 52: 18, 6:...
-3              4         1       1  Futrelle, Mrs. Jacques Hea...  female  35.00      1      0              113803   53.1000             C123        S  [[[96, 48], [96, 48], [96,...  {27: 90, 9: 38, 18: 94, 67...
-4              5         0       4       Allen, Mr. William Henry    male  35.00      0      0              373450    8.0500              NaN        S  [[[60, 84], [60, 84], [60,...  {8: 61, 37: 4, 25: 43, 21:...
-5              6         0       4               Moran, Mr. James    male    NaN      0      0              330877    8.4583              NaN        Q         [[[25, 39], [25, 39]]]       {97: 78, 85: 88, 42: 34}
-6              7         0       1        McCarthy, Mr. Timothy J    male  54.00      0      0               17463   51.8625              E46        S  [[[76, 5], [76, 5], [76, 5...  {56: 51, 13: 24, 84: 24, 9...
-7              8         0       4  Palsson, Master. Gosta Leo...    male   2.00      3      1              349909   21.0750              NaN        S  [[[42, 52], [42, 52], [42,...               {71: 69, 44: 14}
-8              9         1       4  Johnson, Mrs. Oscar W (Eli...  female  27.00      0      2              347742   11.1333              NaN        S  [[[92, 21], [92, 21], [92,...  {61: 17, 72: 44, 81: 74, 3...
-9             10         1       2  Nasser, Mrs. Nicholas (Ade...  female  14.00      1      0              237736   30.0708              NaN        C  [[[88, 97], [88, 97], [88,...                       {69: 43}
-10            11         1       4  Sandstrom, Miss. Marguerit...  female   4.00      1      1             PP 9549   16.7000               G6        S  [[[28, 63], [28, 63], [28,...  {12: 80, 63: 96, 79: 99, 5...
-
-
-
-
-df.loc_positive_and(
-   ("Pclass", "==", 3),
-   ("Sex", "!=", "male"),
-   ("Age", ">=", 1),
-   ("Pclass", ">=", 3),
-   ("listtest", "in_iter", [11, 22, 33, 44, 55, 66, 77, 88, 99]),
-   ("Sex", "in", ["female", "male"]),
-   ("Name", "re", r"Miss\."),
-   ("Ticket", ">", 5000),
-   ("Embarked", "str", "S"),
-)
-
-     PassengerId  Survived  Pclass                           Name     Sex   Age  SibSp  Parch  Ticket     Fare Cabin Embarked                       listtest                       dicttest
-24            25         0       3  Palsson, Miss. Torborg Danira  female   8.0      3      1  349909  21.0750   NaN        S  [[[44, 33], [44, 33], [44,...  {98: 85, 8: 23, 21: 77, 85...
-141          142         1       3       Nysten, Miss. Anna Sofia  female  22.0      0      0  347081   7.7500   NaN        S                   [[[44, 30]]]  {25: 15, 24: 14, 16: 26, 5...
-192          193         1       3  Andersen-Jensen, Miss. Car...  female  19.0      1      0  350046   7.8542   NaN        S  [[[39, 55], [39, 55], [39,...  {1: 44, 16: 59, 80: 13, 81...
-634          635         0       3             Skoog, Miss. Mabel  female   9.0      3      2  347088  27.9000   NaN        S                   [[[11, 22]]]                        {40: 7}
-
-
-
-df.loc_positive_and(('Ticket','==', 373450), ('Pclass','==', 3))
-   PassengerId  Survived  Pclass                      Name   Sex   Age  SibSp  Parch  Ticket  Fare Cabin Embarked                       listtest                       dicttest
-4            5         0       3  Allen, Mr. William Henry  male  35.0      0      0  373450  8.05   NaN        S  [[[60, 84], [60, 84], [60,...  {8: 61, 37: 4, 25: 43, 21:...
-
-
-df.loc_positive_or(('Ticket','==', 373450), ('Pclass','==', 3))
-     PassengerId  Survived  Pclass                           Name     Sex    Age  SibSp  Parch              Ticket     Fare  Cabin Embarked                       listtest                       dicttest
-0              1         0       3        Braund, Mr. Owen Harris    male  22.00      1      0           A/5 21171   7.2500    NaN        S  [[[27, 71], [27, 71], [27,...  {36: 67, 73: 54, 56: 48, 8...
-2              3         1       3         Heikkinen, Miss. Laina  female  26.00      0      0    STON/O2. 3101282   7.9250    NaN        S                   [[[31, 23]]]  {49: 6, 76: 22, 52: 18, 6:...
-4              5         0       3       Allen, Mr. William Henry    male  35.00      0      0              373450   8.0500    NaN        S  [[[60, 84], [60, 84], [60,...  {8: 61, 37: 4, 25: 43, 21:...
-5              6         0       3               Moran, Mr. James    male    NaN      0      0              330877   8.4583    NaN        Q         [[[25, 39], [25, 39]]]       {97: 78, 85: 88, 42: 34}
-7              8         0       3  Palsson, Master. Gosta Leo...    male   2.00      3      1              349909  21.0750    NaN        S  [[[42, 52], [42, 52], [42,...               {71: 69, 44: 14}
-
-
-
-df.loc_positive_and(('Age','>=', 13), ('Age','<=', 19))
-     PassengerId  Survived  Pclass                           Name     Sex   Age  SibSp  Parch             Ticket      Fare            Cabin Embarked                       listtest                       dicttest
-9             10         1       2  Nasser, Mrs. Nicholas (Ade...  female  14.0      1      0             237736   30.0708              NaN        C  [[[88, 97], [88, 97], [88,...                       {69: 43}
-14            15         0       3  Vestrom, Miss. Hulda Amand...  female  14.0      0      0             350406    7.8542              NaN        S  [[[40, 57], [40, 57], [40,...  {54: 39, 8: 35, 76: 84, 20...
-22            23         1       3    McGowan, Miss. Anna "Annie"  female  15.0      0      0             330923    8.0292              NaN        Q  [[[85, 85], [85, 85], [85,...  {80: 2, 70: 5, 27: 24, 10:...
-27            28         0       1  Fortune, Mr. Charles Alexa...    male  19.0      3      2              19950  263.0000      C23 C25 C27        S  [[[7, 96], [7, 96], [7, 96...  {60: 4, 22: 96, 55: 28, 97...
-38            39         0       3  Vander Planke, Miss. Augus...  female  18.0      2      0             345764   18.0000              NaN        S  [[[82, 50], [82, 50], [82,...  {70: 41, 90: 86, 46: 95, 3...
-39            40         1       3    Nicola-Yarred, Miss. Jamila  female  14.0      1      0               2651   11.2417              NaN        C  [[[20, 72], [20, 72], [20,...  {72: 91, 81: 15, 89: 24, 9...
-44            45         1       3  Devaney, Miss. Margaret Delia  female  19.0      0      0             330958    7.8792              NaN        Q  [[[97, 1], [97, 1], [97, 1...  {89: 44, 58: 86, 48: 54, 9...
-49            50         0       3  Arnold-Franchi, Mrs. Josef...  female  18.0      1      0             349237   17.8000              NaN        S         [[[64, 68], [64, 68]]]  {67: 59, 96: 34, 8: 64, 45...
-67            68         0       3       Crease, Mr. Ernest James    male  19.0      0      0          S.P. 3464    8.1583              NaN        S  [[[30, 77], [30, 77], [30,...  {37: 56, 52: 5, 80: 12, 86...
-
-
-
-df.loc_positive_and(('Ticket','!=', 373450), ('Pclass','!=', 3))
-     PassengerId  Survived  Pclass                           Name     Sex    Age  SibSp  Parch            Ticket      Fare            Cabin Embarked                       listtest                       dicttest
-1              2         1       1  Cumings, Mrs. John Bradley...  female  38.00      1      0          PC 17599   71.2833              C85        C  [[[31, 68], [31, 68], [31,...                        {9: 77}
-3              4         1       1  Futrelle, Mrs. Jacques Hea...  female  35.00      1      0            113803   53.1000             C123        S  [[[96, 48], [96, 48], [96,...  {27: 90, 9: 38, 18: 94, 67...
-6              7         0       1        McCarthy, Mr. Timothy J    male  54.00      0      0             17463   51.8625              E46        S  [[[76, 5], [76, 5], [76, 5...  {56: 51, 13: 24, 84: 24, 9...
-9             10         1       2  Nasser, Mrs. Nicholas (Ade...  female  14.00      1      0            237736   30.0708              NaN        C  [[[88, 97], [88, 97], [88,...                       {69: 43}
-11            12         1       1       Bonnell, Miss. Elizabeth  female  58.00      0      0            113783   26.5500             C103        S         [[[66, 84], [66, 84]]]  {87: 7, 75: 62, 84: 22, 94...
-15            16         1       2  Hewlett, Mrs. (Mary D King...  female  55.00      0      0            248706   16.0000              NaN        S  [[[93, 7], [93, 7], [93, 7...  {17: 96, 7: 68, 74: 5, 97:...
-
-
-df.loc_negative_and(('Age','>=', 13), ('Sex','str', 'female'))
-     PassengerId  Survived  Pclass                           Name   Sex    Age  SibSp  Parch           Ticket      Fare    Cabin Embarked                       listtest                       dicttest
-386          387         0       3  Goodwin, Master. Sidney Le...  male   1.00      5      2          CA 2144   46.9000      NaN        S  [[[32, 26], [32, 26], [32,...  {42: 33, 97: 56, 33: 73, 7...
-261          262         1       3  Asplund, Master. Edvin Roj...  male   3.00      4      2           347077   31.3875      NaN        S  [[[40, 73], [40, 73], [40,...  {7: 23, 93: 3, 18: 66, 96:...
-7              8         0       3  Palsson, Master. Gosta Leo...  male   2.00      3      1           349909   21.0750      NaN        S  [[[42, 52], [42, 52], [42,...               {71: 69, 44: 14}
-16            17         0       3           Rice, Master. Eugene  male   2.00      4      1           382652   29.1250      NaN        Q  [[[24, 8], [24, 8], [24, 8...  {20: 91, 56: 55, 11: 16, 3...
-787          788         0       3      Rice, Master. George Hugh  male   8.00      4      1           382652   29.1250      NaN        Q  [[[32, 90], [32, 90], [32,...  {5: 17, 83: 1, 82: 16, 21:...
-788          789         1       3     Dean, Master. Bertram Vere  male   1.00      1      2        C.A. 2315   20.5750      NaN        S  [[[27, 72], [27, 72], [27,...       {58: 65, 42: 92, 61: 72}
-278          279         0       3             Rice, Master. Eric  male   7.00      4      1           382652   29.1250      NaN        Q  [[[48, 59], [48, 59], [48,...  {16: 64, 97: 83, 66: 91, 9...
-
-
-
-df.shortloc_regex('Name', '^Ab').shortloc_not_equal('Sex', 'male').shortloc_equal('Age', 35)
-     PassengerId  Survived  Pclass                           Name     Sex   Age  SibSp  Parch     Ticket   Fare Cabin Embarked                       listtest                       dicttest
-279          280         1       3  Abbott, Mrs. Stanton (Rosa...  female  35.0      1      1  C.A. 2673  20.25   NaN        S  [[[93, 85], [93, 85], [93,...  {37: 16, 68: 58, 42: 7, 20...
-
-
-
-df.shortloc_in_iter('dicttest', 65).shortloc_not_in_iter('listtest', [77,65,80,83])
-     PassengerId  Survived  Pclass                           Name     Sex   Age  SibSp  Parch       Ticket      Fare        Cabin Embarked                       listtest                       dicttest
-515          516         0       1   Walker, Mr. William Anderson    male  47.0      0      0        36967   34.0208          D46        S  [[[55, 13], [55, 13], [55,...  {67: 25, 73: 76, 93: 74, 6...
-772          773         0       2              Mack, Mrs. (Mary)  female  57.0      0      0  S.O./P.P. 3   10.5000          E77        S  [[[3, 67], [3, 67], [3, 67...  {20: 62, 88: 78, 22: 65, 1...
-518          519         1       2  Angle, Mrs. William A (Flo...  female  36.0      1      0       226875   26.0000          NaN        S         [[[78, 94], [78, 94]]]  {32: 53, 48: 66, 20: 5, 67...
-10            11         1       3  Sandstrom, Miss. Marguerit...  female   4.0      1      1      PP 9549   16.7000           G6        S  [[[28, 63], [28, 63], [28,...  {12: 80, 63: 96, 79: 99, 5...
-275          276         1       1  Andrews, Miss. Kornelia Th...  female  63.0      1      0        13502   77.9583           D7        S                   [[[84, 21]]]  {31: 95, 27: 48, 89: 25, 6...
-788          789         1       3     Dean, Master. Bertram Vere    male   1.0      1      2    C.A. 2315   20.5750          NaN        S  [[[27, 72], [27, 72], [27,...       {58: 65, 42: 92, 61: 72}
-
-
-
-df.shortloc_not_isna("Cabin").shortloc_str("Cabin", "C").shortloc_not_regex(
-   "Cabin", "^.{4,}$"
-)
-     PassengerId  Survived  Pclass                           Name     Sex   Age  SibSp  Parch    Ticket      Fare Cabin Embarked                       listtest                       dicttest
-1              2         1       1  Cumings, Mrs. John Bradley...  female  38.0      1      0  PC 17599   71.2833   C85        C  [[[31, 68], [31, 68], [31,...                        {9: 77}
-269          270         1       1         Bissette, Miss. Amelia  female  35.0      0      0  PC 17760  135.6333   C99        S  [[[89, 54], [89, 54], [89,...  {50: 9, 91: 60, 30: 67, 46...
-527          528         0       1             Farthing, Mr. John    male   NaN      0      0  PC 17483  221.7792   C95        S  [[[9, 72], [9, 72], [9, 72...               {41: 24, 63: 10}
-151          152         1       1  Pears, Mrs. Thomas (Edith ...  female  22.0      1      0    113776   66.6000    C2        S  [[[24, 98], [24, 98], [24,...  {80: 92, 25: 89, 32: 82, 1...
-412          413         1       1         Minahan, Miss. Daisy E  female  33.0      1      0     19928   90.0000   C78        Q                    [[[2, 41]]]                       {57: 41}
-544          545         0       1     Douglas, Mr. Walter Donald    male  50.0      1      0  PC 17761  106.4250   C86        C  [[[55, 21], [55, 21], [55,...               {51: 49, 16: 20}
-550          551         1       1    Thayer, Mr. John Borland Jr    male  17.0      0      2     17421  110.8833   C70        C  [[[37, 20], [37, 20], [37,...               {17: 85, 49: 77}
-430          431         1       1  Bjornstrom-Steffansson, Mr...    male  28.0      0      0    110564   26.5500   C52        S  [[[14, 61], [14, 61], [14,...                       {62: 40}
-
-
-df.shortloc_in_iter('listtest',[99, 77]).shortloc_regex('listtest',r"7\b,\s*\b9"))
-     PassengerId  Survived  Pclass                  Name     Sex   Age  SibSp  Parch Ticket     Fare Cabin Embarked                       listtest                       dicttest
-111          112         0       3  Zabour, Miss. Hileni  female  14.5      1      0   2665  14.4542   NaN        C  [[[27, 99], [27, 99], [27,...  {76: 81, 62: 60, 98: 43, 5...
-
-
-#all methods can also be used against Series
-#Two examples
-
-df.Pclass.shortloc_regex('^2$')
-Out[54]: 
-9      2
-15     2
-17     2
-20     2
-21     2
-      ..
-
-df.Pclass.shortloc_regex_replace('^3$',2000)
-Out[56]: 
-0      2000
-1         1
-2      2000
-3         1
-4      2000
-       ... 
+Search and replace values with df.loc without Exceptions due to dtype incompatibility.  If the dtypes of 2 variables don't match, they will be converted until they match. 
+
+```python
+pip install a_pandas_ex_easy_loc
+```
+
+Some examples
+
+```python
+import pandas as pd
+df = pd.read_csv("https://github.com/pandas-dev/pandas/raw/main/doc/data/titanic.csv")
+# df.loc[df.Ticket >20000]
+from random import randrange
+getrandomlist = lambda x: [
+  [[randrange(1, 100), randrange(1, 100)] * 1] * randrange(1, 10)
+]
+df["listtest"] = df.PassengerId.map(getrandomlist)
+
+
+getrandomdict = lambda x: {
+  randrange(1, 100):randrange(1, 100) for _ in range(randrange(1, 10))
+}
+df["dicttest"] = df.PassengerId.map(getrandomdict)
+from a_easy_loc import pd_add_easy_loc
+pd_add_easy_loc()
+df.shortloc_greater_replace('Pclass', 2,3000)
+
+df.shortloc_equal('Pclass', 3)
+     PassengerId  Survived  Pclass       Name     Sex    Age  SibSp  Parch     Ticket     Fare  Cabin Embarked   listtest   dicttest
+0            1           0       3  Braund...    male  22.00      1      0  A/5 21171   7.2500    NaN        S  [[[44,...  {5: 8,...
+2            3           1       3  Heikki...  female  26.00      0      0  STON/O...   7.9250    NaN        S  [[[60,...  {33: 3...
+4            5           0       3  Allen,...    male  35.00      0      0     373450   8.0500    NaN        S  [[[99,...  {96: 1...
+5            6           0       3  Moran,...    male    NaN      0      0     330877   8.4583    NaN        Q  [[[82,...  {23: 1...
+7            8           0       3  Palsso...    male   2.00      3      1     349909  21.0750    NaN        S  [[[14,...  {20: 8...
+8            9           1       3  Johnso...  female  27.00      0      2     347742  11.1333    NaN        S  [[[12,...  {96: 5...
+
+
+df.shortloc_equal('Ticket', 373450)
+   PassengerId  Survived  Pclass       Name   Sex   Age  SibSp  Parch  Ticket  Fare Cabin Embarked   listtest   dicttest
+4          5           0       3  Allen,...  male  35.0      0      0  373450  8.05   NaN        S  [[[99,...  {96: 1...
+
+
+df.shortloc_greater('Pclass', 2)
+     PassengerId  Survived  Pclass       Name     Sex    Age  SibSp  Parch     Ticket     Fare  Cabin Embarked   listtest   dicttest
+0            1           0       3  Braund...    male  22.00      1      0  A/5 21171   7.2500    NaN        S  [[[44,...  {5: 8,...
+2            3           1       3  Heikki...  female  26.00      0      0  STON/O...   7.9250    NaN        S  [[[60,...  {33: 3...
+4            5           0       3  Allen,...    male  35.00      0      0     373450   8.0500    NaN        S  [[[99,...  {96: 1...
+5            6           0       3  Moran,...    male    NaN      0      0     330877   8.4583    NaN        Q  [[[82,...  {23: 1...
+
+df.shortloc_greater('Ticket', 373450)
+     PassengerId  Survived  Pclass       Name     Sex   Age  SibSp  Parch   Ticket     Fare Cabin Embarked   listtest   dicttest
+16          17           0       3  Rice, ...    male   2.0      4      1   382652  29.1250   NaN        Q  [[[17,...  {46: 7...
+50          51           0       3  Panula...    male   7.0      4      1  3101295  39.6875   NaN        S  [[[30,...  {64: 2...
+68          69           1       3  Anders...  female  17.0      4      2  3101281   7.9250   NaN        S  [[[4, ...  {92: 3...
+77          78           0       3  Moutal...    male   NaN      0      0   374746   8.0500   NaN        S  [[[65,...  {47: 9...
+85          86           1       3  Backst...  female  33.0      3      0  3101278  15.8500   NaN        S  [[[55,...  {5: 22...
+
+
+df.shortloc_greater_or_equal('Age', 43)
+     PassengerId  Survived  Pclass       Name     Sex   Age  SibSp  Parch     Ticket      Fare      Cabin Embarked   listtest   dicttest
+6            7           0       1  McCart...    male  54.0      0      0      17463   51.8625        E46        S  [[[47,...   {22: 17}
+11          12           1       1  Bonnel...  female  58.0      0      0     113783   26.5500       C103        S  [[[1, ...    {35: 9}
+15          16           1       2  Hewlet...  female  55.0      0      0     248706   16.0000        NaN        S  [[[43,...  {40: 6...
+33          34           0       2  Wheado...    male  66.0      0      0  C.A. 2...   10.5000        NaN        S  [[[6, ...   {50: 28}
+52          53           1       1  Harper...  female  49.0      1      0   PC 17572   76.7292        D33        C  [[[41,...  {54: 6...
+
+
+df.shortloc_greater_replace('Pclass', 2,3000)
+     PassengerId  Survived  Pclass       Name     Sex    Age  SibSp  Parch     Ticket      Fare      Cabin Embarked   listtest   dicttest
+0            1           0    3000  Braund...    male  22.00      1      0  A/5 21171    7.2500        NaN        S  [[[65,...  {76: 3...
+1            2           1       1  Cuming...  female  38.00      1      0   PC 17599   71.2833        C85        C  [[[1, ...  {55: 3...
+2            3           1    3000  Heikki...  female  26.00      0      0  STON/O...    7.9250        NaN        S  [[[56,...  {7: 54...
+3            4           1       1  Futrel...  female  35.00      1      0     113803   53.1000       C123        S  [[[91,...   {51: 89}
+4            5           0    3000  Allen,...    male  35.00      0      0     373450    8.0500        NaN        S  [[[20,...  {39: 5...
+5            6           0    3000  Moran,...    male    NaN      0      0     330877    8.4583        NaN        Q  [[[60,...  {63: 2...
+6            7           0       1  McCart...    male  54.00      0      0      17463   51.8625        E46        S  [[[51,...  {1: 90...
+
+
+
+df.shortloc_greater_replace('Ticket', 5000, 888000)
+     PassengerId  Survived  Pclass       Name     Sex    Age  SibSp  Parch     Ticket      Fare      Cabin Embarked   listtest   dicttest
+0            1           0       3  Braund...    male  22.00      1      0  A/5 21171    7.2500        NaN        S  [[[74,...  {40: 3...
+1            2           1       1  Cuming...  female  38.00      1      0   PC 17599   71.2833        C85        C  [[[67,...     {1: 8}
+2            3           1       3  Heikki...  female  26.00      0      0  STON/O...    7.9250        NaN        S  [[[62,...   {39: 79}
+3            4           1       1  Futrel...  female  35.00      1      0     888000   53.1000       C123        S  [[[15,...  {13: 2...
+4            5           0       3  Allen,...    male  35.00      0      0     888000    8.0500        NaN        S  [[[81,...   {60: 90}
+5            6           0       3  Moran,...    male    NaN      0      0     888000    8.4583        NaN        Q  [[[58,...    {20: 4}
+6            7           0       1  McCart...    male  54.00      0      0     888000   51.8625        E46        S  [[[28,...  {21: 8...
+7            8           0       3  Palsso...    male   2.00      3      1     888000   21.0750        NaN        S  [[[25,...  {53: 8...
+8            9           1       3  Johnso...  female  27.00      0      2     888000   11.1333        NaN        S  [[[47,...  {19: 3...
+
+
+df.shortloc_greater_replace('Cabin','C123', pd.NA)
+     PassengerId  Survived  Pclass       Name     Sex    Age  SibSp  Parch     Ticket      Fare      Cabin Embarked   listtest   dicttest
+0            1           0       3  Braund...    male  22.00      1      0  A/5 21171    7.2500        NaN        S  [[[74,...  {40: 3...
+1            2           1       1  Cuming...  female  38.00      1      0   PC 17599   71.2833       <NA>        C  [[[67,...     {1: 8}
+2            3           1       3  Heikki...  female  26.00      0      0  STON/O...    7.9250        NaN        S  [[[62,...   {39: 79}
+3            4           1       1  Futrel...  female  35.00      1      0     113803   53.1000       C123        S  [[[15,...  {13: 2...
+4            5           0       3  Allen,...    male  35.00      0      0     373450    8.0500        NaN        S  [[[81,...   {60: 90}
+5            6           0       3  Moran,...    male    NaN      0      0     330877    8.4583        NaN        Q  [[[58,...    {20: 4}
+6            7           0       1  McCart...    male  54.00      0      0      17463   51.8625       <NA>        S  [[[28,...  {21: 8...
+7            8           0       3  Palsso...    male   2.00      3      1     349909   21.0750        NaN        S  [[[25,...  {53: 8...
+
+df.shortloc_in_iter('listtest', 3)
+     PassengerId  Survived  Pclass                 Name     Sex   Age  SibSp  Parch        Ticket     Fare Cabin Embarked             listtest             dicttest
+19            20         1       3  Masselmani, Mrs....  female   NaN      0      0          2649   7.2250   NaN        C  [[[32, 3], [32, ...  {98: 75, 69: 39,...
+66            67         1       2  Nye, Mrs. (Eliza...  female  29.0      0      0    C.A. 29395  10.5000   F33        S  [[[3, 98], [3, 9...             {60: 81}
+92            93         0       1  Chaffee, Mr. Her...    male  46.0      1      0   W.E.P. 5734  61.1750   E31        S  [[[52, 3], [52, ...             {80: 25}
+106          107         1       3  Salkjelsvik, Mis...  female  21.0      0      0        343120   7.6500   NaN        S  [[[85, 3], [85, ...             {62: 49}
+120          121         0       2  Hickman, Mr. Sta...    male  21.0      2      0  S.O.C. 14879  73.5000   NaN        S  [[[40, 3], [40, ...  {28: 85, 60: 72,...
+129          130         0       3   Ekstrom, Mr. Johan    male  45.0      0      0        347061   6.9750   NaN        S  [[[3, 76], [3, 7...  {79: 2, 30: 18, ...
+132          133         0       3  Robins, Mrs. Ale...  female  47.0      1      0     A/5. 3337  14.5000   NaN        S  [[[3, 68], [3, 6...  {69: 90, 1: 23, ...
+184          185         1       3  Kink-Heilmann, M...  female   4.0      0      2        315153  22.0250   NaN        S  [[[3, 88], [3, 8...  {24: 74, 30: 11,...
+
+df.shortloc_in_iter('listtest', [3,4,10])
+     PassengerId  Survived  Pclass                 Name     Sex    Age  SibSp  Parch           Ticket      Fare        Cabin Embarked             listtest             dicttest
+19            20         1       3  Masselmani, Mrs....  female    NaN      0      0             2649    7.2250          NaN        C  [[[32, 3], [32, ...  {98: 75, 69: 39,...
+22            23         1       3  McGowan, Miss. A...  female  15.00      0      0           330923    8.0292          NaN        Q  [[[13, 4], [13, ...  {56: 86, 30: 5, ...
+27            28         0       1  Fortune, Mr. Cha...    male  19.00      3      2            19950  263.0000  C23 C25 C27        S  [[[4, 66], [4, 6...  {58: 98, 32: 55,...
+66            67         1       2  Nye, Mrs. (Eliza...  female  29.00      0      0       C.A. 29395   10.5000          F33        S  [[[3, 98], [3, 9...             {60: 81}
+74            75         1       3        Bing, Mr. Lee    male  32.00      0      0             1601   56.4958          NaN        S  [[[14, 4], [14, ...  {31: 31, 64: 38,...
+84            85         1       2  Ilett, Miss. Bertha  female  17.00      0      0       SO/C 14885   10.5000          NaN        S  [[[18, 10], [18,...  {81: 64, 10: 80,...
+
+
+df.shortloc_in_iter('dicttest', [3,4,10])
+     PassengerId  Survived  Pclass                           Name     Sex    Age  SibSp  Parch             Ticket      Fare            Cabin Embarked                       listtest                       dicttest
+5              6         0       3               Moran, Mr. James    male    NaN      0      0             330877    8.4583              NaN        Q         [[[58, 72], [58, 72]]]                        {20: 4}
+8              9         1       3  Johnson, Mrs. Oscar W (Eli...  female  27.00      0      2             347742   11.1333              NaN        S         [[[47, 12], [47, 12]]]         {19: 3, 60: 24, 9: 38}
+
+
+df.shortloc_in_iter('dicttest', [3,4,10])
+     PassengerId  Survived  Pclass                          Name     Sex   Age  SibSp  Parch         Ticket     Fare Cabin Embarked                                                           listtest                                                               dicttest
+96            97         0       1     Goldschmidt, Mr. George B    male  71.0      0      0       PC 17754  34.6542    A5        C           [[[94, 4], [94, 4], [94, 4], [94, 4], [94, 4], [94, 4]]]       {67: 92, 24: 19, 53: 40, 66: 53, 44: 81, 94: 10, 34: 63, 61: 45}
+103          104         0       3    Johansson, Mr. Gustaf Joel    male  33.0      0      0           7540   8.6542   NaN        S               [[[89, 10], [89, 10], [89, 10], [89, 10], [89, 10]]]                                        {92: 23, 32: 17, 53: 3, 98: 94}
+129          130         0       3            Ekstrom, Mr. Johan    male  45.0      0      0         347061   6.9750   NaN        S  [[[3, 76], [3, 76], [3, 76], [3, 76], [3, 76], [3, 76], [3, 76]]]   {79: 2, 30: 18, 63: 10, 62: 26, 91: 58, 11: 44, 8: 81, 6: 93, 97: 5}
+
+
+df.shortloc_in_iter_replace('dicttest', [3,4,10], 15151515)
+     PassengerId  Survived  Pclass                           Name     Sex    Age  SibSp  Parch              Ticket      Fare            Cabin Embarked                       listtest                       dicttest
+0              1         0       3        Braund, Mr. Owen Harris    male  22.00      1      0           A/5 21171    7.2500              NaN        S  [[[74, 68], [74, 68], [74,...  {40: 30, 93: 84, 24: 92, 7...
+1              2         1       1  Cumings, Mrs. John Bradley...  female  38.00      1      0            PC 17599   71.2833              C85        C  [[[67, 64], [67, 64], [67,...                         {1: 8}
+2              3         1       3         Heikkinen, Miss. Laina  female  26.00      0      0    STON/O2. 3101282    7.9250              NaN        S  [[[62, 65], [62, 65], [62,...                       {39: 79}
+3              4         1       1  Futrelle, Mrs. Jacques Hea...  female  35.00      1      0              113803   53.1000             C123        S  [[[15, 96], [15, 96], [15,...       {13: 29, 65: 59, 99: 31}
+4              5         0       3       Allen, Mr. William Henry    male  35.00      0      0              373450    8.0500              NaN        S                   [[[81, 13]]]                       {60: 90}
+5              6         0       3               Moran, Mr. James    male    NaN      0      0              330877    8.4583              NaN        Q         [[[58, 72], [58, 72]]]                       15151515
+6              7         0       1        McCarthy, Mr. Timothy J    male  54.00      0      0               17463   51.8625              E46        S  [[[28, 98], [28, 98], [28,...  {21: 8, 31: 42, 9: 40, 93:...
+7              8         0       3  Palsson, Master. Gosta Leo...    male   2.00      3      1              349909   21.0750              NaN        S  [[[25, 88], [25, 88], [25,...  {53: 83, 49: 66, 57: 95, 4...
+8              9         1       3  Johnson, Mrs. Oscar W (Eli...  female  27.00      0      2              347742   11.1333              NaN        S         [[[47, 12], [47, 12]]]                       15151515
+
+df.shortloc_isin('Embarked', ['C', 'S'])
+     PassengerId  Survived  Pclass                           Name     Sex    Age  SibSp  Parch              Ticket      Fare            Cabin Embarked                       listtest                       dicttest
+0              1         0       3        Braund, Mr. Owen Harris    male  22.00      1      0           A/5 21171    7.2500              NaN        S  [[[74, 68], [74, 68], [74,...  {40: 30, 93: 84, 24: 92, 7...
+1              2         1       1  Cumings, Mrs. John Bradley...  female  38.00      1      0            PC 17599   71.2833              C85        C  [[[67, 64], [67, 64], [67,...                         {1: 8}
+2              3         1       3         Heikkinen, Miss. Laina  female  26.00      0      0    STON/O2. 3101282    7.9250              NaN        S  [[[62, 65], [62, 65], [62,...                       {39: 79}
+3              4         1       1  Futrelle, Mrs. Jacques Hea...  female  35.00      1      0              113803   53.1000             C123        S  [[[15, 96], [15, 96], [15,...       {13: 29, 65: 59, 99: 31}
+4              5         0       3       Allen, Mr. William Henry    male  35.00      0      0              373450    8.0500              NaN        S                   [[[81, 13]]]                       {60: 90}
+6              7         0       1        McCarthy, Mr. Timothy J    male  54.00      0      0               17463   51.8625              E46        S  [[[28, 98], [28, 98], [28,...  {21: 8, 31: 42, 9: 40, 93:...
+7              8         0       3  Palsson, Master. Gosta Leo...    male   2.00      3      1              349909   21.0750              NaN        S  [[[25, 88], [25, 88], [25,...  {53: 83, 49: 66, 57: 95, 4...
+8              9         1       3  Johnson, Mrs. Oscar W (Eli...  female  27.00      0      2              347742   11.1333              NaN        S         [[[47, 12], [47, 12]]]         {19: 3, 60: 24, 9: 38}
+
+df.shortloc_isin_replace('Embarked', ['C', 'S'], 'CCCCCCCCCCCCCCCCCCCSSSSSSSSSSSSSSSSSSSSSSSSSSSSS')
+     PassengerId  Survived  Pclass       Name     Sex    Age  SibSp  Parch     Ticket      Fare      Cabin   Embarked   listtest   dicttest
+0            1           0       3  Braund...    male  22.00      1      0  A/5 21171    7.2500        NaN  CCCCCC...  [[[74,...  {40: 3...
+1            2           1       1  Cuming...  female  38.00      1      0   PC 17599   71.2833        C85  CCCCCC...  [[[67,...     {1: 8}
+2            3           1       3  Heikki...  female  26.00      0      0  STON/O...    7.9250        NaN  CCCCCC...  [[[62,...   {39: 79}
+3            4           1       1  Futrel...  female  35.00      1      0     113803   53.1000       C123  CCCCCC...  [[[15,...  {13: 2...
+4            5           0       3  Allen,...    male  35.00      0      0     373450    8.0500        NaN  CCCCCC...  [[[81,...   {60: 90}
+5            6           0       3  Moran,...    male    NaN      0      0     330877    8.4583        NaN          Q  [[[58,...    {20: 4}
+
+
+df.shortloc_isna('Age')
+     PassengerId  Survived  Pclass                           Name     Sex  Age  SibSp  Parch              Ticket      Fare  Cabin Embarked                       listtest                       dicttest
+5              6         0       3               Moran, Mr. James    male  NaN      0      0              330877    8.4583    NaN        Q         [[[25, 39], [25, 39]]]       {97: 78, 85: 88, 42: 34}
+17            18         1       2   Williams, Mr. Charles Eugene    male  NaN      0      0              244373   13.0000    NaN        S  [[[17, 6], [17, 6], [17, 6...                 {41: 6, 2: 82}
+19            20         1       3        Masselmani, Mrs. Fatima  female  NaN      0      0                2649    7.2250    NaN        C  [[[11, 37], [11, 37], [11,...  {43: 73, 50: 28, 38: 47, 4...
+26            27         0       3        Emir, Mr. Farred Chehab    male  NaN      0      0                2631    7.2250    NaN        C  [[[48, 66], [48, 66], [48,...               {33: 45, 82: 90}
+28            29         1       3  O'Dwyer, Miss. Ellen "Nellie"  female  NaN      0      0              330959    7.8792    NaN        Q           [[[3, 53], [3, 53]]]               {29: 90, 84: 86}
+29            30         0       3            Todoroff, Mr. Lalio    male  NaN      0      0              349216    7.8958    NaN        S  [[[67, 3], [67, 3], [67, 3...  {57: 49, 23: 71, 64: 45, 1...
+31            32         1       1  Spencer, Mrs. William Augu...  female  NaN      1      0            PC 17569  146.5208    B78        C  [[[88, 94], [88, 94], [88,...  {4: 42, 98: 58, 94: 7, 39:...
+
+
+df.shortloc_isna_replace('Age',16541)
+     PassengerId  Survived  Pclass                           Name     Sex       Age  SibSp  Parch              Ticket      Fare            Cabin Embarked                       listtest                       dicttest
+0              1         0       3        Braund, Mr. Owen Harris    male     22.00      1      0           A/5 21171    7.2500              NaN        S  [[[27, 71], [27, 71], [27,...  {36: 67, 73: 54, 56: 48, 8...
+1              2         1       1  Cumings, Mrs. John Bradley...  female     38.00      1      0            PC 17599   71.2833              C85        C  [[[31, 68], [31, 68], [31,...                        {9: 77}
+2              3         1       3         Heikkinen, Miss. Laina  female     26.00      0      0    STON/O2. 3101282    7.9250              NaN        S                   [[[31, 23]]]  {49: 6, 76: 22, 52: 18, 6:...
+3              4         1       1  Futrelle, Mrs. Jacques Hea...  female     35.00      1      0              113803   53.1000             C123        S  [[[96, 48], [96, 48], [96,...  {27: 90, 9: 38, 18: 94, 67...
+4              5         0       3       Allen, Mr. William Henry    male     35.00      0      0              373450    8.0500              NaN        S  [[[60, 84], [60, 84], [60,...  {8: 61, 37: 4, 25: 43, 21:...
+5              6         0       3               Moran, Mr. James    male  16541.00      0      0              330877    8.4583              NaN        Q         [[[25, 39], [25, 39]]]       {97: 78, 85: 88, 42: 34}
+6              7         0       1        McCarthy, Mr. Timothy J    male     54.00      0      0               17463   51.8625              E46        S  [[[76, 5], [76, 5], [76, 5...  {56: 51, 13: 24, 84: 24, 9...
+
+df.shortloc_less('Ticket', 7534)
+
+     PassengerId  Survived  Pclass                           Name     Sex    Age  SibSp  Parch Ticket     Fare        Cabin Embarked                       listtest                       dicttest
+19            20         1       3        Masselmani, Mrs. Fatima  female    NaN      0      0   2649   7.2250          NaN        C  [[[11, 37], [11, 37], [11,...  {43: 73, 50: 28, 38: 47, 4...
+26            27         0       3        Emir, Mr. Farred Chehab    male    NaN      0      0   2631   7.2250          NaN        C  [[[48, 66], [48, 66], [48,...               {33: 45, 82: 90}
+36            37         1       3               Mamee, Mr. Hanna    male    NaN      0      0   2677   7.2292          NaN        C  [[[84, 24], [84, 24], [84,...  {39: 19, 88: 50, 23: 7, 53...
+39            40         1       3    Nicola-Yarred, Miss. Jamila  female  14.00      1      0   2651  11.2417          NaN        C  [[[20, 72], [20, 72], [20,...  {72: 91, 81: 15, 89: 24, 9...
+48            49         0       3            Samaan, Mr. Youssef    male    NaN      2      0   2662  21.6792          NaN        C  [[[79, 85], [79, 85], [79,...                       {35: 61}
+53            54         1       2  Faunthorpe, Mrs. Lizzie (E...  female  29.00      1      0   2926  26.0000          NaN        S         [[[62, 79], [62, 79]]]  {36: 53, 38: 70, 6: 1, 89:...
+57            58         0       3            Novel, Mr. Mansouer    male  28.50      0      0   2697   7.2292          NaN        C         [[[86, 78], [86, 78]]]                {28: 5, 49: 22}
+60            61         0       3          Sirayanian, Mr. Orsen    male  22.00      0      0   2669   7.2292          NaN        C                   [[[24, 72]]]  {74: 59, 16: 44, 30: 17, 5...
+65            66         1       3       Moubarek, Master. Gerios    male    NaN      1      1   2661  15.2458          NaN        C  [[[56, 96], [56, 96], [56,...  {5: 34, 59: 97, 78: 15, 76...
+73            74         0       3    Chronopoulos, Mr. Apostolos    male  26.00      1      0   2680  14.4542          NaN        C         [[[78, 24], [78, 24]]]  {96: 26, 87: 73, 58: 49, 3...
+74            75         1       3                  Bing, Mr. Lee    male  32.00      0      0   1601  56.4958          NaN        S  [[[86, 20], [86, 20], [86,...  {84: 87, 18: 40, 17: 28, 7...
+
+
+df.shortloc_less_replace('Age', 30, 'less 30')
+     PassengerId  Survived  Pclass                           Name     Sex      Age  SibSp  Parch              Ticket      Fare            Cabin Embarked                       listtest                       dicttest
+0              1         0       3        Braund, Mr. Owen Harris    male  less 30      1      0           A/5 21171    7.2500              NaN        S  [[[27, 71], [27, 71], [27,...  {36: 67, 73: 54, 56: 48, 8...
+1              2         1       1  Cumings, Mrs. John Bradley...  female     38.0      1      0            PC 17599   71.2833              C85        C  [[[31, 68], [31, 68], [31,...                        {9: 77}
+2              3         1       3         Heikkinen, Miss. Laina  female  less 30      0      0    STON/O2. 3101282    7.9250              NaN        S                   [[[31, 23]]]  {49: 6, 76: 22, 52: 18, 6:...
+3              4         1       1  Futrelle, Mrs. Jacques Hea...  female     35.0      1      0              113803   53.1000             C123        S  [[[96, 48], [96, 48], [96,...  {27: 90, 9: 38, 18: 94, 67...
+
+
+df.shortloc_less_or_equal_replace('Survived', 0, 'DEAD')
+     PassengerId Survived  Pclass                           Name     Sex    Age  SibSp  Parch              Ticket      Fare            Cabin Embarked                       listtest                       dicttest
+0              1     DEAD       3        Braund, Mr. Owen Harris    male  22.00      1      0           A/5 21171    7.2500              NaN        S  [[[27, 71], [27, 71], [27,...  {36: 67, 73: 54, 56: 48, 8...
+1              2        1       1  Cumings, Mrs. John Bradley...  female  38.00      1      0            PC 17599   71.2833              C85        C  [[[31, 68], [31, 68], [31,...                        {9: 77}
+2              3        1       3         Heikkinen, Miss. Laina  female  26.00      0      0    STON/O2. 3101282    7.9250              NaN        S                   [[[31, 23]]]  {49: 6, 76: 22, 52: 18, 6:...
+3              4        1       1  Futrelle, Mrs. Jacques Hea...  female  35.00      1      0              113803   53.1000             C123        S  [[[96, 48], [96, 48], [96,...  {27: 90, 9: 38, 18: 94, 67...
+4              5     DEAD       3       Allen, Mr. William Henry    male  35.00      0      0              373450    8.0500              NaN        S  [[[60, 84], [60, 84], [60,...  {8: 61, 37: 4, 25: 43, 21:...
+5              6     DEAD       3               Moran, Mr. James    male    NaN      0      0              330877    8.4583              NaN        Q         [[[25, 39], [25, 39]]]       {97: 78, 85: 88, 42: 34}
+6              7     DEAD       1        McCarthy, Mr. Timothy J    male  54.00      0      0               17463   51.8625              E46        S  [[[76, 5], [76, 5], [76, 5...  {56: 51, 13: 24, 84: 24, 9...
+7              8     DEAD       3  Palsson, Master. Gosta Leo...    male   2.00      3      1              349909   21.0750              NaN        S  [[[42, 52], [42, 52], [42,...               {71: 69, 44: 14}
+
+
+
+df.shortloc_not_equal_replace('Survived', 0, True)
+     PassengerId Survived  Pclass                           Name     Sex    Age  SibSp  Parch              Ticket      Fare            Cabin Embarked                       listtest                       dicttest
+0              1        0       3        Braund, Mr. Owen Harris    male  22.00      1      0           A/5 21171    7.2500              NaN        S  [[[27, 71], [27, 71], [27,...  {36: 67, 73: 54, 56: 48, 8...
+1              2     True       1  Cumings, Mrs. John Bradley...  female  38.00      1      0            PC 17599   71.2833              C85        C  [[[31, 68], [31, 68], [31,...                        {9: 77}
+2              3     True       3         Heikkinen, Miss. Laina  female  26.00      0      0    STON/O2. 3101282    7.9250              NaN        S                   [[[31, 23]]]  {49: 6, 76: 22, 52: 18, 6:...
+3              4     True       1  Futrelle, Mrs. Jacques Hea...  female  35.00      1      0              113803   53.1000             C123        S  [[[96, 48], [96, 48], [96,...  {27: 90, 9: 38, 18: 94, 67...
+4              5        0       3       Allen, Mr. William Henry    male  35.00      0      0              373450    8.0500              NaN        S  [[[60, 84], [60, 84], [60,...  {8: 61, 37: 4, 25: 43, 21:...
+5              6        0       3               Moran, Mr. James    male    NaN      0      0              330877    8.4583              NaN        Q         [[[25, 39], [25, 39]]]       {97: 78, 85: 88, 42: 34}
+
+
+
+df.shortloc_not_in_iter('listtest', list(range(0,90)))
+     PassengerId  Survived  Pclass                           Name     Sex   Age  SibSp  Parch      Ticket      Fare Cabin Embarked                       listtest                       dicttest
+832          833         0       3                 Saad, Mr. Amin    male   NaN      0      0        2671    7.2292   NaN        C  [[[95, 94], [95, 94], [95,...                {82: 66, 84: 5}
+484          485         1       1        Bishop, Mr. Dickinson H    male  25.0      1      0       11967   91.0792   B49        C  [[[97, 92], [97, 92], [97,...  {20: 34, 2: 23, 98: 37, 1:...
+581          582         1       1  Thayer, Mrs. John Borland ...  female  39.0      1      1       17421  110.8833   C68        C         [[[91, 90], [91, 90]]]  {48: 98, 3: 98, 93: 4, 97:...
+336          337         0       1      Pears, Mr. Thomas Clinton    male  29.0      1      0      113776   66.6000    C2        S         [[[90, 98], [90, 98]]]                         {6: 7}
+116          117         0       3           Connors, Mr. Patrick    male  70.5      0      0      370369    7.7500   NaN        Q  [[[92, 99], [92, 99], [92,...  {60: 79, 75: 71, 28: 68, 5...
+52            53         1       1  Harper, Mrs. Henry Sleeper...  female  49.0      1      0    PC 17572   76.7292   D33        C  [[[96, 94], [96, 94], [96,...  {20: 53, 93: 11, 83: 79, 5...
+439          440         0       2  Kvillner, Mr. Johan Henrik...    male  31.0      0      0  C.A. 18723   10.5000   NaN        S  [[[95, 98], [95, 98], [95,...  {58: 11, 89: 23, 22: 66, 1...
+56            57         1       2              Rugg, Miss. Emily  female  21.0      0      0  C.A. 31026   10.5000   NaN        S  [[[92, 92], [92, 92], [92,...                {45: 1, 37: 98}
+
+
+
+df.shortloc_not_in_iter_replace('listtest', list(range(0,20)), 27)
+     PassengerId  Survived  Pclass                           Name     Sex    Age  SibSp  Parch              Ticket      Fare            Cabin Embarked                       listtest                       dicttest
+0              1         0       3        Braund, Mr. Owen Harris    male  22.00      1      0           A/5 21171    7.2500              NaN        S                             27  {36: 67, 73: 54, 56: 48, 8...
+1              2         1       1  Cumings, Mrs. John Bradley...  female  38.00      1      0            PC 17599   71.2833              C85        C                             27                        {9: 77}
+2              3         1       3         Heikkinen, Miss. Laina  female  26.00      0      0    STON/O2. 3101282    7.9250              NaN        S                             27  {49: 6, 76: 22, 52: 18, 6:...
+3              4         1       1  Futrelle, Mrs. Jacques Hea...  female  35.00      1      0              113803   53.1000             C123        S                             27  {27: 90, 9: 38, 18: 94, 67...
+4              5         0       3       Allen, Mr. William Henry    male  35.00      0      0              373450    8.0500              NaN        S                             27  {8: 61, 37: 4, 25: 43, 21:...
+5              6         0       3               Moran, Mr. James    male    NaN      0      0              330877    8.4583              NaN        Q                             27       {97: 78, 85: 88, 42: 34}
+6              7         0       1        McCarthy, Mr. Timothy J    male  54.00      0      0               17463   51.8625              E46        S  [[[76, 5], [76, 5], [76, 5...  {56: 51, 13: 24, 84: 24, 9...
+
+
+df.shortloc_regex('Fare', r'^\d?7\.').to_string(max_colwidth=30)
+     PassengerId  Survived  Pclass                           Name     Sex   Age  SibSp  Parch              Ticket     Fare  Cabin Embarked                       listtest                       dicttest
+0              1         0       3        Braund, Mr. Owen Harris    male  22.0      1      0           A/5 21171   7.2500    NaN        S  [[[27, 71], [27, 71], [27,...  {36: 67, 73: 54, 56: 48, 8...
+2              3         1       3         Heikkinen, Miss. Laina  female  26.0      0      0    STON/O2. 3101282   7.9250    NaN        S                   [[[31, 23]]]  {49: 6, 76: 22, 52: 18, 6:...
+14            15         0       3  Vestrom, Miss. Hulda Amand...  female  14.0      0      0              350406   7.8542    NaN        S  [[[40, 57], [40, 57], [40,...  {54: 39, 8: 35, 76: 84, 20...
+19            20         1       3        Masselmani, Mrs. Fatima  female   NaN      0      0                2649   7.2250    NaN        C  [[[11, 37], [11, 37], [11,...  {43: 73, 50: 28, 38: 47, 4...
+26            27         0       3        Emir, Mr. Farred Chehab    male   NaN      0      0                2631   7.2250    NaN        C  [[[48, 66], [48, 66], [48,...               {33: 45, 82: 90}
+28            29         1       3  O'Dwyer, Miss. Ellen "Nellie"  female   NaN      0      0              330959   7.8792    NaN        Q           [[[3, 53], [3, 53]]]               {29: 90, 84: 86}
+29            30         0       3            Todoroff, Mr. Lalio    male   NaN      0      0              349216   7.8958    NaN        S  [[[67, 3], [67, 3], [67, 3...  {57: 49, 23: 71, 64: 45, 1...
+30            31         0       1       Uruchurtu, Don. Manuel E    male  40.0      0      0            PC 17601  27.7208    NaN        C  [[[91, 32], [91, 32], [91,...         {1: 29, 54: 93, 96: 7}
+
+
+
+df.shortloc_not_regex('Fare', r'^\d?7\.').to_string(max_colwidth=30)
+     PassengerId  Survived  Pclass                           Name     Sex    Age  SibSp  Parch             Ticket      Fare            Cabin Embarked                       listtest                       dicttest
+1              2         1       1  Cumings, Mrs. John Bradley...  female  38.00      1      0           PC 17599   71.2833              C85        C  [[[31, 68], [31, 68], [31,...                        {9: 77}
+3              4         1       1  Futrelle, Mrs. Jacques Hea...  female  35.00      1      0             113803   53.1000             C123        S  [[[96, 48], [96, 48], [96,...  {27: 90, 9: 38, 18: 94, 67...
+4              5         0       3       Allen, Mr. William Henry    male  35.00      0      0             373450    8.0500              NaN        S  [[[60, 84], [60, 84], [60,...  {8: 61, 37: 4, 25: 43, 21:...
+5              6         0       3               Moran, Mr. James    male    NaN      0      0             330877    8.4583              NaN        Q         [[[25, 39], [25, 39]]]       {97: 78, 85: 88, 42: 34}
+6              7         0       1        McCarthy, Mr. Timothy J    male  54.00      0      0              17463   51.8625              E46        S  [[[76, 5], [76, 5], [76, 5...  {56: 51, 13: 24, 84: 24, 9...
+7              8         0       3  Palsson, Master. Gosta Leo...    male   2.00      3      1             349909   21.0750              NaN        S  [[[42, 52], [42, 52], [42,...               {71: 69, 44: 14}
+8              9         1       3  Johnson, Mrs. Oscar W (Eli...  female  27.00      0      2             347742   11.1333              NaN        S  [[[92, 21], [92, 21], [92,...  {61: 17, 72: 44, 81: 74, 3...
+9             10         1       2  Nasser, Mrs. Nicholas (Ade...  female  14.00      1      0             237736   30.0708              NaN        C  [[[88, 97], [88, 97], [88,...                       {69: 43}
+
+
+df.shortloc_str('Pclass', r'3').to_string(max_colwidth=30)
+     PassengerId  Survived  Pclass                           Name     Sex    Age  SibSp  Parch              Ticket     Fare  Cabin Embarked                       listtest                       dicttest
+0              1         0       3        Braund, Mr. Owen Harris    male  22.00      1      0           A/5 21171   7.2500    NaN        S  [[[27, 71], [27, 71], [27,...  {36: 67, 73: 54, 56: 48, 8...
+2              3         1       3         Heikkinen, Miss. Laina  female  26.00      0      0    STON/O2. 3101282   7.9250    NaN        S                   [[[31, 23]]]  {49: 6, 76: 22, 52: 18, 6:...
+4              5         0       3       Allen, Mr. William Henry    male  35.00      0      0              373450   8.0500    NaN        S  [[[60, 84], [60, 84], [60,...  {8: 61, 37: 4, 25: 43, 21:...
+5              6         0       3               Moran, Mr. James    male    NaN      0      0              330877   8.4583    NaN        Q         [[[25, 39], [25, 39]]]       {97: 78, 85: 88, 42: 34}
+7              8         0       3  Palsson, Master. Gosta Leo...    male   2.00      3      1              349909  21.0750    NaN        S  [[[42, 52], [42, 52], [42,...               {71: 69, 44: 14}
+8              9         1       3  Johnson, Mrs. Oscar W (Eli...  female  27.00      0      2              347742  11.1333    NaN        S  [[[92, 21], [92, 21], [92,...  {61: 17, 72: 44, 81: 74, 3...
+10            11         1       3  Sandstrom, Miss. Marguerit...  female   4.00      1      1             PP 9549  16.7000     G6        S  [[[28, 63], [28, 63], [28,...  {12: 80, 63: 96, 79: 99, 5...
+12            13         0       3  Saundercock, Mr. William H...    male  20.00      0      0           A/5. 2151   8.0500    NaN        S  [[[34, 91], [34, 91], [34,...  {42: 68, 46: 90, 66: 96, 3...
+13            14         0       3    Andersson, Mr. Anders Johan    male  39.00      1      5              347082  31.2750    NaN        S  [[[3, 47], [3, 47], [3, 47...  {94: 60, 73: 33, 59: 32, 3...
+14            15         0       3  Vestrom, Miss. Hulda Amand...  female  14.00      0      0              350406   7.8542    NaN        S  [[[40, 57], [40, 57], [40,...  {54: 39, 8: 35, 76: 84, 20...
+16            17         0       3           Rice, Master. Eugene    male   2.00      4      1              382652  29.1250    NaN        Q  [[[24, 8], [24, 8], [24, 8...  {20: 91, 56: 55, 11: 16, 3...
+
+
+
+df.shortloc_str_replace('Pclass', r'3',4).to_string(max_colwidth=30)
+     PassengerId  Survived  Pclass                           Name     Sex    Age  SibSp  Parch              Ticket      Fare            Cabin Embarked                       listtest                       dicttest
+0              1         0       4        Braund, Mr. Owen Harris    male  22.00      1      0           A/5 21171    7.2500              NaN        S  [[[27, 71], [27, 71], [27,...  {36: 67, 73: 54, 56: 48, 8...
+1              2         1       1  Cumings, Mrs. John Bradley...  female  38.00      1      0            PC 17599   71.2833              C85        C  [[[31, 68], [31, 68], [31,...                        {9: 77}
+2              3         1       4         Heikkinen, Miss. Laina  female  26.00      0      0    STON/O2. 3101282    7.9250              NaN        S                   [[[31, 23]]]  {49: 6, 76: 22, 52: 18, 6:...
+3              4         1       1  Futrelle, Mrs. Jacques Hea...  female  35.00      1      0              113803   53.1000             C123        S  [[[96, 48], [96, 48], [96,...  {27: 90, 9: 38, 18: 94, 67...
+4              5         0       4       Allen, Mr. William Henry    male  35.00      0      0              373450    8.0500              NaN        S  [[[60, 84], [60, 84], [60,...  {8: 61, 37: 4, 25: 43, 21:...
+5              6         0       4               Moran, Mr. James    male    NaN      0      0              330877    8.4583              NaN        Q         [[[25, 39], [25, 39]]]       {97: 78, 85: 88, 42: 34}
+6              7         0       1        McCarthy, Mr. Timothy J    male  54.00      0      0               17463   51.8625              E46        S  [[[76, 5], [76, 5], [76, 5...  {56: 51, 13: 24, 84: 24, 9...
+7              8         0       4  Palsson, Master. Gosta Leo...    male   2.00      3      1              349909   21.0750              NaN        S  [[[42, 52], [42, 52], [42,...               {71: 69, 44: 14}
+8              9         1       4  Johnson, Mrs. Oscar W (Eli...  female  27.00      0      2              347742   11.1333              NaN        S  [[[92, 21], [92, 21], [92,...  {61: 17, 72: 44, 81: 74, 3...
+9             10         1       2  Nasser, Mrs. Nicholas (Ade...  female  14.00      1      0              237736   30.0708              NaN        C  [[[88, 97], [88, 97], [88,...                       {69: 43}
+10            11         1       4  Sandstrom, Miss. Marguerit...  female   4.00      1      1             PP 9549   16.7000               G6        S  [[[28, 63], [28, 63], [28,...  {12: 80, 63: 96, 79: 99, 5...
+
+
+
+
+df.loc_positive_and(
+   ("Pclass", "==", 3),
+   ("Sex", "!=", "male"),
+   ("Age", ">=", 1),
+   ("Pclass", ">=", 3),
+   ("listtest", "in_iter", [11, 22, 33, 44, 55, 66, 77, 88, 99]),
+   ("Sex", "in", ["female", "male"]),
+   ("Name", "re", r"Miss\."),
+   ("Ticket", ">", 5000),
+   ("Embarked", "str", "S"),
+)
+
+     PassengerId  Survived  Pclass                           Name     Sex   Age  SibSp  Parch  Ticket     Fare Cabin Embarked                       listtest                       dicttest
+24            25         0       3  Palsson, Miss. Torborg Danira  female   8.0      3      1  349909  21.0750   NaN        S  [[[44, 33], [44, 33], [44,...  {98: 85, 8: 23, 21: 77, 85...
+141          142         1       3       Nysten, Miss. Anna Sofia  female  22.0      0      0  347081   7.7500   NaN        S                   [[[44, 30]]]  {25: 15, 24: 14, 16: 26, 5...
+192          193         1       3  Andersen-Jensen, Miss. Car...  female  19.0      1      0  350046   7.8542   NaN        S  [[[39, 55], [39, 55], [39,...  {1: 44, 16: 59, 80: 13, 81...
+634          635         0       3             Skoog, Miss. Mabel  female   9.0      3      2  347088  27.9000   NaN        S                   [[[11, 22]]]                        {40: 7}
+
+
+
+df.loc_positive_and(('Ticket','==', 373450), ('Pclass','==', 3))
+   PassengerId  Survived  Pclass                      Name   Sex   Age  SibSp  Parch  Ticket  Fare Cabin Embarked                       listtest                       dicttest
+4            5         0       3  Allen, Mr. William Henry  male  35.0      0      0  373450  8.05   NaN        S  [[[60, 84], [60, 84], [60,...  {8: 61, 37: 4, 25: 43, 21:...
+
+
+df.loc_positive_or(('Ticket','==', 373450), ('Pclass','==', 3))
+     PassengerId  Survived  Pclass                           Name     Sex    Age  SibSp  Parch              Ticket     Fare  Cabin Embarked                       listtest                       dicttest
+0              1         0       3        Braund, Mr. Owen Harris    male  22.00      1      0           A/5 21171   7.2500    NaN        S  [[[27, 71], [27, 71], [27,...  {36: 67, 73: 54, 56: 48, 8...
+2              3         1       3         Heikkinen, Miss. Laina  female  26.00      0      0    STON/O2. 3101282   7.9250    NaN        S                   [[[31, 23]]]  {49: 6, 76: 22, 52: 18, 6:...
+4              5         0       3       Allen, Mr. William Henry    male  35.00      0      0              373450   8.0500    NaN        S  [[[60, 84], [60, 84], [60,...  {8: 61, 37: 4, 25: 43, 21:...
+5              6         0       3               Moran, Mr. James    male    NaN      0      0              330877   8.4583    NaN        Q         [[[25, 39], [25, 39]]]       {97: 78, 85: 88, 42: 34}
+7              8         0       3  Palsson, Master. Gosta Leo...    male   2.00      3      1              349909  21.0750    NaN        S  [[[42, 52], [42, 52], [42,...               {71: 69, 44: 14}
+
+
+
+df.loc_positive_and(('Age','>=', 13), ('Age','<=', 19))
+     PassengerId  Survived  Pclass                           Name     Sex   Age  SibSp  Parch             Ticket      Fare            Cabin Embarked                       listtest                       dicttest
+9             10         1       2  Nasser, Mrs. Nicholas (Ade...  female  14.0      1      0             237736   30.0708              NaN        C  [[[88, 97], [88, 97], [88,...                       {69: 43}
+14            15         0       3  Vestrom, Miss. Hulda Amand...  female  14.0      0      0             350406    7.8542              NaN        S  [[[40, 57], [40, 57], [40,...  {54: 39, 8: 35, 76: 84, 20...
+22            23         1       3    McGowan, Miss. Anna "Annie"  female  15.0      0      0             330923    8.0292              NaN        Q  [[[85, 85], [85, 85], [85,...  {80: 2, 70: 5, 27: 24, 10:...
+27            28         0       1  Fortune, Mr. Charles Alexa...    male  19.0      3      2              19950  263.0000      C23 C25 C27        S  [[[7, 96], [7, 96], [7, 96...  {60: 4, 22: 96, 55: 28, 97...
+38            39         0       3  Vander Planke, Miss. Augus...  female  18.0      2      0             345764   18.0000              NaN        S  [[[82, 50], [82, 50], [82,...  {70: 41, 90: 86, 46: 95, 3...
+39            40         1       3    Nicola-Yarred, Miss. Jamila  female  14.0      1      0               2651   11.2417              NaN        C  [[[20, 72], [20, 72], [20,...  {72: 91, 81: 15, 89: 24, 9...
+44            45         1       3  Devaney, Miss. Margaret Delia  female  19.0      0      0             330958    7.8792              NaN        Q  [[[97, 1], [97, 1], [97, 1...  {89: 44, 58: 86, 48: 54, 9...
+49            50         0       3  Arnold-Franchi, Mrs. Josef...  female  18.0      1      0             349237   17.8000              NaN        S         [[[64, 68], [64, 68]]]  {67: 59, 96: 34, 8: 64, 45...
+67            68         0       3       Crease, Mr. Ernest James    male  19.0      0      0          S.P. 3464    8.1583              NaN        S  [[[30, 77], [30, 77], [30,...  {37: 56, 52: 5, 80: 12, 86...
+
+
+
+df.loc_positive_and(('Ticket','!=', 373450), ('Pclass','!=', 3))
+     PassengerId  Survived  Pclass                           Name     Sex    Age  SibSp  Parch            Ticket      Fare            Cabin Embarked                       listtest                       dicttest
+1              2         1       1  Cumings, Mrs. John Bradley...  female  38.00      1      0          PC 17599   71.2833              C85        C  [[[31, 68], [31, 68], [31,...                        {9: 77}
+3              4         1       1  Futrelle, Mrs. Jacques Hea...  female  35.00      1      0            113803   53.1000             C123        S  [[[96, 48], [96, 48], [96,...  {27: 90, 9: 38, 18: 94, 67...
+6              7         0       1        McCarthy, Mr. Timothy J    male  54.00      0      0             17463   51.8625              E46        S  [[[76, 5], [76, 5], [76, 5...  {56: 51, 13: 24, 84: 24, 9...
+9             10         1       2  Nasser, Mrs. Nicholas (Ade...  female  14.00      1      0            237736   30.0708              NaN        C  [[[88, 97], [88, 97], [88,...                       {69: 43}
+11            12         1       1       Bonnell, Miss. Elizabeth  female  58.00      0      0            113783   26.5500             C103        S         [[[66, 84], [66, 84]]]  {87: 7, 75: 62, 84: 22, 94...
+15            16         1       2  Hewlett, Mrs. (Mary D King...  female  55.00      0      0            248706   16.0000              NaN        S  [[[93, 7], [93, 7], [93, 7...  {17: 96, 7: 68, 74: 5, 97:...
+
+
+df.loc_negative_and(('Age','>=', 13), ('Sex','str', 'female'))
+     PassengerId  Survived  Pclass                           Name   Sex    Age  SibSp  Parch           Ticket      Fare    Cabin Embarked                       listtest                       dicttest
+386          387         0       3  Goodwin, Master. Sidney Le...  male   1.00      5      2          CA 2144   46.9000      NaN        S  [[[32, 26], [32, 26], [32,...  {42: 33, 97: 56, 33: 73, 7...
+261          262         1       3  Asplund, Master. Edvin Roj...  male   3.00      4      2           347077   31.3875      NaN        S  [[[40, 73], [40, 73], [40,...  {7: 23, 93: 3, 18: 66, 96:...
+7              8         0       3  Palsson, Master. Gosta Leo...  male   2.00      3      1           349909   21.0750      NaN        S  [[[42, 52], [42, 52], [42,...               {71: 69, 44: 14}
+16            17         0       3           Rice, Master. Eugene  male   2.00      4      1           382652   29.1250      NaN        Q  [[[24, 8], [24, 8], [24, 8...  {20: 91, 56: 55, 11: 16, 3...
+787          788         0       3      Rice, Master. George Hugh  male   8.00      4      1           382652   29.1250      NaN        Q  [[[32, 90], [32, 90], [32,...  {5: 17, 83: 1, 82: 16, 21:...
+788          789         1       3     Dean, Master. Bertram Vere  male   1.00      1      2        C.A. 2315   20.5750      NaN        S  [[[27, 72], [27, 72], [27,...       {58: 65, 42: 92, 61: 72}
+278          279         0       3             Rice, Master. Eric  male   7.00      4      1           382652   29.1250      NaN        Q  [[[48, 59], [48, 59], [48,...  {16: 64, 97: 83, 66: 91, 9...
+
+
+
+df.shortloc_regex('Name', '^Ab').shortloc_not_equal('Sex', 'male').shortloc_equal('Age', 35)
+     PassengerId  Survived  Pclass                           Name     Sex   Age  SibSp  Parch     Ticket   Fare Cabin Embarked                       listtest                       dicttest
+279          280         1       3  Abbott, Mrs. Stanton (Rosa...  female  35.0      1      1  C.A. 2673  20.25   NaN        S  [[[93, 85], [93, 85], [93,...  {37: 16, 68: 58, 42: 7, 20...
+
+
+
+df.shortloc_in_iter('dicttest', 65).shortloc_not_in_iter('listtest', [77,65,80,83])
+     PassengerId  Survived  Pclass                           Name     Sex   Age  SibSp  Parch       Ticket      Fare        Cabin Embarked                       listtest                       dicttest
+515          516         0       1   Walker, Mr. William Anderson    male  47.0      0      0        36967   34.0208          D46        S  [[[55, 13], [55, 13], [55,...  {67: 25, 73: 76, 93: 74, 6...
+772          773         0       2              Mack, Mrs. (Mary)  female  57.0      0      0  S.O./P.P. 3   10.5000          E77        S  [[[3, 67], [3, 67], [3, 67...  {20: 62, 88: 78, 22: 65, 1...
+518          519         1       2  Angle, Mrs. William A (Flo...  female  36.0      1      0       226875   26.0000          NaN        S         [[[78, 94], [78, 94]]]  {32: 53, 48: 66, 20: 5, 67...
+10            11         1       3  Sandstrom, Miss. Marguerit...  female   4.0      1      1      PP 9549   16.7000           G6        S  [[[28, 63], [28, 63], [28,...  {12: 80, 63: 96, 79: 99, 5...
+275          276         1       1  Andrews, Miss. Kornelia Th...  female  63.0      1      0        13502   77.9583           D7        S                   [[[84, 21]]]  {31: 95, 27: 48, 89: 25, 6...
+788          789         1       3     Dean, Master. Bertram Vere    male   1.0      1      2    C.A. 2315   20.5750          NaN        S  [[[27, 72], [27, 72], [27,...       {58: 65, 42: 92, 61: 72}
+
+
+
+df.shortloc_not_isna("Cabin").shortloc_str("Cabin", "C").shortloc_not_regex(
+   "Cabin", "^.{4,}$"
+)
+     PassengerId  Survived  Pclass                           Name     Sex   Age  SibSp  Parch    Ticket      Fare Cabin Embarked                       listtest                       dicttest
+1              2         1       1  Cumings, Mrs. John Bradley...  female  38.0      1      0  PC 17599   71.2833   C85        C  [[[31, 68], [31, 68], [31,...                        {9: 77}
+269          270         1       1         Bissette, Miss. Amelia  female  35.0      0      0  PC 17760  135.6333   C99        S  [[[89, 54], [89, 54], [89,...  {50: 9, 91: 60, 30: 67, 46...
+527          528         0       1             Farthing, Mr. John    male   NaN      0      0  PC 17483  221.7792   C95        S  [[[9, 72], [9, 72], [9, 72...               {41: 24, 63: 10}
+151          152         1       1  Pears, Mrs. Thomas (Edith ...  female  22.0      1      0    113776   66.6000    C2        S  [[[24, 98], [24, 98], [24,...  {80: 92, 25: 89, 32: 82, 1...
+412          413         1       1         Minahan, Miss. Daisy E  female  33.0      1      0     19928   90.0000   C78        Q                    [[[2, 41]]]                       {57: 41}
+544          545         0       1     Douglas, Mr. Walter Donald    male  50.0      1      0  PC 17761  106.4250   C86        C  [[[55, 21], [55, 21], [55,...               {51: 49, 16: 20}
+550          551         1       1    Thayer, Mr. John Borland Jr    male  17.0      0      2     17421  110.8833   C70        C  [[[37, 20], [37, 20], [37,...               {17: 85, 49: 77}
+430          431         1       1  Bjornstrom-Steffansson, Mr...    male  28.0      0      0    110564   26.5500   C52        S  [[[14, 61], [14, 61], [14,...                       {62: 40}
+
+
+df.shortloc_in_iter('listtest',[99, 77]).shortloc_regex('listtest',r"7\b,\s*\b9"))
+     PassengerId  Survived  Pclass                  Name     Sex   Age  SibSp  Parch Ticket     Fare Cabin Embarked                       listtest                       dicttest
+111          112         0       3  Zabour, Miss. Hileni  female  14.5      1      0   2665  14.4542   NaN        C  [[[27, 99], [27, 99], [27,...  {76: 81, 62: 60, 98: 43, 5...
+
+
+#all methods can also be used against Series
+#Two examples
+
+df.Pclass.shortloc_regex('^2$')
+Out[54]: 
+9      2
+15     2
+17     2
+20     2
+21     2
+      ..
+
+df.Pclass.shortloc_regex_replace('^3$',2000)
+Out[56]: 
+0      2000
+1         1
+2      2000
+3         1
+4      2000
+       ... 
 ```
```

### Comparing `a_pandas_ex_easy_loc-0.13/README.md` & `a_pandas_ex_easy_loc-0.14/README.md`

 * *Files identical despite different names*

### Comparing `a_pandas_ex_easy_loc-0.13/a_pandas_ex_easy_loc/README.md` & `a_pandas_ex_easy_loc-0.14/a_pandas_ex_easy_loc/README.md`

 * *Files identical despite different names*

### Comparing `a_pandas_ex_easy_loc-0.13/a_pandas_ex_easy_loc/__init__.py` & `a_pandas_ex_easy_loc-0.14/a_pandas_ex_easy_loc/__init__.py`

 * *Files identical despite different names*

### Comparing `a_pandas_ex_easy_loc-0.13/a_pandas_ex_easy_loc/thirdparty.json` & `a_pandas_ex_easy_loc-0.14/a_pandas_ex_easy_loc/thirdparty.json`

 * *Files identical despite different names*

### Comparing `a_pandas_ex_easy_loc-0.13/a_pandas_ex_easy_loc.egg-info/PKG-INFO` & `a_pandas_ex_easy_loc-0.14/a_pandas_ex_easy_loc.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,469 +1,468 @@
 Metadata-Version: 2.1
 Name: a-pandas-ex-easy-loc
-Version: 0.13
+Version: 0.14
 Summary: Search and replace values with df.loc without Exceptions due to dtype incompatibility
 Home-page: https://github.com/hansalemaos/a_pandas_ex_easy_loc
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: loc,iloc,df.at,df.iat,pandas,DataFrame,Series
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE.rst
 
+### A tolerant version of df.loc
 
-### A tolerant version of df.loc
-
-Search and replace values with df.loc without Exceptions due to dtype incompatibility.  If the dtypes of 2 variables don't match, they will be converted until they match. 
-
-```python
-pip install a_pandas_ex_easy_loc
-```
-
-Some examples
-
-```python
-import pandas as pd
-df = pd.read_csv("https://github.com/pandas-dev/pandas/raw/main/doc/data/titanic.csv")
-# df.loc[df.Ticket >20000]
-from random import randrange
-getrandomlist = lambda x: [
-  [[randrange(1, 100), randrange(1, 100)] * 1] * randrange(1, 10)
-]
-df["listtest"] = df.PassengerId.map(getrandomlist)
-
-
-getrandomdict = lambda x: {
-  randrange(1, 100):randrange(1, 100) for _ in range(randrange(1, 10))
-}
-df["dicttest"] = df.PassengerId.map(getrandomdict)
-from a_easy_loc import pd_add_easy_loc
-pd_add_easy_loc()
-df.shortloc_greater_replace('Pclass', 2,3000)
-
-df.shortloc_equal('Pclass', 3)
-     PassengerId  Survived  Pclass       Name     Sex    Age  SibSp  Parch     Ticket     Fare  Cabin Embarked   listtest   dicttest
-0            1           0       3  Braund...    male  22.00      1      0  A/5 21171   7.2500    NaN        S  [[[44,...  {5: 8,...
-2            3           1       3  Heikki...  female  26.00      0      0  STON/O...   7.9250    NaN        S  [[[60,...  {33: 3...
-4            5           0       3  Allen,...    male  35.00      0      0     373450   8.0500    NaN        S  [[[99,...  {96: 1...
-5            6           0       3  Moran,...    male    NaN      0      0     330877   8.4583    NaN        Q  [[[82,...  {23: 1...
-7            8           0       3  Palsso...    male   2.00      3      1     349909  21.0750    NaN        S  [[[14,...  {20: 8...
-8            9           1       3  Johnso...  female  27.00      0      2     347742  11.1333    NaN        S  [[[12,...  {96: 5...
-
-
-df.shortloc_equal('Ticket', 373450)
-   PassengerId  Survived  Pclass       Name   Sex   Age  SibSp  Parch  Ticket  Fare Cabin Embarked   listtest   dicttest
-4          5           0       3  Allen,...  male  35.0      0      0  373450  8.05   NaN        S  [[[99,...  {96: 1...
-
-
-df.shortloc_greater('Pclass', 2)
-     PassengerId  Survived  Pclass       Name     Sex    Age  SibSp  Parch     Ticket     Fare  Cabin Embarked   listtest   dicttest
-0            1           0       3  Braund...    male  22.00      1      0  A/5 21171   7.2500    NaN        S  [[[44,...  {5: 8,...
-2            3           1       3  Heikki...  female  26.00      0      0  STON/O...   7.9250    NaN        S  [[[60,...  {33: 3...
-4            5           0       3  Allen,...    male  35.00      0      0     373450   8.0500    NaN        S  [[[99,...  {96: 1...
-5            6           0       3  Moran,...    male    NaN      0      0     330877   8.4583    NaN        Q  [[[82,...  {23: 1...
-
-df.shortloc_greater('Ticket', 373450)
-     PassengerId  Survived  Pclass       Name     Sex   Age  SibSp  Parch   Ticket     Fare Cabin Embarked   listtest   dicttest
-16          17           0       3  Rice, ...    male   2.0      4      1   382652  29.1250   NaN        Q  [[[17,...  {46: 7...
-50          51           0       3  Panula...    male   7.0      4      1  3101295  39.6875   NaN        S  [[[30,...  {64: 2...
-68          69           1       3  Anders...  female  17.0      4      2  3101281   7.9250   NaN        S  [[[4, ...  {92: 3...
-77          78           0       3  Moutal...    male   NaN      0      0   374746   8.0500   NaN        S  [[[65,...  {47: 9...
-85          86           1       3  Backst...  female  33.0      3      0  3101278  15.8500   NaN        S  [[[55,...  {5: 22...
-
-
-df.shortloc_greater_or_equal('Age', 43)
-     PassengerId  Survived  Pclass       Name     Sex   Age  SibSp  Parch     Ticket      Fare      Cabin Embarked   listtest   dicttest
-6            7           0       1  McCart...    male  54.0      0      0      17463   51.8625        E46        S  [[[47,...   {22: 17}
-11          12           1       1  Bonnel...  female  58.0      0      0     113783   26.5500       C103        S  [[[1, ...    {35: 9}
-15          16           1       2  Hewlet...  female  55.0      0      0     248706   16.0000        NaN        S  [[[43,...  {40: 6...
-33          34           0       2  Wheado...    male  66.0      0      0  C.A. 2...   10.5000        NaN        S  [[[6, ...   {50: 28}
-52          53           1       1  Harper...  female  49.0      1      0   PC 17572   76.7292        D33        C  [[[41,...  {54: 6...
-
-
-df.shortloc_greater_replace('Pclass', 2,3000)
-     PassengerId  Survived  Pclass       Name     Sex    Age  SibSp  Parch     Ticket      Fare      Cabin Embarked   listtest   dicttest
-0            1           0    3000  Braund...    male  22.00      1      0  A/5 21171    7.2500        NaN        S  [[[65,...  {76: 3...
-1            2           1       1  Cuming...  female  38.00      1      0   PC 17599   71.2833        C85        C  [[[1, ...  {55: 3...
-2            3           1    3000  Heikki...  female  26.00      0      0  STON/O...    7.9250        NaN        S  [[[56,...  {7: 54...
-3            4           1       1  Futrel...  female  35.00      1      0     113803   53.1000       C123        S  [[[91,...   {51: 89}
-4            5           0    3000  Allen,...    male  35.00      0      0     373450    8.0500        NaN        S  [[[20,...  {39: 5...
-5            6           0    3000  Moran,...    male    NaN      0      0     330877    8.4583        NaN        Q  [[[60,...  {63: 2...
-6            7           0       1  McCart...    male  54.00      0      0      17463   51.8625        E46        S  [[[51,...  {1: 90...
-
-
-
-df.shortloc_greater_replace('Ticket', 5000, 888000)
-     PassengerId  Survived  Pclass       Name     Sex    Age  SibSp  Parch     Ticket      Fare      Cabin Embarked   listtest   dicttest
-0            1           0       3  Braund...    male  22.00      1      0  A/5 21171    7.2500        NaN        S  [[[74,...  {40: 3...
-1            2           1       1  Cuming...  female  38.00      1      0   PC 17599   71.2833        C85        C  [[[67,...     {1: 8}
-2            3           1       3  Heikki...  female  26.00      0      0  STON/O...    7.9250        NaN        S  [[[62,...   {39: 79}
-3            4           1       1  Futrel...  female  35.00      1      0     888000   53.1000       C123        S  [[[15,...  {13: 2...
-4            5           0       3  Allen,...    male  35.00      0      0     888000    8.0500        NaN        S  [[[81,...   {60: 90}
-5            6           0       3  Moran,...    male    NaN      0      0     888000    8.4583        NaN        Q  [[[58,...    {20: 4}
-6            7           0       1  McCart...    male  54.00      0      0     888000   51.8625        E46        S  [[[28,...  {21: 8...
-7            8           0       3  Palsso...    male   2.00      3      1     888000   21.0750        NaN        S  [[[25,...  {53: 8...
-8            9           1       3  Johnso...  female  27.00      0      2     888000   11.1333        NaN        S  [[[47,...  {19: 3...
-
-
-df.shortloc_greater_replace('Cabin','C123', pd.NA)
-     PassengerId  Survived  Pclass       Name     Sex    Age  SibSp  Parch     Ticket      Fare      Cabin Embarked   listtest   dicttest
-0            1           0       3  Braund...    male  22.00      1      0  A/5 21171    7.2500        NaN        S  [[[74,...  {40: 3...
-1            2           1       1  Cuming...  female  38.00      1      0   PC 17599   71.2833       <NA>        C  [[[67,...     {1: 8}
-2            3           1       3  Heikki...  female  26.00      0      0  STON/O...    7.9250        NaN        S  [[[62,...   {39: 79}
-3            4           1       1  Futrel...  female  35.00      1      0     113803   53.1000       C123        S  [[[15,...  {13: 2...
-4            5           0       3  Allen,...    male  35.00      0      0     373450    8.0500        NaN        S  [[[81,...   {60: 90}
-5            6           0       3  Moran,...    male    NaN      0      0     330877    8.4583        NaN        Q  [[[58,...    {20: 4}
-6            7           0       1  McCart...    male  54.00      0      0      17463   51.8625       <NA>        S  [[[28,...  {21: 8...
-7            8           0       3  Palsso...    male   2.00      3      1     349909   21.0750        NaN        S  [[[25,...  {53: 8...
-
-df.shortloc_in_iter('listtest', 3)
-     PassengerId  Survived  Pclass                 Name     Sex   Age  SibSp  Parch        Ticket     Fare Cabin Embarked             listtest             dicttest
-19            20         1       3  Masselmani, Mrs....  female   NaN      0      0          2649   7.2250   NaN        C  [[[32, 3], [32, ...  {98: 75, 69: 39,...
-66            67         1       2  Nye, Mrs. (Eliza...  female  29.0      0      0    C.A. 29395  10.5000   F33        S  [[[3, 98], [3, 9...             {60: 81}
-92            93         0       1  Chaffee, Mr. Her...    male  46.0      1      0   W.E.P. 5734  61.1750   E31        S  [[[52, 3], [52, ...             {80: 25}
-106          107         1       3  Salkjelsvik, Mis...  female  21.0      0      0        343120   7.6500   NaN        S  [[[85, 3], [85, ...             {62: 49}
-120          121         0       2  Hickman, Mr. Sta...    male  21.0      2      0  S.O.C. 14879  73.5000   NaN        S  [[[40, 3], [40, ...  {28: 85, 60: 72,...
-129          130         0       3   Ekstrom, Mr. Johan    male  45.0      0      0        347061   6.9750   NaN        S  [[[3, 76], [3, 7...  {79: 2, 30: 18, ...
-132          133         0       3  Robins, Mrs. Ale...  female  47.0      1      0     A/5. 3337  14.5000   NaN        S  [[[3, 68], [3, 6...  {69: 90, 1: 23, ...
-184          185         1       3  Kink-Heilmann, M...  female   4.0      0      2        315153  22.0250   NaN        S  [[[3, 88], [3, 8...  {24: 74, 30: 11,...
-
-df.shortloc_in_iter('listtest', [3,4,10])
-     PassengerId  Survived  Pclass                 Name     Sex    Age  SibSp  Parch           Ticket      Fare        Cabin Embarked             listtest             dicttest
-19            20         1       3  Masselmani, Mrs....  female    NaN      0      0             2649    7.2250          NaN        C  [[[32, 3], [32, ...  {98: 75, 69: 39,...
-22            23         1       3  McGowan, Miss. A...  female  15.00      0      0           330923    8.0292          NaN        Q  [[[13, 4], [13, ...  {56: 86, 30: 5, ...
-27            28         0       1  Fortune, Mr. Cha...    male  19.00      3      2            19950  263.0000  C23 C25 C27        S  [[[4, 66], [4, 6...  {58: 98, 32: 55,...
-66            67         1       2  Nye, Mrs. (Eliza...  female  29.00      0      0       C.A. 29395   10.5000          F33        S  [[[3, 98], [3, 9...             {60: 81}
-74            75         1       3        Bing, Mr. Lee    male  32.00      0      0             1601   56.4958          NaN        S  [[[14, 4], [14, ...  {31: 31, 64: 38,...
-84            85         1       2  Ilett, Miss. Bertha  female  17.00      0      0       SO/C 14885   10.5000          NaN        S  [[[18, 10], [18,...  {81: 64, 10: 80,...
-
-
-df.shortloc_in_iter('dicttest', [3,4,10])
-     PassengerId  Survived  Pclass                           Name     Sex    Age  SibSp  Parch             Ticket      Fare            Cabin Embarked                       listtest                       dicttest
-5              6         0       3               Moran, Mr. James    male    NaN      0      0             330877    8.4583              NaN        Q         [[[58, 72], [58, 72]]]                        {20: 4}
-8              9         1       3  Johnson, Mrs. Oscar W (Eli...  female  27.00      0      2             347742   11.1333              NaN        S         [[[47, 12], [47, 12]]]         {19: 3, 60: 24, 9: 38}
-
-
-df.shortloc_in_iter('dicttest', [3,4,10])
-     PassengerId  Survived  Pclass                          Name     Sex   Age  SibSp  Parch         Ticket     Fare Cabin Embarked                                                           listtest                                                               dicttest
-96            97         0       1     Goldschmidt, Mr. George B    male  71.0      0      0       PC 17754  34.6542    A5        C           [[[94, 4], [94, 4], [94, 4], [94, 4], [94, 4], [94, 4]]]       {67: 92, 24: 19, 53: 40, 66: 53, 44: 81, 94: 10, 34: 63, 61: 45}
-103          104         0       3    Johansson, Mr. Gustaf Joel    male  33.0      0      0           7540   8.6542   NaN        S               [[[89, 10], [89, 10], [89, 10], [89, 10], [89, 10]]]                                        {92: 23, 32: 17, 53: 3, 98: 94}
-129          130         0       3            Ekstrom, Mr. Johan    male  45.0      0      0         347061   6.9750   NaN        S  [[[3, 76], [3, 76], [3, 76], [3, 76], [3, 76], [3, 76], [3, 76]]]   {79: 2, 30: 18, 63: 10, 62: 26, 91: 58, 11: 44, 8: 81, 6: 93, 97: 5}
-
-
-df.shortloc_in_iter_replace('dicttest', [3,4,10], 15151515)
-     PassengerId  Survived  Pclass                           Name     Sex    Age  SibSp  Parch              Ticket      Fare            Cabin Embarked                       listtest                       dicttest
-0              1         0       3        Braund, Mr. Owen Harris    male  22.00      1      0           A/5 21171    7.2500              NaN        S  [[[74, 68], [74, 68], [74,...  {40: 30, 93: 84, 24: 92, 7...
-1              2         1       1  Cumings, Mrs. John Bradley...  female  38.00      1      0            PC 17599   71.2833              C85        C  [[[67, 64], [67, 64], [67,...                         {1: 8}
-2              3         1       3         Heikkinen, Miss. Laina  female  26.00      0      0    STON/O2. 3101282    7.9250              NaN        S  [[[62, 65], [62, 65], [62,...                       {39: 79}
-3              4         1       1  Futrelle, Mrs. Jacques Hea...  female  35.00      1      0              113803   53.1000             C123        S  [[[15, 96], [15, 96], [15,...       {13: 29, 65: 59, 99: 31}
-4              5         0       3       Allen, Mr. William Henry    male  35.00      0      0              373450    8.0500              NaN        S                   [[[81, 13]]]                       {60: 90}
-5              6         0       3               Moran, Mr. James    male    NaN      0      0              330877    8.4583              NaN        Q         [[[58, 72], [58, 72]]]                       15151515
-6              7         0       1        McCarthy, Mr. Timothy J    male  54.00      0      0               17463   51.8625              E46        S  [[[28, 98], [28, 98], [28,...  {21: 8, 31: 42, 9: 40, 93:...
-7              8         0       3  Palsson, Master. Gosta Leo...    male   2.00      3      1              349909   21.0750              NaN        S  [[[25, 88], [25, 88], [25,...  {53: 83, 49: 66, 57: 95, 4...
-8              9         1       3  Johnson, Mrs. Oscar W (Eli...  female  27.00      0      2              347742   11.1333              NaN        S         [[[47, 12], [47, 12]]]                       15151515
-
-df.shortloc_isin('Embarked', ['C', 'S'])
-     PassengerId  Survived  Pclass                           Name     Sex    Age  SibSp  Parch              Ticket      Fare            Cabin Embarked                       listtest                       dicttest
-0              1         0       3        Braund, Mr. Owen Harris    male  22.00      1      0           A/5 21171    7.2500              NaN        S  [[[74, 68], [74, 68], [74,...  {40: 30, 93: 84, 24: 92, 7...
-1              2         1       1  Cumings, Mrs. John Bradley...  female  38.00      1      0            PC 17599   71.2833              C85        C  [[[67, 64], [67, 64], [67,...                         {1: 8}
-2              3         1       3         Heikkinen, Miss. Laina  female  26.00      0      0    STON/O2. 3101282    7.9250              NaN        S  [[[62, 65], [62, 65], [62,...                       {39: 79}
-3              4         1       1  Futrelle, Mrs. Jacques Hea...  female  35.00      1      0              113803   53.1000             C123        S  [[[15, 96], [15, 96], [15,...       {13: 29, 65: 59, 99: 31}
-4              5         0       3       Allen, Mr. William Henry    male  35.00      0      0              373450    8.0500              NaN        S                   [[[81, 13]]]                       {60: 90}
-6              7         0       1        McCarthy, Mr. Timothy J    male  54.00      0      0               17463   51.8625              E46        S  [[[28, 98], [28, 98], [28,...  {21: 8, 31: 42, 9: 40, 93:...
-7              8         0       3  Palsson, Master. Gosta Leo...    male   2.00      3      1              349909   21.0750              NaN        S  [[[25, 88], [25, 88], [25,...  {53: 83, 49: 66, 57: 95, 4...
-8              9         1       3  Johnson, Mrs. Oscar W (Eli...  female  27.00      0      2              347742   11.1333              NaN        S         [[[47, 12], [47, 12]]]         {19: 3, 60: 24, 9: 38}
-
-df.shortloc_isin_replace('Embarked', ['C', 'S'], 'CCCCCCCCCCCCCCCCCCCSSSSSSSSSSSSSSSSSSSSSSSSSSSSS')
-     PassengerId  Survived  Pclass       Name     Sex    Age  SibSp  Parch     Ticket      Fare      Cabin   Embarked   listtest   dicttest
-0            1           0       3  Braund...    male  22.00      1      0  A/5 21171    7.2500        NaN  CCCCCC...  [[[74,...  {40: 3...
-1            2           1       1  Cuming...  female  38.00      1      0   PC 17599   71.2833        C85  CCCCCC...  [[[67,...     {1: 8}
-2            3           1       3  Heikki...  female  26.00      0      0  STON/O...    7.9250        NaN  CCCCCC...  [[[62,...   {39: 79}
-3            4           1       1  Futrel...  female  35.00      1      0     113803   53.1000       C123  CCCCCC...  [[[15,...  {13: 2...
-4            5           0       3  Allen,...    male  35.00      0      0     373450    8.0500        NaN  CCCCCC...  [[[81,...   {60: 90}
-5            6           0       3  Moran,...    male    NaN      0      0     330877    8.4583        NaN          Q  [[[58,...    {20: 4}
-
-
-df.shortloc_isna('Age')
-     PassengerId  Survived  Pclass                           Name     Sex  Age  SibSp  Parch              Ticket      Fare  Cabin Embarked                       listtest                       dicttest
-5              6         0       3               Moran, Mr. James    male  NaN      0      0              330877    8.4583    NaN        Q         [[[25, 39], [25, 39]]]       {97: 78, 85: 88, 42: 34}
-17            18         1       2   Williams, Mr. Charles Eugene    male  NaN      0      0              244373   13.0000    NaN        S  [[[17, 6], [17, 6], [17, 6...                 {41: 6, 2: 82}
-19            20         1       3        Masselmani, Mrs. Fatima  female  NaN      0      0                2649    7.2250    NaN        C  [[[11, 37], [11, 37], [11,...  {43: 73, 50: 28, 38: 47, 4...
-26            27         0       3        Emir, Mr. Farred Chehab    male  NaN      0      0                2631    7.2250    NaN        C  [[[48, 66], [48, 66], [48,...               {33: 45, 82: 90}
-28            29         1       3  O'Dwyer, Miss. Ellen "Nellie"  female  NaN      0      0              330959    7.8792    NaN        Q           [[[3, 53], [3, 53]]]               {29: 90, 84: 86}
-29            30         0       3            Todoroff, Mr. Lalio    male  NaN      0      0              349216    7.8958    NaN        S  [[[67, 3], [67, 3], [67, 3...  {57: 49, 23: 71, 64: 45, 1...
-31            32         1       1  Spencer, Mrs. William Augu...  female  NaN      1      0            PC 17569  146.5208    B78        C  [[[88, 94], [88, 94], [88,...  {4: 42, 98: 58, 94: 7, 39:...
-
-
-df.shortloc_isna_replace('Age',16541)
-     PassengerId  Survived  Pclass                           Name     Sex       Age  SibSp  Parch              Ticket      Fare            Cabin Embarked                       listtest                       dicttest
-0              1         0       3        Braund, Mr. Owen Harris    male     22.00      1      0           A/5 21171    7.2500              NaN        S  [[[27, 71], [27, 71], [27,...  {36: 67, 73: 54, 56: 48, 8...
-1              2         1       1  Cumings, Mrs. John Bradley...  female     38.00      1      0            PC 17599   71.2833              C85        C  [[[31, 68], [31, 68], [31,...                        {9: 77}
-2              3         1       3         Heikkinen, Miss. Laina  female     26.00      0      0    STON/O2. 3101282    7.9250              NaN        S                   [[[31, 23]]]  {49: 6, 76: 22, 52: 18, 6:...
-3              4         1       1  Futrelle, Mrs. Jacques Hea...  female     35.00      1      0              113803   53.1000             C123        S  [[[96, 48], [96, 48], [96,...  {27: 90, 9: 38, 18: 94, 67...
-4              5         0       3       Allen, Mr. William Henry    male     35.00      0      0              373450    8.0500              NaN        S  [[[60, 84], [60, 84], [60,...  {8: 61, 37: 4, 25: 43, 21:...
-5              6         0       3               Moran, Mr. James    male  16541.00      0      0              330877    8.4583              NaN        Q         [[[25, 39], [25, 39]]]       {97: 78, 85: 88, 42: 34}
-6              7         0       1        McCarthy, Mr. Timothy J    male     54.00      0      0               17463   51.8625              E46        S  [[[76, 5], [76, 5], [76, 5...  {56: 51, 13: 24, 84: 24, 9...
-
-df.shortloc_less('Ticket', 7534)
-
-     PassengerId  Survived  Pclass                           Name     Sex    Age  SibSp  Parch Ticket     Fare        Cabin Embarked                       listtest                       dicttest
-19            20         1       3        Masselmani, Mrs. Fatima  female    NaN      0      0   2649   7.2250          NaN        C  [[[11, 37], [11, 37], [11,...  {43: 73, 50: 28, 38: 47, 4...
-26            27         0       3        Emir, Mr. Farred Chehab    male    NaN      0      0   2631   7.2250          NaN        C  [[[48, 66], [48, 66], [48,...               {33: 45, 82: 90}
-36            37         1       3               Mamee, Mr. Hanna    male    NaN      0      0   2677   7.2292          NaN        C  [[[84, 24], [84, 24], [84,...  {39: 19, 88: 50, 23: 7, 53...
-39            40         1       3    Nicola-Yarred, Miss. Jamila  female  14.00      1      0   2651  11.2417          NaN        C  [[[20, 72], [20, 72], [20,...  {72: 91, 81: 15, 89: 24, 9...
-48            49         0       3            Samaan, Mr. Youssef    male    NaN      2      0   2662  21.6792          NaN        C  [[[79, 85], [79, 85], [79,...                       {35: 61}
-53            54         1       2  Faunthorpe, Mrs. Lizzie (E...  female  29.00      1      0   2926  26.0000          NaN        S         [[[62, 79], [62, 79]]]  {36: 53, 38: 70, 6: 1, 89:...
-57            58         0       3            Novel, Mr. Mansouer    male  28.50      0      0   2697   7.2292          NaN        C         [[[86, 78], [86, 78]]]                {28: 5, 49: 22}
-60            61         0       3          Sirayanian, Mr. Orsen    male  22.00      0      0   2669   7.2292          NaN        C                   [[[24, 72]]]  {74: 59, 16: 44, 30: 17, 5...
-65            66         1       3       Moubarek, Master. Gerios    male    NaN      1      1   2661  15.2458          NaN        C  [[[56, 96], [56, 96], [56,...  {5: 34, 59: 97, 78: 15, 76...
-73            74         0       3    Chronopoulos, Mr. Apostolos    male  26.00      1      0   2680  14.4542          NaN        C         [[[78, 24], [78, 24]]]  {96: 26, 87: 73, 58: 49, 3...
-74            75         1       3                  Bing, Mr. Lee    male  32.00      0      0   1601  56.4958          NaN        S  [[[86, 20], [86, 20], [86,...  {84: 87, 18: 40, 17: 28, 7...
-
-
-df.shortloc_less_replace('Age', 30, 'less 30')
-     PassengerId  Survived  Pclass                           Name     Sex      Age  SibSp  Parch              Ticket      Fare            Cabin Embarked                       listtest                       dicttest
-0              1         0       3        Braund, Mr. Owen Harris    male  less 30      1      0           A/5 21171    7.2500              NaN        S  [[[27, 71], [27, 71], [27,...  {36: 67, 73: 54, 56: 48, 8...
-1              2         1       1  Cumings, Mrs. John Bradley...  female     38.0      1      0            PC 17599   71.2833              C85        C  [[[31, 68], [31, 68], [31,...                        {9: 77}
-2              3         1       3         Heikkinen, Miss. Laina  female  less 30      0      0    STON/O2. 3101282    7.9250              NaN        S                   [[[31, 23]]]  {49: 6, 76: 22, 52: 18, 6:...
-3              4         1       1  Futrelle, Mrs. Jacques Hea...  female     35.0      1      0              113803   53.1000             C123        S  [[[96, 48], [96, 48], [96,...  {27: 90, 9: 38, 18: 94, 67...
-
-
-df.shortloc_less_or_equal_replace('Survived', 0, 'DEAD')
-     PassengerId Survived  Pclass                           Name     Sex    Age  SibSp  Parch              Ticket      Fare            Cabin Embarked                       listtest                       dicttest
-0              1     DEAD       3        Braund, Mr. Owen Harris    male  22.00      1      0           A/5 21171    7.2500              NaN        S  [[[27, 71], [27, 71], [27,...  {36: 67, 73: 54, 56: 48, 8...
-1              2        1       1  Cumings, Mrs. John Bradley...  female  38.00      1      0            PC 17599   71.2833              C85        C  [[[31, 68], [31, 68], [31,...                        {9: 77}
-2              3        1       3         Heikkinen, Miss. Laina  female  26.00      0      0    STON/O2. 3101282    7.9250              NaN        S                   [[[31, 23]]]  {49: 6, 76: 22, 52: 18, 6:...
-3              4        1       1  Futrelle, Mrs. Jacques Hea...  female  35.00      1      0              113803   53.1000             C123        S  [[[96, 48], [96, 48], [96,...  {27: 90, 9: 38, 18: 94, 67...
-4              5     DEAD       3       Allen, Mr. William Henry    male  35.00      0      0              373450    8.0500              NaN        S  [[[60, 84], [60, 84], [60,...  {8: 61, 37: 4, 25: 43, 21:...
-5              6     DEAD       3               Moran, Mr. James    male    NaN      0      0              330877    8.4583              NaN        Q         [[[25, 39], [25, 39]]]       {97: 78, 85: 88, 42: 34}
-6              7     DEAD       1        McCarthy, Mr. Timothy J    male  54.00      0      0               17463   51.8625              E46        S  [[[76, 5], [76, 5], [76, 5...  {56: 51, 13: 24, 84: 24, 9...
-7              8     DEAD       3  Palsson, Master. Gosta Leo...    male   2.00      3      1              349909   21.0750              NaN        S  [[[42, 52], [42, 52], [42,...               {71: 69, 44: 14}
-
-
-
-df.shortloc_not_equal_replace('Survived', 0, True)
-     PassengerId Survived  Pclass                           Name     Sex    Age  SibSp  Parch              Ticket      Fare            Cabin Embarked                       listtest                       dicttest
-0              1        0       3        Braund, Mr. Owen Harris    male  22.00      1      0           A/5 21171    7.2500              NaN        S  [[[27, 71], [27, 71], [27,...  {36: 67, 73: 54, 56: 48, 8...
-1              2     True       1  Cumings, Mrs. John Bradley...  female  38.00      1      0            PC 17599   71.2833              C85        C  [[[31, 68], [31, 68], [31,...                        {9: 77}
-2              3     True       3         Heikkinen, Miss. Laina  female  26.00      0      0    STON/O2. 3101282    7.9250              NaN        S                   [[[31, 23]]]  {49: 6, 76: 22, 52: 18, 6:...
-3              4     True       1  Futrelle, Mrs. Jacques Hea...  female  35.00      1      0              113803   53.1000             C123        S  [[[96, 48], [96, 48], [96,...  {27: 90, 9: 38, 18: 94, 67...
-4              5        0       3       Allen, Mr. William Henry    male  35.00      0      0              373450    8.0500              NaN        S  [[[60, 84], [60, 84], [60,...  {8: 61, 37: 4, 25: 43, 21:...
-5              6        0       3               Moran, Mr. James    male    NaN      0      0              330877    8.4583              NaN        Q         [[[25, 39], [25, 39]]]       {97: 78, 85: 88, 42: 34}
-
-
-
-df.shortloc_not_in_iter('listtest', list(range(0,90)))
-     PassengerId  Survived  Pclass                           Name     Sex   Age  SibSp  Parch      Ticket      Fare Cabin Embarked                       listtest                       dicttest
-832          833         0       3                 Saad, Mr. Amin    male   NaN      0      0        2671    7.2292   NaN        C  [[[95, 94], [95, 94], [95,...                {82: 66, 84: 5}
-484          485         1       1        Bishop, Mr. Dickinson H    male  25.0      1      0       11967   91.0792   B49        C  [[[97, 92], [97, 92], [97,...  {20: 34, 2: 23, 98: 37, 1:...
-581          582         1       1  Thayer, Mrs. John Borland ...  female  39.0      1      1       17421  110.8833   C68        C         [[[91, 90], [91, 90]]]  {48: 98, 3: 98, 93: 4, 97:...
-336          337         0       1      Pears, Mr. Thomas Clinton    male  29.0      1      0      113776   66.6000    C2        S         [[[90, 98], [90, 98]]]                         {6: 7}
-116          117         0       3           Connors, Mr. Patrick    male  70.5      0      0      370369    7.7500   NaN        Q  [[[92, 99], [92, 99], [92,...  {60: 79, 75: 71, 28: 68, 5...
-52            53         1       1  Harper, Mrs. Henry Sleeper...  female  49.0      1      0    PC 17572   76.7292   D33        C  [[[96, 94], [96, 94], [96,...  {20: 53, 93: 11, 83: 79, 5...
-439          440         0       2  Kvillner, Mr. Johan Henrik...    male  31.0      0      0  C.A. 18723   10.5000   NaN        S  [[[95, 98], [95, 98], [95,...  {58: 11, 89: 23, 22: 66, 1...
-56            57         1       2              Rugg, Miss. Emily  female  21.0      0      0  C.A. 31026   10.5000   NaN        S  [[[92, 92], [92, 92], [92,...                {45: 1, 37: 98}
-
-
-
-df.shortloc_not_in_iter_replace('listtest', list(range(0,20)), 27)
-     PassengerId  Survived  Pclass                           Name     Sex    Age  SibSp  Parch              Ticket      Fare            Cabin Embarked                       listtest                       dicttest
-0              1         0       3        Braund, Mr. Owen Harris    male  22.00      1      0           A/5 21171    7.2500              NaN        S                             27  {36: 67, 73: 54, 56: 48, 8...
-1              2         1       1  Cumings, Mrs. John Bradley...  female  38.00      1      0            PC 17599   71.2833              C85        C                             27                        {9: 77}
-2              3         1       3         Heikkinen, Miss. Laina  female  26.00      0      0    STON/O2. 3101282    7.9250              NaN        S                             27  {49: 6, 76: 22, 52: 18, 6:...
-3              4         1       1  Futrelle, Mrs. Jacques Hea...  female  35.00      1      0              113803   53.1000             C123        S                             27  {27: 90, 9: 38, 18: 94, 67...
-4              5         0       3       Allen, Mr. William Henry    male  35.00      0      0              373450    8.0500              NaN        S                             27  {8: 61, 37: 4, 25: 43, 21:...
-5              6         0       3               Moran, Mr. James    male    NaN      0      0              330877    8.4583              NaN        Q                             27       {97: 78, 85: 88, 42: 34}
-6              7         0       1        McCarthy, Mr. Timothy J    male  54.00      0      0               17463   51.8625              E46        S  [[[76, 5], [76, 5], [76, 5...  {56: 51, 13: 24, 84: 24, 9...
-
-
-df.shortloc_regex('Fare', r'^\d?7\.').to_string(max_colwidth=30)
-     PassengerId  Survived  Pclass                           Name     Sex   Age  SibSp  Parch              Ticket     Fare  Cabin Embarked                       listtest                       dicttest
-0              1         0       3        Braund, Mr. Owen Harris    male  22.0      1      0           A/5 21171   7.2500    NaN        S  [[[27, 71], [27, 71], [27,...  {36: 67, 73: 54, 56: 48, 8...
-2              3         1       3         Heikkinen, Miss. Laina  female  26.0      0      0    STON/O2. 3101282   7.9250    NaN        S                   [[[31, 23]]]  {49: 6, 76: 22, 52: 18, 6:...
-14            15         0       3  Vestrom, Miss. Hulda Amand...  female  14.0      0      0              350406   7.8542    NaN        S  [[[40, 57], [40, 57], [40,...  {54: 39, 8: 35, 76: 84, 20...
-19            20         1       3        Masselmani, Mrs. Fatima  female   NaN      0      0                2649   7.2250    NaN        C  [[[11, 37], [11, 37], [11,...  {43: 73, 50: 28, 38: 47, 4...
-26            27         0       3        Emir, Mr. Farred Chehab    male   NaN      0      0                2631   7.2250    NaN        C  [[[48, 66], [48, 66], [48,...               {33: 45, 82: 90}
-28            29         1       3  O'Dwyer, Miss. Ellen "Nellie"  female   NaN      0      0              330959   7.8792    NaN        Q           [[[3, 53], [3, 53]]]               {29: 90, 84: 86}
-29            30         0       3            Todoroff, Mr. Lalio    male   NaN      0      0              349216   7.8958    NaN        S  [[[67, 3], [67, 3], [67, 3...  {57: 49, 23: 71, 64: 45, 1...
-30            31         0       1       Uruchurtu, Don. Manuel E    male  40.0      0      0            PC 17601  27.7208    NaN        C  [[[91, 32], [91, 32], [91,...         {1: 29, 54: 93, 96: 7}
-
-
-
-df.shortloc_not_regex('Fare', r'^\d?7\.').to_string(max_colwidth=30)
-     PassengerId  Survived  Pclass                           Name     Sex    Age  SibSp  Parch             Ticket      Fare            Cabin Embarked                       listtest                       dicttest
-1              2         1       1  Cumings, Mrs. John Bradley...  female  38.00      1      0           PC 17599   71.2833              C85        C  [[[31, 68], [31, 68], [31,...                        {9: 77}
-3              4         1       1  Futrelle, Mrs. Jacques Hea...  female  35.00      1      0             113803   53.1000             C123        S  [[[96, 48], [96, 48], [96,...  {27: 90, 9: 38, 18: 94, 67...
-4              5         0       3       Allen, Mr. William Henry    male  35.00      0      0             373450    8.0500              NaN        S  [[[60, 84], [60, 84], [60,...  {8: 61, 37: 4, 25: 43, 21:...
-5              6         0       3               Moran, Mr. James    male    NaN      0      0             330877    8.4583              NaN        Q         [[[25, 39], [25, 39]]]       {97: 78, 85: 88, 42: 34}
-6              7         0       1        McCarthy, Mr. Timothy J    male  54.00      0      0              17463   51.8625              E46        S  [[[76, 5], [76, 5], [76, 5...  {56: 51, 13: 24, 84: 24, 9...
-7              8         0       3  Palsson, Master. Gosta Leo...    male   2.00      3      1             349909   21.0750              NaN        S  [[[42, 52], [42, 52], [42,...               {71: 69, 44: 14}
-8              9         1       3  Johnson, Mrs. Oscar W (Eli...  female  27.00      0      2             347742   11.1333              NaN        S  [[[92, 21], [92, 21], [92,...  {61: 17, 72: 44, 81: 74, 3...
-9             10         1       2  Nasser, Mrs. Nicholas (Ade...  female  14.00      1      0             237736   30.0708              NaN        C  [[[88, 97], [88, 97], [88,...                       {69: 43}
-
-
-df.shortloc_str('Pclass', r'3').to_string(max_colwidth=30)
-     PassengerId  Survived  Pclass                           Name     Sex    Age  SibSp  Parch              Ticket     Fare  Cabin Embarked                       listtest                       dicttest
-0              1         0       3        Braund, Mr. Owen Harris    male  22.00      1      0           A/5 21171   7.2500    NaN        S  [[[27, 71], [27, 71], [27,...  {36: 67, 73: 54, 56: 48, 8...
-2              3         1       3         Heikkinen, Miss. Laina  female  26.00      0      0    STON/O2. 3101282   7.9250    NaN        S                   [[[31, 23]]]  {49: 6, 76: 22, 52: 18, 6:...
-4              5         0       3       Allen, Mr. William Henry    male  35.00      0      0              373450   8.0500    NaN        S  [[[60, 84], [60, 84], [60,...  {8: 61, 37: 4, 25: 43, 21:...
-5              6         0       3               Moran, Mr. James    male    NaN      0      0              330877   8.4583    NaN        Q         [[[25, 39], [25, 39]]]       {97: 78, 85: 88, 42: 34}
-7              8         0       3  Palsson, Master. Gosta Leo...    male   2.00      3      1              349909  21.0750    NaN        S  [[[42, 52], [42, 52], [42,...               {71: 69, 44: 14}
-8              9         1       3  Johnson, Mrs. Oscar W (Eli...  female  27.00      0      2              347742  11.1333    NaN        S  [[[92, 21], [92, 21], [92,...  {61: 17, 72: 44, 81: 74, 3...
-10            11         1       3  Sandstrom, Miss. Marguerit...  female   4.00      1      1             PP 9549  16.7000     G6        S  [[[28, 63], [28, 63], [28,...  {12: 80, 63: 96, 79: 99, 5...
-12            13         0       3  Saundercock, Mr. William H...    male  20.00      0      0           A/5. 2151   8.0500    NaN        S  [[[34, 91], [34, 91], [34,...  {42: 68, 46: 90, 66: 96, 3...
-13            14         0       3    Andersson, Mr. Anders Johan    male  39.00      1      5              347082  31.2750    NaN        S  [[[3, 47], [3, 47], [3, 47...  {94: 60, 73: 33, 59: 32, 3...
-14            15         0       3  Vestrom, Miss. Hulda Amand...  female  14.00      0      0              350406   7.8542    NaN        S  [[[40, 57], [40, 57], [40,...  {54: 39, 8: 35, 76: 84, 20...
-16            17         0       3           Rice, Master. Eugene    male   2.00      4      1              382652  29.1250    NaN        Q  [[[24, 8], [24, 8], [24, 8...  {20: 91, 56: 55, 11: 16, 3...
-
-
-
-df.shortloc_str_replace('Pclass', r'3',4).to_string(max_colwidth=30)
-     PassengerId  Survived  Pclass                           Name     Sex    Age  SibSp  Parch              Ticket      Fare            Cabin Embarked                       listtest                       dicttest
-0              1         0       4        Braund, Mr. Owen Harris    male  22.00      1      0           A/5 21171    7.2500              NaN        S  [[[27, 71], [27, 71], [27,...  {36: 67, 73: 54, 56: 48, 8...
-1              2         1       1  Cumings, Mrs. John Bradley...  female  38.00      1      0            PC 17599   71.2833              C85        C  [[[31, 68], [31, 68], [31,...                        {9: 77}
-2              3         1       4         Heikkinen, Miss. Laina  female  26.00      0      0    STON/O2. 3101282    7.9250              NaN        S                   [[[31, 23]]]  {49: 6, 76: 22, 52: 18, 6:...
-3              4         1       1  Futrelle, Mrs. Jacques Hea...  female  35.00      1      0              113803   53.1000             C123        S  [[[96, 48], [96, 48], [96,...  {27: 90, 9: 38, 18: 94, 67...
-4              5         0       4       Allen, Mr. William Henry    male  35.00      0      0              373450    8.0500              NaN        S  [[[60, 84], [60, 84], [60,...  {8: 61, 37: 4, 25: 43, 21:...
-5              6         0       4               Moran, Mr. James    male    NaN      0      0              330877    8.4583              NaN        Q         [[[25, 39], [25, 39]]]       {97: 78, 85: 88, 42: 34}
-6              7         0       1        McCarthy, Mr. Timothy J    male  54.00      0      0               17463   51.8625              E46        S  [[[76, 5], [76, 5], [76, 5...  {56: 51, 13: 24, 84: 24, 9...
-7              8         0       4  Palsson, Master. Gosta Leo...    male   2.00      3      1              349909   21.0750              NaN        S  [[[42, 52], [42, 52], [42,...               {71: 69, 44: 14}
-8              9         1       4  Johnson, Mrs. Oscar W (Eli...  female  27.00      0      2              347742   11.1333              NaN        S  [[[92, 21], [92, 21], [92,...  {61: 17, 72: 44, 81: 74, 3...
-9             10         1       2  Nasser, Mrs. Nicholas (Ade...  female  14.00      1      0              237736   30.0708              NaN        C  [[[88, 97], [88, 97], [88,...                       {69: 43}
-10            11         1       4  Sandstrom, Miss. Marguerit...  female   4.00      1      1             PP 9549   16.7000               G6        S  [[[28, 63], [28, 63], [28,...  {12: 80, 63: 96, 79: 99, 5...
-
-
-
-
-df.loc_positive_and(
-   ("Pclass", "==", 3),
-   ("Sex", "!=", "male"),
-   ("Age", ">=", 1),
-   ("Pclass", ">=", 3),
-   ("listtest", "in_iter", [11, 22, 33, 44, 55, 66, 77, 88, 99]),
-   ("Sex", "in", ["female", "male"]),
-   ("Name", "re", r"Miss\."),
-   ("Ticket", ">", 5000),
-   ("Embarked", "str", "S"),
-)
-
-     PassengerId  Survived  Pclass                           Name     Sex   Age  SibSp  Parch  Ticket     Fare Cabin Embarked                       listtest                       dicttest
-24            25         0       3  Palsson, Miss. Torborg Danira  female   8.0      3      1  349909  21.0750   NaN        S  [[[44, 33], [44, 33], [44,...  {98: 85, 8: 23, 21: 77, 85...
-141          142         1       3       Nysten, Miss. Anna Sofia  female  22.0      0      0  347081   7.7500   NaN        S                   [[[44, 30]]]  {25: 15, 24: 14, 16: 26, 5...
-192          193         1       3  Andersen-Jensen, Miss. Car...  female  19.0      1      0  350046   7.8542   NaN        S  [[[39, 55], [39, 55], [39,...  {1: 44, 16: 59, 80: 13, 81...
-634          635         0       3             Skoog, Miss. Mabel  female   9.0      3      2  347088  27.9000   NaN        S                   [[[11, 22]]]                        {40: 7}
-
-
-
-df.loc_positive_and(('Ticket','==', 373450), ('Pclass','==', 3))
-   PassengerId  Survived  Pclass                      Name   Sex   Age  SibSp  Parch  Ticket  Fare Cabin Embarked                       listtest                       dicttest
-4            5         0       3  Allen, Mr. William Henry  male  35.0      0      0  373450  8.05   NaN        S  [[[60, 84], [60, 84], [60,...  {8: 61, 37: 4, 25: 43, 21:...
-
-
-df.loc_positive_or(('Ticket','==', 373450), ('Pclass','==', 3))
-     PassengerId  Survived  Pclass                           Name     Sex    Age  SibSp  Parch              Ticket     Fare  Cabin Embarked                       listtest                       dicttest
-0              1         0       3        Braund, Mr. Owen Harris    male  22.00      1      0           A/5 21171   7.2500    NaN        S  [[[27, 71], [27, 71], [27,...  {36: 67, 73: 54, 56: 48, 8...
-2              3         1       3         Heikkinen, Miss. Laina  female  26.00      0      0    STON/O2. 3101282   7.9250    NaN        S                   [[[31, 23]]]  {49: 6, 76: 22, 52: 18, 6:...
-4              5         0       3       Allen, Mr. William Henry    male  35.00      0      0              373450   8.0500    NaN        S  [[[60, 84], [60, 84], [60,...  {8: 61, 37: 4, 25: 43, 21:...
-5              6         0       3               Moran, Mr. James    male    NaN      0      0              330877   8.4583    NaN        Q         [[[25, 39], [25, 39]]]       {97: 78, 85: 88, 42: 34}
-7              8         0       3  Palsson, Master. Gosta Leo...    male   2.00      3      1              349909  21.0750    NaN        S  [[[42, 52], [42, 52], [42,...               {71: 69, 44: 14}
-
-
-
-df.loc_positive_and(('Age','>=', 13), ('Age','<=', 19))
-     PassengerId  Survived  Pclass                           Name     Sex   Age  SibSp  Parch             Ticket      Fare            Cabin Embarked                       listtest                       dicttest
-9             10         1       2  Nasser, Mrs. Nicholas (Ade...  female  14.0      1      0             237736   30.0708              NaN        C  [[[88, 97], [88, 97], [88,...                       {69: 43}
-14            15         0       3  Vestrom, Miss. Hulda Amand...  female  14.0      0      0             350406    7.8542              NaN        S  [[[40, 57], [40, 57], [40,...  {54: 39, 8: 35, 76: 84, 20...
-22            23         1       3    McGowan, Miss. Anna "Annie"  female  15.0      0      0             330923    8.0292              NaN        Q  [[[85, 85], [85, 85], [85,...  {80: 2, 70: 5, 27: 24, 10:...
-27            28         0       1  Fortune, Mr. Charles Alexa...    male  19.0      3      2              19950  263.0000      C23 C25 C27        S  [[[7, 96], [7, 96], [7, 96...  {60: 4, 22: 96, 55: 28, 97...
-38            39         0       3  Vander Planke, Miss. Augus...  female  18.0      2      0             345764   18.0000              NaN        S  [[[82, 50], [82, 50], [82,...  {70: 41, 90: 86, 46: 95, 3...
-39            40         1       3    Nicola-Yarred, Miss. Jamila  female  14.0      1      0               2651   11.2417              NaN        C  [[[20, 72], [20, 72], [20,...  {72: 91, 81: 15, 89: 24, 9...
-44            45         1       3  Devaney, Miss. Margaret Delia  female  19.0      0      0             330958    7.8792              NaN        Q  [[[97, 1], [97, 1], [97, 1...  {89: 44, 58: 86, 48: 54, 9...
-49            50         0       3  Arnold-Franchi, Mrs. Josef...  female  18.0      1      0             349237   17.8000              NaN        S         [[[64, 68], [64, 68]]]  {67: 59, 96: 34, 8: 64, 45...
-67            68         0       3       Crease, Mr. Ernest James    male  19.0      0      0          S.P. 3464    8.1583              NaN        S  [[[30, 77], [30, 77], [30,...  {37: 56, 52: 5, 80: 12, 86...
-
-
-
-df.loc_positive_and(('Ticket','!=', 373450), ('Pclass','!=', 3))
-     PassengerId  Survived  Pclass                           Name     Sex    Age  SibSp  Parch            Ticket      Fare            Cabin Embarked                       listtest                       dicttest
-1              2         1       1  Cumings, Mrs. John Bradley...  female  38.00      1      0          PC 17599   71.2833              C85        C  [[[31, 68], [31, 68], [31,...                        {9: 77}
-3              4         1       1  Futrelle, Mrs. Jacques Hea...  female  35.00      1      0            113803   53.1000             C123        S  [[[96, 48], [96, 48], [96,...  {27: 90, 9: 38, 18: 94, 67...
-6              7         0       1        McCarthy, Mr. Timothy J    male  54.00      0      0             17463   51.8625              E46        S  [[[76, 5], [76, 5], [76, 5...  {56: 51, 13: 24, 84: 24, 9...
-9             10         1       2  Nasser, Mrs. Nicholas (Ade...  female  14.00      1      0            237736   30.0708              NaN        C  [[[88, 97], [88, 97], [88,...                       {69: 43}
-11            12         1       1       Bonnell, Miss. Elizabeth  female  58.00      0      0            113783   26.5500             C103        S         [[[66, 84], [66, 84]]]  {87: 7, 75: 62, 84: 22, 94...
-15            16         1       2  Hewlett, Mrs. (Mary D King...  female  55.00      0      0            248706   16.0000              NaN        S  [[[93, 7], [93, 7], [93, 7...  {17: 96, 7: 68, 74: 5, 97:...
-
-
-df.loc_negative_and(('Age','>=', 13), ('Sex','str', 'female'))
-     PassengerId  Survived  Pclass                           Name   Sex    Age  SibSp  Parch           Ticket      Fare    Cabin Embarked                       listtest                       dicttest
-386          387         0       3  Goodwin, Master. Sidney Le...  male   1.00      5      2          CA 2144   46.9000      NaN        S  [[[32, 26], [32, 26], [32,...  {42: 33, 97: 56, 33: 73, 7...
-261          262         1       3  Asplund, Master. Edvin Roj...  male   3.00      4      2           347077   31.3875      NaN        S  [[[40, 73], [40, 73], [40,...  {7: 23, 93: 3, 18: 66, 96:...
-7              8         0       3  Palsson, Master. Gosta Leo...  male   2.00      3      1           349909   21.0750      NaN        S  [[[42, 52], [42, 52], [42,...               {71: 69, 44: 14}
-16            17         0       3           Rice, Master. Eugene  male   2.00      4      1           382652   29.1250      NaN        Q  [[[24, 8], [24, 8], [24, 8...  {20: 91, 56: 55, 11: 16, 3...
-787          788         0       3      Rice, Master. George Hugh  male   8.00      4      1           382652   29.1250      NaN        Q  [[[32, 90], [32, 90], [32,...  {5: 17, 83: 1, 82: 16, 21:...
-788          789         1       3     Dean, Master. Bertram Vere  male   1.00      1      2        C.A. 2315   20.5750      NaN        S  [[[27, 72], [27, 72], [27,...       {58: 65, 42: 92, 61: 72}
-278          279         0       3             Rice, Master. Eric  male   7.00      4      1           382652   29.1250      NaN        Q  [[[48, 59], [48, 59], [48,...  {16: 64, 97: 83, 66: 91, 9...
-
-
-
-df.shortloc_regex('Name', '^Ab').shortloc_not_equal('Sex', 'male').shortloc_equal('Age', 35)
-     PassengerId  Survived  Pclass                           Name     Sex   Age  SibSp  Parch     Ticket   Fare Cabin Embarked                       listtest                       dicttest
-279          280         1       3  Abbott, Mrs. Stanton (Rosa...  female  35.0      1      1  C.A. 2673  20.25   NaN        S  [[[93, 85], [93, 85], [93,...  {37: 16, 68: 58, 42: 7, 20...
-
-
-
-df.shortloc_in_iter('dicttest', 65).shortloc_not_in_iter('listtest', [77,65,80,83])
-     PassengerId  Survived  Pclass                           Name     Sex   Age  SibSp  Parch       Ticket      Fare        Cabin Embarked                       listtest                       dicttest
-515          516         0       1   Walker, Mr. William Anderson    male  47.0      0      0        36967   34.0208          D46        S  [[[55, 13], [55, 13], [55,...  {67: 25, 73: 76, 93: 74, 6...
-772          773         0       2              Mack, Mrs. (Mary)  female  57.0      0      0  S.O./P.P. 3   10.5000          E77        S  [[[3, 67], [3, 67], [3, 67...  {20: 62, 88: 78, 22: 65, 1...
-518          519         1       2  Angle, Mrs. William A (Flo...  female  36.0      1      0       226875   26.0000          NaN        S         [[[78, 94], [78, 94]]]  {32: 53, 48: 66, 20: 5, 67...
-10            11         1       3  Sandstrom, Miss. Marguerit...  female   4.0      1      1      PP 9549   16.7000           G6        S  [[[28, 63], [28, 63], [28,...  {12: 80, 63: 96, 79: 99, 5...
-275          276         1       1  Andrews, Miss. Kornelia Th...  female  63.0      1      0        13502   77.9583           D7        S                   [[[84, 21]]]  {31: 95, 27: 48, 89: 25, 6...
-788          789         1       3     Dean, Master. Bertram Vere    male   1.0      1      2    C.A. 2315   20.5750          NaN        S  [[[27, 72], [27, 72], [27,...       {58: 65, 42: 92, 61: 72}
-
-
-
-df.shortloc_not_isna("Cabin").shortloc_str("Cabin", "C").shortloc_not_regex(
-   "Cabin", "^.{4,}$"
-)
-     PassengerId  Survived  Pclass                           Name     Sex   Age  SibSp  Parch    Ticket      Fare Cabin Embarked                       listtest                       dicttest
-1              2         1       1  Cumings, Mrs. John Bradley...  female  38.0      1      0  PC 17599   71.2833   C85        C  [[[31, 68], [31, 68], [31,...                        {9: 77}
-269          270         1       1         Bissette, Miss. Amelia  female  35.0      0      0  PC 17760  135.6333   C99        S  [[[89, 54], [89, 54], [89,...  {50: 9, 91: 60, 30: 67, 46...
-527          528         0       1             Farthing, Mr. John    male   NaN      0      0  PC 17483  221.7792   C95        S  [[[9, 72], [9, 72], [9, 72...               {41: 24, 63: 10}
-151          152         1       1  Pears, Mrs. Thomas (Edith ...  female  22.0      1      0    113776   66.6000    C2        S  [[[24, 98], [24, 98], [24,...  {80: 92, 25: 89, 32: 82, 1...
-412          413         1       1         Minahan, Miss. Daisy E  female  33.0      1      0     19928   90.0000   C78        Q                    [[[2, 41]]]                       {57: 41}
-544          545         0       1     Douglas, Mr. Walter Donald    male  50.0      1      0  PC 17761  106.4250   C86        C  [[[55, 21], [55, 21], [55,...               {51: 49, 16: 20}
-550          551         1       1    Thayer, Mr. John Borland Jr    male  17.0      0      2     17421  110.8833   C70        C  [[[37, 20], [37, 20], [37,...               {17: 85, 49: 77}
-430          431         1       1  Bjornstrom-Steffansson, Mr...    male  28.0      0      0    110564   26.5500   C52        S  [[[14, 61], [14, 61], [14,...                       {62: 40}
-
-
-df.shortloc_in_iter('listtest',[99, 77]).shortloc_regex('listtest',r"7\b,\s*\b9"))
-     PassengerId  Survived  Pclass                  Name     Sex   Age  SibSp  Parch Ticket     Fare Cabin Embarked                       listtest                       dicttest
-111          112         0       3  Zabour, Miss. Hileni  female  14.5      1      0   2665  14.4542   NaN        C  [[[27, 99], [27, 99], [27,...  {76: 81, 62: 60, 98: 43, 5...
-
-
-#all methods can also be used against Series
-#Two examples
-
-df.Pclass.shortloc_regex('^2$')
-Out[54]: 
-9      2
-15     2
-17     2
-20     2
-21     2
-      ..
-
-df.Pclass.shortloc_regex_replace('^3$',2000)
-Out[56]: 
-0      2000
-1         1
-2      2000
-3         1
-4      2000
-       ... 
+Search and replace values with df.loc without Exceptions due to dtype incompatibility.  If the dtypes of 2 variables don't match, they will be converted until they match. 
+
+```python
+pip install a_pandas_ex_easy_loc
+```
+
+Some examples
+
+```python
+import pandas as pd
+df = pd.read_csv("https://github.com/pandas-dev/pandas/raw/main/doc/data/titanic.csv")
+# df.loc[df.Ticket >20000]
+from random import randrange
+getrandomlist = lambda x: [
+  [[randrange(1, 100), randrange(1, 100)] * 1] * randrange(1, 10)
+]
+df["listtest"] = df.PassengerId.map(getrandomlist)
+
+
+getrandomdict = lambda x: {
+  randrange(1, 100):randrange(1, 100) for _ in range(randrange(1, 10))
+}
+df["dicttest"] = df.PassengerId.map(getrandomdict)
+from a_easy_loc import pd_add_easy_loc
+pd_add_easy_loc()
+df.shortloc_greater_replace('Pclass', 2,3000)
+
+df.shortloc_equal('Pclass', 3)
+     PassengerId  Survived  Pclass       Name     Sex    Age  SibSp  Parch     Ticket     Fare  Cabin Embarked   listtest   dicttest
+0            1           0       3  Braund...    male  22.00      1      0  A/5 21171   7.2500    NaN        S  [[[44,...  {5: 8,...
+2            3           1       3  Heikki...  female  26.00      0      0  STON/O...   7.9250    NaN        S  [[[60,...  {33: 3...
+4            5           0       3  Allen,...    male  35.00      0      0     373450   8.0500    NaN        S  [[[99,...  {96: 1...
+5            6           0       3  Moran,...    male    NaN      0      0     330877   8.4583    NaN        Q  [[[82,...  {23: 1...
+7            8           0       3  Palsso...    male   2.00      3      1     349909  21.0750    NaN        S  [[[14,...  {20: 8...
+8            9           1       3  Johnso...  female  27.00      0      2     347742  11.1333    NaN        S  [[[12,...  {96: 5...
+
+
+df.shortloc_equal('Ticket', 373450)
+   PassengerId  Survived  Pclass       Name   Sex   Age  SibSp  Parch  Ticket  Fare Cabin Embarked   listtest   dicttest
+4          5           0       3  Allen,...  male  35.0      0      0  373450  8.05   NaN        S  [[[99,...  {96: 1...
+
+
+df.shortloc_greater('Pclass', 2)
+     PassengerId  Survived  Pclass       Name     Sex    Age  SibSp  Parch     Ticket     Fare  Cabin Embarked   listtest   dicttest
+0            1           0       3  Braund...    male  22.00      1      0  A/5 21171   7.2500    NaN        S  [[[44,...  {5: 8,...
+2            3           1       3  Heikki...  female  26.00      0      0  STON/O...   7.9250    NaN        S  [[[60,...  {33: 3...
+4            5           0       3  Allen,...    male  35.00      0      0     373450   8.0500    NaN        S  [[[99,...  {96: 1...
+5            6           0       3  Moran,...    male    NaN      0      0     330877   8.4583    NaN        Q  [[[82,...  {23: 1...
+
+df.shortloc_greater('Ticket', 373450)
+     PassengerId  Survived  Pclass       Name     Sex   Age  SibSp  Parch   Ticket     Fare Cabin Embarked   listtest   dicttest
+16          17           0       3  Rice, ...    male   2.0      4      1   382652  29.1250   NaN        Q  [[[17,...  {46: 7...
+50          51           0       3  Panula...    male   7.0      4      1  3101295  39.6875   NaN        S  [[[30,...  {64: 2...
+68          69           1       3  Anders...  female  17.0      4      2  3101281   7.9250   NaN        S  [[[4, ...  {92: 3...
+77          78           0       3  Moutal...    male   NaN      0      0   374746   8.0500   NaN        S  [[[65,...  {47: 9...
+85          86           1       3  Backst...  female  33.0      3      0  3101278  15.8500   NaN        S  [[[55,...  {5: 22...
+
+
+df.shortloc_greater_or_equal('Age', 43)
+     PassengerId  Survived  Pclass       Name     Sex   Age  SibSp  Parch     Ticket      Fare      Cabin Embarked   listtest   dicttest
+6            7           0       1  McCart...    male  54.0      0      0      17463   51.8625        E46        S  [[[47,...   {22: 17}
+11          12           1       1  Bonnel...  female  58.0      0      0     113783   26.5500       C103        S  [[[1, ...    {35: 9}
+15          16           1       2  Hewlet...  female  55.0      0      0     248706   16.0000        NaN        S  [[[43,...  {40: 6...
+33          34           0       2  Wheado...    male  66.0      0      0  C.A. 2...   10.5000        NaN        S  [[[6, ...   {50: 28}
+52          53           1       1  Harper...  female  49.0      1      0   PC 17572   76.7292        D33        C  [[[41,...  {54: 6...
+
+
+df.shortloc_greater_replace('Pclass', 2,3000)
+     PassengerId  Survived  Pclass       Name     Sex    Age  SibSp  Parch     Ticket      Fare      Cabin Embarked   listtest   dicttest
+0            1           0    3000  Braund...    male  22.00      1      0  A/5 21171    7.2500        NaN        S  [[[65,...  {76: 3...
+1            2           1       1  Cuming...  female  38.00      1      0   PC 17599   71.2833        C85        C  [[[1, ...  {55: 3...
+2            3           1    3000  Heikki...  female  26.00      0      0  STON/O...    7.9250        NaN        S  [[[56,...  {7: 54...
+3            4           1       1  Futrel...  female  35.00      1      0     113803   53.1000       C123        S  [[[91,...   {51: 89}
+4            5           0    3000  Allen,...    male  35.00      0      0     373450    8.0500        NaN        S  [[[20,...  {39: 5...
+5            6           0    3000  Moran,...    male    NaN      0      0     330877    8.4583        NaN        Q  [[[60,...  {63: 2...
+6            7           0       1  McCart...    male  54.00      0      0      17463   51.8625        E46        S  [[[51,...  {1: 90...
+
+
+
+df.shortloc_greater_replace('Ticket', 5000, 888000)
+     PassengerId  Survived  Pclass       Name     Sex    Age  SibSp  Parch     Ticket      Fare      Cabin Embarked   listtest   dicttest
+0            1           0       3  Braund...    male  22.00      1      0  A/5 21171    7.2500        NaN        S  [[[74,...  {40: 3...
+1            2           1       1  Cuming...  female  38.00      1      0   PC 17599   71.2833        C85        C  [[[67,...     {1: 8}
+2            3           1       3  Heikki...  female  26.00      0      0  STON/O...    7.9250        NaN        S  [[[62,...   {39: 79}
+3            4           1       1  Futrel...  female  35.00      1      0     888000   53.1000       C123        S  [[[15,...  {13: 2...
+4            5           0       3  Allen,...    male  35.00      0      0     888000    8.0500        NaN        S  [[[81,...   {60: 90}
+5            6           0       3  Moran,...    male    NaN      0      0     888000    8.4583        NaN        Q  [[[58,...    {20: 4}
+6            7           0       1  McCart...    male  54.00      0      0     888000   51.8625        E46        S  [[[28,...  {21: 8...
+7            8           0       3  Palsso...    male   2.00      3      1     888000   21.0750        NaN        S  [[[25,...  {53: 8...
+8            9           1       3  Johnso...  female  27.00      0      2     888000   11.1333        NaN        S  [[[47,...  {19: 3...
+
+
+df.shortloc_greater_replace('Cabin','C123', pd.NA)
+     PassengerId  Survived  Pclass       Name     Sex    Age  SibSp  Parch     Ticket      Fare      Cabin Embarked   listtest   dicttest
+0            1           0       3  Braund...    male  22.00      1      0  A/5 21171    7.2500        NaN        S  [[[74,...  {40: 3...
+1            2           1       1  Cuming...  female  38.00      1      0   PC 17599   71.2833       <NA>        C  [[[67,...     {1: 8}
+2            3           1       3  Heikki...  female  26.00      0      0  STON/O...    7.9250        NaN        S  [[[62,...   {39: 79}
+3            4           1       1  Futrel...  female  35.00      1      0     113803   53.1000       C123        S  [[[15,...  {13: 2...
+4            5           0       3  Allen,...    male  35.00      0      0     373450    8.0500        NaN        S  [[[81,...   {60: 90}
+5            6           0       3  Moran,...    male    NaN      0      0     330877    8.4583        NaN        Q  [[[58,...    {20: 4}
+6            7           0       1  McCart...    male  54.00      0      0      17463   51.8625       <NA>        S  [[[28,...  {21: 8...
+7            8           0       3  Palsso...    male   2.00      3      1     349909   21.0750        NaN        S  [[[25,...  {53: 8...
+
+df.shortloc_in_iter('listtest', 3)
+     PassengerId  Survived  Pclass                 Name     Sex   Age  SibSp  Parch        Ticket     Fare Cabin Embarked             listtest             dicttest
+19            20         1       3  Masselmani, Mrs....  female   NaN      0      0          2649   7.2250   NaN        C  [[[32, 3], [32, ...  {98: 75, 69: 39,...
+66            67         1       2  Nye, Mrs. (Eliza...  female  29.0      0      0    C.A. 29395  10.5000   F33        S  [[[3, 98], [3, 9...             {60: 81}
+92            93         0       1  Chaffee, Mr. Her...    male  46.0      1      0   W.E.P. 5734  61.1750   E31        S  [[[52, 3], [52, ...             {80: 25}
+106          107         1       3  Salkjelsvik, Mis...  female  21.0      0      0        343120   7.6500   NaN        S  [[[85, 3], [85, ...             {62: 49}
+120          121         0       2  Hickman, Mr. Sta...    male  21.0      2      0  S.O.C. 14879  73.5000   NaN        S  [[[40, 3], [40, ...  {28: 85, 60: 72,...
+129          130         0       3   Ekstrom, Mr. Johan    male  45.0      0      0        347061   6.9750   NaN        S  [[[3, 76], [3, 7...  {79: 2, 30: 18, ...
+132          133         0       3  Robins, Mrs. Ale...  female  47.0      1      0     A/5. 3337  14.5000   NaN        S  [[[3, 68], [3, 6...  {69: 90, 1: 23, ...
+184          185         1       3  Kink-Heilmann, M...  female   4.0      0      2        315153  22.0250   NaN        S  [[[3, 88], [3, 8...  {24: 74, 30: 11,...
+
+df.shortloc_in_iter('listtest', [3,4,10])
+     PassengerId  Survived  Pclass                 Name     Sex    Age  SibSp  Parch           Ticket      Fare        Cabin Embarked             listtest             dicttest
+19            20         1       3  Masselmani, Mrs....  female    NaN      0      0             2649    7.2250          NaN        C  [[[32, 3], [32, ...  {98: 75, 69: 39,...
+22            23         1       3  McGowan, Miss. A...  female  15.00      0      0           330923    8.0292          NaN        Q  [[[13, 4], [13, ...  {56: 86, 30: 5, ...
+27            28         0       1  Fortune, Mr. Cha...    male  19.00      3      2            19950  263.0000  C23 C25 C27        S  [[[4, 66], [4, 6...  {58: 98, 32: 55,...
+66            67         1       2  Nye, Mrs. (Eliza...  female  29.00      0      0       C.A. 29395   10.5000          F33        S  [[[3, 98], [3, 9...             {60: 81}
+74            75         1       3        Bing, Mr. Lee    male  32.00      0      0             1601   56.4958          NaN        S  [[[14, 4], [14, ...  {31: 31, 64: 38,...
+84            85         1       2  Ilett, Miss. Bertha  female  17.00      0      0       SO/C 14885   10.5000          NaN        S  [[[18, 10], [18,...  {81: 64, 10: 80,...
+
+
+df.shortloc_in_iter('dicttest', [3,4,10])
+     PassengerId  Survived  Pclass                           Name     Sex    Age  SibSp  Parch             Ticket      Fare            Cabin Embarked                       listtest                       dicttest
+5              6         0       3               Moran, Mr. James    male    NaN      0      0             330877    8.4583              NaN        Q         [[[58, 72], [58, 72]]]                        {20: 4}
+8              9         1       3  Johnson, Mrs. Oscar W (Eli...  female  27.00      0      2             347742   11.1333              NaN        S         [[[47, 12], [47, 12]]]         {19: 3, 60: 24, 9: 38}
+
+
+df.shortloc_in_iter('dicttest', [3,4,10])
+     PassengerId  Survived  Pclass                          Name     Sex   Age  SibSp  Parch         Ticket     Fare Cabin Embarked                                                           listtest                                                               dicttest
+96            97         0       1     Goldschmidt, Mr. George B    male  71.0      0      0       PC 17754  34.6542    A5        C           [[[94, 4], [94, 4], [94, 4], [94, 4], [94, 4], [94, 4]]]       {67: 92, 24: 19, 53: 40, 66: 53, 44: 81, 94: 10, 34: 63, 61: 45}
+103          104         0       3    Johansson, Mr. Gustaf Joel    male  33.0      0      0           7540   8.6542   NaN        S               [[[89, 10], [89, 10], [89, 10], [89, 10], [89, 10]]]                                        {92: 23, 32: 17, 53: 3, 98: 94}
+129          130         0       3            Ekstrom, Mr. Johan    male  45.0      0      0         347061   6.9750   NaN        S  [[[3, 76], [3, 76], [3, 76], [3, 76], [3, 76], [3, 76], [3, 76]]]   {79: 2, 30: 18, 63: 10, 62: 26, 91: 58, 11: 44, 8: 81, 6: 93, 97: 5}
+
+
+df.shortloc_in_iter_replace('dicttest', [3,4,10], 15151515)
+     PassengerId  Survived  Pclass                           Name     Sex    Age  SibSp  Parch              Ticket      Fare            Cabin Embarked                       listtest                       dicttest
+0              1         0       3        Braund, Mr. Owen Harris    male  22.00      1      0           A/5 21171    7.2500              NaN        S  [[[74, 68], [74, 68], [74,...  {40: 30, 93: 84, 24: 92, 7...
+1              2         1       1  Cumings, Mrs. John Bradley...  female  38.00      1      0            PC 17599   71.2833              C85        C  [[[67, 64], [67, 64], [67,...                         {1: 8}
+2              3         1       3         Heikkinen, Miss. Laina  female  26.00      0      0    STON/O2. 3101282    7.9250              NaN        S  [[[62, 65], [62, 65], [62,...                       {39: 79}
+3              4         1       1  Futrelle, Mrs. Jacques Hea...  female  35.00      1      0              113803   53.1000             C123        S  [[[15, 96], [15, 96], [15,...       {13: 29, 65: 59, 99: 31}
+4              5         0       3       Allen, Mr. William Henry    male  35.00      0      0              373450    8.0500              NaN        S                   [[[81, 13]]]                       {60: 90}
+5              6         0       3               Moran, Mr. James    male    NaN      0      0              330877    8.4583              NaN        Q         [[[58, 72], [58, 72]]]                       15151515
+6              7         0       1        McCarthy, Mr. Timothy J    male  54.00      0      0               17463   51.8625              E46        S  [[[28, 98], [28, 98], [28,...  {21: 8, 31: 42, 9: 40, 93:...
+7              8         0       3  Palsson, Master. Gosta Leo...    male   2.00      3      1              349909   21.0750              NaN        S  [[[25, 88], [25, 88], [25,...  {53: 83, 49: 66, 57: 95, 4...
+8              9         1       3  Johnson, Mrs. Oscar W (Eli...  female  27.00      0      2              347742   11.1333              NaN        S         [[[47, 12], [47, 12]]]                       15151515
+
+df.shortloc_isin('Embarked', ['C', 'S'])
+     PassengerId  Survived  Pclass                           Name     Sex    Age  SibSp  Parch              Ticket      Fare            Cabin Embarked                       listtest                       dicttest
+0              1         0       3        Braund, Mr. Owen Harris    male  22.00      1      0           A/5 21171    7.2500              NaN        S  [[[74, 68], [74, 68], [74,...  {40: 30, 93: 84, 24: 92, 7...
+1              2         1       1  Cumings, Mrs. John Bradley...  female  38.00      1      0            PC 17599   71.2833              C85        C  [[[67, 64], [67, 64], [67,...                         {1: 8}
+2              3         1       3         Heikkinen, Miss. Laina  female  26.00      0      0    STON/O2. 3101282    7.9250              NaN        S  [[[62, 65], [62, 65], [62,...                       {39: 79}
+3              4         1       1  Futrelle, Mrs. Jacques Hea...  female  35.00      1      0              113803   53.1000             C123        S  [[[15, 96], [15, 96], [15,...       {13: 29, 65: 59, 99: 31}
+4              5         0       3       Allen, Mr. William Henry    male  35.00      0      0              373450    8.0500              NaN        S                   [[[81, 13]]]                       {60: 90}
+6              7         0       1        McCarthy, Mr. Timothy J    male  54.00      0      0               17463   51.8625              E46        S  [[[28, 98], [28, 98], [28,...  {21: 8, 31: 42, 9: 40, 93:...
+7              8         0       3  Palsson, Master. Gosta Leo...    male   2.00      3      1              349909   21.0750              NaN        S  [[[25, 88], [25, 88], [25,...  {53: 83, 49: 66, 57: 95, 4...
+8              9         1       3  Johnson, Mrs. Oscar W (Eli...  female  27.00      0      2              347742   11.1333              NaN        S         [[[47, 12], [47, 12]]]         {19: 3, 60: 24, 9: 38}
+
+df.shortloc_isin_replace('Embarked', ['C', 'S'], 'CCCCCCCCCCCCCCCCCCCSSSSSSSSSSSSSSSSSSSSSSSSSSSSS')
+     PassengerId  Survived  Pclass       Name     Sex    Age  SibSp  Parch     Ticket      Fare      Cabin   Embarked   listtest   dicttest
+0            1           0       3  Braund...    male  22.00      1      0  A/5 21171    7.2500        NaN  CCCCCC...  [[[74,...  {40: 3...
+1            2           1       1  Cuming...  female  38.00      1      0   PC 17599   71.2833        C85  CCCCCC...  [[[67,...     {1: 8}
+2            3           1       3  Heikki...  female  26.00      0      0  STON/O...    7.9250        NaN  CCCCCC...  [[[62,...   {39: 79}
+3            4           1       1  Futrel...  female  35.00      1      0     113803   53.1000       C123  CCCCCC...  [[[15,...  {13: 2...
+4            5           0       3  Allen,...    male  35.00      0      0     373450    8.0500        NaN  CCCCCC...  [[[81,...   {60: 90}
+5            6           0       3  Moran,...    male    NaN      0      0     330877    8.4583        NaN          Q  [[[58,...    {20: 4}
+
+
+df.shortloc_isna('Age')
+     PassengerId  Survived  Pclass                           Name     Sex  Age  SibSp  Parch              Ticket      Fare  Cabin Embarked                       listtest                       dicttest
+5              6         0       3               Moran, Mr. James    male  NaN      0      0              330877    8.4583    NaN        Q         [[[25, 39], [25, 39]]]       {97: 78, 85: 88, 42: 34}
+17            18         1       2   Williams, Mr. Charles Eugene    male  NaN      0      0              244373   13.0000    NaN        S  [[[17, 6], [17, 6], [17, 6...                 {41: 6, 2: 82}
+19            20         1       3        Masselmani, Mrs. Fatima  female  NaN      0      0                2649    7.2250    NaN        C  [[[11, 37], [11, 37], [11,...  {43: 73, 50: 28, 38: 47, 4...
+26            27         0       3        Emir, Mr. Farred Chehab    male  NaN      0      0                2631    7.2250    NaN        C  [[[48, 66], [48, 66], [48,...               {33: 45, 82: 90}
+28            29         1       3  O'Dwyer, Miss. Ellen "Nellie"  female  NaN      0      0              330959    7.8792    NaN        Q           [[[3, 53], [3, 53]]]               {29: 90, 84: 86}
+29            30         0       3            Todoroff, Mr. Lalio    male  NaN      0      0              349216    7.8958    NaN        S  [[[67, 3], [67, 3], [67, 3...  {57: 49, 23: 71, 64: 45, 1...
+31            32         1       1  Spencer, Mrs. William Augu...  female  NaN      1      0            PC 17569  146.5208    B78        C  [[[88, 94], [88, 94], [88,...  {4: 42, 98: 58, 94: 7, 39:...
+
+
+df.shortloc_isna_replace('Age',16541)
+     PassengerId  Survived  Pclass                           Name     Sex       Age  SibSp  Parch              Ticket      Fare            Cabin Embarked                       listtest                       dicttest
+0              1         0       3        Braund, Mr. Owen Harris    male     22.00      1      0           A/5 21171    7.2500              NaN        S  [[[27, 71], [27, 71], [27,...  {36: 67, 73: 54, 56: 48, 8...
+1              2         1       1  Cumings, Mrs. John Bradley...  female     38.00      1      0            PC 17599   71.2833              C85        C  [[[31, 68], [31, 68], [31,...                        {9: 77}
+2              3         1       3         Heikkinen, Miss. Laina  female     26.00      0      0    STON/O2. 3101282    7.9250              NaN        S                   [[[31, 23]]]  {49: 6, 76: 22, 52: 18, 6:...
+3              4         1       1  Futrelle, Mrs. Jacques Hea...  female     35.00      1      0              113803   53.1000             C123        S  [[[96, 48], [96, 48], [96,...  {27: 90, 9: 38, 18: 94, 67...
+4              5         0       3       Allen, Mr. William Henry    male     35.00      0      0              373450    8.0500              NaN        S  [[[60, 84], [60, 84], [60,...  {8: 61, 37: 4, 25: 43, 21:...
+5              6         0       3               Moran, Mr. James    male  16541.00      0      0              330877    8.4583              NaN        Q         [[[25, 39], [25, 39]]]       {97: 78, 85: 88, 42: 34}
+6              7         0       1        McCarthy, Mr. Timothy J    male     54.00      0      0               17463   51.8625              E46        S  [[[76, 5], [76, 5], [76, 5...  {56: 51, 13: 24, 84: 24, 9...
+
+df.shortloc_less('Ticket', 7534)
+
+     PassengerId  Survived  Pclass                           Name     Sex    Age  SibSp  Parch Ticket     Fare        Cabin Embarked                       listtest                       dicttest
+19            20         1       3        Masselmani, Mrs. Fatima  female    NaN      0      0   2649   7.2250          NaN        C  [[[11, 37], [11, 37], [11,...  {43: 73, 50: 28, 38: 47, 4...
+26            27         0       3        Emir, Mr. Farred Chehab    male    NaN      0      0   2631   7.2250          NaN        C  [[[48, 66], [48, 66], [48,...               {33: 45, 82: 90}
+36            37         1       3               Mamee, Mr. Hanna    male    NaN      0      0   2677   7.2292          NaN        C  [[[84, 24], [84, 24], [84,...  {39: 19, 88: 50, 23: 7, 53...
+39            40         1       3    Nicola-Yarred, Miss. Jamila  female  14.00      1      0   2651  11.2417          NaN        C  [[[20, 72], [20, 72], [20,...  {72: 91, 81: 15, 89: 24, 9...
+48            49         0       3            Samaan, Mr. Youssef    male    NaN      2      0   2662  21.6792          NaN        C  [[[79, 85], [79, 85], [79,...                       {35: 61}
+53            54         1       2  Faunthorpe, Mrs. Lizzie (E...  female  29.00      1      0   2926  26.0000          NaN        S         [[[62, 79], [62, 79]]]  {36: 53, 38: 70, 6: 1, 89:...
+57            58         0       3            Novel, Mr. Mansouer    male  28.50      0      0   2697   7.2292          NaN        C         [[[86, 78], [86, 78]]]                {28: 5, 49: 22}
+60            61         0       3          Sirayanian, Mr. Orsen    male  22.00      0      0   2669   7.2292          NaN        C                   [[[24, 72]]]  {74: 59, 16: 44, 30: 17, 5...
+65            66         1       3       Moubarek, Master. Gerios    male    NaN      1      1   2661  15.2458          NaN        C  [[[56, 96], [56, 96], [56,...  {5: 34, 59: 97, 78: 15, 76...
+73            74         0       3    Chronopoulos, Mr. Apostolos    male  26.00      1      0   2680  14.4542          NaN        C         [[[78, 24], [78, 24]]]  {96: 26, 87: 73, 58: 49, 3...
+74            75         1       3                  Bing, Mr. Lee    male  32.00      0      0   1601  56.4958          NaN        S  [[[86, 20], [86, 20], [86,...  {84: 87, 18: 40, 17: 28, 7...
+
+
+df.shortloc_less_replace('Age', 30, 'less 30')
+     PassengerId  Survived  Pclass                           Name     Sex      Age  SibSp  Parch              Ticket      Fare            Cabin Embarked                       listtest                       dicttest
+0              1         0       3        Braund, Mr. Owen Harris    male  less 30      1      0           A/5 21171    7.2500              NaN        S  [[[27, 71], [27, 71], [27,...  {36: 67, 73: 54, 56: 48, 8...
+1              2         1       1  Cumings, Mrs. John Bradley...  female     38.0      1      0            PC 17599   71.2833              C85        C  [[[31, 68], [31, 68], [31,...                        {9: 77}
+2              3         1       3         Heikkinen, Miss. Laina  female  less 30      0      0    STON/O2. 3101282    7.9250              NaN        S                   [[[31, 23]]]  {49: 6, 76: 22, 52: 18, 6:...
+3              4         1       1  Futrelle, Mrs. Jacques Hea...  female     35.0      1      0              113803   53.1000             C123        S  [[[96, 48], [96, 48], [96,...  {27: 90, 9: 38, 18: 94, 67...
+
+
+df.shortloc_less_or_equal_replace('Survived', 0, 'DEAD')
+     PassengerId Survived  Pclass                           Name     Sex    Age  SibSp  Parch              Ticket      Fare            Cabin Embarked                       listtest                       dicttest
+0              1     DEAD       3        Braund, Mr. Owen Harris    male  22.00      1      0           A/5 21171    7.2500              NaN        S  [[[27, 71], [27, 71], [27,...  {36: 67, 73: 54, 56: 48, 8...
+1              2        1       1  Cumings, Mrs. John Bradley...  female  38.00      1      0            PC 17599   71.2833              C85        C  [[[31, 68], [31, 68], [31,...                        {9: 77}
+2              3        1       3         Heikkinen, Miss. Laina  female  26.00      0      0    STON/O2. 3101282    7.9250              NaN        S                   [[[31, 23]]]  {49: 6, 76: 22, 52: 18, 6:...
+3              4        1       1  Futrelle, Mrs. Jacques Hea...  female  35.00      1      0              113803   53.1000             C123        S  [[[96, 48], [96, 48], [96,...  {27: 90, 9: 38, 18: 94, 67...
+4              5     DEAD       3       Allen, Mr. William Henry    male  35.00      0      0              373450    8.0500              NaN        S  [[[60, 84], [60, 84], [60,...  {8: 61, 37: 4, 25: 43, 21:...
+5              6     DEAD       3               Moran, Mr. James    male    NaN      0      0              330877    8.4583              NaN        Q         [[[25, 39], [25, 39]]]       {97: 78, 85: 88, 42: 34}
+6              7     DEAD       1        McCarthy, Mr. Timothy J    male  54.00      0      0               17463   51.8625              E46        S  [[[76, 5], [76, 5], [76, 5...  {56: 51, 13: 24, 84: 24, 9...
+7              8     DEAD       3  Palsson, Master. Gosta Leo...    male   2.00      3      1              349909   21.0750              NaN        S  [[[42, 52], [42, 52], [42,...               {71: 69, 44: 14}
+
+
+
+df.shortloc_not_equal_replace('Survived', 0, True)
+     PassengerId Survived  Pclass                           Name     Sex    Age  SibSp  Parch              Ticket      Fare            Cabin Embarked                       listtest                       dicttest
+0              1        0       3        Braund, Mr. Owen Harris    male  22.00      1      0           A/5 21171    7.2500              NaN        S  [[[27, 71], [27, 71], [27,...  {36: 67, 73: 54, 56: 48, 8...
+1              2     True       1  Cumings, Mrs. John Bradley...  female  38.00      1      0            PC 17599   71.2833              C85        C  [[[31, 68], [31, 68], [31,...                        {9: 77}
+2              3     True       3         Heikkinen, Miss. Laina  female  26.00      0      0    STON/O2. 3101282    7.9250              NaN        S                   [[[31, 23]]]  {49: 6, 76: 22, 52: 18, 6:...
+3              4     True       1  Futrelle, Mrs. Jacques Hea...  female  35.00      1      0              113803   53.1000             C123        S  [[[96, 48], [96, 48], [96,...  {27: 90, 9: 38, 18: 94, 67...
+4              5        0       3       Allen, Mr. William Henry    male  35.00      0      0              373450    8.0500              NaN        S  [[[60, 84], [60, 84], [60,...  {8: 61, 37: 4, 25: 43, 21:...
+5              6        0       3               Moran, Mr. James    male    NaN      0      0              330877    8.4583              NaN        Q         [[[25, 39], [25, 39]]]       {97: 78, 85: 88, 42: 34}
+
+
+
+df.shortloc_not_in_iter('listtest', list(range(0,90)))
+     PassengerId  Survived  Pclass                           Name     Sex   Age  SibSp  Parch      Ticket      Fare Cabin Embarked                       listtest                       dicttest
+832          833         0       3                 Saad, Mr. Amin    male   NaN      0      0        2671    7.2292   NaN        C  [[[95, 94], [95, 94], [95,...                {82: 66, 84: 5}
+484          485         1       1        Bishop, Mr. Dickinson H    male  25.0      1      0       11967   91.0792   B49        C  [[[97, 92], [97, 92], [97,...  {20: 34, 2: 23, 98: 37, 1:...
+581          582         1       1  Thayer, Mrs. John Borland ...  female  39.0      1      1       17421  110.8833   C68        C         [[[91, 90], [91, 90]]]  {48: 98, 3: 98, 93: 4, 97:...
+336          337         0       1      Pears, Mr. Thomas Clinton    male  29.0      1      0      113776   66.6000    C2        S         [[[90, 98], [90, 98]]]                         {6: 7}
+116          117         0       3           Connors, Mr. Patrick    male  70.5      0      0      370369    7.7500   NaN        Q  [[[92, 99], [92, 99], [92,...  {60: 79, 75: 71, 28: 68, 5...
+52            53         1       1  Harper, Mrs. Henry Sleeper...  female  49.0      1      0    PC 17572   76.7292   D33        C  [[[96, 94], [96, 94], [96,...  {20: 53, 93: 11, 83: 79, 5...
+439          440         0       2  Kvillner, Mr. Johan Henrik...    male  31.0      0      0  C.A. 18723   10.5000   NaN        S  [[[95, 98], [95, 98], [95,...  {58: 11, 89: 23, 22: 66, 1...
+56            57         1       2              Rugg, Miss. Emily  female  21.0      0      0  C.A. 31026   10.5000   NaN        S  [[[92, 92], [92, 92], [92,...                {45: 1, 37: 98}
+
+
+
+df.shortloc_not_in_iter_replace('listtest', list(range(0,20)), 27)
+     PassengerId  Survived  Pclass                           Name     Sex    Age  SibSp  Parch              Ticket      Fare            Cabin Embarked                       listtest                       dicttest
+0              1         0       3        Braund, Mr. Owen Harris    male  22.00      1      0           A/5 21171    7.2500              NaN        S                             27  {36: 67, 73: 54, 56: 48, 8...
+1              2         1       1  Cumings, Mrs. John Bradley...  female  38.00      1      0            PC 17599   71.2833              C85        C                             27                        {9: 77}
+2              3         1       3         Heikkinen, Miss. Laina  female  26.00      0      0    STON/O2. 3101282    7.9250              NaN        S                             27  {49: 6, 76: 22, 52: 18, 6:...
+3              4         1       1  Futrelle, Mrs. Jacques Hea...  female  35.00      1      0              113803   53.1000             C123        S                             27  {27: 90, 9: 38, 18: 94, 67...
+4              5         0       3       Allen, Mr. William Henry    male  35.00      0      0              373450    8.0500              NaN        S                             27  {8: 61, 37: 4, 25: 43, 21:...
+5              6         0       3               Moran, Mr. James    male    NaN      0      0              330877    8.4583              NaN        Q                             27       {97: 78, 85: 88, 42: 34}
+6              7         0       1        McCarthy, Mr. Timothy J    male  54.00      0      0               17463   51.8625              E46        S  [[[76, 5], [76, 5], [76, 5...  {56: 51, 13: 24, 84: 24, 9...
+
+
+df.shortloc_regex('Fare', r'^\d?7\.').to_string(max_colwidth=30)
+     PassengerId  Survived  Pclass                           Name     Sex   Age  SibSp  Parch              Ticket     Fare  Cabin Embarked                       listtest                       dicttest
+0              1         0       3        Braund, Mr. Owen Harris    male  22.0      1      0           A/5 21171   7.2500    NaN        S  [[[27, 71], [27, 71], [27,...  {36: 67, 73: 54, 56: 48, 8...
+2              3         1       3         Heikkinen, Miss. Laina  female  26.0      0      0    STON/O2. 3101282   7.9250    NaN        S                   [[[31, 23]]]  {49: 6, 76: 22, 52: 18, 6:...
+14            15         0       3  Vestrom, Miss. Hulda Amand...  female  14.0      0      0              350406   7.8542    NaN        S  [[[40, 57], [40, 57], [40,...  {54: 39, 8: 35, 76: 84, 20...
+19            20         1       3        Masselmani, Mrs. Fatima  female   NaN      0      0                2649   7.2250    NaN        C  [[[11, 37], [11, 37], [11,...  {43: 73, 50: 28, 38: 47, 4...
+26            27         0       3        Emir, Mr. Farred Chehab    male   NaN      0      0                2631   7.2250    NaN        C  [[[48, 66], [48, 66], [48,...               {33: 45, 82: 90}
+28            29         1       3  O'Dwyer, Miss. Ellen "Nellie"  female   NaN      0      0              330959   7.8792    NaN        Q           [[[3, 53], [3, 53]]]               {29: 90, 84: 86}
+29            30         0       3            Todoroff, Mr. Lalio    male   NaN      0      0              349216   7.8958    NaN        S  [[[67, 3], [67, 3], [67, 3...  {57: 49, 23: 71, 64: 45, 1...
+30            31         0       1       Uruchurtu, Don. Manuel E    male  40.0      0      0            PC 17601  27.7208    NaN        C  [[[91, 32], [91, 32], [91,...         {1: 29, 54: 93, 96: 7}
+
+
+
+df.shortloc_not_regex('Fare', r'^\d?7\.').to_string(max_colwidth=30)
+     PassengerId  Survived  Pclass                           Name     Sex    Age  SibSp  Parch             Ticket      Fare            Cabin Embarked                       listtest                       dicttest
+1              2         1       1  Cumings, Mrs. John Bradley...  female  38.00      1      0           PC 17599   71.2833              C85        C  [[[31, 68], [31, 68], [31,...                        {9: 77}
+3              4         1       1  Futrelle, Mrs. Jacques Hea...  female  35.00      1      0             113803   53.1000             C123        S  [[[96, 48], [96, 48], [96,...  {27: 90, 9: 38, 18: 94, 67...
+4              5         0       3       Allen, Mr. William Henry    male  35.00      0      0             373450    8.0500              NaN        S  [[[60, 84], [60, 84], [60,...  {8: 61, 37: 4, 25: 43, 21:...
+5              6         0       3               Moran, Mr. James    male    NaN      0      0             330877    8.4583              NaN        Q         [[[25, 39], [25, 39]]]       {97: 78, 85: 88, 42: 34}
+6              7         0       1        McCarthy, Mr. Timothy J    male  54.00      0      0              17463   51.8625              E46        S  [[[76, 5], [76, 5], [76, 5...  {56: 51, 13: 24, 84: 24, 9...
+7              8         0       3  Palsson, Master. Gosta Leo...    male   2.00      3      1             349909   21.0750              NaN        S  [[[42, 52], [42, 52], [42,...               {71: 69, 44: 14}
+8              9         1       3  Johnson, Mrs. Oscar W (Eli...  female  27.00      0      2             347742   11.1333              NaN        S  [[[92, 21], [92, 21], [92,...  {61: 17, 72: 44, 81: 74, 3...
+9             10         1       2  Nasser, Mrs. Nicholas (Ade...  female  14.00      1      0             237736   30.0708              NaN        C  [[[88, 97], [88, 97], [88,...                       {69: 43}
+
+
+df.shortloc_str('Pclass', r'3').to_string(max_colwidth=30)
+     PassengerId  Survived  Pclass                           Name     Sex    Age  SibSp  Parch              Ticket     Fare  Cabin Embarked                       listtest                       dicttest
+0              1         0       3        Braund, Mr. Owen Harris    male  22.00      1      0           A/5 21171   7.2500    NaN        S  [[[27, 71], [27, 71], [27,...  {36: 67, 73: 54, 56: 48, 8...
+2              3         1       3         Heikkinen, Miss. Laina  female  26.00      0      0    STON/O2. 3101282   7.9250    NaN        S                   [[[31, 23]]]  {49: 6, 76: 22, 52: 18, 6:...
+4              5         0       3       Allen, Mr. William Henry    male  35.00      0      0              373450   8.0500    NaN        S  [[[60, 84], [60, 84], [60,...  {8: 61, 37: 4, 25: 43, 21:...
+5              6         0       3               Moran, Mr. James    male    NaN      0      0              330877   8.4583    NaN        Q         [[[25, 39], [25, 39]]]       {97: 78, 85: 88, 42: 34}
+7              8         0       3  Palsson, Master. Gosta Leo...    male   2.00      3      1              349909  21.0750    NaN        S  [[[42, 52], [42, 52], [42,...               {71: 69, 44: 14}
+8              9         1       3  Johnson, Mrs. Oscar W (Eli...  female  27.00      0      2              347742  11.1333    NaN        S  [[[92, 21], [92, 21], [92,...  {61: 17, 72: 44, 81: 74, 3...
+10            11         1       3  Sandstrom, Miss. Marguerit...  female   4.00      1      1             PP 9549  16.7000     G6        S  [[[28, 63], [28, 63], [28,...  {12: 80, 63: 96, 79: 99, 5...
+12            13         0       3  Saundercock, Mr. William H...    male  20.00      0      0           A/5. 2151   8.0500    NaN        S  [[[34, 91], [34, 91], [34,...  {42: 68, 46: 90, 66: 96, 3...
+13            14         0       3    Andersson, Mr. Anders Johan    male  39.00      1      5              347082  31.2750    NaN        S  [[[3, 47], [3, 47], [3, 47...  {94: 60, 73: 33, 59: 32, 3...
+14            15         0       3  Vestrom, Miss. Hulda Amand...  female  14.00      0      0              350406   7.8542    NaN        S  [[[40, 57], [40, 57], [40,...  {54: 39, 8: 35, 76: 84, 20...
+16            17         0       3           Rice, Master. Eugene    male   2.00      4      1              382652  29.1250    NaN        Q  [[[24, 8], [24, 8], [24, 8...  {20: 91, 56: 55, 11: 16, 3...
+
+
+
+df.shortloc_str_replace('Pclass', r'3',4).to_string(max_colwidth=30)
+     PassengerId  Survived  Pclass                           Name     Sex    Age  SibSp  Parch              Ticket      Fare            Cabin Embarked                       listtest                       dicttest
+0              1         0       4        Braund, Mr. Owen Harris    male  22.00      1      0           A/5 21171    7.2500              NaN        S  [[[27, 71], [27, 71], [27,...  {36: 67, 73: 54, 56: 48, 8...
+1              2         1       1  Cumings, Mrs. John Bradley...  female  38.00      1      0            PC 17599   71.2833              C85        C  [[[31, 68], [31, 68], [31,...                        {9: 77}
+2              3         1       4         Heikkinen, Miss. Laina  female  26.00      0      0    STON/O2. 3101282    7.9250              NaN        S                   [[[31, 23]]]  {49: 6, 76: 22, 52: 18, 6:...
+3              4         1       1  Futrelle, Mrs. Jacques Hea...  female  35.00      1      0              113803   53.1000             C123        S  [[[96, 48], [96, 48], [96,...  {27: 90, 9: 38, 18: 94, 67...
+4              5         0       4       Allen, Mr. William Henry    male  35.00      0      0              373450    8.0500              NaN        S  [[[60, 84], [60, 84], [60,...  {8: 61, 37: 4, 25: 43, 21:...
+5              6         0       4               Moran, Mr. James    male    NaN      0      0              330877    8.4583              NaN        Q         [[[25, 39], [25, 39]]]       {97: 78, 85: 88, 42: 34}
+6              7         0       1        McCarthy, Mr. Timothy J    male  54.00      0      0               17463   51.8625              E46        S  [[[76, 5], [76, 5], [76, 5...  {56: 51, 13: 24, 84: 24, 9...
+7              8         0       4  Palsson, Master. Gosta Leo...    male   2.00      3      1              349909   21.0750              NaN        S  [[[42, 52], [42, 52], [42,...               {71: 69, 44: 14}
+8              9         1       4  Johnson, Mrs. Oscar W (Eli...  female  27.00      0      2              347742   11.1333              NaN        S  [[[92, 21], [92, 21], [92,...  {61: 17, 72: 44, 81: 74, 3...
+9             10         1       2  Nasser, Mrs. Nicholas (Ade...  female  14.00      1      0              237736   30.0708              NaN        C  [[[88, 97], [88, 97], [88,...                       {69: 43}
+10            11         1       4  Sandstrom, Miss. Marguerit...  female   4.00      1      1             PP 9549   16.7000               G6        S  [[[28, 63], [28, 63], [28,...  {12: 80, 63: 96, 79: 99, 5...
+
+
+
+
+df.loc_positive_and(
+   ("Pclass", "==", 3),
+   ("Sex", "!=", "male"),
+   ("Age", ">=", 1),
+   ("Pclass", ">=", 3),
+   ("listtest", "in_iter", [11, 22, 33, 44, 55, 66, 77, 88, 99]),
+   ("Sex", "in", ["female", "male"]),
+   ("Name", "re", r"Miss\."),
+   ("Ticket", ">", 5000),
+   ("Embarked", "str", "S"),
+)
+
+     PassengerId  Survived  Pclass                           Name     Sex   Age  SibSp  Parch  Ticket     Fare Cabin Embarked                       listtest                       dicttest
+24            25         0       3  Palsson, Miss. Torborg Danira  female   8.0      3      1  349909  21.0750   NaN        S  [[[44, 33], [44, 33], [44,...  {98: 85, 8: 23, 21: 77, 85...
+141          142         1       3       Nysten, Miss. Anna Sofia  female  22.0      0      0  347081   7.7500   NaN        S                   [[[44, 30]]]  {25: 15, 24: 14, 16: 26, 5...
+192          193         1       3  Andersen-Jensen, Miss. Car...  female  19.0      1      0  350046   7.8542   NaN        S  [[[39, 55], [39, 55], [39,...  {1: 44, 16: 59, 80: 13, 81...
+634          635         0       3             Skoog, Miss. Mabel  female   9.0      3      2  347088  27.9000   NaN        S                   [[[11, 22]]]                        {40: 7}
+
+
+
+df.loc_positive_and(('Ticket','==', 373450), ('Pclass','==', 3))
+   PassengerId  Survived  Pclass                      Name   Sex   Age  SibSp  Parch  Ticket  Fare Cabin Embarked                       listtest                       dicttest
+4            5         0       3  Allen, Mr. William Henry  male  35.0      0      0  373450  8.05   NaN        S  [[[60, 84], [60, 84], [60,...  {8: 61, 37: 4, 25: 43, 21:...
+
+
+df.loc_positive_or(('Ticket','==', 373450), ('Pclass','==', 3))
+     PassengerId  Survived  Pclass                           Name     Sex    Age  SibSp  Parch              Ticket     Fare  Cabin Embarked                       listtest                       dicttest
+0              1         0       3        Braund, Mr. Owen Harris    male  22.00      1      0           A/5 21171   7.2500    NaN        S  [[[27, 71], [27, 71], [27,...  {36: 67, 73: 54, 56: 48, 8...
+2              3         1       3         Heikkinen, Miss. Laina  female  26.00      0      0    STON/O2. 3101282   7.9250    NaN        S                   [[[31, 23]]]  {49: 6, 76: 22, 52: 18, 6:...
+4              5         0       3       Allen, Mr. William Henry    male  35.00      0      0              373450   8.0500    NaN        S  [[[60, 84], [60, 84], [60,...  {8: 61, 37: 4, 25: 43, 21:...
+5              6         0       3               Moran, Mr. James    male    NaN      0      0              330877   8.4583    NaN        Q         [[[25, 39], [25, 39]]]       {97: 78, 85: 88, 42: 34}
+7              8         0       3  Palsson, Master. Gosta Leo...    male   2.00      3      1              349909  21.0750    NaN        S  [[[42, 52], [42, 52], [42,...               {71: 69, 44: 14}
+
+
+
+df.loc_positive_and(('Age','>=', 13), ('Age','<=', 19))
+     PassengerId  Survived  Pclass                           Name     Sex   Age  SibSp  Parch             Ticket      Fare            Cabin Embarked                       listtest                       dicttest
+9             10         1       2  Nasser, Mrs. Nicholas (Ade...  female  14.0      1      0             237736   30.0708              NaN        C  [[[88, 97], [88, 97], [88,...                       {69: 43}
+14            15         0       3  Vestrom, Miss. Hulda Amand...  female  14.0      0      0             350406    7.8542              NaN        S  [[[40, 57], [40, 57], [40,...  {54: 39, 8: 35, 76: 84, 20...
+22            23         1       3    McGowan, Miss. Anna "Annie"  female  15.0      0      0             330923    8.0292              NaN        Q  [[[85, 85], [85, 85], [85,...  {80: 2, 70: 5, 27: 24, 10:...
+27            28         0       1  Fortune, Mr. Charles Alexa...    male  19.0      3      2              19950  263.0000      C23 C25 C27        S  [[[7, 96], [7, 96], [7, 96...  {60: 4, 22: 96, 55: 28, 97...
+38            39         0       3  Vander Planke, Miss. Augus...  female  18.0      2      0             345764   18.0000              NaN        S  [[[82, 50], [82, 50], [82,...  {70: 41, 90: 86, 46: 95, 3...
+39            40         1       3    Nicola-Yarred, Miss. Jamila  female  14.0      1      0               2651   11.2417              NaN        C  [[[20, 72], [20, 72], [20,...  {72: 91, 81: 15, 89: 24, 9...
+44            45         1       3  Devaney, Miss. Margaret Delia  female  19.0      0      0             330958    7.8792              NaN        Q  [[[97, 1], [97, 1], [97, 1...  {89: 44, 58: 86, 48: 54, 9...
+49            50         0       3  Arnold-Franchi, Mrs. Josef...  female  18.0      1      0             349237   17.8000              NaN        S         [[[64, 68], [64, 68]]]  {67: 59, 96: 34, 8: 64, 45...
+67            68         0       3       Crease, Mr. Ernest James    male  19.0      0      0          S.P. 3464    8.1583              NaN        S  [[[30, 77], [30, 77], [30,...  {37: 56, 52: 5, 80: 12, 86...
+
+
+
+df.loc_positive_and(('Ticket','!=', 373450), ('Pclass','!=', 3))
+     PassengerId  Survived  Pclass                           Name     Sex    Age  SibSp  Parch            Ticket      Fare            Cabin Embarked                       listtest                       dicttest
+1              2         1       1  Cumings, Mrs. John Bradley...  female  38.00      1      0          PC 17599   71.2833              C85        C  [[[31, 68], [31, 68], [31,...                        {9: 77}
+3              4         1       1  Futrelle, Mrs. Jacques Hea...  female  35.00      1      0            113803   53.1000             C123        S  [[[96, 48], [96, 48], [96,...  {27: 90, 9: 38, 18: 94, 67...
+6              7         0       1        McCarthy, Mr. Timothy J    male  54.00      0      0             17463   51.8625              E46        S  [[[76, 5], [76, 5], [76, 5...  {56: 51, 13: 24, 84: 24, 9...
+9             10         1       2  Nasser, Mrs. Nicholas (Ade...  female  14.00      1      0            237736   30.0708              NaN        C  [[[88, 97], [88, 97], [88,...                       {69: 43}
+11            12         1       1       Bonnell, Miss. Elizabeth  female  58.00      0      0            113783   26.5500             C103        S         [[[66, 84], [66, 84]]]  {87: 7, 75: 62, 84: 22, 94...
+15            16         1       2  Hewlett, Mrs. (Mary D King...  female  55.00      0      0            248706   16.0000              NaN        S  [[[93, 7], [93, 7], [93, 7...  {17: 96, 7: 68, 74: 5, 97:...
+
+
+df.loc_negative_and(('Age','>=', 13), ('Sex','str', 'female'))
+     PassengerId  Survived  Pclass                           Name   Sex    Age  SibSp  Parch           Ticket      Fare    Cabin Embarked                       listtest                       dicttest
+386          387         0       3  Goodwin, Master. Sidney Le...  male   1.00      5      2          CA 2144   46.9000      NaN        S  [[[32, 26], [32, 26], [32,...  {42: 33, 97: 56, 33: 73, 7...
+261          262         1       3  Asplund, Master. Edvin Roj...  male   3.00      4      2           347077   31.3875      NaN        S  [[[40, 73], [40, 73], [40,...  {7: 23, 93: 3, 18: 66, 96:...
+7              8         0       3  Palsson, Master. Gosta Leo...  male   2.00      3      1           349909   21.0750      NaN        S  [[[42, 52], [42, 52], [42,...               {71: 69, 44: 14}
+16            17         0       3           Rice, Master. Eugene  male   2.00      4      1           382652   29.1250      NaN        Q  [[[24, 8], [24, 8], [24, 8...  {20: 91, 56: 55, 11: 16, 3...
+787          788         0       3      Rice, Master. George Hugh  male   8.00      4      1           382652   29.1250      NaN        Q  [[[32, 90], [32, 90], [32,...  {5: 17, 83: 1, 82: 16, 21:...
+788          789         1       3     Dean, Master. Bertram Vere  male   1.00      1      2        C.A. 2315   20.5750      NaN        S  [[[27, 72], [27, 72], [27,...       {58: 65, 42: 92, 61: 72}
+278          279         0       3             Rice, Master. Eric  male   7.00      4      1           382652   29.1250      NaN        Q  [[[48, 59], [48, 59], [48,...  {16: 64, 97: 83, 66: 91, 9...
+
+
+
+df.shortloc_regex('Name', '^Ab').shortloc_not_equal('Sex', 'male').shortloc_equal('Age', 35)
+     PassengerId  Survived  Pclass                           Name     Sex   Age  SibSp  Parch     Ticket   Fare Cabin Embarked                       listtest                       dicttest
+279          280         1       3  Abbott, Mrs. Stanton (Rosa...  female  35.0      1      1  C.A. 2673  20.25   NaN        S  [[[93, 85], [93, 85], [93,...  {37: 16, 68: 58, 42: 7, 20...
+
+
+
+df.shortloc_in_iter('dicttest', 65).shortloc_not_in_iter('listtest', [77,65,80,83])
+     PassengerId  Survived  Pclass                           Name     Sex   Age  SibSp  Parch       Ticket      Fare        Cabin Embarked                       listtest                       dicttest
+515          516         0       1   Walker, Mr. William Anderson    male  47.0      0      0        36967   34.0208          D46        S  [[[55, 13], [55, 13], [55,...  {67: 25, 73: 76, 93: 74, 6...
+772          773         0       2              Mack, Mrs. (Mary)  female  57.0      0      0  S.O./P.P. 3   10.5000          E77        S  [[[3, 67], [3, 67], [3, 67...  {20: 62, 88: 78, 22: 65, 1...
+518          519         1       2  Angle, Mrs. William A (Flo...  female  36.0      1      0       226875   26.0000          NaN        S         [[[78, 94], [78, 94]]]  {32: 53, 48: 66, 20: 5, 67...
+10            11         1       3  Sandstrom, Miss. Marguerit...  female   4.0      1      1      PP 9549   16.7000           G6        S  [[[28, 63], [28, 63], [28,...  {12: 80, 63: 96, 79: 99, 5...
+275          276         1       1  Andrews, Miss. Kornelia Th...  female  63.0      1      0        13502   77.9583           D7        S                   [[[84, 21]]]  {31: 95, 27: 48, 89: 25, 6...
+788          789         1       3     Dean, Master. Bertram Vere    male   1.0      1      2    C.A. 2315   20.5750          NaN        S  [[[27, 72], [27, 72], [27,...       {58: 65, 42: 92, 61: 72}
+
+
+
+df.shortloc_not_isna("Cabin").shortloc_str("Cabin", "C").shortloc_not_regex(
+   "Cabin", "^.{4,}$"
+)
+     PassengerId  Survived  Pclass                           Name     Sex   Age  SibSp  Parch    Ticket      Fare Cabin Embarked                       listtest                       dicttest
+1              2         1       1  Cumings, Mrs. John Bradley...  female  38.0      1      0  PC 17599   71.2833   C85        C  [[[31, 68], [31, 68], [31,...                        {9: 77}
+269          270         1       1         Bissette, Miss. Amelia  female  35.0      0      0  PC 17760  135.6333   C99        S  [[[89, 54], [89, 54], [89,...  {50: 9, 91: 60, 30: 67, 46...
+527          528         0       1             Farthing, Mr. John    male   NaN      0      0  PC 17483  221.7792   C95        S  [[[9, 72], [9, 72], [9, 72...               {41: 24, 63: 10}
+151          152         1       1  Pears, Mrs. Thomas (Edith ...  female  22.0      1      0    113776   66.6000    C2        S  [[[24, 98], [24, 98], [24,...  {80: 92, 25: 89, 32: 82, 1...
+412          413         1       1         Minahan, Miss. Daisy E  female  33.0      1      0     19928   90.0000   C78        Q                    [[[2, 41]]]                       {57: 41}
+544          545         0       1     Douglas, Mr. Walter Donald    male  50.0      1      0  PC 17761  106.4250   C86        C  [[[55, 21], [55, 21], [55,...               {51: 49, 16: 20}
+550          551         1       1    Thayer, Mr. John Borland Jr    male  17.0      0      2     17421  110.8833   C70        C  [[[37, 20], [37, 20], [37,...               {17: 85, 49: 77}
+430          431         1       1  Bjornstrom-Steffansson, Mr...    male  28.0      0      0    110564   26.5500   C52        S  [[[14, 61], [14, 61], [14,...                       {62: 40}
+
+
+df.shortloc_in_iter('listtest',[99, 77]).shortloc_regex('listtest',r"7\b,\s*\b9"))
+     PassengerId  Survived  Pclass                  Name     Sex   Age  SibSp  Parch Ticket     Fare Cabin Embarked                       listtest                       dicttest
+111          112         0       3  Zabour, Miss. Hileni  female  14.5      1      0   2665  14.4542   NaN        C  [[[27, 99], [27, 99], [27,...  {76: 81, 62: 60, 98: 43, 5...
+
+
+#all methods can also be used against Series
+#Two examples
+
+df.Pclass.shortloc_regex('^2$')
+Out[54]: 
+9      2
+15     2
+17     2
+20     2
+21     2
+      ..
+
+df.Pclass.shortloc_regex_replace('^3$',2000)
+Out[56]: 
+0      2000
+1         1
+2      2000
+3         1
+4      2000
+       ... 
 ```
```

### Comparing `a_pandas_ex_easy_loc-0.13/setup.py` & `a_pandas_ex_easy_loc-0.14/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 from setuptools import setup, find_packages
-import codecs
-import os
+# import codecs
+# import os
+# 
+# here = os.path.abspath(os.path.dirname(__file__))
+# 
+# with codecs.open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'README.md'), encoding="utf-8") as fh:
+#     long_description = "\n" + fh.read()\
 
-here = os.path.abspath(os.path.dirname(__file__))
+from pathlib import Path
+this_directory = Path(__file__).parent
+long_description = (this_directory / "README.md").read_text()
 
-with codecs.open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'README.md'), encoding="utf-8") as fh:
-    long_description = "\n" + fh.read()
-
-VERSION = '''0.13'''
+VERSION = '''0.14'''
 DESCRIPTION = '''Search and replace values with df.loc without Exceptions due to dtype incompatibility'''
 
 # Setting up
 setup(
     name="a_pandas_ex_easy_loc",
     version=VERSION,
     license='MIT',
     url = 'https://github.com/hansalemaos/a_pandas_ex_easy_loc',
     author="Johannes Fischer",
     author_email="aulasparticularesdealemaosp@gmail.com",
     description=DESCRIPTION,
-    long_description_content_type="text/markdown",
-    long_description=long_description,
+long_description = long_description,
+long_description_content_type="text/markdown",
     #packages=['a_pandas_ex_less_memory_more_speed', 'a_pandas_ex_plode_tool', 'cprinter', 'flatten_everything', 'numpy', 'pandas'],
     keywords=['loc', 'iloc', 'df.at', 'df.iat', 'pandas', 'DataFrame', 'Series'],
     classifiers=['Development Status :: 4 - Beta', 'Programming Language :: Python :: 3 :: Only', 'Programming Language :: Python :: 3.10', 'Topic :: Software Development :: Libraries :: Python Modules', 'Topic :: Utilities'],
     install_requires=['a_pandas_ex_less_memory_more_speed', 'a_pandas_ex_plode_tool', 'cprinter', 'flatten_everything', 'numpy', 'pandas'],
     include_package_data=True
 )
 #python setup.py sdist bdist_wheel
```

