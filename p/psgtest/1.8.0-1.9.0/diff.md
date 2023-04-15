# Comparing `tmp/psgtest-1.8.0.tar.gz` & `tmp/psgtest-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\psgtest-1.8.0.tar", last modified: Tue Nov  9 13:55:52 2021, max compression
+gzip compressed data, was "dist\psgtest-1.9.0.tar", last modified: Fri Nov 12 18:30:09 2021, max compression
```

## Comparing `psgtest-1.8.0.tar` & `psgtest-1.9.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2021-11-09 13:55:52.000000 psgtest-1.8.0/
--rw-rw-rw-   0        0        0     6025 2021-11-09 13:55:52.000000 psgtest-1.8.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2021-11-09 13:55:52.000000 psgtest-1.8.0/psgtest/
--rw-rw-rw-   0        0        0    16958 2021-11-04 18:03:39.000000 psgtest-1.8.0/psgtest/gui.ico
--rw-rw-rw-   0        0        0    28067 2021-11-09 13:46:40.000000 psgtest-1.8.0/psgtest/gui.py
--rw-rw-rw-   0        0        0       23 2021-11-09 13:26:02.000000 psgtest-1.8.0/psgtest/__init__.py
-drwxrwxrwx   0        0        0        0 2021-11-09 13:55:52.000000 psgtest-1.8.0/psgtest.egg-info/
--rw-rw-rw-   0        0        0        1 2021-11-09 13:55:52.000000 psgtest-1.8.0/psgtest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2021-11-09 13:55:52.000000 psgtest-1.8.0/psgtest.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0     6025 2021-11-09 13:55:52.000000 psgtest-1.8.0/psgtest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       12 2021-11-09 13:55:52.000000 psgtest-1.8.0/psgtest.egg-info/requires.txt
--rw-rw-rw-   0        0        0      257 2021-11-09 13:55:52.000000 psgtest-1.8.0/psgtest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        8 2021-11-09 13:55:52.000000 psgtest-1.8.0/psgtest.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5034 2021-11-09 13:51:10.000000 psgtest-1.8.0/README.md
--rw-rw-rw-   0        0        0       42 2021-11-09 13:55:52.000000 psgtest-1.8.0/setup.cfg
--rw-rw-rw-   0        0        0     1401 2021-11-09 13:25:50.000000 psgtest-1.8.0/setup.py
+drwxrwxrwx   0        0        0        0 2021-11-12 18:30:09.000000 psgtest-1.9.0/
+-rw-rw-rw-   0        0        0     6316 2021-11-12 18:30:09.000000 psgtest-1.9.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2021-11-12 18:30:09.000000 psgtest-1.9.0/psgtest/
+-rw-rw-rw-   0        0        0    16958 2021-11-04 18:03:39.000000 psgtest-1.9.0/psgtest/gui.ico
+-rw-rw-rw-   0        0        0    28596 2021-11-12 18:21:37.000000 psgtest-1.9.0/psgtest/gui.py
+-rw-rw-rw-   0        0        0       23 2021-11-12 18:21:37.000000 psgtest-1.9.0/psgtest/__init__.py
+drwxrwxrwx   0        0        0        0 2021-11-12 18:30:09.000000 psgtest-1.9.0/psgtest.egg-info/
+-rw-rw-rw-   0        0        0        1 2021-11-12 18:30:09.000000 psgtest-1.9.0/psgtest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2021-11-12 18:30:09.000000 psgtest-1.9.0/psgtest.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0     6316 2021-11-12 18:30:09.000000 psgtest-1.9.0/psgtest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       20 2021-11-12 18:30:09.000000 psgtest-1.9.0/psgtest.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      257 2021-11-12 18:30:09.000000 psgtest-1.9.0/psgtest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        8 2021-11-12 18:30:09.000000 psgtest-1.9.0/psgtest.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5325 2021-11-12 18:29:52.000000 psgtest-1.9.0/README.md
+-rw-rw-rw-   0        0        0       42 2021-11-12 18:30:09.000000 psgtest-1.9.0/setup.cfg
+-rw-rw-rw-   0        0        0     1409 2021-11-12 18:24:18.000000 psgtest-1.9.0/setup.py
```

### Comparing `psgtest-1.8.0/PKG-INFO` & `psgtest-1.9.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psgtest
-Version: 1.8.0
+Version: 1.9.0
 Summary: Run your Python programs, capture the output, using your choice of interpreters
 Home-page: https://github.com/PySimpleGUI/psgtest
 Author: PySimpleGUI
 Author-email: PySimpleGUI@PySimpleGUI.org
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -97,14 +97,20 @@
 You can find the location of psgtest after pip installing it by running psgtest, right clicking, and choosing "File Location".  You'll be shown where the `gui.py` file is located (the name of the psgtest program when pip installed).  It will usually be located in the `site-packages` folder in a folder named  `psgtest`.
 
 Instructions on how to make shortcuts to pip installed PySimpleGUI programs can be found in [description for psgshortcut on PyPI](https://pypi.org/project/psgshortcut/).
 
 
 ## Release Notes
 
+### 1.9.0
+
+* Fix for exception when no settings are initially found.  Oy.... bad bug to have released reight away
+* Will create a settings file with the currently running version of Python if one is not found
+* Added minimum of 4.55.1 requirement for PySimpleGUI to the setup.py file
+
 ### 1.8.0
 
 * Support for Python 3.4, 3.5, 3.11 added to settings 
 * Set the settings filename to be `psgtest` instead of the default filename. This is needed because the file for these psg projects on PyPI are all name gui.py and thus will have all point to the same settings file if not explicitly set
 * Only show configured interpreters in the Combo in main window     
 
 ## License
```

### Comparing `psgtest-1.8.0/psgtest/gui.ico` & `psgtest-1.9.0/psgtest/gui.ico`

 * *Files identical despite different names*

### Comparing `psgtest-1.8.0/psgtest/gui.py` & `psgtest-1.9.0/psgtest/gui.py`

 * *Files 5% similar despite different names*

```diff
@@ -210,15 +210,15 @@
 '''
 
 
 def make_output_tab(tab_text, key, tab_key):
     tab = sg.Tab(tab_text, [[sg.Multiline(
         size=(sg.user_settings_get_entry('-output width-', DEFAULT_OUTPUT_SIZE[0]), sg.user_settings_get_entry('-output height-', DEFAULT_OUTPUT_SIZE[1])),
         expand_x=True, expand_y=True, write_only=True, key=key, auto_refresh=True, font=sg.user_settings_get_entry('-output font-', 'Courier 10')), ],
-                            [sg.B('Copy To Clipboard', k=('-COPY-', key)), sg.B('Clear', k=('-CLEAR-', key)), sg.B('Close Tab', k=('-CLOSE-', tab_key))]],
+        [sg.B('Copy To Clipboard', k=('-COPY-', key)), sg.B('Clear', k=('-CLEAR-', key)), sg.B('Close Tab', k=('-CLOSE-', tab_key))]],
                  right_click_menu=['', [f'Close::{tab_key}', 'Exit']], k=tab_key, )
 
     return tab
 
 
 '''
 M"""""`'"""`YM          dP                
@@ -294,19 +294,26 @@
     # interpreter_keys = sorted(list(interpreter_dict.values()))
     interpreter_list = []
     for key, value in interpreter_dict.items():
         if sg.user_settings_get_entry(value, ''):
             interpreter_list.append(key)
 
     interpreter_list = sorted(interpreter_list)
-
+    if len(interpreter_list) == 0:  # no interpreters found in settings file, so set one using the currently running version of Python
+        default_interpreter = f'{sys.version_info[0]}.{sys.version_info[1]}'
+        sg.user_settings_set_entry('-current interpreter-', default_interpreter)
+        sg.user_settings_set_entry('-interpreter path-', sys.executable)
+        key = interpreter_dict[default_interpreter]
+        sg.user_settings_set_entry(key, sys.executable)
+    else:
+        default_interpreter = interpreter_list[0]
     choose_interpreter_at_top = sg.pin(sg.Column([[sg.T('Launch using'),
                                                    sg.Combo(sorted(interpreter_list),
-                                                            default_value=sg.user_settings_get_entry('-current interpreter-', interpreter_list[0]),
-                                                            size=(4, len(interpreter_list)), key='-INTERPRETER TOP-', enable_events=True, readonly=True)]],
+                                                            default_value=sg.user_settings_get_entry('-current interpreter-', default_interpreter),
+                                                            size=(4, 10), key='-INTERPRETER TOP-', enable_events=True, readonly=True)]],
                                                  pad=(0, 0), k='-INTEPRETER CHOOSE-', expand_x=True, expand_y=True))
 
     # ----- Full layout -----
 
     layout = [[sg.Image(data=icon, background_color='white'), sg.Text('psgtest - Simple Python Testing', font='Any 20')],
               [sg.T('Testing Using Interpreter: ' + sg.user_settings_get_entry('-current interpreter-', ''), font='Default 12', k='-CURRENT INTERPRETER-'),
                sg.T('Interpreter path: ' + sg.user_settings_get_entry('-interpreter path-', ''), font='Default 12', k='-INTERPRETER PATH-')],
@@ -375,24 +382,24 @@
 
 
 def main():
     """
     The main program that contains the event loop.
     It will call the make_window function to create the window.
     """
-    sg.user_settings_filename(filename='psgtest')
+    sg.user_settings_filename(filename='psgtest.json')
     os.environ['PYTHONUNBUFFERED'] = '1'
     file_list_dict = get_file_list_dict()
     file_list = get_file_list()
     try:
         window = make_window()
     except Exception as e:
         if sg.popup_yes_no('Exception making the Window... likely means a corrupt settings file.', f'Exception: {e}', 'Do you want to clear your settings?',
                            title='Exception making window') == 'Yes':
-            sg.user_settings_delete_filename()
+            sg.user_settings_delete_filename(filename='psgtest.json')
             sg.popup_auto_close('Settings file deleted... please restart the program')
             exit()
         else:
             sg.popup_auto_close('Cancelling operation... See what you can do about the problem...')
             exit()
     window['-FILTER NUMBER-'].update(f'{len(file_list)} files')
     sp_to_mline_dict = {}
```

### Comparing `psgtest-1.8.0/psgtest.egg-info/PKG-INFO` & `psgtest-1.9.0/psgtest.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psgtest
-Version: 1.8.0
+Version: 1.9.0
 Summary: Run your Python programs, capture the output, using your choice of interpreters
 Home-page: https://github.com/PySimpleGUI/psgtest
 Author: PySimpleGUI
 Author-email: PySimpleGUI@PySimpleGUI.org
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -97,14 +97,20 @@
 You can find the location of psgtest after pip installing it by running psgtest, right clicking, and choosing "File Location".  You'll be shown where the `gui.py` file is located (the name of the psgtest program when pip installed).  It will usually be located in the `site-packages` folder in a folder named  `psgtest`.
 
 Instructions on how to make shortcuts to pip installed PySimpleGUI programs can be found in [description for psgshortcut on PyPI](https://pypi.org/project/psgshortcut/).
 
 
 ## Release Notes
 
+### 1.9.0
+
+* Fix for exception when no settings are initially found.  Oy.... bad bug to have released reight away
+* Will create a settings file with the currently running version of Python if one is not found
+* Added minimum of 4.55.1 requirement for PySimpleGUI to the setup.py file
+
 ### 1.8.0
 
 * Support for Python 3.4, 3.5, 3.11 added to settings 
 * Set the settings filename to be `psgtest` instead of the default filename. This is needed because the file for these psg projects on PyPI are all name gui.py and thus will have all point to the same settings file if not explicitly set
 * Only show configured interpreters in the Combo in main window     
 
 ## License
```

### Comparing `psgtest-1.8.0/README.md` & `psgtest-1.9.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -74,14 +74,20 @@
 You can find the location of psgtest after pip installing it by running psgtest, right clicking, and choosing "File Location".  You'll be shown where the `gui.py` file is located (the name of the psgtest program when pip installed).  It will usually be located in the `site-packages` folder in a folder named  `psgtest`.
 
 Instructions on how to make shortcuts to pip installed PySimpleGUI programs can be found in [description for psgshortcut on PyPI](https://pypi.org/project/psgshortcut/).
 
 
 ## Release Notes
 
+### 1.9.0
+
+* Fix for exception when no settings are initially found.  Oy.... bad bug to have released reight away
+* Will create a settings file with the currently running version of Python if one is not found
+* Added minimum of 4.55.1 requirement for PySimpleGUI to the setup.py file
+
 ### 1.8.0
 
 * Support for Python 3.4, 3.5, 3.11 added to settings 
 * Set the settings filename to be `psgtest` instead of the default filename. This is needed because the file for these psg projects on PyPI are all name gui.py and thus will have all point to the same settings file if not explicitly set
 * Only show configured interpreters in the Combo in main window     
 
 ## License
```

### Comparing `psgtest-1.8.0/setup.py` & `psgtest-1.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
             return f.read()
     except IOError:
         return ''
 
 
 setuptools.setup(
     name="psgtest",
-    version="1.8.0",
+    version="1.9.0",
     author="PySimpleGUI",
     author_email="PySimpleGUI@PySimpleGUI.org",
     description="Run your Python programs, capture the output, using your choice of interpreters",
     long_description=readme(),
     long_description_content_type="text/markdown",
     url="https://github.com/PySimpleGUI/psgtest",
     packages=['psgtest'],
-    install_requires=['PySimpleGUI'],
+    install_requires=['PySimpleGUI>=4.55.1'],
     classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.4",
         "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
```

