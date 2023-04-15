# Comparing `tmp/AksharaJaana-0.2.1.0.tar.gz` & `tmp/AksharaJaana-1.0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AksharaJaana-0.2.1.0.tar", last modified: Sat Apr 15 13:53:44 2023, max compression
+gzip compressed data, was "dist\AksharaJaana-1.0.0.1.tar", last modified: Mon Jun 13 17:28:29 2022, max compression
```

## Comparing `AksharaJaana-0.2.1.0.tar` & `AksharaJaana-1.0.0.1.tar`

### file list

```diff
@@ -1,18 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:53:44.691339 AksharaJaana-0.2.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:53:44.687339 AksharaJaana-0.2.1.0/AksharaJaana/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 13:53:31.000000 AksharaJaana-0.2.1.0/AksharaJaana/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-04-15 13:53:31.000000 AksharaJaana-0.2.1.0/AksharaJaana/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    10026 2023-04-15 13:53:31.000000 AksharaJaana-0.2.1.0/AksharaJaana/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:53:44.691339 AksharaJaana-0.2.1.0/AksharaJaana.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4561 2023-04-15 13:53:44.000000 AksharaJaana-0.2.1.0/AksharaJaana.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-15 13:53:44.000000 AksharaJaana-0.2.1.0/AksharaJaana.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 13:53:44.000000 AksharaJaana-0.2.1.0/AksharaJaana.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-15 13:53:44.000000 AksharaJaana-0.2.1.0/AksharaJaana.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4561 2023-04-15 13:53:44.691339 AksharaJaana-0.2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-04-15 13:53:31.000000 AksharaJaana-0.2.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 13:53:44.691339 AksharaJaana-0.2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-15 13:53:31.000000 AksharaJaana-0.2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:53:44.691339 AksharaJaana-0.2.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 13:53:31.000000 AksharaJaana-0.2.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-15 13:53:31.000000 AksharaJaana-0.2.1.0/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5003 2023-04-15 13:53:31.000000 AksharaJaana-0.2.1.0/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2022-06-13 17:28:29.793770 AksharaJaana-1.0.0.1/
+drwxrwxrwx   0        0        0        0 2022-06-13 17:28:29.689768 AksharaJaana-1.0.0.1/AksharaJaana/
+-rw-rw-rw-   0        0        0        0 2022-06-13 13:37:16.000000 AksharaJaana-1.0.0.1/AksharaJaana/__init__.py
+-rw-rw-rw-   0        0        0     2323 2022-06-13 15:17:08.000000 AksharaJaana-1.0.0.1/AksharaJaana/main.py
+-rw-rw-rw-   0        0        0    10687 2022-06-13 13:37:16.000000 AksharaJaana-1.0.0.1/AksharaJaana/utils.py
+drwxrwxrwx   0        0        0        0 2022-06-13 17:28:29.787772 AksharaJaana-1.0.0.1/AksharaJaana.egg-info/
+-rw-rw-rw-   0        0        0     4202 2022-06-13 17:28:29.000000 AksharaJaana-1.0.0.1/AksharaJaana.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      230 2022-06-13 17:28:29.000000 AksharaJaana-1.0.0.1/AksharaJaana.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-06-13 17:28:29.000000 AksharaJaana-1.0.0.1/AksharaJaana.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2022-06-13 17:28:29.000000 AksharaJaana-1.0.0.1/AksharaJaana.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4202 2022-06-13 17:28:29.791769 AksharaJaana-1.0.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3730 2022-06-13 15:01:30.000000 AksharaJaana-1.0.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2022-06-13 17:28:29.794772 AksharaJaana-1.0.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      711 2022-06-13 17:27:47.000000 AksharaJaana-1.0.0.1/setup.py
```

### Comparing `AksharaJaana-0.2.1.0/AksharaJaana.egg-info/PKG-INFO` & `AksharaJaana-1.0.0.1/AksharaJaana.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,129 +1,119 @@
-Metadata-Version: 2.1
-Name: AksharaJaana
-Version: 0.2.1.0
-Summary: A Kannada OCR
-Home-page: https://github.com/Navaneeth-Sharma/Akshara-Jaana/
-Author: Navaneeth
-Author-email: navaneethsharma2310oct@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-
-# AksharaJaana
-
-<p align="center">
-     <img src="https://user-images.githubusercontent.com/63489382/173864136-118db121-fcf4-4c8a-9b7d-7c4e4c0e48f9.png" width=200px>
-</p>
-
-<p align="center">
-   An OCR for Kannada.
-</p>
-
-<p align="center">
-   <a href="https://www.npmjs.com/package/@swc/core">
-     <a href="https://pypi.org/project/AksharaJaana/"><img src="https://img.shields.io/badge/pypi-package-blue?labelColor=black&style=flat&logo=python&link=https://pypi.org/project/AksharaJaana/" alt="pypi" /></a>
-   </a>
-</p>
-
-AksharaJaana is a package which uses tesseract ocr in the backend to convert the read-only kannada text to editable format.
-A Special feature of this is it can separate columns in the page and thus making it easier to read and edit.
-Do consider using this  package if necessary and feel free to mail me for any clarifications.
-
-- Email : navaneethsharma2310oct@gmail.com
-- Twitter handle: https://twitter.com/navaneethakbh
-
-Happy coding and installing.
-
-To see the python package visit https://pypi.org/project/AksharaJaana/
-
-## The Requirements
-
-***Conda environment is preferred for the smooth use***
-
-- AksharaJaana *(pip package)*, check out the latest version available
-- Tesseract
-- poppler
-
-## Details for Installation
-
-### Ubuntu
-
-Open terminal and execute below commands.
-
-1. **Installing tesseract-ocr in the system**
-
-     ```bash
-     sudo apt-get update -y 
-     sudo apt-get install -y tesseract-ocr 
-     ```
-
-2. **Installing poppler in the system**
-
-   ```bash
-   sudo apt-get install -y poppler-utils 
-   ```
-
-3. **Installing python and pip (if pip is not installed)**
-
-   ```bash
-   sudo apt install python==3.6.9
-   ```
-
-4. **Installing packages for AksharaJaana**
-
-   ```bash
-   pip install --upgrade AksharaJaana
-   ```
-
-### Windows
-
-1. Installing tesseract-ocr in the system
-   - **Download tesseract**
-     - go to the <a href="https://github.com/UB-Mannheim/tesseract/wiki">website</a>
-     - click on `tesseract-ocr-w64-setup-v5.0.0-alpha.20200328.exe (64 bit)`.
-   - **Install tesseract for Kannada Language and Script**
-     - open the downloaded file and click next and accept the agreement.
-     - Next you will give an option to choose the languages.
-     - **Choose kannada in both script and language**
-   - **Add tesseract to Path**
-     - Check if this folder `C:\Program Files\Tesseract-OCR\` is present. If yes, follow below procedure
-     - Add `C:\Program Files\Tesseract-OCR\`  to your system PATH by doing the following
-        1. Click on the `Windows start button`, search for `Edit the system environment variables`, click on Environment Variables
-        2. Under System variables, look for and double-click on PATH, click on `New`.
-        3. then add `C:\Program Files\Tesseract-OCR\`, click OK.
-     - if folder is not present, manually add the folder tesseract-ocr to the Program Files in the C drive which must be present at the download section (after extraction) and follow the same procedure
-     - See complete [docs](docs/tesseract_installation/README.md).
-
-2. Installing poppler in the system
-
-    - **Download Poppler**
-      - go to <a href="http://blog.alivate.com.au/poppler-windows/">this</a> page
-      - click on `poppler-0.54_x86`
-    - **Unzip** the file and copy files to `C:\Users\Program Files\poppler-0.68.0_x86`
-    - **Add poppler to path**
-      - Add `C:\Program Files\poppler-0.68.0_x86\bin` to your system PATH by doing the following:
-        1. Click on the Windows start button, search for Edit the system environment variables, click on Environment Variables
-        2. under System variables, look for and double-click on PATH, click on New
-        3. then add C:\Users\Program Files\poppler-0.68.0_x86\bin, click OK.
-
-3. Installing python and pip in the system (If pip is not installed)
-   - <a href="https://www.python.org/downloads/">Download python</a>
-
-4. Installing packages for AksharaJaana
-   - open command prompt
-
-     ```bash
-     pip install AksharaJaana
-     ```
-
-5. **Reboot** the system before starting to use
-
-### Python Script
-
-```python
-import AksharaJaana.main as ak 
-text = ak.ocr_engine("Your file Path") 
-print(text) 
-```
+Metadata-Version: 2.1
+Name: AksharaJaana
+Version: 1.0.0.1
+Summary: A Kannada OCR
+Home-page: https://github.com/Navaneeth-Sharma/Akshara-Jaana/
+Author: Navaneeth
+Author-email: navaneethsharma2310oct@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+
+# AksharaJaana
+
+AksharaJaana is a package which uses tesseract ocr in the backend to convert the read-only kannada text to editable format.
+A Special feature of this is it can separate columns in the page and thus making it easier to read and edit.
+Do consider using this  package if necessary and feel free to mail me for any clarifications.
+
+- Email : navaneethsharma2310oct@gmail.com
+- Twitter handle: https://twitter.com/navaneethakbh
+
+Happy coding and installing.
+
+To see the python package visit https://pypi.org/project/AksharaJaana/
+
+## The Requirements
+
+***Conda environment is preferred for the smooth use***
+
+- AksharaJaana *(pip package)*, check out the latest version available
+- Tesseract
+- poppler
+
+## Details for Installation
+
+### Ubuntu
+
+Open terminal and execute below commands.
+
+1. **Installing tesseract-ocr in the system**
+
+     ```bash
+     sudo apt-get update -y 
+     sudo apt-get install -y tesseract-ocr 
+     ```
+
+2. **Installing poppler in the system**
+
+   ```bash
+   sudo apt-get install -y poppler-utils 
+   ```
+
+3. **Installing python and pip (if pip is not installed)**
+
+   ```bash
+   sudo apt install python==3.6.9
+   ```
+
+4. **Installing packages for AksharaJaana**
+
+   ```bash
+   pip install AksharaJaana
+   ```
+
+### Windows
+
+1. Installing tesseract-ocr in the system
+   - **Download tesseract**
+     - go to the <a href="https://github.com/UB-Mannheim/tesseract/wiki">website</a>
+     - click on `tesseract-ocr-w64-setup-v5.0.0-alpha.20200328.exe (64 bit)`.
+   - **Install tesseract for Kannada Language and Script**
+     - open the downloaded file and click next and accept the agreement.
+     - Next you will give an option to choose the languages.
+     - **Choose kannada in both script and language**
+   - **Add tesseract to Path**
+     - Check if this folder `C:\Program Files\Tesseract-OCR\` is present. If yes, follow below procedure
+     - Add `C:\Program Files\Tesseract-OCR\`  to your system PATH by doing the following
+        1. Click on the `Windows start button`, search for `Edit the system environment variables`, click on Environment Variables
+        2. Under System variables, look for and double-click on PATH, click on `New`.
+        3. then add `C:\Program Files\Tesseract-OCR\`, click OK.
+     - if folder is not present, manually add the folder tesseract-ocr to the Program Files in the C drive which must be present at the download section (after extraction) and follow the same procedure
+     - See complete [docs](docs/tesseract_installation/README.md).
+
+2. Installing poppler in the system
+
+    - **Download Poppler**
+      - go to <a href="http://blog.alivate.com.au/poppler-windows/">this</a> page
+      - click on `poppler-0.54_x86`
+    - **Unzip** the file and copy files to `C:\Users\Program Files\poppler-0.68.0_x86`
+    - **Add poppler to path**
+      - Add `C:\Program Files\poppler-0.68.0_x86\bin` to your system PATH by doing the following:
+        1. Click on the Windows start button, search for Edit the system environment variables, click on Environment Variables
+        2. under System variables, look for and double-click on PATH, click on New
+        3. then add C:\Users\Program Files\poppler-0.68.0_x86\bin, click OK.
+
+3. Installing python and pip in the system (If pip is not installed)
+   - <a href="https://www.python.org/downloads/">Download python</a>
+
+4. Installing packages for AksharaJaana
+   - open command prompt
+
+     ```bash
+     pip install AksharaJaana
+     ```
+
+5. **Reboot** the system before starting to use
+
+### Python Script
+
+```python
+import AksharaJaana.main as ak 
+text = ak.ocr_engine("Your file Path") 
+print(text) 
+```
+
+
```

#### html2text {}

```diff
@@ -1,33 +1,29 @@
-Metadata-Version: 2.1 Name: AksharaJaana Version: 0.2.1.0 Summary: A Kannada
+Metadata-Version: 2.1 Name: AksharaJaana Version: 1.0.0.1 Summary: A Kannada
 OCR Home-page: https://github.com/Navaneeth-Sharma/Akshara-Jaana/ Author:
-Navaneeth Author-email: navaneethsharma2310oct@gmail.com Classifier:
-Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
-License Classifier: Operating System :: OS Independent Requires-Python: >=3.6
-Description-Content-Type: text/markdown # AksharaJaana
- [https://user-images.githubusercontent.com/63489382/173864136-118db121-fcf4-
-                          4c8a-9b7d-7c4e4c0e48f9.png]
-                              An OCR for Kannada.
-                                    [pypi]
-AksharaJaana is a package which uses tesseract ocr in the backend to convert
-the read-only kannada text to editable format. A Special feature of this is it
-can separate columns in the page and thus making it easier to read and edit. Do
-consider using this package if necessary and feel free to mail me for any
-clarifications. - Email : navaneethsharma2310oct@gmail.com - Twitter handle:
-https://twitter.com/navaneethakbh Happy coding and installing. To see the
-python package visit https://pypi.org/project/AksharaJaana/ ## The Requirements
-***Conda environment is preferred for the smooth use*** - AksharaJaana *(pip
-package)*, check out the latest version available - Tesseract - poppler ##
-Details for Installation ### Ubuntu Open terminal and execute below commands.
-1. **Installing tesseract-ocr in the system** ```bash sudo apt-get update -
-y sudo apt-get install -y tesseract-ocr ``` 2. **Installing poppler in the
-system** ```bash sudo apt-get install -y poppler-utils ``` 3. **Installing
-python and pip (if pip is not installed)** ```bash sudo apt install
-python==3.6.9 ``` 4. **Installing packages for AksharaJaana** ```bash pip
-install --upgrade AksharaJaana ``` ### Windows 1. Installing tesseract-ocr in
+Navaneeth Author-email: navaneethsharma2310oct@gmail.com License: UNKNOWN
+Platform: UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier:
+License :: OSI Approved :: MIT License Classifier: Operating System :: OS
+Independent Requires-Python: >=3.6 Description-Content-Type: text/markdown #
+AksharaJaana AksharaJaana is a package which uses tesseract ocr in the backend
+to convert the read-only kannada text to editable format. A Special feature of
+this is it can separate columns in the page and thus making it easier to read
+and edit. Do consider using this package if necessary and feel free to mail me
+for any clarifications. - Email : navaneethsharma2310oct@gmail.com - Twitter
+handle: https://twitter.com/navaneethakbh Happy coding and installing. To see
+the python package visit https://pypi.org/project/AksharaJaana/ ## The
+Requirements ***Conda environment is preferred for the smooth use*** -
+AksharaJaana *(pip package)*, check out the latest version available -
+Tesseract - poppler ## Details for Installation ### Ubuntu Open terminal and
+execute below commands. 1. **Installing tesseract-ocr in the system** ```bash
+sudo apt-get update -y sudo apt-get install -y tesseract-ocr ``` 2.
+**Installing poppler in the system** ```bash sudo apt-get install -y poppler-
+utils ``` 3. **Installing python and pip (if pip is not installed)** ```bash
+sudo apt install python==3.6.9 ``` 4. **Installing packages for AksharaJaana**
+```bash pip install AksharaJaana ``` ### Windows 1. Installing tesseract-ocr in
 the system - **Download tesseract** - go to the website - click on `tesseract-
 ocr-w64-setup-v5.0.0-alpha.20200328.exe (64 bit)`. - **Install tesseract for
 Kannada Language and Script** - open the downloaded file and click next and
 accept the agreement. - Next you will give an option to choose the languages. -
 **Choose kannada in both script and language** - **Add tesseract to Path** -
 Check if this folder `C:\Program Files\Tesseract-OCR\` is present. If yes,
 follow below procedure - Add `C:\Program Files\Tesseract-OCR\` to your system
```

### Comparing `AksharaJaana-0.2.1.0/PKG-INFO` & `AksharaJaana-1.0.0.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,129 +1,119 @@
-Metadata-Version: 2.1
-Name: AksharaJaana
-Version: 0.2.1.0
-Summary: A Kannada OCR
-Home-page: https://github.com/Navaneeth-Sharma/Akshara-Jaana/
-Author: Navaneeth
-Author-email: navaneethsharma2310oct@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-
-# AksharaJaana
-
-<p align="center">
-     <img src="https://user-images.githubusercontent.com/63489382/173864136-118db121-fcf4-4c8a-9b7d-7c4e4c0e48f9.png" width=200px>
-</p>
-
-<p align="center">
-   An OCR for Kannada.
-</p>
-
-<p align="center">
-   <a href="https://www.npmjs.com/package/@swc/core">
-     <a href="https://pypi.org/project/AksharaJaana/"><img src="https://img.shields.io/badge/pypi-package-blue?labelColor=black&style=flat&logo=python&link=https://pypi.org/project/AksharaJaana/" alt="pypi" /></a>
-   </a>
-</p>
-
-AksharaJaana is a package which uses tesseract ocr in the backend to convert the read-only kannada text to editable format.
-A Special feature of this is it can separate columns in the page and thus making it easier to read and edit.
-Do consider using this  package if necessary and feel free to mail me for any clarifications.
-
-- Email : navaneethsharma2310oct@gmail.com
-- Twitter handle: https://twitter.com/navaneethakbh
-
-Happy coding and installing.
-
-To see the python package visit https://pypi.org/project/AksharaJaana/
-
-## The Requirements
-
-***Conda environment is preferred for the smooth use***
-
-- AksharaJaana *(pip package)*, check out the latest version available
-- Tesseract
-- poppler
-
-## Details for Installation
-
-### Ubuntu
-
-Open terminal and execute below commands.
-
-1. **Installing tesseract-ocr in the system**
-
-     ```bash
-     sudo apt-get update -y 
-     sudo apt-get install -y tesseract-ocr 
-     ```
-
-2. **Installing poppler in the system**
-
-   ```bash
-   sudo apt-get install -y poppler-utils 
-   ```
-
-3. **Installing python and pip (if pip is not installed)**
-
-   ```bash
-   sudo apt install python==3.6.9
-   ```
-
-4. **Installing packages for AksharaJaana**
-
-   ```bash
-   pip install --upgrade AksharaJaana
-   ```
-
-### Windows
-
-1. Installing tesseract-ocr in the system
-   - **Download tesseract**
-     - go to the <a href="https://github.com/UB-Mannheim/tesseract/wiki">website</a>
-     - click on `tesseract-ocr-w64-setup-v5.0.0-alpha.20200328.exe (64 bit)`.
-   - **Install tesseract for Kannada Language and Script**
-     - open the downloaded file and click next and accept the agreement.
-     - Next you will give an option to choose the languages.
-     - **Choose kannada in both script and language**
-   - **Add tesseract to Path**
-     - Check if this folder `C:\Program Files\Tesseract-OCR\` is present. If yes, follow below procedure
-     - Add `C:\Program Files\Tesseract-OCR\`  to your system PATH by doing the following
-        1. Click on the `Windows start button`, search for `Edit the system environment variables`, click on Environment Variables
-        2. Under System variables, look for and double-click on PATH, click on `New`.
-        3. then add `C:\Program Files\Tesseract-OCR\`, click OK.
-     - if folder is not present, manually add the folder tesseract-ocr to the Program Files in the C drive which must be present at the download section (after extraction) and follow the same procedure
-     - See complete [docs](docs/tesseract_installation/README.md).
-
-2. Installing poppler in the system
-
-    - **Download Poppler**
-      - go to <a href="http://blog.alivate.com.au/poppler-windows/">this</a> page
-      - click on `poppler-0.54_x86`
-    - **Unzip** the file and copy files to `C:\Users\Program Files\poppler-0.68.0_x86`
-    - **Add poppler to path**
-      - Add `C:\Program Files\poppler-0.68.0_x86\bin` to your system PATH by doing the following:
-        1. Click on the Windows start button, search for Edit the system environment variables, click on Environment Variables
-        2. under System variables, look for and double-click on PATH, click on New
-        3. then add C:\Users\Program Files\poppler-0.68.0_x86\bin, click OK.
-
-3. Installing python and pip in the system (If pip is not installed)
-   - <a href="https://www.python.org/downloads/">Download python</a>
-
-4. Installing packages for AksharaJaana
-   - open command prompt
-
-     ```bash
-     pip install AksharaJaana
-     ```
-
-5. **Reboot** the system before starting to use
-
-### Python Script
-
-```python
-import AksharaJaana.main as ak 
-text = ak.ocr_engine("Your file Path") 
-print(text) 
-```
+Metadata-Version: 2.1
+Name: AksharaJaana
+Version: 1.0.0.1
+Summary: A Kannada OCR
+Home-page: https://github.com/Navaneeth-Sharma/Akshara-Jaana/
+Author: Navaneeth
+Author-email: navaneethsharma2310oct@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+
+# AksharaJaana
+
+AksharaJaana is a package which uses tesseract ocr in the backend to convert the read-only kannada text to editable format.
+A Special feature of this is it can separate columns in the page and thus making it easier to read and edit.
+Do consider using this  package if necessary and feel free to mail me for any clarifications.
+
+- Email : navaneethsharma2310oct@gmail.com
+- Twitter handle: https://twitter.com/navaneethakbh
+
+Happy coding and installing.
+
+To see the python package visit https://pypi.org/project/AksharaJaana/
+
+## The Requirements
+
+***Conda environment is preferred for the smooth use***
+
+- AksharaJaana *(pip package)*, check out the latest version available
+- Tesseract
+- poppler
+
+## Details for Installation
+
+### Ubuntu
+
+Open terminal and execute below commands.
+
+1. **Installing tesseract-ocr in the system**
+
+     ```bash
+     sudo apt-get update -y 
+     sudo apt-get install -y tesseract-ocr 
+     ```
+
+2. **Installing poppler in the system**
+
+   ```bash
+   sudo apt-get install -y poppler-utils 
+   ```
+
+3. **Installing python and pip (if pip is not installed)**
+
+   ```bash
+   sudo apt install python==3.6.9
+   ```
+
+4. **Installing packages for AksharaJaana**
+
+   ```bash
+   pip install AksharaJaana
+   ```
+
+### Windows
+
+1. Installing tesseract-ocr in the system
+   - **Download tesseract**
+     - go to the <a href="https://github.com/UB-Mannheim/tesseract/wiki">website</a>
+     - click on `tesseract-ocr-w64-setup-v5.0.0-alpha.20200328.exe (64 bit)`.
+   - **Install tesseract for Kannada Language and Script**
+     - open the downloaded file and click next and accept the agreement.
+     - Next you will give an option to choose the languages.
+     - **Choose kannada in both script and language**
+   - **Add tesseract to Path**
+     - Check if this folder `C:\Program Files\Tesseract-OCR\` is present. If yes, follow below procedure
+     - Add `C:\Program Files\Tesseract-OCR\`  to your system PATH by doing the following
+        1. Click on the `Windows start button`, search for `Edit the system environment variables`, click on Environment Variables
+        2. Under System variables, look for and double-click on PATH, click on `New`.
+        3. then add `C:\Program Files\Tesseract-OCR\`, click OK.
+     - if folder is not present, manually add the folder tesseract-ocr to the Program Files in the C drive which must be present at the download section (after extraction) and follow the same procedure
+     - See complete [docs](docs/tesseract_installation/README.md).
+
+2. Installing poppler in the system
+
+    - **Download Poppler**
+      - go to <a href="http://blog.alivate.com.au/poppler-windows/">this</a> page
+      - click on `poppler-0.54_x86`
+    - **Unzip** the file and copy files to `C:\Users\Program Files\poppler-0.68.0_x86`
+    - **Add poppler to path**
+      - Add `C:\Program Files\poppler-0.68.0_x86\bin` to your system PATH by doing the following:
+        1. Click on the Windows start button, search for Edit the system environment variables, click on Environment Variables
+        2. under System variables, look for and double-click on PATH, click on New
+        3. then add C:\Users\Program Files\poppler-0.68.0_x86\bin, click OK.
+
+3. Installing python and pip in the system (If pip is not installed)
+   - <a href="https://www.python.org/downloads/">Download python</a>
+
+4. Installing packages for AksharaJaana
+   - open command prompt
+
+     ```bash
+     pip install AksharaJaana
+     ```
+
+5. **Reboot** the system before starting to use
+
+### Python Script
+
+```python
+import AksharaJaana.main as ak 
+text = ak.ocr_engine("Your file Path") 
+print(text) 
+```
+
+
```

#### html2text {}

```diff
@@ -1,33 +1,29 @@
-Metadata-Version: 2.1 Name: AksharaJaana Version: 0.2.1.0 Summary: A Kannada
+Metadata-Version: 2.1 Name: AksharaJaana Version: 1.0.0.1 Summary: A Kannada
 OCR Home-page: https://github.com/Navaneeth-Sharma/Akshara-Jaana/ Author:
-Navaneeth Author-email: navaneethsharma2310oct@gmail.com Classifier:
-Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
-License Classifier: Operating System :: OS Independent Requires-Python: >=3.6
-Description-Content-Type: text/markdown # AksharaJaana
- [https://user-images.githubusercontent.com/63489382/173864136-118db121-fcf4-
-                          4c8a-9b7d-7c4e4c0e48f9.png]
-                              An OCR for Kannada.
-                                    [pypi]
-AksharaJaana is a package which uses tesseract ocr in the backend to convert
-the read-only kannada text to editable format. A Special feature of this is it
-can separate columns in the page and thus making it easier to read and edit. Do
-consider using this package if necessary and feel free to mail me for any
-clarifications. - Email : navaneethsharma2310oct@gmail.com - Twitter handle:
-https://twitter.com/navaneethakbh Happy coding and installing. To see the
-python package visit https://pypi.org/project/AksharaJaana/ ## The Requirements
-***Conda environment is preferred for the smooth use*** - AksharaJaana *(pip
-package)*, check out the latest version available - Tesseract - poppler ##
-Details for Installation ### Ubuntu Open terminal and execute below commands.
-1. **Installing tesseract-ocr in the system** ```bash sudo apt-get update -
-y sudo apt-get install -y tesseract-ocr ``` 2. **Installing poppler in the
-system** ```bash sudo apt-get install -y poppler-utils ``` 3. **Installing
-python and pip (if pip is not installed)** ```bash sudo apt install
-python==3.6.9 ``` 4. **Installing packages for AksharaJaana** ```bash pip
-install --upgrade AksharaJaana ``` ### Windows 1. Installing tesseract-ocr in
+Navaneeth Author-email: navaneethsharma2310oct@gmail.com License: UNKNOWN
+Platform: UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier:
+License :: OSI Approved :: MIT License Classifier: Operating System :: OS
+Independent Requires-Python: >=3.6 Description-Content-Type: text/markdown #
+AksharaJaana AksharaJaana is a package which uses tesseract ocr in the backend
+to convert the read-only kannada text to editable format. A Special feature of
+this is it can separate columns in the page and thus making it easier to read
+and edit. Do consider using this package if necessary and feel free to mail me
+for any clarifications. - Email : navaneethsharma2310oct@gmail.com - Twitter
+handle: https://twitter.com/navaneethakbh Happy coding and installing. To see
+the python package visit https://pypi.org/project/AksharaJaana/ ## The
+Requirements ***Conda environment is preferred for the smooth use*** -
+AksharaJaana *(pip package)*, check out the latest version available -
+Tesseract - poppler ## Details for Installation ### Ubuntu Open terminal and
+execute below commands. 1. **Installing tesseract-ocr in the system** ```bash
+sudo apt-get update -y sudo apt-get install -y tesseract-ocr ``` 2.
+**Installing poppler in the system** ```bash sudo apt-get install -y poppler-
+utils ``` 3. **Installing python and pip (if pip is not installed)** ```bash
+sudo apt install python==3.6.9 ``` 4. **Installing packages for AksharaJaana**
+```bash pip install AksharaJaana ``` ### Windows 1. Installing tesseract-ocr in
 the system - **Download tesseract** - go to the website - click on `tesseract-
 ocr-w64-setup-v5.0.0-alpha.20200328.exe (64 bit)`. - **Install tesseract for
 Kannada Language and Script** - open the downloaded file and click next and
 accept the agreement. - Next you will give an option to choose the languages. -
 **Choose kannada in both script and language** - **Add tesseract to Path** -
 Check if this folder `C:\Program Files\Tesseract-OCR\` is present. If yes,
 follow below procedure - Add `C:\Program Files\Tesseract-OCR\` to your system
```

### Comparing `AksharaJaana-0.2.1.0/README.md` & `AksharaJaana-1.0.0.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,9 @@
 # AksharaJaana
 
-<p align="center">
-     <img src="https://user-images.githubusercontent.com/63489382/173864136-118db121-fcf4-4c8a-9b7d-7c4e4c0e48f9.png" width=200px>
-</p>
-
-<p align="center">
-   An OCR for Kannada.
-</p>
-
-<p align="center">
-   <a href="https://www.npmjs.com/package/@swc/core">
-     <a href="https://pypi.org/project/AksharaJaana/"><img src="https://img.shields.io/badge/pypi-package-blue?labelColor=black&style=flat&logo=python&link=https://pypi.org/project/AksharaJaana/" alt="pypi" /></a>
-   </a>
-</p>
-
 AksharaJaana is a package which uses tesseract ocr in the backend to convert the read-only kannada text to editable format.
 A Special feature of this is it can separate columns in the page and thus making it easier to read and edit.
 Do consider using this  package if necessary and feel free to mail me for any clarifications.
 
 - Email : navaneethsharma2310oct@gmail.com
 - Twitter handle: https://twitter.com/navaneethakbh
 
@@ -57,15 +43,15 @@
    ```bash
    sudo apt install python==3.6.9
    ```
 
 4. **Installing packages for AksharaJaana**
 
    ```bash
-   pip install --upgrade AksharaJaana
+   pip install AksharaJaana
    ```
 
 ### Windows
 
 1. Installing tesseract-ocr in the system
    - **Download tesseract**
      - go to the <a href="https://github.com/UB-Mannheim/tesseract/wiki">website</a>
```

#### html2text {}

```diff
@@ -1,48 +1,43 @@
-# AksharaJaana
- [https://user-images.githubusercontent.com/63489382/173864136-118db121-fcf4-
-                          4c8a-9b7d-7c4e4c0e48f9.png]
-                              An OCR for Kannada.
-                                    [pypi]
-AksharaJaana is a package which uses tesseract ocr in the backend to convert
-the read-only kannada text to editable format. A Special feature of this is it
-can separate columns in the page and thus making it easier to read and edit. Do
-consider using this package if necessary and feel free to mail me for any
-clarifications. - Email : navaneethsharma2310oct@gmail.com - Twitter handle:
-https://twitter.com/navaneethakbh Happy coding and installing. To see the
-python package visit https://pypi.org/project/AksharaJaana/ ## The Requirements
-***Conda environment is preferred for the smooth use*** - AksharaJaana *(pip
-package)*, check out the latest version available - Tesseract - poppler ##
-Details for Installation ### Ubuntu Open terminal and execute below commands.
-1. **Installing tesseract-ocr in the system** ```bash sudo apt-get update -
-y sudo apt-get install -y tesseract-ocr ``` 2. **Installing poppler in the
-system** ```bash sudo apt-get install -y poppler-utils ``` 3. **Installing
-python and pip (if pip is not installed)** ```bash sudo apt install
-python==3.6.9 ``` 4. **Installing packages for AksharaJaana** ```bash pip
-install --upgrade AksharaJaana ``` ### Windows 1. Installing tesseract-ocr in
-the system - **Download tesseract** - go to the website - click on `tesseract-
-ocr-w64-setup-v5.0.0-alpha.20200328.exe (64 bit)`. - **Install tesseract for
-Kannada Language and Script** - open the downloaded file and click next and
-accept the agreement. - Next you will give an option to choose the languages. -
-**Choose kannada in both script and language** - **Add tesseract to Path** -
-Check if this folder `C:\Program Files\Tesseract-OCR\` is present. If yes,
-follow below procedure - Add `C:\Program Files\Tesseract-OCR\` to your system
-PATH by doing the following 1. Click on the `Windows start button`, search for
-`Edit the system environment variables`, click on Environment Variables 2.
-Under System variables, look for and double-click on PATH, click on `New`. 3.
-then add `C:\Program Files\Tesseract-OCR\`, click OK. - if folder is not
-present, manually add the folder tesseract-ocr to the Program Files in the C
-drive which must be present at the download section (after extraction) and
-follow the same procedure - See complete [docs](docs/tesseract_installation/
-README.md). 2. Installing poppler in the system - **Download Poppler** - go to
-this page - click on `poppler-0.54_x86` - **Unzip** the file and copy files to
-`C:\Users\Program Files\poppler-0.68.0_x86` - **Add poppler to path** - Add `C:
-\Program Files\poppler-0.68.0_x86\bin` to your system PATH by doing the
-following: 1. Click on the Windows start button, search for Edit the system
-environment variables, click on Environment Variables 2. under System
-variables, look for and double-click on PATH, click on New 3. then add C:
-\Users\Program Files\poppler-0.68.0_x86\bin, click OK. 3. Installing python and
-pip in the system (If pip is not installed) - Download_python 4. Installing
-packages for AksharaJaana - open command prompt ```bash pip install
-AksharaJaana ``` 5. **Reboot** the system before starting to use ### Python
-Script ```python import AksharaJaana.main as ak text = ak.ocr_engine("Your file
-Path") print(text) ```
+# AksharaJaana AksharaJaana is a package which uses tesseract ocr in the
+backend to convert the read-only kannada text to editable format. A Special
+feature of this is it can separate columns in the page and thus making it
+easier to read and edit. Do consider using this package if necessary and feel
+free to mail me for any clarifications. - Email :
+navaneethsharma2310oct@gmail.com - Twitter handle: https://twitter.com/
+navaneethakbh Happy coding and installing. To see the python package visit
+https://pypi.org/project/AksharaJaana/ ## The Requirements ***Conda environment
+is preferred for the smooth use*** - AksharaJaana *(pip package)*, check out
+the latest version available - Tesseract - poppler ## Details for Installation
+### Ubuntu Open terminal and execute below commands. 1. **Installing tesseract-
+ocr in the system** ```bash sudo apt-get update -y sudo apt-get install -
+y tesseract-ocr ``` 2. **Installing poppler in the system** ```bash sudo apt-
+get install -y poppler-utils ``` 3. **Installing python and pip (if pip is not
+installed)** ```bash sudo apt install python==3.6.9 ``` 4. **Installing
+packages for AksharaJaana** ```bash pip install AksharaJaana ``` ### Windows 1.
+Installing tesseract-ocr in the system - **Download tesseract** - go to the
+website - click on `tesseract-ocr-w64-setup-v5.0.0-alpha.20200328.exe (64
+bit)`. - **Install tesseract for Kannada Language and Script** - open the
+downloaded file and click next and accept the agreement. - Next you will give
+an option to choose the languages. - **Choose kannada in both script and
+language** - **Add tesseract to Path** - Check if this folder `C:\Program
+Files\Tesseract-OCR\` is present. If yes, follow below procedure - Add `C:
+\Program Files\Tesseract-OCR\` to your system PATH by doing the following 1.
+Click on the `Windows start button`, search for `Edit the system environment
+variables`, click on Environment Variables 2. Under System variables, look for
+and double-click on PATH, click on `New`. 3. then add `C:\Program
+Files\Tesseract-OCR\`, click OK. - if folder is not present, manually add the
+folder tesseract-ocr to the Program Files in the C drive which must be present
+at the download section (after extraction) and follow the same procedure - See
+complete [docs](docs/tesseract_installation/README.md). 2. Installing poppler
+in the system - **Download Poppler** - go to this page - click on `poppler-
+0.54_x86` - **Unzip** the file and copy files to `C:\Users\Program
+Files\poppler-0.68.0_x86` - **Add poppler to path** - Add `C:\Program
+Files\poppler-0.68.0_x86\bin` to your system PATH by doing the following: 1.
+Click on the Windows start button, search for Edit the system environment
+variables, click on Environment Variables 2. under System variables, look for
+and double-click on PATH, click on New 3. then add C:\Users\Program
+Files\poppler-0.68.0_x86\bin, click OK. 3. Installing python and pip in the
+system (If pip is not installed) - Download_python 4. Installing packages for
+AksharaJaana - open command prompt ```bash pip install AksharaJaana ``` 5.
+**Reboot** the system before starting to use ### Python Script ```python import
+AksharaJaana.main as ak text = ak.ocr_engine("Your file Path") print(text) ```
```

