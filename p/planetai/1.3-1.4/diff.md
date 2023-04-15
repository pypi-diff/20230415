# Comparing `tmp/planetai-1.3.tar.gz` & `tmp/planetai-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "planetai-1.3.tar", last modified: Sat Apr 15 11:36:28 2023, max compression
+gzip compressed data, was "planetai-1.4.tar", last modified: Sat Apr 15 12:24:50 2023, max compression
```

## Comparing `planetai-1.3.tar` & `planetai-1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 11:36:28.542544 planetai-1.3/
--rw-rw-rw-   0        0        0      137 2023-04-15 11:36:28.542544 planetai-1.3/PKG-INFO
--rw-rw-rw-   0        0        0      317 2023-04-15 11:11:06.000000 planetai-1.3/README.md
--rw-rw-rw-   0        0        0     1066 2023-04-15 10:41:38.000000 planetai-1.3/license.txt
-drwxrwxrwx   0        0        0        0 2023-04-15 11:36:28.432227 planetai-1.3/planetai/
--rw-rw-rw-   0        0        0       27 2023-04-15 11:31:24.000000 planetai-1.3/planetai/__init__.py
--rw-rw-rw-   0        0        0       35 2023-04-15 11:10:33.000000 planetai-1.3/planetai/main.py
--rw-rw-rw-   0        0        0     3047 2023-04-15 11:35:38.000000 planetai-1.3/planetai/planet.py
-drwxrwxrwx   0        0        0        0 2023-04-15 11:36:28.540545 planetai-1.3/planetai.egg-info/
--rw-rw-rw-   0        0        0      137 2023-04-15 11:36:28.000000 planetai-1.3/planetai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      256 2023-04-15 11:36:28.000000 planetai-1.3/planetai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 11:36:28.000000 planetai-1.3/planetai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-15 11:36:28.000000 planetai-1.3/planetai.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        9 2023-04-15 11:36:28.000000 planetai-1.3/planetai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-04-15 11:36:28.543544 planetai-1.3/setup.cfg
--rw-rw-rw-   0        0        0      331 2023-04-15 11:35:44.000000 planetai-1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 12:24:50.029624 planetai-1.4/
+-rw-rw-rw-   0        0        0      137 2023-04-15 12:24:50.029624 planetai-1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      317 2023-04-15 11:11:06.000000 planetai-1.4/README.md
+-rw-rw-rw-   0        0        0     1066 2023-04-15 10:41:38.000000 planetai-1.4/license.txt
+drwxrwxrwx   0        0        0        0 2023-04-15 12:24:49.891331 planetai-1.4/planetai/
+-rw-rw-rw-   0        0        0       27 2023-04-15 11:31:24.000000 planetai-1.4/planetai/__init__.py
+-rw-rw-rw-   0        0        0       35 2023-04-15 11:10:33.000000 planetai-1.4/planetai/main.py
+-rw-rw-rw-   0        0        0     3037 2023-04-15 12:22:18.000000 planetai-1.4/planetai/planet.py
+drwxrwxrwx   0        0        0        0 2023-04-15 12:24:50.028622 planetai-1.4/planetai.egg-info/
+-rw-rw-rw-   0        0        0      137 2023-04-15 12:24:49.000000 planetai-1.4/planetai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      256 2023-04-15 12:24:49.000000 planetai-1.4/planetai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 12:24:49.000000 planetai-1.4/planetai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-15 12:24:49.000000 planetai-1.4/planetai.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        9 2023-04-15 12:24:49.000000 planetai-1.4/planetai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-04-15 12:24:50.034624 planetai-1.4/setup.cfg
+-rw-rw-rw-   0        0        0      331 2023-04-15 12:22:48.000000 planetai-1.4/setup.py
```

### Comparing `planetai-1.3/license.txt` & `planetai-1.4/license.txt`

 * *Files identical despite different names*

### Comparing `planetai-1.3/planetai/planet.py` & `planetai-1.4/planetai/planet.py`

 * *Files 6% similar despite different names*

```diff
@@ -63,11 +63,11 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 THE SOFTWARE.""")
 
     def license():
-        print('Kuwinda Corp. License')
+        print('MIT License')
 
     def credits():
         print('Author: Aziz Brown \n https://kuwindacorp.com/ \n github: https://github.com/sageofnamek')
```

