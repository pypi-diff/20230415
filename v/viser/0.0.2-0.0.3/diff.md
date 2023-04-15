# Comparing `tmp/viser-0.0.2.tar.gz` & `tmp/viser-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "viser-0.0.2.tar", max compression
+gzip compressed data, was "viser-0.0.3.tar", max compression
```

## Comparing `viser-0.0.2.tar` & `viser-0.0.3.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0     1791 2023-04-14 20:35:30.495308 viser-0.0.2/README.md
--rw-r--r--   0        0        0      655 2023-04-14 20:35:30.495308 viser-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      578 2023-04-14 20:35:30.495308 viser-0.0.2/viser/__init__.py
--rw-r--r--   0        0        0     5503 2023-04-14 20:35:30.495308 viser-0.0.2/viser/_gui.py
--rw-r--r--   0        0        0    21128 2023-04-14 20:35:30.495308 viser-0.0.2/viser/_message_api.py
--rw-r--r--   0        0        0     5918 2023-04-14 20:35:30.495308 viser-0.0.2/viser/_messages.py
--rw-r--r--   0        0        0     3249 2023-04-14 20:35:30.495308 viser-0.0.2/viser/_scene_handle.py
--rw-r--r--   0        0        0     4146 2023-04-14 20:35:30.495308 viser-0.0.2/viser/_viser.py
--rw-r--r--   0        0        0     1115 2023-04-14 20:35:30.495308 viser-0.0.2/viser/client/.eslintrc.js
--rw-r--r--   0        0        0      289 2023-04-14 20:35:30.495308 viser-0.0.2/viser/client/.gitignore
--rw-r--r--   0        0        0     2117 2023-04-14 20:35:30.495308 viser-0.0.2/viser/client/README.md
--rw-r--r--   0        0        0      369 2023-04-14 20:35:30.495308 viser-0.0.2/viser/client/build/asset-manifest.json
--rw-r--r--   0        0        0     1800 2023-04-14 20:35:30.495308 viser-0.0.2/viser/client/build/favicon.svg
--rw-r--r--   0        0        0      640 2023-04-14 20:35:30.495308 viser-0.0.2/viser/client/build/index.html
--rw-r--r--   0        0        0      286 2023-04-14 20:35:30.495308 viser-0.0.2/viser/client/build/manifest.json
--rw-r--r--   0        0        0       67 2023-04-14 20:35:30.495308 viser-0.0.2/viser/client/build/robots.txt
--rw-r--r--   0        0        0      441 2023-04-14 20:35:30.495308 viser-0.0.2/viser/client/build/static/css/main.992126cd.css
--rw-r--r--   0        0        0      843 2023-04-14 20:35:30.495308 viser-0.0.2/viser/client/build/static/css/main.992126cd.css.map
--rw-r--r--   0        0        0  1510463 2023-04-14 20:35:30.503308 viser-0.0.2/viser/client/build/static/js/main.721d9a9f.js
--rw-r--r--   0        0        0     4434 2023-04-14 20:35:30.503308 viser-0.0.2/viser/client/build/static/js/main.721d9a9f.js.LICENSE.txt
--rw-r--r--   0        0        0  5161937 2023-04-14 20:35:30.531309 viser-0.0.2/viser/client/build/static/js/main.721d9a9f.js.map
--rw-r--r--   0        0        0     1910 2023-04-14 20:35:30.531309 viser-0.0.2/viser/client/package.json
--rw-r--r--   0        0        0     1800 2023-04-14 20:35:30.531309 viser-0.0.2/viser/client/public/favicon.svg
--rw-r--r--   0        0        0     1717 2023-04-14 20:35:30.531309 viser-0.0.2/viser/client/public/index.html
--rw-r--r--   0        0        0      286 2023-04-14 20:35:30.531309 viser-0.0.2/viser/client/public/manifest.json
--rw-r--r--   0        0        0       67 2023-04-14 20:35:30.531309 viser-0.0.2/viser/client/public/robots.txt
--rw-r--r--   0        0        0     7126 2023-04-14 20:35:30.531309 viser-0.0.2/viser/client/src/CameraControls.tsx
--rw-r--r--   0        0        0    11080 2023-04-14 20:35:30.531309 viser-0.0.2/viser/client/src/ControlPanel/ControlPanel.tsx
--rw-r--r--   0        0        0     5790 2023-04-14 20:35:30.531309 viser-0.0.2/viser/client/src/ControlPanel/Generated.tsx
--rw-r--r--   0        0        0     2307 2023-04-14 20:35:30.531309 viser-0.0.2/viser/client/src/ControlPanel/GuiState.tsx
--rw-r--r--   0        0        0     3802 2023-04-14 20:35:30.531309 viser-0.0.2/viser/client/src/ControlPanel/SceneTreeUI.tsx
--rw-r--r--   0        0        0     2154 2023-04-14 20:35:30.531309 viser-0.0.2/viser/client/src/ControlPanel/Server.tsx
--rw-r--r--   0        0        0     1120 2023-04-14 20:35:30.531309 viser-0.0.2/viser/client/src/LabelRenderer.tsx
--rw-r--r--   0        0        0     7338 2023-04-14 20:35:30.531309 viser-0.0.2/viser/client/src/SceneTree.tsx
--rw-r--r--   0        0        0     1678 2023-04-14 20:35:30.531309 viser-0.0.2/viser/client/src/SearchParamsUtils.tsx
--rw-r--r--   0        0        0     3840 2023-04-14 20:35:30.531309 viser-0.0.2/viser/client/src/ThreeAssets.tsx
--rw-r--r--   0        0        0    14773 2023-04-14 20:35:30.531309 viser-0.0.2/viser/client/src/WebsocketInterface.tsx
--rw-r--r--   0        0        0     3548 2023-04-14 20:35:30.531309 viser-0.0.2/viser/client/src/WebsocketMessages.tsx
--rw-r--r--   0        0        0      509 2023-04-14 20:35:30.531309 viser-0.0.2/viser/client/src/index.css
--rw-r--r--   0        0        0     6406 2023-04-14 20:35:30.531309 viser-0.0.2/viser/client/src/index.tsx
--rw-r--r--   0        0        0       40 2023-04-14 20:35:30.531309 viser-0.0.2/viser/client/src/react-app-env.d.ts
--rw-r--r--   0        0        0      503 2023-04-14 20:35:30.531309 viser-0.0.2/viser/client/tsconfig.json
--rw-r--r--   0        0        0   495759 2023-04-14 20:35:30.531309 viser-0.0.2/viser/client/yarn.lock
--rw-r--r--   0        0        0      160 2023-04-14 20:35:30.531309 viser-0.0.2/viser/extras/__init__.py
--rw-r--r--   0        0        0     4099 2023-04-14 20:35:30.531309 viser-0.0.2/viser/extras/_record3d.py
--rw-r--r--   0        0        0      898 2023-04-14 20:35:30.531309 viser-0.0.2/viser/infra/__init__.py
--rw-r--r--   0        0        0     2994 2023-04-14 20:35:30.531309 viser-0.0.2/viser/infra/_async_message_buffer.py
--rw-r--r--   0        0        0    11095 2023-04-14 20:35:30.531309 viser-0.0.2/viser/infra/_infra.py
--rw-r--r--   0        0        0     2775 2023-04-14 20:35:30.531309 viser-0.0.2/viser/infra/_messages.py
--rw-r--r--   0        0        0     3110 2023-04-14 20:35:30.531309 viser-0.0.2/viser/infra/_typescript_interface_gen.py
--rw-r--r--   0        0        0        0 2023-04-14 20:35:30.535308 viser-0.0.2/viser/py.typed
--rw-r--r--   0        0        0     2623 1970-01-01 00:00:00.000000 viser-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1958 2023-04-15 01:49:43.943343 viser-0.0.3/README.md
+-rw-r--r--   0        0        0      655 2023-04-15 01:49:43.943343 viser-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      578 2023-04-15 01:49:43.943343 viser-0.0.3/viser/__init__.py
+-rw-r--r--   0        0        0     5503 2023-04-15 01:49:43.943343 viser-0.0.3/viser/_gui.py
+-rw-r--r--   0        0        0    21224 2023-04-15 01:49:43.947344 viser-0.0.3/viser/_message_api.py
+-rw-r--r--   0        0        0     5918 2023-04-15 01:49:43.947344 viser-0.0.3/viser/_messages.py
+-rw-r--r--   0        0        0     3249 2023-04-15 01:49:43.947344 viser-0.0.3/viser/_scene_handle.py
+-rw-r--r--   0        0        0     4146 2023-04-15 01:49:43.947344 viser-0.0.3/viser/_viser.py
+-rw-r--r--   0        0        0     1115 2023-04-15 01:49:43.947344 viser-0.0.3/viser/client/.eslintrc.js
+-rw-r--r--   0        0        0      289 2023-04-15 01:49:43.947344 viser-0.0.3/viser/client/.gitignore
+-rw-r--r--   0        0        0     2117 2023-04-15 01:49:43.947344 viser-0.0.3/viser/client/README.md
+-rw-r--r--   0        0        0      369 2023-04-15 01:49:43.947344 viser-0.0.3/viser/client/build/asset-manifest.json
+-rw-r--r--   0        0        0     1800 2023-04-15 01:49:43.947344 viser-0.0.3/viser/client/build/favicon.svg
+-rw-r--r--   0        0        0      640 2023-04-15 01:49:43.947344 viser-0.0.3/viser/client/build/index.html
+-rw-r--r--   0        0        0      286 2023-04-15 01:49:43.947344 viser-0.0.3/viser/client/build/manifest.json
+-rw-r--r--   0        0        0       67 2023-04-15 01:49:43.947344 viser-0.0.3/viser/client/build/robots.txt
+-rw-r--r--   0        0        0      441 2023-04-15 01:49:43.947344 viser-0.0.3/viser/client/build/static/css/main.992126cd.css
+-rw-r--r--   0        0        0      843 2023-04-15 01:49:43.947344 viser-0.0.3/viser/client/build/static/css/main.992126cd.css.map
+-rw-r--r--   0        0        0  1510463 2023-04-15 01:49:43.955344 viser-0.0.3/viser/client/build/static/js/main.721d9a9f.js
+-rw-r--r--   0        0        0     4434 2023-04-15 01:49:43.955344 viser-0.0.3/viser/client/build/static/js/main.721d9a9f.js.LICENSE.txt
+-rw-r--r--   0        0        0  5161937 2023-04-15 01:49:43.983345 viser-0.0.3/viser/client/build/static/js/main.721d9a9f.js.map
+-rw-r--r--   0        0        0     1910 2023-04-15 01:49:43.983345 viser-0.0.3/viser/client/package.json
+-rw-r--r--   0        0        0     1800 2023-04-15 01:49:43.983345 viser-0.0.3/viser/client/public/favicon.svg
+-rw-r--r--   0        0        0     1717 2023-04-15 01:49:43.983345 viser-0.0.3/viser/client/public/index.html
+-rw-r--r--   0        0        0      286 2023-04-15 01:49:43.983345 viser-0.0.3/viser/client/public/manifest.json
+-rw-r--r--   0        0        0       67 2023-04-15 01:49:43.983345 viser-0.0.3/viser/client/public/robots.txt
+-rw-r--r--   0        0        0     7126 2023-04-15 01:49:43.983345 viser-0.0.3/viser/client/src/CameraControls.tsx
+-rw-r--r--   0        0        0    11080 2023-04-15 01:49:43.983345 viser-0.0.3/viser/client/src/ControlPanel/ControlPanel.tsx
+-rw-r--r--   0        0        0     5790 2023-04-15 01:49:43.983345 viser-0.0.3/viser/client/src/ControlPanel/Generated.tsx
+-rw-r--r--   0        0        0     2307 2023-04-15 01:49:43.987345 viser-0.0.3/viser/client/src/ControlPanel/GuiState.tsx
+-rw-r--r--   0        0        0     3802 2023-04-15 01:49:43.987345 viser-0.0.3/viser/client/src/ControlPanel/SceneTreeUI.tsx
+-rw-r--r--   0        0        0     2154 2023-04-15 01:49:43.987345 viser-0.0.3/viser/client/src/ControlPanel/Server.tsx
+-rw-r--r--   0        0        0     1120 2023-04-15 01:49:43.987345 viser-0.0.3/viser/client/src/LabelRenderer.tsx
+-rw-r--r--   0        0        0     7229 2023-04-15 01:49:43.987345 viser-0.0.3/viser/client/src/SceneTree.tsx
+-rw-r--r--   0        0        0     1678 2023-04-15 01:49:43.987345 viser-0.0.3/viser/client/src/SearchParamsUtils.tsx
+-rw-r--r--   0        0        0     3840 2023-04-15 01:49:43.987345 viser-0.0.3/viser/client/src/ThreeAssets.tsx
+-rw-r--r--   0        0        0    14673 2023-04-15 01:49:43.987345 viser-0.0.3/viser/client/src/WebsocketInterface.tsx
+-rw-r--r--   0        0        0     3548 2023-04-15 01:49:43.987345 viser-0.0.3/viser/client/src/WebsocketMessages.tsx
+-rw-r--r--   0        0        0      509 2023-04-15 01:49:43.987345 viser-0.0.3/viser/client/src/index.css
+-rw-r--r--   0        0        0     6406 2023-04-15 01:49:43.987345 viser-0.0.3/viser/client/src/index.tsx
+-rw-r--r--   0        0        0       40 2023-04-15 01:49:43.987345 viser-0.0.3/viser/client/src/react-app-env.d.ts
+-rw-r--r--   0        0        0      503 2023-04-15 01:49:43.987345 viser-0.0.3/viser/client/tsconfig.json
+-rw-r--r--   0        0        0   495759 2023-04-15 01:49:43.987345 viser-0.0.3/viser/client/yarn.lock
+-rw-r--r--   0        0        0      160 2023-04-15 01:49:43.987345 viser-0.0.3/viser/extras/__init__.py
+-rw-r--r--   0        0        0     4099 2023-04-15 01:49:43.987345 viser-0.0.3/viser/extras/_record3d.py
+-rw-r--r--   0        0        0      898 2023-04-15 01:49:43.987345 viser-0.0.3/viser/infra/__init__.py
+-rw-r--r--   0        0        0     2994 2023-04-15 01:49:43.987345 viser-0.0.3/viser/infra/_async_message_buffer.py
+-rw-r--r--   0        0        0    11095 2023-04-15 01:49:43.987345 viser-0.0.3/viser/infra/_infra.py
+-rw-r--r--   0        0        0     2775 2023-04-15 01:49:43.987345 viser-0.0.3/viser/infra/_messages.py
+-rw-r--r--   0        0        0     3110 2023-04-15 01:49:43.987345 viser-0.0.3/viser/infra/_typescript_interface_gen.py
+-rw-r--r--   0        0        0        0 2023-04-15 01:49:43.987345 viser-0.0.3/viser/py.typed
+-rw-r--r--   0        0        0     2790 1970-01-01 00:00:00.000000 viser-0.0.3/PKG-INFO
```

### Comparing `viser-0.0.2/README.md` & `viser-0.0.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -50,10 +50,19 @@
 
 ```bash
 cd ./viser/viser/client
 yarn
 yarn start
 ```
 
-## Interactive SMPL-X Example
+## Demos
+
+### Interactive SMPL-X Example
 
 https://user-images.githubusercontent.com/6992947/228734499-87d8a12a-df1a-4511-a4e0-0a46bd8532fd.mov
+
+
+### Interactive NeRF rendering
+
+(code not released)
+
+https://user-images.githubusercontent.com/6992947/232163875-ff788455-f074-4bd3-9154-5330b5ed4733.mov
```

### Comparing `viser-0.0.2/pyproject.toml` & `viser-0.0.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "viser"
-version = "0.0.2"
+version = "0.0.3"
 description = "3D visualization helper"
 authors = ["brentyi <brentyi@berkeley.edu>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 websockets = ">=10.4"
```

### Comparing `viser-0.0.2/viser/__init__.py` & `viser-0.0.3/viser/__init__.py`

 * *Files identical despite different names*

### Comparing `viser-0.0.2/viser/_gui.py` & `viser-0.0.3/viser/_gui.py`

 * *Files identical despite different names*

### Comparing `viser-0.0.2/viser/_message_api.py` & `viser-0.0.3/viser/_message_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,16 +59,19 @@
 
 
 def _encode_rgb(
     rgb: Tuple[int, int, int]
     | Tuple[float, float, float]
     | onp.ndarray = (80, 120, 255),
 ) -> int:
+    if isinstance(rgb, onp.ndarray):
+        assert rgb.shape == (3,)
     rgb_fixed = tuple(
-        value if isinstance(value, int) else int(value * 255) for value in rgb
+        value if onp.issubdtype(type(value), onp.integer) else int(value * 255)
+        for value in rgb
     )
     assert len(rgb_fixed) == 3
     return int(rgb_fixed[0] * (256**2) + rgb_fixed[1] * 256 + rgb_fixed[2])
 
 
 def _encode_image_base64(
     image: onp.ndarray,
```

### Comparing `viser-0.0.2/viser/_messages.py` & `viser-0.0.3/viser/_messages.py`

 * *Files identical despite different names*

### Comparing `viser-0.0.2/viser/_scene_handle.py` & `viser-0.0.3/viser/_scene_handle.py`

 * *Files identical despite different names*

### Comparing `viser-0.0.2/viser/_viser.py` & `viser-0.0.3/viser/_viser.py`

 * *Files identical despite different names*

### Comparing `viser-0.0.2/viser/client/.eslintrc.js` & `viser-0.0.3/viser/client/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `viser-0.0.2/viser/client/README.md` & `viser-0.0.3/viser/client/README.md`

 * *Files identical despite different names*

### Comparing `viser-0.0.2/viser/client/build/favicon.svg` & `viser-0.0.3/viser/client/build/favicon.svg`

 * *Files identical despite different names*

### Comparing `viser-0.0.2/viser/client/build/index.html` & `viser-0.0.3/viser/client/build/index.html`

 * *Files identical despite different names*

### Comparing `viser-0.0.2/viser/client/build/static/css/main.992126cd.css.map` & `viser-0.0.3/viser/client/build/static/css/main.992126cd.css.map`

 * *Files identical despite different names*

### Comparing `viser-0.0.2/viser/client/build/static/js/main.721d9a9f.js` & `viser-0.0.3/viser/client/build/static/js/main.721d9a9f.js`

 * *Files identical despite different names*

### Comparing `viser-0.0.2/viser/client/build/static/js/main.721d9a9f.js.LICENSE.txt` & `viser-0.0.3/viser/client/build/static/js/main.721d9a9f.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `viser-0.0.2/viser/client/build/static/js/main.721d9a9f.js.map` & `viser-0.0.3/viser/client/build/static/js/main.721d9a9f.js.map`

 * *Files identical despite different names*

### Comparing `viser-0.0.2/viser/client/package.json` & `viser-0.0.3/viser/client/package.json`

 * *Files identical despite different names*

### Comparing `viser-0.0.2/viser/client/public/favicon.svg` & `viser-0.0.3/viser/client/public/favicon.svg`

 * *Files identical despite different names*

### Comparing `viser-0.0.2/viser/client/public/index.html` & `viser-0.0.3/viser/client/public/index.html`

 * *Files identical despite different names*

### Comparing `viser-0.0.2/viser/client/src/CameraControls.tsx` & `viser-0.0.3/viser/client/src/CameraControls.tsx`

 * *Files identical despite different names*

### Comparing `viser-0.0.2/viser/client/src/ControlPanel/ControlPanel.tsx` & `viser-0.0.3/viser/client/src/ControlPanel/ControlPanel.tsx`

 * *Files identical despite different names*

### Comparing `viser-0.0.2/viser/client/src/ControlPanel/Generated.tsx` & `viser-0.0.3/viser/client/src/ControlPanel/Generated.tsx`

 * *Files identical despite different names*

### Comparing `viser-0.0.2/viser/client/src/ControlPanel/GuiState.tsx` & `viser-0.0.3/viser/client/src/ControlPanel/GuiState.tsx`

 * *Files identical despite different names*

### Comparing `viser-0.0.2/viser/client/src/ControlPanel/SceneTreeUI.tsx` & `viser-0.0.3/viser/client/src/ControlPanel/SceneTreeUI.tsx`

 * *Files identical despite different names*

### Comparing `viser-0.0.2/viser/client/src/ControlPanel/Server.tsx` & `viser-0.0.3/viser/client/src/ControlPanel/Server.tsx`

 * *Files identical despite different names*

### Comparing `viser-0.0.2/viser/client/src/LabelRenderer.tsx` & `viser-0.0.3/viser/client/src/LabelRenderer.tsx`

 * *Files identical despite different names*

### Comparing `viser-0.0.2/viser/client/src/SceneTree.tsx` & `viser-0.0.3/viser/client/src/SceneTree.tsx`

 * *Files 3% similar despite different names*

```diff
@@ -123,15 +123,15 @@
             );
             remove_names.forEach((remove_name) => {
               delete state.nodeFromName[remove_name];
             });
           }),
         resetScene: () =>
           set((state) => {
-            Object.assign(state, cleanSceneTreeState);
+            state = { ...state, ...cleanSceneTreeState }; // eslint-disable-line @typescript-eslint/no-unused-vars
           }),
       }))
     )
   )[0];
 }
 
 /** Type corresponding to a zustand-style useSceneTree hook. */
@@ -174,23 +174,22 @@
   function SceneNodeThreeObject(props: {
     name: string;
     useSceneTree: UseSceneTree;
   }) {
     const sceneNode = props.useSceneTree(
       (state) => state.nodeFromName[props.name]
     );
-    const obj = props.useSceneTree((state) => state.objFromName[props.name]);
     const setObj = props.useSceneTree((state) => state.setObj);
     const clearObj = props.useSceneTree((state) => state.clearObj);
     const ref = React.useRef<THREE.Object3D>(null);
 
     React.useEffect(() => {
       ref.current && setObj(props.name, ref.current);
       return () => clearObj(props.name);
-    }, [obj]); // This `obj` dependency is needed for when resetScene() clears the world axis obj.
+    });
 
     return (
       <>
         {sceneNode.make_object(ref)}
         <SceneNodeUpdater
           name={props.name}
           objRef={ref}
```

### Comparing `viser-0.0.2/viser/client/src/SearchParamsUtils.tsx` & `viser-0.0.3/viser/client/src/SearchParamsUtils.tsx`

 * *Files identical despite different names*

### Comparing `viser-0.0.2/viser/client/src/ThreeAssets.tsx` & `viser-0.0.3/viser/client/src/ThreeAssets.tsx`

 * *Files identical despite different names*

### Comparing `viser-0.0.2/viser/client/src/WebsocketInterface.tsx` & `viser-0.0.3/viser/client/src/WebsocketInterface.tsx`

 * *Files 1% similar despite different names*

```diff
@@ -434,16 +434,14 @@
         // Try our best to handle messages in order. If this takes more than 1 second, we give up. :)
         await orderLock.acquireAsync({ timeout: 1000 }).catch(() => {
           console.log("Order lock timed out.");
           orderLock.release();
         });
         try {
           messageQueue.push(await messagePromise);
-          // handleMessage(await messagePromise);
-          // handleMessage(await messagePromise);
         } finally {
           orderLock.acquired && orderLock.release();
         }
       };
     }
 
     let timeout = setTimeout(tryConnect, 500);
```

### Comparing `viser-0.0.2/viser/client/src/WebsocketMessages.tsx` & `viser-0.0.3/viser/client/src/WebsocketMessages.tsx`

 * *Files identical despite different names*

### Comparing `viser-0.0.2/viser/client/src/index.tsx` & `viser-0.0.3/viser/client/src/index.tsx`

 * *Files identical despite different names*

### Comparing `viser-0.0.2/viser/client/yarn.lock` & `viser-0.0.3/viser/client/yarn.lock`

 * *Files identical despite different names*

### Comparing `viser-0.0.2/viser/extras/_record3d.py` & `viser-0.0.3/viser/extras/_record3d.py`

 * *Files identical despite different names*

### Comparing `viser-0.0.2/viser/infra/__init__.py` & `viser-0.0.3/viser/infra/__init__.py`

 * *Files identical despite different names*

### Comparing `viser-0.0.2/viser/infra/_async_message_buffer.py` & `viser-0.0.3/viser/infra/_async_message_buffer.py`

 * *Files identical despite different names*

### Comparing `viser-0.0.2/viser/infra/_infra.py` & `viser-0.0.3/viser/infra/_infra.py`

 * *Files identical despite different names*

### Comparing `viser-0.0.2/viser/infra/_messages.py` & `viser-0.0.3/viser/infra/_messages.py`

 * *Files identical despite different names*

### Comparing `viser-0.0.2/viser/infra/_typescript_interface_gen.py` & `viser-0.0.3/viser/infra/_typescript_interface_gen.py`

 * *Files identical despite different names*

### Comparing `viser-0.0.2/PKG-INFO` & `viser-0.0.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viser
-Version: 0.0.2
+Version: 0.0.3
 Summary: 3D visualization helper
 Author: brentyi
 Author-email: brentyi@berkeley.edu
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -75,11 +75,20 @@
 
 ```bash
 cd ./viser/viser/client
 yarn
 yarn start
 ```
 
-## Interactive SMPL-X Example
+## Demos
+
+### Interactive SMPL-X Example
 
 https://user-images.githubusercontent.com/6992947/228734499-87d8a12a-df1a-4511-a4e0-0a46bd8532fd.mov
 
+
+### Interactive NeRF rendering
+
+(code not released)
+
+https://user-images.githubusercontent.com/6992947/232163875-ff788455-f074-4bd3-9154-5330b5ed4733.mov
+
```

