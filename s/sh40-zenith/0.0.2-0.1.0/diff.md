# Comparing `tmp/sh40_zenith-0.0.2.tar.gz` & `tmp/sh40_zenith-0.1.0.tar.gz`

## Comparing `sh40_zenith-0.0.2.tar` & `sh40_zenith-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,21 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sh40_zenith-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 sh40_zenith-0.0.2/tests/test_color.py
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 sh40_zenith-0.0.2/tests/test_lru_cache.py
--rw-r--r--   0        0        0     5287 2020-02-02 00:00:00.000000 sh40_zenith-0.0.2/tests/test_markup.py
--rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 sh40_zenith-0.0.2/tests/test_palette.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 sh40_zenith-0.0.2/zenith/__about__.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 sh40_zenith-0.0.2/zenith/__init__.py
--rw-r--r--   0        0        0     8247 2020-02-02 00:00:00.000000 sh40_zenith-0.0.2/zenith/color.py
--rw-r--r--   0        0        0     9330 2020-02-02 00:00:00.000000 sh40_zenith-0.0.2/zenith/color_info.py
--rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 sh40_zenith-0.0.2/zenith/lru_cache.py
--rw-r--r--   0        0        0    11761 2020-02-02 00:00:00.000000 sh40_zenith-0.0.2/zenith/markup.py
--rw-r--r--   0        0        0     7159 2020-02-02 00:00:00.000000 sh40_zenith-0.0.2/zenith/palette.py
--rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 sh40_zenith-0.0.2/.gitignore
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 sh40_zenith-0.0.2/LICENSE.txt
--rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 sh40_zenith-0.0.2/README.md
--rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 sh40_zenith-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 sh40_zenith-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sh40_zenith-0.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     5049 2020-02-02 00:00:00.000000 sh40_zenith-0.1.0/tests/dont_test_markup.py
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 sh40_zenith-0.1.0/tests/test_color.py
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 sh40_zenith-0.1.0/tests/test_lru_cache.py
+-rw-r--r--   0        0        0     4229 2020-02-02 00:00:00.000000 sh40_zenith-0.1.0/tests/test_markup.py
+-rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 sh40_zenith-0.1.0/tests/test_palette.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 sh40_zenith-0.1.0/zenith/__about__.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 sh40_zenith-0.1.0/zenith/__init__.py
+-rw-r--r--   0        0        0     8247 2020-02-02 00:00:00.000000 sh40_zenith-0.1.0/zenith/color.py
+-rw-r--r--   0        0        0     9500 2020-02-02 00:00:00.000000 sh40_zenith-0.1.0/zenith/color_info.py
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 sh40_zenith-0.1.0/zenith/exceptions.py
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 sh40_zenith-0.1.0/zenith/lru_cache.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sh40_zenith-0.1.0/zenith/macros.py
+-rw-r--r--   0        0        0    12503 2020-02-02 00:00:00.000000 sh40_zenith-0.1.0/zenith/markup.old.py
+-rw-r--r--   0        0        0    10714 2020-02-02 00:00:00.000000 sh40_zenith-0.1.0/zenith/markup.py
+-rw-r--r--   0        0        0     7166 2020-02-02 00:00:00.000000 sh40_zenith-0.1.0/zenith/palette.py
+-rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 sh40_zenith-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 sh40_zenith-0.1.0/LICENSE.txt
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 sh40_zenith-0.1.0/README.md
+-rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 sh40_zenith-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2287 2020-02-02 00:00:00.000000 sh40_zenith-0.1.0/PKG-INFO
```

### Comparing `sh40_zenith-0.0.2/tests/test_color.py` & `sh40_zenith-0.1.0/tests/test_color.py`

 * *Files identical despite different names*

### Comparing `sh40_zenith-0.0.2/tests/test_markup.py` & `sh40_zenith-0.1.0/tests/dont_test_markup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,174 +1,170 @@
 import pytest
 from slate import Span
 
-from zenith.markup import alias, define, markup, markup_spans
+from zenith.markup import (
+    zml,
+    zml_get_spans,
+    zml_alias,
+    zml_macro,
+    zml_pre_process,
+    GLOBAL_CONTEXT,
+)
 
 
 def test_markup_str_parse():
-    def _upper(text: str) -> str:
+    @zml_macro
+    def upper(text: str) -> str:
         return text.upper()
 
-    define("!upper", _upper)
-
     assert (
-        markup("[bold underline 61]Hello [141 /bold]There")
+        zml("[bold underline 61]Hello [141 /bold]There")
         == "\x1b[38;5;61;1;4mHello \x1b[22m\x1b[38;5;141mThere\x1b[0m"
     )
 
-    assert markup("[38]Hello [!upper]There") == "\x1b[38;5;38mHello THERE\x1b[0m"
+    assert zml("[38]Hello [!upper]There") == "\x1b[38;5;38mHello THERE\x1b[0m"
 
-    assert markup(
+    assert zml(
         "Click [141 underline ~https://google.com]me[61] and me[/~ / bold red] NOW"
     ) == (
         "Click \x1b]8;;https://google.com\x1b\\\x1b[38;5;141;4mme"
         + "\x1b]8;;https://google.com\x1b\\\x1b[38;5;61m and me\x1b[0m"
         + "\x1b]8;;\x1b\\\x1b[38;2;255;0;0;1m NOW\x1b[0m"
     )
 
-    assert markup("The never-ending [~https://google.com]URI") == (
+    assert zml("The never-ending [~https://google.com]URI") == (
         "The never-ending \x1b]8;;https://google.com\x1b\\URI\x1b]8;;\x1b\\"
-    ), repr(markup("The never-ending [~https://google.com]URI"))
+    ), repr(zml("The never-ending [~https://google.com]URI"))
 
-    assert markup("[blue][@red]This is hard to parse") == (
+    assert zml("[blue][@red]This is hard to parse") == (
         "\x1b[38;2;0;0;255;48;2;255;0;0mThis is hard to parse\x1b[0m"
     )
 
 
 def test_markup_parse():
-    assert list(markup_spans("[bold italic]Hello")) == [
+    assert list(zml_get_spans("[bold italic]Hello")) == [
         Span("Hello", bold=True, italic=True),
     ]
 
-    assert list(markup_spans("[bold italic]Hello[/bold]Not bold")) == [
+    assert list(zml_get_spans("[bold italic]Hello[/bold]Not bold")) == [
         Span("Hello", bold=True, italic=True),
         Span("Not bold", italic=True),
     ]
 
 
 def test_markup_color():
     # 0-7 indexed colors
-    assert list(markup_spans("[@0 1]Test[@1 0]Other")) == [
+    assert list(zml_get_spans("[@0 1]Test[@1 0]Other")) == [
         Span("Test", background="40", foreground="31"),
         Span("Other", background="41", foreground="30"),
     ]
 
     # 8-15 indexed colors
-    assert list(markup_spans("[@9 15]Test[@14 10]Other")) == [
+    assert list(zml_get_spans("[@9 15]Test[@14 10]Other")) == [
         Span("Test", background="101", foreground="97"),
         Span("Other", background="106", foreground="92"),
     ]
 
     # 16-256 indexed colors
-    assert list(markup_spans("[@141 61]Test[@54 78]Other")) == [
+    assert list(zml_get_spans("[@141 61]Test[@54 78]Other")) == [
         Span("Test", background="48;5;141", foreground="38;5;61"),
         Span("Other", background="48;5;54", foreground="38;5;78"),
     ]
 
     # OOB indexed color
     with pytest.raises(ValueError):
-        list(markup_spans("[@333 231]Please don't parse..."))
+        list(zml_get_spans("[@333 231]Please don't parse..."))
 
     # CSS colors
-    assert list(markup_spans("[@lavender cadetblue]Pretty colors")) == [
+    assert list(zml_get_spans("[@lavender cadetblue]Pretty colors")) == [
         Span(
             "Pretty colors", foreground="38;2;95;158;160", background="48;2;230;230;250"
         )
     ]
 
     # HEX colors
-    assert list(markup_spans("[@#212121 #dedede]Nice contrast")) == [
+    assert list(zml_get_spans("[@#212121 #dedede]Nice contrast")) == [
         Span("Nice contrast", foreground="38;2;222;222;222", background="48;2;33;33;33")
     ]
 
     # RGB colors
-    assert list(markup_spans("[@11;22;123 123;22;11]What even are these colors")) == [
+    assert list(zml_get_spans("[@11;22;123 123;22;11]What even are these colors")) == [
         Span(
             "What even are these colors",
             foreground="38;2;123;22;11",
             background="48;2;11;22;123",
         )
     ]
 
 
 def test_markup_auto_foreground():
-    assert list(markup_spans("[@#FFFFFF]test")) == [
+    assert list(zml_get_spans("[@#FFFFFF]test")) == [
         Span("test", background="48;2;255;255;255", foreground="38;2;35;35;35")
     ]
 
-    assert list(markup_spans("[@0]White[@7]Black[@160]White[@116]Black")) == [
+    assert list(zml_get_spans("[@0]White[@7]Black[@160]White[@116]Black")) == [
         Span("White", background="40", foreground="38;2;245;245;245"),
         Span("Black", background="47", foreground="38;2;35;35;35"),
         Span("White", background="48;5;160", foreground="38;2;245;245;245"),
         Span("Black", background="48;5;116", foreground="38;2;35;35;35"),
     ]
 
 
 def test_markup_macros():
-    def _upper(text: str) -> str:
+    @zml_macro
+    def upper(text: str) -> str:
         return text.upper()
 
-    def _conceal(text: str) -> str:
+    @zml_macro
+    def conceal(text: str) -> str:
         return "*" * (len(text) - 1) + text[-1]
 
-    define("!upper", _upper)
-    define("!conceal", _conceal)
-
-    assert list(
-        markup_spans("[!upper 141]Test[/!upper /fg !conceal bold]other test")
-    ) == [
-        Span("TEST", foreground="38;5;141"),
-        Span("*********t", bold=True),
-    ]
+    assert (
+        zml_pre_process("[!upper 141]Test[/!upper /fg !conceal bold]other test")
+        == "[141]TEST[/fg bold]*********t"
+    )
 
     with pytest.raises(ValueError):
-        list(markup_spans("[!undefined]Test"))
+        zml_pre_process("[!undefined]Test")
 
     with pytest.raises(ValueError):
-        list(markup_spans("[undefined]Test"))
+        zml_pre_process("[undefined]Test")
 
     with pytest.raises(ValueError):
-        list(markup_spans("[/!upper]Test"))
+        zml_pre_process("[/!upper]Test")
 
 
 def test_markup_aliases():
-    alias(a="b", test="141 bold")
+    zml_alias(a="b", test="141 bold")
 
-    assert list(markup_spans("[test italic]What is this?")) == [
-        Span("What is this?", italic=True, bold=True, foreground="38;5;141")
-    ]
+    assert zml_pre_process("[test italic]What is this?") == (
+        "[141 bold italic]What is this?"
+    )
 
-    def _upper(text: str) -> str:
+    @zml_macro
+    def upper(text: str) -> str:
         return text.upper()
 
-    define("!upper", _upper)
-
-    alias(complex_with_macro="!upper lavender")
+    zml_alias(complex_with_macro="!upper lavender")
 
-    assert list(markup_spans("[complex-with-macro]test")) == [
-        Span("TEST", foreground="38;2;230;230;250")
-    ]
+    assert zml_pre_process("[complex-with-macro]test") == "[lavender]TEST"
 
-    alias(complex_with_hyperlink="~https://google.com underline slategray")
+    zml_alias(complex_with_hyperlink="~https://google.com underline slategray")
 
-    assert list(markup_spans("[complex-with-hyperlink]test")) == [
-        Span(
-            "test",
-            underline=True,
-            hyperlink="https://google.com",
-            foreground="38;2;112;128;144",
-        )
-    ]
+    assert (
+        zml_pre_process("[complex-with-hyperlink]test")
+        == "[~https://google.com underline slategray]test"
+    )
 
 
 def test_markup_hyperlink():
     assert list(
-        markup_spans("[~https://google.com]Test [bold]me [/~]no more link")
+        zml_get_spans("[~https://google.com]Test [bold]me [/~]no more link")
     ) == [
         Span("Test ", hyperlink="https://google.com"),
         Span("me ", bold=True, hyperlink="https://google.com"),
         Span("no more link", bold=True),
     ]
 
 
 def test_markup_parse_plain():
-    assert list(markup_spans("Test")) == [Span("Test")]
+    assert list(zml_get_spans("Test")) == [Span("Test")]
```

### Comparing `sh40_zenith-0.0.2/tests/test_palette.py` & `sh40_zenith-0.1.0/tests/test_palette.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from zenith.color import Color
-from zenith.markup import ContextMapping
+from zenith.markup import zml_context
 from zenith.palette import Palette, analogous, tetradic, triadic
 
 
 def test_palette_triadic():
     pal = Palette.from_hex("#FABCDE", strategy=triadic)
 
     assert pal.primary == Color.from_hex("#FABCDE")
@@ -28,15 +28,15 @@
     assert pal.secondary == pal.primary.hue_shift(1 / 4)
     assert pal.tertiary == pal.primary.hue_shift(2 / 4)
     assert pal.quaternary == pal.primary.hue_shift(3 / 4)
 
 
 def test_palette_alias():
     pal = Palette.from_hex("#42DFBC")
-    ctx = ContextMapping.new()
+    ctx = zml_context()
 
     pal.alias(ctx=ctx)
 
     assert ctx["aliases"]["error-2"] == pal.error.darken(2).hex
     assert ctx["aliases"]["surface3"] == pal.surface3.hex
     assert ctx["aliases"]["success+3"] == pal.success.lighten(3).hex
```

### Comparing `sh40_zenith-0.0.2/zenith/color.py` & `sh40_zenith-0.1.0/zenith/color.py`

 * *Files identical despite different names*

### Comparing `sh40_zenith-0.0.2/zenith/color_info.py` & `sh40_zenith-0.1.0/zenith/color_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -410,7 +410,17 @@
     "violet": "#ee82ee",
     "wheat": "#f5deb3",
     "white": "#ffffff",
     "whitesmoke": "#f5f5f5",
     "yellow": "#ffff00",
     "yellowgreen": "#9acd32",
 }
+
+NAMED_COLORS = {
+    **CSS_COLORS,
+    **{
+        "slate": "#717e8d",
+        "zenith": "#4a7a9f",
+        "celadon": "#afe1af",
+        "carmine": "#d70040",
+    },
+}
```

### Comparing `sh40_zenith-0.0.2/zenith/lru_cache.py` & `sh40_zenith-0.1.0/zenith/lru_cache.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,21 +4,23 @@
 and adding support (through another decorator) is messy and impossible to read.
 """
 
 from __future__ import annotations
 
 from collections import OrderedDict
 from dataclasses import dataclass, field
-from typing import Hashable
+from typing import Generic, Hashable, TypeVar
 
 __all__ = ["LRUCache"]
 
+CacheItemType = TypeVar("CacheItem")
+
 
 @dataclass
-class LRUCache:
+class LRUCache(Generic[CacheItemType]):
     """A Least-Recently-Used cache.
 
     Usage:
 
     ```python3
     cache = LRUCache(1024)
 
@@ -34,25 +36,32 @@
         cache[key] = result
 
         return result
     ```
     """
 
     _capacity: int
-    _cache: OrderedDict[Hashable, str] = field(init=False, default_factory=OrderedDict)
+    _cache: OrderedDict[Hashable, CacheItemType] = field(
+        init=False, default_factory=OrderedDict
+    )
 
     def __contains__(self, key: Hashable) -> bool:
         return key in self._cache
 
-    def __getitem__(self, key: Hashable) -> str:
+    def __getitem__(self, key: Hashable) -> CacheItemType:
         if key not in self._cache:
             raise KeyError(f"Key {key!r} not found in cache.")
 
         self._cache.move_to_end(key)
         return self._cache[key]
 
-    def __setitem__(self, key: Hashable, value: str) -> None:
+    def __setitem__(self, key: Hashable, value: CacheItemType) -> None:
         self._cache[key] = value
         self._cache.move_to_end(key)
 
         if len(self._cache) > self._capacity:
             self._cache.popitem(last=False)
+
+    def get(
+        self, key: Hashable, default: CacheItemType | None = None
+    ) -> CacheItemType | None:
+        return self._cache.get(key, default)
```

### Comparing `sh40_zenith-0.0.2/zenith/markup.py` & `sh40_zenith-0.1.0/zenith/markup.old.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 
 from .color import Color
 from .color_info import CSS_COLORS
 from .lru_cache import LRUCache
 
 __all__ = [
     "alias",
-    "define",
+    "get_macro_definition",
+    "macro",
     "FULL_RESET",
     "parse_spans",
     "markup",
     "ContextMapping",
     "GLOBAL_CONTEXT",
 ]
 
@@ -105,34 +106,26 @@
 
     for key, value in aliases.items():
         key = key if keep_case else key.replace("_", "-")
 
         ctx_aliases[key] = value
 
 
-def define(
-    identifier: str, value: Callable[[str], str], ctx: ContextMapping | None = None
-) -> None:
-    """Defines a markup macro within the given context.
+MacroType = Callable[[str], str]
 
-    Args:
-        identifier: The name the macro can be referenced by. Must start with '!'.
-        value: The callback that is executed by the macro. This takes the partially
-            parsed output at the moment the macro is found, and returns some
-            modification of it.
-        ctx: The context to alias within. Defaults to the global context.
-    """
 
-    if not identifier.startswith("!"):
-        raise ValueError(
-            "Macro identifiers must start with `!`, {identifier!r} doesn't."
-        )
+def get_macro_definition(*, ctx: ContextMapping) -> Callable[[MacroType], MacroType]:
+    def _def_macro(func: Callable[[str], str]) -> None:
+        identifier = func.__name__.replace("_", "-")
+        ctx["macros"][f"!{identifier}"] = func
 
-    ctx = ctx or GLOBAL_CONTEXT
-    ctx["macros"][identifier] = value
+    return _def_macro
+
+
+macro = get_macro_definition(ctx=GLOBAL_CONTEXT)
 
 
 def _parse_color(color: str) -> str:
     background = color.startswith("@") * 10
     color = color.lstrip("@")
 
     if color.isdigit():
@@ -204,15 +197,15 @@
         ),
         prefix,
     )
 
 
 def markup_spans(
     text: str, ctx: ContextMapping | None = None, prefix: str = ""
-) -> Generator[Span, None, None]:
+) -> tuple[Span, ...]:
     """Generates Span objects representative of the markup text given.
 
     Aliases are evaluated first, followed by macros. After that, the resulting markup is
     parsed.
 
     Args:
         text: Some markup string.
@@ -233,20 +226,17 @@
             return "@" + prefix + key[1:]
 
         return prefix + key
 
     ctx = ctx or GLOBAL_CONTEXT
 
     style_stack = cast("dict[str, str | bool]", BASE_STYLE_STACK.copy())
-    macros: list[Callable[[str], str]] = []
-
-    get_macro = ctx["macros"].get
     get_alias = ctx["aliases"].get
 
-    text = text.replace("][", " ")
+    text = _expand_macros(text.replace("][", " "), ctx=ctx)
 
     def _apply_tag(tag: str) -> None:
         """Parses and applies the given tag to the style stack.
 
         Args:
             tag: The markup tag to apply.
         """
@@ -270,76 +260,127 @@
 
         # Colors
         if RE_COLOR.match(tag) or tag.lstrip("@") in CSS_COLORS:
             layer = "background" if tag.startswith("@") else "foreground"
             style_stack[layer] = _parse_color(tag)
             return
 
-        # Macros
-        if tag.startswith("!"):
-            macro = get_macro(_add_prefix(tag), None)
-
-            if macro is None:
-                raise ValueError(f"Undefined macro {tag!r}.")
-
-            if not is_setter:
-                try:
-                    macros.remove(macro)
-                except ValueError:
-                    raise ValueError(
-                        f"Macro {tag!r} is not set, so it can't be unset."
-                    ) from None
-
-                return
-
-            macros.append(macro)
-            return
-
         # Hyperlinks
         if tag.startswith("~"):
             style_stack["hyperlink"] = "" if not is_setter else tag.lstrip("~")
             return
 
         # Aliases
         found_alias = get_alias(_add_prefix(tag))
 
         if found_alias is None:
             raise ValueError(f"Unknown tag {tag!r}.")
 
         for part in found_alias.split():
             _apply_tag(part)
 
+    spans = []
+
     for mtch in RE_MARKUP.finditer(text):
         tags, plain = mtch.groups()
 
         if tags is None:
             if plain is None:
                 continue
 
             tags = ""
 
         plain = plain or ""
 
         for tag in tags.split():
             if tag == "/":
-                yield FULL_RESET
+                spans.append(FULL_RESET)
 
             _apply_tag(tag)
 
-        # TODO: Yield macros to consumer to allow smartly caching things.
-        for macro in macros:
-            plain = macro(plain)
-
         should_delete_foreground = _apply_auto_foreground(style_stack)
 
-        yield Span(plain, **style_stack)
+        spans.append(Span(plain, **style_stack))
 
         if should_delete_foreground:
             del style_stack["foreground"]
 
+    return tuple(spans)
+
+
+def _parse_macro_name(tag: str) -> tuple[str, tuple[str, ...]]:
+    args_start = tag.find("(")
+
+    if args_start == -1:
+        return tag, []
+
+    arguments = [arg.strip() for arg in tag[args_start + 1 : -1].split(",")]
+
+    return tag[:args_start], arguments
+
+
+def _expand_macros(text: str, ctx: ContextMapping) -> str:
+    """Expands all !macros in text to evaluated returned content."""
+
+    get_macro = ctx["macros"].get
+    current: dict[str, Callable[[str], str]] = {}
+    expanded = ""
+
+    for mtch in RE_MARKUP.finditer(text):
+        tag_group, plain = mtch.groups()
+
+        # This usually happens at the end of a string
+        if plain is None and tag_group is None:
+            continue
+
+        if plain is None:
+            plain = ""
+
+        if tag_group is None:
+            tag_group = ""
+
+        tags = tag_group.split()
+
+        for tag in tags.copy():
+            if tag == "/":
+                current.clear()
+                continue
+
+            if tag.startswith("/!"):
+                tag = tag.lstrip("/")
+
+                if tag not in current:
+                    raise ValueError(f"Cannot unset not-set macro {tag!r}.")
+
+                del current[tag]
+                tags.remove(f"/{tag}")
+                continue
+
+            if not tag.startswith("!"):
+                continue
+
+            name, arguments = _parse_macro_name(tag)
+            macro = get_macro(name, None)
+
+            if macro is None:
+                raise ValueError(f"Undefined macro {tag!r}.")
+
+            current[tag] = (macro, arguments)
+            tags.remove(tag)
+
+        if len(tags) > 0:
+            expanded += f"[{' '.join(tags)}]"
+
+        for macro, arguments in current.values():
+            plain = macro(plain, *arguments)
+
+        expanded += plain
+
+    return expanded
+
 
 def parse_spans(spans: Iterable[Span]) -> str:  # pylint: disable=too-many-branches
     """Parses spans into an optimized ANSI string.
 
     Args:
         spans: Any iterable of spans.
 
@@ -424,17 +465,17 @@
 
     Returns:
         The parsed string that is represented by the given markup.
     """
 
     ctx = ctx or GLOBAL_CONTEXT
 
-    hashable_key = _get_hashable_key(text, ctx, prefix)
+    # hashable_key = _get_hashable_key(text, ctx, prefix)
 
-    if hashable_key in _markup_cache:
-        return _markup_cache[hashable_key]
+    # if hashable_key in _markup_cache:
+    #     return _markup_cache[hashable_key]
 
     buff = parse_spans(markup_spans(text, ctx, prefix))
 
-    _markup_cache[hashable_key] = buff
+    # _markup_cache[hashable_key] = buff
 
     return buff
```

### Comparing `sh40_zenith-0.0.2/zenith/palette.py` & `sh40_zenith-0.1.0/zenith/palette.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from __future__ import annotations
 
 from dataclasses import dataclass, field
 from typing import Callable
 
 from .color import Color
-from .markup import ContextMapping, alias
+from .markup import MarkupContext, zml_alias
 
 __all__ = [
     "triadic",
     "analogous",
     "tetradic",
     "PalettingFunction",
     "Palette",
@@ -206,15 +206,15 @@
                     key = f"{name}{i}"
                     colorhex = color.darken(-i, step_size=shade_step).hex
 
                 else:
                     key = f"{name}+{i}"
                     colorhex = color.lighten(i, step_size=shade_step).hex
 
-                alias(**{key: colorhex, f"@{key}": f"@{colorhex}"}, ctx=ctx)
+                zml_alias(**{key: colorhex, f"@{key}": f"@{colorhex}"}, ctx=ctx)
 
     def render(self) -> str:
         """Returns markup that shows off the palette.
 
         Note that this is done according to the current `color_mapping`.
         """
```

### Comparing `sh40_zenith-0.0.2/.gitignore` & `sh40_zenith-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `sh40_zenith-0.0.2/LICENSE.txt` & `sh40_zenith-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sh40_zenith-0.0.2/README.md` & `sh40_zenith-0.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ![zenith](https://singlecolorimage.com/get/4A7A9F/1600x200)
 
 ## zenith
 
 A markup language and color palette generators targeting the terminal.
 
 ```
-pip install zenith
+pip install sh40-zenith
 ```
 
 ![rule](https://singlecolorimage.com/get/4A7A9F/1600x5)
 
 ### Purpose
 
 The primary usecase for Zenith is to color and style text in the terminal. We do this through 2 connected systems, our markup language and palette generation.
```

### Comparing `sh40_zenith-0.0.2/pyproject.toml` & `sh40_zenith-0.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sh40_zenith-0.0.2/PKG-INFO` & `sh40_zenith-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sh40-zenith
-Version: 0.0.2
+Version: 0.1.0
 Summary: A markup language and color palette generators targeting the terminal.
 Project-URL: Documentation, https://github.com/shade40/zenith#readme
 Project-URL: Issues, https://github.com/shade40/zenith#issues
 Project-URL: Source, https://github.com/shade40/zenith
 Author-email: bczsalba <bczsalba@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -23,15 +23,15 @@
 ![zenith](https://singlecolorimage.com/get/4A7A9F/1600x200)
 
 ## zenith
 
 A markup language and color palette generators targeting the terminal.
 
 ```
-pip install zenith
+pip install sh40-zenith
 ```
 
 ![rule](https://singlecolorimage.com/get/4A7A9F/1600x5)
 
 ### Purpose
 
 The primary usecase for Zenith is to color and style text in the terminal. We do this through 2 connected systems, our markup language and palette generation.
```

