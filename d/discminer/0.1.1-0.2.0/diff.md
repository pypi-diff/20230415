# Comparing `tmp/discminer-0.1.1.tar.gz` & `tmp/discminer-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discminer-0.1.1.tar", last modified: Wed Apr 12 17:35:31 2023, max compression
+gzip compressed data, was "discminer-0.2.0.tar", last modified: Sat Apr 15 10:03:47 2023, max compression
```

## Comparing `discminer-0.1.1.tar` & `discminer-0.2.0.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-04-12 17:35:31.394144 discminer-0.1.1/
--rw-r--r--   0 aizquier  (8218)     5000     1074 2022-01-26 21:14:15.000000 discminer-0.1.1/LICENSE
--rw-r--r--   0 aizquier  (8218)     5000     7128 2023-04-12 17:35:31.394499 discminer-0.1.1/PKG-INFO
--rw-r--r--   0 aizquier  (8218)     5000     5343 2023-04-04 12:11:03.000000 discminer-0.1.1/README.md
-drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-04-12 17:35:31.369120 discminer-0.1.1/_mining/
--rw-r--r--   0 aizquier  (8218)     5000     4979 2023-03-19 13:26:42.000000 discminer-0.1.1/_mining/make_channels.py
--rw-r--r--   0 aizquier  (8218)     5000    10743 2023-04-03 12:56:52.000000 discminer-0.1.1/_mining/make_parfile.py
--rw-r--r--   0 aizquier  (8218)     5000     1057 2023-04-03 09:01:36.000000 discminer-0.1.1/_mining/make_single_moments.py
--rw-r--r--   0 aizquier  (8218)     5000     4239 2023-03-07 14:28:23.000000 discminer-0.1.1/_mining/plot_attributes_model.py
--rw-r--r--   0 aizquier  (8218)     5000     5101 2023-04-03 15:04:19.000000 discminer-0.1.1/_mining/plot_azimuthal_profiles.py
--rw-r--r--   0 aizquier  (8218)     5000     4562 2023-04-02 22:11:37.000000 discminer-0.1.1/_mining/plot_moment+offset.py
--rw-r--r--   0 aizquier  (8218)     5000     4511 2023-04-02 22:12:18.000000 discminer-0.1.1/_mining/plot_moment+residuals.py
--rw-r--r--   0 aizquier  (8218)     5000     7134 2023-04-12 16:20:22.000000 discminer-0.1.1/_mining/plot_peak_residuals.py
--rw-r--r--   0 aizquier  (8218)     5000    10949 2023-04-03 15:09:09.000000 discminer-0.1.1/_mining/plot_radial_profiles.py
--rw-r--r--   0 aizquier  (8218)     5000     5592 2023-04-03 12:50:09.000000 discminer-0.1.1/_mining/plot_residuals+all.py
--rw-r--r--   0 aizquier  (8218)     5000     4608 2023-04-12 16:36:38.000000 discminer-0.1.1/_mining/plot_residuals+deproj.py
--rw-r--r--   0 aizquier  (8218)     5000     8203 2023-04-02 22:04:40.000000 discminer-0.1.1/_mining/utils.py
-drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-04-12 17:35:31.381277 discminer-0.1.1/discminer/
--rw-r--r--   0 aizquier  (8218)     5000       34 2023-04-03 15:53:12.000000 discminer-0.1.1/discminer/__init__.py
--rw-r--r--   0 aizquier  (8218)     5000       22 2023-04-12 17:33:33.000000 discminer-0.1.1/discminer/_version.py
--rw-r--r--   0 aizquier  (8218)     5000     1812 2023-02-12 15:59:29.000000 discminer-0.1.1/discminer/cart.py
--rw-r--r--   0 aizquier  (8218)     5000      456 2022-11-24 22:45:25.000000 discminer-0.1.1/discminer/constants.py
--rw-r--r--   0 aizquier  (8218)     5000     8108 2023-03-26 15:14:30.000000 discminer-0.1.1/discminer/core.py
--rw-r--r--   0 aizquier  (8218)     5000    74020 2023-04-04 09:57:01.000000 discminer-0.1.1/discminer/cube.py
--rw-r--r--   0 aizquier  (8218)     5000    70761 2023-04-12 16:51:53.000000 discminer-0.1.1/discminer/disc2d.py
--rw-r--r--   0 aizquier  (8218)     5000     4146 2023-03-17 13:08:01.000000 discminer-0.1.1/discminer/grid.py
-drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-04-12 17:35:31.385849 discminer-0.1.1/discminer/icons/
--rw-r--r--   0 aizquier  (8218)     5000    19647 2021-06-29 11:43:47.000000 discminer-0.1.1/discminer/icons/button_box.png
--rw-r--r--   0 aizquier  (8218)     5000    72205 2021-06-29 11:43:47.000000 discminer-0.1.1/discminer/icons/button_cursor.jpeg
--rw-r--r--   0 aizquier  (8218)     5000    39306 2022-02-22 03:18:26.000000 discminer-0.1.1/discminer/icons/button_path.png
--rw-r--r--   0 aizquier  (8218)     5000    12142 2022-02-22 03:26:08.000000 discminer-0.1.1/discminer/icons/button_return.png
--rw-r--r--   0 aizquier  (8218)     5000   110584 2021-06-29 11:43:47.000000 discminer-0.1.1/discminer/icons/button_surface.png
--rw-r--r--   0 aizquier  (8218)     5000    11838 2021-06-29 11:43:47.000000 discminer-0.1.1/discminer/icons/button_trash.jpg
--rw-r--r--   0 aizquier  (8218)     5000      336 2021-06-29 11:43:47.000000 discminer-0.1.1/discminer/icons/logo.txt
--rw-r--r--   0 aizquier  (8218)     5000    12931 2023-04-02 20:42:03.000000 discminer-0.1.1/discminer/pick.py
--rw-r--r--   0 aizquier  (8218)     5000    25381 2023-04-12 16:18:52.000000 discminer-0.1.1/discminer/plottools.py
--rw-r--r--   0 aizquier  (8218)     5000    35149 2023-04-12 16:32:43.000000 discminer-0.1.1/discminer/rail.py
--rw-r--r--   0 aizquier  (8218)     5000   160740 2022-01-27 11:46:40.000000 discminer-0.1.1/discminer/testyapf.py
-drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-04-12 17:35:31.388276 discminer-0.1.1/discminer/tools/
--rw-r--r--   0 aizquier  (8218)     5000      569 2023-03-16 20:41:38.000000 discminer-0.1.1/discminer/tools/discminer.mplstyle
--rw-r--r--   0 aizquier  (8218)     5000    16972 2023-04-03 09:18:56.000000 discminer-0.1.1/discminer/tools/fit_kernel.py
--rw-r--r--   0 aizquier  (8218)     5000     6997 2023-04-04 09:09:51.000000 discminer-0.1.1/discminer/tools/utils.py
--rw-r--r--   0 aizquier  (8218)     5000      411 2022-11-24 22:45:39.000000 discminer-0.1.1/discminer/units.py
-drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-04-12 17:35:31.383393 discminer-0.1.1/discminer.egg-info/
--rw-r--r--   0 aizquier  (8218)     5000     7128 2023-04-12 17:35:31.000000 discminer-0.1.1/discminer.egg-info/PKG-INFO
--rw-r--r--   0 aizquier  (8218)     5000     1284 2023-04-12 17:35:31.000000 discminer-0.1.1/discminer.egg-info/SOURCES.txt
--rw-r--r--   0 aizquier  (8218)     5000        1 2023-04-12 17:35:31.000000 discminer-0.1.1/discminer.egg-info/dependency_links.txt
--rw-r--r--   0 aizquier  (8218)     5000      108 2023-04-12 17:35:31.000000 discminer-0.1.1/discminer.egg-info/requires.txt
--rw-r--r--   0 aizquier  (8218)     5000       10 2023-04-12 17:35:31.000000 discminer-0.1.1/discminer.egg-info/top_level.txt
--rw-r--r--   0 aizquier  (8218)     5000      151 2023-04-03 21:10:19.000000 discminer-0.1.1/pyproject.toml
--rw-r--r--   0 aizquier  (8218)     5000       74 2023-04-12 17:35:31.395121 discminer-0.1.1/setup.cfg
--rw-r--r--   0 aizquier  (8218)     5000     3219 2023-04-03 21:16:45.000000 discminer-0.1.1/setup.py
-drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-04-12 17:35:31.393004 discminer-0.1.1/template/
--rw-r--r--   0 aizquier  (8218)     5000     8130 2023-04-04 14:41:58.000000 discminer-0.1.1/template/README.rst
--rw-r--r--   0 aizquier  (8218)     5000     5072 2022-01-02 19:37:02.000000 discminer-0.1.1/template/download_MAPS.sh
--rw-r--r--   0 aizquier  (8218)     5000     1019 2023-04-03 09:07:58.000000 discminer-0.1.1/template/log_pars_mwc480_12co_0p2_maps_cube_256walkers_10000steps.txt
--rw-r--r--   0 aizquier  (8218)     5000      617 2023-04-03 08:37:18.000000 discminer-0.1.1/template/prepare_data.py
+drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-04-15 10:03:47.308641 discminer-0.2.0/
+-rw-r--r--   0 aizquier  (8218)     5000     1074 2022-01-26 21:14:15.000000 discminer-0.2.0/LICENSE
+-rw-r--r--   0 aizquier  (8218)     5000     7128 2023-04-15 10:03:47.308859 discminer-0.2.0/PKG-INFO
+-rw-r--r--   0 aizquier  (8218)     5000     5343 2023-04-04 12:11:03.000000 discminer-0.2.0/README.md
+drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-04-15 10:03:47.281924 discminer-0.2.0/_mining/
+-rw-r--r--   0 aizquier  (8218)     5000     4974 2023-04-15 07:21:20.000000 discminer-0.2.0/_mining/make_channels.py
+-rw-r--r--   0 aizquier  (8218)     5000    10743 2023-04-03 12:56:52.000000 discminer-0.2.0/_mining/make_parfile.py
+-rw-r--r--   0 aizquier  (8218)     5000     1057 2023-04-03 09:02:09.000000 discminer-0.2.0/_mining/make_single_moments.py
+-rw-r--r--   0 aizquier  (8218)     5000     3447 2023-04-15 07:27:55.000000 discminer-0.2.0/_mining/plot_attributes_model.py
+-rw-r--r--   0 aizquier  (8218)     5000     4007 2023-04-13 16:59:47.000000 discminer-0.2.0/_mining/plot_azimuthal_profiles.py
+-rw-r--r--   0 aizquier  (8218)     5000     4476 2023-04-13 17:30:46.000000 discminer-0.2.0/_mining/plot_moment+offset.py
+-rw-r--r--   0 aizquier  (8218)     5000     4425 2023-04-13 17:30:39.000000 discminer-0.2.0/_mining/plot_moment+residuals.py
+-rw-r--r--   0 aizquier  (8218)     5000     6146 2023-04-14 21:07:52.000000 discminer-0.2.0/_mining/plot_peak_residuals.py
+-rw-r--r--   0 aizquier  (8218)     5000    11249 2023-04-13 17:34:25.000000 discminer-0.2.0/_mining/plot_radial_profiles.py
+-rw-r--r--   0 aizquier  (8218)     5000     5628 2023-04-13 17:29:19.000000 discminer-0.2.0/_mining/plot_residuals+all.py
+-rw-r--r--   0 aizquier  (8218)     5000     4711 2023-04-13 17:41:59.000000 discminer-0.2.0/_mining/plot_residuals+deproj.py
+-rw-r--r--   0 aizquier  (8218)     5000    10412 2023-04-13 16:23:21.000000 discminer-0.2.0/_mining/utils.py
+drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-04-15 10:03:47.292228 discminer-0.2.0/discminer/
+-rw-r--r--   0 aizquier  (8218)     5000       34 2023-04-03 15:53:12.000000 discminer-0.2.0/discminer/__init__.py
+-rw-r--r--   0 aizquier  (8218)     5000       22 2023-04-15 10:00:30.000000 discminer-0.2.0/discminer/_version.py
+-rw-r--r--   0 aizquier  (8218)     5000     1812 2023-02-12 15:59:29.000000 discminer-0.2.0/discminer/cart.py
+-rw-r--r--   0 aizquier  (8218)     5000      456 2022-11-24 22:45:25.000000 discminer-0.2.0/discminer/constants.py
+-rw-r--r--   0 aizquier  (8218)     5000     8108 2023-03-26 15:14:30.000000 discminer-0.2.0/discminer/core.py
+-rw-r--r--   0 aizquier  (8218)     5000    74020 2023-04-04 09:57:01.000000 discminer-0.2.0/discminer/cube.py
+-rw-r--r--   0 aizquier  (8218)     5000    70761 2023-04-12 16:51:53.000000 discminer-0.2.0/discminer/disc2d.py
+-rw-r--r--   0 aizquier  (8218)     5000     4147 2023-04-13 13:36:17.000000 discminer-0.2.0/discminer/grid.py
+drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-04-15 10:03:47.302432 discminer-0.2.0/discminer/icons/
+-rw-r--r--   0 aizquier  (8218)     5000    19647 2021-06-29 11:43:47.000000 discminer-0.2.0/discminer/icons/button_box.png
+-rw-r--r--   0 aizquier  (8218)     5000    72205 2021-06-29 11:43:47.000000 discminer-0.2.0/discminer/icons/button_cursor.jpeg
+-rw-r--r--   0 aizquier  (8218)     5000    39306 2022-02-22 03:18:26.000000 discminer-0.2.0/discminer/icons/button_path.png
+-rw-r--r--   0 aizquier  (8218)     5000    12142 2022-02-22 03:26:08.000000 discminer-0.2.0/discminer/icons/button_return.png
+-rw-r--r--   0 aizquier  (8218)     5000   110584 2021-06-29 11:43:47.000000 discminer-0.2.0/discminer/icons/button_surface.png
+-rw-r--r--   0 aizquier  (8218)     5000    11838 2021-06-29 11:43:47.000000 discminer-0.2.0/discminer/icons/button_trash.jpg
+-rw-r--r--   0 aizquier  (8218)     5000      336 2021-06-29 11:43:47.000000 discminer-0.2.0/discminer/icons/logo.txt
+-rw-r--r--   0 aizquier  (8218)     5000    12931 2023-04-02 20:42:03.000000 discminer-0.2.0/discminer/pick.py
+-rw-r--r--   0 aizquier  (8218)     5000    28759 2023-04-14 21:15:05.000000 discminer-0.2.0/discminer/plottools.py
+-rw-r--r--   0 aizquier  (8218)     5000    35149 2023-04-12 16:32:43.000000 discminer-0.2.0/discminer/rail.py
+-rw-r--r--   0 aizquier  (8218)     5000   160740 2022-01-27 11:46:40.000000 discminer-0.2.0/discminer/testyapf.py
+drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-04-15 10:03:47.304561 discminer-0.2.0/discminer/tools/
+-rw-r--r--   0 aizquier  (8218)     5000      569 2023-03-16 20:41:38.000000 discminer-0.2.0/discminer/tools/discminer.mplstyle
+-rw-r--r--   0 aizquier  (8218)     5000    16972 2023-04-03 09:18:56.000000 discminer-0.2.0/discminer/tools/fit_kernel.py
+-rw-r--r--   0 aizquier  (8218)     5000     6997 2023-04-04 09:09:51.000000 discminer-0.2.0/discminer/tools/utils.py
+-rw-r--r--   0 aizquier  (8218)     5000      411 2022-11-24 22:45:39.000000 discminer-0.2.0/discminer/units.py
+drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-04-15 10:03:47.294554 discminer-0.2.0/discminer.egg-info/
+-rw-r--r--   0 aizquier  (8218)     5000     7128 2023-04-15 10:03:47.000000 discminer-0.2.0/discminer.egg-info/PKG-INFO
+-rw-r--r--   0 aizquier  (8218)     5000     1284 2023-04-15 10:03:47.000000 discminer-0.2.0/discminer.egg-info/SOURCES.txt
+-rw-r--r--   0 aizquier  (8218)     5000        1 2023-04-15 10:03:47.000000 discminer-0.2.0/discminer.egg-info/dependency_links.txt
+-rw-r--r--   0 aizquier  (8218)     5000      108 2023-04-15 10:03:47.000000 discminer-0.2.0/discminer.egg-info/requires.txt
+-rw-r--r--   0 aizquier  (8218)     5000       10 2023-04-15 10:03:47.000000 discminer-0.2.0/discminer.egg-info/top_level.txt
+-rw-r--r--   0 aizquier  (8218)     5000      151 2023-04-03 21:10:19.000000 discminer-0.2.0/pyproject.toml
+-rw-r--r--   0 aizquier  (8218)     5000       74 2023-04-15 10:03:47.309448 discminer-0.2.0/setup.cfg
+-rw-r--r--   0 aizquier  (8218)     5000     3219 2023-04-03 21:16:45.000000 discminer-0.2.0/setup.py
+drwxr-xr-x   0 aizquier  (8218)     5000        0 2023-04-15 10:03:47.307851 discminer-0.2.0/template/
+-rw-r--r--   0 aizquier  (8218)     5000     8550 2023-04-15 07:40:20.000000 discminer-0.2.0/template/README.rst
+-rw-r--r--   0 aizquier  (8218)     5000     5072 2022-01-02 19:37:02.000000 discminer-0.2.0/template/download_MAPS.sh
+-rw-r--r--   0 aizquier  (8218)     5000     1019 2023-04-03 09:07:58.000000 discminer-0.2.0/template/log_pars_mwc480_12co_0p2_maps_cube_256walkers_10000steps.txt
+-rw-r--r--   0 aizquier  (8218)     5000      617 2023-04-03 08:37:18.000000 discminer-0.2.0/template/prepare_data.py
```

### Comparing `discminer-0.1.1/LICENSE` & `discminer-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `discminer-0.1.1/PKG-INFO` & `discminer-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discminer
-Version: 0.1.1
+Version: 0.2.0
 Summary: Python package for parametric modelling of intensity channel maps from gas discs
 Home-page: https://github.com/andizq/discminer
 Author: Andres F. Izquierdo
 Author-email: andres.izquierdo.c@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/andizq/discminer/issues
 Project-URL: Source, https://github.com/andizq/discminer/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: discminer Version: 0.1.1 Summary: Python package
+Metadata-Version: 2.1 Name: discminer Version: 0.2.0 Summary: Python package
 for parametric modelling of intensity channel maps from gas discs Home-page:
 https://github.com/andizq/discminer Author: Andres F. Izquierdo Author-email:
 andres.izquierdo.c@gmail.com License: UNKNOWN Project-URL: Bug Reports, https:/
 /github.com/andizq/discminer/issues Project-URL: Source, https://github.com/
 andizq/discminer/ Description:
  [https://raw.githubusercontent.com/andizq/andizq.github.io/master/discminer/
                              discminer_logo.jpeg]
```

### Comparing `discminer-0.1.1/README.md` & `discminer-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `discminer-0.1.1/_mining/make_channels.py` & `discminer-0.2.0/_mining/make_channels.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,15 +100,15 @@
 
 #MODEL CHANNELS
 fig, ax, im, cbar = modelcube.make_channel_maps(channels={'indices': plot_channels}, ncols=5, levels=im[0].levels, contours_from=model)
 plt.savefig('channel_maps_model.png', bbox_inches = 'tight', dpi=200)
 plt.close()
 
 #RESIDUAL CHANNELS
-noise_mean, mask = get_noise_mask(datacube.data)
+noise_mean, mask = get_noise_mask(datacube)
 
 residualscube = Cube(datacube.data-modelcube.data, datacube.header, datacube.vchannels, dpc, beam=datacube.beam)
 residualscube.filename = 'cube_residuals_%s.fits'%tag
 residualscube.writefits() 
 
 fig, ax, im, cbar = residualscube.make_channel_maps(channels={'indices': plot_channels}, ncols=5,
                                                     kind='residuals',
```

### Comparing `discminer-0.1.1/_mining/make_parfile.py` & `discminer-0.2.0/_mining/make_parfile.py`

 * *Files identical despite different names*

### Comparing `discminer-0.1.1/_mining/make_single_moments.py` & `discminer-0.2.0/_mining/make_single_moments.py`

 * *Files identical despite different names*

### Comparing `discminer-0.1.1/_mining/plot_attributes_model.py` & `discminer-0.2.0/_mining/plot_attributes_model.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-from discminer.core import Data
-from discminer.disc2d import General2d
 from discminer.plottools import use_discminer_style, make_up_ax
-import discminer.cart as cart
+from utils import init_data_and_model, get_noise_mask
 
 import numpy as np
 import matplotlib.pyplot as plt
 from matplotlib.ticker import FormatStrFormatter
 
 from astropy import units as u
 
@@ -23,47 +21,24 @@
 custom = pars['custom']
 
 #****************
 #SOME DEFINITIONS
 #****************
 file_data = meta['file_data']
 tag = meta['tag']
-au_to_m = u.au.to('m')
 
-dpc = meta['dpc']*u.pc
 Rmax = 1.1*best['intensity']['Rout']*u.au #Max model radius, 10% larger than disc Rout
 
-#*********
-#LOAD DATA
-#*********
-datacube = Data(file_data, dpc) # Read data and convert to Cube object
-vchannels = datacube.vchannels
-
-#****************************
-#INIT MODEL AND PRESCRIPTIONS
-#****************************
-model = General2d(datacube, Rmax, Rmin=0, prototype=True)
-
-model.z_upper_func = cart.z_upper_exp_tapered
-model.z_lower_func = cart.z_lower_exp_tapered
-model.velocity_func = model.keplerian_vertical # vrot = sqrt(GM/r**3)*R
-model.line_profile = model.line_profile_bell
-
-if 'I2pwl' in meta['kind']:
-    model.intensity_func = cart.intensity_powerlaw_rbreak
-elif 'I2pwlnosurf' in meta['kind']:
-    model.intensity_func = cart.intensity_powerlaw_rbreak_nosurf    
-else:
-    model.intensity_func = cart.intensity_powerlaw_rout
+#*******************
+#LOAD DATA AND MODEL
+#*******************
+datacube, model = init_data_and_model()
 
-#**************
-#PROTOTYPE PARS
-#**************
-model.params = copy.copy(best)
-model.params['intensity']['I0'] /= meta['downsamp_factor']
+noise_mean, mask = get_noise_mask(datacube, thres=2)
+vchannels = datacube.vchannels
 model.make_model()
 
 #**************
 #MAKE PLOT
 #**************
 fig = plt.figure(figsize=(14,5))
 ax0 = fig.add_axes([0.08,0.1,0.4,0.4])
```

### Comparing `discminer-0.1.1/_mining/plot_azimuthal_profiles.py` & `discminer-0.2.0/_mining/plot_azimuthal_profiles.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,23 @@
-from discminer.core import Data
+from discminer.rail import Rail, Contours
 from discminer.plottools import (get_discminer_cmap,
                                  make_up_ax, mod_major_ticks,
                                  use_discminer_style, mod_nticks_cbars)
-from discminer.rail import Rail, Contours
-from discminer.disc2d import General2d
-import discminer.cart as cart
 
 import numpy as np
 import matplotlib.pyplot as plt
 from astropy import units as u
 from astropy.io import fits
 
 import json
 import copy
 import sys
 
 from argparse import ArgumentParser
-from utils import get_1d_plot_decorators
+from utils import init_data_and_model, get_noise_mask, get_1d_plot_decorators
 
 use_discminer_style()
 
 parser = ArgumentParser(prog='plot azimuthal contours', description='Plot azimuthal contours from a given moment map [velocity, linewidth, [peakintensity, peakint]?')
 parser.add_argument('-m', '--moment', default='velocity', type=str, choices=['velocity', 'linewidth', 'lineslope', 'peakint', 'peakintensity'], help="velocity, linewidth or peakintensity")
 parser.add_argument('-k', '--kind', default='residuals', type=str, choices=['data', 'model', 'residuals'], help="data, model or residuals")
 args = parser.parse_args()
@@ -36,79 +33,44 @@
 
 meta = pars['metadata']
 best = pars['best_fit']
 custom = pars['custom']
 
 vsys = best['velocity']['vsys']
 incl = best['orientation']['incl']
+Rout = best['intensity']['Rout']
 
 clabel, clabel_res, clim0, clim0_res, clim1, clim1_res, unit = get_1d_plot_decorators(args.moment, tag=args.kind)
 
 if args.kind=='residuals':
     clim0 = clim0_res
     clim1 = clim1_res
     clabel = clabel_res
 
 if args.moment=='velocity':
     if args.kind=='residuals':
         clabel = r'Velocity %s %s'%(args.kind, unit)
     else:
         clabel = r'Deprojected Velocity %s %s'%(args.kind, unit)        
-    
-#****************
-#SOME DEFINITIONS
-#****************
-file_data = meta['file_data']
-tag = meta['tag']
-au_to_m = u.au.to('m')
 
-dpc = meta['dpc']*u.pc
-Rout = best['intensity']['Rout']
-Rmax = 1.1*Rout*u.au #Max model radius, 10% larger than disc Rout
+#*******************
+#LOAD DATA AND MODEL
+#*******************
+datacube, model = init_data_and_model()
 
-#**********
-#LOAD DATA
-#**********
-datacube = Data(file_data, dpc) # Read data and convert to Cube object
-noise = np.std( np.append(datacube.data[:5,:,:], datacube.data[-5:,:,:], axis=0), axis=0)
-mask = np.max(datacube.data, axis=0) < 4*np.mean(noise)
+noise_mean, mask = get_noise_mask(datacube, thres=2)
 vchannels = datacube.vchannels
-
-#****************************
-#INIT MODEL AND PRESCRIPTIONS
-#****************************
-model = General2d(datacube, Rmax, Rmin=0, prototype=True)
-
-model.z_upper_func = cart.z_upper_exp_tapered
-model.z_lower_func = cart.z_lower_exp_tapered
-model.velocity_func = model.keplerian_vertical
-model.line_profile = model.line_profile_bell
-
-if 'I2pwl' in meta['kind']:
-    model.intensity_func = cart.intensity_powerlaw_rbreak
-elif 'I2pwlnosurf' in meta['kind']:
-    model.intensity_func = cart.intensity_powerlaw_rbreak_nosurf    
-else:
-    model.intensity_func = cart.intensity_powerlaw_rout
-  
-#**************
-#PROTOTYPE PARS
-#**************
-model.params = copy.copy(best)
-model.params['intensity']['I0'] /= meta['downsamp_factor']
-
-#**************************
-#MAKE MODEL (2D ATTRIBUTES)
-#**************************
-model.make_model() #Make model, just needed to load disc geometry
+model.make_model()
 
 #*************************
 #LOAD MOMENT MAPS
 moment_data = fits.getdata('%s_gaussian_data.fits'%args.moment)
 moment_model = fits.getdata('%s_gaussian_model.fits'%args.moment) 
+#moment_data = fits.getdata('%s_up_doublebell_mask_data.fits'%args.moment)
+#moment_model = fits.getdata('%s_up_doublebell_mask_model.fits'%args.moment) 
 
 #**************************
 #MASK AND COMPUTE RESIDUALS
 moment_data = np.where(mask, np.nan, moment_data)
 moment_model = np.where(mask, np.nan, moment_model)
 moment_residuals = moment_data - moment_model
 
@@ -121,15 +83,15 @@
     
 #**************************
 #MAKE PLOT
 
 beam_au = datacube.beam_size.to('au').value
 R_prof = np.arange(2*beam_au, 0.8*Rout, beam_au/4)
 
-color_bounds = np.array([0.33, 0.66, 1.0])*Rout
+color_bounds = np.array([0.5, 1.0])*Rout
 
 rail = Rail(model, map2d, R_prof)
 
 fig, ax = plt.subplots(ncols=1, nrows=1, figsize=(14,6))
 ax2 = fig.add_axes([0.85,0.6,0.3*6/14,0.3])
 
 R_ref = 100
```

### Comparing `discminer-0.1.1/_mining/plot_moment+offset.py` & `discminer-0.2.0/_mining/plot_moment+offset.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,17 +19,14 @@
 import json
 from argparse import ArgumentParser
 
 use_discminer_style()
 
 parser = ArgumentParser(prog='plot moment maps', description='Plot moment map [velocity, linewidth, [peakintensity, peakint]?')
 args = add_parser_args(parser, moment=True, kind=True, surface=True)
-
-if args.moment=='peakint':
-     args.moment = 'peakintensity'
      
 #**********************
 #JSON AND PARSER STUFF
 #**********************
 with open('parfile.json') as json_file:
     pars = json.load(json_file)
 
@@ -42,24 +39,23 @@
 ctitle, clabel, clim, cfmt, cmap_mom, cmap_res, levels_im, levels_cc, unit = get_2d_plot_decorators(args.moment)
     
 #****************
 #SOME DEFINITIONS
 #****************
 file_data = meta['file_data']
 tag = meta['tag']
-au_to_m = u.au.to('m')
 
 dpc = meta['dpc']*u.pc
 Rmax = 1.1*Rout*u.au #Max model radius, 10% larger than disc Rout
 
 #********************
 #LOAD DATA AND GRID
 #********************
 datacube = Data(file_data, dpc) # Read data and convert to Cube object
-noise_mean, mask = get_noise_mask(datacube.data)
+noise_mean, mask = get_noise_mask(datacube)
 
 #Useful definitions for plots
 with open('grid_extent.json') as json_file:
     grid = json.load(json_file)
 
 xmax = grid['xsky'] 
 xlim = 1.15*np.min([xmax, Rmax.value])
@@ -113,15 +109,15 @@
         axi.spines[side].set_linewidth(4.0)
         axi.spines[side].set_color(zoomcolor)
         axi.spines[side].set_linestyle((0, (1,1.5)))
         axi.spines[side].set_capstyle('round')
     axi.grid(color='k', ls='--')
     
 for i,axi in enumerate(ax):
-    Contours.emission_surface(axi, R, phi, extent=extent, R_lev=np.linspace(0.1, 1.0, 10)*Rout*au_to_m, which=mtags['surf'])
+    Contours.emission_surface(axi, R, phi, extent=extent, R_lev=np.linspace(0.1, 1.0, 10)*Rout*u.au.to('m'), which=mtags['surf'])
      
 patch = Rectangle([-zoomwidth]*2, 2*zoomwidth, 2*zoomwidth, edgecolor=zoomcolor, facecolor='none',
                   lw=2.0, ls=(0, (1,1.5)), capstyle='round')
 ax[0].add_artist(patch)
 
 cbar0 = plt.colorbar(im, cax=ax_cbar0, format='%.1f', **kwargs_cbar)
 cbar0.ax.tick_params(labelsize=15)
```

### Comparing `discminer-0.1.1/_mining/plot_moment+residuals.py` & `discminer-0.2.0/_mining/plot_moment+residuals.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,17 +18,14 @@
 import json
 from argparse import ArgumentParser
 
 use_discminer_style()
 
 parser = ArgumentParser(prog='plot moment maps', description='Plot moment map [velocity, linewidth, [peakintensity, peakint]?')
 args = add_parser_args(parser, moment=True, kind=True, surface=True)
-
-if args.moment=='peakint':
-     args.moment = 'peakintensity'
      
 #**********************
 #JSON AND PARSER STUFF
 #**********************
 with open('parfile.json') as json_file:
     pars = json.load(json_file)
 
@@ -41,24 +38,23 @@
 ctitle, clabel, clim, cfmt, cmap_mom, cmap_res, levels_im, levels_cc, unit = get_2d_plot_decorators(args.moment)
 
 #****************
 #SOME DEFINITIONS
 #****************
 file_data = meta['file_data']
 tag = meta['tag']
-au_to_m = u.au.to('m')
 
 dpc = meta['dpc']*u.pc
 Rmax = 1.1*Rout*u.au #Max model radius, 10% larger than disc Rout
 
 #********************
 #LOAD DATA AND GRID
 #********************
 datacube = Data(file_data, dpc) # Read data and convert to Cube object
-noise_mean, mask = get_noise_mask(datacube.data)
+noise_mean, mask = get_noise_mask(datacube)
 
 #Useful definitions for plots
 with open('grid_extent.json') as json_file:
     grid = json.load(json_file)
 
 xmax = grid['xsky'] 
 xlim = 1.15*np.min([xmax, Rmax.value])
@@ -125,13 +121,13 @@
     mod_major_ticks(axi, axis='both', nbins=8)
     datacube.plot_beam(axi, fc='lime')
     axi.set_aspect(1)
     
 for axi in ax[1:]: axi.tick_params(labelleft=False)
 
 for i,axi in enumerate(ax):
-    Contours.emission_surface(axi, R, phi, extent=extent, R_lev=np.linspace(0.1, 1.0, 10)*Rout*au_to_m, which=mtags['surf'])
+    Contours.emission_surface(axi, R, phi, extent=extent, R_lev=np.linspace(0.1, 1.0, 10)*Rout*u.au.to('m'), which=mtags['surf'])
                               
     
 plt.savefig('moment+residuals_%s.png'%mtags['base'], bbox_inches='tight', dpi=200)
 plt.show()
 plt.close()
```

### Comparing `discminer-0.1.1/_mining/plot_peak_residuals.py` & `discminer-0.2.0/_mining/plot_peak_residuals.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,35 @@
-from discminer.core import Data
 from discminer.plottools import (get_discminer_cmap, append_sigma_panel,
                                  make_up_ax, mod_minor_ticks, mod_major_ticks,
                                  use_discminer_style, mod_nticks_cbars,
                                  make_substructures, make_round_map)
-from discminer.disc2d import General2d
-import discminer.cart as cart
 from discminer.pick import Pick
 from discminer.rail import Contours
 
 import numpy as np
 import matplotlib.pyplot as plt
 
 from astropy import units as u
 import json
 import copy
 
-from utils import add_parser_args, get_2d_plot_decorators, load_moments
+from utils import (init_data_and_model,
+                   get_noise_mask,
+                   add_parser_args,
+                   get_2d_plot_decorators,
+                   load_moments)
+
 from argparse import ArgumentParser
 
 use_discminer_style()
 
 parser = ArgumentParser(prog='Identify and show peak residuals', description='Identify peak residuals in folded maps.')
 parser.add_argument('-c', '--clean_thres', default=np.inf, type=float, help="Threshold above which peak residuals will be rejected.")
 args = add_parser_args(parser, moment=True, kind=True, surface=True, fold=True, projection=True, Rinner=True, Router=True)
 
-if args.moment=='peakint':
-     args.moment = 'peakintensity'
-
 #**********************
 #JSON AND PARSER STUFF
 #**********************
 with open('parfile.json') as json_file:
     pars = json.load(json_file)
 
 meta = pars['metadata']
@@ -55,48 +54,21 @@
 file_data = meta['file_data']
 tag = meta['tag']
 au_to_m = u.au.to('m')
 
 dpc = meta['dpc']*u.pc
 Rmax = 1.1*Rout*u.au #Max model radius, 10% larger than disc Rout
 
-#********
-#LOAD DATA
-#********
-datacube = Data(file_data, dpc) # Read data and convert to Cube object
-noise = np.std( np.append(datacube.data[:5,:,:], datacube.data[-5:,:,:], axis=0), axis=0)
-mask = np.max(datacube.data, axis=0) < 4*np.mean(noise)
-vchannels = datacube.vchannels
-
-#****************************
-#INIT MODEL AND PRESCRIPTIONS
-#****************************
-model = General2d(datacube, Rmax, Rmin=0, prototype=True)
-
-model.z_upper_func = cart.z_upper_exp_tapered
-model.z_lower_func = cart.z_lower_exp_tapered
-model.velocity_func = model.keplerian_vertical # vrot = sqrt(GM/r**3)*R
-model.line_profile = model.line_profile_bell
-
-if 'I2pwl' in meta['kind']:
-    model.intensity_func = cart.intensity_powerlaw_rbreak
-elif 'I2pwlnosurf' in meta['kind']:
-    model.intensity_func = cart.intensity_powerlaw_rbreak_nosurf    
-else:
-    model.intensity_func = cart.intensity_powerlaw_rout
-
-#**************
-#PROTOTYPE PARS
-#**************
-model.params = copy.copy(best)
-model.params['intensity']['I0'] /= meta['downsamp_factor']
+#*******************
+#LOAD DATA AND MODEL
+#*******************
+datacube, model = init_data_and_model()
 
-#**************************
-#MAKE MODEL (2D ATTRIBUTES)
-#**************************
+noise_mean, mask = get_noise_mask(datacube, thres=2)
+vchannels = datacube.vchannels
 model.make_model()
 
 #*************************
 #LOAD MOMENT MAPS
 moment_data, moment_model, mtags = load_moments(args)
 
 #**************************
@@ -173,19 +145,19 @@
 cos_peak = np.cos(np.radians(peak_angle))
 sin_peak = np.sin(np.radians(peak_angle))
 
 if args.projection=='cartesian':
     levels_resid = np.linspace(-clim, clim, 32)
     
     if args.surface in ['up', 'upper']:
-        z_func = cart.z_upper_exp_tapered
+        z_func = model.z_upper_func
         z_pars = best['height_upper']
 
     elif args.surface in ['low', 'lower']:
-        z_func = cart.z_lower_exp_tapered
+        z_func = model.z_lower_func
         z_pars = best['height_lower']
     
     fig, ax = make_round_map(folded_map, levels_resid, pick.X*u.au, pick.Y*u.au, R_prof[-1]*u.au,
                              z_func=z_func, z_pars=z_pars, incl=incl, PA=PA, xc=xc, yc=yc,
                              cmap=cmap_res, clabel=unit, fmt=cfmt, 
                              rings=rings,
                              mask_wedge=(90, 270)*u.deg,
```

### Comparing `discminer-0.1.1/_mining/plot_radial_profiles.py` & `discminer-0.2.0/_mining/plot_radial_profiles.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,122 +1,98 @@
-from discminer.core import Data
-from discminer.plottools import (get_discminer_cmap,
+from discminer.plottools import (get_discminer_cmap, make_substructures,
                                  make_up_ax, mod_minor_ticks, mod_major_ticks,
                                  use_discminer_style, mod_nticks_cbars)
 from discminer.rail import Rail, Contours
-from discminer.disc2d import General2d
-import discminer.cart as cart
 
 import numpy as np
 import matplotlib.pyplot as plt
 from scipy.signal import savgol_filter
+from scipy.interpolate import interp1d
 
 from astropy import units as u
 from astropy.io import fits
 import json
 import copy
 
-from utils import get_1d_plot_decorators, load_moments, add_parser_args
+from utils import (init_data_and_model,
+                   get_noise_mask,
+                   get_1d_plot_decorators,
+                   load_moments,
+                   load_disc_grid,
+                   add_parser_args,
+                   make_1d_legend,
+                   MEDIUM_SIZE)
+
 from argparse import ArgumentParser
 
 use_discminer_style()
 
 parser = ArgumentParser(prog='plot radial profiles', description='Plot radial profiles from moments and residuals [velocity, linewidth, [peakintensity, peakint]?')
-args = add_parser_args(parser, moment=True, kind=True, surface=True, writetxt=True, mask_ang=True)
-
-if args.moment=='peakint':
-     args.moment = 'peakintensity'
+args = add_parser_args(parser, moment=True, kind=True, surface=True, writetxt=True, mask_minor=True, mask_major=True, Rinner=True, Router=True)
 
 #**********************
 #JSON AND PARSER STUFF
 #**********************
 with open('parfile.json') as json_file:
     pars = json.load(json_file)
 
 meta = pars['metadata']
 best = pars['best_fit']
 custom = pars['custom']
 
 Mstar = best['velocity']['Mstar']
 vsys = best['velocity']['vsys']
 vel_sign = best['velocity']['vel_sign']
+Rout = best['intensity']['Rout']
 incl = best['orientation']['incl']
 
 gaps = custom['gaps']
 rings = custom['rings']
-kinks = custom['kinks']
+Rmax = 1.1*Rout*u.au #Max model radius, 10% larger than disc Rout
 
 clabel, clabel_res, clim0, clim0_res, clim1, clim1_res, unit = get_1d_plot_decorators(args.moment)
 
-#****************
-#SOME DEFINITIONS
-#****************
-file_data = meta['file_data']
-tag = meta['tag']
-au_to_m = u.au.to('m')
-
-dpc = meta['dpc']*u.pc
-Rmax = 1.1*best['intensity']['Rout']*u.au #Max model radius, 10% larger than disc Rout
-
-#********
-#LOAD DATA
-#********
-datacube = Data(file_data, dpc) # Read data and convert to Cube object
-noise = np.std( np.append(datacube.data[:5,:,:], datacube.data[-5:,:,:], axis=0), axis=0)
-mask = np.max(datacube.data, axis=0) < 4*np.mean(noise)
-vchannels = datacube.vchannels
+#*******************
+#LOAD DATA AND MODEL
+#*******************
+datacube, model = init_data_and_model()
 
-#****************************
-#INIT MODEL AND PRESCRIPTIONS
-#****************************
-model = General2d(datacube, Rmax, Rmin=0, prototype=True)
-
-model.z_upper_func = cart.z_upper_exp_tapered
-model.z_lower_func = cart.z_lower_exp_tapered
-model.velocity_func = model.keplerian_vertical # vrot = sqrt(GM/r**3)*R
-model.line_profile = model.line_profile_bell
-
-if 'I2pwl' in meta['kind']:
-    model.intensity_func = cart.intensity_powerlaw_rbreak
-elif 'I2pwlnosurf' in meta['kind']:
-    model.intensity_func = cart.intensity_powerlaw_rbreak_nosurf    
-else:
-    model.intensity_func = cart.intensity_powerlaw_rout
+noise_mean, mask = get_noise_mask(datacube, thres=2)
+vchannels = datacube.vchannels
+model.make_model()
 
-#**************
-#PROTOTYPE PARS
-#**************
-model.params = copy.copy(best)
-model.params['intensity']['I0'] /= meta['downsamp_factor']
+#*************************
+#LOAD DISC GEOMETRY
+R, phi, z = load_disc_grid()
 
-#**************************
-#MAKE MODEL (2D ATTRIBUTES)
-#**************************
-model.make_model()
+R_s = R[args.surface]*u.m.to('au')
+phi_s = phi[args.surface]
 
 #*************************
 #LOAD MOMENT MAPS
 moment_data, moment_model, mtags = load_moments(args)
 if mtags['surf']=='both':
     surf_ref = 'upper'
+else:
+    surf_ref = args.surface
 tag_base = mtags['base']
 
 #**************************
 #MASK AND COMPUTE RESIDUALS
 moment_data = np.where(mask, np.nan, moment_data)
 moment_model = np.where(mask, np.nan, moment_model)
 moment_residuals = moment_data - moment_model
     
 if args.moment=='velocity':
     moment_residuals_abs = np.abs(moment_data-vsys) - np.abs(moment_model-vsys)
 
 #**************************
 #MAKE PLOTS
 beam_au = datacube.beam_size.to('au').value
-R_prof = np.arange(1*beam_au, 0.9*best['intensity']['Rout'], beam_au/4)
+R_prof = np.arange(args.Rinner*beam_au, args.Router*Rout, beam_au/5)
 xlim0, xlim1 = 0.5*R_prof[0], 1.05*R_prof[-1]
 
 def writetxt(arr, tag=''):
     if tag!='': tag = '_'+tag
     arr = np.asarray(arr).T
     np.savetxt('radial_profile_%s%s.dat'%(args.moment, tag), arr, fmt='%.6f', header='R[au] attribute stddev')
 
@@ -140,102 +116,126 @@
     except np.linalg.LinAlgError:
         ysav = prof
         ysav_deriv = None
     return ysav, ysav_deriv 
 
 
 if args.moment=='velocity':
-    mask_ang = args.mask_ang #+-mask around disc minor axis
+    mask_ang = args.mask_minor #+-mask around disc minor axis
     #*******************
     #VELOCITY COMPONENTS
     #*******************    
+
+    #VZ
     rail_vz = Rail(model, moment_residuals, R_prof)
     vel_z, vel_z_error = rail_vz.get_average(mask_ang=mask_ang, surface=surf_ref)
     div_factor_z = get_normalisation(mask_ang, component='z')
 
     vel_z /= div_factor_z
     vel_z_error /= div_factor_z 
-    
+
+    #DVPHI
     rail_phi = Rail(model, moment_residuals_abs, R_prof)
     vel_phi, vel_phi_error = rail_phi.get_average(mask_ang=mask_ang, surface=surf_ref)
     div_factor_phi = get_normalisation(mask_ang, component='phi')
 
     vel_phi /= div_factor_phi
     vel_phi_error /= div_factor_phi 
 
-    fig, ax = plt.subplots(ncols=1, nrows=1, figsize=(14,4))
-    ysav_z, ysav_z_deriv = make_savgol(vel_z)
-        
-    ax.plot(R_prof, ysav_z, c='k', lw=3, label=r'$z$-component', zorder=12)
-    ax.fill_between(R_prof, vel_z+vel_z_error, vel_z-vel_z_error, color='k', alpha=0.15, zorder=9)
+    #VPHI
+    rail_phi = Rail(model, np.abs(moment_data-vsys), R_prof)
+    vel_rot, _ = rail_phi.get_average(mask_ang=mask_ang, surface=surf_ref)
+    vel_rot /= div_factor_phi
+    vel_rot_error = vel_phi_error
+
+    #VR
+    mask_r = mask | (np.abs(phi_s) < np.radians(args.mask_major)) | (np.abs(phi_s) > np.radians(180-args.mask_major))
+    moment_data_r = np.where(mask_r, np.nan, moment_data) 
 
+    f_vp = interp1d(R_prof, vel_rot)
+    f_vz = interp1d(R_prof, vel_z)
+    R_interp = np.where((R_s>R_prof[0]) & (R_s<R_prof[-1]), R_s, R_prof[0])
+
+    vr = -1/(np.sin(phi_s)*np.sin(incl)) * (moment_data_r - vsys - vel_sign*f_vp(R_interp)*np.cos(phi_s)*np.sin(incl) + f_vz(R_interp)*np.cos(incl))
+
+    rail_vr = Rail(model, vr, R_prof)
+    vel_r, vel_r_error = rail_vr.get_average(mask_ang=0.0, surface=surf_ref, av_func=np.nanmedian)
+
+    #WRITE?
     if args.writetxt: writetxt([R_prof, vel_z, vel_z_error], tag='vz')
+    if args.writetxt: writetxt([R_prof, vel_r, vel_r_error], tag='vr')
     if args.writetxt: writetxt([R_prof, vel_phi, vel_phi_error], tag='vphi')
+    if args.writetxt: writetxt([R_prof, vel_rot, vel_phi_error], tag='rotationcurve')
     
+    #PLOT 3D VELOCITIES
+    fig, ax = plt.subplots(ncols=1, nrows=1, figsize=(14,4))
+        
     ysav_phi, ysav_phi_deriv = make_savgol(vel_phi)
-    ax.plot(R_prof, ysav_phi, c='dodgerblue', lw=3, label=r'$\phi$-component', zorder=12)
+    ax.plot(R_prof, ysav_phi, c='dodgerblue', lw=3, label=r'$\Delta\upsilon_\phi$', zorder=12)
     ax.fill_between(R_prof, vel_phi+vel_phi_error, vel_phi-vel_phi_error, color='dodgerblue', alpha=0.15, zorder=9)
 
+    ysav_z, ysav_z_deriv = make_savgol(vel_z)    
+    ax.plot(R_prof, ysav_z, c='k', lw=3, label=r'$\upsilon_{\rm z}$', zorder=8)
+    ax.fill_between(R_prof, vel_z+vel_z_error, vel_z-vel_z_error, color='k', alpha=0.15, zorder=8)
+        
+    ysav_r, ysav_r_deriv = make_savgol(vel_r)
+    ax.plot(R_prof, ysav_r, c='#FFB000', lw=3, label=r'$\upsilon_{\rm R}$', zorder=7)
+    ax.fill_between(R_prof, vel_r+vel_r_error, vel_r-vel_r_error, color='#FFB000', alpha=0.15, zorder=7)
+
     ax.axhline(0, lw=2, ls='--', color='0.7')
     
     ax.set_xlabel('Radius [au]')
     ax.set_xlim(xlim0, xlim1)
     ax.set_ylabel(r'$\delta\upsilon$ [km/s]')
     ax.set_ylim(clim0_res, clim1_res)
     mod_major_ticks(ax, axis='x', nbins=10)
     mod_minor_ticks(ax)
-    ax.legend(frameon=False, fontsize=12)
-
-    Contours.make_substructures(ax, gaps=gaps, rings=rings, kinks=kinks)
+    make_1d_legend(ax, fontsize=MEDIUM_SIZE+1)
+    
+    make_substructures(ax, gaps=gaps, rings=rings, label_gaps=True, label_rings=True)
     
     plt.savefig('velocity_components_%s.png'%tag_base, bbox_inches='tight', dpi=200)
     plt.show()
 
     #*******************
     #ROTATION CURVE
     #*******************
-    fig, ax = plt.subplots(ncols=1, nrows=1, figsize=(14,4))
-    
-    #DATA CURVE
-    rail_phi = Rail(model, np.abs(moment_data-vsys), R_prof)
-    vel_rot, _ = rail_phi.get_average(mask_ang=mask_ang, surface=surf_ref)
-    vel_rot /= div_factor_phi
+    fig, ax = plt.subplots(ncols=1, nrows=1, figsize=(14,4))        
 
+    #DATA CURVE
     ysav_rot, ysav_rot_deriv = make_savgol(vel_rot)
-    ax.plot(R_prof, ysav_rot, c='tomato', lw=3.5, label=r'Data curve', zorder=12)
-    ax.fill_between(R_prof, vel_rot+vel_phi_error, vel_rot-vel_phi_error, color='tomato', alpha=0.15, zorder=9)
-
-    if args.writetxt: writetxt([R_prof, vel_rot, vel_phi_error], tag='rotationcurve')    
-
+    ax.plot(R_prof, ysav_rot, c='tomato', lw=3.5, label=r'Data', zorder=12)
+    ax.fill_between(R_prof, vel_rot+vel_rot_error, vel_rot-vel_rot_error, color='tomato', alpha=0.15, zorder=9)
+    
     #r"""
     #MODEL CURVE
     rail_phi = Rail(model, np.abs(moment_model-vsys), R_prof)
     vel_phi, _ = rail_phi.get_average(mask_ang=mask_ang, surface=surf_ref)
     vel_phi /= div_factor_phi
     ysav_phi, ysav_phi_deriv = make_savgol(vel_phi)
-    ax.plot(R_prof, ysav_phi, c='0.7', lw=4.0, label=r'Model curve', zorder=11)
+    ax.plot(R_prof, ysav_phi, c='0.7', lw=4.0, label=r'Model', zorder=11)
     #"""
     
     #PERFECT KEPLERIAN
-    coords = {'R': R_prof*au_to_m}
+    coords = {'R': R_prof*u.au.to('m')}
     velocity_upper = model.get_attribute_map(coords, 'velocity', surface=surf_ref) * vel_sign
     ax.plot(R_prof, velocity_upper, c='k', lw=2.5, ls='--', label=r'Keplerian (%.2f Msun)'%Mstar, zorder=13)
 
     #DECORATIONS
     ax.axhline(0, lw=2, ls='--', color='0.7')
 
     ax.set_xlabel('Radius [au]')
     ax.set_xlim(xlim0, xlim1)    
     ax.set_ylabel(r'Rotation velocity [km/s]')
     ax.set_ylim(clim0, 1.2*np.nanmax(vel_phi))
     mod_major_ticks(ax, axis='x', nbins=10)
     mod_minor_ticks(ax)    
-    ax.legend(frameon=False, fontsize=12)
+    make_1d_legend(ax)
 
-    Contours.make_substructures(ax, gaps=gaps, rings=rings, kinks=kinks)
+    make_substructures(ax, gaps=gaps, rings=rings, label_gaps=True, label_rings=True)  
     
     plt.savefig('rotation_curve_%s.png'%tag_base, bbox_inches='tight', dpi=200)
     plt.show()
 
     """
     #Data rotation curve - perfect_Keplerian
     fig, ax = plt.subplots(ncols=1, nrows=1, figsize=(14,4)) 
@@ -253,40 +253,40 @@
     fig, ax = plt.subplots(ncols=1, nrows=1, figsize=(14,4))
 
     #DATA CURVE
     rail_phi = Rail(model, moment_data, R_prof)
     vel_phi, vel_phi_error = rail_phi.get_average(**kw_avg)
 
     ysav_phi, ysav_phi_deriv = make_savgol(vel_phi)    
-    ax.plot(R_prof, ysav_phi, c='tomato', lw=4.0, label=r'Data curve', zorder=12)
+    ax.plot(R_prof, ysav_phi, c='tomato', lw=4.0, label=r'Data', zorder=12)
     ax.fill_between(R_prof, vel_phi+vel_phi_error, vel_phi-vel_phi_error, color='tomato', alpha=0.15, zorder=9)
 
     if args.writetxt: writetxt([R_prof, vel_phi, vel_phi_error], tag='data')
 
     #MODEL CURVE
     rail_phi = Rail(model, moment_model, R_prof)
     vel_phi, vel_phi_error = rail_phi.get_average(**kw_avg)
 
     ysav_phi, ysav_phi_deriv = make_savgol(vel_phi)    
-    ax.plot(R_prof, ysav_phi, c='dodgerblue', lw=3.5, label=r'Model curve', zorder=11)
+    ax.plot(R_prof, ysav_phi, c='dodgerblue', lw=3.5, label=r'Model', zorder=11)
 
     if args.writetxt: writetxt([R_prof, vel_phi, vel_phi_error], tag='model')
     
     #DECORATIONS
     ax.axhline(0, lw=2, ls='--', color='0.7')
 
     ax.set_xlabel('Radius [au]')
     ax.set_xlim(xlim0, xlim1)    
     ax.set_ylabel(clabel)
     ax.set_ylim(clim0, clim1)
     mod_major_ticks(ax, axis='x', nbins=10)
     mod_minor_ticks(ax)
-    ax.legend(frameon=False, fontsize=12)
+    make_1d_legend(ax)
 
-    Contours.make_substructures(ax, gaps=gaps, rings=rings, kinks=kinks)
+    make_substructures(ax, gaps=gaps, rings=rings, label_gaps=True, label_rings=True)  
     
     plt.savefig('radial_profile_%s.png'%tag_base, bbox_inches='tight', dpi=200)
     plt.show()
 
     #****************
     #RESIDUALS
     #****************    
@@ -307,13 +307,13 @@
     ax.set_xlabel('Radius [au]')
     ax.set_xlim(xlim0, xlim1)    
     ax.set_ylabel(clabel_res)
     ax.set_ylim(clim0_res, clim1_res)
     mod_major_ticks(ax, axis='x', nbins=10)
     mod_minor_ticks(ax)
 
-    Contours.make_substructures(ax, gaps=gaps, rings=rings, kinks=kinks)
+    make_substructures(ax, gaps=gaps, rings=rings, label_gaps=True, label_rings=True)
         
     plt.savefig('radial_profile_residuals_%s.png'%tag_base, bbox_inches='tight', dpi=200)
     plt.show()
```

### Comparing `discminer-0.1.1/_mining/plot_residuals+all.py` & `discminer-0.2.0/_mining/plot_residuals+all.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from discminer.core import Data
 from discminer.rail import Contours
 from discminer.plottools import (add_cbar_ax,
+                                 make_substructures,
+                                 _make_radial_grid_2D,
                                  make_up_ax,
                                  mod_minor_ticks,
                                  mod_major_ticks,
                                  use_discminer_style)
 
 from utils import (get_2d_plot_decorators,
                    get_noise_mask,
@@ -40,15 +42,14 @@
 incl = best['orientation']['incl']
 PA = best['orientation']['PA']
 xc = best['orientation']['xc']
 yc = best['orientation']['yc']
 
 gaps = custom['gaps']
 rings = custom['rings']
-kinks = custom['kinks']
 
 #****************
 #SOME DEFINITIONS
 #****************
 file_data = meta['file_data']
 tag = meta['tag']
 au_to_m = u.au.to('m')
@@ -56,15 +57,15 @@
 dpc = meta['dpc']*u.pc
 Rmax = 1.1*Rout*u.au
 
 #********************
 #LOAD DATA AND GRID
 #********************
 datacube = Data(file_data, dpc) # Read data and convert to Cube object
-noise_mean, mask = get_noise_mask(datacube.data)
+noise_mean, mask = get_noise_mask(datacube)
 
 #Useful definitions for plots
 with open('grid_extent.json') as json_file:
     grid = json.load(json_file)
 
 xmax = grid['xsky'] 
 xlim = 1.15*np.min([xmax, Rmax.value]) 
@@ -144,16 +145,16 @@
         Contours.disc_axes(axi,
                            R[args.surface][nh]/au_to_m,
                            z[args.surface][nh]/au_to_m,
                            incl, PA, xc=xc, yc=yc)
         
     elif args.coords=='disc':
         im = axi.contourf(Xproj, Yproj, clip_prop_radially(residuals[moment], Rmax=Rout), **kwargs_im)                         
-        Contours.make_substructures(axi, gaps=gaps, rings=rings, kinks=kinks, twodim=True)
-        axi.plot(Rout*np.cos(fill_angs_2pi), Rout*np.sin(fill_angs_2pi), color='k', ls='-', lw=3.5, alpha=0.9) #Rout
+        make_substructures(axi, gaps=gaps, rings=rings, twodim=True)
+        _make_radial_grid_2D(axi, Rout, gaps=gaps, rings=rings, make_labels=True, label_freq=2)
         
     cbar = plt.colorbar(im, cax=cbar_axes[i], **kwargs_cbar)
     cbar.set_label(clabels[moment], fontsize=14)
 
     decorate_ax_res_2D(axi, cbar)
     datacube.plot_beam(axi, fc='lime')
```

### Comparing `discminer-0.1.1/_mining/plot_residuals+deproj.py` & `discminer-0.2.0/_mining/plot_residuals+deproj.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from discminer.core import Data
 from discminer.rail import Contours
 import discminer.cart as cart
 from discminer.plottools import (make_round_map,
                                  make_polar_map,
+                                 make_substructures,
                                  make_up_ax,
                                  mod_major_ticks,
                                  mod_nticks_cbars,
                                  use_discminer_style)
 
 from utils import (get_2d_plot_decorators,
                    get_noise_mask,
@@ -22,17 +23,14 @@
 from argparse import ArgumentParser
 
 use_discminer_style()
 
 parser = ArgumentParser(prog='plot residual maps', description='Plot residual maps')
 args = add_parser_args(parser, moment=True, kind=True, surface=True, projection=True)
 
-if args.moment=='peakint':
-    args.moment = 'peakintensity'
-     
 #**********************
 #JSON AND PARSER STUFF
 #**********************
 with open('parfile.json') as json_file:
     pars = json.load(json_file)
 
 meta = pars['metadata']
@@ -44,15 +42,14 @@
 incl = best['orientation']['incl']
 PA = best['orientation']['PA']
 xc = best['orientation']['xc']
 yc = best['orientation']['yc']
 
 gaps = custom['gaps']
 rings = custom['rings']
-kinks = custom['kinks']
 
 ctitle, clabel, clim, cfmt, cmap_mom, cmap_res, levels_im, levels_cc, unit = get_2d_plot_decorators(args.moment, unit_simple=True, fmt_vertical=True)
 
 #****************
 #SOME DEFINITIONS
 #****************
 file_data = meta['file_data']
@@ -62,15 +59,15 @@
 dpc = meta['dpc']*u.pc
 Rmax = 1.1*Rout*u.au #Max model radius, 10% larger than disc Rout
 
 #********************
 #LOAD DATA AND GRID
 #********************
 datacube = Data(file_data, dpc) # Read data and convert to Cube object
-noise_mean, mask = get_noise_mask(datacube.data, thres=2)
+noise_mean, mask = get_noise_mask(datacube, thres=2)
 
 #Useful definitions for plots
 with open('grid_extent.json') as json_file:
     grid = json.load(json_file)
 
 xmax = grid['xsky'] 
 xlim = 1.15*np.min([xmax, Rmax.value])
@@ -122,23 +119,25 @@
     elif args.surface in ['low', 'lower']:
         z_func = cart.z_lower_exp_tapered
         z_pars = best['height_lower']
     
     fig, ax = make_round_map(residuals, levels_resid, Xproj*u.m, Yproj*u.m, Rout*u.au,
                              z_func=z_func, z_pars=z_pars, incl=incl, PA=PA, xc=xc, yc=yc,
                              cmap=cmap_res, clabel=unit, fmt=cfmt, 
-                             rings=rings, kinks=kinks)
-
+                             gaps=gaps, rings=rings)
+    
+    make_substructures(ax, gaps=gaps, rings=rings, twodim=True, label_rings=True)
 
 elif args.projection=='polar':
     levels_resid = np.linspace(-clim, clim, 48)    
     fig, ax, cbar = make_polar_map(residuals, levels_resid,
                                    R[args.surface]*u.m, phi[args.surface]*u.rad, Rout*u.au,
                                    Rin = datacube.beam_size,
-                                   cmap=cmap_res, fmt=cfmt, clabel=clabels[args.moment],
-                                   gaps=gaps, rings=rings, kinks=kinks)
-
+                                   cmap=cmap_res, fmt=cfmt, clabel=clabels[args.moment])
+                                   
+    make_substructures(ax, gaps=gaps, rings=rings, twodim=True, polar=True, label_rings=True)
+    
 ax.set_title(ctitle, fontsize=16, color='k')
 
 plt.savefig('residuals_deproj_%s_%s.png'%(mtags['base'], args.projection), bbox_inches='tight', dpi=200)
 plt.show()
 plt.close()
```

### Comparing `discminer-0.1.1/_mining/utils.py` & `discminer-0.2.0/_mining/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,54 +1,121 @@
 """
 Useful repeating code
 """
 import json
 import decimal
-import numpy as np
-from astropy.io import fits
 import warnings
+import copy
 
 from discminer.plottools import get_discminer_cmap
+from discminer.core import Data
+from discminer.disc2d import Model
+import discminer.cart as cart
+
+from astropy.io import fits
+import astropy.units as u
+
+import numpy as np
 
 molplot = {
     '12co': r'$^{\rm 12}$CO',
     '13co': r'$^{\rm 13}$CO',
     'cs': r'CS'
 }
 
 warnings.filterwarnings("ignore", category=UserWarning)
 warnings.filterwarnings("ignore", category=RuntimeWarning)
 
+SMALL_SIZE = 10
+MEDIUM_SIZE = 15
+
+    
 def add_parser_args(parser,
                     moment=False, kind=False, surface=False, projection=False,
-                    mask_ang=False, Rinner=False, Router=False,
+                    mask_minor=False, mask_major=False, Rinner=False, Router=False,
                     fold=False, writetxt=False, 
 ):
 
     if moment:
         parser.add_argument('-m', '--moment', default='velocity', type=str, choices=['velocity', 'linewidth', 'lineslope', 'peakint', 'peakintensity'], help="velocity, linewidth or peakintensity")
-    if mask_ang:
-        parser.add_argument('-a', '--mask_ang', default=60.0, type=float, help="+- azimuthal mask around disc minor axis for computation of velocity components")
+
+    if mask_minor:
+        parser.add_argument('-b', '--mask_minor', default=60.0, type=float, help="+- azimuthal mask around disc minor axis for computation of vphi and vz velocity components")
+    if mask_major:
+        parser.add_argument('-a', '--mask_major', default=30.0, type=float, help="+- azimuthal mask around disc major axis for computation of vR velocity component")
     if kind:
         parser.add_argument('-k', '--kind', default='gaussian', type=str, choices=['gauss', 'gaussian', 'bell', 'dgauss', 'doublegaussian', 'dbell', 'doublebell'], help="gauss(or gaussian), dbell(or doublebell)")
     if surface:
         parser.add_argument('-s', '--surface', default='upper', type=str, choices=['up', 'upper', 'low', 'lower'], help="upper or lower surface moment map")
     if fold:
         parser.add_argument('-f', '--fold', default='absolute', type=str, choices=['absolute', 'standard'], help="if moment=velocity, fold absolute or standard velocity residuals")
     if projection:
         parser.add_argument('-p', '--projection', default='cartesian', type=str, choices=['cartesian', 'polar'], help="Project residuals onto a cartesian or a polar map")
     if writetxt:
         parser.add_argument('-w', '--writetxt', default=False, type=bool, help="write txt files")
     if Rinner:
         parser.add_argument('-i', '--Rinner', default=1.0, type=float, help="Number of beams to mask out from inner region")
     if Router:
         parser.add_argument('-o', '--Router', default=0.9, type=float, help="Fraction of Rout to consider as the outer radius for the analysis")
+
+    args = parser.parse_args()
+
+    try:
+        if args.moment=='peakint':
+            args.moment = 'peakintensity'
+    except AttributeError:
+        pass
+
+    return args
+
+
+def init_data_and_model(parfile='parfile.json', Rmin=0, Rmax=1.1, init_model=True):
+    #Rmin: If dimensionless, fraction of beam_size
+    #Rmax: If dimensionless, fraction of Rout    
+    with open(parfile) as jf:
+        pars = json.load(jf)
+
+    meta = pars['metadata']
+    best = pars['best_fit']
+    custom = pars['custom']
+
+    file_data = meta['file_data']
+    Rout = best['intensity']['Rout']
+    dpc = meta['dpc']*u.pc
+
+    datacube = Data(file_data, dpc) # Read data and convert to Cube object
+
+    if init_model:
+        Rmax = Rmax*Rout*u.au
+        model = Model(datacube, Rmax=Rmax, Rmin=Rmin, prototype=True)
         
-    return parser.parse_args()
-        
+        model.z_upper_func = cart.z_upper_exp_tapered
+        model.z_lower_func = cart.z_lower_exp_tapered
+        model.velocity_func = model.keplerian_vertical # vrot = sqrt(GM/r**3)*R
+        model.line_profile = model.line_profile_bell
+    
+        if 'I2pwl' in meta['kind']:
+            model.intensity_func = cart.intensity_powerlaw_rbreak
+        elif 'I2pwlnosurf' in meta['kind']:
+            model.intensity_func = cart.intensity_powerlaw_rbreak_nosurf    
+        else:
+            model.intensity_func = cart.intensity_powerlaw_rout
+
+        #****************
+        #PROTOTYPE PARAMS
+        #****************
+        model.params = copy.copy(best)
+        model.params['intensity']['I0'] /= meta['downsamp_factor']
+
+        return datacube, model
+
+    else:
+        return datacube
+
+    
 def read_json(decimals=True): #Read json file again but keep track of (if) decimals
     if decimals:
         parse_func = lambda x: decimal.Decimal(str(x))
     else:
         parse_func = float
 
     with open('parfile.json') as json_file: 
@@ -166,16 +233,17 @@
         clim0, clim1 = 0.0, I_res2abs*clim1_res
         unit = '[K]'
         clabel = r'Peak Intensity %s%s'%(tag, unit)
         clabel_res = r'Peak Int. residuals %s'%unit    
     
     return clabel, clabel_res, clim0, clim0_res, clim1, clim1_res, unit
 
-def get_noise_mask(data, thres=4, return_mean=True):
+def get_noise_mask(datacube, thres=4, return_mean=True):
     #std from line-free channels, per pixel
+    data = datacube.data
     noise = np.std( np.append(data[:5,:,:], data[-5:,:,:], axis=0), axis=0) 
     if return_mean:
         noise_mean = np.mean(noise)
         mask = np.nanmax(data, axis=0) < thres*noise_mean
         return noise_mean, mask
     else:
         mask = np.nanmax(data, axis=0) < thres*noise
@@ -219,7 +287,12 @@
     )
 
     z = dict(
         upper=np.load('upper_z.npy'),
         lower=np.load('lower_z.npy')
     )
     return R, phi, z
+
+def make_1d_legend(ax, **kwargs):
+    kwargs_def = dict(frameon=False, fontsize=MEDIUM_SIZE-2, ncol=3, loc='lower right', bbox_to_anchor=(1.0, 1.0))
+    kwargs_def.update(kwargs)
+    return ax.legend(**kwargs_def)
```

### Comparing `discminer-0.1.1/discminer/cart.py` & `discminer-0.2.0/discminer/cart.py`

 * *Files identical despite different names*

### Comparing `discminer-0.1.1/discminer/core.py` & `discminer-0.2.0/discminer/core.py`

 * *Files identical despite different names*

### Comparing `discminer-0.1.1/discminer/cube.py` & `discminer-0.2.0/discminer/cube.py`

 * *Files identical despite different names*

### Comparing `discminer-0.1.1/discminer/disc2d.py` & `discminer-0.2.0/discminer/disc2d.py`

 * *Files identical despite different names*

### Comparing `discminer-0.1.1/discminer/grid.py` & `discminer-0.2.0/discminer/grid.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
     xgrid = np.linspace(-xmax, xmax, nx)
     xygrid = [xgrid, xgrid]
     XY = np.meshgrid(xgrid, xgrid, indexing=indexing)
     xList, yList = [xy.flatten() for xy in XY]
     RList = np.linalg.norm([xList, yList], axis=0)
     phiList = np.arctan2(yList, xList)
-    phiList = np.where(phiList < 0, phiList + 2 * np.pi, phiList)
+    #phiList = np.where(phiList < 0, phiList + 2 * np.pi, phiList)
     _break_line()
 
     return {
         "x": xList,
         "y": yList,
         "R": RList,
         "phi": phiList,
```

### Comparing `discminer-0.1.1/discminer/icons/button_box.png` & `discminer-0.2.0/discminer/icons/button_box.png`

 * *Files identical despite different names*

### Comparing `discminer-0.1.1/discminer/icons/button_cursor.jpeg` & `discminer-0.2.0/discminer/icons/button_cursor.jpeg`

 * *Files identical despite different names*

### Comparing `discminer-0.1.1/discminer/icons/button_path.png` & `discminer-0.2.0/discminer/icons/button_path.png`

 * *Files identical despite different names*

### Comparing `discminer-0.1.1/discminer/icons/button_return.png` & `discminer-0.2.0/discminer/icons/button_return.png`

 * *Files identical despite different names*

### Comparing `discminer-0.1.1/discminer/icons/button_surface.png` & `discminer-0.2.0/discminer/icons/button_surface.png`

 * *Files identical despite different names*

### Comparing `discminer-0.1.1/discminer/icons/button_trash.jpg` & `discminer-0.2.0/discminer/icons/button_trash.jpg`

 * *Files identical despite different names*

### Comparing `discminer-0.1.1/discminer/pick.py` & `discminer-0.2.0/discminer/pick.py`

 * *Files identical despite different names*

### Comparing `discminer-0.1.1/discminer/plottools.py` & `discminer-0.2.0/discminer/plottools.py`

 * *Files 11% similar despite different names*

```diff
@@ -271,76 +271,29 @@
             return 0
 
     kwargs = dict(fontsize=SMALL_SIZE+3, ha='center', va=_va, weight='bold', rotation=0)
     kwargs.update(kwargs_text)
     for Ri in Rlist:
         ax.text(posx, sposy*(Ri+dy), fmt%Ri, **kwargs)
         
-def _make_text_1D_substructures(ax, gaps=[], rings=[], kinks=[]):
+def _make_text_1D_substructures(ax, gaps=[], rings=[], kinks=[],
+                                label_gaps=False, label_rings=False, label_kinks=False):
     kwargs_text = dict(fontsize=SMALL_SIZE+2, ha='center', va='bottom', transform=ax.transAxes, weight='bold', rotation=90)    
     xlims = ax.get_xlim()
     xext = xlims[1]-xlims[0]
 
     def text_it(R, text):
         for Ri in R:
             if Ri < xlims[0]: continue
             posx = (Ri-xlims[0])/xext
             ax.text(posx, 1.02, text%Ri, **kwargs_text)        
 
-    text_it(gaps, r'D%d')
-    text_it(rings, r'B%d')
-    text_it(kinks, r'K%d')
-
-def make_substructures(ax, gaps=[], rings=[], kinks=[],
-                       twodim=False, polar=False, make_labels=True, make_legend=False, 
-                       kwargs_gaps={}, kwargs_rings={}, kwargs_kinks={}, func1d='axvline'):
-    '''Overlay ring-like (if twodim) or vertical lines (if not twodim) to illustrate the radial location of substructures in the disc'''
-    kwargs_g = dict(color='0.2', ls='--', lw=1.7, dash_capstyle='round', dashes=(3.0, 2.5), alpha=1.0)
-    kwargs_r = dict(color='0.2', ls='-', lw=1.7, dash_capstyle='round', alpha=1.0)
-    kwargs_k = dict(color='purple', ls=':', lw=2.5, dash_capstyle='round', dashes=(0.5, 1.5), alpha=0.9)
-    kwargs_g.update(kwargs_gaps)
-    kwargs_r.update(kwargs_rings)
-    kwargs_k.update(kwargs_kinks)        
-    if twodim:
-        nphi = 100
-        phi = np.linspace(0, 2*np.pi, nphi)
-        phi_deg = np.degrees(phi-np.pi)
-        subst_fmt = zip([gaps, rings, kinks], ['D%d', 'B%d', 'K%d'])
-        if polar:
-            for R in gaps: ax.plot(phi_deg, [R]*nphi, **kwargs_g)
-            for R in rings: ax.plot(phi_deg, [R]*nphi, **kwargs_r)
-            for R in kinks: ax.plot(phi_deg, [R]*nphi, **kwargs_k)
-            if make_labels:
-                for subst, fmt in subst_fmt:
-                    _make_text_2D(ax, subst, posx=-45, fmt=fmt)                
-        else:
-            cos_phi = np.cos(phi)
-            sin_phi = np.sin(phi)
-            for R in gaps: ax.plot(R*cos_phi, R*sin_phi, **kwargs_g)
-            for R in rings: ax.plot(R*cos_phi, R*sin_phi, **kwargs_r)
-            for R in kinks: ax.plot(R*cos_phi, R*sin_phi, **kwargs_k)
-            if make_labels:
-                for subst, fmt in subst_fmt:
-                    _make_text_2D(ax, subst, sposy=-1, fmt=fmt)
-            
-    else:
-        if func1d=='axvline': func1d=ax.axvline
-        elif func1d=='axhline': func1d=ax.axhline            
-        for R in gaps: func1d(R, **kwargs_g)
-        for R in rings: func1d(R, **kwargs_r)
-        for R in kinks: func1d(R, **kwargs_k)
-
-        if make_labels:
-            _make_text_1D_substructures(ax, gaps=gaps, rings=rings, kinks=kinks)
-        
-    if make_legend and len(gaps)>0: ax.plot([None], [None], label='Gaps', **kwargs_g)
-    if make_legend and len(rings)>0: ax.plot([None], [None], label='Rings', **kwargs_r)
-    if make_legend and len(kinks)>0: ax.plot([None], [None], label='Kinks', **kwargs_k)
-
-    return ax
+    if label_gaps: text_it(gaps, r'D%d')
+    if label_rings: text_it(rings, r'B%d')
+    if label_kinks: text_it(kinks, r'K%d')
 
 def _make_radial_grid_2D(ax, Rout, gaps=[], rings=[], kinks=[], make_labels=True, label_freq=2):
     get_intdigits = lambda n: len(str(n).split('.')[0])
     
     angs = np.linspace(0, 2*np.pi, 100)
     cos_angs = np.cos(angs)
     sin_angs = np.sin(angs)
@@ -410,22 +363,74 @@
         ii = np.argmin(np.abs(cn-xlim))
         text_nsky(xn[ii], yn[ii])
     else:
         text_nsky(xni, yni)
 
     return xni, yni
 
+def make_substructures(ax, gaps=[], rings=[], kinks=[],
+                       twodim=False, polar=False, make_legend=False,
+                       label_gaps=False, label_rings=False, label_kinks=False,
+                       kwargs_gaps={}, kwargs_rings={}, kwargs_kinks={}, func1d='axvline'):
+    '''Overlay ring-like (if twodim) or vertical lines (if not twodim) to illustrate the radial location of substructures in the disc'''
+    kwargs_g = dict(color='0.2', ls='--', lw=1.7, dash_capstyle='round', dashes=(3.0, 2.5), alpha=1.0)
+    kwargs_r = dict(color='0.2', ls='-', lw=1.7, dash_capstyle='round', alpha=1.0)
+    kwargs_k = dict(color='purple', ls=':', lw=2.5, dash_capstyle='round', dashes=(0.5, 1.5), alpha=0.9)
+    kwargs_g.update(kwargs_gaps)
+    kwargs_r.update(kwargs_rings)
+    kwargs_k.update(kwargs_kinks)        
+    if twodim:
+        nphi = 100
+        phi = np.linspace(0, 2*np.pi, nphi)
+        phi_deg = np.degrees(phi-np.pi)
+        subst_fmt = zip([gaps, rings, kinks], ['D%d', 'B%d', 'K%d'], [label_gaps, label_rings, label_kinks])
+        if polar:
+            for R in gaps: ax.plot(phi_deg, [R]*nphi, **kwargs_g)
+            for R in rings: ax.plot(phi_deg, [R]*nphi, **kwargs_r)
+            for R in kinks: ax.plot(phi_deg, [R]*nphi, **kwargs_k)
 
+            for subst, fmt, label in subst_fmt:
+                if label:
+                    _make_text_2D(ax, subst, posx=-45, fmt=fmt)                
+        else:
+            cos_phi = np.cos(phi)
+            sin_phi = np.sin(phi)
+            for R in gaps: ax.plot(R*cos_phi, R*sin_phi, **kwargs_g)
+            for R in rings: ax.plot(R*cos_phi, R*sin_phi, **kwargs_r)
+            for R in kinks: ax.plot(R*cos_phi, R*sin_phi, **kwargs_k)
+
+            for subst, fmt, label in subst_fmt:
+                if label:
+                    _make_text_2D(ax, subst, sposy=-1, fmt=fmt)
+            
+    else:
+        if func1d=='axvline': func1d=ax.axvline
+        elif func1d=='axhline': func1d=ax.axhline            
+        for R in gaps: func1d(R, **kwargs_g)
+        for R in rings: func1d(R, **kwargs_r)
+        for R in kinks: func1d(R, **kwargs_k)
+
+        _make_text_1D_substructures(ax, gaps=gaps, rings=rings, kinks=kinks,
+                                    label_gaps=label_gaps, label_rings=label_rings, label_kinks=label_kinks)
+        
+    if make_legend and len(gaps)>0: ax.plot([None], [None], label='Gaps', **kwargs_g)
+    if make_legend and len(rings)>0: ax.plot([None], [None], label='Rings', **kwargs_r)
+    if make_legend and len(kinks)>0: ax.plot([None], [None], label='Kinks', **kwargs_k)
+
+    return ax
+
+#*********************
+#MAKE DEPROJECTED MAPS
+#*********************
 def make_round_map(
         map2d, levels, X, Y, Rout,
         z_func=None, z_pars=None, incl=None, PA=None, xc=0, yc=0, #Optional, make N-sky axis
         fig=None, ax=None,
         rwidth=0.06, cmap=get_discminer_cmap('velocity'), clabel='km/s', fmt='%5.2f', quadrant=None, #cbar kwargs
         gaps=[], rings=[], kinks=[],
-        label_gaps=False, label_rings=True, label_kinks=True,
         mask_wedge=None, mask_inner=None
 ):
 
     #SOME DEFINITIONS
     if fig is None:
         fig, ax = plt.subplots(ncols=1, nrows=1, figsize=(10, 10))
 
@@ -437,36 +442,27 @@
     
     cmap_c = copy.copy(cmap)
     cmap_c.set_under('0.4')
     cmap_c.set_over('0.4')
     
     #MAIN PLOT
     im = ax.contourf(X, Y, map2d, levels=levels, cmap=cmap_c, extend='both', origin='lower')
-    make_substructures(ax, gaps=gaps, rings=rings, kinks=kinks, twodim=True, make_labels=False)
 
     #RADIAL GRID
     _make_radial_grid_2D(ax, Rout, gaps=gaps, rings=rings, kinks=kinks, label_freq=2)
     
     #AZIMUTHAL GRID
     _make_azimuthal_grid_2D(ax, Rout)
     
     #SKY AXIS
     if np.all(np.asarray([z_func, z_pars, incl, PA])!=None):
         xni, yni = _make_nsky_2D(ax, Rout, xlim_rec,
                                  z_func, z_pars, incl, PA, xc=xc, yc=yc)
     else:
         xni, yni = None, None
-        
-    #SUBSTRUCTURE LABELS
-    if label_gaps:
-        _make_text_2D(ax, gaps, sposy=-1, fmt='D%d')
-    if label_rings:
-        _make_text_2D(ax, rings, sposy=-1, fmt='B%d')
-    if label_kinks:
-        _make_text_2D(ax, kinks, sposy=-1, fmt='K%d')
 
     #SET LIMITS AND AXES
     for side in ['left','top','right']: ax.spines[side].set_visible(False)
     make_up_ax(ax,
                xlims=(-xlim_rec, xlim_rec),
                ylims=(-xlim_rec, xlim_rec),
                labelleft=False, left=False, right=False, labeltop=False, top=False, labelbottom=True, bottom=True,
@@ -493,30 +489,40 @@
     }[quadrant]
         
     ax.plot([sq*Rout, sq*Rout], [0, -xlim_rec], color='0.0', lw=1.0, dash_capstyle='round', dashes=(1.5, 2.5)) #Rout projected onto Cartesian xaxis
 
     #MASK
     kw_mask = dict(facecolor='0.5', edgecolor='k', lw=1.0, alpha=0.6)
     if mask_wedge is not None:
-        wedge = patches.Wedge((0,0), Rout, *mask_wedge.to('deg').value, **kw_mask)
-        ax.add_artist(wedge)
 
+        for wedge in mask_wedge:
+
+            if np.isscalar(wedge.value): #single wedge
+                w = patches.Wedge((0,0), Rout, *mask_wedge.to('deg').value, **kw_mask)
+                ax.add_artist(w)
+                break            
+
+            else: #list of wedges
+                w = patches.Wedge((0,0), Rout, *wedge.to('deg').value, **kw_mask)
+                ax.add_artist(w)
+    
     if mask_inner is not None:
         inner = patches.Circle((0,0), mask_inner.to('au').value, **kw_mask)
         ax.add_artist(inner)
         
     return fig, ax
-        
+
+
 def make_polar_map(
         map2d, levels, R, PHI, Rout,
         Rin = 0.0,
         fig=None, ax=None, 
         cmap=get_discminer_cmap('velocity'),
         fmt='%5.2f', clabel=None, 
-        gaps=[], rings=[], kinks=[] #,filaments=[],                            
+        #,filaments=[],                            
 ):
     from scipy.interpolate import griddata
 
     #SOME DEFINITIONS
     if fig is None:
         fig, ax = plt.subplots(ncols=1, nrows=1, figsize=(12, 3))
     Rout = Rout.to('au').value
@@ -560,26 +566,116 @@
 
     make_up_ax(ax, labelbottom=True, labeltop=False, labelsize=SMALL_SIZE+1,
                xlims=(-180.1, 180.1), ylims=(1.1*Rin, 0.95*Rout))
     ax.set_xticks(np.linspace(-180, 180, 13))
     ax.set_xlabel('Azimuth [deg]', fontsize=MEDIUM_SIZE)
     ax.set_ylabel('Radius [au]', fontsize=MEDIUM_SIZE)
     mod_major_ticks(ax, axis='y', nbins=10)
-    
-    make_substructures(ax, gaps=gaps, rings=rings, kinks=kinks, twodim=True, polar=True)
                        
     cax = add_cbar_ax(fig, ax, orientation='vertical', subplots=False, perc=6)    
     cbar = plt.colorbar(im, cax=cax, format=fmt, orientation='vertical', ticks=np.linspace(levels.min(), levels.max(), 5))
     cbar.ax.tick_params(which='major', direction='in', width=2.7, size=4.8, pad=4, labelsize=SMALL_SIZE)
     cbar.ax.tick_params(which='minor', direction='in', width=2.7, size=3.3)
     cbar.set_label(clabel, fontsize=SMALL_SIZE, labelpad=20, rotation=270)
     mod_minor_ticks(cbar.ax)
 
     return fig, ax, cbar
 
+
+def make_pie_map(
+        X, Y, Rout,
+        quadrant_map2d = {1: None, 2: None, 3: None, 4: None},
+        quadrant_levels = {1: None, 2: None, 3: None, 4: None},
+        quadrant_cmap = {1: 'gnuplot2', 2: 'jet', 3: 'plasma', 4: 'seismic'},
+        quadrant_clabel = {1: None, 2: None, 3: None, 4: None},
+        quadrant_fmt = {1: '%4d', 2: '%4d', 3: '%4d', 4: '%4d'},        
+        gaps=[], rings=[], kinks=[],
+        fig=None, ax=None,        
+):
+    #SOME DEFINITIONS
+    if fig is None:
+        fig, ax = plt.subplots(ncols=1, nrows=1, figsize=(10, 10))
+
+    Rout = Rout.to('au').value
+    X = X.to('au').value
+    Y = Y.to('au').value
+
+    quadrant_reg = {4: ((X>=0) & (Y<0)),
+                    3: ((X<0) & (Y<=0)),
+                    2: ((X<=0) & (Y>0)),
+                    1: ((X>0) & (Y>=0))
+    }
+    
+    #CBAR STUFF
+    figx, figy = fig.get_size_inches()
+    figr = figy/figx
+    axp = ax.get_position()
+    x0, x1, y0, y1 = axp.x0, axp.x1, axp.y0, axp.y1
+    w = x1 - x0
+    h = y1 - y0
+    dx = 0.02
+    dy = 6*dx
+
+    cbar_pos = {1: [x1, y1-0.4*h, dx, dy],
+                2: [x0-dx, y1-0.4*h, dx, dy],
+                3: [x0-dx, y0+0.4*h-dy, dx, dy],
+                4: [x1, y0+0.4*h-dy, dx, dy]}
+
+    #MAKE ALL
+    for quad in [1,2,3,4]:
+        inquad = quadrant_reg[quad]
+        map2d = quadrant_map2d[quad]
+        levels = quadrant_levels[quad]
+        cmap = quadrant_cmap[quad]
+        clabel = quadrant_clabel[quad]
+        cfmt = quadrant_fmt[quad]
+        
+        if map2d is None:
+            map2d = np.zeros_like(X)
+        else:
+            map2d[~inquad] = np.nan
+
+        if levels is None:
+            levels = np.linspace(np.nanmin(map2d), np.nanmax(map2d), 64)
+            
+        im = ax.contourf(X, Y, map2d, levels=levels, extend='both', cmap=cmap)
+    
+        ax_cbar = fig.add_axes(cbar_pos[quad])
+        cbar_ticks = np.linspace(np.min(levels), np.max(levels), 5)
+        cbar = plt.colorbar(im, cax=ax_cbar, format=cfmt, orientation='vertical', ticks=cbar_ticks)
+        cbar.ax.tick_params(which='major', direction='in', width=2.7, size=4.8, pad=7, labelsize=MEDIUM_SIZE-2)
+        cbar.ax.tick_params(which='minor', direction='in', width=2.7, size=3.3)
+        cbar.set_label(clabel, fontsize=MEDIUM_SIZE, rotation=90, labelpad=7)        
+        mod_minor_ticks(cbar.ax)
+
+        if quad==2 or quad==3:
+            cbar.ax.tick_params(which='both', left=True, right=False, labelleft=True, labelright=False)
+        else:
+            cbar.ax.yaxis.set_label_position('left')
+            
+    _make_radial_grid_2D(ax, Rout, gaps=gaps, rings=rings, kinks=kinks, make_labels=True, label_freq=2)
+
+    for side in ['left','top','right']: ax.spines[side].set_visible(False)
+    for side in ['left']: ax.spines[side].set_linewidth(3.5)
+
+    make_up_ax(ax,
+               xlims=(-1.15*Rout, 1.15*Rout),
+               ylims=(-Rout-5, Rout+5),
+               labelleft=False, left=False, right=False,
+               labeltop=False, top=False,
+               labelbottom=True, bottom=True,
+               labelsize=MEDIUM_SIZE+2, rotation=45)
+    mod_major_ticks(ax, axis='x', nbins=10)
+    
+    ax.set_xlabel('Offset [au]', fontsize=MEDIUM_SIZE+2)
+    ax.set_aspect(1)
+    
+    return fig, ax
+
+
 #***************************
 #PEAK RESIDUALS AND CLUSTERS
 #***************************
 def append_sigma_panel(fig, ax, values, ax_std=None, weights=None, hist=False, fit_gauss_hist=False): #attach sigma panel to AxesSubplot, based on input values
     ax = np.atleast_1d(ax)
 
     if ax_std is None:
```

### Comparing `discminer-0.1.1/discminer/rail.py` & `discminer-0.2.0/discminer/rail.py`

 * *Files identical despite different names*

### Comparing `discminer-0.1.1/discminer/testyapf.py` & `discminer-0.2.0/discminer/testyapf.py`

 * *Files identical despite different names*

### Comparing `discminer-0.1.1/discminer/tools/discminer.mplstyle` & `discminer-0.2.0/discminer/tools/discminer.mplstyle`

 * *Files identical despite different names*

### Comparing `discminer-0.1.1/discminer/tools/fit_kernel.py` & `discminer-0.2.0/discminer/tools/fit_kernel.py`

 * *Files identical despite different names*

### Comparing `discminer-0.1.1/discminer/tools/utils.py` & `discminer-0.2.0/discminer/tools/utils.py`

 * *Files identical despite different names*

### Comparing `discminer-0.1.1/discminer.egg-info/PKG-INFO` & `discminer-0.2.0/discminer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discminer
-Version: 0.1.1
+Version: 0.2.0
 Summary: Python package for parametric modelling of intensity channel maps from gas discs
 Home-page: https://github.com/andizq/discminer
 Author: Andres F. Izquierdo
 Author-email: andres.izquierdo.c@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/andizq/discminer/issues
 Project-URL: Source, https://github.com/andizq/discminer/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: discminer Version: 0.1.1 Summary: Python package
+Metadata-Version: 2.1 Name: discminer Version: 0.2.0 Summary: Python package
 for parametric modelling of intensity channel maps from gas discs Home-page:
 https://github.com/andizq/discminer Author: Andres F. Izquierdo Author-email:
 andres.izquierdo.c@gmail.com License: UNKNOWN Project-URL: Bug Reports, https:/
 /github.com/andizq/discminer/issues Project-URL: Source, https://github.com/
 andizq/discminer/ Description:
  [https://raw.githubusercontent.com/andizq/andizq.github.io/master/discminer/
                              discminer_logo.jpeg]
```

### Comparing `discminer-0.1.1/discminer.egg-info/SOURCES.txt` & `discminer-0.2.0/discminer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `discminer-0.1.1/setup.py` & `discminer-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `discminer-0.1.1/template/README.rst` & `discminer-0.2.0/template/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -175,8 +175,21 @@
    :width: 80 %
    :align: center
 	   
 .. image:: ../images/radial_profile_residuals_linewidth_gaussian.png
    :width: 80 %
    :align: center
 
+
+- **TIP**: The ``writetxt`` argument activated with a ``-w 1`` flag in command line is particularly useful to produce .txt outputs of radial profiles for further analysis.
+  
+  .. code-block:: bash
+
+	python ../_mining/plot_radial_profiles.py -m velocity -w 1
+	python ../_mining/plot_velocity_components.py
+
+.. image:: ../images/pie_velocity_components_velocity_gaussian.png
+   :width: 80 %
+   :align: center	   
+	
+	   
 Details on the physical interpretation of the substructures identified in this and in the other discs of the MAPS sample can be found in the work of Izquierdo et al. (2023).
```

### Comparing `discminer-0.1.1/template/download_MAPS.sh` & `discminer-0.2.0/template/download_MAPS.sh`

 * *Files identical despite different names*

### Comparing `discminer-0.1.1/template/log_pars_mwc480_12co_0p2_maps_cube_256walkers_10000steps.txt` & `discminer-0.2.0/template/log_pars_mwc480_12co_0p2_maps_cube_256walkers_10000steps.txt`

 * *Files identical despite different names*

### Comparing `discminer-0.1.1/template/prepare_data.py` & `discminer-0.2.0/template/prepare_data.py`

 * *Files identical despite different names*

