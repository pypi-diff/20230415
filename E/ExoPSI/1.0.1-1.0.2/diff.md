# Comparing `tmp/ExoPSI-1.0.1.tar.gz` & `tmp/ExoPSI-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ExoPSI-1.0.1.tar", last modified: Thu Apr 13 17:37:49 2023, max compression
+gzip compressed data, was "ExoPSI-1.0.2.tar", last modified: Sat Apr 15 18:42:54 2023, max compression
```

## Comparing `ExoPSI-1.0.1.tar` & `ExoPSI-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 17:37:49.348549 ExoPSI-1.0.1/
-drwxrwxrwx   0        0        0        0 2023-04-13 17:37:49.317146 ExoPSI-1.0.1/ExoPSI/
--rw-rw-rw-   0        0        0       28 2023-02-26 07:09:10.000000 ExoPSI-1.0.1/ExoPSI/__init__.py
--rw-rw-rw-   0        0        0     7980 2023-03-06 03:18:59.000000 ExoPSI-1.0.1/ExoPSI/exopsi.py
--rw-rw-rw-   0        0        0     1872 2023-03-21 17:45:32.000000 ExoPSI-1.0.1/ExoPSI/subfunctions.py
-drwxrwxrwx   0        0        0        0 2023-04-13 17:37:49.337540 ExoPSI-1.0.1/ExoPSI.egg-info/
--rw-rw-rw-   0        0        0     6734 2023-04-13 17:37:48.000000 ExoPSI-1.0.1/ExoPSI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      234 2023-04-13 17:37:49.000000 ExoPSI-1.0.1/ExoPSI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 17:37:48.000000 ExoPSI-1.0.1/ExoPSI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-04-13 17:37:48.000000 ExoPSI-1.0.1/ExoPSI.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-13 17:37:48.000000 ExoPSI-1.0.1/ExoPSI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35823 2023-02-25 08:19:59.000000 ExoPSI-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     6734 2023-04-13 17:37:49.337540 ExoPSI-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     5860 2023-04-13 17:19:38.000000 ExoPSI-1.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-04-13 17:37:49.348549 ExoPSI-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1417 2023-04-13 17:28:56.000000 ExoPSI-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 18:42:54.439152 ExoPSI-1.0.2/
+drwxrwxrwx   0        0        0        0 2023-04-15 18:42:54.360786 ExoPSI-1.0.2/ExoPSI/
+-rw-rw-rw-   0        0        0       28 2023-02-26 07:09:10.000000 ExoPSI-1.0.2/ExoPSI/__init__.py
+-rw-rw-rw-   0        0        0     8081 2023-04-15 18:40:59.000000 ExoPSI-1.0.2/ExoPSI/exopsi.py
+-rw-rw-rw-   0        0        0     1872 2023-04-15 18:40:14.000000 ExoPSI-1.0.2/ExoPSI/subfunctions.py
+drwxrwxrwx   0        0        0        0 2023-04-15 18:42:54.423268 ExoPSI-1.0.2/ExoPSI.egg-info/
+-rw-rw-rw-   0        0        0     6734 2023-04-15 18:42:53.000000 ExoPSI-1.0.2/ExoPSI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      234 2023-04-15 18:42:54.000000 ExoPSI-1.0.2/ExoPSI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 18:42:53.000000 ExoPSI-1.0.2/ExoPSI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-04-15 18:42:53.000000 ExoPSI-1.0.2/ExoPSI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-15 18:42:53.000000 ExoPSI-1.0.2/ExoPSI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35823 2023-02-25 08:19:59.000000 ExoPSI-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     6734 2023-04-15 18:42:54.439152 ExoPSI-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5860 2023-04-13 17:19:38.000000 ExoPSI-1.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-15 18:42:54.439152 ExoPSI-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1417 2023-04-15 18:42:07.000000 ExoPSI-1.0.2/setup.py
```

### Comparing `ExoPSI-1.0.1/ExoPSI/exopsi.py` & `ExoPSI-1.0.2/ExoPSI/exopsi.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,16 @@
     #Calculate Weight
     def calc_weight(self, ref_val, upper_lim, lower_lim, threshold=0.8):
         weight = list() 
         for i in range(0,len(ref_val)):
             weight.append(calculate_weight(ref_val[i], upper_lim[i], lower_lim[i], threshold))
 
         print(f"The calculated weight(s) is(are): {weight}")
+        return weight
+    
 
 
 
     #Calculate PSI
     def calc_psi(self, params, upper_lims=None, lower_lims=None,ref_val=None,threshold = 0.8,int_param = None,surf_param = None,p_index = pd.DataFrame()):
         colnames = list(params.columns)
     
@@ -126,14 +128,15 @@
                         annotation.set_visible(False)
                         fig.canvas.draw_idle()
 
 
         fig.canvas.mpl_connect('motion_notify_event', mouse_hover)
         plt.show()
         plt.close()
+        return plt
       
 
     #Plot 2: Planetary bodies histogram
     def psi_dist(self, df):
 
         facecolor = '#EAEAEA'
         color_bars = '#3475D0'
@@ -188,22 +191,24 @@
         # plot values on top of bars
         for idx, value in enumerate(n):
             if value > 0:
                 plt.text(x_ticks[idx], value+5, int(value),ha='center', fontsize=8, c=txt_color1)
                 
         plt.show()
         plt.close()
+        return plt
          
 
     #function to convert units of P1 wrt P2, all columns should have same units
     def unit_conv(self, data,ref_index,unit_name, p_index = pd.DataFrame()):
         unit_conv_df = pd.DataFrame() 
         for j in data.index:
             k=0 
             for i in data.columns:
                 x = float(data.loc[j,i])/ref_index[k]
+                x= round(x, 8)
                 unit_conv_colname = "{} in {}".format(i,unit_name)
                 unit_conv_df.loc[j,unit_conv_colname] = x
                 k+=1
         if p_index.empty != True:
             unit_conv_df.index = p_index        
         return unit_conv_df
```

### Comparing `ExoPSI-1.0.1/ExoPSI/subfunctions.py` & `ExoPSI-1.0.2/ExoPSI/subfunctions.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         weight = calculate_weight(ref_val, upper_lim,  lower_lim,  threshold)
   else:
     weight = calculate_weight(ref_val, upper_lim,  lower_lim,  threshold)  
     
   PSI_P = [] 
   
   for i in range(len(param)):
-    V = round(math.pow(1-abs((param.iat[i,0] - ref_val)/(ref_val + param.iat[i,0])), weight), 6)
+    V = round(math.pow(1-abs((param.iat[i,0] - ref_val)/(ref_val + param.iat[i,0])), weight), 2)
     PSI_P.append(V)
   
   return PSI_P
```

### Comparing `ExoPSI-1.0.1/ExoPSI.egg-info/PKG-INFO` & `ExoPSI-1.0.2/ExoPSI.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ExoPSI
-Version: 1.0.1
+Version: 1.0.2
 Summary: Library to calculate Planet Similarity Indexes
 Home-page: https://github.com/ExoPSI/ExoPSI
 Author: ['Aditya Rai', 'Vaibhav Garg']
 Author-email: rai.aditya01@gmail.com
 License: GNU GPL v3.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `ExoPSI-1.0.1/LICENSE` & `ExoPSI-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ExoPSI-1.0.1/PKG-INFO` & `ExoPSI-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ExoPSI
-Version: 1.0.1
+Version: 1.0.2
 Summary: Library to calculate Planet Similarity Indexes
 Home-page: https://github.com/ExoPSI/ExoPSI
 Author: ['Aditya Rai', 'Vaibhav Garg']
 Author-email: rai.aditya01@gmail.com
 License: GNU GPL v3.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `ExoPSI-1.0.1/README.md` & `ExoPSI-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `ExoPSI-1.0.1/setup.py` & `ExoPSI-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="ExoPSI",
-    version="1.0.1",
+    version="1.0.2",
     description="Library to calculate Planet Similarity Indexes",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ExoPSI/ExoPSI",
     author=["Aditya Rai","Vaibhav Garg"],
     author_email="rai.aditya01@gmail.com",
     license="GNU GPL v3.0",
```

