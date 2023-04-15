# Comparing `tmp/cpggen-0.9.1.tar.gz` & `tmp/cpggen-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpggen-0.9.1.tar", max compression
+gzip compressed data, was "cpggen-0.9.2.tar", max compression
```

## Comparing `cpggen-0.9.1.tar` & `cpggen-0.9.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11357 2023-04-12 05:18:26.641698 cpggen-0.9.1/LICENSE
--rw-r--r--   0        0        0     6746 2023-04-12 05:18:26.641698 cpggen-0.9.1/README.md
--rw-r--r--   0        0        0        0 2023-04-12 05:18:26.645698 cpggen-0.9.1/cpggen/__init__.py
--rw-r--r--   0        0        0    12397 2023-04-12 05:18:26.645698 cpggen-0.9.1/cpggen/cli.py
--rw-r--r--   0        0        0    24879 2023-04-12 05:18:26.645698 cpggen-0.9.1/cpggen/executor.py
--rw-r--r--   0        0        0      746 2023-04-12 05:18:26.645698 cpggen-0.9.1/cpggen/logger.py
--rw-r--r--   0        0        0    10340 2023-04-12 05:18:26.645698 cpggen-0.9.1/cpggen/utils.py
--rw-r--r--   0        0        0     1245 2023-04-12 05:18:26.645698 cpggen-0.9.1/pyproject.toml
--rw-r--r--   0        0        0     8074 1970-01-01 00:00:00.000000 cpggen-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-15 00:43:28.683513 cpggen-0.9.2/LICENSE
+-rw-r--r--   0        0        0     6774 2023-04-15 00:43:28.683513 cpggen-0.9.2/README.md
+-rw-r--r--   0        0        0        0 2023-04-15 00:43:28.683513 cpggen-0.9.2/cpggen/__init__.py
+-rw-r--r--   0        0        0    12893 2023-04-15 00:43:28.683513 cpggen-0.9.2/cpggen/cli.py
+-rw-r--r--   0        0        0    28621 2023-04-15 00:43:28.683513 cpggen-0.9.2/cpggen/executor.py
+-rw-r--r--   0        0        0      746 2023-04-15 00:43:28.687514 cpggen-0.9.2/cpggen/logger.py
+-rw-r--r--   0        0        0    10937 2023-04-15 00:43:28.687514 cpggen-0.9.2/cpggen/utils.py
+-rw-r--r--   0        0        0     1245 2023-04-15 00:43:28.687514 cpggen-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0     8102 1970-01-01 00:00:00.000000 cpggen-0.9.2/PKG-INFO
```

### Comparing `cpggen-0.9.1/LICENSE` & `cpggen-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cpggen-0.9.1/README.md` & `cpggen-0.9.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -40,28 +40,28 @@
 # podman pull ghcr.io/appthreat/cpggen:nightly
 ```
 
 ### Single executable binaries
 
 Download the executable binary for your operating system from the [releases page](https://github.com/appthreat/cpggen/releases). These binary bundle the following:
 
+- Joern with all the CPG frontends
 - cpggen with Python 3.10
-- cdxgen with Node.js 18
-- cdxgen binary plugins
+- cdxgen with Node.js 18 - Generates SBoM
 
 ```bash
-curl -LO https://github.com/AppThreat/cpggen/releases/download/v0.9.1/cpggen-linux-amd64
+curl -LO https://github.com/AppThreat/cpggen/releases/download/v0.9.2/cpggen-linux-amd64
 chmod +x cpggen-linux-amd64
 ./cpggen-linux-amd64 --help
 ```
 
 On Windows,
 
 ```powershell
-curl -LO https://github.com/appthreat/cpggen/releases/download/v0.9.1/cpggen.exe
+curl -LO https://github.com/appthreat/cpggen/releases/download/v0.9.2/cpggen.exe
 .\cpggen.exe --help
 ```
 
 ### OCI Artifacts via ORAS cli
 
 Use [ORAS cli](https://oras.land/cli/) to download the cpggen binary with Python and Node.js preinstalled.
```

### Comparing `cpggen-0.9.1/cpggen/cli.py` & `cpggen-0.9.2/cpggen/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -305,23 +305,30 @@
 
 
 def main():
     print(product_logo)
     args = build_args()
     if args.server_mode:
         return run_server(args)
-    src = str(PurePath(args.src))
+    src = args.src
     cpg_out_dir = args.cpg_out_dir
-    if not cpg_out_dir and src:
-        cpg_out_dir = os.path.join(src, "cpg_out")
-    cpg_out_dir = str(PurePath(cpg_out_dir))
     export_out_dir = args.export_out_dir
-    if not export_out_dir and src:
-        export_out_dir = os.path.join(src, "export_out")
-    export_out_dir = str(PurePath(export_out_dir))
+    if not src.startswith("http") and not src.startswith("git://"):
+        src = str(PurePath(args.src))
+        if not cpg_out_dir and src:
+            if os.path.isfile(src):
+                cpg_out_dir = os.path.join(os.path.dirname(src), "cpg_out")
+            else:
+                cpg_out_dir = os.path.join(src, "cpg_out")
+        if not export_out_dir and src:
+            export_out_dir = os.path.join(src, "export_out")
+    if cpg_out_dir:
+        cpg_out_dir = str(PurePath(cpg_out_dir))
+    if export_out_dir:
+        export_out_dir = str(PurePath(export_out_dir))
     languages = args.language
     joern_home = args.joern_home
     use_container = args.use_container
     if joern_home and not os.path.exists(joern_home):
         if utils.check_command("docker") or utils.check_command("podman"):
             use_container = True
         else:
@@ -331,18 +338,22 @@
             console.print(
                 "Alternatively, ensure docker or podman is available to use cpggen container image"
             )
     # GitHub action is very weird
     if os.getenv("GITHUB_PATH") and utils.check_command("joern"):
         joern_home = ""
     is_temp_dir = False
-    if src.startswith("http") or src.startswith("git"):
+    if src.startswith("http") or src.startswith("git://"):
         clone_dir = tempfile.mkdtemp(prefix="cpggen")
         src = utils.clone_repo(src, clone_dir)
         is_temp_dir = True
+        if not cpg_out_dir:
+            cpg_out_dir = tempfile.mkdtemp(prefix="cpggen_cpg_out")
+        if not export_out_dir:
+            export_out_dir = tempfile.mkdtemp(prefix="cpggen_export_out")
     if not languages or languages == "autodetect":
         languages = utils.detect_project_type(src)
     else:
         languages = languages.split(",")
     if cpg_out_dir and not os.path.exists(cpg_out_dir):
         os.makedirs(cpg_out_dir, exist_ok=True)
```

### Comparing `cpggen-0.9.1/cpggen/executor.py` & `cpggen-0.9.2/cpggen/executor.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 import json
 import os
+import shutil
 import subprocess
+import sys
 import tempfile
+import zipfile
 from pathlib import Path
 
 import psutil
 from psutil._common import bytes2human
 from rich.progress import Progress
 
 from cpggen.logger import DEBUG, LOG, console
@@ -23,14 +26,68 @@
 
 runtimeValues = {}
 svmem = psutil.virtual_memory()
 max_memory = bytes2human(getattr(svmem, "available"), format="%(value).0f%(symbol)s")
 cpu_count = str(psutil.cpu_count())
 
 
+def resource_path(relative_path):
+    try:
+        base_path = sys._MEIPASS
+    except Exception:
+        base_path = os.path.dirname(__file__)
+    return os.path.join(base_path, relative_path)
+
+
+# Check if we are running as a bundled executable and
+# extract the binaries
+cdxgen_cmd = os.environ.get("CDXGEN_CMD", "cdxgen")
+local_bin_dir = resource_path("local_bin")
+if os.path.exists(local_bin_dir):
+    csharp2cpg_bundled = resource_path(
+        os.path.join("local_bin", "joern-cli", "csharp2cpg.zip")
+    )
+    joern_bundled = resource_path(os.path.join("local_bin", "joern-cli.zip"))
+    if os.path.exists(csharp2cpg_bundled):
+        with zipfile.ZipFile(csharp2cpg_bundled, "r") as zip_ref:
+            zip_ref.extractall(local_bin_dir)
+            os.symlink(
+                os.path.join(local_bin_dir, "bin", "csharp2cpg"),
+                os.path.join(local_bin_dir, "joern-cli", "csharp2cpg"),
+            )
+    if os.path.exists(joern_bundled):
+        with zipfile.ZipFile(joern_bundled, "r") as zip_ref:
+            zip_ref.extractall(local_bin_dir)
+            try:
+                # Add execute permissions
+                for dirname, subdirs, files in os.walk(local_bin_dir):
+                    for filename in files:
+                        if not filename.endswith(".jar") and (
+                            filename.endswith(".sh") or "2cpg" in filename
+                        ):
+                            os.chmod(os.path.join(dirname, filename), 0o755)
+                LOG.debug(f"Extracted {joern_bundled}")
+                os.environ["JOERN_HOME"] = os.path.join(local_bin_dir, "joern-cli")
+                os.environ["CPGGEN_BIN_DIR"] = local_bin_dir
+                os.environ["PATH"] += os.sep + os.environ["JOERN_HOME"] + os.sep
+            except Exception:
+                # Ignore errors
+                pass
+    if not shutil.which(cdxgen_cmd):
+        local_cdxgen_cmd = resource_path(
+            os.path.join(
+                "local_bin", "cdxgen.exe" if sys.platform == "win32" else "cdxgen"
+            )
+        )
+        if os.path.exists(local_cdxgen_cmd):
+            cdxgen_cmd = local_cdxgen_cmd
+            # Set the plugins directory as an environment variable
+            os.environ["CDXGEN_PLUGINS_DIR"] = local_bin_dir
+
+
 def get(configName, default_value=None):
     """Method to retrieve a config given a name. This method lazy loads configuration
     values and helps with overriding using a local config
     :param configName: Name of the config
     :return Config value
     """
     try:
@@ -53,22 +110,22 @@
     "ts": "%(joern_home)sjssrc2cpg.sh -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
     "kotlin": "%(joern_home)skotlin2cpg -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
     "kotlin-with-deps": "%(joern_home)skotlin2cpg -J-Xmx%(memory)s -o %(cpg_out)s %(src)s --download-dependencies",
     "kotlin-with-classpath": "%(joern_home)skotlin2cpg -J-Xmx%(memory)s -o %(cpg_out)s %(src)s --classpath %(home_dir)s/.m2 --classpath %(home_dir)s/.gradle/caches/modules-2/files-2.1",
     "php": "%(joern_home)sphp2cpg -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
     "python": "%(joern_home)spysrc2cpg -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
     "csharp": "%(joern_home)scsharp2cpg -i %(csharp_artifacts)s -o %(cpg_out)s --ignore-tests -l error",
-    "dotnet": "%(joern_home)scsharp2cpg -i %(csharp_artifacts)s -o %(cpg_out)s --ignore-tests -l error",
+    "dotnet": "%(joern_home)scsharp2cpg -i %(csharp_artifacts)s -o %(cpg_out)s --collect-js-files %(src)s --ignore-errors --no-log-file --ignore-tests -l error",
     "go": "%(joern_home)sgo2cpg generate -o %(cpg_out)s ./...",
-    "jar": "java -Xmx%(memory)s -Dorg.apache.el.parser.SKIP_IDENTIFIER_CHECK=true -jar /usr/local/bin/java2cpg.jar --experimental-langs=scala -su -o %(cpg_out)s %(uber_jar)s",
-    "jar-without-blocklist": "java -Xmx%(memory)s -Dorg.apache.el.parser.SKIP_IDENTIFIER_CHECK=true -jar /usr/local/bin/java2cpg.jar -nb --experimental-langs=scala -su -o %(cpg_out)s %(uber_jar)s",
-    "scala": "java -Xmx%(memory)s -Dorg.apache.el.parser.SKIP_IDENTIFIER_CHECK=true -jar /usr/local/bin/java2cpg.jar -nojsp --experimental-langs=scala -su -o %(cpg_out)s %(uber_jar)s",
-    "jsp": "java -Xmx%(memory)s -Dorg.apache.el.parser.SKIP_IDENTIFIER_CHECK=true -jar /usr/local/bin/java2cpg.jar --experimental-langs=scala -su -o %(cpg_out)s %(uber_jar)s",
-    "jsp-without-blocklist": "java -Xmx%(memory)s -Dorg.apache.el.parser.SKIP_IDENTIFIER_CHECK=true -jar /usr/local/bin/java2cpg.jar -nb --experimental-langs=scala -su -o %(cpg_out)s %(uber_jar)s",
-    "sbom": "cdxgen -r -t %(tool_lang)s -o %(sbom_out)s %(src)s",
+    "jar": "java -Xmx%(memory)s -Dorg.apache.el.parser.SKIP_IDENTIFIER_CHECK=true -jar %(cpggen_bin_dir)s/java2cpg.jar --experimental-langs=scala -su -o %(cpg_out)s %(uber_jar)s",
+    "jar-without-blocklist": "java -Xmx%(memory)s -Dorg.apache.el.parser.SKIP_IDENTIFIER_CHECK=true -jar %(cpggen_bin_dir)s/java2cpg.jar -nb --experimental-langs=scala -su -o %(cpg_out)s %(uber_jar)s",
+    "scala": "java -Xmx%(memory)s -Dorg.apache.el.parser.SKIP_IDENTIFIER_CHECK=true -jar %(cpggen_bin_dir)s/java2cpg.jar -nojsp --experimental-langs=scala -su -o %(cpg_out)s %(uber_jar)s",
+    "jsp": "java -Xmx%(memory)s -Dorg.apache.el.parser.SKIP_IDENTIFIER_CHECK=true -jar %(cpggen_bin_dir)s/java2cpg.jar --experimental-langs=scala -su -o %(cpg_out)s %(uber_jar)s",
+    "jsp-without-blocklist": "java -Xmx%(memory)s -Dorg.apache.el.parser.SKIP_IDENTIFIER_CHECK=true -jar %(cpggen_bin_dir)s/java2cpg.jar -nb --experimental-langs=scala -su -o %(cpg_out)s %(uber_jar)s",
+    "sbom": "%(cdxgen_cmd)s -r -t %(tool_lang)s -o %(sbom_out)s %(src)s",
     "export": "joern-export --repr=%(export_repr)s --format=%(export_format)s --out %(cpg_out)s %(src)s",
     "qwiet": "sl analyze %(policy)s%(vcs_correction)s--tag app.group=%(group)s --app %(app)s --%(language)s --cpgupload --bomupload %(sbom)s %(cpg)s",
 }
 
 build_tools_map = {
     "csharp": ["dotnet", "build"],
     "java": {
@@ -103,36 +160,37 @@
     "nodejs": {
         "npm": ["npm", "install", "--prefer-offline", "--no-audit", "--progress=false"],
         "yarn": ["yarn", "install"],
         "rush": ["rush", "install", "--bypass-policy", "--no-link"],
     },
     "go": {
         "go": ["go", "build", "./..."],
-        "make": ["make", "build"],
+        "make": ["make"],
+        "mage": ["mage", "build"],
     },
     "php": {
         "init": ["composer", "init", "--quiet"],
         "install": ["composer", "install", "-n", "--ignore-platform-reqs"],
         "update": ["composer", "update", "-n", "--ignore-platform-reqs"],
         "autoload": ["composer", "dump-autoload", "-o"],
     },
-    "make": ["make", "build"],
+    "make": ["make"],
 }
 
 
 def qwiet_analysis(app_manifest, cwd, env):
     try:
         LOG.info(f"Submitting {app_manifest['app']} for Qwiet.AI analysis")
         build_args = cpg_tools_map["qwiet"]
         policy = ""
         vcs_correction = ""
         if os.getenv("SHIFTLEFT_POLICY"):
             policy = f"""--policy {os.getenv("SHIFTLEFT_POLICY")} """
         elif os.getenv("ENABLE_BEST_PRACTICES") in ("true", "1"):
-            policy = f"""--policy io.shiftleft/defaultWithDictAndBestPractices """
+            policy = """--policy io.shiftleft/defaultWithDictAndBestPractices """
 
         if app_manifest.get("tool_lang"):
             if "jar" in app_manifest.get("tool_lang") or "jsp" in app_manifest.get(
                 "tool_lang"
             ):
                 vcs_correction = '--vcs-prefix-correction "*=src/main/java" '
             if "scala" in app_manifest.get("tool_lang"):
@@ -160,20 +218,27 @@
                 LOG.info(f"{app_manifest['app']} uploaded successfully")
     except Exception as e:
         LOG.error(e)
 
 
 def do_x_build(src, env, build_artefacts, tool_lang):
     tool_lang = tool_lang.split("-")[0]
+    build_crashes = {}
     for k, v in build_artefacts.items():
+        failed_modules = 0
+        crashed_modules = 0
         build_sets = build_tools_map.get(tool_lang)
         if isinstance(build_sets, dict):
             build_args = build_tools_map[tool_lang][k]
         else:
             build_args = build_sets
+        if len(v) > 5:
+            LOG.debug(
+                f"This project has {len(v)} modules. Build might take a while ..."
+            )
         for afile in v:
             base_dir = os.path.dirname(afile)
             build_args_str = " ".join(build_args)
             if "%(" in build_args_str:
                 gradle_cmd = "gradle"
                 maven_cmd = "mvn"
                 if os.path.exists(os.path.join(base_dir, "gradlew")):
@@ -202,18 +267,24 @@
                     cwd=base_dir,
                     env=env,
                     check=False,
                     shell=False,
                     encoding="utf-8",
                 )
                 if cp and LOG.isEnabledFor(DEBUG) and cp.returncode and cp.stderr:
-                    if cp.stderr:
-                        LOG.debug(cp.stderr)
+                    LOG.debug(cp.stderr)
+                    failed_modules = failed_modules + 1
             except Exception as e:
                 LOG.debug(e)
+                crashed_modules = crashed_modules + 1
+        build_crashes[k] = {
+            "failed_modules": failed_modules,
+            "crashed_modules": crashed_modules,
+        }
+    return build_crashes
 
 
 def do_jar_build(tool_lang, src, env):
     build_artefacts = {
         "gradle": find_gradle_files(src),
         "maven": find_pom_files(src),
         "sbt": find_sbt_files(src),
@@ -227,29 +298,37 @@
             LOG.info(
                 "Set the environment variable AT_DEBUG_MODE to debug and look for any build errors"
             )
     return do_x_build(src, env, build_artefacts, tool_lang)
 
 
 def do_go_build(src, env):
-    build_artefacts = {"go": find_go_mods(src), "make": find_makefiles(src)}
+    build_artefacts = {
+        "mage": find_files(src, "magefile.go", False, False),
+        "go": find_go_mods(src),
+        "make": find_makefiles(src),
+    }
     return do_x_build(src, env, build_artefacts, "go")
 
 
 def do_build(tool_lang, src, cwd, env):
     if tool_lang in ("csharp",):
-        do_x_build(src, env, {"csharp": find_csharp_artifacts(src)}, "csharp")
+        return do_x_build(src, env, {"csharp": find_csharp_artifacts(src)}, "csharp")
     elif (
         tool_lang in ("jar", "scala")
         or tool_lang.startswith("jar")
         or tool_lang.startswith("jsp")
     ):
-        do_jar_build(tool_lang, src, env)
+        return do_jar_build(tool_lang, src, env)
     elif tool_lang == "go":
-        do_go_build(src, env)
+        return do_go_build(src, env)
+
+
+def troubleshoot_app(lang_build_crashes, tool_lang):
+    pass
 
 
 def exec_tool(
     tool_lang,
     src,
     cpg_out_dir,
     cwd=None,
@@ -264,14 +343,17 @@
         console=console,
         transient=True,
         redirect_stderr=False,
         redirect_stdout=False,
         refresh_per_second=1,
     ) as progress:
         task = None
+        lang_build_crashes = {}
+        if cwd and os.path.isfile(cwd):
+            cwd = os.path.dirname(cwd)
         if joern_home and not joern_home.endswith(os.path.sep):
             joern_home = f"{joern_home}{os.path.sep}"
         try:
             stderr = subprocess.DEVNULL
             if LOG.isEnabledFor(DEBUG):
                 stdout = subprocess.PIPE
                 stderr = stdout
@@ -287,15 +369,15 @@
             if not cmd_with_args:
                 return
             # Perform build first
             if auto_build:
                 LOG.info(
                     f"Automatically building {src}. To speed up this step, cache the build dependencies using the CI cache settings."
                 )
-                do_build(tool_lang, src, cwd, env)
+                lang_build_crashes[tool_lang] = do_build(tool_lang, src, cwd, env)
             uber_jar = ""
             csharp_artifacts = ""
             # For languages like scala, jsp or jar we need to create a uber jar containing all jar, war files from the source directory
             if "uber_jar" in cmd_with_args:
                 stdout = subprocess.PIPE
                 java_artifacts = find_java_artifacts(src)
                 if len(java_artifacts):
@@ -355,30 +437,37 @@
                     joern_home=joern_home,
                     home_dir=str(Path.home()),
                     uber_jar=uber_jar,
                     csharp_artifacts=csharp_artifacts,
                     memory=os.getenv("CPGGEN_MEMORY", max_memory),
                     tool_lang=tool_lang,
                     sbom_out=sbom_out,
+                    cpggen_bin_dir=os.getenv("CPGGEN_BIN_DIR", "/usr/local/bin"),
                     **extra_args,
                 )
                 sbom_lang = tool_lang
                 if (
                     tool_lang in ("jar", "scala")
                     or tool_lang.startswith("jar")
                     or tool_lang.startswith("jsp")
                 ):
                     sbom_lang = "java"
                 sbom_cmd_with_args = sbom_cmd_with_args % dict(
-                    src=src, tool_lang=sbom_lang, sbom_out=sbom_out, **extra_args
+                    src=src,
+                    tool_lang=sbom_lang,
+                    cwd=cwd,
+                    sbom_out=sbom_out,
+                    cdxgen_cmd=cdxgen_cmd,
+                    cpggen_bin_dir=os.getenv("CPGGEN_BIN_DIR", "/usr/local/bin"),
+                    **extra_args,
                 )
                 cmd_list_with_args = cmd_with_args.split(" ")
                 sbom_cmd_list_with_args = sbom_cmd_with_args.split(" ")
                 lang_cmd = cmd_list_with_args[0]
-                if not check_command(lang_cmd):
+                if not check_command(lang_cmd) and not os.path.exists(lang_cmd):
                     if not use_container:
                         LOG.warn(
                             f"{lang_cmd} is not found. Try running cpggen with --use-container argument"
                         )
                     else:
                         LOG.warn(
                             f"{lang_cmd} is not found. Ensure the PATH variable in your container image is set to the bin directory of Joern."
@@ -434,44 +523,46 @@
                         os.path.basename(amodule),
                         " ".join(cmd_list_with_args),
                     )
                 )
                 cwd = amodule
                 if tool_lang in ("binary",):
                     cwd = os.getcwd()
-                # Generate sbom first since this would even download dependencies for java
-                try:
-                    progress.update(
-                        task,
-                        description="Generating SBoM using cdxgen",
-                        completed=10,
-                        total=100,
-                    )
-                    # Enable debug for sbom tool
-                    if LOG.isEnabledFor(DEBUG):
-                        env["SCAN_DEBUG_MODE"] = "debug"
-                    LOG.debug(f"Executing {' '.join(sbom_cmd_list_with_args)}")
-                    cp = subprocess.run(
-                        sbom_cmd_list_with_args,
-                        stdout=stdout,
-                        stderr=stderr,
-                        cwd=cwd,
-                        env=env,
-                        check=False,
-                        shell=False,
-                        encoding="utf-8",
-                    )
-                    if cp and LOG.isEnabledFor(DEBUG):
-                        if cp.stdout:
-                            LOG.debug(cp.stdout)
-                        if cp.stderr:
-                            LOG.debug(cp.stderr)
-                except Exception:
-                    # Ignore SBoM errors
-                    pass
+                if tool_lang != "binary":
+                    # Generate sbom first since this would even download dependencies for java
+                    try:
+                        progress.update(
+                            task,
+                            description="Generating SBoM using cdxgen",
+                            completed=10,
+                            total=100,
+                        )
+                        # Enable debug for sbom tool
+                        if LOG.isEnabledFor(DEBUG):
+                            env["SCAN_DEBUG_MODE"] = "debug"
+                        LOG.debug(f"Executing {' '.join(sbom_cmd_list_with_args)}")
+
+                        cp = subprocess.run(
+                            sbom_cmd_list_with_args,
+                            stdout=stdout,
+                            stderr=stderr,
+                            cwd=cwd,
+                            env=env,
+                            check=False,
+                            shell=False,
+                            encoding="utf-8",
+                        )
+                        if cp and LOG.isEnabledFor(DEBUG):
+                            if cp.stdout:
+                                LOG.debug(cp.stdout)
+                            if cp.stderr:
+                                LOG.debug(cp.stderr)
+                    except Exception:
+                        # Ignore SBoM errors
+                        pass
                 progress.update(
                     task, description="Generating CPG", completed=20, total=100
                 )
                 cp = subprocess.run(
                     cmd_list_with_args,
                     stdout=stdout,
                     stderr=stderr,
@@ -548,14 +639,15 @@
                         LOG.info(
                             "Set the environment variable AT_DEBUG_MODE to debug to see the debug logs"
                         )
                     if cp.stdout:
                         LOG.info(cp.stdout)
                     if cp.stderr:
                         LOG.info(cp.stderr)
+                    troubleshoot_app(lang_build_crashes, tool_lang)
                 progress.update(task, completed=100, total=100)
         except Exception as e:
             if not os.getenv("AT_DEBUG_MODE"):
                 LOG.info(
                     "Set the environment variable AT_DEBUG_MODE to debug to see the debug logs"
                 )
             LOG.error(e)
```

### Comparing `cpggen-0.9.1/cpggen/logger.py` & `cpggen-0.9.2/cpggen/logger.py`

 * *Files identical despite different names*

### Comparing `cpggen-0.9.1/cpggen/utils.py` & `cpggen-0.9.2/cpggen/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 import re
 import shutil
 import tempfile
 import zipfile
 from pathlib import Path
+from sys import platform
 
 import git
 
 # Default ignore list
 ignore_directories = [
     ".git",
     ".svn",
@@ -34,14 +35,16 @@
     "mock",
     "mocks",
     "vendor",
     "instancemode-tests",
     "integration-tests",
     "oauth2-tests",
     "twofactor-tests",
+    "gradle",
+    "buildSrc",
 ]
 
 ignore_files = [
     ".pyc",
     ".gz",
     ".tar",
     ".tar.gz",
@@ -121,20 +124,21 @@
     Method to find if the given directory is an ignored directory
     :param base_dir: Base directory
     :param dir_name: Directory to compare
     :return: Boolean True if directory can be ignored. False otherwise
     """
     base_dir = base_dir.lower()
     dir_name = dir_name.lower()
-    if dir_name.startswith("."):
-        return True
-    elif dir_name.startswith(os.path.sep + base_dir):
-        dir_name = re.sub(r"^" + os.path.sep + base_dir + os.path.sep, "", dir_name)
-    elif dir_name.startswith(base_dir):
-        dir_name = re.sub(r"^" + base_dir + os.path.sep, "", dir_name)
+    if platform != "win32":
+        if dir_name.startswith("."):
+            return True
+        elif dir_name.startswith(os.path.sep + base_dir):
+            dir_name = re.sub(r"^" + os.path.sep + base_dir + os.path.sep, "", dir_name)
+        elif dir_name.startswith(base_dir):
+            dir_name = re.sub(r"^" + base_dir + os.path.sep, "", dir_name)
     for d in ignore_directories:
         if (
             dir_name == d
             or dir_name.startswith(d)
             or (os.path.sep + d + os.path.sep) in dir_name
         ):
             return True
@@ -332,14 +336,18 @@
         or find_files(src_dir, ".gradle", False, True)
         or find_files(src_dir, ".java", False, True)
     ):
         if os.getenv("SHIFTLEFT_ACCESS_TOKEN"):
             project_types.append("jar")
         else:
             project_types.append("java")
+    if find_files(src_dir, ".bzl", False, True) or find_files(
+        src_dir, "BUILD", False, True
+    ):
+        project_types.append("java")
     if find_files(src_dir, ".jsp", False, True):
         project_types.append("jsp")
     if (
         find_files(src_dir, "package.json", False, True)
         or find_files(src_dir, "yarn.lock", False, True)
         or find_files(src_dir, ".js", False, True)
         or find_files(src_dir, ".ts", False, True)
@@ -356,17 +364,24 @@
     ):
         project_types.append("go")
     if (
         find_files(src_dir, "conan.lock", False, True)
         or find_files(src_dir, "conanfile.txt", False, True)
         or find_files(src_dir, ".c", False, True)
         or find_files(src_dir, ".cpp", False, True)
+        or find_files(src_dir, ".cc", False, True)
+        or find_files(src_dir, ".h", False, True)
+        or find_files(src_dir, ".hpp", False, True)
+        or find_files(src_dir, ".hh", False, True)
     ):
         project_types.append("c")
-
+    if find_files(src_dir, ".bc", False, True) or find_files(
+        src_dir, ".ll", False, True
+    ):
+        project_types.append("llvm")
     if is_exe(src_dir):
         project_types.append("binary")
     return project_types
 
 
 def clone_repo(repo_url, clone_dir, depth=1):
     git.Repo.clone_from(repo_url, clone_dir, depth=depth)
```

### Comparing `cpggen-0.9.1/pyproject.toml` & `cpggen-0.9.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cpggen"
-version = "0.9.1"
+version = "0.9.2"
 description = "Generate CPG for multiple languages for use with joern"
 authors = ["Team AppThreat <cloud@appthreat.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "cpggen"}]
 homepage = "https://github.com/AppThreat/cpggen"
 repository = "https://github.com/AppThreat/cpggen"
```

### Comparing `cpggen-0.9.1/PKG-INFO` & `cpggen-0.9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpggen
-Version: 0.9.1
+Version: 0.9.2
 Summary: Generate CPG for multiple languages for use with joern
 Home-page: https://github.com/AppThreat/cpggen
 License: Apache-2.0
 Keywords: joern,code analysis,static analysis,cpg,code property graph
 Author: Team AppThreat
 Author-email: cloud@appthreat.com
 Requires-Python: >=3.8,<3.12
@@ -72,28 +72,28 @@
 # podman pull ghcr.io/appthreat/cpggen:nightly
 ```
 
 ### Single executable binaries
 
 Download the executable binary for your operating system from the [releases page](https://github.com/appthreat/cpggen/releases). These binary bundle the following:
 
+- Joern with all the CPG frontends
 - cpggen with Python 3.10
-- cdxgen with Node.js 18
-- cdxgen binary plugins
+- cdxgen with Node.js 18 - Generates SBoM
 
 ```bash
-curl -LO https://github.com/AppThreat/cpggen/releases/download/v0.9.1/cpggen-linux-amd64
+curl -LO https://github.com/AppThreat/cpggen/releases/download/v0.9.2/cpggen-linux-amd64
 chmod +x cpggen-linux-amd64
 ./cpggen-linux-amd64 --help
 ```
 
 On Windows,
 
 ```powershell
-curl -LO https://github.com/appthreat/cpggen/releases/download/v0.9.1/cpggen.exe
+curl -LO https://github.com/appthreat/cpggen/releases/download/v0.9.2/cpggen.exe
 .\cpggen.exe --help
 ```
 
 ### OCI Artifacts via ORAS cli
 
 Use [ORAS cli](https://oras.land/cli/) to download the cpggen binary with Python and Node.js preinstalled.
```

