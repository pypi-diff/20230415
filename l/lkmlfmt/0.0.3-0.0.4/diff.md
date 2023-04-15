# Comparing `tmp/lkmlfmt-0.0.3.tar.gz` & `tmp/lkmlfmt-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lkmlfmt-0.0.3.tar", max compression
+gzip compressed data, was "lkmlfmt-0.0.4.tar", max compression
```

## Comparing `lkmlfmt-0.0.3.tar` & `lkmlfmt-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     2518 2023-04-12 15:53:19.500161 lkmlfmt-0.0.3/README.md
--rw-r--r--   0        0        0       53 2023-04-12 15:53:19.500161 lkmlfmt-0.0.3/lkmlfmt/__init__.py
--rw-r--r--   0        0        0       70 2023-04-12 15:53:19.500161 lkmlfmt-0.0.3/lkmlfmt/__main__.py
--rw-r--r--   0        0        0     2391 2023-04-12 15:53:19.500161 lkmlfmt-0.0.3/lkmlfmt/command.py
--rw-r--r--   0        0        0      100 2023-04-12 15:53:19.500161 lkmlfmt-0.0.3/lkmlfmt/exception.py
--rw-r--r--   0        0        0     9409 2023-04-12 15:53:19.500161 lkmlfmt-0.0.3/lkmlfmt/formatter.py
--rw-r--r--   0        0        0      754 2023-04-12 15:53:19.500161 lkmlfmt-0.0.3/lkmlfmt/lkml.lark
--rw-r--r--   0        0        0       64 2023-04-12 15:53:19.500161 lkmlfmt-0.0.3/lkmlfmt/logger.py
--rw-r--r--   0        0        0     2292 2023-04-12 15:53:19.500161 lkmlfmt-0.0.3/lkmlfmt/parser.py
--rw-r--r--   0        0        0     5028 2023-04-12 15:53:19.504161 lkmlfmt-0.0.3/lkmlfmt/template.py
--rw-r--r--   0        0        0      552 2023-04-12 15:53:19.504161 lkmlfmt-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2962 1970-01-01 00:00:00.000000 lkmlfmt-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     2647 2023-04-15 14:03:39.198916 lkmlfmt-0.0.4/README.md
+-rw-r--r--   0        0        0       53 2023-04-15 14:03:39.198916 lkmlfmt-0.0.4/lkmlfmt/__init__.py
+-rw-r--r--   0        0        0       70 2023-04-15 14:03:39.198916 lkmlfmt-0.0.4/lkmlfmt/__main__.py
+-rw-r--r--   0        0        0     2391 2023-04-15 14:03:39.198916 lkmlfmt-0.0.4/lkmlfmt/command.py
+-rw-r--r--   0        0        0      100 2023-04-15 14:03:39.198916 lkmlfmt-0.0.4/lkmlfmt/exception.py
+-rw-r--r--   0        0        0    10847 2023-04-15 14:03:39.198916 lkmlfmt-0.0.4/lkmlfmt/formatter.py
+-rw-r--r--   0        0        0      757 2023-04-15 14:03:39.198916 lkmlfmt-0.0.4/lkmlfmt/lkml.lark
+-rw-r--r--   0        0        0       64 2023-04-15 14:03:39.198916 lkmlfmt-0.0.4/lkmlfmt/logger.py
+-rw-r--r--   0        0        0     2292 2023-04-15 14:03:39.198916 lkmlfmt-0.0.4/lkmlfmt/parser.py
+-rw-r--r--   0        0        0     4802 2023-04-15 14:03:39.198916 lkmlfmt-0.0.4/lkmlfmt/template.py
+-rw-r--r--   0        0        0      552 2023-04-15 14:03:39.198916 lkmlfmt-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3091 1970-01-01 00:00:00.000000 lkmlfmt-0.0.4/PKG-INFO
```

### Comparing `lkmlfmt-0.0.3/README.md` & `lkmlfmt-0.0.4/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -27,17 +27,17 @@
       where ts between current_date()-7 and current_date())
     select column_name from cte
     ;;
   }
   dimension: column_name {
     html:
 {% if value == "foo" %}
-<img src="https://example.com/{{ value }}"/>
+<img src="https://example.com/foo"/>
 {% else %}
-<img src="https://example.com/{{ value }}"/>
+<img src="https://example.com/bar"/>
 {% endif %} ;;
   }
 }
 """)
 
 assert lkml == """\
 view: view_name {
@@ -52,17 +52,17 @@
       select column_name
       from cte
     ;;
   }
   dimension: column_name {
     html:
       {% if value == "foo" %}
-        <img src="https://example.com/{{ value }}"/>
+        <img src="https://example.com/foo"/>
       {% else %}
-        <img src="https://example.com/{{ value }}"/>
+        <img src="https://example.com/bar"/>
       {% endif %}
     ;;
   }
 }
 """
 ```
 
@@ -110,7 +110,13 @@
         with:
           branch: format/${{ github.ref_name }}
 ```
 
 ## Feedback
 I'm not ready to accept pull requests, but your feedback is always welcome.
 If you find any bugs, please feel free to create an issue.
+
+## See also
+lkmlfmt depends on these awesome formatter and indenter.
+
+* [sqlfmt](https://github.com/tconbeer/sqlfmt)
+* [djhtml](https://github.com/rtts/djhtml)
```

### Comparing `lkmlfmt-0.0.3/lkmlfmt/command.py` & `lkmlfmt-0.0.4/lkmlfmt/command.py`

 * *Files identical despite different names*

### Comparing `lkmlfmt-0.0.3/lkmlfmt/formatter.py` & `lkmlfmt-0.0.4/lkmlfmt/formatter.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,14 +11,17 @@
 from lkmlfmt import parser, template
 from lkmlfmt.exception import LkmlfmtException
 from lkmlfmt.logger import logger
 
 COMMENT_MARKER = "#LKMLFMT_MARKER#"
 COMMENT = re.compile(rf"{COMMENT_MARKER}")
 BLANK_LINE = re.compile(r"^\s*$")
+ESCAPED_STRING_SINGLE = re.compile(r'"(?P<inner>(.|\n)*?(?<!\\)(\\\\)*?)"')
+ESCAPED_STRING_TRIPLE = re.compile(r'"""(?P<inner>(.|\n)*?(?<!\\)(\\\\)*?)"""')
+NOT_AND_OR = re.compile(r"(?<!\w)(not|and|or)(?!\w)")
 INDENT_WIDTH = 2
 MODE = api.Mode()
 
 
 class LkmlFormatter:
     def __init__(self, lkml: str) -> None:
         self.lkml = lkml
@@ -76,15 +79,15 @@
 {self.fmt_indent()}]"""
 
     def fmt_code_pair(self, pair: ParseTree) -> str:
         lcomments = self.fmt_leading_comments_of(_token(pair.children[0]))
         key = self.fmt(pair.children[0]).lstrip()
         value = str(pair.children[1])
 
-        if key == "html":
+        if key.startswith("html"):
             with self.indent():
                 indent = self.curr_indent
                 f: Any = (
                     lambda s, w: " " * (w * (s.level + indent) + s.offset) + t
                     if (t := s.text.strip())
                     else t
                 )
@@ -101,19 +104,25 @@
 
         # sql_xxx: ... ;; or expression_xxx: ... ;;
         with self.indent():
             # https://docs.python.org/3/library/functions.html#property
             Line.prefix = property(  # type: ignore
                 lambda s: " " * INDENT_WIDTH * (s.depth[0] + self.curr_indent)
             )
-            value = _fmt_sql(value)
+            if key.startswith("sql"):
+                value = _fmt_sql(value)
+            else:
+                value = _fmt_expr(value)
 
         if "\n" not in value:
             return f"{lcomments}{self.fmt_indent()}{key}: {value.lstrip()} ;;"
 
+        if not value.startswith(" "):  # fallback if sqlfmt does not support
+            value = " " * ((self.curr_indent + 1) * INDENT_WIDTH) + value
+
         return f"""{lcomments}{self.fmt_indent()}{key}:
 {value}
 {self.fmt_indent()};;"""
 
     def fmt_dict(self, dict_: ParseTree) -> str:
         with self.indent():
             pairs = self.fmt(dict_.children)
@@ -272,23 +281,52 @@
 
 def _token(token: Token | ParseTree) -> Token:
     if isinstance(token, Token):
         return token
     raise LkmlfmtException()
 
 
-def _fmt_html(html: str) -> str:
-    formatted: str = DjHTML(html).indent(2)
-    return formatted
+def _fmt_html(liquid: str) -> str:
+    jinja, templates, dummies = template.to_jinja(liquid, "djhtml")
+    jinja = DjHTML(jinja).indent(2)
+    liquid = template.to_liquid_djhtml(jinja, templates, dummies)
+    return liquid
 
 
 def _fmt_sql(liquid: str) -> str:
-    jinja, templates, *_ = template.to_jinja(liquid)
-    # NOTE let's rely on sqlfmt for not only sql but also looker expression!
+    jinja, templates, dummies = template.to_jinja(liquid, "sqlfmt")
     jinja = api.format_string(jinja, mode=MODE).rstrip()
-    liquid = template.to_liquid(jinja, templates, [])
+    liquid = template.to_liquid_sqlfmt(jinja, templates, dummies)
     return liquid
 
 
+# NOTE let's rely on sqlfmt for not only sql but also looker expression!
+def _fmt_expr(liquid: str) -> str:
+    # convert looker expr into sql
+    temp = liquid
+    temp = temp.replace("case", "lkmlfmt_case")
+    temp = temp.replace("when", "lkmlfmt_when")
+    temp = ESCAPED_STRING_SINGLE.sub(r'"""\g<inner>"""', temp)  # " -> """
+
+    temp = _fmt_sql(temp)
+
+    # convert sql into looker expression
+    temp = ESCAPED_STRING_TRIPLE.sub(r'"\g<inner>"', temp)
+    temp = temp.replace("lkmlfmt_when", "when")
+    temp = temp.replace("lkmlfmt_case", "case")
+
+    splited = ESCAPED_STRING_SINGLE.split(temp)
+    expr = ""
+    for i, s in enumerate(splited):
+        match divmod(i, 4)[1]:  # mod
+            case 0:
+                uppered = NOT_AND_OR.sub(lambda x: x.group(0).upper(), s)
+                expr += uppered
+            case 1:
+                expr += f'"{s}"'
+
+    return expr
+
+
 def fmt(lkml: str) -> str:
     formatter = LkmlFormatter(lkml)
     return formatter.fmt()
```

### Comparing `lkmlfmt-0.0.3/lkmlfmt/lkml.lark` & `lkmlfmt-0.0.4/lkmlfmt/lkml.lark`

 * *Files 19% similar despite different names*

```diff
@@ -13,15 +13,15 @@
       | IDENT
 CNAME: DIGIT* ("_"|LETTER) ("_"|LETTER|DIGIT)*
 IDENT: [/(\+|-)\s*/] CNAME (/\s*\.\s*/ CNAME)* [/\s*?\*/]
 COMMENT: /#.*/
 // \S is needed cause 0 width regexp is not allowed here
 CODEBLOCK: /\S(.|\n)*?(?=\s*;;)/
 // higher priority than IDENT
-CODEBLOCKKEY.1: /expression\w*/ | "html" | /sql\w*/
+CODEBLOCKKEY.1: /expression\w*/ | /html\w*/ | /sql\w*/
 STRING : "\"" /(.|\n)*?/ /(?<!\\)(\\\\)*?/ "\""
 
 %import common.DIGIT
 %import common.LETTER
 %import common.NUMBER
 %import common.WS
 %ignore WS
```

### Comparing `lkmlfmt-0.0.3/lkmlfmt/parser.py` & `lkmlfmt-0.0.4/lkmlfmt/parser.py`

 * *Files identical despite different names*

### Comparing `lkmlfmt-0.0.3/lkmlfmt/template.py` & `lkmlfmt-0.0.4/lkmlfmt/template.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 import re
 from typing import Literal
 
-from lkmlfmt.exception import LkmlfmtException
-
 LIQUID_MARKER = "{{% set LKMLFMT_MARKER = {} %}}"
 TEMPLATE = re.compile(
     r"""(?P<tag>\{%-?\s*(?P<type>#|([a-z]*))([^"'}]*|'[^']*?'|"[^"]*?")*?-?%\})"""
     + r"""|(?P<obj>\{\{([^"'}]*|'[^']*?'|"[^"]*?")*?\}\})"""
     + r"""|(?P<looker>\$\{[^}]*?\})""",
 )
 DUMMY = re.compile(r"^(?P<lead_n> *?\n)?(?P<indent> *)")
@@ -58,18 +56,18 @@
                 dummy = "{{ var }}"
             case "tablerow":
                 dummy = "{% for i in [] %}"
             case "endtablerow":
                 dummy = "{% endfor %}"
             # template https://shopify.github.io/liquid/tags/template/
             case "comment":
-                dummy = "{% if False %}{% raw %}"
+                dummy = "{% raw %}"
                 skip_to = "endcomment"
             case "endcomment":
-                dummy = "{% endraw %}{% endif %}"
+                dummy = "{% endraw %}"
             case "#":
                 dummy = "{% set x = 'x' %}"
             case "liquid":
                 dummy = "{% set x = 'x' %}"
             case "echo":
                 dummy = "{{ var }}"
             case "raw":
@@ -104,45 +102,40 @@
             # default
             case _:
                 dummy = f"{{% {type_} %}}"
 
         # append results
         marker = LIQUID_MARKER.format(id_)
         if mode == "sqlfmt":
-            jinja += f"{liquid[: match.start()]}{marker}{dummy}{marker}"
+            jinja += f"{liquid[: match.start()]}{marker}{dummy}"
         else:
             jinja += f"{liquid[: match.start()]}{dummy}{marker}"
 
         templates.append(match.group(0))
         dummies.append(dummy)
 
         # prepare for next iteration
         liquid = liquid[match.end() :]
         id_ += 1
 
     return jinja, templates, dummies
 
 
-def to_liquid(
-    jinja: str, templates: list[str], dummies: list[str], mode: MODE = "sqlfmt"
-) -> str:
-    if mode == "djhtml":
-        return to_liquid_djhtml(jinja, templates, dummies)
-
-    for i, template in enumerate(templates):
-        leading, dummy, trailing, *_ = jinja.split(LIQUID_MARKER.format(i))
-        match = DUMMY.match(dummy)
-        if match is None:
-            raise LkmlfmtException()
+def to_liquid_sqlfmt(jinja: str, templates: list[str], dummies: list[str]) -> str:
+    for i in range(len(templates)):
+        leading, trailing, *_ = jinja.split(LIQUID_MARKER.format(i))
+        space, *_ = trailing.split(dummies[i])
+        if "\n" in space:
+            leading = leading.rstrip("\n ")
+        else:
+            trailing = trailing.lstrip(" ")
 
-        if match.group("lead_n") is not None:
-            leading = leading.rstrip("\n ") + "\n"
-            template = match.group("indent") + template
+        trailing = trailing.replace(dummies[i], templates[i], 1)
+        jinja = leading + trailing
 
-        jinja = leading + template + trailing
     return jinja
 
 
 def to_liquid_djhtml(jinja: str, templates: list[str], dummies: list[str]) -> str:
     liquid = ""
     trailing = ""
```

### Comparing `lkmlfmt-0.0.3/pyproject.toml` & `lkmlfmt-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lkmlfmt"
-version = "0.0.3"
+version = "0.0.4"
 description = ""
 authors = ["dr666m1 <skndr666m1@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 lkmlfmt = "lkmlfmt.command:run"
```

### Comparing `lkmlfmt-0.0.3/PKG-INFO` & `lkmlfmt-0.0.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lkmlfmt
-Version: 0.0.3
+Version: 0.0.4
 Summary: 
 Author: dr666m1
 Author-email: skndr666m1@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
@@ -42,17 +42,17 @@
       where ts between current_date()-7 and current_date())
     select column_name from cte
     ;;
   }
   dimension: column_name {
     html:
 {% if value == "foo" %}
-<img src="https://example.com/{{ value }}"/>
+<img src="https://example.com/foo"/>
 {% else %}
-<img src="https://example.com/{{ value }}"/>
+<img src="https://example.com/bar"/>
 {% endif %} ;;
   }
 }
 """)
 
 assert lkml == """\
 view: view_name {
@@ -67,17 +67,17 @@
       select column_name
       from cte
     ;;
   }
   dimension: column_name {
     html:
       {% if value == "foo" %}
-        <img src="https://example.com/{{ value }}"/>
+        <img src="https://example.com/foo"/>
       {% else %}
-        <img src="https://example.com/{{ value }}"/>
+        <img src="https://example.com/bar"/>
       {% endif %}
     ;;
   }
 }
 """
 ```
 
@@ -126,7 +126,13 @@
           branch: format/${{ github.ref_name }}
 ```
 
 ## Feedback
 I'm not ready to accept pull requests, but your feedback is always welcome.
 If you find any bugs, please feel free to create an issue.
 
+## See also
+lkmlfmt depends on these awesome formatter and indenter.
+
+* [sqlfmt](https://github.com/tconbeer/sqlfmt)
+* [djhtml](https://github.com/rtts/djhtml)
+
```

