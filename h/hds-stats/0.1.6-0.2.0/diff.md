# Comparing `tmp/hds-stats-0.1.6.tar.gz` & `tmp/hds-stats-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hds-stats-0.1.6.tar", last modified: Sat Apr 15 14:43:00 2023, max compression
+gzip compressed data, was "hds-stats-0.2.0.tar", last modified: Sat Apr 15 14:53:25 2023, max compression
```

## Comparing `hds-stats-0.1.6.tar` & `hds-stats-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 hdsceokevin   (501) staff       (20)        0 2023-04-15 14:43:00.349420 hds-stats-0.1.6/
--rw-rw-r--   0 hdsceokevin   (501) staff       (20)     1073 2023-04-09 06:26:23.000000 hds-stats-0.1.6/LICENSE
--rw-r--r--   0 hdsceokevin   (501) staff       (20)      632 2023-04-15 14:43:00.349167 hds-stats-0.1.6/PKG-INFO
--rw-rw-r--   0 hdsceokevin   (501) staff       (20)       65 2023-04-09 06:26:23.000000 hds-stats-0.1.6/README.md
-drwxr-xr-x   0 hdsceokevin   (501) staff       (20)        0 2023-04-15 14:43:00.347314 hds-stats-0.1.6/hds_stats/
--rw-r--r--   0 hdsceokevin   (501) staff       (20)       82 2023-04-09 20:34:59.000000 hds-stats-0.1.6/hds_stats/__init__.py
--rw-r--r--   0 hdsceokevin   (501) staff       (20)    11220 2023-04-15 14:30:59.000000 hds-stats-0.1.6/hds_stats/plot.py
--rw-r--r--   0 hdsceokevin   (501) staff       (20)    26553 2023-04-15 14:41:45.000000 hds-stats-0.1.6/hds_stats/stat.py
-drwxr-xr-x   0 hdsceokevin   (501) staff       (20)        0 2023-04-15 14:43:00.348799 hds-stats-0.1.6/hds_stats.egg-info/
--rw-r--r--   0 hdsceokevin   (501) staff       (20)      632 2023-04-15 14:43:00.000000 hds-stats-0.1.6/hds_stats.egg-info/PKG-INFO
--rw-r--r--   0 hdsceokevin   (501) staff       (20)      263 2023-04-15 14:43:00.000000 hds-stats-0.1.6/hds_stats.egg-info/SOURCES.txt
--rw-r--r--   0 hdsceokevin   (501) staff       (20)        1 2023-04-15 14:43:00.000000 hds-stats-0.1.6/hds_stats.egg-info/dependency_links.txt
--rw-r--r--   0 hdsceokevin   (501) staff       (20)       63 2023-04-15 14:43:00.000000 hds-stats-0.1.6/hds_stats.egg-info/requires.txt
--rw-r--r--   0 hdsceokevin   (501) staff       (20)       20 2023-04-15 14:43:00.000000 hds-stats-0.1.6/hds_stats.egg-info/top_level.txt
--rw-r--r--   0 hdsceokevin   (501) staff       (20)      104 2023-04-03 08:08:53.000000 hds-stats-0.1.6/pyproject.toml
--rw-r--r--   0 hdsceokevin   (501) staff       (20)       38 2023-04-15 14:43:00.349509 hds-stats-0.1.6/setup.cfg
--rw-r--r--   0 hdsceokevin   (501) staff       (20)     1177 2023-04-15 14:41:57.000000 hds-stats-0.1.6/setup.py
+drwxr-xr-x   0 hdsceokevin   (501) staff       (20)        0 2023-04-15 14:53:25.182725 hds-stats-0.2.0/
+-rw-rw-r--   0 hdsceokevin   (501) staff       (20)     1073 2023-04-09 06:26:23.000000 hds-stats-0.2.0/LICENSE
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)      632 2023-04-15 14:53:25.182486 hds-stats-0.2.0/PKG-INFO
+-rw-rw-r--   0 hdsceokevin   (501) staff       (20)       65 2023-04-09 06:26:23.000000 hds-stats-0.2.0/README.md
+drwxr-xr-x   0 hdsceokevin   (501) staff       (20)        0 2023-04-15 14:53:25.180718 hds-stats-0.2.0/hds_stats/
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)       82 2023-04-09 20:34:59.000000 hds-stats-0.2.0/hds_stats/__init__.py
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)    11840 2023-04-15 14:49:49.000000 hds-stats-0.2.0/hds_stats/plot.py
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)    27199 2023-04-15 14:49:49.000000 hds-stats-0.2.0/hds_stats/stat.py
+drwxr-xr-x   0 hdsceokevin   (501) staff       (20)        0 2023-04-15 14:53:25.182141 hds-stats-0.2.0/hds_stats.egg-info/
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)      632 2023-04-15 14:53:25.000000 hds-stats-0.2.0/hds_stats.egg-info/PKG-INFO
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)      263 2023-04-15 14:53:25.000000 hds-stats-0.2.0/hds_stats.egg-info/SOURCES.txt
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)        1 2023-04-15 14:53:25.000000 hds-stats-0.2.0/hds_stats.egg-info/dependency_links.txt
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)       63 2023-04-15 14:53:25.000000 hds-stats-0.2.0/hds_stats.egg-info/requires.txt
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)       20 2023-04-15 14:53:25.000000 hds-stats-0.2.0/hds_stats.egg-info/top_level.txt
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)      104 2023-04-03 08:08:53.000000 hds-stats-0.2.0/pyproject.toml
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)       38 2023-04-15 14:53:25.182807 hds-stats-0.2.0/setup.cfg
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)     1178 2023-04-15 14:52:36.000000 hds-stats-0.2.0/setup.py
```

### Comparing `hds-stats-0.1.6/LICENSE` & `hds-stats-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hds-stats-0.1.6/PKG-INFO` & `hds-stats-0.2.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hds-stats
-Version: 0.1.6
+Version: 0.2.0
 Summary: Useful functions for Statistics and Machine Learning
 Home-page: https://github.com/HelloDataScience/hds-stats
 Author: HelloDataScience
 Author-email: hellodatasciencekorea@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/HelloDataScience/hds-stats/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hds-stats-0.1.6/hds_stats/plot.py` & `hds-stats-0.2.0/hds_stats/plot.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,8 @@
 
-# 의존성 라이브러리 호출
-def import_library():
-    import numpy as np
-    import pandas as pd
-    from scipy import stats
-    import seaborn as sns
-    import matplotlib.pyplot as plt
-
-
 # 집단별 상자 수염 그림을 그리는 함수
 def box_group(data, x: str, y: str, pal: list = None) -> None:
     '''
     이 함수는 범주형 변수(x축)에 따라 연속형 변수(y축)의 상자 수염 그림을 그립니다.
     상자에 빨간 점은 해당 범주의 평균이며, 가로 직선은 전체 평균입니다.
     
     매개변수:
@@ -19,15 +10,19 @@
         x: 범주형 변수명을 문자열로 지정합니다.
         y: 연속형 변수명을 문자열로 지정합니다.
         pal: 팔레트를 리스트로 지정합니다.
     
     반환:
         그래프 외에 반환하는 객체는 없습니다.
     '''
-    import_library()
+    import numpy as np
+    import pandas as pd
+    from scipy import stats
+    import seaborn as sns
+    import matplotlib.pyplot as plt
     
     avg = data.groupby(x)[y].mean().reset_index()
     
     sns.boxplot(
         data = data, 
         x = x, 
         y = y, 
@@ -71,15 +66,19 @@
         x: 원인이 되는 연속형 변수명을 문자열로 지정합니다.
         y: 결과가 되는 연속형 변수명을 문자열로 지정합니다.
         color: 점의 채우기 색을 문자열로 지정합니다.(기본값: '0.3')
     
     반환:
         그래프 외에 반환하는 객체는 없습니다.
     '''
-    import_library()
+    import numpy as np
+    import pandas as pd
+    from scipy import stats
+    import seaborn as sns
+    import matplotlib.pyplot as plt
     
     sns.scatterplot(
         data = data, 
         x = x, 
         y = y, 
         color = color
     )
@@ -98,16 +97,20 @@
         y: 결과가 되는 연속형 변수명을 문자열로 지정합니다.
         color: 점의 채우기 색을 문자열로 지정합니다.(기본값: '0.3')
         size: 점의 크기를 정수로 지정합니다.(기본값: 15)
     
     반환:
         그래프 외에 반환하는 객체는 없습니다.
     '''
-    import_library()
-    
+    import numpy as np
+    import pandas as pd
+    from scipy import stats
+    import seaborn as sns
+    import matplotlib.pyplot as plt
+        
     sns.regplot(
         data = data, 
         x = x, 
         y = y, 
         ci = None, 
         scatter_kws = {
             'color': color, 
@@ -138,15 +141,19 @@
         x: 범주형 변수명을 문자열로 지정합니다.
         color: 점의 채우기 색을 문자열로 지정합니다.
         pal: 팔레트를 리스트로 지정합니다.
     
     반환:
         그래프 외에 반환하는 객체는 없습니다.
     '''
-    import_library()
+    import numpy as np
+    import pandas as pd
+    from scipy import stats
+    import seaborn as sns
+    import matplotlib.pyplot as plt
     
     grp = data[x].value_counts()
     v_max = grp.values.max()
     space = np.ceil(v_max * 0.01)
     
     sns.countplot(
         data = data, 
@@ -180,15 +187,19 @@
         x: 범주형 변수명을 문자열로 지정합니다.
         group: x를 소그룹으로 나눌 범주형 변수명을 문자열로 지정합니다.
         pal: 팔레트를 리스트로 지정합니다.
     
     반환:
         그래프 외에 반환하는 객체는 없습니다.
     '''
-    import_library()
+    import numpy as np
+    import pandas as pd
+    from scipy import stats
+    import seaborn as sns
+    import matplotlib.pyplot as plt
     
     grp = data.groupby(by = [x, group]).count().iloc[:, 0]
     v_max = grp.values.max()
     space = np.ceil(v_max * 0.01)
     
     sns.countplot(
         data = data, 
@@ -228,15 +239,19 @@
         group: x를 소그룹으로 나눌 범주형 변수명을 문자열로 지정합니다.
         kind: 막대 그래프의 종류를 'bar' 또는 'barh'로 지정합니다.(기본값: 'bar')
         pal: 팔레트를 리스트로 지정합니다.
     
     반환:
         그래프 외에 반환하는 객체는 없습니다.
     '''
-    import_library()
+    import numpy as np
+    import pandas as pd
+    from scipy import stats
+    import seaborn as sns
+    import matplotlib.pyplot as plt
     
     p = data[group].unique().size
     pv = pd.pivot_table(
         data = data, 
         index = x, 
         columns = group, 
         aggfunc = 'count'
@@ -300,15 +315,19 @@
         group: x를 소그룹으로 나눌 범주형 변수명을 문자열로 지정합니다.
         kind: 막대 그래프의 종류를 'bar' 또는 'barh'로 지정합니다.(기본값: 'bar')
         pal: 팔레트를 리스트로 지정합니다.
     
     반환:
         그래프 외에 반환하는 객체는 없습니다.
     '''
-    import_library()
+    import numpy as np
+    import pandas as pd
+    from scipy import stats
+    import seaborn as sns
+    import matplotlib.pyplot as plt
     
     p = data[group].unique().size
     pv = pd.pivot_table(
         data = data, 
         index = x, 
         columns = group, 
         aggfunc = 'count'
```

### Comparing `hds-stats-0.1.6/hds_stats/stat.py` & `hds-stats-0.2.0/hds_stats/stat.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,43 +1,21 @@
 
-# 의존성 라이브러리 호출
-def import_library():
-    import numpy as np
-    import pandas as pd
-    from scipy import stats
-    import seaborn as sns
-    import matplotlib.pyplot as plt
-    import statsmodels.api as sa
-    import statsmodels.formula.api as smf
-    from statsmodels.stats.outliers_influence import OLSInfluence
-    import statsmodels.stats.outliers_influence as oi
-    from sklearn.metrics import mean_squared_error
-    from sklearn.metrics import mean_squared_log_error
-    from sklearn.metrics import mean_absolute_error
-    from sklearn.metrics import mean_absolute_percentage_error
-    from sklearn.metrics import roc_curve, auc
-    from sklearn.metrics import PrecisionRecallDisplay
-    from sklearn.metrics import confusion_matrix
-    from sklearn.metrics import classification_report
-    from sklearn.metrics import matthews_corrcoef
-    
-
 # 다중선형 회귀모형 적합
 def ols(y, X):
     '''
     이 함수는 다중선형 회귀모형을 적합합니다.
     
     매개변수:
         y: 목표변수 벡터를 pd.Series 또는 1차원 np.ndarray로 지정합니다.
         X: 입력변수 행렬을 pd.DataFrame 또는 2차원 np.ndarray로 지정합니다.
     
     반환:
         다중선형 회귀모형을 적합한 모형을 반환합니다.
     '''
-    import_library()
+    import statsmodels.api as sa
     
     model = sa.OLS(endog = y, exog = X)
     
     return model.fit()
 
 
 # 다중선형 회귀모형 변수선택법 중 전진선택법
@@ -49,15 +27,17 @@
         y: 목표변수 벡터를 pd.Series 또는 1차원 np.ndarray로 지정합니다.
         X: 입력변수 행렬을 pd.DataFrame 또는 2차원 np.ndarray로 지정합니다.
     
     반환:
         전진선택법으로 회귀모형을 적합하고 AIC가 최소인 모형을 반환합니다.
         statsmodels.formula.api.ols 함수를 사용합니다.
     '''
-    import_library()
+    import numpy as np
+    import pandas as pd
+    import statsmodels.formula.api as smf
     
     if 'const' in X.columns:
         X = X.drop(labels = ['const'], axis = 1)
     
     Xvars = set(X.columns)
     dat = pd.concat(objs = [X, y], axis = 1)
     
@@ -98,15 +78,17 @@
         y: 목표변수 벡터를 pd.Series 또는 1차원 np.ndarray로 지정합니다.
         X: 입력변수 행렬을 pd.DataFrame 또는 2차원 np.ndarray로 지정합니다.
     
     반환:
         후진소거법으로 회귀모형을 적합하고 AIC가 최소인 모형을 반환합니다.
         statsmodels.formula.api.ols 함수를 사용합니다.
     '''
-    import_library()
+    import numpy as np
+    import pandas as pd
+    import statsmodels.formula.api as smf
     
     if 'const' in X.columns:
         X = X.drop(labels = ['const'], axis = 1)
     
     Xvars = set(X.columns)
     dat = pd.concat(objs = [X, y], axis = 1)
     
@@ -152,15 +134,17 @@
         y: 목표변수 벡터를 pd.Series 또는 1차원 np.ndarray로 지정합니다.
         X: 입력변수 행렬을 pd.DataFrame 또는 2차원 np.ndarray로 지정합니다.
     
     반환:
         단계적방법으로 회귀모형을 적합하고 AIC가 최소인 모형을 반환합니다.
         statsmodels.formula.api.ols 함수를 사용합니다.
     '''
-    import_library()
+    import numpy as np
+    import pandas as pd
+    import statsmodels.formula.api as smf
     
     if 'const' in X.columns:
         X = X.drop(labels = ['const'], axis = 1)
     
     Xvars = set(X.columns)
     dat = pd.concat(objs = [X, y], axis = 1)
     
@@ -241,15 +225,20 @@
     
     매개변수:
         model: statsmodels.formula.api.ols 함수로 적합한 선형 회귀모형을 지정합니다.
     
     반환:
         네 가지 그래프 외에 반환하는 객체는 없습니다.
     '''
-    import_library()
+    import numpy as np
+    import pandas as pd
+    import seaborn as sns
+    import matplotlib.pyplot as plt
+    from scipy import stats
+    import statsmodels.api as sm
     
     plt.figure(figsize = (10, 10), dpi = 100)
     
     # 선형성 가정
     # 잔차로 lowess(locally weighted linear regression) 회귀선을 산점도에 추가
     ax1 = plt.subplot(2, 2, 1)
     sns.regplot(
@@ -353,15 +342,15 @@
     plt.ylabel(
         ylabel = 'Sqrt of Standardized residuals', 
         fontdict = dict(size = 12)
     )
 
     # 쿡의 거리(이상치 탐지)
     ax4 = plt.subplot(2, 2, 4)
-    sa.graphics.influence_plot(
+    sm.graphics.influence_plot(
         results = model, 
         criterion = 'cooks', 
         size = 24, 
         plot_alpha = 0.2, 
         ax = ax4
     )
     
@@ -376,15 +365,15 @@
     
     매개변수:
         model: statsmodels.formula.api.ols 함수로 적합한 선형 회귀모형을 지정합니다.
     
     반환:
         훈련셋의 관측값별 쿡의 거리를 반환합니다.
     '''
-    import_library()
+    from statsmodels.stats.outliers_influence import OLSInfluence
     
     cd, _ = OLSInfluence(results = model).cooks_distance
     cd = cd.sort_values(ascending = False)
     
     return cd
 
 
@@ -395,15 +384,16 @@
     
     매개변수:
         X: 입력변수 행렬을 pd.DataFrame으로 지정합니다.
     
     반환:
         훈련셋의 햇 매트릭스를 반환합니다.
     '''
-    import_library()
+    import numpy as np
+    import pandas as pd
     
     X = np.array(object = X)
     XtX = np.matmul(X.transpose(), X)
     XtX_inv = np.linalg.inv(XtX)
     result = np.matmul(np.matmul(X, XtX_inv), X.transpose())
     
     return result
@@ -416,15 +406,16 @@
     
     매개변수:
         X: 입력변수 행렬을 pd.DataFrame으로 지정합니다.
     
     반환:
         훈련셋의 관측값별 Leverage를 반환합니다.
     '''
-    import_library()
+    import numpy as np
+    import pandas as pd
     
     n = X.shape[0]
     hatMat = hat_matrix(X = X)
     X['Leverage'] = np.array([hatMat[i][i] for i in range(n)])
     X = X.iloc[:, -1].sort_values(ascending = False)
     
     return X
@@ -437,15 +428,15 @@
     
     매개변수:
         model: statsmodels.formula.api.ols 함수로 적합한 선형 회귀모형을 지정합니다.
     
     반환:
         훈련셋의 관측값별 표준화 잔차를 반환합니다.
     '''
-    import_library()
+    from scipy import stats
     
     stdres = stats.zscore(a = model.resid)
     locs = stdres.abs().sort_values(ascending = False)
     
     return stdres[locs.index]
 
 
@@ -456,15 +447,16 @@
     
     매개변수:
         model: statsmodels.formula.api.ols 함수로 적합한 선형 회귀모형을 지정합니다.
     
     반환:
         선형 회귀모형의 영향점에 관련한 여러 지표를 데이터프레임으로 반환합니다.
     '''
-    import_library()
+    import numpy as np
+    import pandas as pd
     
     infl = model.get_influence()
     
     df1 = pd.DataFrame(
         data = {model.model.endog_names: infl.endog},
         index = model.fittedvalues.index
     )
@@ -492,17 +484,19 @@
     
     매개변수:
         model: statsmodels.formula.api.ols 함수로 적합한 선형 회귀모형을 지정합니다.
     
     반환:
         선형 회귀모형의 잔차 등분산성 검정 결과를 반환합니다.
     '''
-    import_library()
+    import numpy as np
+    import pandas as pd
+    import statsmodels.api as sm
     
-    test = sa.stats.het_breuschpagan(
+    test = sm.stats.het_breuschpagan(
         resid = model.resid, 
         exog_het = model.model.exog
     )
     
     result = pd.DataFrame(
         data = test, 
         index = ['Statistic', 'P-Value', 'F-Value', 'F P-Value']
@@ -518,15 +512,17 @@
     
     매개변수:
          X: 입력변수 행렬을 pd.DataFrame으로 지정합니다.
     
     반환:
         입력변수 행렬의 열별 분산 팽창 지수를 반환합니다.
     '''
-    import_library()
+    import numpy as np
+    import pandas as pd
+    import statsmodels.stats.outliers_influence as oi
     
     X2 = X.copy()
     if 'const' not in X2.columns:
         X2.insert(loc = 0, column = 'const', value = 1)
     
     func = oi.variance_inflation_factor
     ncol = X2.shape[1]
@@ -543,15 +539,16 @@
     
     매개변수:
         model: statsmodels.formula.api.ols 함수로 적합한 선형 회귀모형을 지정합니다.
     
     반환:
         회귀모형의 회귀계수를 반환합니다.
     '''
-    import_library()
+    import numpy as np
+    import pandas as pd
     
     if model.coef_.ndim == 1:
         coefs = pd.Series(
             data = model.coef_, 
             index = model.feature_names_in_
         )
     elif model.coef_.ndim == 2:
@@ -572,15 +569,16 @@
     
     매개변수:
         model: statsmodels.formula.api.ols 함수로 적합한 선형 회귀모형을 지정합니다.
     
     반환:
         회귀모형의 표준화 회귀계수를 반환합니다.
     '''
-    import_library()
+    import numpy as np
+    import pandas as pd
     
     model_type = str(type(model.model))
     
     X = pd.DataFrame(
         data = model.model.exog, 
         columns = model.model.exog_names
     )
@@ -603,15 +601,20 @@
         y_true: 목표변수의 실제값을 pd.Series 또는 1차원 np.ndarray로 지정합니다.
         y_pred: 목표변수의 추정값을 pd.Series 또는 1차원 np.ndarray로 지정합니다.
     
     반환:
         회귀모형의 다양한 성능 지표를 데이터프레임으로 반환합니다.
         실제값과 추정값이 음수일 때 RMSLE는 결측값으로 채웁니다.
     '''
-    import_library()
+    import numpy as np
+    import pandas as pd
+    from sklearn.metrics import mean_squared_error
+    from sklearn.metrics import mean_squared_log_error
+    from sklearn.metrics import mean_absolute_error
+    from sklearn.metrics import mean_absolute_percentage_error
     
     MSE = mean_squared_error(
         y_true = y_true, 
         y_pred = y_pred
     )
     
     RMSE = MSE**(1/2)
@@ -654,15 +657,15 @@
         y: 목표변수 벡터를 pd.Series 또는 1차원 np.ndarray로 지정합니다.
         X: 입력변수 행렬을 pd.DataFrame 또는 2차원 np.ndarray로 지정합니다.
         family: 목표변수의 확률분포를 지정합니다.
     
     반환:
         다중선형 회귀모형을 적합한 모형을 반환합니다.
     '''
-    import_library()
+    import statsmodels.api as sa
     
     model = sa.GLM(endog = y, exog = X, family = sa.families.Binomial())
     
     return model.fit()
 
 
 # 분류모형의 ROC 곡선 시각화 및 AUC 계산
@@ -680,15 +683,19 @@
         y_pred: 목표변수의 추정값을 pd.Series 또는 1차원 np.ndarray로 지정합니다.
         pos: Positive 범주를 문자열로 지정합니다.
         color: 곡선의 색을 문자열로 지정합니다.
     
     반환:
         ROC 곡선 그래프 외에 반환하는 객체는 없습니다.
     '''
-    import_library()
+    import numpy as np
+    import pandas as pd
+    import seaborn as sns
+    import matplotlib.pyplot as plt
+    from sklearn.metrics import roc_curve, auc
     
     y_class = y_true.value_counts().sort_index()
     
     if pos == None:
         pos = y_class.loc[y_class == y_class.min()].index[0]
     
     idx = np.where(y_class.index == pos)[0][0]
@@ -740,15 +747,19 @@
         y_pred: 목표변수의 추정값을 pd.Series 또는 1차원 np.ndarray로 지정합니다.
         pos: Positive 범주를 문자열로 지정합니다.
         color: 곡선의 색을 문자열로 지정합니다.
     
     반환:
         ROC 곡선 그래프 외에 반환하는 객체는 없습니다.
     '''
-    import_library()
+    import numpy as np
+    import pandas as pd
+    import seaborn as sns
+    import matplotlib.pyplot as plt
+    from sklearn.metrics import PrecisionRecallDisplay
     
     y_class = y_true.value_counts().sort_index()
     
     if pos == None:
         pos = y_class.loc[y_class == y_class.min()].index[0]
     
     idx = np.where(y_class.index == pos)[0][0]
@@ -778,15 +789,16 @@
     매개변수:
         y_true: 목표변수의 실제값을 pd.Series 또는 1차원 np.ndarray로 지정합니다.
         y_pred: 목표변수의 추정값을 pd.Series 또는 1차원 np.ndarray로 지정합니다.
     
     반환:
         분류모형의 다양한 성능 지표를 출력합니다.
     '''
-    import_library()
+    from sklearn.metrics import confusion_matrix
+    from sklearn.metrics import classification_report
     
     print('▶ Confusion Matrix')
     print(
         confusion_matrix(
             y_true = y_true, 
             y_pred = y_pred
         )
@@ -811,16 +823,20 @@
     
     매개변수:
         y_true: 목표변수의 실제값을 pd.Series 또는 1차원 np.ndarray로 지정합니다.
         y_pred: 목표변수의 추정값을 pd.Series 또는 1차원 np.ndarray로 지정합니다.
     
     반환:
         분류모형의 분리 기준점별로 TPR, FPR, MCC 등을 반환합니다.
-    '''
-    import_library()
+    '''    
+    import numpy as np
+    import pandas as pd
+    from sklearn.metrics import confusion_matrix
+    from sklearn.metrics import classification_report
+    from sklearn.metrics import matthews_corrcoef
     
     cutoffs = np.linspace(0, 1, 101)
     sens = []
     spec = []
     prec = []
     mccs = []
     
@@ -874,40 +890,39 @@
     
     매개변수:
         y_true: 목표변수의 실제값을 pd.Series 또는 1차원 np.ndarray로 지정합니다.
         y_pred: 목표변수의 추정값을 pd.Series 또는 1차원 np.ndarray로 지정합니다.
     
     반환:
          ROC 곡선 그래프 외에 반환하는 객체는 없습니다.
-    '''
-    import_library()
+    '''   
+    import seaborn as sns
+    import matplotlib.pyplot as plt
     
     obj = clfCutoffs(y_true, y_prob)
     
     # Draw ROC curve
     sns.lineplot(
         data = obj, 
         x = 'FPR', 
         y = 'TPR', 
         color = 'black'
     )
-    
     plt.title(label = '최적의 분리 기준점 탐색')
     
     # Draw diagonal line
     plt.plot(
         [0, 1], 
         [0, 1], 
         color = '0.5', 
         ls = '--'
     )
     
     # Add the Optimal Point
     opt = obj.iloc[[obj['Optimal'].argmax()]]
-    
     sns.scatterplot(
         data = opt, 
         x = 'FPR', 
         y = 'TPR', 
         color = 'red'
     )
     
@@ -925,15 +940,14 @@
     #     [y1, y2],
     #     color = 'red',
     #     lw = 0.5,
     #     ls = '-.'
     # )
     
     b = optY - optX
-    
     plt.plot(
         [0, 1-b], 
         [b, 1], 
         color = 'red', 
         lw = 0.5, 
         ls = '-.'
     )
```

### Comparing `hds-stats-0.1.6/hds_stats.egg-info/PKG-INFO` & `hds-stats-0.2.0/hds_stats.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hds-stats
-Version: 0.1.6
+Version: 0.2.0
 Summary: Useful functions for Statistics and Machine Learning
 Home-page: https://github.com/HelloDataScience/hds-stats
 Author: HelloDataScience
 Author-email: hellodatasciencekorea@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/HelloDataScience/hds-stats/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hds-stats-0.1.6/setup.py` & `hds-stats-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
+
 from setuptools import setup
 from setuptools import find_packages
 
 with open(file = 'README.md', mode = 'r', encoding = 'utf-8') as file:
     long_description = file.read()
 
 setup(
     name = 'hds-stats',
-    version = '0.1.6',
+    version = '0.2.0',
     author = 'HelloDataScience',
     author_email = 'hellodatasciencekorea@gmail.com',
     
     description = 'Useful functions for Statistics and Machine Learning',
     long_description = long_description,
     long_description_content_type = 'text/markdown',
```

