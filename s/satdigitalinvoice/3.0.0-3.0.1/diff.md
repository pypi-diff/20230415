# Comparing `tmp/satdigitalinvoice-3.0.0.tar.gz` & `tmp/satdigitalinvoice-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satdigitalinvoice-3.0.0.tar", last modified: Sat Apr 15 08:01:33 2023, max compression
+gzip compressed data, was "satdigitalinvoice-3.0.1.tar", last modified: Sat Apr 15 21:41:52 2023, max compression
```

## Comparing `satdigitalinvoice-3.0.0.tar` & `satdigitalinvoice-3.0.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:01:33.598478 satdigitalinvoice-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-15 08:01:33.598478 satdigitalinvoice-3.0.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:01:33.598478 satdigitalinvoice-3.0.0/satdigitalinvoice/
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-04-15 08:01:23.000000 satdigitalinvoice-3.0.0/satdigitalinvoice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-15 08:01:23.000000 satdigitalinvoice-3.0.0/satdigitalinvoice/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-04-15 08:01:23.000000 satdigitalinvoice-3.0.0/satdigitalinvoice/client_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-15 08:01:23.000000 satdigitalinvoice-3.0.0/satdigitalinvoice/environments.py
--rw-r--r--   0 runner    (1001) docker     (123)    36499 2023-04-15 08:01:23.000000 satdigitalinvoice-3.0.0/satdigitalinvoice/facturacion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4762 2023-04-15 08:01:23.000000 satdigitalinvoice-3.0.0/satdigitalinvoice/file_data_managers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:01:33.598478 satdigitalinvoice-3.0.0/satdigitalinvoice/formatting_functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 08:01:23.000000 satdigitalinvoice-3.0.0/satdigitalinvoice/formatting_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-04-15 08:01:23.000000 satdigitalinvoice-3.0.0/satdigitalinvoice/formatting_functions/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    10761 2023-04-15 08:01:23.000000 satdigitalinvoice-3.0.0/satdigitalinvoice/gui_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:01:33.598478 satdigitalinvoice-3.0.0/satdigitalinvoice/images/
--rw-r--r--   0 runner    (1001) docker     (123)    71867 2023-04-15 08:01:23.000000 satdigitalinvoice-3.0.0/satdigitalinvoice/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    17581 2023-04-15 08:01:23.000000 satdigitalinvoice-3.0.0/satdigitalinvoice/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-04-15 08:01:23.000000 satdigitalinvoice-3.0.0/satdigitalinvoice/localdb.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-15 08:01:23.000000 satdigitalinvoice-3.0.0/satdigitalinvoice/log_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:01:33.598478 satdigitalinvoice-3.0.0/satdigitalinvoice/markdown_styles/
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-15 08:01:23.000000 satdigitalinvoice-3.0.0/satdigitalinvoice/markdown_styles/markdown6.css
--rw-r--r--   0 runner    (1001) docker     (123)     5694 2023-04-15 08:01:23.000000 satdigitalinvoice-3.0.0/satdigitalinvoice/mycfdi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:01:33.598478 satdigitalinvoice-3.0.0/satdigitalinvoice/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-15 08:01:23.000000 satdigitalinvoice-3.0.0/satdigitalinvoice/schemas/cliente.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-15 08:01:23.000000 satdigitalinvoice-3.0.0/satdigitalinvoice/schemas/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-15 08:01:23.000000 satdigitalinvoice-3.0.0/satdigitalinvoice/schemas/factura.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-04-15 08:01:23.000000 satdigitalinvoice-3.0.0/satdigitalinvoice/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:01:33.598478 satdigitalinvoice-3.0.0/satdigitalinvoice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-15 08:01:33.000000 satdigitalinvoice-3.0.0/satdigitalinvoice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-15 08:01:33.000000 satdigitalinvoice-3.0.0/satdigitalinvoice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 08:01:33.000000 satdigitalinvoice-3.0.0/satdigitalinvoice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-15 08:01:33.000000 satdigitalinvoice-3.0.0/satdigitalinvoice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-15 08:01:33.000000 satdigitalinvoice-3.0.0/satdigitalinvoice.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 08:01:33.598478 satdigitalinvoice-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-04-15 08:01:23.000000 satdigitalinvoice-3.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:01:33.598478 satdigitalinvoice-3.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-15 08:01:23.000000 satdigitalinvoice-3.0.0/tests/test_clients.py
--rw-r--r--   0 runner    (1001) docker     (123)     6276 2023-04-15 08:01:23.000000 satdigitalinvoice-3.0.0/tests/test_crear_facturas.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-04-15 08:01:23.000000 satdigitalinvoice-3.0.0/tests/test_localdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-04-15 08:01:23.000000 satdigitalinvoice-3.0.0/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 21:41:52.207517 satdigitalinvoice-3.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-15 21:41:52.207517 satdigitalinvoice-3.0.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 21:41:52.203517 satdigitalinvoice-3.0.1/satdigitalinvoice/
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-04-15 21:41:41.000000 satdigitalinvoice-3.0.1/satdigitalinvoice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-15 21:41:41.000000 satdigitalinvoice-3.0.1/satdigitalinvoice/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-04-15 21:41:41.000000 satdigitalinvoice-3.0.1/satdigitalinvoice/client_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-15 21:41:41.000000 satdigitalinvoice-3.0.1/satdigitalinvoice/environments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37039 2023-04-15 21:41:41.000000 satdigitalinvoice-3.0.1/satdigitalinvoice/facturacion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4762 2023-04-15 21:41:41.000000 satdigitalinvoice-3.0.1/satdigitalinvoice/file_data_managers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 21:41:52.203517 satdigitalinvoice-3.0.1/satdigitalinvoice/formatting_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 21:41:41.000000 satdigitalinvoice-3.0.1/satdigitalinvoice/formatting_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-04-15 21:41:41.000000 satdigitalinvoice-3.0.1/satdigitalinvoice/formatting_functions/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10761 2023-04-15 21:41:41.000000 satdigitalinvoice-3.0.1/satdigitalinvoice/gui_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 21:41:52.203517 satdigitalinvoice-3.0.1/satdigitalinvoice/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    71867 2023-04-15 21:41:41.000000 satdigitalinvoice-3.0.1/satdigitalinvoice/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    19075 2023-04-15 21:41:41.000000 satdigitalinvoice-3.0.1/satdigitalinvoice/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-04-15 21:41:41.000000 satdigitalinvoice-3.0.1/satdigitalinvoice/localdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-15 21:41:41.000000 satdigitalinvoice-3.0.1/satdigitalinvoice/log_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 21:41:52.203517 satdigitalinvoice-3.0.1/satdigitalinvoice/markdown_styles/
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-15 21:41:41.000000 satdigitalinvoice-3.0.1/satdigitalinvoice/markdown_styles/markdown6.css
+-rw-r--r--   0 runner    (1001) docker     (123)     5694 2023-04-15 21:41:41.000000 satdigitalinvoice-3.0.1/satdigitalinvoice/mycfdi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 21:41:52.207517 satdigitalinvoice-3.0.1/satdigitalinvoice/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-15 21:41:41.000000 satdigitalinvoice-3.0.1/satdigitalinvoice/schemas/cliente.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-15 21:41:41.000000 satdigitalinvoice-3.0.1/satdigitalinvoice/schemas/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-15 21:41:41.000000 satdigitalinvoice-3.0.1/satdigitalinvoice/schemas/factura.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-04-15 21:41:41.000000 satdigitalinvoice-3.0.1/satdigitalinvoice/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 21:41:52.203517 satdigitalinvoice-3.0.1/satdigitalinvoice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-15 21:41:52.000000 satdigitalinvoice-3.0.1/satdigitalinvoice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-15 21:41:52.000000 satdigitalinvoice-3.0.1/satdigitalinvoice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 21:41:52.000000 satdigitalinvoice-3.0.1/satdigitalinvoice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-15 21:41:52.000000 satdigitalinvoice-3.0.1/satdigitalinvoice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-15 21:41:52.000000 satdigitalinvoice-3.0.1/satdigitalinvoice.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 21:41:52.207517 satdigitalinvoice-3.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-04-15 21:41:41.000000 satdigitalinvoice-3.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 21:41:52.207517 satdigitalinvoice-3.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-15 21:41:41.000000 satdigitalinvoice-3.0.1/tests/test_clients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6276 2023-04-15 21:41:41.000000 satdigitalinvoice-3.0.1/tests/test_crear_facturas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-04-15 21:41:41.000000 satdigitalinvoice-3.0.1/tests/test_localdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-04-15 21:41:41.000000 satdigitalinvoice-3.0.1/tests/test_main.py
```

### Comparing `satdigitalinvoice-3.0.0/PKG-INFO` & `satdigitalinvoice-3.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satdigitalinvoice
-Version: 3.0.0
+Version: 3.0.1
 Summary: GUI APP to Generate CFDI
 Home-page: https://github.com/SAT-CFDI/python-satdigitalinvoice
 Author: satcfdi@outlook.com
 Author-email: satcfdi@outlook.com
 License: MIT License
 Project-URL: Documentation, https://satdigitalinvoice.readthedocs.io
 Project-URL: Source, https://github.com/SAT-CFDI/python-satdigitalinvoice
```

### Comparing `satdigitalinvoice-3.0.0/satdigitalinvoice/__init__.py` & `satdigitalinvoice-3.0.1/satdigitalinvoice/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import logging
 import os
 import sys
-
+from zipfile import ZipFile
 import PySimpleGUI as sg
 
 SOURCE_DIRECTORY = os.path.dirname(__file__)
+
 DATA_DIRECTORY = ".data"
 ARCHIVOS_DIRECTORY = "archivos"
 TEMPLATES_DIRECTORY = "templates"
 TEMP_DIRECTORY = ".data/temp"
 
 PPD = "PPD"
 PUE = "PUE"
@@ -25,23 +26,38 @@
     formatter = logging.Formatter('%(asctime)s - %(message)s')
     fh.setFormatter(formatter)
     logging.root.addHandler(fh)
 
 
 class FacturacionLauncher:
 
-    def __init__(self, debug=False):
+    def __init__(self, cwd=None, debug=False):
+        app_dir = os.getcwd()
+
+        if cwd:
+            os.chdir(cwd)
+
         # set up logging
         if debug:
             logging.basicConfig(
                 level=logging.DEBUG,
                 stream=sys.stderr,
             )
         add_file_handler()
 
+        # loading the sample.zip
+        try:
+            with ZipFile(os.path.join(app_dir, 'sample.zip'), 'r') as zf:
+                for member in zf.infolist():
+                    if not os.path.exists(member.filename):
+                        zf.extract(member)
+        except FileNotFoundError:
+            pass
+
+        # layout
         layout = [
             [sg.Column([[
                 sg.Image(source=os.path.join(SOURCE_DIRECTORY, "images", "logo.png"), pad=2),
             ]], justification='center', pad=0, background_color='black')],
             [
                 sg.Multiline(
                     "Cargando Aplicación...",
@@ -54,22 +70,22 @@
                     write_only=True,
                     disabled=True,
                 )
             ]
         ]
 
         self.window = sg.Window(
-            f"Facturación Masiva CFDI 4.0",  # {self.csd_signer.rfc}
+            f"Facturación Masiva CFDI 4.0",
             layout,
             size=(640, 480),
             resizable=True,
             font=("Courier New", 11, "bold"),
             no_titlebar=True,
             modal=True,
-            background_color='#a0dbd9', # sg.theme_background_color(),
+            background_color='#a0dbd9',  # sg.theme_background_color(),
             auto_close=True,
             auto_close_duration=10,  # seconds
         )
 
     @staticmethod
     def read_config():
         from satdigitalinvoice.file_data_managers import ConfigManager
@@ -82,15 +98,15 @@
         try:
             from satdigitalinvoice.facturacion import FacturacionGUI
             config = self.read_config()
             app = FacturacionGUI(config)
         except Exception as ex:
             logging.exception(ex)
             self.window['console'].update(
-               f"Error al cargar la aplicación. {ex.__class__.__name__}: {ex}",
+                f"Error al cargar la aplicación. {ex.__class__.__name__}: {ex}",
                 text_color='red4',
             )
             self.window.read()
             self.window.close()
             return
 
         self.window.close()
```

### Comparing `satdigitalinvoice-3.0.0/satdigitalinvoice/__version__.py` & `satdigitalinvoice-3.0.1/satdigitalinvoice/__version__.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-3.0.0/satdigitalinvoice/client_validation.py` & `satdigitalinvoice-3.0.1/satdigitalinvoice/client_validation.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-3.0.0/satdigitalinvoice/environments.py` & `satdigitalinvoice-3.0.1/satdigitalinvoice/environments.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-3.0.0/satdigitalinvoice/facturacion.py` & `satdigitalinvoice-3.0.1/satdigitalinvoice/facturacion.py`

 * *Files 0% similar despite different names*

```diff
@@ -429,17 +429,18 @@
                         if values['main_tab_group'] == 'console_tab':
                             self.action_button_manager.clear()
 
                         if values['main_tab_group'] == 'recuperar_tab':
                             self.action_button_manager.clear()
 
                         if values['main_tab_group'] == 'facturas_tab':
+                            self.window['facturas_table'].update(values=[])
+
                             if dp is None or dp.month is None:
                                 self.window['preparar_facturas_text'].update("Periodo no válido")
-                                self.window['facturas_table'].update(values=[])
                                 continue
 
                             self.window['preparar_facturas_text'].update(f"{period_desc(dp)}")
                             self.console.update("")
                             cfdis = generate_ingresos(
                                 clients=ClientsManager(),
                                 facturas=FacturasManager(dp)["Facturas"],
@@ -464,14 +465,15 @@
                             self.window['facturas_table'].update(
                                 values=rows,
                             )
                             self.window['facturas_table'].metadata = cfdis
                             self.action_button_manager.set_items('facturas', cfdis)
 
                         if values['main_tab_group'] == 'clients_tab':
+                            self.window['clientes_table'].update(values=[])
                             clients = list(ClientsManager().values())
                             facturas = FacturasManager(dp)["Facturas"]
                             rows = [
                                 [
                                     i,
                                     client["RazonSocial"][:36],
                                     client["Rfc"],
@@ -759,14 +761,29 @@
 
                     case "ver_carpeta":
                         directory = archivos_folder(dp)
                         os.startfile(
                             os.path.abspath(directory)
                         )
 
+                    case "ver_config":
+                        os.startfile(
+                            os.path.abspath(".")
+                        )
+
+                    case "editar_clientes":
+                        os.startfile(
+                            os.path.abspath("clientes.yaml")
+                        )
+
+                    case "editar_facturas":
+                        os.startfile(
+                            os.path.abspath("facturas.yaml")
+                        )
+
                     case "sat_status_todas":
                         def fact_iter():
                             for i in self.get_all_invoices().values():
                                 if i["Fecha"] == dp:
                                     yield i
 
                         for cfdi in fact_iter():
@@ -779,17 +796,16 @@
                     case "periodo" | "inicio" | "final" | "fecha_pago" | "forma_pago" | "importe_pago" | ' ':
                         pass
 
                     case _:
                         logger.error(f"Unknown event '{event}'")
 
             except Exception as ex:
-                if values['main_tab_group'] == 'console_tab':
-                    logger.exception(header_line("ERROR"))
-                else:
+                logger.exception(header_line("ERROR"))
+                if values['main_tab_group'] != 'console_tab':
                     PySimpleGUI.Popup(
                         ex,
                         no_titlebar=True,
                         grab_anywhere=True,
                         any_key_closes=True,
                         background_color="red4",
                     )
```

### Comparing `satdigitalinvoice-3.0.0/satdigitalinvoice/file_data_managers.py` & `satdigitalinvoice-3.0.1/satdigitalinvoice/file_data_managers.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-3.0.0/satdigitalinvoice/formatting_functions/common.py` & `satdigitalinvoice-3.0.1/satdigitalinvoice/formatting_functions/common.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-3.0.0/satdigitalinvoice/gui_functions.py` & `satdigitalinvoice-3.0.1/satdigitalinvoice/gui_functions.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-3.0.0/satdigitalinvoice/images/logo.png` & `satdigitalinvoice-3.0.1/satdigitalinvoice/images/logo.png`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-3.0.0/satdigitalinvoice/layout.py` & `satdigitalinvoice-3.0.1/satdigitalinvoice/layout.py`

 * *Files 7% similar despite different names*

```diff
@@ -44,21 +44,30 @@
                "+FYhixdADniTzvSRUQDeVXSsNiwUJ+ItbzpnpICy2vAhA4v2bLzl//ALOtSCJzC7jH4AAAAASUVORK5CYII="
 
 SEARCH_ICON = "iVBORw0KGgoAAAANSUhEUgAAABgAAAAYCAYAAADgdz34AAAACXBIWXMAAAsTAAALEwEAmpwYAAABM0lEQVR4nOXTuytAYRzG8Y8RJTPJ5jJIitwGoxiZGSTZDAaDTQaJhYWBf0A" \
               "WRDHjD7BIMrkUg2wol079lEGc1yXJU2c4b8/5Pu/vfZ/Df1MjJrGKLSyjHyVfBZdjE0+4wwH2cB5rVxj8LLwmQNcYeWO3TdiOoJlUeDGOcIbqd3wFmI2QgZSAcTyiPYc3C9nBZcq" \
               "dnGAjYUPNMUVfHnNlmIcSArIpLrCUx9wSAZ3StB8V/lD1EdCTGJBVeCVvg+4wlQAvxT0m8n6wERUtyukfjakb8ga04QELOby1uMGaxFbsxq4W49jeUke05xRlKfD5gO/GJBlkGr3" \
               "ownA0JvsZD1H1Gfh8vLdiHbex/vIcYwyFX4G/VnbhdRFYIVEZbO7VmRekAn4Nnqn7nWP5NnX9JNyf1DM+Yku7BVpvYgAAAABJRU5ErkJggg=="
 
+CONFIG_ICON = "iVBORw0KGgoAAAANSUhEUgAAABgAAAAYCAYAAADgdz34AAAACXBIWXMAAAsTAAALEwEAmpwYAAABPElEQVR4nOWVvWoCQRSFP5NCSJHOdGkECaa3s" \
+              "/MtUu6CYOcTaGMZU2efwNYtrKwkWPgK9nmAEC38IRMGTmCZrIMru6B44MLOmXPP7N6ZvQPXgiowdcJyueEFMMBMYcTlhjfgG7hR2OfhqWYB0AEqQBnoA1/APKGZi" \
+              "+tLU1GOzfXiEVirBDvgE9gA70A9oauL20izU85aHgcxAlZACxgAH0DDo29IM1DOSh6paAI/QJQyVwJCIFaE4lxE8rBe//AALIA90HbMY5VgqTDikou0lbuQVyrugIkMnsSFGttN/ENHnJ1DWqNc6+FFV" \
+              "+J7jWO9tYul5pDWKJc8FxhnXSBriQKNa8eUqPBNbh5xTMeK4JRjWviP5msVkdMqnsVts7aKtGbX8zS7XtZmdwhDff5tol2/ckkXTrXoK/N88Qvnr38CSEQRlwAAAABJRU5ErkJggg=="
+
+EDIT_ICON = "iVBORw0KGgoAAAANSUhEUgAAABgAAAAYCAYAAADgdz34AAAACXBIWXMAAAsTAAALEwEAmpwYAAAA10lEQVR4nO3UPUpDQRSG4cfCQgn" \
+            "+LSPLSCcEC1u3EXdgEXdg3EC2IXYS0N4itZWWGkGvDHyBkE45Npq3usyB95tz5s6w4ZfZwwQveMIFtqvkB5jhDZe4xmdCyuQdxivrk3RSIl/gAe84Ta118oytCvkQPdwmZJxxXVXJl/TSSZd6O/hvs4+7yE" \
+            "/Wasd4xT2ONvIl/3gsuys3dLRWGyZ0ll/2RwwiX2SnZ5XyxnkerD5uEjKqkjemmOe7H3FXJW885rGaR9xVyg/xkZBpxjXIwZewU7VTf4ovf6VSMafchm4AAAAASUVORK5CYII="
 
 BUTTON_COLOR = (sg.theme_background_color(), sg.theme_background_color())
 
 
 def make_layout(has_fiel):
     # LAYOUT
     button_column = [
+        sg.Button(image_data=CONFIG_ICON, key="ver_config", border_width=0, button_color=BUTTON_COLOR),
         sg.Text("Periodo:", pad=TEXT_PADDING),
         sg.Input(date.today().strftime('%Y-%m'), size=(11, 1), key="periodo"),
         sg.Button(image_data=FOLDER_ICON, key="ver_carpeta", border_width=0, button_color=BUTTON_COLOR),
         sg.Button(image_data=EXCEL_ICON, key="ver_excel", border_width=0, button_color=BUTTON_COLOR),
         sg.Button(image_data=HTML_ICON, key="ver_html", border_width=0, button_color=BUTTON_COLOR),
 
         sg.Push(),
@@ -89,71 +98,75 @@
                                 autoscroll=True,
                                 reroute_stdout=True
                             )]
                         ],
                         key='console_tab',
                     ),
                     sg.Tab(
-                        'Facturas'.center(13),
+                        'Clientes'.center(13),
                         [
                             [
-                                sg.Button("Refrescar", key="refresh_facturas", border_width=0, ),
-                                sg.Text("", pad=TEXT_PADDING, key="preparar_facturas_text"),
+                                sg.Button("Refrescar", key="refresh_clientes", border_width=0),
+                                sg.Push(),
+                                sg.Button(image_data=EDIT_ICON, key="editar_clientes", border_width=0, button_color=BUTTON_COLOR),
                             ],
                             [
                                 sg.Table(
                                     values=[],
                                     headings=[
-                                        '#',
-                                        'EReg',
-                                        'Receptor Razon Social',
-                                        'Recep. Rfc',
-                                        "Tipo",
-                                        "Subtotal",
-                                        "Total"
+                                        "#",
+                                        "Razon Social",
+                                        "Rfc",
+                                        "Reg",
+                                        "CP",
+                                        "Facturas",
                                     ],
-                                    key="facturas_table",
+                                    key="clientes_table",
                                     expand_x=True,
                                     expand_y=True,
                                     select_mode=sg.TABLE_SELECT_MODE_EXTENDED,
                                     enable_events=True,
                                     text_color="black",
                                     background_color="white",
+                                    def_col_width=10,
                                 )
                             ]],
-                        key='facturas_tab',
+                        key='clients_tab',
                     ),
                     sg.Tab(
-                        'Clientes'.center(13),
+                        'Facturas'.center(13),
                         [
                             [
-                                sg.Button("Refrescar", key="refresh_clientes", border_width=0, ),
+                                sg.Button("Refrescar", key="refresh_facturas", border_width=0, ),
+                                sg.Text("", pad=TEXT_PADDING, key="preparar_facturas_text"),
+                                sg.Push(),
+                                sg.Button(image_data=EDIT_ICON, key="editar_facturas", border_width=0, button_color=BUTTON_COLOR),
                             ],
                             [
                                 sg.Table(
                                     values=[],
                                     headings=[
-                                        "#",
-                                        "Razon Social",
-                                        "Rfc",
-                                        "Reg",
-                                        "CP",
-                                        "Facturas",
+                                        '#',
+                                        'EReg',
+                                        'Receptor Razon Social',
+                                        'Recep. Rfc',
+                                        "Tipo",
+                                        "Subtotal",
+                                        "Total"
                                     ],
-                                    key="clientes_table",
+                                    key="facturas_table",
                                     expand_x=True,
                                     expand_y=True,
                                     select_mode=sg.TABLE_SELECT_MODE_EXTENDED,
                                     enable_events=True,
                                     text_color="black",
                                     background_color="white",
-                                    def_col_width=10,
                                 )
                             ]],
-                        key='clients_tab',
+                        key='facturas_tab',
                     ),
                     sg.Tab(
                         'Emitidas'.center(13),
                         [
                             [
                                 sg.Button("Pendientes", key="facturas_pendientes", border_width=0),
                                 sg.Button("Todas", key="facturas_emitidas", border_width=0),
```

### Comparing `satdigitalinvoice-3.0.0/satdigitalinvoice/localdb.py` & `satdigitalinvoice-3.0.1/satdigitalinvoice/localdb.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-3.0.0/satdigitalinvoice/log_tools.py` & `satdigitalinvoice-3.0.1/satdigitalinvoice/log_tools.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-3.0.0/satdigitalinvoice/markdown_styles/markdown6.css` & `satdigitalinvoice-3.0.1/satdigitalinvoice/markdown_styles/markdown6.css`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-3.0.0/satdigitalinvoice/mycfdi.py` & `satdigitalinvoice-3.0.1/satdigitalinvoice/mycfdi.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-3.0.0/satdigitalinvoice/schemas/factura.yaml` & `satdigitalinvoice-3.0.1/satdigitalinvoice/schemas/factura.yaml`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-3.0.0/satdigitalinvoice/utils.py` & `satdigitalinvoice-3.0.1/satdigitalinvoice/utils.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-3.0.0/satdigitalinvoice.egg-info/PKG-INFO` & `satdigitalinvoice-3.0.1/satdigitalinvoice.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satdigitalinvoice
-Version: 3.0.0
+Version: 3.0.1
 Summary: GUI APP to Generate CFDI
 Home-page: https://github.com/SAT-CFDI/python-satdigitalinvoice
 Author: satcfdi@outlook.com
 Author-email: satcfdi@outlook.com
 License: MIT License
 Project-URL: Documentation, https://satdigitalinvoice.readthedocs.io
 Project-URL: Source, https://github.com/SAT-CFDI/python-satdigitalinvoice
```

### Comparing `satdigitalinvoice-3.0.0/satdigitalinvoice.egg-info/SOURCES.txt` & `satdigitalinvoice-3.0.1/satdigitalinvoice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-3.0.0/setup.py` & `satdigitalinvoice-3.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-3.0.0/tests/test_crear_facturas.py` & `satdigitalinvoice-3.0.1/tests/test_crear_facturas.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-3.0.0/tests/test_localdb.py` & `satdigitalinvoice-3.0.1/tests/test_localdb.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-3.0.0/tests/test_main.py` & `satdigitalinvoice-3.0.1/tests/test_main.py`

 * *Files identical despite different names*

