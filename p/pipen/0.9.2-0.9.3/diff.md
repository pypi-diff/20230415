# Comparing `tmp/pipen-0.9.2.tar.gz` & `tmp/pipen-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipen-0.9.2.tar", max compression
+gzip compressed data, was "pipen-0.9.3.tar", max compression
```

## Comparing `pipen-0.9.2.tar` & `pipen-0.9.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    11357 2023-04-14 06:12:33.272959 pipen-0.9.2/LICENSE
--rw-r--r--   0        0        0     9390 2023-04-14 06:12:33.272959 pipen-0.9.2/README.md
--rw-r--r--   0        0        0      318 2023-04-14 06:12:33.276959 pipen-0.9.2/pipen/__init__.py
--rw-r--r--   0        0        0       68 2023-04-14 06:12:33.276959 pipen-0.9.2/pipen/__main__.py
--rw-r--r--   0        0        0     7143 2023-04-14 06:12:33.276959 pipen-0.9.2/pipen/_job_caching.py
--rw-r--r--   0        0        0     6434 2023-04-14 06:12:33.276959 pipen-0.9.2/pipen/channel.py
--rw-r--r--   0        0        0       83 2023-04-14 06:12:33.276959 pipen-0.9.2/pipen/cli/__init__.py
--rw-r--r--   0        0        0      912 2023-04-14 06:12:33.276959 pipen-0.9.2/pipen/cli/_hooks.py
--rw-r--r--   0        0        0     1651 2023-04-14 06:12:33.276959 pipen-0.9.2/pipen/cli/_main.py
--rw-r--r--   0        0        0      973 2023-04-14 06:12:33.276959 pipen-0.9.2/pipen/cli/help.py
--rw-r--r--   0        0        0     3701 2023-04-14 06:12:33.276959 pipen-0.9.2/pipen/cli/plugins.py
--rw-r--r--   0        0        0     2906 2023-04-14 06:12:33.276959 pipen-0.9.2/pipen/cli/profile.py
--rw-r--r--   0        0        0     1181 2023-04-14 06:12:33.276959 pipen-0.9.2/pipen/cli/version.py
--rw-r--r--   0        0        0     2709 2023-04-14 06:12:33.276959 pipen-0.9.2/pipen/defaults.py
--rw-r--r--   0        0        0     1832 2023-04-14 06:12:33.276959 pipen-0.9.2/pipen/exceptions.py
--rw-r--r--   0        0        0     9499 2023-04-14 06:12:33.276959 pipen-0.9.2/pipen/job.py
--rw-r--r--   0        0        0    15070 2023-04-14 06:12:33.276959 pipen-0.9.2/pipen/pipen.py
--rw-r--r--   0        0        0     9965 2023-04-14 06:12:33.276959 pipen-0.9.2/pipen/pluginmgr.py
--rw-r--r--   0        0        0    23466 2023-04-14 06:12:33.276959 pipen-0.9.2/pipen/proc.py
--rw-r--r--   0        0        0     5489 2023-04-14 06:12:33.276959 pipen-0.9.2/pipen/procgroup.py
--rw-r--r--   0        0        0     4066 2023-04-14 06:12:33.276959 pipen-0.9.2/pipen/progressbar.py
--rw-r--r--   0        0        0     2404 2023-04-14 06:12:33.276959 pipen-0.9.2/pipen/scheduler.py
--rw-r--r--   0        0        0     3668 2023-04-14 06:12:33.276959 pipen-0.9.2/pipen/template.py
--rw-r--r--   0        0        0    14380 2023-04-14 06:12:33.276959 pipen-0.9.2/pipen/utils.py
--rw-r--r--   0        0        0       54 2023-04-14 06:12:33.276959 pipen-0.9.2/pipen/version.py
--rw-r--r--   0        0        0     1644 2023-04-14 06:12:33.276959 pipen-0.9.2/pyproject.toml
--rw-r--r--   0        0        0    10494 1970-01-01 00:00:00.000000 pipen-0.9.2/setup.py
--rw-r--r--   0        0        0    10314 1970-01-01 00:00:00.000000 pipen-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-15 03:49:12.291656 pipen-0.9.3/LICENSE
+-rw-r--r--   0        0        0     9390 2023-04-15 03:49:12.291656 pipen-0.9.3/README.md
+-rw-r--r--   0        0        0      318 2023-04-15 03:49:12.295656 pipen-0.9.3/pipen/__init__.py
+-rw-r--r--   0        0        0       68 2023-04-15 03:49:12.295656 pipen-0.9.3/pipen/__main__.py
+-rw-r--r--   0        0        0     7143 2023-04-15 03:49:12.295656 pipen-0.9.3/pipen/_job_caching.py
+-rw-r--r--   0        0        0     6434 2023-04-15 03:49:12.295656 pipen-0.9.3/pipen/channel.py
+-rw-r--r--   0        0        0       83 2023-04-15 03:49:12.295656 pipen-0.9.3/pipen/cli/__init__.py
+-rw-r--r--   0        0        0      912 2023-04-15 03:49:12.295656 pipen-0.9.3/pipen/cli/_hooks.py
+-rw-r--r--   0        0        0     1651 2023-04-15 03:49:12.295656 pipen-0.9.3/pipen/cli/_main.py
+-rw-r--r--   0        0        0      973 2023-04-15 03:49:12.295656 pipen-0.9.3/pipen/cli/help.py
+-rw-r--r--   0        0        0     3701 2023-04-15 03:49:12.295656 pipen-0.9.3/pipen/cli/plugins.py
+-rw-r--r--   0        0        0     2906 2023-04-15 03:49:12.295656 pipen-0.9.3/pipen/cli/profile.py
+-rw-r--r--   0        0        0     1181 2023-04-15 03:49:12.295656 pipen-0.9.3/pipen/cli/version.py
+-rw-r--r--   0        0        0     2709 2023-04-15 03:49:12.295656 pipen-0.9.3/pipen/defaults.py
+-rw-r--r--   0        0        0     1832 2023-04-15 03:49:12.295656 pipen-0.9.3/pipen/exceptions.py
+-rw-r--r--   0        0        0     9499 2023-04-15 03:49:12.295656 pipen-0.9.3/pipen/job.py
+-rw-r--r--   0        0        0    15070 2023-04-15 03:49:12.295656 pipen-0.9.3/pipen/pipen.py
+-rw-r--r--   0        0        0     9965 2023-04-15 03:49:12.295656 pipen-0.9.3/pipen/pluginmgr.py
+-rw-r--r--   0        0        0    23466 2023-04-15 03:49:12.295656 pipen-0.9.3/pipen/proc.py
+-rw-r--r--   0        0        0     5416 2023-04-15 03:49:12.295656 pipen-0.9.3/pipen/procgroup.py
+-rw-r--r--   0        0        0     4066 2023-04-15 03:49:12.295656 pipen-0.9.3/pipen/progressbar.py
+-rw-r--r--   0        0        0     2404 2023-04-15 03:49:12.295656 pipen-0.9.3/pipen/scheduler.py
+-rw-r--r--   0        0        0     3668 2023-04-15 03:49:12.295656 pipen-0.9.3/pipen/template.py
+-rw-r--r--   0        0        0    14438 2023-04-15 03:49:12.295656 pipen-0.9.3/pipen/utils.py
+-rw-r--r--   0        0        0       54 2023-04-15 03:49:12.295656 pipen-0.9.3/pipen/version.py
+-rw-r--r--   0        0        0     1644 2023-04-15 03:49:12.299656 pipen-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0    10494 1970-01-01 00:00:00.000000 pipen-0.9.3/setup.py
+-rw-r--r--   0        0        0    10314 1970-01-01 00:00:00.000000 pipen-0.9.3/PKG-INFO
```

### Comparing `pipen-0.9.2/LICENSE` & `pipen-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pipen-0.9.2/README.md` & `pipen-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `pipen-0.9.2/pipen/_job_caching.py` & `pipen-0.9.3/pipen/_job_caching.py`

 * *Files identical despite different names*

### Comparing `pipen-0.9.2/pipen/channel.py` & `pipen-0.9.3/pipen/channel.py`

 * *Files identical despite different names*

### Comparing `pipen-0.9.2/pipen/cli/_hooks.py` & `pipen-0.9.3/pipen/cli/_hooks.py`

 * *Files identical despite different names*

### Comparing `pipen-0.9.2/pipen/cli/_main.py` & `pipen-0.9.3/pipen/cli/_main.py`

 * *Files identical despite different names*

### Comparing `pipen-0.9.2/pipen/cli/help.py` & `pipen-0.9.3/pipen/cli/help.py`

 * *Files identical despite different names*

### Comparing `pipen-0.9.2/pipen/cli/plugins.py` & `pipen-0.9.3/pipen/cli/plugins.py`

 * *Files identical despite different names*

### Comparing `pipen-0.9.2/pipen/cli/profile.py` & `pipen-0.9.3/pipen/cli/profile.py`

 * *Files identical despite different names*

### Comparing `pipen-0.9.2/pipen/cli/version.py` & `pipen-0.9.3/pipen/cli/version.py`

 * *Files identical despite different names*

### Comparing `pipen-0.9.2/pipen/defaults.py` & `pipen-0.9.3/pipen/defaults.py`

 * *Files identical despite different names*

### Comparing `pipen-0.9.2/pipen/exceptions.py` & `pipen-0.9.3/pipen/exceptions.py`

 * *Files identical despite different names*

### Comparing `pipen-0.9.2/pipen/job.py` & `pipen-0.9.3/pipen/job.py`

 * *Files identical despite different names*

### Comparing `pipen-0.9.2/pipen/pipen.py` & `pipen-0.9.3/pipen/pipen.py`

 * *Files identical despite different names*

### Comparing `pipen-0.9.2/pipen/pluginmgr.py` & `pipen-0.9.3/pipen/pluginmgr.py`

 * *Files identical despite different names*

### Comparing `pipen-0.9.2/pipen/proc.py` & `pipen-0.9.3/pipen/proc.py`

 * *Files identical despite different names*

### Comparing `pipen-0.9.2/pipen/procgroup.py` & `pipen-0.9.3/pipen/procgroup.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,14 +95,16 @@
 
     def _load_runtime_procs(self):
         """Load all processes that are added at runtime"""
         # Load all processes if they are decorated by ProcGroup.add_proc
         for name, attr in self.__class__.__dict__.items():
             if isinstance(attr, cached_property):
                 getattr(self, name)
+            elif isinstance(attr, type) and issubclass(attr, Proc):
+                self.add_proc(attr)
 
     def add_proc(
         self_or_method: ProcGroup | Callable[[ProcGroup], Type[Proc]],
         proc: Type[Proc] | None = None,
     ) -> Type[Proc] | cached_property:
         """Add a process to the proc group
 
@@ -138,22 +140,16 @@
         @wraps(self_or_method)
         def wrapper(self):
             proc = self_or_method(self)
 
             if proc is None:
                 return None
 
-            if (
-                not isinstance(proc, Proc)
-                and (not isinstance(proc, type) or not issubclass(proc, Proc))
-            ):
-                raise ValueError(
-                    f"`{proc}` is not a process "
-                    "(either a subclass or an instance of Proc)"
-                )
+            if (not isinstance(proc, type) or not issubclass(proc, Proc)):
+                raise ValueError(f"`{proc}` is not a Proc subclass")
 
             proc.__meta__["procgroup"] = self
             if not proc.requires:
                 self.starts.append(proc)
             self.procs[proc.name] = proc
             return proc
```

### Comparing `pipen-0.9.2/pipen/progressbar.py` & `pipen-0.9.3/pipen/progressbar.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 if TYPE_CHECKING:  # pragma: no cover
     import enlighten
 
 # [12/02/20 12:44:06] I core
 #                 pipeline: 100%|
 # |        desc_len      |
-PBAR_DESC_LEN = 23
+PBAR_DESC_LEN = 24
 
 
 class ProcPBar:
     """The progress bar for processes"""
 
     def __init__(
         self, manager: enlighten.Manager, proc_size: int, proc_name: str
```

### Comparing `pipen-0.9.2/pipen/scheduler.py` & `pipen-0.9.3/pipen/scheduler.py`

 * *Files identical despite different names*

### Comparing `pipen-0.9.2/pipen/template.py` & `pipen-0.9.3/pipen/template.py`

 * *Files identical despite different names*

### Comparing `pipen-0.9.2/pipen/utils.py` & `pipen-0.9.3/pipen/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,16 +87,16 @@
                 self._width = CONSOLE_DEFAULT_WIDTH
 
     def _render_buffer(self, buffer: Iterable[Segment]) -> str:
         out = super()._render_buffer(buffer)
         return out.rstrip() + "\n"
 
 
+logging.lastResort = logging.NullHandler()  # type: ignore
 logger_console = RichConsole()
-
 _logger_handler = RichHandler(
     show_path=False,
     show_level=True,
     console=logger_console,
     rich_tracebacks=True,
     omit_repeated_times=False,  # rich 10+
     markup=True,
```

### Comparing `pipen-0.9.2/pyproject.toml` & `pipen-0.9.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry>=0.12",]
 build-backend = "poetry.masonry.api"
 
 [tool.poetry]
 name = "pipen"
-version = "0.9.2"
+version = "0.9.3"
 description = "A pipeline framework for python"
 authors = [ "pwwang <pwwang@pwwang.com>",]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/pwwang/pipen"
 repository = "https://github.com/pwwang/pipen"
```

### Comparing `pipen-0.9.2/setup.py` & `pipen-0.9.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
  'xqute>=0.2.1,<0.3.0']
 
 entry_points = \
 {'console_scripts': ['pipen = pipen.cli:main']}
 
 setup_kwargs = {
     'name': 'pipen',
-    'version': '0.9.2',
+    'version': '0.9.3',
     'description': 'A pipeline framework for python',
     'long_description': '<div align="center">\n    <img src="./pipen.png" width="320px">\n\n**A pipeline framework for python**\n\n</div>\n\n______________________________________________________________________\n\n[![Pypi][6]][7] [![Github][8]][9] ![Building][10] [![Docs and API][11]][1] [![Codacy][12]][13] [![Codacy coverage][14]][13] [![Deps][5]][23]\n\n[Documentation][1] | [ChangeLog][2] | [Examples][3] | [API][4]\n\n## Features\n\n- Easy to use\n- Nearly zero-configuration\n- Nice logging\n- Highly extendable\n\n## Installation\n\n```bash\npip install -U pipen\n```\n\n## Quickstart\n\n`example.py`\n\n```python\nfrom pipen import Proc, Pipen\n\nclass P1(Proc):\n    """Sort input file"""\n    input = "infile"\n    input_data = ["/tmp/data.txt"]\n    output = "outfile:file:intermediate.txt"\n    script = "cat {{in.infile}} | sort > {{out.outfile}}"\n\nclass P2(Proc):\n    """Paste line number"""\n    requires = P1\n    input = "infile"\n    output = "outfile:file:result.txt"\n    script = "paste <(seq 1 3) {{in.infile}} > {{out.outfile}}"\n\nclass MyPipeline(Pipen):\n    starts = P1\n\nif __name__ == "__main__":\n    MyPipeline().run()\n```\n\n```shell\n> echo -e "3\\n2\\n1" > /tmp/data.txt\n> python example.py\n```\n\n```log\n[09/13/21 04:23:37] I main                    _____________________________________   __\n[09/13/21 04:23:37] I main                    ___  __ \\___  _/__  __ \\__  ____/__  | / /\n[09/13/21 04:23:37] I main                    __  /_/ /__  / __  /_/ /_  __/  __   |/ /\n[09/13/21 04:23:37] I main                    _  ____/__/ /  _  ____/_  /___  _  /|  /\n[09/13/21 04:23:37] I main                    /_/     /___/  /_/     /_____/  /_/ |_/\n[09/13/21 04:23:37] I main\n[09/13/21 04:23:37] I main                                 version: 0.9.0\n[09/13/21 04:23:37] I main\n[09/13/21 04:23:37] I main    ╭═════════════════════════════ MYPIPELIN ═══════════════════════════════╮\n[09/13/21 04:23:37] I main    ║  # procs          = 2                                                 ║\n[09/13/21 04:23:37] I main    ║  plugins          = [\'main\', \'verbose-0.0.1\']                         ║\n[09/13/21 04:23:37] I main    ║  profile          = default                                           ║\n[09/13/21 04:23:37] I main    ║  outdir           = mypipeline_results                                ║\n[09/13/21 04:23:37] I main    ║  cache            = True                                              ║\n[09/13/21 04:23:37] I main    ║  dirsig           = 1                                                 ║\n[09/13/21 04:23:37] I main    ║  error_strategy   = ignore                                            ║\n[09/13/21 04:23:37] I main    ║  forks            = 1                                                 ║\n[09/13/21 04:23:37] I main    ║  lang             = bash                                              ║\n[09/13/21 04:23:37] I main    ║  loglevel         = info                                              ║\n[09/13/21 04:23:37] I main    ║  num_retries      = 3                                                 ║\n[09/13/21 04:23:37] I main    ║  plugin_opts      = {}                                                ║\n[09/13/21 04:23:37] I main    ║  plugins          = None                                              ║\n[09/13/21 04:23:37] I main    ║  scheduler        = local                                             ║\n[09/13/21 04:23:37] I main    ║  scheduler_opts   = {}                                                ║\n[09/13/21 04:23:37] I main    ║  submission_batch = 8                                                 ║\n[09/13/21 04:23:37] I main    ║  template         = liquid                                            ║\n[09/13/21 04:23:37] I main    ║  template_opts    = {}                                                ║\n[09/13/21 04:23:37] I main    ║  workdir          = ./.pipen                                          ║\n[09/13/21 04:23:37] I main    ╰═══════════════════════════════════════════════════════════════════════╯\n[09/13/21 04:23:37] I main\n[09/13/21 04:23:37] I main    ╭───────────────────────────────── P1 ──────────────────────────────────╮\n[09/13/21 04:23:37] I main    │ Sort input file                                                       │\n[09/13/21 04:23:37] I main    ╰───────────────────────────────────────────────────────────────────────╯\n[09/13/21 04:23:37] I main    P1: Workdir: \'.pipen/mypipeline/p1\'\n[09/13/21 04:23:37] I main    P1: <<< [START]\n[09/13/21 04:23:37] I main    P1: >>> [\'P2\']\n[09/13/21 04:23:37] I verbose P1: size: 1\n[09/13/21 04:23:37] I verbose P1: [0/0] in.infile: /tmp/data.txt\n[09/13/21 04:23:37] I verbose P1: [0/0] out.outfile:\n                      /home/pwwang/github/pipen/.pipen/mypipeline/p1/0/output/intermediate.txt\n[09/13/21 04:23:38] I verbose P1: Time elapsed: 00:00:01.039s\n[09/13/21 04:23:38] I main\n[09/13/21 04:23:38] I main    ╭═════════════════════════════════ P2 ══════════════════════════════════╮\n[09/13/21 04:23:38] I main    ║ Paste line number                                                     ║\n[09/13/21 04:23:38] I main    ╰═══════════════════════════════════════════════════════════════════════╯\n[09/13/21 04:23:38] I main    P2: Workdir: \'.pipen/mypipeline/p2\'\n[09/13/21 04:23:38] I main    P2: <<< [\'P1\']\n[09/13/21 04:23:38] I main    P2: >>> [END]\n[09/13/21 04:23:38] I verbose P2: size: 1\n[09/13/21 04:23:38] I verbose P2: [0/0] in.infile:\n                      /home/pwwang/github/pipen/.pipen/mypipeline/p1/0/output/intermediate.txt\n[09/13/21 04:23:38] I verbose P2: [0/0] out.outfile:\n                      /home/pwwang/github/pipen/mypipeline_results/P2/result.txt\n[09/13/21 04:23:40] I verbose P2: Time elapsed: 00:00:02.074s\n[09/13/21 04:23:40] I main\n\n                PIPEN-0: 100%|████████████████████████████████████████| 2/2 [00:04<00:00, 0.56 procs/s]\n```\n\n```shell\n> cat ./mypipeline_results/P2/result.txt\n1       1\n2       2\n3       3\n```\n\n## Examples\n\nSee more examples at `examples/` and a more realcase example at:\nhttps://github.com/pwwang/pipen-report/tree/master/example\n\n## Plugin gallery\n\nPlugins make `pipen` even better.\n\n- [`pipen-verbose`][15]: Add verbosal information in logs for pipen.\n- [`pipen-lock`][25]: Process lock for pipen to prevent multiple runs at the same time.\n- [`pipen-report`][16]: Generate report for pipen\n- [`pipen-filters`][17]: Add a set of useful filters for pipen templates.\n- [`pipen-diagram`][18]: Draw pipeline diagrams for pipen\n- [`pipen-annotate`][26]: Use docstring to annotate pipen processes\n- [`pipen-args`][19]: Command line argument parser for pipen\n- [`pipen-dry`][20]: Dry runner for pipen pipelines\n- [`pipen-cli-init`][21]: A pipen CLI plugin to create a pipen project (pipeline)\n- [`pipen-cli-run`][22]: A pipen cli plugin to run a process or a pipeline\n- [`pipen-cli-config`][27]: UI wizard to generate configuration for pipen pipelines\n- [`pipen-cli-require`][24]: A pipen cli plugin check the requirements of a pipeline\n\n\n[1]: https://pwwang.github.io/pipen\n[2]: https://pwwang.github.io/pipen/CHANGELOG\n[3]: https://pwwang.github.io/pipen/examples\n[4]: https://pwwang.github.io/pipen/api/pipen\n[5]: https://img.shields.io/librariesio/release/pypi/pipen?style=flat-square\n[6]: https://img.shields.io/pypi/v/pipen?style=flat-square\n[7]: https://pypi.org/project/pipen/\n[8]: https://img.shields.io/github/v/tag/pwwang/pipen?style=flat-square\n[9]: https://github.com/pwwang/pipen\n[10]: https://img.shields.io/github/actions/workflow/status/pwwang/pipen/build.yml?style=flat-square\n[11]: https://img.shields.io/github/actions/workflow/status/pwwang/pipen/docs.yml?label=docs&style=flat-square\n[12]: https://img.shields.io/codacy/grade/cf1c6c97e5c4480386a05b42dec10c6e?style=flat-square\n[13]: https://app.codacy.com/gh/pwwang/pipen\n[14]: https://img.shields.io/codacy/coverage/cf1c6c97e5c4480386a05b42dec10c6e?style=flat-square\n[15]: https://github.com/pwwang/pipen-verbose\n[16]: https://github.com/pwwang/pipen-report\n[17]: https://github.com/pwwang/pipen-filters\n[18]: https://github.com/pwwang/pipen-diagram\n[19]: https://github.com/pwwang/pipen-args\n[20]: https://github.com/pwwang/pipen-dry\n[21]: https://github.com/pwwang/pipen-cli-init\n[22]: https://github.com/pwwang/pipen-cli-run\n[23]: https://libraries.io/github/pwwang/pipen#repository_dependencies\n[24]: https://github.com/pwwang/pipen-cli-require\n[25]: https://github.com/pwwang/pipen-lock\n[26]: https://github.com/pwwang/pipen-annotate\n[27]: https://github.com/pwwang/pipen-cli-config\n',
     'author': 'pwwang',
     'author_email': 'pwwang@pwwang.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/pwwang/pipen',
```

### Comparing `pipen-0.9.2/PKG-INFO` & `pipen-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipen
-Version: 0.9.2
+Version: 0.9.3
 Summary: A pipeline framework for python
 Home-page: https://github.com/pwwang/pipen
 License: MIT
 Author: pwwang
 Author-email: pwwang@pwwang.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

