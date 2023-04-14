# Comparing `tmp/mediaify-1.3.0.tar.gz` & `tmp/mediaify-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mediaify-1.3.0.tar", last modified: Fri Apr 14 01:43:30 2023, max compression
+gzip compressed data, was "mediaify-1.4.0.tar", last modified: Fri Apr 14 22:13:28 2023, max compression
```

## Comparing `mediaify-1.3.0.tar` & `mediaify-1.4.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1147 2023-04-14 01:43:21.413853 mediaify-1.3.0/LICENSE
--rw-r--r--   0        0        0     3530 2023-04-14 01:43:21.413853 mediaify-1.3.0/README.md
--rw-r--r--   0        0        0     1469 2023-04-14 01:43:21.429855 mediaify-1.3.0/mediaify/__init__.py
--rw-r--r--   0        0        0      185 2023-04-14 01:43:21.429855 mediaify-1.3.0/mediaify/animation/__init__.py
--rw-r--r--   0        0        0     2381 2023-04-14 01:43:21.429855 mediaify-1.3.0/mediaify/animation/encode.py
--rw-r--r--   0        0        0     1180 2023-04-14 01:43:21.429855 mediaify-1.3.0/mediaify/animation/exports.py
--rw-r--r--   0        0        0     1232 2023-04-14 01:43:21.429855 mediaify-1.3.0/mediaify/animation/gif.py
--rw-r--r--   0        0        0     1035 2023-04-14 01:43:21.429855 mediaify-1.3.0/mediaify/animation/utils.py
--rw-r--r--   0        0        0     1653 2023-04-14 01:43:21.429855 mediaify-1.3.0/mediaify/animation/webp.py
--rw-r--r--   0        0        0     1433 2023-04-14 01:43:21.429855 mediaify-1.3.0/mediaify/configs.py
--rw-r--r--   0        0        0     2431 2023-04-14 01:43:21.429855 mediaify-1.3.0/mediaify/files.py
--rw-r--r--   0        0        0      145 2023-04-14 01:43:21.429855 mediaify-1.3.0/mediaify/image/__init__.py
--rw-r--r--   0        0        0     1934 2023-04-14 01:43:21.429855 mediaify-1.3.0/mediaify/image/encode.py
--rw-r--r--   0        0        0     1104 2023-04-14 01:43:21.429855 mediaify-1.3.0/mediaify/image/exports.py
--rw-r--r--   0        0        0      798 2023-04-14 01:43:21.429855 mediaify-1.3.0/mediaify/image/jpeg.py
--rw-r--r--   0        0        0      722 2023-04-14 01:43:21.429855 mediaify-1.3.0/mediaify/image/png.py
--rw-r--r--   0        0        0      778 2023-04-14 01:43:21.429855 mediaify-1.3.0/mediaify/image/webp.py
--rw-r--r--   0        0        0     2457 2023-04-14 01:43:21.429855 mediaify-1.3.0/mediaify/media.py
--rw-r--r--   0        0        0     1802 2023-04-14 01:43:21.429855 mediaify-1.3.0/mediaify/presets.py
--rw-r--r--   0        0        0      733 2023-04-14 01:43:21.429855 mediaify-1.3.0/mediaify/resize.py
--rw-r--r--   0        0        0      328 2023-04-14 01:43:21.429855 mediaify-1.3.0/mediaify/utils.py
--rw-r--r--   0        0        0      162 2023-04-14 01:43:21.429855 mediaify-1.3.0/mediaify/video/__init__.py
--rw-r--r--   0        0        0     1218 2023-04-14 01:43:21.429855 mediaify-1.3.0/mediaify/video/encode.py
--rw-r--r--   0        0        0     1154 2023-04-14 01:43:21.429855 mediaify-1.3.0/mediaify/video/exports.py
--rw-r--r--   0        0        0      226 2023-04-14 01:43:21.429855 mediaify-1.3.0/mediaify/video/ffmpeg.py
--rw-r--r--   0        0        0     1878 2023-04-14 01:43:21.433855 mediaify-1.3.0/mediaify/video/info.py
--rw-r--r--   0        0        0     1445 2023-04-14 01:43:21.433855 mediaify-1.3.0/mediaify/video/summary.py
--rw-r--r--   0        0        0      900 2023-04-14 01:43:21.433855 mediaify-1.3.0/mediaify/video/thumbnail.py
--rw-r--r--   0        0        0     1653 2023-04-14 01:43:21.433855 mediaify-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     4885 1970-01-01 00:00:00.000000 mediaify-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1147 2023-04-14 22:13:17.398703 mediaify-1.4.0/LICENSE
+-rw-r--r--   0        0        0     3780 2023-04-14 22:13:17.398703 mediaify-1.4.0/README.md
+-rw-r--r--   0        0        0     1559 2023-04-14 22:13:17.418703 mediaify-1.4.0/mediaify/__init__.py
+-rw-r--r--   0        0        0      185 2023-04-14 22:13:17.418703 mediaify-1.4.0/mediaify/animation/__init__.py
+-rw-r--r--   0        0        0     2381 2023-04-14 22:13:17.418703 mediaify-1.4.0/mediaify/animation/encode.py
+-rw-r--r--   0        0        0     1180 2023-04-14 22:13:17.418703 mediaify-1.4.0/mediaify/animation/exports.py
+-rw-r--r--   0        0        0     1232 2023-04-14 22:13:17.418703 mediaify-1.4.0/mediaify/animation/gif.py
+-rw-r--r--   0        0        0     1035 2023-04-14 22:13:17.418703 mediaify-1.4.0/mediaify/animation/utils.py
+-rw-r--r--   0        0        0     1653 2023-04-14 22:13:17.418703 mediaify-1.4.0/mediaify/animation/webp.py
+-rw-r--r--   0        0        0     1898 2023-04-14 22:13:17.418703 mediaify-1.4.0/mediaify/configs.py
+-rw-r--r--   0        0        0     2431 2023-04-14 22:13:17.418703 mediaify-1.4.0/mediaify/files.py
+-rw-r--r--   0        0        0      145 2023-04-14 22:13:17.418703 mediaify-1.4.0/mediaify/image/__init__.py
+-rw-r--r--   0        0        0     1920 2023-04-14 22:13:17.418703 mediaify-1.4.0/mediaify/image/encode.py
+-rw-r--r--   0        0        0     1104 2023-04-14 22:13:17.418703 mediaify-1.4.0/mediaify/image/exports.py
+-rw-r--r--   0        0        0     2114 2023-04-14 22:13:17.418703 mediaify-1.4.0/mediaify/image/formats.py
+-rw-r--r--   0        0        0     2457 2023-04-14 22:13:17.418703 mediaify-1.4.0/mediaify/media.py
+-rw-r--r--   0        0        0     1645 2023-04-14 22:13:17.418703 mediaify-1.4.0/mediaify/presets.py
+-rw-r--r--   0        0        0      733 2023-04-14 22:13:17.418703 mediaify-1.4.0/mediaify/resize.py
+-rw-r--r--   0        0        0      328 2023-04-14 22:13:17.418703 mediaify-1.4.0/mediaify/utils.py
+-rw-r--r--   0        0        0      162 2023-04-14 22:13:17.418703 mediaify-1.4.0/mediaify/video/__init__.py
+-rw-r--r--   0        0        0     1519 2023-04-14 22:13:17.418703 mediaify-1.4.0/mediaify/video/encode.py
+-rw-r--r--   0        0        0     1154 2023-04-14 22:13:17.418703 mediaify-1.4.0/mediaify/video/exports.py
+-rw-r--r--   0        0        0      226 2023-04-14 22:13:17.418703 mediaify-1.4.0/mediaify/video/ffmpeg.py
+-rw-r--r--   0        0        0     1150 2023-04-14 22:13:17.418703 mediaify-1.4.0/mediaify/video/formats.py
+-rw-r--r--   0        0        0     1914 2023-04-14 22:13:17.422703 mediaify-1.4.0/mediaify/video/info.py
+-rw-r--r--   0        0        0     1731 2023-04-14 22:13:17.422703 mediaify-1.4.0/mediaify/video/process.py
+-rw-r--r--   0        0        0     1445 2023-04-14 22:13:17.422703 mediaify-1.4.0/mediaify/video/summary.py
+-rw-r--r--   0        0        0      909 2023-04-14 22:13:17.422703 mediaify-1.4.0/mediaify/video/thumbnail.py
+-rw-r--r--   0        0        0     1651 2023-04-14 22:13:17.422703 mediaify-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     5184 1970-01-01 00:00:00.000000 mediaify-1.4.0/PKG-INFO
```

### Comparing `mediaify-1.3.0/LICENSE` & `mediaify-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mediaify-1.3.0/README.md` & `mediaify-1.4.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # Mediaify
 
-Media encoding made simple. Encode media without the hassle by describing the output declaratively!
+Media encoding made simple!
+
+Encode media without the hassle of handling binary data and filenames, instead declare your output declaratively!
 
 ## [Simple](./examples/simple.py)
 
 ```python
 import mediaify
 
 with open('ricardo.gif', 'rb') as f:
@@ -123,7 +125,21 @@
 - Debian/Ubuntu: `sudo apt-get install libmagic1`
 - Homebrew: `brew install libmagic`
 - macports: `port install file`
 
 # Documentation
 
 Unfinished.
+
+# Roadmap
+
+- New Encoders
+    - Video
+        - [ ] WEBM
+        - [ ] MP4
+        - [ ] Video to Animation
+- Audio Support
+    - []
+- Better Resizing
+    - [] Min Size
+    - [] Cropping
+    - [] Blackbars
```

### Comparing `mediaify-1.3.0/mediaify/__init__.py` & `mediaify-1.4.0/mediaify/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 )
 from .configs import (
     WEBPImageEncodeConfig,
     JPEGEncodeConfig,
     PNGEncodeConfig,
     GIFEncodeConfig,
     WEBPAnimationEncodeConfig,
+    WEBMEncodeConfig,
+    MP4EncodeConfig,
     ThumbnailConfig,
     AnimationSummaryConfig,
     UnencodedConfig,
     ResizeConfig,
 
     AnimationConfig,
     ImageConfig,
@@ -69,14 +71,16 @@
     "VideoFile",
 
     "WEBPImageEncodeConfig",
     "JPEGEncodeConfig",
     "PNGEncodeConfig",
     "GIFEncodeConfig",
     "WEBPAnimationEncodeConfig",
+    "WEBMEncodeConfig",
+    "MP4EncodeConfig",
     "AnimationSummaryConfig",
     "ThumbnailConfig",
     "UnencodedConfig",
     "ResizeConfig",
 
     "AnimationConfig",
     "ImageConfig",
```

### Comparing `mediaify-1.3.0/mediaify/animation/encode.py` & `mediaify-1.4.0/mediaify/animation/encode.py`

 * *Files identical despite different names*

### Comparing `mediaify-1.3.0/mediaify/animation/exports.py` & `mediaify-1.4.0/mediaify/animation/exports.py`

 * *Files identical despite different names*

### Comparing `mediaify-1.3.0/mediaify/animation/gif.py` & `mediaify-1.4.0/mediaify/animation/gif.py`

 * *Files identical despite different names*

### Comparing `mediaify-1.3.0/mediaify/animation/utils.py` & `mediaify-1.4.0/mediaify/animation/utils.py`

 * *Files identical despite different names*

### Comparing `mediaify-1.3.0/mediaify/animation/webp.py` & `mediaify-1.4.0/mediaify/animation/webp.py`

 * *Files identical despite different names*

### Comparing `mediaify-1.3.0/mediaify/configs.py` & `mediaify-1.4.0/mediaify/configs.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from dataclasses import dataclass
-from typing_extensions import TypeAlias
+from typing_extensions import Literal, TypeAlias
 
 ImageConfig: TypeAlias = """
     PNGEncodeConfig |
     JPEGEncodeConfig |
     WEBPImageEncodeConfig |
     UnencodedConfig |
     ThumbnailConfig
@@ -11,25 +11,27 @@
 AnimationConfig: TypeAlias = """
     GIFEncodeConfig |
     WEBPAnimationEncodeConfig |
     UnencodedConfig |
     ThumbnailConfig
 """
 VideoConfig: TypeAlias = """
+    WEBMEncodeConfig |
+    MP4EncodeConfig |
     AnimationSummaryConfig  |
     UnencodedConfig |
     ThumbnailConfig
 """
 
 
 @dataclass
 class ResizeConfig:
     width: "int | None" = None
     height: "int | None" = None
-    
+
     max_width: "int | None" = None
     max_height: "int | None" = None
 
 
 @dataclass
 class UnencodedConfig:
     pass
@@ -63,14 +65,33 @@
 class WEBPAnimationEncodeConfig:
     resize: "ResizeConfig | None" = None
     quality: int = 85
     lossless: bool = False
 
 
 @dataclass
+class WEBMEncodeConfig:
+    resize: "ResizeConfig | None" = None
+    framerate: "float|None" = None
+
+
+MP4Preset: TypeAlias = Literal[
+    "ultrafast", "superfast", "veryfast",
+    "faster", "fast", "medium", "slow",
+    "slower", "veryslow"
+]
+@dataclass
+class MP4EncodeConfig:
+    resize: "ResizeConfig | None" = None
+    framerate: "float|None" = None
+    crf: int = 21
+    preset: MP4Preset = "fast"
+
+
+@dataclass
 class ThumbnailConfig:
     encoding: ImageConfig
     offset: float = 0.2
 
 
 @dataclass
 class AnimationSummaryConfig:
```

### Comparing `mediaify-1.3.0/mediaify/files.py` & `mediaify-1.4.0/mediaify/files.py`

 * *Files identical despite different names*

### Comparing `mediaify-1.3.0/mediaify/image/encode.py` & `mediaify-1.4.0/mediaify/image/encode.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,17 +4,19 @@
     WEBPImageEncodeConfig,
     PNGEncodeConfig,
     JPEGEncodeConfig,
     ThumbnailConfig,
     ImageConfig
 )
 from ..utils import guess_mimetype
-from .png import encode_as_png
-from .jpeg import encode_as_jpeg
-from .webp import encode_as_webp
+from .formats import (
+    encode_as_jpeg,
+    encode_as_png,
+    encode_as_webp
+)
 from PIL import Image as PILImage
 import io
 
 
 def encode_with_config(
         data: bytes,
         pillow: PILImage.Image,
```

### Comparing `mediaify-1.3.0/mediaify/image/exports.py` & `mediaify-1.4.0/mediaify/image/exports.py`

 * *Files identical despite different names*

### Comparing `mediaify-1.3.0/mediaify/media.py` & `mediaify-1.4.0/mediaify/media.py`

 * *Files identical despite different names*

### Comparing `mediaify-1.3.0/mediaify/presets.py` & `mediaify-1.4.0/mediaify/presets.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from .configs import (
     ResizeConfig,
     WEBPImageEncodeConfig,
     WEBPAnimationEncodeConfig,
     ThumbnailConfig,
-    UnencodedConfig,
+    MP4EncodeConfig,
     ImageConfig,
     AnimationConfig,
     VideoConfig,
 )
 from typing import List
 
 _default_thumbnails = [
@@ -53,25 +53,17 @@
     ),
 ]
 
 
 class Default:
     image: "ImageConfig" = WEBPImageEncodeConfig(quality=95)
     animation: "AnimationConfig" = WEBPAnimationEncodeConfig(quality=90)
-    video: "VideoConfig" = UnencodedConfig()
+    video: "VideoConfig" = MP4EncodeConfig()
+
+    batch_image = list(_default_thumbnails + [WEBPImageEncodeConfig(quality=90)])
+    batch_animation = list(_default_thumbnails + [WEBPAnimationEncodeConfig(quality=90)])
+    batch_video = list(_default_thumbnails + [MP4EncodeConfig()])
 
-    batch_image = list(_default_thumbnails + [
-        WEBPImageEncodeConfig(
-            resize=ResizeConfig(
-                max_width=1024,
-                max_height=1024,
-            ),
-            quality=90,
-        ),
-        UnencodedConfig(),
-    ])
-    batch_animation = list(_default_thumbnails + [UnencodedConfig()])
-    batch_video = list(_default_thumbnails + [UnencodedConfig()])
 
 __all__ = [
     "Default",
 ]
```

### Comparing `mediaify-1.3.0/mediaify/resize.py` & `mediaify-1.4.0/mediaify/resize.py`

 * *Files identical despite different names*

### Comparing `mediaify-1.3.0/mediaify/video/encode.py` & `mediaify-1.4.0/mediaify/video/encode.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,36 @@
 from ..files import VideoFile, AnimationFile, ImageFile
 from ..configs import (
     VideoConfig,
     UnencodedConfig,
     ThumbnailConfig,
+    WEBMEncodeConfig,
+    MP4EncodeConfig,
     AnimationSummaryConfig,
 )
 from .info import VideoInfo
 from .ffmpeg import assert_ffmpeg_installed
+from .formats import encode_as_mp4, encode_as_webm
 from .summary import encode_as_animation_summary
 from .thumbnail import encode_as_thumbnail
 
 
 def encode_video_with_config(
         data: bytes,
         path: str,
         info: VideoInfo,
         config: "VideoConfig"
         ) -> "VideoFile|AnimationFile|ImageFile":
     assert_ffmpeg_installed()
     if isinstance(config, UnencodedConfig):
         return encode_as_original(data, info)
+    elif isinstance(config, WEBMEncodeConfig):
+        return encode_as_webm(data, path, info, config)
+    elif isinstance(config, MP4EncodeConfig):
+        return encode_as_mp4(data, path, info, config)
     elif isinstance(config, ThumbnailConfig):
         return encode_as_thumbnail(data, path, info, config)
     elif isinstance(config, AnimationSummaryConfig):
         return encode_as_animation_summary(data, path, info, config)
     else:
         raise ValueError("Invalid encoding config")
 
@@ -32,9 +39,9 @@
     return VideoFile(
         data=data,
         mimetype=info.mimetype,
         height=info.height,
         width=info.width,
         duration=info.duration,
         framerate=info.framerate,
-        hasAudio=info.audio,
+        hasAudio=info.hasAudio,
     )
```

### Comparing `mediaify-1.3.0/mediaify/video/exports.py` & `mediaify-1.4.0/mediaify/video/exports.py`

 * *Files identical despite different names*

### Comparing `mediaify-1.3.0/mediaify/video/info.py` & `mediaify-1.4.0/mediaify/video/info.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from .ffmpeg import assert_ffmpeg_installed
+from ..files import VideoFile
 import mimetypes
 from typing import Any
 from typing import Dict
 from dataclasses import dataclass
 from magic import Magic
 import numexpr  # type: ignore
 import ffmpeg  # type: ignore
@@ -11,15 +12,15 @@
 @dataclass
 class VideoInfo:
     height: int
     width: int
     framerate: int
     mimetype: str
     extention: str
-    audio: bool
+    hasAudio: bool
     duration: float
     frame_count: "int|None"
 
 
 def get_video_info(filepath: str) -> VideoInfo:
     assert_ffmpeg_installed()
     probe_data = ffmpeg.probe(filepath)
@@ -53,15 +54,15 @@
 
     return VideoInfo(
         width=width,
         height=height,
         mimetype=mimetype,
         extention=extention,
         framerate=framerate,
-        audio=hasAudio,
+        hasAudio=hasAudio,
         frame_count=frame_count,
         duration=duration,
     )
 
 
 def _get_video_stream(probe_data: Dict[str, Any]) -> "Dict[str, Any]":
     video_streams = [
```

### Comparing `mediaify-1.3.0/mediaify/video/summary.py` & `mediaify-1.4.0/mediaify/video/summary.py`

 * *Files identical despite different names*

### Comparing `mediaify-1.3.0/mediaify/video/thumbnail.py` & `mediaify-1.4.0/mediaify/video/thumbnail.py`

 * *Files 14% similar despite different names*

```diff
@@ -30,10 +30,10 @@
             .run(
                 input=data,
                 capture_stdout=True,
                 capture_stderr=True
             )
         )
     except ffmpeg.Error as e:
-        raise ValueError(e.stderr)
+        raise ValueError(e.stderr.decode())
 
     return encode_image(data, config)
```

### Comparing `mediaify-1.3.0/pyproject.toml` & `mediaify-1.4.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "flit_core.buildapi"
 requires = ["flit_core >=3.8.0,<4"]
 
 [project]
 name = "mediaify"
-version = "1.3.0"
+version = "1.4.0"
 description = "Media encoding made simple"
 license = {file = "LICENSE"}
 readme = "README.md"
 authors = [
     {name = "Ben Brady", email = "benbradybusiness@gmail.com"},
 ]
 classifiers = [
@@ -42,17 +42,17 @@
 Source = "https://github.com/Ben-Brady/mediaify"
 
 
 [project.optional-dependencies]
 test = [
     "mypy ==0.982",
     "pytest >=7.1.3,<8.0.0",
+    "black == 23.1.0",
     # "coverage[toml] >= 6.5.0,< 8.0",
     # "ruff ==0.0.138",
-    # "black == 23.1.0",
 ]
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 addopts = "-ra -q"
 testpaths = [
     "tests",
```

### Comparing `mediaify-1.3.0/PKG-INFO` & `mediaify-1.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mediaify
-Version: 1.3.0
+Version: 1.4.0
 Summary: Media encoding made simple
 Author-email: Ben Brady <benbradybusiness@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
@@ -25,20 +25,23 @@
 Requires-Dist: ffmpeg-python~=0.2.0
 Requires-Dist: pillow~=9.5.0
 Requires-Dist: python_magic~=0.4.27
 Requires-Dist: python-magic-bin; sys_platform == 'win32'
 Requires-Dist: numexpr
 Requires-Dist: mypy ==0.982 ; extra == "test"
 Requires-Dist: pytest >=7.1.3,<8.0.0 ; extra == "test"
+Requires-Dist: black == 23.1.0 ; extra == "test"
 Project-URL: Source, https://github.com/Ben-Brady/mediaify
 Provides-Extra: test
 
 # Mediaify
 
-Media encoding made simple. Encode media without the hassle by describing the output declaratively!
+Media encoding made simple!
+
+Encode media without the hassle of handling binary data and filenames, instead declare your output declaratively!
 
 ## [Simple](./examples/simple.py)
 
 ```python
 import mediaify
 
 with open('ricardo.gif', 'rb') as f:
@@ -158,7 +161,21 @@
 - Homebrew: `brew install libmagic`
 - macports: `port install file`
 
 # Documentation
 
 Unfinished.
 
+# Roadmap
+
+- New Encoders
+    - Video
+        - [ ] WEBM
+        - [ ] MP4
+        - [ ] Video to Animation
+- Audio Support
+    - []
+- Better Resizing
+    - [] Min Size
+    - [] Cropping
+    - [] Blackbars
+
```

