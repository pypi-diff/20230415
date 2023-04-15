# Comparing `tmp/sball-0.9.5.tar.gz` & `tmp/sball-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sball-0.9.5.tar", last modified: Sat Apr 15 02:30:16 2023, max compression
+gzip compressed data, was "sball-0.9.6.tar", last modified: Sat Apr 15 03:10:24 2023, max compression
```

## Comparing `sball-0.9.5.tar` & `sball-0.9.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 02:30:16.489534 sball-0.9.5/
--rw-rw-rw-   0        0        0     4100 2023-04-15 02:30:16.488535 sball-0.9.5/PKG-INFO
--rw-rw-rw-   0        0        0     3625 2023-04-15 02:22:06.000000 sball-0.9.5/README.md
--rw-rw-rw-   0        0        0      632 2023-04-15 02:12:59.000000 sball-0.9.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-15 02:30:16.490537 sball-0.9.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-15 02:30:16.457439 sball-0.9.5/src/
-drwxrwxrwx   0        0        0        0 2023-04-15 02:30:16.464438 sball-0.9.5/src/sball/
--rw-rw-rw-   0        0        0       38 2023-04-15 02:26:03.000000 sball-0.9.5/src/sball/__init__.py
--rw-rw-rw-   0        0        0      302 2023-04-15 02:27:19.000000 sball-0.9.5/src/sball/__main__.py
--rw-rw-rw-   0        0        0     4795 2023-04-15 02:28:23.000000 sball-0.9.5/src/sball/sball.py
-drwxrwxrwx   0        0        0        0 2023-04-15 02:30:16.487535 sball-0.9.5/src/sball.egg-info/
--rw-rw-rw-   0        0        0     4100 2023-04-15 02:30:16.000000 sball-0.9.5/src/sball.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      255 2023-04-15 02:30:16.000000 sball-0.9.5/src/sball.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 02:30:16.000000 sball-0.9.5/src/sball.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-04-15 02:30:16.000000 sball-0.9.5/src/sball.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        6 2023-04-15 02:30:16.000000 sball-0.9.5/src/sball.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-15 03:10:24.516938 sball-0.9.6/
+-rw-rw-rw-   0        0        0     4244 2023-04-15 03:10:24.514938 sball-0.9.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3769 2023-04-15 03:09:19.000000 sball-0.9.6/README.md
+-rw-rw-rw-   0        0        0      632 2023-04-15 03:05:45.000000 sball-0.9.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-15 03:10:24.516938 sball-0.9.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-15 03:10:24.495937 sball-0.9.6/src/
+drwxrwxrwx   0        0        0        0 2023-04-15 03:10:24.503937 sball-0.9.6/src/sball/
+-rw-rw-rw-   0        0        0       38 2023-04-15 03:05:38.000000 sball-0.9.6/src/sball/__init__.py
+-rw-rw-rw-   0        0        0      302 2023-04-15 02:27:19.000000 sball-0.9.6/src/sball/__main__.py
+-rw-rw-rw-   0        0        0     4972 2023-04-15 03:09:39.000000 sball-0.9.6/src/sball/sball.py
+drwxrwxrwx   0        0        0        0 2023-04-15 03:10:24.513938 sball-0.9.6/src/sball.egg-info/
+-rw-rw-rw-   0        0        0     4244 2023-04-15 03:10:24.000000 sball-0.9.6/src/sball.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      255 2023-04-15 03:10:24.000000 sball-0.9.6/src/sball.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 03:10:24.000000 sball-0.9.6/src/sball.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-04-15 03:10:24.000000 sball-0.9.6/src/sball.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        6 2023-04-15 03:10:24.000000 sball-0.9.6/src/sball.egg-info/top_level.txt
```

### Comparing `sball-0.9.5/PKG-INFO` & `sball-0.9.6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,26 @@
-Metadata-Version: 2.1
-Name: sball
-Version: 0.9.5
-Summary: Submit scripts in job arrays using Yale's dSQ.
-Author-email: Michael Wilson <michael.a.wilson@yale.edu>
-Project-URL: Homepage, https://github.com/mawilson1234/sball
-Keywords: slurm,job array,sbatch,dSQ,dsq
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3
-Description-Content-Type: text/markdown
-
 # sball
 
 `sball` facilitates submitting multiple scripts in Slurm job arrays using Yale's dSQ module. "sball" is short for "sbatch all".
 
 ## Usage
 
 After installing using `pip`, you can run `sball` as a command. It takes a few arguments, which are the following. Any additional arguments not provided here are passed along to `sbatch` when the job array is submitted. Arguments must be specified as `key=value` pairs, with the exception of the `pattern` argument, which should always be passed as the final argument. Additional arguments should be specified in the usual way for `sbatch`; i.e., `--$argument_name $argument_value`.
 
 If you need to include spaces in arguments, make sure to escape them by using single quotes. If you do not escape `pattern` using single quotes, make sure to escape any `*` in the glob expression with a backslash, since otherwise they will be expanded by the shell before sball gets them.
 
 - `name`: (required) the name to give the job array.
 - `regex`: (optional) only scripts with filenames matching `regex` will be included in any arrays.
+- `log_dir`: (optional) the directory where log files for the job array should be stored. Default is `joblogs`.
 - (`pattern`): (required, not named) a glob expression that matches scripts to include in job arrays. Only files ending in `.sh` that match the glob will be included. If a glob expression is insufficient to filter to just the scripts you want, you should use the `regex` argument.
 - Additional arguments are passed to the underlying calls to `sbatch`. This allows you to, e.g., set up job dependencies. They should be inserted _before_ the final, pattern argument.
 
 ## Description
 
-`sball` finds all `.sh` scripts matching `pattern` (and `regex`, if provided). If scripts are found, it sorts them into bins with unique sets of SBATCH options (since job arrays must all be run with the same SBATCH options). For each bin, the scripts are added to a job file, where the contents of each script takes up a single line. These files are named `$name.txt`, and are saved in the deepest directory common to all scripts in a bin. In case there is more than one bin, the file is suffixed with their bin number. Then, `dsq` is loaded and called to create a job script from this file with the SBATCH options for that bin. Finally, the created job script is submitted to the queue with `sbatch`, and the (now unnecessary) job script is removed. The `$name.txt` files must be present when the job actually procs in the queue, so they are not removed (and should not be removed until after the jobs finish).
+`sball` finds all `.sh` scripts matching `pattern` (and `regex`, if provided). If scripts are found, it sorts them into bins with unique sets of SBATCH options (since job arrays must all be run with the same SBATCH options). For each bin, the scripts are added to a job file, where the contents of each script takes up a single line. These files are named `$name.txt`, and are saved in the deepest directory common to all scripts in a bin. In case there is more than one bin, the file is suffixed with their bin number. Then, `dsq` called to create a job script from this file with the SBATCH options for that bin. Finally, the created job script is submitted to the queue with `sbatch`, and the (now unnecessary) job script is removed. The `$name.txt` files must be present when the job actually procs in the queue, so they are not removed (and should not be removed until after the jobs finish).
 
 In case a bin contains only one script, that script is just submitted in the usual way with `sbatch`, as a fallback.
 
 ## Examples
 
 Sample directory structure:
 ```
@@ -43,15 +31,16 @@
 	├── script1.sh
 	├── script2.sh
 	├── script3.sh
 	└── ...
 ```
 
 To submit all the scripts in `main-project-directory/scripts` in a job array named `my-job-array`, from `main-project-directory` you would run:
-```
+```bash
+module load dSQ # if not already loaded
 sball name=my-job-array scripts/\*
 ```
 
 Note that the `*` in the glob expression in `pattern` is escaped. After running this, your job array will be created, and you will have a new file in `main-project-directory/scripts` that Slurm references to find the jobs.
 ```
 main-project-directory/
 ├── ...
@@ -59,8 +48,8 @@
 └── scripts/
 	├── script1.sh
 	├── script2.sh
 	├── script3.sh
 	├── ...
 	└── my-job-array.txt
 ```
-After your job array finishes running, you can safely remove `my-job-array.txt`. You can make further refinements of which scripts to run by changing the glob expression, or by using the `regex=` argument.
+After your job array finishes running, you can safely remove `my-job-array.txt`. You can make further refinements of which scripts to run by changing the glob expression, or by using the `regex=` argument.
```

### Comparing `sball-0.9.5/README.md` & `sball-0.9.6/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,39 @@
+Metadata-Version: 2.1
+Name: sball
+Version: 0.9.6
+Summary: Submit scripts in job arrays using Yale's dSQ.
+Author-email: Michael Wilson <michael.a.wilson@yale.edu>
+Project-URL: Homepage, https://github.com/mawilson1234/sball
+Keywords: slurm,job array,sbatch,dSQ,dsq
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3
+Description-Content-Type: text/markdown
+
 # sball
 
 `sball` facilitates submitting multiple scripts in Slurm job arrays using Yale's dSQ module. "sball" is short for "sbatch all".
 
 ## Usage
 
 After installing using `pip`, you can run `sball` as a command. It takes a few arguments, which are the following. Any additional arguments not provided here are passed along to `sbatch` when the job array is submitted. Arguments must be specified as `key=value` pairs, with the exception of the `pattern` argument, which should always be passed as the final argument. Additional arguments should be specified in the usual way for `sbatch`; i.e., `--$argument_name $argument_value`.
 
 If you need to include spaces in arguments, make sure to escape them by using single quotes. If you do not escape `pattern` using single quotes, make sure to escape any `*` in the glob expression with a backslash, since otherwise they will be expanded by the shell before sball gets them.
 
 - `name`: (required) the name to give the job array.
 - `regex`: (optional) only scripts with filenames matching `regex` will be included in any arrays.
+- `log_dir`: (optional) the directory where log files for the job array should be stored. Default is `joblogs`.
 - (`pattern`): (required, not named) a glob expression that matches scripts to include in job arrays. Only files ending in `.sh` that match the glob will be included. If a glob expression is insufficient to filter to just the scripts you want, you should use the `regex` argument.
 - Additional arguments are passed to the underlying calls to `sbatch`. This allows you to, e.g., set up job dependencies. They should be inserted _before_ the final, pattern argument.
 
 ## Description
 
-`sball` finds all `.sh` scripts matching `pattern` (and `regex`, if provided). If scripts are found, it sorts them into bins with unique sets of SBATCH options (since job arrays must all be run with the same SBATCH options). For each bin, the scripts are added to a job file, where the contents of each script takes up a single line. These files are named `$name.txt`, and are saved in the deepest directory common to all scripts in a bin. In case there is more than one bin, the file is suffixed with their bin number. Then, `dsq` is loaded and called to create a job script from this file with the SBATCH options for that bin. Finally, the created job script is submitted to the queue with `sbatch`, and the (now unnecessary) job script is removed. The `$name.txt` files must be present when the job actually procs in the queue, so they are not removed (and should not be removed until after the jobs finish).
+`sball` finds all `.sh` scripts matching `pattern` (and `regex`, if provided). If scripts are found, it sorts them into bins with unique sets of SBATCH options (since job arrays must all be run with the same SBATCH options). For each bin, the scripts are added to a job file, where the contents of each script takes up a single line. These files are named `$name.txt`, and are saved in the deepest directory common to all scripts in a bin. In case there is more than one bin, the file is suffixed with their bin number. Then, `dsq` called to create a job script from this file with the SBATCH options for that bin. Finally, the created job script is submitted to the queue with `sbatch`, and the (now unnecessary) job script is removed. The `$name.txt` files must be present when the job actually procs in the queue, so they are not removed (and should not be removed until after the jobs finish).
 
 In case a bin contains only one script, that script is just submitted in the usual way with `sbatch`, as a fallback.
 
 ## Examples
 
 Sample directory structure:
 ```
@@ -30,15 +44,16 @@
 	├── script1.sh
 	├── script2.sh
 	├── script3.sh
 	└── ...
 ```
 
 To submit all the scripts in `main-project-directory/scripts` in a job array named `my-job-array`, from `main-project-directory` you would run:
-```
+```bash
+module load dSQ # if not already loaded
 sball name=my-job-array scripts/\*
 ```
 
 Note that the `*` in the glob expression in `pattern` is escaped. After running this, your job array will be created, and you will have a new file in `main-project-directory/scripts` that Slurm references to find the jobs.
 ```
 main-project-directory/
 ├── ...
@@ -46,8 +61,8 @@
 └── scripts/
 	├── script1.sh
 	├── script2.sh
 	├── script3.sh
 	├── ...
 	└── my-job-array.txt
 ```
-After your job array finishes running, you can safely remove `my-job-array.txt`. You can make further refinements of which scripts to run by changing the glob expression, or by using the `regex=` argument.
+After your job array finishes running, you can safely remove `my-job-array.txt`. You can make further refinements of which scripts to run by changing the glob expression, or by using the `regex=` argument.
```

### Comparing `sball-0.9.5/pyproject.toml` & `sball-0.9.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires=['setuptools', 'wheel']
 build-backend='setuptools.build_meta'
 
 [project]
 name='sball'
-version='0.9.5'
+version='0.9.6'
 description="Submit scripts in job arrays using Yale's dSQ."
 readme='README.md'
 authors=[{name="Michael Wilson", email='michael.a.wilson@yale.edu'}]
 classifiers=[
 	'Development Status :: 4 - Beta',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
```

### Comparing `sball-0.9.5/src/sball/sball.py` & `sball-0.9.6/src/sball/sball.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 		if not script_options in batches.keys():
 			batches[script_options] = [script_file]
 		else:
 			batches[script_options].append(script_file)
 	
 	return batches
 
-def submit_batched_jobs(name, args, batches):
+def submit_batched_jobs(name, args, batches, log_dir = 'joblogs'):
 	print('Submitting jobs in ' + str(len(batches)) + ' array(s).')
 	for i, (options, files) in enumerate(batches.items()):
 		if len(files) == 1:
 			x = subprocess.Popen(['sbatch', *args, files[0]])
 			time.sleep(1)
 			x.kill()
 			continue
@@ -75,17 +75,17 @@
 			
 		options = ['--' + k + ' ' + v for k, v in options]
 		options = [i for sublist in [option.split(' ') for option in options] for i in sublist]
 		
 		x = subprocess.Popen([
 			'dsq', 
 			'--job-file', joblist_file, 
-			'--status-dir', 'joblogs' + os.path.sep,
+			'--status-dir', log_dir + os.path.sep,
 			'--job-name', name + formatter,
-			'--output', os.path.join('joblogs', name + formatter + '-%A_%a.txt'),
+			'--output', os.path.join(log_dir, name + formatter + '-%A_%a.txt'),
 			'--batch-file', os.path.join(dirname, name + formatter + '.sh'),
 			*options, 
 			*args
 		], stdout=subprocess.DEVNULL)
 		time.sleep(2)
 		x.kill()
 		
@@ -115,14 +115,17 @@
 	args = [arg for arg in s[:-1] if not arg.startswith('name=')]
 	name = [arg.split('=')[1] for arg in s[:-1] if arg.startswith('name=')]
 	name = name[0] if name else []
 	
 	regex = [arg.split('=')[1] for arg in s[:-1] if arg.startswith('regex=')]
 	regex = regex[0] if regex else []
 	
+	log_dir = [arg.split('=')[1] for arg in s[:-1] if arg.startswith('log_dir=')]
+	log_dir = log_dir[0] if log_dir else 'joblogs'
+	
 	globbed = []
 	for script in scripts:
 		globbed.append(glob(script, recursive=True))
 	
 	globbed = [script for l in globbed for script in l if script.endswith('.sh')]
 	
 	if regex:
@@ -132,21 +135,21 @@
 		print('No scripts matching expression "' + s[-1] + '" found.')
 		sys.exit(0)
 	
 	globbed = sorted(globbed)
 	batches = find_batches(globbed)
 	
 	try:
-		_ = os.system('module load dSQ')
-		submit_batched_jobs(name=name, args=args, batches=batches)
+		submit_batched_jobs(name=name, args=args, batches=batches, log_dir=log_dir)
 	except KeyboardInterrupt:
 		print('User terminated.')
 		sys.exit(0)
 	except Exception:
-		response = input('Error submitting jobs using dSQ. Submit individually (y/n)? ')
+		print('Error submitting jobs using dSQ (did you `module load dSQ` first?).')
+		response = input('Submit individually (y/n)? ')
 		while response not in {'y', 'n'}:
 			response = input('Invalid option. Please enter one of "y", "n": ')	
 		
 		if response == 'y':
 			for script in globbed:
 				x = subprocess.Popen(['sbatch', *args, script])
 				time.sleep(1)
```

### Comparing `sball-0.9.5/src/sball.egg-info/PKG-INFO` & `sball-0.9.6/src/sball.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sball
-Version: 0.9.5
+Version: 0.9.6
 Summary: Submit scripts in job arrays using Yale's dSQ.
 Author-email: Michael Wilson <michael.a.wilson@yale.edu>
 Project-URL: Homepage, https://github.com/mawilson1234/sball
 Keywords: slurm,job array,sbatch,dSQ,dsq
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -19,20 +19,21 @@
 
 After installing using `pip`, you can run `sball` as a command. It takes a few arguments, which are the following. Any additional arguments not provided here are passed along to `sbatch` when the job array is submitted. Arguments must be specified as `key=value` pairs, with the exception of the `pattern` argument, which should always be passed as the final argument. Additional arguments should be specified in the usual way for `sbatch`; i.e., `--$argument_name $argument_value`.
 
 If you need to include spaces in arguments, make sure to escape them by using single quotes. If you do not escape `pattern` using single quotes, make sure to escape any `*` in the glob expression with a backslash, since otherwise they will be expanded by the shell before sball gets them.
 
 - `name`: (required) the name to give the job array.
 - `regex`: (optional) only scripts with filenames matching `regex` will be included in any arrays.
+- `log_dir`: (optional) the directory where log files for the job array should be stored. Default is `joblogs`.
 - (`pattern`): (required, not named) a glob expression that matches scripts to include in job arrays. Only files ending in `.sh` that match the glob will be included. If a glob expression is insufficient to filter to just the scripts you want, you should use the `regex` argument.
 - Additional arguments are passed to the underlying calls to `sbatch`. This allows you to, e.g., set up job dependencies. They should be inserted _before_ the final, pattern argument.
 
 ## Description
 
-`sball` finds all `.sh` scripts matching `pattern` (and `regex`, if provided). If scripts are found, it sorts them into bins with unique sets of SBATCH options (since job arrays must all be run with the same SBATCH options). For each bin, the scripts are added to a job file, where the contents of each script takes up a single line. These files are named `$name.txt`, and are saved in the deepest directory common to all scripts in a bin. In case there is more than one bin, the file is suffixed with their bin number. Then, `dsq` is loaded and called to create a job script from this file with the SBATCH options for that bin. Finally, the created job script is submitted to the queue with `sbatch`, and the (now unnecessary) job script is removed. The `$name.txt` files must be present when the job actually procs in the queue, so they are not removed (and should not be removed until after the jobs finish).
+`sball` finds all `.sh` scripts matching `pattern` (and `regex`, if provided). If scripts are found, it sorts them into bins with unique sets of SBATCH options (since job arrays must all be run with the same SBATCH options). For each bin, the scripts are added to a job file, where the contents of each script takes up a single line. These files are named `$name.txt`, and are saved in the deepest directory common to all scripts in a bin. In case there is more than one bin, the file is suffixed with their bin number. Then, `dsq` called to create a job script from this file with the SBATCH options for that bin. Finally, the created job script is submitted to the queue with `sbatch`, and the (now unnecessary) job script is removed. The `$name.txt` files must be present when the job actually procs in the queue, so they are not removed (and should not be removed until after the jobs finish).
 
 In case a bin contains only one script, that script is just submitted in the usual way with `sbatch`, as a fallback.
 
 ## Examples
 
 Sample directory structure:
 ```
@@ -43,15 +44,16 @@
 	├── script1.sh
 	├── script2.sh
 	├── script3.sh
 	└── ...
 ```
 
 To submit all the scripts in `main-project-directory/scripts` in a job array named `my-job-array`, from `main-project-directory` you would run:
-```
+```bash
+module load dSQ # if not already loaded
 sball name=my-job-array scripts/\*
 ```
 
 Note that the `*` in the glob expression in `pattern` is escaped. After running this, your job array will be created, and you will have a new file in `main-project-directory/scripts` that Slurm references to find the jobs.
 ```
 main-project-directory/
 ├── ...
```

