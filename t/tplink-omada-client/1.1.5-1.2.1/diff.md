# Comparing `tmp/tplink_omada_client-1.1.5.tar.gz` & `tmp/tplink_omada_client-1.2.1.tar.gz`

## Comparing `tplink_omada_client-1.1.5.tar` & `tplink_omada_client-1.2.1.tar`

### file list

```diff
@@ -1,23 +1,34 @@
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 tplink_omada_client-1.1.5/.pylintrc
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 tplink_omada_client-1.1.5/Dockerfile.dev
--rw-r--r--   0        0        0     3817 2020-02-02 00:00:00.000000 tplink_omada_client-1.1.5/package_constraints.txt
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 tplink_omada_client-1.1.5/requirements.txt
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 tplink_omada_client-1.1.5/requirements_test.txt
--rwxr-xr-x   0        0        0     3375 2020-02-02 00:00:00.000000 tplink_omada_client-1.1.5/sample_client.py
--rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 tplink_omada_client-1.1.5/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 tplink_omada_client-1.1.5/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 tplink_omada_client-1.1.5/.vscode/launch.json
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 tplink_omada_client-1.1.5/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tplink_omada_client-1.1.5/src/tplink_omada_client/__init__.py
--rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 tplink_omada_client-1.1.5/src/tplink_omada_client/definitions.py
--rw-r--r--   0        0        0    14399 2020-02-02 00:00:00.000000 tplink_omada_client-1.1.5/src/tplink_omada_client/devices.py
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 tplink_omada_client-1.1.5/src/tplink_omada_client/exceptions.py
--rw-r--r--   0        0        0     6826 2020-02-02 00:00:00.000000 tplink_omada_client-1.1.5/src/tplink_omada_client/omadaapiconnection.py
--rw-r--r--   0        0        0     2908 2020-02-02 00:00:00.000000 tplink_omada_client-1.1.5/src/tplink_omada_client/omadaclient.py
--rw-r--r--   0        0        0    10480 2020-02-02 00:00:00.000000 tplink_omada_client-1.1.5/src/tplink_omada_client/omadasiteclient.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tplink_omada_client-1.1.5/src/tplink_omada_client/py.typed
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 tplink_omada_client-1.1.5/.gitignore
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 tplink_omada_client-1.1.5/LICENSE
--rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 tplink_omada_client-1.1.5/README.md
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 tplink_omada_client-1.1.5/pyproject.toml
--rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 tplink_omada_client-1.1.5/PKG-INFO
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.1/.pylintrc
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.1/Dockerfile.dev
+-rw-r--r--   0        0        0     3817 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.1/package_constraints.txt
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.1/requirements.txt
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.1/requirements_test.txt
+-rwxr-xr-x   0        0        0     3375 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.1/sample_client.py
+-rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.1/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.1/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.1/.vscode/launch.json
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.1/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.1/src/tplink_omada_client/__init__.py
+-rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.1/src/tplink_omada_client/definitions.py
+-rw-r--r--   0        0        0    14464 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.1/src/tplink_omada_client/devices.py
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.1/src/tplink_omada_client/exceptions.py
+-rw-r--r--   0        0        0     6875 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.1/src/tplink_omada_client/omadaapiconnection.py
+-rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.1/src/tplink_omada_client/omadaclient.py
+-rw-r--r--   0        0        0    10480 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.1/src/tplink_omada_client/omadasiteclient.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.1/src/tplink_omada_client/py.typed
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.1/src/tplink_omada_client/cli/__init__.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.1/src/tplink_omada_client/cli/__main__.py
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.1/src/tplink_omada_client/cli/command_devices.py
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.1/src/tplink_omada_client/cli/command_switch.py
+-rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.1/src/tplink_omada_client/cli/command_switches.py
+-rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.1/src/tplink_omada_client/cli/command_target.py
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.1/src/tplink_omada_client/cli/command_targets.py
+-rw-r--r--   0        0        0     2376 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.1/src/tplink_omada_client/cli/config.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.1/src/tplink_omada_client/cli/util.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.1/tests/conftest.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.1/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.1/LICENSE
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.1/README.md
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 tplink_omada_client-1.2.1/PKG-INFO
```

### Comparing `tplink_omada_client-1.1.5/Dockerfile.dev` & `tplink_omada_client-1.2.1/Dockerfile.dev`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.1.5/package_constraints.txt` & `tplink_omada_client-1.2.1/package_constraints.txt`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.1.5/sample_client.py` & `tplink_omada_client-1.2.1/sample_client.py`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.1.5/.devcontainer/devcontainer.json` & `tplink_omada_client-1.2.1/.devcontainer/devcontainer.json`

 * *Files 24% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 {
 	"name": "Existing Dockerfile",
 
 	// Sets the run context to one level up instead of the .devcontainer folder.
 	"context": "..",
 
 	// Update the 'dockerFile' property if you aren't using the standard 'Dockerfile' filename.
-	"dockerFile": "../Dockerfile.dev"
+	"dockerFile": "../Dockerfile.dev",
 
 	// Use 'forwardPorts' to make a list of ports inside the container available locally.
 	// "forwardPorts": [],
 
-	// Uncomment the next line to run commands after the container is created - for example installing curl.
-	// "postCreateCommand": "apt-get update && apt-get install -y curl",
+	// Install package in "dev mode" to expose CLI
+	"postCreateCommand": "pip3 install -e ."
 
 	// Uncomment when using a ptrace-based debugger like C++, Go, and Rust
 	// "runArgs": [ "--cap-add=SYS_PTRACE", "--security-opt", "seccomp=unconfined" ],
 
 	// Uncomment to use the Docker CLI from inside the container. See https://aka.ms/vscode-remote/samples/docker-from-docker.
 	// "mounts": [ "source=/var/run/docker.sock,target=/var/run/docker.sock,type=bind" ],
```

### Comparing `tplink_omada_client-1.1.5/.github/workflows/python-publish.yml` & `tplink_omada_client-1.2.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.1.5/.vscode/launch.json` & `tplink_omada_client-1.2.1/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.1.5/src/tplink_omada_client/definitions.py` & `tplink_omada_client-1.2.1/src/tplink_omada_client/definitions.py`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.1.5/src/tplink_omada_client/devices.py` & `tplink_omada_client-1.2.1/src/tplink_omada_client/devices.py`

 * *Files 0% similar despite different names*

```diff
@@ -259,15 +259,17 @@
     @property
     def ports(self) -> List[OmadaSwitchPort]:
         """List of ports attached to the switch."""
         return [OmadaSwitchPort(p) for p in self._data["ports"]]
 
     @property
     def uplink(self) -> Optional[OmadaUplink]:
-        """Uplink device for this switch."""
+        """ Uplink device for this switch. """
+        if not "uplink" in self._data:
+            return None
         uplink = self._data["uplink"]
         if uplink is None:
             return None
         return OmadaUplink(uplink)
 
     @property
     def downlink(self) -> List[OmadaDownlink]:
```

### Comparing `tplink_omada_client-1.1.5/src/tplink_omada_client/exceptions.py` & `tplink_omada_client-1.2.1/src/tplink_omada_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.1.5/src/tplink_omada_client/omadaapiconnection.py` & `tplink_omada_client-1.2.1/src/tplink_omada_client/omadaapiconnection.py`

 * *Files 5% similar despite different names*

```diff
@@ -66,19 +66,20 @@
             await self.login()
             return self
         except Exception as error:
             if self._own_session:
                 await self.close()
             raise error
 
-    async def __aexit__(self, *args):
+    async def __aexit__(self, exc_type, exc_val, exc_tb) -> bool:
         """Call when the client is disposed."""
         # Close the web session, if we created it (i.e. it was not passed in)
         if self._own_session:
             await self.close()
+        return False
 
     async def close(self):
         """Close the current web session."""
         if self._session:
             await self._session.close()
             self._session = None
```

### Comparing `tplink_omada_client-1.1.5/src/tplink_omada_client/omadaclient.py` & `tplink_omada_client-1.2.1/src/tplink_omada_client/omadaclient.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,19 +39,19 @@
     ):
         self._api = OmadaApiConnection(url, username, password, websession, verify_ssl)
 
     async def __aenter__(self):
         await self._api.__aenter__()
         return self
 
-    async def __aexit__(self, *args):
+    async def __aexit__(self, *args) -> bool:
         """Call when the client is disposed."""
         # Close the web session, if we created it (i.e. it was not passed in)
-        await self._api.__aexit__(*args)
-        return self
+        return await self._api.__aexit__(*args)
+        
 
     async def login(self) -> str:
         """
         Log in to the controller and returns the controller's unique ID.
 
         Calls to login are optional, as the API will automatically authenticate as necessary.
         However, you may want to attempt a login to check connectivity.
```

### Comparing `tplink_omada_client-1.1.5/src/tplink_omada_client/omadasiteclient.py` & `tplink_omada_client-1.2.1/src/tplink_omada_client/omadasiteclient.py`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.1.5/LICENSE` & `tplink_omada_client-1.2.1/LICENSE`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright 2022 Mark Godwin
+Copyright 2022-2023 Mark Godwin, Mike Heath
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `tplink_omada_client-1.1.5/README.md` & `tplink_omada_client-1.2.1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -19,14 +19,43 @@
     * Basic device information
     * Get firmware information and initiating automatic updates
     * Port status and configuraton for Switches
     * Lan port configuration for Access Points
 
 Tested with OC200 on Omada Controller Version 5.5.7 - 5.7.6. Other versions may not be fully compatible.
 
+## CLI
+
+This package provides a simple CLI for interacting with one or more Omada Controllers. To start using the
+CLI, you must first target a Controller.
+
+```sh
+$ omada -t NAME target --url https://your.omada.controller.here --user admin --password password --site MySite
+```
+
+Where `NAME` is a name of your choosing to identify the targeted controller. `--site` defaults to the Omada
+default site name, 'Default'.  If you do not provide a password as an argument, you will be prompted for a
+password.
+
+Once you have successfully targeted a controller you can test that things are working by running:
+
+```sh
+$ omada -t NAME devices
+```
+
+This will list all the devices being managed by your controller.
+
+To see a list of all the available commands, run:
+
+```sh
+$ omada -h
+```
+
+The CLI is still young so if there is any functionality you need, please create an issue and let us know.
+
 ## Future
 
 The available API surface is quite large. More of this could be exposed in the future.
 There is an undocumented Websocket API which could potentially be used to get a stream of updates. However,
 I'm not sure how fully featured this subscription channel is on the controller. It seems to be rarely used,
 so probably doesn't include client connect/disconnect notifications.
```

### Comparing `tplink_omada_client-1.1.5/pyproject.toml` & `tplink_omada_client-1.2.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "tplink_omada_client"
-version = "1.1.5"
+version = "1.2.1"
 authors = [
   { name="Mark Godwin", email="author@example.com" },
 ]
 description = "Python wrapper for TP-Link Omada SDN Controller API (OC200/OC300/Software Controller)"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
@@ -16,10 +16,13 @@
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
 ]
 dependencies = [
   "aiohttp >= 3.8.1, <4"
 ]
 
+[project.scripts]
+omada = "tplink_omada_client.cli:main"
+
 [project.urls]
 "Homepage" = "https://github.com/MarkGodwin/tplink-omada-api"
 "Bug Tracker" = "https://github.com/MarkGodwin/tplink-omada-api/issues"
```

