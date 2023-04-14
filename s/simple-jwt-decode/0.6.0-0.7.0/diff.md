# Comparing `tmp/simple_jwt_decode-0.6.0.tar.gz` & `tmp/simple_jwt_decode-0.7.0.tar.gz`

## Comparing `simple_jwt_decode-0.6.0.tar` & `simple_jwt_decode-0.7.0.tar`

### file list

```diff
@@ -1,10 +1,12 @@
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 simple_jwt_decode-0.6.0/src/simple_jwt/__about__.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 simple_jwt_decode-0.6.0/src/simple_jwt/__init__.py
--rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 simple_jwt_decode-0.6.0/src/simple_jwt/jwt.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 simple_jwt_decode-0.6.0/tests/__init__.py
--rw-r--r--   0        0        0     3820 2020-02-02 00:00:00.000000 simple_jwt_decode-0.6.0/tests/test_jwt.py
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 simple_jwt_decode-0.6.0/.gitignore
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 simple_jwt_decode-0.6.0/LICENSE.txt
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 simple_jwt_decode-0.6.0/README.md
--rw-r--r--   0        0        0     3329 2020-02-02 00:00:00.000000 simple_jwt_decode-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     2714 2020-02-02 00:00:00.000000 simple_jwt_decode-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 simple_jwt_decode-0.7.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 simple_jwt_decode-0.7.0/requirements-dev.txt
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 simple_jwt_decode-0.7.0/src/simple_jwt/__about__.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 simple_jwt_decode-0.7.0/src/simple_jwt/__init__.py
+-rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 simple_jwt_decode-0.7.0/src/simple_jwt/jwt.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 simple_jwt_decode-0.7.0/tests/__init__.py
+-rw-r--r--   0        0        0     3878 2020-02-02 00:00:00.000000 simple_jwt_decode-0.7.0/tests/jwt_test.py
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 simple_jwt_decode-0.7.0/.gitignore
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 simple_jwt_decode-0.7.0/LICENSE.txt
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 simple_jwt_decode-0.7.0/README.md
+-rw-r--r--   0        0        0     3382 2020-02-02 00:00:00.000000 simple_jwt_decode-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     2714 2020-02-02 00:00:00.000000 simple_jwt_decode-0.7.0/PKG-INFO
```

### Comparing `simple_jwt_decode-0.6.0/src/simple_jwt/jwt.py` & `simple_jwt_decode-0.7.0/src/simple_jwt/jwt.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,48 +1,57 @@
+from __future__ import annotations
+
 import base64
+import binascii
 import json
 from time import time
 
+
 def decode(token: str | bytes) -> dict:
     """Decode a JWT token.
 
     Args:
         token (str | bytes): The token to decode.
 
     Returns:
         dict: The decoded token without the verification of signature.
     """
     if isinstance(token, bytes):
         token = token.decode()
     if not isinstance(token, str):
-        raise TypeError("Invalid token: token must be a string or bytes")
+        raise TypeError('Invalid token: token must be a string or bytes')
 
     try:
-        headers, claims, signature = token.split(".")
+        headers, claims, signature = token.split('.')
     except ValueError:
-        raise ValueError("Invalid token: token must have 3 parts separated by '.'")
-    
+        raise ValueError(
+            "Invalid token: token must have 3 parts separated by '.'",
+        )
+
     try:
         header_decoded = base64.b64decode(headers)
         claims_decoded = base64.b64decode(claims)
-    except base64.binascii.Error:
-        raise base64.binascii.Error("Invalid token: token must be base64 encoded")
-    
+    except binascii.Error:
+        raise binascii.Error(
+            'Invalid token: token must be base64 encoded',
+        )
+
     # try:
     header_data = json.loads(header_decoded)
     claims_data = json.loads(claims_decoded)
     # except json.JSONDecodeError:
-        # print("Invalid token: token must be json encoded")
+    # print("Invalid token: token must be json encoded")
+
+    return {'headers': header_data, 'claims': claims_data, 'signature': signature}
 
-    return {"headers": header_data, "claims": claims_data, "signature": signature}
 
 def is_expired(token: str | bytes) -> bool:
     """Check if a JWT token is expired.
 
     Args:
         token (str | bytes): The token to check.
 
     Returns:
         bool: True if the token is expired, False otherwise.
     """
     decoded = decode(token)
-    return decoded["claims"]["exp"] < time()
+    return decoded['claims']['exp'] < time()
```

### Comparing `simple_jwt_decode-0.6.0/tests/test_jwt.py` & `simple_jwt_decode-0.7.0/tests/jwt_test.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,59 +1,71 @@
-from simple_jwt import jwt
+from __future__ import annotations
+
 import base64
+import binascii
 import json
 from time import time
+
 import pytest
+from simple_jwt import jwt
 
 param = 'eyJhbGciOiJIUzUxMiJ9.eyJleHAiOjE2ODEzMzcyNTYsImlhdCI6MTY4MTMzMzY1Niwic2lkIjoiMTUzMDcxNjQyNzYiLCJhaWQiOiI4NjUyNTk4MDg1IiwiY2lkIjoiNTA0MzA3MDIiLCJ0eXBlIjoiciJ9.jmFoOydgYnL8AqmgnLSFU2l_E6q3pnPHh7ss-g7xKO7tLD_JY8vZR3O-cthNInFzi9G2M3t2boRzMTatlbsZ7Q'
 
+
 @pytest.fixture
 def token() -> str:
     return 'eyJhbGciOiJIUzUxMiJ9.eyJleHAiOjE2ODEzMzcyNTYsImlhdCI6MTY4MTMzMzY1Niwic2lkIjoiMTUzMDcxNjQyNzYiLCJhaWQiOiI4NjUyNTk4MDg1IiwiY2lkIjoiNTA0MzA3MDIiLCJ0eXBlIjoiciJ9.jmFoOydgYnL8AqmgnLSFU2l_E6q3pnPHh7ss-g7xKO7tLD_JY8vZR3O-cthNInFzi9G2M3t2boRzMTatlbsZ7Q'
+
+
 @pytest.fixture
 def too_many_segments() -> str:
     return 'eyJhbGciOiJIUzUxMiJ9.eyJleHAiOjE2ODEzMzcyNTYsImlhdCI6MTY4MTMzMzY1Niwic2lkIjoiMTUzMDcxNjQyNzYiLCJhaWQiOiI4NjUyNTk4MDg1IiwiY2lkIjoiNTA0MzA3MDIiLCJ0eXBlIjoiciJ9.jmFoOydgYnL8AqmgnLSFU2l_E6q3pnPHh7ss-g7xKO7tLD_JY8vZR3O-cthNInFzi9G2M3t2.boRzMTatlbsZ7Q'
+
+
 @pytest.fixture
 def invalid_base64() -> str:
     return 'eyJhbGciOiJIUzUxMiJ9.eyJleHAiOjE2ODEzMzcyNTYsImlhdCI6MTY4MTMzMzY1Niwic2lkIjoiMTUzMDcxNjQyNzYiLCJhaWQiOiI4NjUyNTk4MDg1IiwiY2lkIjoiNTA0MzA3MDIiLCJ0eXBlIjoiciJ.jmFoOydgYnL8AqmgnLSFU2l_E6q3pnPHh7ss-g7xKO7tLD_JY8vZR3O-cthNInFzi9G2M3t2boRzMTatlbsZ7Q'
 
+
 @pytest.fixture
 def active_token() -> str:
-    claims =  {
-        "exp": int(time()) + 3600,
-        "iat": int(time()),
-        "sid": "15307164276",
-        "aid": "8652598085",
-        "cid": "50430702",
-        "type": "r"
+    claims = {
+        'exp': int(time()) + 3600,
+        'iat': int(time()),
+        'sid': '15307164276',
+        'aid': '8652598085',
+        'cid': '50430702',
+        'type': 'r',
     }
     input = json.dumps(claims).encode('utf-8')
     payload = base64.urlsafe_b64encode(input)
     header = 'eyJhbGciOiJIUzUxMiJ9'
     fake_sig = 'SflKxwRJSMeKKF2QT4fwpMeJf36POk6yJV_adQssw5c'
     active_token = f'{header}.{payload.decode()}.{fake_sig}'
     return active_token
 
+
 @pytest.fixture
 def bad_json_token() -> str:
-    claims =  {
-        "exp": int(time()) + 3600,
-        "iat": int(time()),
-        "sid": "15307164276",
-        "aid": "8652598085",
-        "cid": "50430702",
-        "type": "r"
+    claims = {
+        'exp': int(time()) + 3600,
+        'iat': int(time()),
+        'sid': '15307164276',
+        'aid': '8652598085',
+        'cid': '50430702',
+        'type': 'r',
     }
     input = json.dumps(claims).encode('utf-8') + b'bad'
     payload = base64.urlsafe_b64encode(input)
     header = 'eyJhbGciOiJIUzUxMiJ9'
     fake_sig = 'SflKxwRJSMeKKF2QT4fwpMeJf36POk6yJV_adQssw5c'
     active_token = f'{header}.{payload.decode()}.{fake_sig}'
     return active_token
 
+
 def test_decode(token: str):
     decoded = jwt.decode(token)
     assert decoded['headers']['alg'] == 'HS512'
     assert decoded['claims']['exp'] == 1681337256
     assert decoded['claims']['iat'] == 1681333656
     assert decoded['claims']['sid'] == '15307164276'
     assert decoded['claims']['aid'] == '8652598085'
@@ -62,39 +74,43 @@
     assert decoded['signature'] == 'jmFoOydgYnL8AqmgnLSFU2l_E6q3pnPHh7ss-g7xKO7tLD_JY8vZR3O-cthNInFzi9G2M3t2boRzMTatlbsZ7Q'
 
 
 def test_decode_too_many_segments(too_many_segments: str):
     with pytest.raises(ValueError):
         jwt.decode(too_many_segments)
 
+
 def test_invalid_base64(invalid_base64: str):
-    with pytest.raises(base64.binascii.Error):
+    with pytest.raises(binascii.Error):
         jwt.decode(invalid_base64)
 
+
 def test_json_encoded(bad_json_token: str):
     with pytest.raises(json.JSONDecodeError):
         jwt.decode(bad_json_token)
 
 
 def test_expired_token(token: str):
     assert jwt.is_expired(token)
 
+
 def test_not_expired_token(active_token: str):
     assert not jwt.is_expired(active_token)
 
 
 class does_not_raise:
     def __enter__(self):
         pass
 
     def __exit__(self, *args):
         pass
 
+
 @pytest.mark.parametrize(
-    "test_input, expected",
+    'test_input, expected',
     [
         (123, pytest.raises(TypeError)),
         ({token: param}, pytest.raises(TypeError)),
         (param, does_not_raise()),
         (bytes(param, 'utf-8'), does_not_raise()),
     ],
 )
```

### Comparing `simple_jwt_decode-0.6.0/.gitignore` & `simple_jwt_decode-0.7.0/.gitignore`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,11 @@
-
 __pycache__/
 *.py[cod]
 *$py.class
-
 *.so
-
 .Python
 build/
 develop-eggs/
 dist/
 downloads/
 eggs/
 .eggs/
@@ -19,94 +16,65 @@
 var/
 wheels/
 share/python-wheels/
 *.egg-info/
 .installed.cfg
 *.egg
 MANIFEST
-
 *.manifest
 *.spec
-
 pip-log.txt
 pip-delete-this-directory.txt
-
 htmlcov/
 .tox/
 .nox/
 .coverage
 .coverage.*
 .cache
 nosetests.xml
 coverage.xml
 *.cover
 *.py,cover
 .hypothesis/
 .pytest_cache/
 cover/
-
 *.mo
 *.pot
-
 *.log
 local_settings.py
 db.sqlite3
 db.sqlite3-journal
-
 instance/
 .webassets-cache
-
 .scrapy
-
 docs/_build/
-
 .pybuilder/
 target/
-
 .ipynb_checkpoints
-
 profile_default/
 ipython_config.py
-
-
-
-
 .pdm.toml
-
 __pypackages__/
-
 celerybeat-schedule
 celerybeat.pid
-
 *.sage.py
-
 .env
 .venv
 env/
 venv/
 ENV/
 env.bak/
 venv.bak/
-
 .spyderproject
 .spyproject
-
 .ropeproject
-
 /site
-
 .mypy_cache/
 .dmypy.json
 dmypy.json
-
 .pyre/
-
 .pytype/
-
 cython_debug/
-
-
 poetry.toml
-
 .ruff_cache/
-
-pyrightconfig.json
+pyrightconfig.json
+.python-version
```

### Comparing `simple_jwt_decode-0.6.0/LICENSE.txt` & `simple_jwt_decode-0.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `simple_jwt_decode-0.6.0/README.md` & `simple_jwt_decode-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `simple_jwt_decode-0.6.0/pyproject.toml` & `simple_jwt_decode-0.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -153,8 +153,13 @@
 tests = ["tests", "*/simple-jwt/tests"]
 
 [tool.coverage.report]
 exclude_lines = [
   "no cov",
   "if __name__ == .__main__.:",
   "if TYPE_CHECKING:",
-]
+]
+
+[tool.pytest.ini_options]
+pythonpath = [
+  "src"
+]
```

### Comparing `simple_jwt_decode-0.6.0/PKG-INFO` & `simple_jwt_decode-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-jwt-decode
-Version: 0.6.0
+Version: 0.7.0
 Summary: Simple Python Package for decoding JWT claims and checking if its expired. No verification of signatures.
 Project-URL: Documentation, https://github.com/u-clarkdeveloper/simple-jwt#readme
 Project-URL: Issues, https://github.com/u-clarkdeveloper/simple-jwt/issues
 Project-URL: Source, https://github.com/u-clarkdeveloper/simple-jwt
 Author-email: Jesse Clark <jesse@clarkdeveloper.com>
 License-Expression: MIT
 License-File: LICENSE.txt
```

