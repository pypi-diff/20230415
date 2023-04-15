# Comparing `tmp/satdigitalinvoice-2.2.0.tar.gz` & `tmp/satdigitalinvoice-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satdigitalinvoice-2.2.0.tar", last modified: Wed Apr 12 02:20:04 2023, max compression
+gzip compressed data, was "satdigitalinvoice-3.0.0.tar", last modified: Sat Apr 15 08:01:33 2023, max compression
```

## Comparing `satdigitalinvoice-2.2.0.tar` & `satdigitalinvoice-3.0.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 02:20:04.191590 satdigitalinvoice-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-12 02:20:04.191590 satdigitalinvoice-2.2.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 02:20:04.187590 satdigitalinvoice-2.2.0/satdigitalinvoice/
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-04-12 02:19:49.000000 satdigitalinvoice-2.2.0/satdigitalinvoice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-12 02:19:49.000000 satdigitalinvoice-2.2.0/satdigitalinvoice/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-04-12 02:19:49.000000 satdigitalinvoice-2.2.0/satdigitalinvoice/client_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-04-12 02:19:49.000000 satdigitalinvoice-2.2.0/satdigitalinvoice/environments.py
--rw-r--r--   0 runner    (1001) docker     (123)    31866 2023-04-12 02:19:49.000000 satdigitalinvoice-2.2.0/satdigitalinvoice/facturacion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-04-12 02:19:49.000000 satdigitalinvoice-2.2.0/satdigitalinvoice/file_data_managers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 02:20:04.187590 satdigitalinvoice-2.2.0/satdigitalinvoice/formatting_functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 02:19:49.000000 satdigitalinvoice-2.2.0/satdigitalinvoice/formatting_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-04-12 02:19:49.000000 satdigitalinvoice-2.2.0/satdigitalinvoice/formatting_functions/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    17445 2023-04-12 02:19:49.000000 satdigitalinvoice-2.2.0/satdigitalinvoice/gui_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 02:20:04.191590 satdigitalinvoice-2.2.0/satdigitalinvoice/images/
--rw-r--r--   0 runner    (1001) docker     (123)    71867 2023-04-12 02:19:49.000000 satdigitalinvoice-2.2.0/satdigitalinvoice/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     9864 2023-04-12 02:19:49.000000 satdigitalinvoice-2.2.0/satdigitalinvoice/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-04-12 02:19:49.000000 satdigitalinvoice-2.2.0/satdigitalinvoice/localdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-12 02:19:49.000000 satdigitalinvoice-2.2.0/satdigitalinvoice/log_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 02:20:04.191590 satdigitalinvoice-2.2.0/satdigitalinvoice/markdown_styles/
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-12 02:19:49.000000 satdigitalinvoice-2.2.0/satdigitalinvoice/markdown_styles/markdown6.css
--rw-r--r--   0 runner    (1001) docker     (123)     5694 2023-04-12 02:19:49.000000 satdigitalinvoice-2.2.0/satdigitalinvoice/mycfdi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 02:20:04.191590 satdigitalinvoice-2.2.0/satdigitalinvoice/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-12 02:19:49.000000 satdigitalinvoice-2.2.0/satdigitalinvoice/schemas/cliente.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-12 02:19:49.000000 satdigitalinvoice-2.2.0/satdigitalinvoice/schemas/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-12 02:19:49.000000 satdigitalinvoice-2.2.0/satdigitalinvoice/schemas/factura.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-04-12 02:19:49.000000 satdigitalinvoice-2.2.0/satdigitalinvoice/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 02:20:04.187590 satdigitalinvoice-2.2.0/satdigitalinvoice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-12 02:20:04.000000 satdigitalinvoice-2.2.0/satdigitalinvoice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-12 02:20:04.000000 satdigitalinvoice-2.2.0/satdigitalinvoice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 02:20:04.000000 satdigitalinvoice-2.2.0/satdigitalinvoice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-12 02:20:04.000000 satdigitalinvoice-2.2.0/satdigitalinvoice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-12 02:20:04.000000 satdigitalinvoice-2.2.0/satdigitalinvoice.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 02:20:04.191590 satdigitalinvoice-2.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-04-12 02:19:49.000000 satdigitalinvoice-2.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 02:20:04.191590 satdigitalinvoice-2.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-12 02:19:49.000000 satdigitalinvoice-2.2.0/tests/test_clients.py
--rw-r--r--   0 runner    (1001) docker     (123)     6298 2023-04-12 02:19:49.000000 satdigitalinvoice-2.2.0/tests/test_crear_facturas.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-04-12 02:19:49.000000 satdigitalinvoice-2.2.0/tests/test_localdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-04-12 02:19:49.000000 satdigitalinvoice-2.2.0/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:01:33.598478 satdigitalinvoice-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-15 08:01:33.598478 satdigitalinvoice-3.0.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:01:33.598478 satdigitalinvoice-3.0.0/satdigitalinvoice/
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-04-15 08:01:23.000000 satdigitalinvoice-3.0.0/satdigitalinvoice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-15 08:01:23.000000 satdigitalinvoice-3.0.0/satdigitalinvoice/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-04-15 08:01:23.000000 satdigitalinvoice-3.0.0/satdigitalinvoice/client_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-15 08:01:23.000000 satdigitalinvoice-3.0.0/satdigitalinvoice/environments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36499 2023-04-15 08:01:23.000000 satdigitalinvoice-3.0.0/satdigitalinvoice/facturacion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4762 2023-04-15 08:01:23.000000 satdigitalinvoice-3.0.0/satdigitalinvoice/file_data_managers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:01:33.598478 satdigitalinvoice-3.0.0/satdigitalinvoice/formatting_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 08:01:23.000000 satdigitalinvoice-3.0.0/satdigitalinvoice/formatting_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-04-15 08:01:23.000000 satdigitalinvoice-3.0.0/satdigitalinvoice/formatting_functions/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10761 2023-04-15 08:01:23.000000 satdigitalinvoice-3.0.0/satdigitalinvoice/gui_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:01:33.598478 satdigitalinvoice-3.0.0/satdigitalinvoice/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    71867 2023-04-15 08:01:23.000000 satdigitalinvoice-3.0.0/satdigitalinvoice/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    17581 2023-04-15 08:01:23.000000 satdigitalinvoice-3.0.0/satdigitalinvoice/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-04-15 08:01:23.000000 satdigitalinvoice-3.0.0/satdigitalinvoice/localdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-15 08:01:23.000000 satdigitalinvoice-3.0.0/satdigitalinvoice/log_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:01:33.598478 satdigitalinvoice-3.0.0/satdigitalinvoice/markdown_styles/
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-15 08:01:23.000000 satdigitalinvoice-3.0.0/satdigitalinvoice/markdown_styles/markdown6.css
+-rw-r--r--   0 runner    (1001) docker     (123)     5694 2023-04-15 08:01:23.000000 satdigitalinvoice-3.0.0/satdigitalinvoice/mycfdi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:01:33.598478 satdigitalinvoice-3.0.0/satdigitalinvoice/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-15 08:01:23.000000 satdigitalinvoice-3.0.0/satdigitalinvoice/schemas/cliente.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-15 08:01:23.000000 satdigitalinvoice-3.0.0/satdigitalinvoice/schemas/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-15 08:01:23.000000 satdigitalinvoice-3.0.0/satdigitalinvoice/schemas/factura.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-04-15 08:01:23.000000 satdigitalinvoice-3.0.0/satdigitalinvoice/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:01:33.598478 satdigitalinvoice-3.0.0/satdigitalinvoice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-15 08:01:33.000000 satdigitalinvoice-3.0.0/satdigitalinvoice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-15 08:01:33.000000 satdigitalinvoice-3.0.0/satdigitalinvoice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 08:01:33.000000 satdigitalinvoice-3.0.0/satdigitalinvoice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-15 08:01:33.000000 satdigitalinvoice-3.0.0/satdigitalinvoice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-15 08:01:33.000000 satdigitalinvoice-3.0.0/satdigitalinvoice.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 08:01:33.598478 satdigitalinvoice-3.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-04-15 08:01:23.000000 satdigitalinvoice-3.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 08:01:33.598478 satdigitalinvoice-3.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-15 08:01:23.000000 satdigitalinvoice-3.0.0/tests/test_clients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6276 2023-04-15 08:01:23.000000 satdigitalinvoice-3.0.0/tests/test_crear_facturas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-04-15 08:01:23.000000 satdigitalinvoice-3.0.0/tests/test_localdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-04-15 08:01:23.000000 satdigitalinvoice-3.0.0/tests/test_main.py
```

### Comparing `satdigitalinvoice-2.2.0/PKG-INFO` & `satdigitalinvoice-3.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satdigitalinvoice
-Version: 2.2.0
+Version: 3.0.0
 Summary: GUI APP to Generate CFDI
 Home-page: https://github.com/SAT-CFDI/python-satdigitalinvoice
 Author: satcfdi@outlook.com
 Author-email: satcfdi@outlook.com
 License: MIT License
 Project-URL: Documentation, https://satdigitalinvoice.readthedocs.io
 Project-URL: Source, https://github.com/SAT-CFDI/python-satdigitalinvoice
```

### Comparing `satdigitalinvoice-2.2.0/satdigitalinvoice/__init__.py` & `satdigitalinvoice-3.0.0/satdigitalinvoice/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import logging
 import os
+import sys
 
 import PySimpleGUI as sg
 
 SOURCE_DIRECTORY = os.path.dirname(__file__)
 DATA_DIRECTORY = ".data"
 ARCHIVOS_DIRECTORY = "archivos"
 TEMPLATES_DIRECTORY = "templates"
+TEMP_DIRECTORY = ".data/temp"
 
 PPD = "PPD"
 PUE = "PUE"
 
 
 def add_file_handler():
     os.makedirs(DATA_DIRECTORY, exist_ok=True)
@@ -26,15 +28,18 @@
 
 
 class FacturacionLauncher:
 
     def __init__(self, debug=False):
         # set up logging
         if debug:
-            logging.basicConfig(level=logging.ERROR)
+            logging.basicConfig(
+                level=logging.DEBUG,
+                stream=sys.stderr,
+            )
         add_file_handler()
 
         layout = [
             [sg.Column([[
                 sg.Image(source=os.path.join(SOURCE_DIRECTORY, "images", "logo.png"), pad=2),
             ]], justification='center', pad=0, background_color='black')],
             [
```

### Comparing `satdigitalinvoice-2.2.0/satdigitalinvoice/__version__.py` & `satdigitalinvoice-3.0.0/satdigitalinvoice/__version__.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.2.0/satdigitalinvoice/client_validation.py` & `satdigitalinvoice-3.0.0/satdigitalinvoice/client_validation.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,48 +10,49 @@
 sat_service = SAT()
 logger = logging.getLogger(__name__)
 warnings.filterwarnings("ignore", category=XMLParsedAsHTMLWarning)
 
 EMAIL_REGEX = r'\b[A-Za-z0-9._%+-]+@[A-Za-z0-9.-]+\.[A-Z|a-z]{2,7}\b'
 
 
-def validar_client(rfc, details):
+def validar_client(client):
+    rfc = client['Rfc']
     try:
         rfc = RFC(rfc)
         if not rfc.is_valid():
             raise ValueError("RFC Not Valid Regex")
     except ValueError as ex:
         logger.info(f"{rfc}: {ex}")
         return
 
-    for email in details["Email"]:
+    for email in client["Email"]:
         match = re.fullmatch(EMAIL_REGEX, email)
         if not match:
             logger.info(f"{rfc}: Correo '{email}' is invalid")
 
-    if id_cif := details["IdCIF"]:
+    if id_cif := client["IdCIF"]:
         try:
             res = csf.retrieve(rfc, id_cif=id_cif)
         except ValueError as ex:
             logger.info(f"{rfc}: idCIF '{id_cif}' is invalid")
             return
 
         if rfc.type == RFCType.MORAL:
-            if details['RazonSocial'] != res['Denominación o Razón Social']:
-                logger.info(f"{rfc}: RazonSocial '{details['RazonSocial']}' is invalid, expected '{res['Denominación o Razón Social']}'")
+            if client['RazonSocial'] != res['Denominación o Razón Social']:
+                logger.info(f"{rfc}: RazonSocial '{client['RazonSocial']}' is invalid, expected '{res['Denominación o Razón Social']}'")
         elif rfc.type == RFCType.FISICA:
-            if details['RazonSocial'] != f"{res['Nombre']} {res['Apellido Paterno']} {res['Apellido Materno']}":
-                logger.info(f"{rfc}: RazonSocial '{details['RazonSocial']}' is invalid, expected '{res['Nombre']} {res['Apellido Paterno']} {res['Apellido Materno']}'")
+            if client['RazonSocial'] != f"{res['Nombre']} {res['Apellido Paterno']} {res['Apellido Materno']}":
+                logger.info(f"{rfc}: RazonSocial '{client['RazonSocial']}' is invalid, expected '{res['Nombre']} {res['Apellido Paterno']} {res['Apellido Materno']}'")
 
-        if details['CodigoPostal'] != res['CP']:
-            logger.info(f"{rfc}: CodigoPostal '{details['CodigoPostal']}' is invalid, expected '{res['CP']}'")
+        if client['CodigoPostal'] != res['CP']:
+            logger.info(f"{rfc}: CodigoPostal '{client['CodigoPostal']}' is invalid, expected '{res['CP']}'")
 
-        if details['RegimenFiscal'] not in (r['RegimenFiscal'] for r in res['Regimenes']):
+        if client['RegimenFiscal'] not in (r['RegimenFiscal'] for r in res['Regimenes']):
             logger.info(
-                f"{rfc}: RegimenFiscal '{details['RegimenFiscal']}' is invalid, "
+                f"{rfc}: RegimenFiscal '{client['RegimenFiscal']}' is invalid, "
                 f"expected '{(r['RegimenFiscal'].code for r in res['Regimenes'])}'"
             )
 
         if res['Situación del contribuyente'] not in ['ACTIVO', 'REACTIVADO']:
             logger.info(f"{rfc}: Is not ACTIVO '{res['Situación del contribuyente']}'")
 
         taxpayer_status = sat_service.list_69b(rfc)
```

### Comparing `satdigitalinvoice-2.2.0/satdigitalinvoice/environments.py` & `satdigitalinvoice-3.0.0/satdigitalinvoice/environments.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import jinja2
 from jinja2 import Environment, Undefined
 from jinja2.filters import do_mark_safe
 # noinspection PyUnresolvedReferences
 from satcfdi.transform.catalog import CATALOGS
 from satcfdi.transform.helpers import iterate as h_iterate
 
-from satdigitalinvoice import TEMPLATES_DIRECTORY
+from . import TEMPLATES_DIRECTORY
 
 
 class FacturacionEnvironment(Environment):
     @property
     def filter(self):
         def sub(f):
             self.filters[f.__name__] = f
@@ -45,12 +45,12 @@
         @self.filter
         def bold(k):
             return do_mark_safe(
                 tag(html_escape(k), "b")
             )
 
 
-facturacion_environment = FacturacionEnvironment()
-
-
 def tag(text, tag):
     return '<' + tag + '>' + text + '</' + tag + '>'
+
+
+facturacion_environment = FacturacionEnvironment()
```

### Comparing `satdigitalinvoice-2.2.0/satdigitalinvoice/facturacion.py` & `satdigitalinvoice-3.0.0/satdigitalinvoice/facturacion.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,57 +3,54 @@
 import itertools
 import logging
 import os
 from datetime import timedelta, date
 from zipfile import ZipFile
 
 from PySimpleGUI import POPUP_BUTTONS_OK_CANCEL, PySimpleGUI
-from satcfdi import DatePeriod
+from satcfdi import DatePeriod, csf
 from satcfdi.accounting import EmailManager
-from satcfdi.exceptions import ResponseError, DocumentNotFoundError
+from satcfdi.create.cfd import cfdi40
+from satcfdi.exceptions import ResponseError
 from satcfdi.pacs import Accept
 from satcfdi.pacs.sat import SAT, TipoDescargaMasivaTerceros, EstadoSolicitud
 from satcfdi.printer import Representable
 # noinspection PyUnresolvedReferences
 from satcfdi.transform.catalog import CATALOGS
-from tabulate import tabulate
 
-from . import __version__, PPD, PUE
+from . import __version__, PPD, PUE, TEMP_DIRECTORY
 from .client_validation import validar_client
+from .environments import facturacion_environment
 from .file_data_managers import ClientsManager, FacturasManager
-from .gui_functions import generate_ingresos, pago_factura, exportar_facturas, facturas_filename, \
-    generate_html_template, mf_pago_fmt, print_invoices, print_cfdis, print_cfdi_details, ajustes, facturas_folder, year_month_desc
+from .formatting_functions.common import fecha, pesos, porcentaje
+from .gui_functions import generate_ingresos, pago_factura, exportar_facturas, archivos_filename, mf_pago_fmt, archivos_folder, period_desc, ajustes_directory, find_ajustes, \
+    format_concepto_desc, generate_pdf_template, periodicidad_desc, parse_fecha_pago, parse_importe_pago, preview_cfdis
 from .layout import make_layout, ActionButtonManager
 from .localdb import LocalDBSatCFDI, LiquidatedState
-from .log_tools import log_line, log_item, cfdi_header, header_line, print_yaml
+from .log_tools import cfdi_header, header_line, print_yaml
 from .mycfdi import get_all_cfdi, MyCFDI, move_to_folder
-from .utils import random_string, to_uuid, parse_date_period, load_certificate, to_int, cert_info, parse_rango
+from .utils import random_string, parse_date_period, load_certificate, to_int, cert_info, add_month, clear_directory, find_best_match, months_between
 
 logging.getLogger("weasyprint").setLevel(logging.ERROR)
 logging.getLogger("fontTools").setLevel(logging.ERROR)
 
 logger = logging.getLogger(__name__)
-logger.setLevel(logging.INFO)
-
-ACTION_FACTURAS = "facturas"
-ACTION_EMAILS = "emails"
-ACTION_CLIENTS = "clients"
-ACTION_AJUSTES = "ajustes"
 
 
 def open_launch_window():
     layout = [[PySimpleGUI.Text("New Window", key="new")]]
     window = PySimpleGUI.Window("Launch Window", layout, modal=True, size=(300, 300))
     window.read(timeout=1000)
 
     return window
 
 
 class FacturacionGUI:
     def __init__(self, config):
+        os.makedirs(TEMP_DIRECTORY, exist_ok=True)
         self.email_manager = EmailManager(
             **config['email']
         )
         pac = config['pac']
         pac_module, pac_class = pac['type'].split(".")
         mod = __import__(f"satcfdi.pacs.{pac_module}", fromlist=[pac_class])
         self.pac_service = getattr(mod, pac_class)(
@@ -63,15 +60,15 @@
         self.csd_signer = load_certificate(config.get('csd')) if 'csd' in config else None
         self.fiel_signer = load_certificate(config.get('fiel')) if 'fiel' in config else None
 
         self.sat_service = SAT(signer=self.fiel_signer)
         self.rfc_prediales = config['rfc_prediales']
 
         self.window = PySimpleGUI.Window(
-            f"Facturación Masiva CFDI 4.0 {self.csd_signer.rfc}",
+            f"Facturación Mensual CFDI 4.0 {self.csd_signer.rfc}",
             make_layout(bool(self.fiel_signer)),
             size=(1280, 800),
             resizable=True,
             font=("Courier New", 10, "bold"),
         )
 
         self.all_invoices = None
@@ -89,21 +86,24 @@
 
     def run(self):
         self.window.finalize()
 
         self.set_folio()
         self.window['serie'].update(self.serie)
 
-        self.window['factura_pagar'].bind("<Return>", "_enter")
         self.window['periodo'].bind("<Return>", "_enter")
         self.window['importe_pago'].bind("<Return>", "_enter")
         self.window['fecha_pago'].bind("<Return>", "_enter")
-        self.window['rango'].bind("<Return>", "_enter")
         self.window['forma_pago'].bind("<Return>", "_enter")
-        # self.window['console'].bind('<Button-3>', '_double_click')
+        self.window['emitidas_search'].bind("<Return>", "_enter")
+
+        self.window['facturas_table'].bind('<Double-Button-1>', '_double_click')
+        self.window['clientes_table'].bind('<Double-Button-1>', '_double_click')
+        self.window['emitidas_table'].bind('<Double-Button-1>', '_double_click')
+        self.window['ajustes_table'].bind('<Double-Button-1>', '_double_click')
 
         # Add logging to the window
         h = logging.StreamHandler(self.window['console'])
         h.setLevel(logging.INFO)
         logging.root.addHandler(h)
 
         self.main_loop()
@@ -128,14 +128,21 @@
         if self.all_invoices:
             return self.all_invoices
         self.all_invoices = get_all_cfdi()
         return self.all_invoices
 
     def generate_invoice(self, invoice):
         ref_id = random_string()
+
+        # Add Serie and Folio and signature
+        invoice['Serie'] = self.serie
+        folio = self.local_db.folio()
+        invoice['Folio'] = str(folio)
+        cfdi40.Comprobante.sign(invoice, self.csd_signer)
+
         attempts = 3
         for i in range(attempts):
             if i:
                 print(f'Intentando de nuevo... Intento {i + 1} de {attempts}')
                 self._read(timeout=2000 * i)
 
             try:
@@ -147,52 +154,21 @@
             except Exception as ex:
                 logger.error(f"Error Generando: {invoice.get('Serie')}{invoice.get('Folio')} {invoice['Receptor']['Rfc']}")
                 if isinstance(ex, ResponseError):
                     logger.error(f"Status Code: {ex.response.status_code}")
                     logger.error(f"Response: {ex.response.text}")
                 continue
 
-            self.set_folio(int(res['Folio']) + 1)
+            self.set_folio(folio + 1)
             return move_to_folder(res.xml, pdf_data=res.pdf)
 
     def set_folio(self, folio: int = None):
         if folio:
             self.local_db.folio_set(folio)
-            self.window['folio'].update(folio)
-        else:
-            self.window['folio'].update(self.local_db.folio())
-
-    def enviar_correos(self, emisor_cif, emails):
-        with self.email_manager.sender as s:
-            for receptor, notify_invoices, pendientes_meses_anteriores in emails:
-                attachments = []
-                for r in notify_invoices:
-                    attachments += [r.filename + ".xml", r.filename + ".pdf"]
-
-                subject = f"Comprobantes Fiscales {receptor['RazonSocial']} - {receptor['Rfc']}"
-                s.send_email(
-                    subject=subject,
-                    to_addrs=receptor["Email"],
-                    html=generate_html_template(
-                        'mail_facturas_template.html',
-                        fields={
-                            "facturas": notify_invoices,
-                            'pendientes_meses_anteriores': pendientes_meses_anteriores,
-                            'emisor': emisor_cif,
-                        },
-                    ),
-                    file_attachments=attachments
-                )
-                for r in notify_invoices:
-                    self.local_db.notified_set(r.uuid, True)
-                print_yaml({
-                    "correo": subject,
-                    "para": receptor["Email"]
-                })
-                self._read()
+        self.window['folio'].update(folio or self.local_db.folio())
 
     def recupera_comprobantes(self, id_solicitud):
         response = self.sat_service.recover_comprobante_status(
             id_solicitud=id_solicitud
         )
         print_yaml(response)
         self._read()
@@ -214,203 +190,212 @@
 
     def _read(self, timeout=0):
         event, values = self.window.read(timeout=timeout)
         if event in ("Exit", PySimpleGUI.WIN_CLOSED):
             exit(0)
 
     def action_button(self, action_name, action_items):
-        if action_name == ACTION_FACTURAS:
+        if action_name == 'facturas':
             self.all_invoices = None
             for invoice in action_items:
                 cfdi = self.generate_invoice(invoice=invoice)
                 if cfdi is None:
                     break
                 print_yaml({
                     "FacturaGenerada": cfdi_header(cfdi),
                 })
                 self._read()
-        elif action_name == ACTION_EMAILS:
+        elif action_name == 'correos':
             clients = ClientsManager()
             emisor_cif = clients[self.csd_signer.rfc]
-            self.enviar_correos(emisor_cif, action_items)
-        elif action_name == ACTION_CLIENTS:
-            for rfc, details in action_items.items():
-                print(f"Validando: {rfc}")
+            with self.email_manager.sender as s:
+                for receptor, notify_invoices, pendientes_meses_anteriores in action_items:
+                    def attachments():
+                        for ni in notify_invoices:
+                            yield ni.filename + ".xml"
+                            yield ni.filename + ".pdf"
+
+                    subject = f"Comprobantes Fiscales {receptor['RazonSocial']} - {receptor['Rfc']}"
+
+                    s.send_email(
+                        subject=subject,
+                        to_addrs=receptor["Email"],
+                        html=facturacion_environment.get_template('mail_facturas_template.html').render(
+                            facturas=notify_invoices,
+                            pendientes_meses_anteriores=pendientes_meses_anteriores,
+                            emisor=emisor_cif,
+                        ),
+                        file_attachments=attachments()
+                    )
+                    for r in notify_invoices:
+                        self.local_db.notified_set(r.uuid, True)
+                    print_yaml({
+                        "correo": subject,
+                        "para": receptor["Email"]
+                    })
+                    self._read()
+        elif action_name == 'clientes':
+            for client in action_items:
+                print(f"Validando: {client['Rfc']}")
+                validar_client(client)
                 self._read()
-                validar_client(rfc, details)
+        else:
+            raise ValueError(f"Invalid action: {action_name}")
+        print("FIN")
 
     def set_selected_satcfdi(self, factura):
         i = factura
         self.selected_satcfdi = i
-        self.window["ver_factura"].update(disabled=not i)
         if i:
             estado = self.local_db.status_sat(i).get('Estado', 'Vigente')
             self.window["status_sat"].update(
-                estado,
-                visible=True,
+                estado.center(10),
+                disabled=False,
                 button_color="red4" if estado != "Vigente" else "green",
             )
         else:
             self.window["status_sat"].update(
-                visible=False
+                "".ljust(10), disabled=True, button_color=PySimpleGUI.theme_background_color()
             )
 
         # Email
         is_enviable = i \
                       and i["Emisor"]["Rfc"] == self.csd_signer.rfc \
                       and i.estatus == "1"
         if is_enviable:
             self.window["email_notificada"].update(
-                " Enviada  " if self.local_db.notified(i) else "Por Enviar",
-                visible=True,
+                "Enviada".center(10) if self.local_db.notified(i) else "Por Enviar",
+                disabled=False,
                 button_color="green" if self.local_db.notified(i) else "red4",
             )
         else:
-            self.window["email_notificada"].update("", visible=False)
+            self.window["email_notificada"].update(
+                "".ljust(10), disabled=True, button_color=PySimpleGUI.theme_background_color()
+            )
 
         # Pendiente de Pago
         is_pendientable = i \
                           and i["Emisor"]["Rfc"] == self.csd_signer.rfc \
                           and i["TipoDeComprobante"] == "I" \
                           and i.estatus == "1" \
                           and (i["MetodoPago"] == PUE or i.saldo_pendiente) \
                           and i["Total"]
         if is_pendientable:
             self.window["pendiente_pago"].update(
-                (" Pagada  " if i["MetodoPago"] == PUE else "Ignorada ") if self.local_db.liquidated(i) else "Por Pagar",
-                visible=True,
+                ("Pagada".center(10) if i["MetodoPago"] == PUE else "Ignorada".center(10)) if self.local_db.liquidated(i) else "Por Pagar".center(10),
+                disabled=False,
                 button_color="green" if self.local_db.liquidated(i) else "red4",
             )
         else:
-            self.window["pendiente_pago"].update("", visible=False)
+            self.window["pendiente_pago"].update(
+                "".ljust(10), disabled=True, button_color=PySimpleGUI.theme_background_color()
+            )
 
         # PPD
         is_ppd_active = i \
                         and i["Emisor"]["Rfc"] == self.csd_signer.rfc \
                         and i.get("MetodoPago") == PPD \
                         and i.estatus == "1" \
                         and i.saldo_pendiente
         is_ppd_active = bool(is_ppd_active)
-        self.window["fecha_pago_select"].update(visible=is_ppd_active)
-        self.window["fecha_pago"].update(visible=is_ppd_active)
-        self.window["forma_pago_text"].update(visible=is_ppd_active)
-        self.window["forma_pago"].update(visible=is_ppd_active)
-
-        self.window["prepare_pago"].update(visible=is_ppd_active)
-        self.window["imp_pagado_text"].update(visible=is_ppd_active)
-        self.window["importe_pago"].update(visible=is_ppd_active)
-
-    def print_satcfdis(self, cfdis):
-        def info_fmt(i):
-            return "" if self.local_db.notified(i) else "📧"
-
-        if cfdis := sorted(cfdis, key=lambda i: (i["Fecha"], i.name), reverse=True):
-            if self.window['detallado'].get():
-                for i, cfdi in enumerate(cfdis, start=1):
-                    log_item(f"FACTURA NUMERO: {i}")
-                    print_yaml(cfdi)
-                    self.local_db.describe(cfdi)
-            else:
-                print_invoices(
-                    [
-                        [
-                            i,
-                            cfdi['Receptor'].get('Nombre', '')[0:36],
-                            cfdi['Receptor']['Rfc'],
-                            cfdi.name,
-                            cfdi["Fecha"].strftime("%Y-%m-%d"),
-                            cfdi["Total"],
-                            self.local_db.liquidated_state(cfdi),
-                            mf_pago_fmt(cfdi),
-                            cfdi.uuid,
-                            info_fmt(cfdi)
-                        ]
-                        for i, cfdi in enumerate(cfdis, start=1)
-                    ]
-                )
-            if len(cfdis) == 1:
-                print_cfdi_details(cfdis[0])
-                self.set_selected_satcfdi(cfdis[0])
-            else:
-                self.set_selected_satcfdi(None)
-        else:
-            print("No hay resultados")
-            self.set_selected_satcfdi(None)
-
-    def print_prepared_cfdis(self, cfdis, start=1):
-        if cfdis:
-            if self.window['detallado'].get():
-                for i, cfdi in enumerate(cfdis, start=start):
-                    log_item(f"FACTURA NUMERO: {i}")
-                    print_yaml(cfdi)
-            else:
-                print_cfdis(cfdis, start=start)
-            self.action_button_manager.set_items(ACTION_FACTURAS, cfdis)
-        else:
-            print("No hay facturas para este mes")
+        self.window["ppd_action_items"].update(visible=is_ppd_active)
+        self.window["importe_pago"].update("")
 
-    def header(self, name, clear=True):
-        if clear:
-            self.console.update("")
-        log_line(name)
+    def header(self, name):
+        self.console.update("")
+        print(header_line(name))
+
+    def facturas_search(self, search_text):
+        search_text = search_text.strip().upper()
+        if len(search_text) < 3:
+            self.window["emitidas_text"].update("El texto de búsqueda debe tener al menos 3 caracteres")
+            return
+
+        self.window["emitidas_text"].update(search_text)
+
+        def fact_iter():
+            for i in self.get_all_invoices().values():
+                if i["Emisor"]["Rfc"] == self.csd_signer.rfc \
+                        and (
+                        i.name == search_text
+                        or i["Receptor"]["Rfc"] == search_text
+                        or search_text in i["Receptor"].get("Nombre", "")
+                ):
+                    yield i
+
+        cfdis = list(fact_iter())
+        self.emitidas_show(cfdis)
+
+    def facturas_pendientes(self):
+        self.window["emitidas_text"].update("Facturas Pendientes de Pago")
+
+        def fact_iter():
+            for i in self.get_all_invoices().values():
+                if i["Emisor"]["Rfc"] == self.csd_signer.rfc \
+                        and self.local_db.liquidated_state(i) == LiquidatedState.NO:
+                    yield i
+
+        cfdis = list(fact_iter())
+        self.emitidas_show(cfdis)
+
+    def facturas_emitidas(self, dp):
+        self.window["emitidas_text"].update("Facturas Emitidas en " + str(dp))
+
+        def fact_iter():
+            for i in self.get_all_invoices().values():
+                if i["Emisor"]["Rfc"] == self.csd_signer.rfc \
+                        and i["Fecha"] == dp:
+                    yield i
+
+        cfdis = list(fact_iter())
+        self.emitidas_show(cfdis)
+
+    def emitidas_show(self, cfdis):
+        rows = [
+            [
+                i,
+                cfdi['Receptor'].get('Nombre', '')[0:36],
+                cfdi['Receptor']['Rfc'],
+                cfdi.name,
+                cfdi["Fecha"].strftime("%Y-%m-%d"),
+                cfdi["Total"],
+                self.local_db.liquidated_state(cfdi),
+                mf_pago_fmt(cfdi)
+            ]
+            for i, cfdi in enumerate(cfdis, start=1)
+        ]
+        self.window['emitidas_table'].update(
+            values=rows,
+        )
+        self.window['emitidas_table'].metadata = cfdis
 
     def main_loop(self):
         while True:
             event, values = self.window.read()
-            dp = parse_date_period(values["periodo"])
-
             try:
                 if event in ("Exit", PySimpleGUI.WIN_CLOSED):
                     return
 
-                action_name, action_items = self.action_button_manager.clear()
+                try:
+                    dp = parse_date_period(values["periodo"])
+                except ValueError:
+                    dp = None
 
-                if event in ("prepare_correos", "prepare_clientes", "prepare_facturas", "crear_facturas",
-                             "rango_enter", "preparar_ajuste_anual", "recuperar_emitidas", "recuperar_recibidas"):
-                    self.set_selected_satcfdi([])
+                if event in ("periodo_enter", "refresh_facturas", "refresh_ajustes", "refresh_clientes", "refresh_correos"):
+                    event = 'main_tab_group'
 
                 match event:
                     case "folio":
                         self.set_folio(to_int(values["folio"]))
 
                     case "about":
                         clients = ClientsManager()
                         self.initial_screen(clients[self.csd_signer.rfc])
 
-                    case "buscar_factura" | 'factura_pagar_enter':
-                        self.header("Buscar Factura")
-
-                        if search_text := values["factura_pagar"].strip().upper():
-                            if len(search_text) < 3:
-                                self.console.update("El texto de búsqueda debe tener al menos 3 caracteres")
-                                continue
-
-                            if search_uuid := to_uuid(search_text):
-                                def fac_iter():
-                                    if v := self.get_all_invoices().get(search_uuid):
-                                        yield v
-                            else:
-                                def fac_iter():
-                                    for i in self.get_all_invoices().values():
-                                        if i["Emisor"]["Rfc"] == self.csd_signer.rfc and \
-                                                (i.name == search_text or i["Receptor"]["Rfc"] == search_text or search_text in i["Receptor"].get("Nombre", "")):
-                                            yield i
-
-                            self.print_satcfdis(fac_iter())
-                            self.window["descarga"].update(disabled=not search_uuid)
-
-                    case "preparar_ajuste_anual":
-                        self.header(f"AJUSTES")
-                        ajustes(
-                            emisor_rfc=self.csd_signer.rfc,
-                            dp=dp
-                        )
-
                     case "recuperar_emitidas" | "recuperar_recibidas":
-                        self.header("RECUPERAR")
                         fecha_final = date.today()
                         fecha_inicial = fecha_final - timedelta(days=int(values["recuperar_dias"]))
                         id_solicitud = self.local_db.get(event)
 
                         if not id_solicitud:
                             self._read()
                             response = self.sat_service.recover_comprobante_request(
@@ -432,284 +417,379 @@
                                 if data:
                                     self.all_invoices = None
                                     with io.BytesIO(data) as b:
                                         self.unzip_cfdi(b)
                                 del self.local_db[event]
                             print("FIN")
 
-                    case "prepare_clientes":
-                        self.header("CLIENTES")
-                        clients = ClientsManager()
-                        if clients:
-                            facturas = FacturasManager(dp)["Facturas"]
-                            print(
-                                tabulate(
-                                    [
-                                        [
-                                            i,
-                                            client["RazonSocial"][:36],
-                                            client["Rfc"],
-                                            client["RegimenFiscal"].code,
-                                            client["CodigoPostal"],
-                                            sum(1 for f in facturas if f["Receptor"] == k) or None,
-                                            "; ".join(client["Email"])[0:72],
-                                        ]
-                                        for i, (k, client) in enumerate(clients.items(), start=1)
-                                    ],
-                                    headers=(
-                                        "",
-                                        "Razon Social",
-                                        "Rfc",
-                                        "Reg",
-                                        "CP",
-                                        "#",
-                                        "Email",
-                                    ),
-                                    colalign=("right", "left", "left", "left", "left", "right"),
-                                )
-                            )
-                            self.action_button_manager.set_items(ACTION_CLIENTS, clients)
-                        else:
-                            print("No hay clientes")
+                    case "emitidas_search_enter":
+                        self.action_button_manager.clear()
+                        self.facturas_search(values["emitidas_search"])
+
+                    case 'main_tab_group':
+                        if values['main_tab_group'] == 'console_tab':
+                            self.action_button_manager.clear()
+
+                        if values['main_tab_group'] == 'recuperar_tab':
+                            self.action_button_manager.clear()
+
+                        if values['main_tab_group'] == 'facturas_tab':
+                            if dp is None or dp.month is None:
+                                self.window['preparar_facturas_text'].update("Periodo no válido")
+                                self.window['facturas_table'].update(values=[])
+                                continue
 
-                    case "prepare_facturas" | "rango_enter":
-                        self.header(f"PREPARAR FACTURAS {values['periodo']}")
-                        print('Periodo:', year_month_desc(dp), '[AL ...]')
-                        inicio, final = parse_rango(values["rango"])
-
-                        if cfdis := generate_ingresos(
-                                folio=int(values["folio"]),
-                                serie=self.serie,
+                            self.window['preparar_facturas_text'].update(f"{period_desc(dp)}")
+                            self.console.update("")
+                            cfdis = generate_ingresos(
                                 clients=ClientsManager(),
                                 facturas=FacturasManager(dp)["Facturas"],
                                 dp=dp,
-                                csd_signer=self.csd_signer
-                        ):
-                            final = final or len(cfdis)
-                            cfdis = cfdis[max(inicio - 1, 0):max(final, 0)]
+                                emisor_rfc=self.csd_signer.rfc
+                            )
+                            if cfdis is None:
+                                self.window['console_tab'].select()
+                                continue
+
+                            rows = [[
+                                i,
+                                cfdi['Emisor']['RegimenFiscal'].code,
+                                cfdi['Receptor']['Nombre'][0:36],
+                                cfdi['Receptor']['Rfc'],
+                                mf_pago_fmt(cfdi),
+                                cfdi['SubTotal'],
+                                cfdi['Total'],
+                            ]
+                                for i, cfdi in enumerate(cfdis, start=1)
+                            ]
+                            self.window['facturas_table'].update(
+                                values=rows,
+                            )
+                            self.window['facturas_table'].metadata = cfdis
+                            self.action_button_manager.set_items('facturas', cfdis)
 
-                        self.print_prepared_cfdis(cfdis, start=inicio)
+                        if values['main_tab_group'] == 'clients_tab':
+                            clients = list(ClientsManager().values())
+                            facturas = FacturasManager(dp)["Facturas"]
+                            rows = [
+                                [
+                                    i,
+                                    client["RazonSocial"][:36],
+                                    client["Rfc"],
+                                    client["RegimenFiscal"].code,
+                                    client["CodigoPostal"],
+                                    sum(1 for f in facturas if f["Receptor"] == client["Rfc"]) or "",
+                                ]
+                                for i, client in enumerate(clients, start=1)
+                            ]
+                            self.window['clientes_table'].update(
+                                values=rows,
+                            )
+                            self.window['clientes_table'].metadata = clients
+                            self.action_button_manager.set_items('clientes', clients)
 
-                    case "prepare_pago" | "importe_pago_enter" | "fecha_pago_enter" | "forma_pago_enter":
-                        self.header("COMPROBANTE PAGO")
-                        if i := self.selected_satcfdi:
-                            if cfdi := pago_factura(
-                                    serie=self.serie,
-                                    folio=int(values["folio"]),
-                                    factura_pagar=i,
-                                    fecha_pago=values["fecha_pago"],
-                                    forma_pago=values["forma_pago"],
-                                    importe_pago=values["importe_pago"],
-                                    csd_signer=self.csd_signer
+                        if values['main_tab_group'] == 'emitidas_tab':
+                            self.action_button_manager.clear()
+                            self.facturas_pendientes()
+
+                        if values['main_tab_group'] == 'correos_tab':
+                            now = date.today()
+                            dp_now = DatePeriod(now.year, now.month)
+                            clients = ClientsManager()
+                            a_invoices = self.get_all_invoices()
+
+                            cfdi_correos = []
+                            for receptor_rfc, notify_invoices in itertools.groupby(
+                                    sorted(
+                                        (i for i in a_invoices.values() if i.estatus == "1" and not self.local_db.notified(i)),
+                                        key=lambda r: r["Receptor"]["Rfc"]
+                                    ),
+                                    lambda r: r["Receptor"]["Rfc"]
                             ):
-                                self.print_prepared_cfdis([cfdi])
-                                print_cfdi_details(cfdi)
+                                notify_invoices = list(notify_invoices)
 
-                    case "ver_factura":
-                        if i := self.selected_satcfdi:
+                                def fac_pen_iter():
+                                    for i in self.get_all_invoices().values():
+                                        if i["Emisor"]["Rfc"] == self.csd_signer.rfc \
+                                                and self.local_db.liquidated_state(i) == LiquidatedState.NO \
+                                                and i["Fecha"] < dp_now \
+                                                and i["Receptor"]["Rfc"] == receptor_rfc \
+                                                and i not in notify_invoices:
+                                            yield i
+
+                                fac_pen = sorted(
+                                    fac_pen_iter(),
+                                    key=lambda r: r["Fecha"]
+                                )
+                                receptor = clients[receptor_rfc]
+                                cfdi_correos.append((receptor, notify_invoices, fac_pen))
+
+                            rows = [
+                                [
+                                    i,
+                                    receptor["RazonSocial"][0:36],
+                                    receptor["Rfc"],
+                                    ",".join(n.name for n in notify_invoices),
+                                    ",".join(n.name for n in facturas_pendientes)
+                                ] for i, (receptor, notify_invoices, facturas_pendientes) in enumerate(cfdi_correos, start=1)
+                            ]
+                            self.window['correos_table'].update(
+                                values=rows,
+                            )
+                            self.window['correos_table'].metadata = cfdi_correos
+                            self.action_button_manager.set_items('correos', cfdi_correos)
+
+                        if values['main_tab_group'] == 'ajustes_tab':
+                            if dp is None or dp.month is None:
+                                self.window['preparar_ajustes_text'].update("Periodo no válido")
+                                self.window['ajustes_table'].update(values=[])
+                                continue
+
+                            dp_effective = add_month(dp, 1)
+                            self.window['preparar_ajustes_text'].update(f"Ajustes Efectivos Al: {period_desc(dp_effective)}")
+
+                            # clear directory
+                            ajustes_dir = ajustes_directory(DatePeriod(dp.year, dp.month))
+                            clear_directory(ajustes_dir)
+                            emisor_rfc = self.csd_signer.rfc
+
+                            clients = ClientsManager()
+                            facturas = FacturasManager(None)["Facturas"]
+
+                            def ajustes_iter():
+                                for i, (rfc, concepto) in enumerate(find_ajustes(facturas, dp_effective.month)):
+                                    receptor = clients[rfc]  # type: dict
+                                    valor_unitario_raw = concepto["ValorUnitario"]
+
+                                    if isinstance(valor_unitario_raw, dict):
+                                        vud, vu = find_best_match(valor_unitario_raw, dp)
+                                        vund, vun = find_best_match(valor_unitario_raw, dp_effective)
+                                        meses = months_between(vund, vud)
+                                        ajuste_porcentaje = (vun / vu - 1)
+                                    else:
+                                        vu = valor_unitario_raw
+                                        vun = None
+                                        meses = None
+                                        ajuste_porcentaje = None
+
+                                    concepto = format_concepto_desc(concepto, periodo="INMUEBLE")
+                                    file_name = os.path.join(ajustes_dir, f'AjusteRenta_{rfc}_{i}.pdf')
+
+                                    data = {
+                                        "receptor": receptor,
+                                        "emisor": clients[emisor_rfc],
+                                        "concepto": concepto,
+                                        "valor_unitario": pesos(vu),
+                                        "valor_unitario_nuevo": pesos(vun) if vun else "",
+                                        "ajuste_porcentaje": porcentaje(ajuste_porcentaje, 2) if ajuste_porcentaje is not None else "",
+                                        "ajuste_periodo": f"{meses} MESES",
+                                        "efectivo_periodo_desc": periodicidad_desc(dp_effective, concepto['_periodo_mes_ajuste'], concepto.get('_desfase_mes')),
+                                        "periodo": concepto['_periodo_mes_ajuste'].split('.')[0].upper(),
+                                        "fecha_hoy": fecha(date.today()),
+                                        'file_name': file_name
+                                    }
+                                    if ajuste_porcentaje is not None:
+                                        res = generate_pdf_template(
+                                            template_name='incremento_template.md',
+                                            fields=data
+                                        )
+                                        with open(file_name, 'wb') as f:
+                                            f.write(res)
+                                    yield data
+
+                            ajustes_iter = list(ajustes_iter())
+                            rows = [
+                                [
+                                    i,
+                                    ajuste["receptor"]["RazonSocial"][:36],
+                                    ajuste["receptor"]["Rfc"],
+                                    ajuste["valor_unitario"].split(' ')[0],
+                                    ajuste["valor_unitario_nuevo"].split(' ')[0],
+                                    ajuste["ajuste_porcentaje"].split(' ')[0],
+                                    ajuste["periodo"],
+                                    ajuste["ajuste_periodo"],
+                                    ajuste["efectivo_periodo_desc"]
+                                ]
+                                for i, ajuste in enumerate(ajustes_iter, start=1)
+                            ]
+                            self.window['ajustes_table'].update(
+                                values=rows,
+                            )
+                            self.window['ajustes_table'].metadata = ajustes_iter
+                            self.action_button_manager.set_items('ajustes', ajustes_iter)
+
+                    case "facturas_pendientes":
+                        self.facturas_pendientes()
+
+                    case "facturas_emitidas":
+                        self.facturas_emitidas(dp)
+
+                    case 'facturas_table_double_click':
+                        items = self.window["facturas_table"].metadata
+                        selection = values["facturas_table"]
+                        s_items = [items[i] for i in selection] if selection else items
+                        preview_cfdis(s_items)
+
+                    case 'clientes_table_double_click':
+                        items = self.window["clientes_table"].metadata
+                        selection = values["clientes_table"]
+                        s_items = [items[i] for i in selection] if selection else items
+
+                        if s_items:
+                            client = s_items[0]
+                            url = csf.url(rfc=client["Rfc"], id_cif=client["IdCIF"])
+                            os.startfile(url)
+
+                    case 'emitidas_table_double_click':
+                        items = self.window["emitidas_table"].metadata
+                        selection = values["emitidas_table"]
+                        s_items = [items[i] for i in selection] if selection else items
+
+                        if s_items:
+                            cfdi = s_items[0]  # type: MyCFDI
                             os.startfile(
-                                os.path.abspath(i.filename + ".pdf")
+                                os.path.abspath(cfdi.filename + ".pdf")
                             )
 
+                    case 'ajustes_table_double_click':
+                        items = self.window["ajustes_table"].metadata
+                        selection = values["ajustes_table"]
+                        s_items = [items[i] for i in selection] if selection else items
+
+                        if s_items:
+                            ajuste = s_items[0]
+                            os.startfile(
+                                os.path.abspath(ajuste['file_name'])
+                            )
+
+                    case "facturas_table" | "clientes_table" | "correos_table" | "ajustes_table" | "emitidas_table":
+                        items = self.window[event].metadata
+                        selection = values[event]
+                        if event == "emitidas_table":
+                            if selection:
+                                self.set_selected_satcfdi(
+                                    items[selection[0]]
+                                )
+                            else:
+                                self.set_selected_satcfdi([])
+                        else:
+                            s_items = [items[i] for i in selection] if selection else items
+                            self.action_button_manager.set_items(event.split("_")[0], s_items)
+
+                    case "prepare_pago" | "importe_pago_enter" | "fecha_pago_enter" | "forma_pago_enter" | "ver_html_pago":
+                        if i := self.selected_satcfdi:
+                            fecha_pago = parse_fecha_pago(values["fecha_pago"])
+                            importe_pago = parse_importe_pago(values["importe_pago"])
+                            importe_pago = importe_pago or i.saldo_pendiente
+                            self.window["importe_pago"].update(importe_pago)
+
+                            cfdi = pago_factura(
+                                factura_pagar=i,
+                                fecha_pago=fecha_pago,
+                                forma_pago=values["forma_pago"],
+                                importe_pago=importe_pago,
+                            )
+                            self.action_button_manager.set_items('facturas', [cfdi])
+                            if event == "ver_html_pago":
+                                preview_cfdis([cfdi])
+
                     case "status_sat":
-                        self.header("STATUS SAT")
                         if i := self.selected_satcfdi:
-                            estado = self.local_db.status_sat(i, update=True)
-                            self.print_satcfdis([i])
-                            print_yaml(estado)
+                            self.local_db.status_sat(i, update=True)
+                            self.set_selected_satcfdi(i)
 
                     case "pendiente_pago":
                         if i := self.selected_satcfdi:
-                            st = self.local_db.liquidated_flip(i)
-                            self.console.update("")
-                            self.header(self.window[event].ButtonText.upper())
-                            self.print_satcfdis([i])
-                            if i["MetodoPago"] == PUE:
-                                print(f"FACTURA MARCADA COMO {'' if st else '-NO- '}PAGADA")
-                            else:
-                                print(f"FACTURA MARCADA COMO {'' if st else '-NO- '}IGNORADA")
+                            self.local_db.liquidated_flip(i)
+                            self.set_selected_satcfdi(i)
 
                     case "email_notificada":
                         if i := self.selected_satcfdi:
-                            st = self.local_db.notified_flip(i)
-                            self.console.update("")
-                            self.header(self.window[event].ButtonText.upper())
-                            self.print_satcfdis([i])
-                            print(f"FACTURA MARCADA COMO {'' if st else '-NO- '}NOTIFICADA")
-
-                    case "prepare_correos":
-                        self.header("CORREOS")
-                        now = date.today()
-                        dp_now = DatePeriod(now.year, now.month)
-                        clients = ClientsManager()
-                        a_invoices = self.get_all_invoices()
-
-                        cfdi_correos = []
-                        for receptor_rfc, notify_invoices in itertools.groupby(
-                                sorted(
-                                    (i for i in a_invoices.values() if i.estatus == "1" and not self.local_db.notified(i)),
-                                    key=lambda r: r["Receptor"]["Rfc"]
-                                ),
-                                lambda r: r["Receptor"]["Rfc"]
-                        ):
-                            notify_invoices = list(notify_invoices)
-
-                            def fac_pen_iter():
-                                for i in self.get_all_invoices().values():
-                                    if i["Emisor"]["Rfc"] == self.csd_signer.rfc \
-                                            and self.local_db.liquidated_state(i) == LiquidatedState.NO \
-                                            and i["Fecha"] < dp_now \
-                                            and i["Receptor"]["Rfc"] == receptor_rfc:
-                                        yield i
-
-                            fac_pen = sorted(
-                                fac_pen_iter(),
-                                key=lambda r: r["Fecha"]
-                            )
-                            receptor = clients[receptor_rfc]
-                            cfdi_correos.append((receptor, notify_invoices, fac_pen))
-
-                        if cfdi_correos:
-                            print(tabulate(
-                                [
-                                    [
-                                        i,
-                                        receptor["RazonSocial"][0:36],
-                                        receptor["Rfc"],
-                                        ",".join(n.name for n in notify_invoices),
-                                        ",".join(n.name for n in facturas_pendientes)
-                                    ] for i, (receptor, notify_invoices, facturas_pendientes) in enumerate(cfdi_correos, start=1)
-                                ],
-                                headers=(
-                                    '',
-                                    'Receptor Razon Social',
-                                    'Recep. Rfc',
-                                    'Facturas',
-                                    'Pendientes Emitidas Meses Anteriores'
-                                ),
-                                disable_numparse=True,
-                                colalign=("right", "left", "left", "left", "left")
-                            ))
-
-                            self.action_button_manager.set_items(ACTION_EMAILS, cfdi_correos)
-                        else:
-                            print("No hay correos pendientes de enviar")
+                            self.local_db.notified_flip(i)
+                            self.set_selected_satcfdi(i)
 
                     case "crear_facturas":
-                        self.console.update(autoscroll=True)
-                        self.header(f"PROCESAR {action_name.upper()}", clear=False)
+                        action_text = self.action_button_manager.text()
                         res = PySimpleGUI.popup(
-                            f"Estas seguro que quieres procesar {len(action_items)} {action_name}?",
-                            title=self.window[event].ButtonText,
+                            f"{action_text}?",
+                            title="Confirmar",
                             button_type=POPUP_BUTTONS_OK_CANCEL,
                         )
                         if res == "OK":
-                            self.action_button(action_name, action_items)
-                            print("FIN")
-                        else:
-                            print("OPERACION CANCELADA")
-                        self.console.update(autoscroll=False)
-
-                    case "facturas_pendientes":
-                        self.header("FACTURAS PENDIENTES")
-
-                        def fac_iter():
-                            for i in self.get_all_invoices().values():
-                                if i["Emisor"]["Rfc"] == self.csd_signer.rfc \
-                                        and self.local_db.liquidated_state(i) == LiquidatedState.NO:
-                                    yield i
-
-                        self.print_satcfdis(fac_iter())
-
-                    case "descarga":
-                        self.header('DESCARGADA')
-                        try:
-                            res = self.pac_service.recover(values["factura_pagar"], accept=Accept.XML_PDF)
-                            self.all_invoices = None
-                            cfdi = move_to_folder(res.xml, pdf_data=res.pdf)
-                            cfdi = self.get_all_invoices()[to_uuid(cfdi["Complemento"]["TimbreFiscalDigital"]["UUID"])]
-                            self.print_satcfdis([cfdi])
-                        except DocumentNotFoundError:
-                            logger.info("Factura no encontrada")
-
-                    case "facturas_emitidas" | "periodo_enter":
-                        self.header(f"FACTURAS EMITIDAS {values['periodo']}")
-
-                        def fact_iter():
-                            for i in self.get_all_invoices().values():
-                                if i["Emisor"]["Rfc"] == self.csd_signer.rfc \
-                                        and i["Fecha"] == dp:
-                                    yield i
-
-                        self.print_satcfdis(fact_iter())
+                            self.header(action_text.upper())
+                            self.window['console_tab'].select()
+                            self._read()
+                            self.action_button(
+                                action_name=self.action_button_manager.name,
+                                action_items=self.action_button_manager.items
+                            )
+                            self.action_button_manager.clear()
 
                     case "ver_excel":
-                        self.header("EXCEL")
                         clients = ClientsManager()
                         emisor_cif = clients[self.csd_signer.rfc]
                         if archivo_excel := exportar_facturas(
                                 self.get_all_invoices(),
                                 dp,
                                 emisor_cif,
                                 self.rfc_prediales
                         ):
-                            print("Archivo generado: " + archivo_excel)
                             os.startfile(
                                 os.path.abspath(archivo_excel)
                             )
                         else:
-                            print("No se pudo crear el archivo, cierra el archivo si se tiene abierto")
+                            raise Exception("No se pudo crear el archivo, cierra el archivo si se tiene abierto")
 
                     case "ver_html":
-                        self.header("HTML")
-
                         def fact_iter():
                             for i in self.get_all_invoices().values():
-                                if i["Emisor"]["Rfc"] == self.csd_signer.rfc \
-                                        and i["Fecha"] == dp:
+                                if i["Fecha"] == dp:
                                     yield i
 
                         if cfdis := list(fact_iter()):
-                            outfile = facturas_filename(dp, ext="html")
+                            outfile = archivos_filename(dp, ext="html")
                             Representable.html_write_all(
                                 objs=cfdis,
                                 target=outfile,
                             )
-                            print("Archivo generado: " + outfile)
                             os.startfile(
                                 os.path.abspath(outfile)
                             )
                         else:
-                            print("No hay facturas para periodo seleccionado")
+                            raise Exception("No hay facturas para el periodo seleccionado")
 
                     case "ver_carpeta":
-                        directory = facturas_folder(dp)
+                        directory = archivos_folder(dp)
                         os.startfile(
                             os.path.abspath(directory)
                         )
 
                     case "sat_status_todas":
-                        self.console.update(autoscroll=True)
-                        self.header("SAT STATUS")
-
                         def fact_iter():
                             for i in self.get_all_invoices().values():
                                 if i["Fecha"] == dp:
                                     yield i
 
                         for cfdi in fact_iter():
-                            print(f"Estado SAT: {cfdi.name} - {cfdi.uuid}")
+                            print(f"Estado SAT: {cfdi_header(cfdi)}")
                             self._read()
                             estado = self.local_db.status_sat(cfdi, update=True)
                             print_yaml(estado)
-
                         print("FIN")
-                        self.console.update(autoscroll=False)
 
                     case "periodo" | "inicio" | "final" | "fecha_pago" | "forma_pago" | "importe_pago" | ' ':
                         pass
 
                     case _:
                         logger.error(f"Unknown event '{event}'")
 
             except Exception as ex:
-                logger.exception(header_line("ERROR"))
+                if values['main_tab_group'] == 'console_tab':
+                    logger.exception(header_line("ERROR"))
+                else:
+                    PySimpleGUI.Popup(
+                        ex,
+                        no_titlebar=True,
+                        grab_anywhere=True,
+                        any_key_closes=True,
+                        background_color="red4",
+                    )
```

### Comparing `satdigitalinvoice-2.2.0/satdigitalinvoice/file_data_managers.py` & `satdigitalinvoice-3.0.0/satdigitalinvoice/file_data_managers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import collections.abc
 import json
 import logging
 import os
-from datetime import date
 from decimal import Decimal
 
 import jsonschema as jsonschema
 import yaml
 from satcfdi import Code, DatePeriod
 from satcfdi.pacs import sat
 # noinspection PyUnresolvedReferences
```

### Comparing `satdigitalinvoice-2.2.0/satdigitalinvoice/formatting_functions/common.py` & `satdigitalinvoice-3.0.0/satdigitalinvoice/formatting_functions/common.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.2.0/satdigitalinvoice/images/logo.png` & `satdigitalinvoice-3.0.0/satdigitalinvoice/images/logo.png`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.2.0/satdigitalinvoice/localdb.py` & `satdigitalinvoice-3.0.0/satdigitalinvoice/localdb.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 logger = logging.getLogger(__name__)
 
 
 class LocalDB(diskcache.Cache):
     def __init__(self):
         super().__init__(directory=os.path.join(DATA_DIRECTORY, 'cache'))
 
-    def folio(self):
+    def folio(self) -> int:
         return self.get(FOLIO, 1)
 
     def folio_set(self, value: int):
         self[FOLIO] = value
 
     def liquidated(self, uuid: UUID):
         return self.get((LIQUIDATED, uuid))
```

### Comparing `satdigitalinvoice-2.2.0/satdigitalinvoice/markdown_styles/markdown6.css` & `satdigitalinvoice-3.0.0/satdigitalinvoice/markdown_styles/markdown6.css`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.2.0/satdigitalinvoice/mycfdi.py` & `satdigitalinvoice-3.0.0/satdigitalinvoice/mycfdi.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.2.0/satdigitalinvoice/schemas/factura.yaml` & `satdigitalinvoice-3.0.0/satdigitalinvoice/schemas/factura.yaml`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.2.0/satdigitalinvoice/utils.py` & `satdigitalinvoice-3.0.0/satdigitalinvoice/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,17 @@
 from datetime import datetime
 from uuid import UUID
 
 from satcfdi import Signer, DatePeriod
 
 
 def parse_date_period(periodo):
+    if not periodo:
+        return DatePeriod(year=None)
+
     fmt, period = try_parsing_date(periodo)
     if fmt == '%Y':
         return DatePeriod(period.year)
     if fmt == '%Y-%m':
         return DatePeriod(period.year, period.month)
     if fmt == '%Y-%m-%d':
         return DatePeriod(period.year, period.month, period.day)
```

### Comparing `satdigitalinvoice-2.2.0/satdigitalinvoice.egg-info/PKG-INFO` & `satdigitalinvoice-3.0.0/satdigitalinvoice.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satdigitalinvoice
-Version: 2.2.0
+Version: 3.0.0
 Summary: GUI APP to Generate CFDI
 Home-page: https://github.com/SAT-CFDI/python-satdigitalinvoice
 Author: satcfdi@outlook.com
 Author-email: satcfdi@outlook.com
 License: MIT License
 Project-URL: Documentation, https://satdigitalinvoice.readthedocs.io
 Project-URL: Source, https://github.com/SAT-CFDI/python-satdigitalinvoice
```

### Comparing `satdigitalinvoice-2.2.0/satdigitalinvoice.egg-info/SOURCES.txt` & `satdigitalinvoice-3.0.0/satdigitalinvoice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.2.0/setup.py` & `satdigitalinvoice-3.0.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         package: [
             "markdown_styles/*",
             "schemas/*",
             'images/*',
         ],
     },
     install_requires=[
-        'satcfdi==4.0.10',
+        'satcfdi==4.0.11',
         'diskcache',
         'num2words',
         'PyYAML',
         'babel',
         'markdown2',
         'PySimpleGUI',
         'XlsxWriter',
```

### Comparing `satdigitalinvoice-2.2.0/tests/test_crear_facturas.py` & `satdigitalinvoice-3.0.0/tests/test_crear_facturas.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,43 +3,41 @@
 from decimal import Decimal
 from unittest import mock
 
 from satcfdi import Signer, DatePeriod
 
 from satdigitalinvoice.__version__ import __package__
 from satdigitalinvoice.file_data_managers import ClientsManager, FacturasManager, ConfigManager
-from satdigitalinvoice.gui_functions import generate_ingresos, periodo_desc
+from satdigitalinvoice.gui_functions import generate_ingresos, periodicidad_desc
 from satdigitalinvoice.utils import find_best_match
 from tests.utils import verify_result, XElementPrettyPrinter
 
 csd_signer = Signer.load(
     certificate=open('csd/cacx7605101p8.cer', 'rb').read(),
     key=open('csd/cacx7605101p8.key', 'rb').read(),
     password=open('csd/cacx7605101p8.txt', 'rb').read(),
 )
-ym_date = datetime(year=2023, month=4, day=1)
+ym_date = DatePeriod(year=2023, month=4)
 clients = ClientsManager()
 module = __package__
 
 
 def test_generar_ingresos(caplog):
     caplog.set_level(logging.INFO)
     config = ConfigManager()
     facturas = FacturasManager(ym_date)["Facturas"]
 
     with mock.patch(f'satcfdi.create.cfd.cfdi40.datetime') as m:
         m.now = mock.Mock(return_value=datetime(2022, 1, 1))
 
         facturas = generate_ingresos(
-            serie=config["serie"],
-            folio=1000,
             clients=clients,
             facturas=facturas,
             dp=date(year=2023, month=4, day=1),
-            csd_signer=csd_signer,
+            emisor_rfc=csd_signer.rfc
         )
 
         assert caplog.records == []
         assert len(facturas) == 3
 
         pp = XElementPrettyPrinter()
         verify = verify_result(data=pp.pformat(facturas), filename=f"facturas.pretty.py")
@@ -52,75 +50,71 @@
 def test_generar_ingresos_error(caplog):
     caplog.set_level(logging.INFO)
     config = ConfigManager()
     facturas = FacturasManager(ym_date)["FacturasIncorrectas"]
     print(len(facturas))
 
     ingresos = generate_ingresos(
-        serie=config["serie"],
-        folio=1000,
         clients=clients,
         facturas=facturas,
         dp=date(year=2023, month=4, day=1),
-        csd_signer=csd_signer,
+        emisor_rfc=csd_signer.rfc
     )
 
     assert len(caplog.records) == 1
     assert caplog.records[0].message == "ABMG891115PD7: Total '41000.16' is invalid, expected '37019.16'"
     assert ingresos is None
 
 
 def test_generar_ingresos_error2(caplog):
     caplog.set_level(logging.INFO)
     config = ConfigManager()
     facturas = FacturasManager(ym_date)["FacturasIncorrectas2"]
     print(len(facturas))
 
     ingresos = generate_ingresos(
-        serie=config["serie"],
-        folio=1000,
         clients=ClientsManager(),
         facturas=facturas,
         dp=date(year=2023, month=4, day=1),
-        csd_signer=csd_signer,
+        emisor_rfc=csd_signer.rfc
     )
 
     assert len(caplog.records) == 1
     assert caplog.records[0].message == "XXXNOEXISTO: client not found"
     assert ingresos is None
 
 
 def test_periodo_desc():
-    assert periodo_desc(DatePeriod(year=2021, month=1), 'Mensual.1', offset=0) == 'MES DE ENERO DEL 2021'
-    assert periodo_desc(DatePeriod(year=2021, month=1), 'Bimestral.2', offset=0) is None
-    assert periodo_desc(DatePeriod(year=2021, month=1), 'Trimestral.3', offset=0) is None
-    assert periodo_desc(DatePeriod(year=2021, month=1), 'Cuatrimestral.4', offset=0) is None
-    assert periodo_desc(DatePeriod(year=2021, month=1), 'Semestral.5', offset=0) is None
-    assert periodo_desc(DatePeriod(year=2021, month=1), 'Anual.6', offset=0) is None
-
-    assert periodo_desc(DatePeriod(year=2021, month=12), 'Mensual.7', offset=0) == 'MES DE DICIEMBRE DEL 2021'
-    assert periodo_desc(DatePeriod(year=2021, month=12), 'Bimestral.8', offset=0) == 'MES DE DICIEMBRE DEL 2021 AL MES DE ENERO DEL 2022'
-    assert periodo_desc(DatePeriod(year=2021, month=12), 'Trimestral.9', offset=0) == 'MES DE DICIEMBRE DEL 2021 AL MES DE FEBRERO DEL 2022'
-    assert periodo_desc(DatePeriod(year=2021, month=12), 'Cuatrimestral.8', offset=0) == 'MES DE DICIEMBRE DEL 2021 AL MES DE MARZO DEL 2022'
-    assert periodo_desc(DatePeriod(year=2021, month=12), 'Semestral.6', offset=0) == 'MES DE DICIEMBRE DEL 2021 AL MES DE MAYO DEL 2022'
-    assert periodo_desc(DatePeriod(year=2021, month=12), 'Anual.12', offset=0) == 'MES DE DICIEMBRE DEL 2021 AL MES DE NOVIEMBRE DEL 2022'
-
-    assert periodo_desc(DatePeriod(year=2021, month=1), 'Mensual.1', offset=1) == 'MES DE FEBRERO DEL 2021'
-    assert periodo_desc(DatePeriod(year=2021, month=1), 'Bimestral.2', offset=1) is None
-    assert periodo_desc(DatePeriod(year=2021, month=1), 'Trimestral.3', offset=1) is None
-    assert periodo_desc(DatePeriod(year=2021, month=1), 'Cuatrimestral.4', offset=1) is None
-    assert periodo_desc(DatePeriod(year=2021, month=1), 'Semestral.5', offset=1) is None
-    assert periodo_desc(DatePeriod(year=2021, month=1), 'Anual.6', offset=1) is None
-
-    assert periodo_desc(DatePeriod(year=2021, month=12), 'Mensual.7', offset=1) == 'MES DE ENERO DEL 2022'
-    assert periodo_desc(DatePeriod(year=2021, month=12), 'Bimestral.8', offset=1) == 'MES DE ENERO DEL 2022 AL MES DE FEBRERO DEL 2022'
-    assert periodo_desc(DatePeriod(year=2021, month=12), 'Trimestral.9', offset=1) == 'MES DE ENERO DEL 2022 AL MES DE MARZO DEL 2022'
-    assert periodo_desc(DatePeriod(year=2021, month=12), 'Cuatrimestral.8', offset=1) == 'MES DE ENERO DEL 2022 AL MES DE ABRIL DEL 2022'
-    assert periodo_desc(DatePeriod(year=2021, month=12), 'Semestral.6', offset=1) == 'MES DE ENERO DEL 2022 AL MES DE JUNIO DEL 2022'
-    assert periodo_desc(DatePeriod(year=2021, month=12), 'Anual.12', offset=1) == 'MES DE ENERO DEL 2022 AL MES DE DICIEMBRE DEL 2022'
+    assert periodicidad_desc(DatePeriod(year=2021, month=1), 'Mensual.1', offset=0) == 'MES DE ENERO DEL 2021'
+    assert periodicidad_desc(DatePeriod(year=2021, month=1), 'Bimestral.2', offset=0) is None
+    assert periodicidad_desc(DatePeriod(year=2021, month=1), 'Trimestral.3', offset=0) is None
+    assert periodicidad_desc(DatePeriod(year=2021, month=1), 'Cuatrimestral.4', offset=0) is None
+    assert periodicidad_desc(DatePeriod(year=2021, month=1), 'Semestral.5', offset=0) is None
+    assert periodicidad_desc(DatePeriod(year=2021, month=1), 'Anual.6', offset=0) is None
+
+    assert periodicidad_desc(DatePeriod(year=2021, month=12), 'Mensual.7', offset=0) == 'MES DE DICIEMBRE DEL 2021'
+    assert periodicidad_desc(DatePeriod(year=2021, month=12), 'Bimestral.8', offset=0) == 'MES DE DICIEMBRE DEL 2021 AL MES DE ENERO DEL 2022'
+    assert periodicidad_desc(DatePeriod(year=2021, month=12), 'Trimestral.9', offset=0) == 'MES DE DICIEMBRE DEL 2021 AL MES DE FEBRERO DEL 2022'
+    assert periodicidad_desc(DatePeriod(year=2021, month=12), 'Cuatrimestral.8', offset=0) == 'MES DE DICIEMBRE DEL 2021 AL MES DE MARZO DEL 2022'
+    assert periodicidad_desc(DatePeriod(year=2021, month=12), 'Semestral.6', offset=0) == 'MES DE DICIEMBRE DEL 2021 AL MES DE MAYO DEL 2022'
+    assert periodicidad_desc(DatePeriod(year=2021, month=12), 'Anual.12', offset=0) == 'MES DE DICIEMBRE DEL 2021 AL MES DE NOVIEMBRE DEL 2022'
+
+    assert periodicidad_desc(DatePeriod(year=2021, month=1), 'Mensual.1', offset=1) == 'MES DE FEBRERO DEL 2021'
+    assert periodicidad_desc(DatePeriod(year=2021, month=1), 'Bimestral.2', offset=1) is None
+    assert periodicidad_desc(DatePeriod(year=2021, month=1), 'Trimestral.3', offset=1) is None
+    assert periodicidad_desc(DatePeriod(year=2021, month=1), 'Cuatrimestral.4', offset=1) is None
+    assert periodicidad_desc(DatePeriod(year=2021, month=1), 'Semestral.5', offset=1) is None
+    assert periodicidad_desc(DatePeriod(year=2021, month=1), 'Anual.6', offset=1) is None
+
+    assert periodicidad_desc(DatePeriod(year=2021, month=12), 'Mensual.7', offset=1) == 'MES DE ENERO DEL 2022'
+    assert periodicidad_desc(DatePeriod(year=2021, month=12), 'Bimestral.8', offset=1) == 'MES DE ENERO DEL 2022 AL MES DE FEBRERO DEL 2022'
+    assert periodicidad_desc(DatePeriod(year=2021, month=12), 'Trimestral.9', offset=1) == 'MES DE ENERO DEL 2022 AL MES DE MARZO DEL 2022'
+    assert periodicidad_desc(DatePeriod(year=2021, month=12), 'Cuatrimestral.8', offset=1) == 'MES DE ENERO DEL 2022 AL MES DE ABRIL DEL 2022'
+    assert periodicidad_desc(DatePeriod(year=2021, month=12), 'Semestral.6', offset=1) == 'MES DE ENERO DEL 2022 AL MES DE JUNIO DEL 2022'
+    assert periodicidad_desc(DatePeriod(year=2021, month=12), 'Anual.12', offset=1) == 'MES DE ENERO DEL 2022 AL MES DE DICIEMBRE DEL 2022'
 
 
 def test_find_best_match():
     casesA = {
         '2022-12': Decimal('20.00'),
         '2023-12': Decimal('30.00'),
         '2024-12': Decimal('40.00'),
@@ -130,12 +124,12 @@
         '2025-12': None,
         '2024-12': Decimal('40.00'),
         '2023-12': Decimal('30.00'),
         '2022-12': Decimal('20.00'),
     }
 
     for cases in (casesA, casesB):
-        assert find_best_match(cases, datetime(2022, 4, 5))[1] is None
-        assert find_best_match(cases, datetime(2023, 4, 5))[1] == Decimal('20.00')
-        assert find_best_match(cases, datetime(2024, 4, 5))[1] == Decimal('30.00')
-        assert find_best_match(cases, datetime(2025, 4, 5))[1] == Decimal('40.00')
-        assert find_best_match(cases, datetime(2026, 4, 5))[1] is None
+        assert find_best_match(cases, DatePeriod(2022, 4, 5))[1] is None
+        assert find_best_match(cases, DatePeriod(2023, 4, 5))[1] == Decimal('20.00')
+        assert find_best_match(cases, DatePeriod(2024, 4, 5))[1] == Decimal('30.00')
+        assert find_best_match(cases, DatePeriod(2025, 4, 5))[1] == Decimal('40.00')
+        assert find_best_match(cases, DatePeriod(2026, 4, 5))[1] is None
```

### Comparing `satdigitalinvoice-2.2.0/tests/test_localdb.py` & `satdigitalinvoice-3.0.0/tests/test_localdb.py`

 * *Files identical despite different names*

### Comparing `satdigitalinvoice-2.2.0/tests/test_main.py` & `satdigitalinvoice-3.0.0/tests/test_main.py`

 * *Files identical despite different names*

