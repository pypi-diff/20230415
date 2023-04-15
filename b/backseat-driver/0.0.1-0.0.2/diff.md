# Comparing `tmp/backseat-driver-0.0.1.tar.gz` & `tmp/backseat-driver-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backseat-driver-0.0.1.tar", last modified: Sat Apr 15 17:17:46 2023, max compression
+gzip compressed data, was "backseat-driver-0.0.2.tar", last modified: Sat Apr 15 18:47:32 2023, max compression
```

## Comparing `backseat-driver-0.0.1.tar` & `backseat-driver-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 leo        (501) staff       (20)        0 2023-04-15 17:17:46.592748 backseat-driver-0.0.1/
--rw-r--r--   0 leo        (501) staff       (20)     1066 2023-03-30 10:49:47.000000 backseat-driver-0.0.1/LICENSE
--rw-r--r--   0 leo        (501) staff       (20)     3703 2023-04-15 17:17:46.592864 backseat-driver-0.0.1/PKG-INFO
--rw-r--r--   0 leo        (501) staff       (20)     3178 2023-04-08 15:18:29.000000 backseat-driver-0.0.1/README.md
-drwxr-xr-x   0 leo        (501) staff       (20)        0 2023-04-15 17:17:46.588480 backseat-driver-0.0.1/backseat_driver/
--rw-r--r--   0 leo        (501) staff       (20)       83 2023-04-15 17:13:10.000000 backseat-driver-0.0.1/backseat_driver/__init__.py
--rw-r--r--   0 leo        (501) staff       (20)     5714 2023-04-08 19:40:12.000000 backseat-driver-0.0.1/backseat_driver/backseat_driver.py
-drwxr-xr-x   0 leo        (501) staff       (20)        0 2023-04-15 17:17:46.591565 backseat-driver-0.0.1/backseat_driver.egg-info/
--rw-r--r--   0 leo        (501) staff       (20)     3703 2023-04-15 17:17:46.000000 backseat-driver-0.0.1/backseat_driver.egg-info/PKG-INFO
--rw-r--r--   0 leo        (501) staff       (20)      371 2023-04-15 17:17:46.000000 backseat-driver-0.0.1/backseat_driver.egg-info/SOURCES.txt
--rw-r--r--   0 leo        (501) staff       (20)        1 2023-04-15 17:17:46.000000 backseat-driver-0.0.1/backseat_driver.egg-info/dependency_links.txt
--rw-r--r--   0 leo        (501) staff       (20)       73 2023-04-15 17:17:46.000000 backseat-driver-0.0.1/backseat_driver.egg-info/entry_points.txt
--rw-r--r--   0 leo        (501) staff       (20)        7 2023-04-15 17:17:46.000000 backseat-driver-0.0.1/backseat_driver.egg-info/requires.txt
--rw-r--r--   0 leo        (501) staff       (20)       16 2023-04-15 17:17:46.000000 backseat-driver-0.0.1/backseat_driver.egg-info/top_level.txt
--rw-r--r--   0 leo        (501) staff       (20)       81 2023-04-15 17:10:33.000000 backseat-driver-0.0.1/pyproject.toml
--rw-r--r--   0 leo        (501) staff       (20)      797 2023-04-15 17:17:46.593437 backseat-driver-0.0.1/setup.cfg
-drwxr-xr-x   0 leo        (501) staff       (20)        0 2023-04-15 17:17:46.592004 backseat-driver-0.0.1/tests/
--rw-r--r--   0 leo        (501) staff       (20)     8181 2023-04-08 19:40:12.000000 backseat-driver-0.0.1/tests/test_backseat_driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:47:32.150813 backseat-driver-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-15 18:47:10.000000 backseat-driver-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-04-15 18:47:32.150813 backseat-driver-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-04-15 18:47:10.000000 backseat-driver-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:47:32.150813 backseat-driver-0.0.2/backseat_driver/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-15 18:47:10.000000 backseat-driver-0.0.2/backseat_driver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-04-15 18:47:10.000000 backseat-driver-0.0.2/backseat_driver/backseat_driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:47:32.150813 backseat-driver-0.0.2/backseat_driver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-04-15 18:47:32.000000 backseat-driver-0.0.2/backseat_driver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-15 18:47:32.000000 backseat-driver-0.0.2/backseat_driver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 18:47:32.000000 backseat-driver-0.0.2/backseat_driver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-15 18:47:32.000000 backseat-driver-0.0.2/backseat_driver.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-15 18:47:32.000000 backseat-driver-0.0.2/backseat_driver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-15 18:47:32.000000 backseat-driver-0.0.2/backseat_driver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-15 18:47:10.000000 backseat-driver-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-15 18:47:32.150813 backseat-driver-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:47:32.150813 backseat-driver-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     8181 2023-04-15 18:47:10.000000 backseat-driver-0.0.2/tests/test_backseat_driver.py
```

### Comparing `backseat-driver-0.0.1/LICENSE` & `backseat-driver-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `backseat-driver-0.0.1/PKG-INFO` & `backseat-driver-0.0.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,76 +1,116 @@
 Metadata-Version: 2.1
 Name: backseat-driver
-Version: 0.0.1
+Version: 0.0.2
 Summary: A tool for large language model-enabled code review.
 Home-page: https://github.com/kostaleonard/backseat-driver
 Author: Leo Kosta
 Author-email: kostaleonard@gmail.com
 Project-URL: Bug Tracker, https://github.com/kostaleonard/backseat-driver/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Backseat Driver
 
-Software developers want reviews from colleagues so that they can improve the
-code they write.
-But often, a developer's peers are too busy or lack the context to provide
-comments.
-Backseat Driver prompts a large language model to give a code base a letter
-grade for readability, expressiveness, and organization.
-It also instructs the model to explain its reasoning.
-Developers gain the benefits of a code review without needing another engineer.
+Requests a code review from a large language model.
 
-Backseat Driver is not a linting tool.
-Linters check code compliance with a language-specific style guide.
-While linters are extremely valuable for promoting readability and
-standardizing practices within a team, they don't examine a code base for key
-elements that make code relatable to another human being.
-For example, linters don't comment on whether function or variable names
-express the intent of the author.
-They only ensure that names use the correct combination of lower case, upper
-case, and other characters.
-Linters also do not discuss whether functions or classes have intuitive
-interfaces.
-Backseat Driver goes beyond linting, looking for deeper ways to improve code.
+Software developers want reviews so that they can improve their code.
+But developers are busy.
+Peers may be unavailable or lack the context to provide comments.
+Backseat Driver prompts a large language model to give code a letter grade for
+readability, expressiveness, and organization.
+It also instructs the model to explain its reasoning.
+Developers gain the benefits of code review without needing another engineer.
 
 ## Installation
 
-TODO pip install
+```shell
+pip install backseat-driver
+```
 
 ## Usage
 
-TODO users need to specify an OpenAI API key
+Users need to [create an OpenAI account](https://platform.openai.com/signup)
+and API key.
+Backseat Driver needs the API key to be able to request code review from a
+language model.
+Set the `OPENAI_API_KEY` environment variable to your API key.
+
+Note that OpenAI will charge your account for Backseat Driver's requests.
+Each Backseat Driver invocation will make a request of at most 4096 tokens on a
+language model.
+[ChatGPT's current pricing model](https://openai.com/pricing) is $0.002 per 1K
+tokens.
+At this price, users can expect each call to Backseat Driver to cost
+$0.002 * 4.096 = $0.008192, or just under 1 cent.
 
 ### Local
 
-TODO
+Run Backseat Driver on the command line with the following.
+
+```shell
+backseat-driver my_script.py
+```
+
+Provide multiple scripts for simultaneous code review of all given files.
+
+```shell
+backseat-driver script1.py script2.py script3.py
+```
+
+Wildcard operators also work as expected.
+
+```shell
+backseat-driver *.py
+```
+
+Set the `fail_under` flag to cause Backseat Driver to exit with an error if the
+model gives the code a lower grade than what you have specified.
+
+```shell
+backseat-driver --fail_under B *.py
+```
 
 ### GitHub Actions
 
 TODO
 
 ```yaml
 # TODO not sure what source-directory should be in GitHub Actions
 backseat-driver:
   openai_api_key: ${{ secrets.OPENAI_API_KEY }}
   fail_under: B
   source_directory: /
   filter_files_by_suffix: ".py"
 ```
 
+## Help
+
+```console
+foo@bar:~$ backseat-driver -h
+usage: backseat-driver [-h] [--fail_under {A,B,C,D}] filenames [filenames ...]
+
+Requests a code review from a large language model (LLM). The model will grade the code based on readability, expressiveness, and organization. The output will include a letter grade in ['A', 'B', 'C', 'D', 'F'], as well as the model's reasoning.
+
+positional arguments:
+  filenames             The files to pass to the LLM for code review.
+
+options:
+  -h, --help            show this help message and exit
+  --fail_under {A,B,C,D}
+                        If specified, exit with non-zero status if the LLM's grade falls below the given value. This value is not inclusive: if this value is "B" and the LLM gives a final grade of "B," then the program will exit with a zero status. If not specified, then the program will exit with a zero status no matter the LLM's grade.
+```
+
 ## Example output
 
 You can try Backseat Driver on the input program below to see how it works.
-Copy the code below into a file and run Backseat Driver with the following.
-
-TODO show python command to reproduce this output
+Copy the code into `test.py`.
 
 ```python
 """A file for testing prompt creation."""
 
 
 def fib(n):
     """Returns the nth fibonacci number."""
@@ -94,14 +134,20 @@
         return [n]
     if n % 2 == 0:
         return [n] + hailstone(n // 2)
     return [n] + hailstone(3 * n + 1)
 
 ```
 
+Run Backseat Driver with the following.
+
+```shell
+backseat-driver test.py
+```
+
 What Backseat Driver says:
 
 > Grade: A
 > 
 > This code is well-written, easy to read, and well-organized. The function names are clear and descriptive, and the docstrings provide useful information about the functions' purpose and behavior. The code also follows the recommended Python style guidelines (PEP 8), including appropriate indentation, whitespace, and naming conventions. Overall, there are no major issues with the code, and it is highly readable and maintainable.
 > 
 > One possible improvement could be to add some error handling to the `fib()` and `fact()` functions, for cases where the input is not a positive integer. Another potential improvement could be to add some more comments to explain the logic behind the `hailstone()` function. However, these are minor suggestions and are not necessary for the code to function correctly.
```

### Comparing `backseat-driver-0.0.1/README.md` & `backseat-driver-0.0.2/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,62 +1,102 @@
 # Backseat Driver
 
-Software developers want reviews from colleagues so that they can improve the
-code they write.
-But often, a developer's peers are too busy or lack the context to provide
-comments.
-Backseat Driver prompts a large language model to give a code base a letter
-grade for readability, expressiveness, and organization.
-It also instructs the model to explain its reasoning.
-Developers gain the benefits of a code review without needing another engineer.
+Requests a code review from a large language model.
 
-Backseat Driver is not a linting tool.
-Linters check code compliance with a language-specific style guide.
-While linters are extremely valuable for promoting readability and
-standardizing practices within a team, they don't examine a code base for key
-elements that make code relatable to another human being.
-For example, linters don't comment on whether function or variable names
-express the intent of the author.
-They only ensure that names use the correct combination of lower case, upper
-case, and other characters.
-Linters also do not discuss whether functions or classes have intuitive
-interfaces.
-Backseat Driver goes beyond linting, looking for deeper ways to improve code.
+Software developers want reviews so that they can improve their code.
+But developers are busy.
+Peers may be unavailable or lack the context to provide comments.
+Backseat Driver prompts a large language model to give code a letter grade for
+readability, expressiveness, and organization.
+It also instructs the model to explain its reasoning.
+Developers gain the benefits of code review without needing another engineer.
 
 ## Installation
 
-TODO pip install
+```shell
+pip install backseat-driver
+```
 
 ## Usage
 
-TODO users need to specify an OpenAI API key
+Users need to [create an OpenAI account](https://platform.openai.com/signup)
+and API key.
+Backseat Driver needs the API key to be able to request code review from a
+language model.
+Set the `OPENAI_API_KEY` environment variable to your API key.
+
+Note that OpenAI will charge your account for Backseat Driver's requests.
+Each Backseat Driver invocation will make a request of at most 4096 tokens on a
+language model.
+[ChatGPT's current pricing model](https://openai.com/pricing) is $0.002 per 1K
+tokens.
+At this price, users can expect each call to Backseat Driver to cost
+$0.002 * 4.096 = $0.008192, or just under 1 cent.
 
 ### Local
 
-TODO
+Run Backseat Driver on the command line with the following.
+
+```shell
+backseat-driver my_script.py
+```
+
+Provide multiple scripts for simultaneous code review of all given files.
+
+```shell
+backseat-driver script1.py script2.py script3.py
+```
+
+Wildcard operators also work as expected.
+
+```shell
+backseat-driver *.py
+```
+
+Set the `fail_under` flag to cause Backseat Driver to exit with an error if the
+model gives the code a lower grade than what you have specified.
+
+```shell
+backseat-driver --fail_under B *.py
+```
 
 ### GitHub Actions
 
 TODO
 
 ```yaml
 # TODO not sure what source-directory should be in GitHub Actions
 backseat-driver:
   openai_api_key: ${{ secrets.OPENAI_API_KEY }}
   fail_under: B
   source_directory: /
   filter_files_by_suffix: ".py"
 ```
 
+## Help
+
+```console
+foo@bar:~$ backseat-driver -h
+usage: backseat-driver [-h] [--fail_under {A,B,C,D}] filenames [filenames ...]
+
+Requests a code review from a large language model (LLM). The model will grade the code based on readability, expressiveness, and organization. The output will include a letter grade in ['A', 'B', 'C', 'D', 'F'], as well as the model's reasoning.
+
+positional arguments:
+  filenames             The files to pass to the LLM for code review.
+
+options:
+  -h, --help            show this help message and exit
+  --fail_under {A,B,C,D}
+                        If specified, exit with non-zero status if the LLM's grade falls below the given value. This value is not inclusive: if this value is "B" and the LLM gives a final grade of "B," then the program will exit with a zero status. If not specified, then the program will exit with a zero status no matter the LLM's grade.
+```
+
 ## Example output
 
 You can try Backseat Driver on the input program below to see how it works.
-Copy the code below into a file and run Backseat Driver with the following.
-
-TODO show python command to reproduce this output
+Copy the code into `test.py`.
 
 ```python
 """A file for testing prompt creation."""
 
 
 def fib(n):
     """Returns the nth fibonacci number."""
@@ -80,14 +120,20 @@
         return [n]
     if n % 2 == 0:
         return [n] + hailstone(n // 2)
     return [n] + hailstone(3 * n + 1)
 
 ```
 
+Run Backseat Driver with the following.
+
+```shell
+backseat-driver test.py
+```
+
 What Backseat Driver says:
 
 > Grade: A
 > 
 > This code is well-written, easy to read, and well-organized. The function names are clear and descriptive, and the docstrings provide useful information about the functions' purpose and behavior. The code also follows the recommended Python style guidelines (PEP 8), including appropriate indentation, whitespace, and naming conventions. Overall, there are no major issues with the code, and it is highly readable and maintainable.
 > 
 > One possible improvement could be to add some error handling to the `fib()` and `fact()` functions, for cases where the input is not a positive integer. Another potential improvement could be to add some more comments to explain the logic behind the `hailstone()` function. However, these are minor suggestions and are not necessary for the code to function correctly.
```

### Comparing `backseat-driver-0.0.1/backseat_driver/backseat_driver.py` & `backseat-driver-0.0.2/backseat_driver/backseat_driver.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,15 @@
         description="Requests a code review from a large language model "
         "(LLM). The model will grade the code based on "
         "readability, expressiveness, and organization. The "
         f"output will include a letter grade in {LETTER_GRADES}, "
         "as well as the model's reasoning."
     )
     parser.add_argument(
-        "filenames", nargs="+", help="The files to pass to the LLm for code review."
+        "filenames", nargs="+", help="The files to pass to the LLM for code review."
     )
     parser.add_argument(
         "--fail_under",
         default=None,
         choices=LETTER_GRADES[:-1],
         help="If specified, exit with non-zero status if the LLM's grade "
         "falls below the given value. This value is not inclusive: if "
```

### Comparing `backseat-driver-0.0.1/backseat_driver.egg-info/PKG-INFO` & `backseat-driver-0.0.2/backseat_driver.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,76 +1,116 @@
 Metadata-Version: 2.1
 Name: backseat-driver
-Version: 0.0.1
+Version: 0.0.2
 Summary: A tool for large language model-enabled code review.
 Home-page: https://github.com/kostaleonard/backseat-driver
 Author: Leo Kosta
 Author-email: kostaleonard@gmail.com
 Project-URL: Bug Tracker, https://github.com/kostaleonard/backseat-driver/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Backseat Driver
 
-Software developers want reviews from colleagues so that they can improve the
-code they write.
-But often, a developer's peers are too busy or lack the context to provide
-comments.
-Backseat Driver prompts a large language model to give a code base a letter
-grade for readability, expressiveness, and organization.
-It also instructs the model to explain its reasoning.
-Developers gain the benefits of a code review without needing another engineer.
+Requests a code review from a large language model.
 
-Backseat Driver is not a linting tool.
-Linters check code compliance with a language-specific style guide.
-While linters are extremely valuable for promoting readability and
-standardizing practices within a team, they don't examine a code base for key
-elements that make code relatable to another human being.
-For example, linters don't comment on whether function or variable names
-express the intent of the author.
-They only ensure that names use the correct combination of lower case, upper
-case, and other characters.
-Linters also do not discuss whether functions or classes have intuitive
-interfaces.
-Backseat Driver goes beyond linting, looking for deeper ways to improve code.
+Software developers want reviews so that they can improve their code.
+But developers are busy.
+Peers may be unavailable or lack the context to provide comments.
+Backseat Driver prompts a large language model to give code a letter grade for
+readability, expressiveness, and organization.
+It also instructs the model to explain its reasoning.
+Developers gain the benefits of code review without needing another engineer.
 
 ## Installation
 
-TODO pip install
+```shell
+pip install backseat-driver
+```
 
 ## Usage
 
-TODO users need to specify an OpenAI API key
+Users need to [create an OpenAI account](https://platform.openai.com/signup)
+and API key.
+Backseat Driver needs the API key to be able to request code review from a
+language model.
+Set the `OPENAI_API_KEY` environment variable to your API key.
+
+Note that OpenAI will charge your account for Backseat Driver's requests.
+Each Backseat Driver invocation will make a request of at most 4096 tokens on a
+language model.
+[ChatGPT's current pricing model](https://openai.com/pricing) is $0.002 per 1K
+tokens.
+At this price, users can expect each call to Backseat Driver to cost
+$0.002 * 4.096 = $0.008192, or just under 1 cent.
 
 ### Local
 
-TODO
+Run Backseat Driver on the command line with the following.
+
+```shell
+backseat-driver my_script.py
+```
+
+Provide multiple scripts for simultaneous code review of all given files.
+
+```shell
+backseat-driver script1.py script2.py script3.py
+```
+
+Wildcard operators also work as expected.
+
+```shell
+backseat-driver *.py
+```
+
+Set the `fail_under` flag to cause Backseat Driver to exit with an error if the
+model gives the code a lower grade than what you have specified.
+
+```shell
+backseat-driver --fail_under B *.py
+```
 
 ### GitHub Actions
 
 TODO
 
 ```yaml
 # TODO not sure what source-directory should be in GitHub Actions
 backseat-driver:
   openai_api_key: ${{ secrets.OPENAI_API_KEY }}
   fail_under: B
   source_directory: /
   filter_files_by_suffix: ".py"
 ```
 
+## Help
+
+```console
+foo@bar:~$ backseat-driver -h
+usage: backseat-driver [-h] [--fail_under {A,B,C,D}] filenames [filenames ...]
+
+Requests a code review from a large language model (LLM). The model will grade the code based on readability, expressiveness, and organization. The output will include a letter grade in ['A', 'B', 'C', 'D', 'F'], as well as the model's reasoning.
+
+positional arguments:
+  filenames             The files to pass to the LLM for code review.
+
+options:
+  -h, --help            show this help message and exit
+  --fail_under {A,B,C,D}
+                        If specified, exit with non-zero status if the LLM's grade falls below the given value. This value is not inclusive: if this value is "B" and the LLM gives a final grade of "B," then the program will exit with a zero status. If not specified, then the program will exit with a zero status no matter the LLM's grade.
+```
+
 ## Example output
 
 You can try Backseat Driver on the input program below to see how it works.
-Copy the code below into a file and run Backseat Driver with the following.
-
-TODO show python command to reproduce this output
+Copy the code into `test.py`.
 
 ```python
 """A file for testing prompt creation."""
 
 
 def fib(n):
     """Returns the nth fibonacci number."""
@@ -94,14 +134,20 @@
         return [n]
     if n % 2 == 0:
         return [n] + hailstone(n // 2)
     return [n] + hailstone(3 * n + 1)
 
 ```
 
+Run Backseat Driver with the following.
+
+```shell
+backseat-driver test.py
+```
+
 What Backseat Driver says:
 
 > Grade: A
 > 
 > This code is well-written, easy to read, and well-organized. The function names are clear and descriptive, and the docstrings provide useful information about the functions' purpose and behavior. The code also follows the recommended Python style guidelines (PEP 8), including appropriate indentation, whitespace, and naming conventions. Overall, there are no major issues with the code, and it is highly readable and maintainable.
 > 
 > One possible improvement could be to add some error handling to the `fib()` and `fact()` functions, for cases where the input is not a positive integer. Another potential improvement could be to add some more comments to explain the logic behind the `hailstone()` function. However, these are minor suggestions and are not necessary for the code to function correctly.
```

### Comparing `backseat-driver-0.0.1/setup.cfg` & `backseat-driver-0.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `backseat-driver-0.0.1/tests/test_backseat_driver.py` & `backseat-driver-0.0.2/tests/test_backseat_driver.py`

 * *Files identical despite different names*

