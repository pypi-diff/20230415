# Comparing `tmp/Erutils-1.3.0.tar.gz` & `tmp/Erutils-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Erutils-1.3.0.tar", last modified: Sun Apr  9 18:01:41 2023, max compression
+gzip compressed data, was "Erutils-1.3.1.tar", last modified: Sat Apr 15 14:15:12 2023, max compression
```

## Comparing `Erutils-1.3.0.tar` & `Erutils-1.3.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 18:01:41.652065 Erutils-1.3.0/
-drwxrwxrwx   0        0        0        0 2023-04-09 18:01:41.634993 Erutils-1.3.0/Erutils/
--rw-rw-rw-   0        0        0      631 2023-04-09 17:44:30.000000 Erutils-1.3.0/Erutils/__init__.py
--rw-rw-rw-   0        0        0      169 2023-04-09 17:44:30.000000 Erutils-1.3.0/Erutils/__main__.py
--rw-rw-rw-   0        0        0       69 2023-04-09 17:44:30.000000 Erutils-1.3.0/Erutils/config.py
--rw-rw-rw-   0        0        0    32172 2023-04-09 17:44:30.000000 Erutils-1.3.0/Erutils/lightning.py
--rw-rw-rw-   0        0        0     3485 2023-04-09 17:44:30.000000 Erutils-1.3.0/Erutils/loggers.py
--rw-rw-rw-   0        0        0    48407 2023-04-09 17:44:30.000000 Erutils-1.3.0/Erutils/nn.py
--rw-rw-rw-   0        0        0    13359 2023-04-09 17:44:30.000000 Erutils-1.3.0/Erutils/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-09 18:01:41.644487 Erutils-1.3.0/Erutils.egg-info/
--rw-rw-rw-   0        0        0     3075 2023-04-09 18:01:41.000000 Erutils-1.3.0/Erutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      316 2023-04-09 18:01:41.000000 Erutils-1.3.0/Erutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 18:01:41.000000 Erutils-1.3.0/Erutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      109 2023-04-09 18:01:41.000000 Erutils-1.3.0/Erutils.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-09 18:01:41.000000 Erutils-1.3.0/Erutils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3075 2023-04-09 18:01:41.645487 Erutils-1.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     2355 2023-04-09 17:59:20.000000 Erutils-1.3.0/README.md
--rw-rw-rw-   0        0        0      601 2023-04-09 17:44:30.000000 Erutils-1.3.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-09 18:01:41.652065 Erutils-1.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1249 2023-04-09 18:01:29.000000 Erutils-1.3.0/setup.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-04-15 14:15:12.733213 Erutils-1.3.1/
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-04-15 14:15:12.729213 Erutils-1.3.1/Erutils/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      601 2023-04-15 14:09:00.000000 Erutils-1.3.1/Erutils/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      160 2023-04-15 14:06:10.000000 Erutils-1.3.1/Erutils/__main__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       67 2023-04-15 14:06:10.000000 Erutils-1.3.1/Erutils/config.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    32172 2023-04-15 14:06:10.000000 Erutils-1.3.1/Erutils/lightning.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     3379 2023-04-15 14:06:10.000000 Erutils-1.3.1/Erutils/loggers.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    47142 2023-04-15 14:06:10.000000 Erutils-1.3.1/Erutils/nn.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    12973 2023-04-15 14:07:54.000000 Erutils-1.3.1/Erutils/utils.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-04-15 14:15:12.729213 Erutils-1.3.1/Erutils.egg-info/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     3023 2023-04-15 14:15:12.000000 Erutils-1.3.1/Erutils.egg-info/PKG-INFO
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      316 2023-04-15 14:15:12.000000 Erutils-1.3.1/Erutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)        1 2023-04-15 14:15:12.000000 Erutils-1.3.1/Erutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      120 2023-04-15 14:15:12.000000 Erutils-1.3.1/Erutils.egg-info/requires.txt
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)        8 2023-04-15 14:15:12.000000 Erutils-1.3.1/Erutils.egg-info/top_level.txt
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     3023 2023-04-15 14:15:12.729213 Erutils-1.3.1/PKG-INFO
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     2287 2023-04-15 14:06:10.000000 Erutils-1.3.1/README.md
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      576 2023-04-15 14:06:10.000000 Erutils-1.3.1/pyproject.toml
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       38 2023-04-15 14:15:12.733213 Erutils-1.3.1/setup.cfg
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     1272 2023-04-15 14:15:02.000000 Erutils-1.3.1/setup.py
```

### Comparing `Erutils-1.3.0/Erutils/__init__.py` & `Erutils-1.3.1/Erutils/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,11 +5,11 @@
 : dll
 : lightning
 : nn
 : utils
 """
 
 from .utils import create_config, CF, GB, make2d, save_model, str_to_list, tokenize_words, \
-    detokenize_words, download, as_minutes, download_webfile, time_since, mp4_to_mp3, wrd_print, \
+    detokenize_words, download, as_minutes, time_since, wrd_print, \
     file_reader, read_video, read_toml, read_json, read_txt, read_yaml, write_video_frame, HyperParameters, get_memory, \
     monitor_function, device_info, create_output_path
 from .loggers import fprint, Cp, print_model, attar_print, list_color, draw_rec, show_array, Logger
```

### Comparing `Erutils-1.3.0/Erutils/lightning.py` & `Erutils-1.3.1/Erutils/lightning.py`

 * *Files identical despite different names*

### Comparing `Erutils-1.3.0/Erutils/loggers.py` & `Erutils-1.3.1/Erutils/loggers.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,106 +1,106 @@
-import dataclasses
-import sys
-import cv2 as cv
-import keyboard
-import numpy as np
-import matplotlib.pylab as plt
-from .config import DEFAULT_COLOR, STRIDE_COLOR
-from typing import Optional, Union
-
-
-def show_array(array: (np.ndarray, list, tuple)):
-    while True:
-        if isinstance(array, list):
-            array = np.array(array)
-        if array.shape[0] == 3:
-            array = array.reshape((array.shape[1], array.shape[2], array.shape[0]))
-        array = array.astype(np.uint8)
-        cv.imshow('show function', array)
-        cv.waitKey(1)
-        if keyboard.is_pressed('q'):
-            break
-
-
-list_color: Optional[list[list[int]]] = [
-    [255, 0, 0],
-    [0, 255, 0],
-    [0, 0, 255],
-    [255, 255, 0],
-    [0, 255, 255],
-    [255, 0, 255],
-    [100, 200, 220],
-]
-
-
-def draw_rec(x1, y1, x2, y2, img_size: int = 640, thickness=3):
-    fig, ax = plt.subplots()
-    frame = np.zeros((img_size, img_size, 3), dtype=np.uint8)
-    frame[:, :] = [255, 255, 255]
-    print(f'x1, y1, x2, y2 : {x1, y1, x2, y2}')
-    for i, (_x1, _x2, _y1, _y2) in enumerate(zip(x1, x2, y1, y2)):
-        for h in range(img_size):
-            for w in range(img_size):
-                if _x1 < w < _x2 and _y1 < h < _y2:
-                    if _x1 < w < _x1 + thickness or _y1 < h < _y1 + thickness or _x2 - thickness < w < _x2 or _y2 - thickness < h < _y2:
-                        frame[h, w] = list_color[i]
-
-    plt.imshow(frame)
-
-
-@dataclasses.dataclass
-class Cp:
-    Type: Optional[int] = 1
-    BLACK: Optional[str] = f'\033[{Type};30m'
-    RED: Optional[str] = f'\033[{Type};31m'
-    GREEN: Optional[str] = f'\033[{Type};32m'
-    YELLOW: Optional[str] = f'\033[{Type};33m'
-    BLUE: Optional[str] = f'\033[{Type};34m'
-    MAGENTA: Optional[str] = f'\033[{Type};35m'
-    CYAN: Optional[str] = f'\033[{Type};36m'
-    WHITE: Optional[str] = f'\033[{Type};1m'
-    RESET: Optional[str] = f"\033[{Type};39m"
-
-
-def fprint(*args, color: str = DEFAULT_COLOR, **kwargs):
-    print(*(f"{color}{arg}" for arg in args), **kwargs)
-
-
-def attar_print(end: str = '\n', color: str = DEFAULT_COLOR, **kwargs):
-    assert len(kwargs) > 0, 'Keys And Vals Should Have same size'
-
-    fprint((f'{k} : {v} \n' for k, v in kwargs.items()), color=color, end=end)
-
-
-def print_model(model, args, form, rank, index):
-    print('{}  {:<5}{:>20}{:>5}{:>10}    -    {:<25} \n'.format(f'\033[1;39m', f"{index}", f"{form}", f"{rank}",
-                                                                f"{model}",
-                                                                f"{args}"))
-
-
-class Logger:
-    def __init__(self):
-        super(Logger, self).__init__()
-        self.data = ''
-
-    def __call__(self, *args, **kwargs):
-        sys.stdout.write(f"\r {self.data}")
-
-    def set_desc(self, *args):
-        self.data = ''.join(*(d for d in args))
-
-    def end(self):
-        sys.stdout.write('\n')
-
-    def flush(self):
-        sys.stdout.flush()
-
-
-def show_hyper_parameters(hyper_parameters: object) -> None:
-    len_t = 30 + 30 + 8
-
-    fprint('-' * len_t, color=STRIDE_COLOR)
-    for k, v in hyper_parameters.__dict__.items():
-        text: Optional[str] = '{}|{} {:<30} => {:>30} {}|{}'.format(STRIDE_COLOR, DEFAULT_COLOR, f'{k}', f'{v}',
-                                                                    STRIDE_COLOR, DEFAULT_COLOR)
-        fprint(text)
-    fprint('-' * len_t, color=STRIDE_COLOR)
+import dataclasses
+import sys
+import cv2 as cv
+import keyboard
+import numpy as np
+import matplotlib.pylab as plt
+from .config import DEFAULT_COLOR, STRIDE_COLOR
+from typing import Optional, Union
+
+
+def show_array(array: (np.ndarray, list, tuple)):
+    while True:
+        if isinstance(array, list):
+            array = np.array(array)
+        if array.shape[0] == 3:
+            array = array.reshape((array.shape[1], array.shape[2], array.shape[0]))
+        array = array.astype(np.uint8)
+        cv.imshow('show function', array)
+        cv.waitKey(1)
+        if keyboard.is_pressed('q'):
+            break
+
+
+list_color: Optional[list[list[int]]] = [
+    [255, 0, 0],
+    [0, 255, 0],
+    [0, 0, 255],
+    [255, 255, 0],
+    [0, 255, 255],
+    [255, 0, 255],
+    [100, 200, 220],
+]
+
+
+def draw_rec(x1, y1, x2, y2, img_size: int = 640, thickness=3):
+    fig, ax = plt.subplots()
+    frame = np.zeros((img_size, img_size, 3), dtype=np.uint8)
+    frame[:, :] = [255, 255, 255]
+    print(f'x1, y1, x2, y2 : {x1, y1, x2, y2}')
+    for i, (_x1, _x2, _y1, _y2) in enumerate(zip(x1, x2, y1, y2)):
+        for h in range(img_size):
+            for w in range(img_size):
+                if _x1 < w < _x2 and _y1 < h < _y2:
+                    if _x1 < w < _x1 + thickness or _y1 < h < _y1 + thickness or _x2 - thickness < w < _x2 or _y2 - thickness < h < _y2:
+                        frame[h, w] = list_color[i]
+
+    plt.imshow(frame)
+
+
+@dataclasses.dataclass
+class Cp:
+    Type: Optional[int] = 1
+    BLACK: Optional[str] = f'\033[{Type};30m'
+    RED: Optional[str] = f'\033[{Type};31m'
+    GREEN: Optional[str] = f'\033[{Type};32m'
+    YELLOW: Optional[str] = f'\033[{Type};33m'
+    BLUE: Optional[str] = f'\033[{Type};34m'
+    MAGENTA: Optional[str] = f'\033[{Type};35m'
+    CYAN: Optional[str] = f'\033[{Type};36m'
+    WHITE: Optional[str] = f'\033[{Type};1m'
+    RESET: Optional[str] = f"\033[{Type};39m"
+
+
+def fprint(*args, color: str = DEFAULT_COLOR, **kwargs):
+    print(*(f"{color}{arg}" for arg in args), **kwargs)
+
+
+def attar_print(end: str = '\n', color: str = DEFAULT_COLOR, **kwargs):
+    assert len(kwargs) > 0, 'Keys And Vals Should Have same size'
+
+    fprint((f'{k} : {v} \n' for k, v in kwargs.items()), color=color, end=end)
+
+
+def print_model(model, args, form, rank, index):
+    print('{}  {:<5}{:>20}{:>5}{:>10}    -    {:<25} \n'.format(f'\033[1;39m', f"{index}", f"{form}", f"{rank}",
+                                                                f"{model}",
+                                                                f"{args}"))
+
+
+class Logger:
+    def __init__(self):
+        super(Logger, self).__init__()
+        self.data = ''
+
+    def __call__(self, *args, **kwargs):
+        sys.stdout.write(f"\r {self.data}")
+
+    def set_desc(self, *args):
+        self.data = ''.join(*(d for d in args))
+
+    def end(self):
+        sys.stdout.write('\n')
+
+    def flush(self):
+        sys.stdout.flush()
+
+
+def show_hyper_parameters(hyper_parameters: object) -> None:
+    len_t = 30 + 30 + 8
+
+    fprint('-' * len_t, color=STRIDE_COLOR)
+    for k, v in hyper_parameters.__dict__.items():
+        text: Optional[str] = '{}|{} {:<30} => {:>30} {}|{}'.format(STRIDE_COLOR, DEFAULT_COLOR, f'{k}', f'{v}',
+                                                                    STRIDE_COLOR, DEFAULT_COLOR)
+        fprint(text)
+    fprint('-' * len_t, color=STRIDE_COLOR)
```

### Comparing `Erutils-1.3.0/Erutils/utils.py` & `Erutils-1.3.1/Erutils/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,396 +1,396 @@
-import json
-import math
-import time
-import typing
-from typing import Union, Optional
-import pefile
-import glob
-import os
-import shutil
-from pathlib import Path
-import cv2 as cv
-import psutil
-import requests
-import toml
-import yaml
-from moviepy.editor import *
-import dataclasses
-
-import torch
-
-
-# __call__ = ['as_minutes', 'time_since', 'read_video', 'write_video_frame', 'download', 'read_yaml', 'read_json',
-#             'read_txt', 'str_to_list', 'wrd_print', 'mp4_to_mp3', 'read_toml', 'file_reader']
-
-
-class HyperParameters(object):
-    def __init__(self, **kwargs):
-        self.__dict__.update(**kwargs)
-
-
-def as_minutes(s):
-    m = math.floor(s / 60)
-    s -= m * 60
-    return '%dm %ds' % (m, s)
-
-
-def time_since(since, percent):
-    now = time.time()
-    s = now - since
-    es = s / percent
-    rs = es - s
-    return '%s (- %s)' % (as_minutes(s), as_minutes(rs))
-
-
-def read_video(path):
-    fr = cv.VideoCapture(path)
-    return fr
-
-
-def write_video_frame(video):
-    if not os.path.exists('../data/reader'):
-        os.mkdir("../data/reader")
-    cap = read_video(video)
-    f = 0
-    while True:
-        ret, frame = cap.read()
-        # print(ret,frame)
-        if ret:
-            f += 1
-            cv.imshow('windows', frame)
-            cv.imwrite(f'reader/{f}.jpg', frame)
-            cv.waitKey(1)
-            if cv.waitKey(1) == ord('q'):
-                break
-        else:
-            break
-
-    cap.release()
-    cv.destroyAllWindows()
-
-
-def download(path: Union[str, os.PathLike], from_file: bool = False):
-    if from_file:
-        s = open(path, 'r').readlines()
-        for u in s:
-            u = u.replace('\n', '')
-            download(u, from_file=False)
-    else:
-        get = requests.get(url=path, stream=True)
-        name = path.split('/')[-1].replace('%20', '')
-
-        file_size = int(get.headers['content-length'])
-        mb_size = int(file_size / 1000000)
-        downloaded = 0
-        if not os.path.exists(name):
-            with open(name, 'wb') as fp:
-                start = time.time()
-                for chunk in get.iter_content(chunk_size=4096):
-                    downloaded += fp.write(chunk)
-                    now = time.time()
-                    ts = now - start
-                    if ts > 1:
-                        pct_done = round(downloaded / file_size * 100)
-                        speed = round(downloaded / (now - start) / 1024)
-                        pct = int((pct_done / 100) * 50)
-                        downloads = (pct_done / mb_size) if pct_done != 0 else 0
-                        print(
-                            f'\r Download [\033[1;36m{"█" * pct}{" " * (50 - pct)}\033[1;37m] '
-                            f'[{pct_done} % done] | avg speed {speed} kbps || {int(abs(start - now))}'
-                            f' sec :: file size {downloaded / 1000000} / {mb_size} MB',
-                            end='')
-
-        else:
-            def rt():
-                sas: str = input(f'\033[1;31m File already exists [{name}] do you want to replace this file ? [y/n]   ')
-                if sas.lower() == 'y':
-                    os.remove(name)
-                    download(path, from_file)
-                elif sas.lower() == 'n':
-                    pass
-                else:
-                    print(f'Wrong input type  : {sas}')
-                    rt()
-
-            rt()
-
-
-def read_yaml(path: Union[str, os.PathLike] = None):
-    with open(path, 'r') as stream:
-        try:
-            data = yaml.safe_load(stream)
-        except yaml.YAMLError as exc:
-            print(exc)
-    return data
-
-
-def read_json(path: Union[str, os.PathLike] = None):
-    with open(path, 'r') as stream:
-        try:
-            data = json.load(stream)
-        except json.JSONDecodeError as exc:
-            print(exc)
-    return data
-
-
-def read_txt(path: Union[str, os.PathLike] = None):
-    data = []
-    with open(path, 'r') as r:
-        data.append([v for v in r.readlines()])
-    data = [d.replace('\n', '') for d in data[0]]
-    return data
-
-
-def str_to_list(string: str = ''):
-    string += ' '
-    cp = [i for i, v in enumerate(string) if v == ' ']
-    word = [string[0:idx] if i == 0 else string[cp[i - 1]:idx] for i, idx in enumerate(cp)]
-    word = [w.replace(' ', '') for w in word]
-    return word
-
-
-def wrd_print(words: list = None, action: str = None):
-    for idx, i in enumerate(words):
-        name = f'{i=}'.split('=')[0]
-        string = f"{name}" + ("." if action is not None else "") + (action if action is not None else "")
-        print(
-            f'\033[1;36m{idx} : {eval(string)}')
-
-
-def read_toml(path: Union[str, os.PathLike] = None):
-    with open(path, 'r') as r:
-        data = toml.load(r)
-    return data
-
-
-def mp4_to_mp3(mp4, mp3):
-    fc = AudioFileClip(mp4)
-    fc.write_audiofile(mp3)
-    fc.close()
-
-
-def file_reader(path: Union[str, os.PathLike]) -> list:
-    """
-
-    :param path: path to crawl
-    :return: a list with 2 index, index 1 for directories and index 2 for file paths
-    """
-    files = [os.path.join(path, s) for s in os.listdir(path) if os.path.exists(os.path.join(path, s)) if
-             not os.path.isdir(os.path.join(path, s))]
-    dirs = [os.path.join(path, s) for s in os.listdir(path) if os.path.exists(os.path.join(path, s)) if
-            os.path.isdir(os.path.join(path, s))]
-    if len(dirs) != 0:
-
-        for da in dirs:
-
-            if not len(da) == 0 and not isinstance(da, list):
-
-                d, f = file_reader(da)
-                files.append(f)
-                dirs.append(d)
-            else:
-                return [[x for x in dirs if x], [x for x in files if x]]
-    else:
-        return [[x for x in dirs if x], [x for x in files if x]]
-
-
-class GB:
-    def __init__(self, train_data, eval_data, batch_size, chunk_size):
-        self.train_data = train_data
-        self.eval_data = eval_data
-        self.batch_size = batch_size
-        self.chunk_size = chunk_size
-
-    def __call__(self, *args, **kwargs):
-        return self.forward(*args, *kwargs)
-
-    def forward(self, mode: str, *args, **kwargs):
-        data = self.train_data if mode == 'train' else self.eval_data
-        ix = torch.randint(len(data) - self.chunk_size, (self.batch_size,))
-        x = torch.stack([data[i:i + self.chunk_size] for i in ix])
-        y = torch.stack([data[i + 1:i + self.chunk_size + 1] for i in ix])
-        return x, y
-
-
-def save_model(name: str = 'model_save.pt', **kwargs):
-    v = {**kwargs}
-
-    torch.save(v, name)
-
-
-def tokenize_words(word: list, first_word_token: int = 0, swap: int = 1001, last_word_token: int = 1002,
-                   pad_index: int = 1003):
-    """
-    :param swap:
-    :param pad_index:
-    :param last_word_token:
-    :param first_word_token:
-    :param word: index
-    :return: 0 for start token | 1002 for end token
-    """
-    word = [(swap if w == 0 else w) for w in word]
-    word = [first_word_token] + word
-    word.append(last_word_token)
-    word.append(pad_index)
-    return word
-
-
-def detokenize_words(word: list, first_word_token: int = 0, last_word_token: int = 1002, pad_index: int = 1003):
-    """
-    :param pad_index:
-    :param last_word_token:
-    :param first_word_token:
-    :param word: index
-    :return: un tokenized words
-    """
-
-    w = [(first_word_token if w == last_word_token - 1 else w) for w in
-         [w for w in word if w not in [last_word_token, first_word_token]]]
-    del w[-1]
-
-    return w
-
-
-@dataclasses.dataclass
-class CF:
-    ...
-
-
-def create_config(
-        model_type: str = 'PGT-s',
-        num_embedding: int = 512,
-        num_heads: int = 8,
-        chunk: int = 256,
-        vocab_size: int = 5000,
-        num_layers: int = 2,
-        scale_attn_by_layer_idx: bool = False,
-        use_mask: bool = True,
-        attn_dropout: float = 0.2,
-        residual_dropout: float = 0.2,
-        activation: str = "gelu_new",
-        embd_pdrop: float = 0.1,
-        epochs: int = 500,
-        lr: float = 4e-4,
-        pad_token_id: int = 0,
-        create_attention_mask: bool = True,
-        device: str = 'cuda' if torch.cuda.is_available() else 'cpu',
-        weight_decay: float = 2e-1,
-        **kwargs
-
-):
-    intermediate_size: int = num_embedding * 4
-    hidden_size: int = num_embedding
-    max_len = chunk
-    max_position_embeddings = max_len
-    ttl = ['max_position_embeddings', 'hidden_size',
-           'intermediate_size', 'device', 'lr', 'chunk',
-           'embd_pdrop', 'activation', 'epochs', 'pad_token_id',
-           'create_attention_mask',
-           'residual_dropout', 'attn_dropout', 'weight_decay',
-           'use_mask', 'scale_attn_by_layer_idx',
-           'num_layers', 'vocab_size',
-           'max_len', 'num_heads', 'num_embedding']
-    cash = CF()
-    for t in ttl:
-        cash.__setattr__(t, eval(t))
-    v = {**kwargs}
-    if len(v) != 0:
-        for k, v in v.items():
-            cash.__setattr__(k, v)
-
-    return cash
-
-
-def make2d(tensor):
-    return tensor.view(-1, tensor.size(-1))
-
-
-def device_info() -> None:
-    prp = torch.cuda.get_device_properties("cuda")
-    memory = psutil.virtual_memory()
-    free, total_gpu = torch.cuda.mem_get_info('cuda:0')
-    used_gpu = total_gpu - free
-    print('\033[1;36m',
-          f'DEVICES : [ {torch.cuda.get_device_name()} ] | [ Free : {free / 1e9} GB ] | [ Used : {used_gpu / 1e9} GB ] | '
-          f'[ Total : {total_gpu / 1e9} GB ]\n'
-          f'RAM : [ Free : {memory.free / 1e9} GB ] | [ Total : {memory.total / 1e9} GB ]')
-
-
-def get_memory(index: int) -> typing.Tuple[float, float, float]:
-    """
-    :param index: cuda index
-    :return: free,used_gpu,total_gpu memory
-    """
-    free, total_gpu = torch.cuda.mem_get_info(f'cuda:{index}')
-    used_gpu = total_gpu - free
-    free, total_gpu, used_gpu = free / 1e9, total_gpu / 1e9, used_gpu / 1e9
-    return free, used_gpu, total_gpu
-
-
-def monitor_function(function):
-    def wrapper(*args, **kwargs):
-        start = time.perf_counter()
-        result = function(*args, **kwargs)
-        end = time.perf_counter()
-        print(f'\033[1;92m {function.__name__} took {end - start:.6f} seconds to complete')
-        return result
-
-    return wrapper
-
-
-def create_output_path(path: Union[os.PathLike, str], name: Optional[str]):
-    pp = Path(os.path.join(path, name))
-    pp.mkdir(parents=True, exist_ok=True)
-    return pp
-
-
-def fixer_dll(input_path: Union[str, os.PathLike] = "*.dll", backup: bool = False, recursive: bool = False):
-    failures = []
-    for file in glob.glob(input_path, recursive=recursive):
-        print(f"\n---\nChecking {file}...")
-        pe = pefile.PE(file, fast_load=True)
-        nvbSect = [section for section in pe.sections if section.Name.decode().startswith(".nv_fatb")]
-        if len(nvbSect) == 1:
-            sect = nvbSect[0]
-            size = sect.Misc_VirtualSize
-            aslr = pe.OPTIONAL_HEADER.IMAGE_DLLCHARACTERISTICS_DYNAMIC_BASE
-            writable = 0 != (sect.Characteristics & pefile.SECTION_CHARACTERISTICS['IMAGE_SCN_MEM_WRITE'])
-            print(f"Found NV FatBin! Size: {size / 1024 / 1024:0.2f}MB  ASLR: {aslr}  Writable: {writable}")
-            if (writable or aslr) and size > 0:
-                print("- Modifying DLL")
-                if backup:
-                    bakFile = f"{file}_bak"
-                    print(f"- Backing up [{file}] -> [{bakFile}]")
-                    if os.path.exists(bakFile):
-                        print(
-                            f"- Warning: Backup file already exists ({bakFile}), not modifying file! Delete the 'bak' to allow modification")
-                        failures.append(file)
-                        continue
-                    try:
-                        shutil.copy2(file, bakFile)
-                    except Exception as e:
-                        print(f"- Failed to create backup! [{str(e)}], not modifying file!")
-                        failures.append(file)
-                        continue
-                # Disable ASLR for DLL, and disable writing for section
-                pe.OPTIONAL_HEADER.DllCharacteristics &= ~pefile.DLL_CHARACTERISTICS[
-                    'IMAGE_DLLCHARACTERISTICS_DYNAMIC_BASE']
-                sect.Characteristics = sect.Characteristics & ~pefile.SECTION_CHARACTERISTICS['IMAGE_SCN_MEM_WRITE']
-                try:
-                    newFile = f"{file}_mod"
-                    print(f"- Writing modified DLL to [{newFile}]")
-                    pe.write(newFile)
-                    pe.close()
-                    print(f"- Moving modified DLL to [{file}]")
-                    os.remove(file)
-                    shutil.move(newFile, file)
-                except Exception as e:
-                    print(f"- Failed to write modified DLL! [{str(e)}]")
-                    failures.append(file)
-                    continue
-
-    print("\n\nDone!")
-    if len(failures) > 0:
-        print("***WARNING**** These files needed modification but failed: ")
-        for failure in failures:
-            print(f" - {failure}")
+import json
+import math
+import time
+import typing
+from typing import Union, Optional
+import pefile
+import glob
+import os
+import shutil
+from pathlib import Path
+import cv2 as cv
+import psutil
+import requests
+import toml
+import yaml
+# from moviepy.editor import *
+import dataclasses
+
+import torch
+
+
+# __call__ = ['as_minutes', 'time_since', 'read_video', 'write_video_frame', 'download', 'read_yaml', 'read_json',
+#             'read_txt', 'str_to_list', 'wrd_print', 'mp4_to_mp3', 'read_toml', 'file_reader']
+
+
+class HyperParameters(object):
+    def __init__(self, **kwargs):
+        self.__dict__.update(**kwargs)
+
+
+def as_minutes(s):
+    m = math.floor(s / 60)
+    s -= m * 60
+    return '%dm %ds' % (m, s)
+
+
+def time_since(since, percent):
+    now = time.time()
+    s = now - since
+    es = s / percent
+    rs = es - s
+    return '%s (- %s)' % (as_minutes(s), as_minutes(rs))
+
+
+def read_video(path):
+    fr = cv.VideoCapture(path)
+    return fr
+
+
+def write_video_frame(video):
+    if not os.path.exists('../data/reader'):
+        os.mkdir("../data/reader")
+    cap = read_video(video)
+    f = 0
+    while True:
+        ret, frame = cap.read()
+        # print(ret,frame)
+        if ret:
+            f += 1
+            cv.imshow('windows', frame)
+            cv.imwrite(f'reader/{f}.jpg', frame)
+            cv.waitKey(1)
+            if cv.waitKey(1) == ord('q'):
+                break
+        else:
+            break
+
+    cap.release()
+    cv.destroyAllWindows()
+
+
+def download(path: Union[str, os.PathLike], from_file: bool = False):
+    if from_file:
+        s = open(path, 'r').readlines()
+        for u in s:
+            u = u.replace('\n', '')
+            download(u, from_file=False)
+    else:
+        get = requests.get(url=path, stream=True)
+        name = path.split('/')[-1].replace('%20', '')
+
+        file_size = int(get.headers['content-length'])
+        mb_size = int(file_size / 1000000)
+        downloaded = 0
+        if not os.path.exists(name):
+            with open(name, 'wb') as fp:
+                start = time.time()
+                for chunk in get.iter_content(chunk_size=4096):
+                    downloaded += fp.write(chunk)
+                    now = time.time()
+                    ts = now - start
+                    if ts > 1:
+                        pct_done = round(downloaded / file_size * 100)
+                        speed = round(downloaded / (now - start) / 1024)
+                        pct = int((pct_done / 100) * 50)
+                        downloads = (pct_done / mb_size) if pct_done != 0 else 0
+                        print(
+                            f'\r Download [\033[1;36m{"█" * pct}{" " * (50 - pct)}\033[1;37m] '
+                            f'[{pct_done} % done] | avg speed {speed} kbps || {int(abs(start - now))}'
+                            f' sec :: file size {downloaded / 1000000} / {mb_size} MB',
+                            end='')
+
+        else:
+            def rt():
+                sas: str = input(f'\033[1;31m File already exists [{name}] do you want to replace this file ? [y/n]   ')
+                if sas.lower() == 'y':
+                    os.remove(name)
+                    download(path, from_file)
+                elif sas.lower() == 'n':
+                    pass
+                else:
+                    print(f'Wrong input type  : {sas}')
+                    rt()
+
+            rt()
+
+
+def read_yaml(path: Union[str, os.PathLike] = None):
+    with open(path, 'r') as stream:
+        try:
+            data = yaml.safe_load(stream)
+        except yaml.YAMLError as exc:
+            print(exc)
+    return data
+
+
+def read_json(path: Union[str, os.PathLike] = None):
+    with open(path, 'r') as stream:
+        try:
+            data = json.load(stream)
+        except json.JSONDecodeError as exc:
+            print(exc)
+    return data
+
+
+def read_txt(path: Union[str, os.PathLike] = None):
+    data = []
+    with open(path, 'r') as r:
+        data.append([v for v in r.readlines()])
+    data = [d.replace('\n', '') for d in data[0]]
+    return data
+
+
+def str_to_list(string: str = ''):
+    string += ' '
+    cp = [i for i, v in enumerate(string) if v == ' ']
+    word = [string[0:idx] if i == 0 else string[cp[i - 1]:idx] for i, idx in enumerate(cp)]
+    word = [w.replace(' ', '') for w in word]
+    return word
+
+
+def wrd_print(words: list = None, action: str = None):
+    for idx, i in enumerate(words):
+        name = f'{i=}'.split('=')[0]
+        string = f"{name}" + ("." if action is not None else "") + (action if action is not None else "")
+        print(
+            f'\033[1;36m{idx} : {eval(string)}')
+
+
+def read_toml(path: Union[str, os.PathLike] = None):
+    with open(path, 'r') as r:
+        data = toml.load(r)
+    return data
+
+
+# def mp4_to_mp3(mp4, mp3):
+#     fc = AudioFileClip(mp4)
+#     fc.write_audiofile(mp3)
+#     fc.close()
+
+
+def file_reader(path: Union[str, os.PathLike]) -> list:
+    """
+
+    :param path: path to crawl
+    :return: a list with 2 index, index 1 for directories and index 2 for file paths
+    """
+    files = [os.path.join(path, s) for s in os.listdir(path) if os.path.exists(os.path.join(path, s)) if
+             not os.path.isdir(os.path.join(path, s))]
+    dirs = [os.path.join(path, s) for s in os.listdir(path) if os.path.exists(os.path.join(path, s)) if
+            os.path.isdir(os.path.join(path, s))]
+    if len(dirs) != 0:
+
+        for da in dirs:
+
+            if not len(da) == 0 and not isinstance(da, list):
+
+                d, f = file_reader(da)
+                files.append(f)
+                dirs.append(d)
+            else:
+                return [[x for x in dirs if x], [x for x in files if x]]
+    else:
+        return [[x for x in dirs if x], [x for x in files if x]]
+
+
+class GB:
+    def __init__(self, train_data, eval_data, batch_size, chunk_size):
+        self.train_data = train_data
+        self.eval_data = eval_data
+        self.batch_size = batch_size
+        self.chunk_size = chunk_size
+
+    def __call__(self, *args, **kwargs):
+        return self.forward(*args, *kwargs)
+
+    def forward(self, mode: str, *args, **kwargs):
+        data = self.train_data if mode == 'train' else self.eval_data
+        ix = torch.randint(len(data) - self.chunk_size, (self.batch_size,))
+        x = torch.stack([data[i:i + self.chunk_size] for i in ix])
+        y = torch.stack([data[i + 1:i + self.chunk_size + 1] for i in ix])
+        return x, y
+
+
+def save_model(name: str = 'model_save.pt', **kwargs):
+    v = {**kwargs}
+
+    torch.save(v, name)
+
+
+def tokenize_words(word: list, first_word_token: int = 0, swap: int = 1001, last_word_token: int = 1002,
+                   pad_index: int = 1003):
+    """
+    :param swap:
+    :param pad_index:
+    :param last_word_token:
+    :param first_word_token:
+    :param word: index
+    :return: 0 for start token | 1002 for end token
+    """
+    word = [(swap if w == 0 else w) for w in word]
+    word = [first_word_token] + word
+    word.append(last_word_token)
+    word.append(pad_index)
+    return word
+
+
+def detokenize_words(word: list, first_word_token: int = 0, last_word_token: int = 1002, pad_index: int = 1003):
+    """
+    :param pad_index:
+    :param last_word_token:
+    :param first_word_token:
+    :param word: index
+    :return: un tokenized words
+    """
+
+    w = [(first_word_token if w == last_word_token - 1 else w) for w in
+         [w for w in word if w not in [last_word_token, first_word_token]]]
+    del w[-1]
+
+    return w
+
+
+@dataclasses.dataclass
+class CF:
+    ...
+
+
+def create_config(
+        model_type: str = 'PGT-s',
+        num_embedding: int = 512,
+        num_heads: int = 8,
+        chunk: int = 256,
+        vocab_size: int = 5000,
+        num_layers: int = 2,
+        scale_attn_by_layer_idx: bool = False,
+        use_mask: bool = True,
+        attn_dropout: float = 0.2,
+        residual_dropout: float = 0.2,
+        activation: str = "gelu_new",
+        embd_pdrop: float = 0.1,
+        epochs: int = 500,
+        lr: float = 4e-4,
+        pad_token_id: int = 0,
+        create_attention_mask: bool = True,
+        device: str = 'cuda' if torch.cuda.is_available() else 'cpu',
+        weight_decay: float = 2e-1,
+        **kwargs
+
+):
+    intermediate_size: int = num_embedding * 4
+    hidden_size: int = num_embedding
+    max_len = chunk
+    max_position_embeddings = max_len
+    ttl = ['max_position_embeddings', 'hidden_size',
+           'intermediate_size', 'device', 'lr', 'chunk',
+           'embd_pdrop', 'activation', 'epochs', 'pad_token_id',
+           'create_attention_mask',
+           'residual_dropout', 'attn_dropout', 'weight_decay',
+           'use_mask', 'scale_attn_by_layer_idx',
+           'num_layers', 'vocab_size',
+           'max_len', 'num_heads', 'num_embedding']
+    cash = CF()
+    for t in ttl:
+        cash.__setattr__(t, eval(t))
+    v = {**kwargs}
+    if len(v) != 0:
+        for k, v in v.items():
+            cash.__setattr__(k, v)
+
+    return cash
+
+
+def make2d(tensor):
+    return tensor.view(-1, tensor.size(-1))
+
+
+def device_info() -> None:
+    prp = torch.cuda.get_device_properties("cuda")
+    memory = psutil.virtual_memory()
+    free, total_gpu = torch.cuda.mem_get_info('cuda:0')
+    used_gpu = total_gpu - free
+    print('\033[1;36m',
+          f'DEVICES : [ {torch.cuda.get_device_name()} ] | [ Free : {free / 1e9} GB ] | [ Used : {used_gpu / 1e9} GB ] | '
+          f'[ Total : {total_gpu / 1e9} GB ]\n'
+          f'RAM : [ Free : {memory.free / 1e9} GB ] | [ Total : {memory.total / 1e9} GB ]')
+
+
+def get_memory(index: int) -> typing.Tuple[float, float, float]:
+    """
+    :param index: cuda index
+    :return: free,used_gpu,total_gpu memory
+    """
+    free, total_gpu = torch.cuda.mem_get_info(f'cuda:{index}')
+    used_gpu = total_gpu - free
+    free, total_gpu, used_gpu = free / 1e9, total_gpu / 1e9, used_gpu / 1e9
+    return free, used_gpu, total_gpu
+
+
+def monitor_function(function):
+    def wrapper(*args, **kwargs):
+        start = time.perf_counter()
+        result = function(*args, **kwargs)
+        end = time.perf_counter()
+        print(f'\033[1;92m {function.__name__} took {end - start:.6f} seconds to complete')
+        return result
+
+    return wrapper
+
+
+def create_output_path(path: Union[os.PathLike, str], name: Optional[str]):
+    pp = Path(os.path.join(path, name))
+    pp.mkdir(parents=True, exist_ok=True)
+    return pp
+
+
+def fixer_dll(input_path: Union[str, os.PathLike] = "*.dll", backup: bool = False, recursive: bool = False):
+    failures = []
+    for file in glob.glob(input_path, recursive=recursive):
+        print(f"\n---\nChecking {file}...")
+        pe = pefile.PE(file, fast_load=True)
+        nvbSect = [section for section in pe.sections if section.Name.decode().startswith(".nv_fatb")]
+        if len(nvbSect) == 1:
+            sect = nvbSect[0]
+            size = sect.Misc_VirtualSize
+            aslr = pe.OPTIONAL_HEADER.IMAGE_DLLCHARACTERISTICS_DYNAMIC_BASE
+            writable = 0 != (sect.Characteristics & pefile.SECTION_CHARACTERISTICS['IMAGE_SCN_MEM_WRITE'])
+            print(f"Found NV FatBin! Size: {size / 1024 / 1024:0.2f}MB  ASLR: {aslr}  Writable: {writable}")
+            if (writable or aslr) and size > 0:
+                print("- Modifying DLL")
+                if backup:
+                    bakFile = f"{file}_bak"
+                    print(f"- Backing up [{file}] -> [{bakFile}]")
+                    if os.path.exists(bakFile):
+                        print(
+                            f"- Warning: Backup file already exists ({bakFile}), not modifying file! Delete the 'bak' to allow modification")
+                        failures.append(file)
+                        continue
+                    try:
+                        shutil.copy2(file, bakFile)
+                    except Exception as e:
+                        print(f"- Failed to create backup! [{str(e)}], not modifying file!")
+                        failures.append(file)
+                        continue
+                # Disable ASLR for DLL, and disable writing for section
+                pe.OPTIONAL_HEADER.DllCharacteristics &= ~pefile.DLL_CHARACTERISTICS[
+                    'IMAGE_DLLCHARACTERISTICS_DYNAMIC_BASE']
+                sect.Characteristics = sect.Characteristics & ~pefile.SECTION_CHARACTERISTICS['IMAGE_SCN_MEM_WRITE']
+                try:
+                    newFile = f"{file}_mod"
+                    print(f"- Writing modified DLL to [{newFile}]")
+                    pe.write(newFile)
+                    pe.close()
+                    print(f"- Moving modified DLL to [{file}]")
+                    os.remove(file)
+                    shutil.move(newFile, file)
+                except Exception as e:
+                    print(f"- Failed to write modified DLL! [{str(e)}]")
+                    failures.append(file)
+                    continue
+
+    print("\n\nDone!")
+    if len(failures) > 0:
+        print("***WARNING**** These files needed modification but failed: ")
+        for failure in failures:
+            print(f" - {failure}")
```

### Comparing `Erutils-1.3.0/Erutils.egg-info/PKG-INFO` & `Erutils-1.3.1/Erutils.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,88 +1,91 @@
-Metadata-Version: 2.1
-Name: Erutils
-Version: 1.3.0
-Home-page: https://github.com/erfanzar/
-Author: Erfan Zare Chavoshi
-Author-email: erfanzare82@yahoo.com
-License: Apache License 2.0
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.6, <3.11
-Description-Content-Type: text/markdown
-
-# Erutils
-
-The Erutils package includes a collection of utilities and pre-built neural networks that I frequently use in my
-personal projects. While this package is mainly for my personal use, others may find it useful as well.
-
-# Installation
-
-You can install Erutils using pip:
-
-```shell
-pip install Erutils
-````
-
-Open [erfan zare Github](https://github.com/erfanzar/)
-
-Open [Package Github](https://github.com/erfanzar/Erutils)
-
-## 🚀 APIs and Usages
-
-```python
-import Erutils
-from Erutils.loggers import *
-# Loggers contain Logging stuff
-from Erutils.nn import *
-# NN contain Nural networks built in Pytorch
-# you can easily import Erutils.nn and use many prebuilt neurons in the project 
-# if you thing any refrence should be added tell me in discussion 
-from Erutils.lightning import *
-# Lightning Contain Some CV Packages
-from Erutils.utils import *
-# Utils Contain Some Utils like reading files downloading and etc ...
-```
-
-# Neural Networks
-
-Erutils includes a diverse collection of over 80 pre-built neural networks that cover a wide range of applications, such
-as natural language processing, computer vision, and more. Some of the neural networks included are:
-
-- Transformers: Customized transformer encoder and decoder layers for natural language processing tasks and a lot of
-  customized Layers like RoEmbedding ...
-- Feed-forward networks: Customized feed-forward layers for various applications
-- Custom CNN backbones: A variety of pre-built CNN backbones for computer vision tasks, such as ResNet, VGG, and more
-- Object Detection: Pre-built networks for object detection and localization, including YOLOv5, RetinaNet, and Faster
-  R-CNN
-- Custom CNN architectures: Custom CNN architectures designed for specific applications, such as image classification,
-  segmentation, and more.
-
-## 🚀 About Me
-
-Hi there 👋
-I like to train deep neural nets on large datasets 🧠.
-Among other things in this world:)
-
-## License
-
-[MIT](https://choosealicense.com/licenses/mit/)
-
-# Contributing
-
-While this package is mainly for my personal use, contributions and suggestions are welcome. If you find a bug or have
-an idea for a new feature, please open an issue on the GitHub repository.
-
-## Used By
-
-Private Project
-
-## Author
-
-- [@erfanzar](https://www.github.com/erfanzar)
+Metadata-Version: 2.1
+Name: Erutils
+Version: 1.3.1
+Summary: UNKNOWN
+Home-page: https://github.com/erfanzar/
+Author: Erfan Zare Chavoshi
+Author-email: erfanzare82@yahoo.com
+License: Apache License 2.0
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.6, <3.11
+Description-Content-Type: text/markdown
+
+# Erutils
+
+The Erutils package includes a collection of utilities and pre-built neural networks that I frequently use in my
+personal projects. While this package is mainly for my personal use, others may find it useful as well.
+
+# Installation
+
+You can install Erutils using pip:
+
+```shell
+pip install Erutils
+````
+
+Open [erfan zare Github](https://github.com/erfanzar/)
+
+Open [Package Github](https://github.com/erfanzar/Erutils)
+
+## 🚀 APIs and Usages
+
+```python
+import Erutils
+from Erutils.loggers import *
+# Loggers contain Logging stuff
+from Erutils.nn import *
+# NN contain Nural networks built in Pytorch
+# you can easily import Erutils.nn and use many prebuilt neurons in the project 
+# if you thing any refrence should be added tell me in discussion 
+from Erutils.lightning import *
+# Lightning Contain Some CV Packages
+from Erutils.utils import *
+# Utils Contain Some Utils like reading files downloading and etc ...
+```
+
+# Neural Networks
+
+Erutils includes a diverse collection of over 80 pre-built neural networks that cover a wide range of applications, such
+as natural language processing, computer vision, and more. Some of the neural networks included are:
+
+- Transformers: Customized transformer encoder and decoder layers for natural language processing tasks and a lot of
+  customized Layers like RoEmbedding ...
+- Feed-forward networks: Customized feed-forward layers for various applications
+- Custom CNN backbones: A variety of pre-built CNN backbones for computer vision tasks, such as ResNet, VGG, and more
+- Object Detection: Pre-built networks for object detection and localization, including YOLOv5, RetinaNet, and Faster
+  R-CNN
+- Custom CNN architectures: Custom CNN architectures designed for specific applications, such as image classification,
+  segmentation, and more.
+
+## 🚀 About Me
+
+Hi there 👋
+I like to train deep neural nets on large datasets 🧠.
+Among other things in this world:)
+
+## License
+
+[MIT](https://choosealicense.com/licenses/mit/)
+
+# Contributing
+
+While this package is mainly for my personal use, contributions and suggestions are welcome. If you find a bug or have
+an idea for a new feature, please open an issue on the GitHub repository.
+
+## Used By
+
+Private Project
+
+## Author
+
+- [@erfanzar](https://www.github.com/erfanzar)
+
```

### Comparing `Erutils-1.3.0/PKG-INFO` & `Erutils-1.3.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,88 +1,91 @@
-Metadata-Version: 2.1
-Name: Erutils
-Version: 1.3.0
-Home-page: https://github.com/erfanzar/
-Author: Erfan Zare Chavoshi
-Author-email: erfanzare82@yahoo.com
-License: Apache License 2.0
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.6, <3.11
-Description-Content-Type: text/markdown
-
-# Erutils
-
-The Erutils package includes a collection of utilities and pre-built neural networks that I frequently use in my
-personal projects. While this package is mainly for my personal use, others may find it useful as well.
-
-# Installation
-
-You can install Erutils using pip:
-
-```shell
-pip install Erutils
-````
-
-Open [erfan zare Github](https://github.com/erfanzar/)
-
-Open [Package Github](https://github.com/erfanzar/Erutils)
-
-## 🚀 APIs and Usages
-
-```python
-import Erutils
-from Erutils.loggers import *
-# Loggers contain Logging stuff
-from Erutils.nn import *
-# NN contain Nural networks built in Pytorch
-# you can easily import Erutils.nn and use many prebuilt neurons in the project 
-# if you thing any refrence should be added tell me in discussion 
-from Erutils.lightning import *
-# Lightning Contain Some CV Packages
-from Erutils.utils import *
-# Utils Contain Some Utils like reading files downloading and etc ...
-```
-
-# Neural Networks
-
-Erutils includes a diverse collection of over 80 pre-built neural networks that cover a wide range of applications, such
-as natural language processing, computer vision, and more. Some of the neural networks included are:
-
-- Transformers: Customized transformer encoder and decoder layers for natural language processing tasks and a lot of
-  customized Layers like RoEmbedding ...
-- Feed-forward networks: Customized feed-forward layers for various applications
-- Custom CNN backbones: A variety of pre-built CNN backbones for computer vision tasks, such as ResNet, VGG, and more
-- Object Detection: Pre-built networks for object detection and localization, including YOLOv5, RetinaNet, and Faster
-  R-CNN
-- Custom CNN architectures: Custom CNN architectures designed for specific applications, such as image classification,
-  segmentation, and more.
-
-## 🚀 About Me
-
-Hi there 👋
-I like to train deep neural nets on large datasets 🧠.
-Among other things in this world:)
-
-## License
-
-[MIT](https://choosealicense.com/licenses/mit/)
-
-# Contributing
-
-While this package is mainly for my personal use, contributions and suggestions are welcome. If you find a bug or have
-an idea for a new feature, please open an issue on the GitHub repository.
-
-## Used By
-
-Private Project
-
-## Author
-
-- [@erfanzar](https://www.github.com/erfanzar)
+Metadata-Version: 2.1
+Name: Erutils
+Version: 1.3.1
+Summary: UNKNOWN
+Home-page: https://github.com/erfanzar/
+Author: Erfan Zare Chavoshi
+Author-email: erfanzare82@yahoo.com
+License: Apache License 2.0
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.6, <3.11
+Description-Content-Type: text/markdown
+
+# Erutils
+
+The Erutils package includes a collection of utilities and pre-built neural networks that I frequently use in my
+personal projects. While this package is mainly for my personal use, others may find it useful as well.
+
+# Installation
+
+You can install Erutils using pip:
+
+```shell
+pip install Erutils
+````
+
+Open [erfan zare Github](https://github.com/erfanzar/)
+
+Open [Package Github](https://github.com/erfanzar/Erutils)
+
+## 🚀 APIs and Usages
+
+```python
+import Erutils
+from Erutils.loggers import *
+# Loggers contain Logging stuff
+from Erutils.nn import *
+# NN contain Nural networks built in Pytorch
+# you can easily import Erutils.nn and use many prebuilt neurons in the project 
+# if you thing any refrence should be added tell me in discussion 
+from Erutils.lightning import *
+# Lightning Contain Some CV Packages
+from Erutils.utils import *
+# Utils Contain Some Utils like reading files downloading and etc ...
+```
+
+# Neural Networks
+
+Erutils includes a diverse collection of over 80 pre-built neural networks that cover a wide range of applications, such
+as natural language processing, computer vision, and more. Some of the neural networks included are:
+
+- Transformers: Customized transformer encoder and decoder layers for natural language processing tasks and a lot of
+  customized Layers like RoEmbedding ...
+- Feed-forward networks: Customized feed-forward layers for various applications
+- Custom CNN backbones: A variety of pre-built CNN backbones for computer vision tasks, such as ResNet, VGG, and more
+- Object Detection: Pre-built networks for object detection and localization, including YOLOv5, RetinaNet, and Faster
+  R-CNN
+- Custom CNN architectures: Custom CNN architectures designed for specific applications, such as image classification,
+  segmentation, and more.
+
+## 🚀 About Me
+
+Hi there 👋
+I like to train deep neural nets on large datasets 🧠.
+Among other things in this world:)
+
+## License
+
+[MIT](https://choosealicense.com/licenses/mit/)
+
+# Contributing
+
+While this package is mainly for my personal use, contributions and suggestions are welcome. If you find a bug or have
+an idea for a new feature, please open an issue on the GitHub repository.
+
+## Used By
+
+Private Project
+
+## Author
+
+- [@erfanzar](https://www.github.com/erfanzar)
+
```

### Comparing `Erutils-1.3.0/README.md` & `Erutils-1.3.1/README.md`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,69 +1,69 @@
-# Erutils
-
-The Erutils package includes a collection of utilities and pre-built neural networks that I frequently use in my
-personal projects. While this package is mainly for my personal use, others may find it useful as well.
-
-# Installation
-
-You can install Erutils using pip:
-
-```shell
-pip install Erutils
-````
-
-Open [erfan zare Github](https://github.com/erfanzar/)
-
-Open [Package Github](https://github.com/erfanzar/Erutils)
-
-## 🚀 APIs and Usages
-
-```python
-import Erutils
-from Erutils.loggers import *
-# Loggers contain Logging stuff
-from Erutils.nn import *
-# NN contain Nural networks built in Pytorch
-# you can easily import Erutils.nn and use many prebuilt neurons in the project 
-# if you thing any refrence should be added tell me in discussion 
-from Erutils.lightning import *
-# Lightning Contain Some CV Packages
-from Erutils.utils import *
-# Utils Contain Some Utils like reading files downloading and etc ...
-```
-
-# Neural Networks
-
-Erutils includes a diverse collection of over 80 pre-built neural networks that cover a wide range of applications, such
-as natural language processing, computer vision, and more. Some of the neural networks included are:
-
-- Transformers: Customized transformer encoder and decoder layers for natural language processing tasks and a lot of
-  customized Layers like RoEmbedding ...
-- Feed-forward networks: Customized feed-forward layers for various applications
-- Custom CNN backbones: A variety of pre-built CNN backbones for computer vision tasks, such as ResNet, VGG, and more
-- Object Detection: Pre-built networks for object detection and localization, including YOLOv5, RetinaNet, and Faster
-  R-CNN
-- Custom CNN architectures: Custom CNN architectures designed for specific applications, such as image classification,
-  segmentation, and more.
-
-## 🚀 About Me
-
-Hi there 👋
-I like to train deep neural nets on large datasets 🧠.
-Among other things in this world:)
-
-## License
-
-[MIT](https://choosealicense.com/licenses/mit/)
-
-# Contributing
-
-While this package is mainly for my personal use, contributions and suggestions are welcome. If you find a bug or have
-an idea for a new feature, please open an issue on the GitHub repository.
-
-## Used By
-
-Private Project
-
-## Author
-
+# Erutils
+
+The Erutils package includes a collection of utilities and pre-built neural networks that I frequently use in my
+personal projects. While this package is mainly for my personal use, others may find it useful as well.
+
+# Installation
+
+You can install Erutils using pip:
+
+```shell
+pip install Erutils
+````
+
+Open [erfan zare Github](https://github.com/erfanzar/)
+
+Open [Package Github](https://github.com/erfanzar/Erutils)
+
+## 🚀 APIs and Usages
+
+```python
+import Erutils
+from Erutils.loggers import *
+# Loggers contain Logging stuff
+from Erutils.nn import *
+# NN contain Nural networks built in Pytorch
+# you can easily import Erutils.nn and use many prebuilt neurons in the project 
+# if you thing any refrence should be added tell me in discussion 
+from Erutils.lightning import *
+# Lightning Contain Some CV Packages
+from Erutils.utils import *
+# Utils Contain Some Utils like reading files downloading and etc ...
+```
+
+# Neural Networks
+
+Erutils includes a diverse collection of over 80 pre-built neural networks that cover a wide range of applications, such
+as natural language processing, computer vision, and more. Some of the neural networks included are:
+
+- Transformers: Customized transformer encoder and decoder layers for natural language processing tasks and a lot of
+  customized Layers like RoEmbedding ...
+- Feed-forward networks: Customized feed-forward layers for various applications
+- Custom CNN backbones: A variety of pre-built CNN backbones for computer vision tasks, such as ResNet, VGG, and more
+- Object Detection: Pre-built networks for object detection and localization, including YOLOv5, RetinaNet, and Faster
+  R-CNN
+- Custom CNN architectures: Custom CNN architectures designed for specific applications, such as image classification,
+  segmentation, and more.
+
+## 🚀 About Me
+
+Hi there 👋
+I like to train deep neural nets on large datasets 🧠.
+Among other things in this world:)
+
+## License
+
+[MIT](https://choosealicense.com/licenses/mit/)
+
+# Contributing
+
+While this package is mainly for my personal use, contributions and suggestions are welcome. If you find a bug or have
+an idea for a new feature, please open an issue on the GitHub repository.
+
+## Used By
+
+Private Project
+
+## Author
+
 - [@erfanzar](https://www.github.com/erfanzar)
```

### Comparing `Erutils-1.3.0/setup.py` & `Erutils-1.3.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="Erutils",
-    version='1.3.0',
+    version='1.3.1',
     author="Erfan Zare Chavoshi",
     author_email="erfanzare82@yahoo.com",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/erfanzar/",
     packages=setuptools.find_packages(),
     install_requires=[
@@ -21,15 +21,16 @@
         'nltk',
         'pandas',
         'json5',
         'PyYAML',
         'torchtext>=0.9.0',
         'torchaudio>=0.9.0',
         'onnxruntime',
-        'thop'
+        'thop',
+        'matplotlib'
     ],
     python_requires=">=3.6, <3.11",
     license='Apache License 2.0',
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
```

