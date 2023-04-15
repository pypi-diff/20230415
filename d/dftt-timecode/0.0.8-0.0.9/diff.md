# Comparing `tmp/dftt_timecode-0.0.8.tar.gz` & `tmp/dftt_timecode-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\dftt_timecode-0.0.8.tar", last modified: Tue Jan 18 15:28:05 2022, max compression
+gzip compressed data, was "dist\dftt_timecode-0.0.9.tar", last modified: Wed Feb  2 15:29:05 2022, max compression
```

## Comparing `dftt_timecode-0.0.8.tar` & `dftt_timecode-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2022-01-18 15:28:05.299356 dftt_timecode-0.0.8/
--rw-rw-rw-   0        0        0    26526 2022-01-16 17:06:52.000000 dftt_timecode-0.0.8/LICENSE.txt
--rw-rw-rw-   0        0        0     7615 2022-01-18 15:28:05.299356 dftt_timecode-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     6948 2022-01-18 15:22:55.000000 dftt_timecode-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2022-01-18 15:28:05.283396 dftt_timecode-0.0.8/dftt_timecode/
--rw-rw-rw-   0        0        0      121 2022-01-18 15:27:55.000000 dftt_timecode-0.0.8/dftt_timecode/__init__.py
--rw-rw-rw-   0        0        0    39481 2022-01-18 10:31:57.000000 dftt_timecode-0.0.8/dftt_timecode/core.py
--rw-rw-rw-   0        0        0      962 2022-01-11 11:01:09.000000 dftt_timecode-0.0.8/dftt_timecode/dispatch.py
--rw-rw-rw-   0        0        0      140 2022-01-16 13:53:26.000000 dftt_timecode-0.0.8/dftt_timecode/error.py
--rw-rw-rw-   0        0        0     1399 2022-01-17 16:09:24.000000 dftt_timecode-0.0.8/dftt_timecode/pattern.py
-drwxrwxrwx   0        0        0        0 2022-01-18 15:28:05.298358 dftt_timecode-0.0.8/dftt_timecode.egg-info/
--rw-rw-rw-   0        0        0     7615 2022-01-18 15:28:05.000000 dftt_timecode-0.0.8/dftt_timecode.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      300 2022-01-18 15:28:05.000000 dftt_timecode-0.0.8/dftt_timecode.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-01-18 15:28:05.000000 dftt_timecode-0.0.8/dftt_timecode.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2022-01-18 15:28:05.000000 dftt_timecode-0.0.8/dftt_timecode.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-01-18 15:28:05.300353 dftt_timecode-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      855 2022-01-18 15:27:53.000000 dftt_timecode-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2022-02-02 15:29:05.980053 dftt_timecode-0.0.9/
+-rw-rw-rw-   0        0        0    26526 2022-01-16 17:06:52.000000 dftt_timecode-0.0.9/LICENSE.txt
+-rw-rw-rw-   0        0        0    33496 2022-02-02 15:29:05.980053 dftt_timecode-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0    32829 2022-02-02 15:24:03.000000 dftt_timecode-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2022-02-02 15:29:05.970081 dftt_timecode-0.0.9/dftt_timecode/
+-rw-rw-rw-   0        0        0      121 2022-02-02 15:25:20.000000 dftt_timecode-0.0.9/dftt_timecode/__init__.py
+-rw-rw-rw-   0        0        0    40995 2022-02-02 14:55:54.000000 dftt_timecode-0.0.9/dftt_timecode/core.py
+-rw-rw-rw-   0        0        0      962 2022-01-11 11:01:09.000000 dftt_timecode-0.0.9/dftt_timecode/dispatch.py
+-rw-rw-rw-   0        0        0      140 2022-01-16 13:53:26.000000 dftt_timecode-0.0.9/dftt_timecode/error.py
+-rw-rw-rw-   0        0        0     1398 2022-01-30 17:13:17.000000 dftt_timecode-0.0.9/dftt_timecode/pattern.py
+drwxrwxrwx   0        0        0        0 2022-02-02 15:29:05.979074 dftt_timecode-0.0.9/dftt_timecode.egg-info/
+-rw-rw-rw-   0        0        0    33496 2022-02-02 15:29:05.000000 dftt_timecode-0.0.9/dftt_timecode.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      300 2022-02-02 15:29:05.000000 dftt_timecode-0.0.9/dftt_timecode.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-02-02 15:29:05.000000 dftt_timecode-0.0.9/dftt_timecode.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2022-02-02 15:29:05.000000 dftt_timecode-0.0.9/dftt_timecode.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2022-02-02 15:29:05.980053 dftt_timecode-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      855 2022-02-02 15:27:55.000000 dftt_timecode-0.0.9/setup.py
```

### Comparing `dftt_timecode-0.0.8/LICENSE.txt` & `dftt_timecode-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dftt_timecode-0.0.8/dftt_timecode/core.py` & `dftt_timecode-0.0.9/dftt_timecode/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     @InstanceMethodDispatch.register('__init__', str)  # 若传入的TC值为字符串，则调用此函数
     def _(self, timecode_value, timecode_type='auto', fps=24.0, drop_frame=False, strict=True):
         if timecode_value[0] == '-':  # 判断首位是否为负，并为flag赋值
             minus_flag = True
         else:
             minus_flag = False
         self.__fps = fps
-        self.__nominal_fps = ceil(fps)  # 读入帧率取整为名义帧率便于后续计算（包括判断时码是否合法，DF/NDF逻辑等）
+        self.__nominal_fps = ceil(fps)  # 读入帧率取整为名义帧率便于后续计算（包括判断时码是否合法，DF/NDF逻辑等) 用进一法是因为要判断ff值是否大于fps-1
         self.__drop_frame = drop_frame
         self.__strict = strict
         if round(self.__fps, 2) % 29.97 != 0 and self.__drop_frame == True:  # 判断丢帧状态与时码输入是否匹配 不匹配则强制转换
             self.__drop_frame = False
             logging.log(20, 'Timecode.__init__.str: This FPS is NOT Drop-Framable, force drop_frame to False')
         else:
             pass
@@ -97,14 +97,18 @@
                             self.__nominal_fps / 30) * 2 * (
                                           total_minutes - total_minutes // 10)  # 逢十分钟不丢帧 http://andrewduncan.net/timecodes/
             if self.__strict == True:  # strict输入逻辑
                 frame_index = frame_index % (self.__fps * 86400) if self.__drop_frame == True else frame_index % (
                         self.__nominal_fps * 86400)  # 对于DF时码来说，严格处理取真实FPS的模，对于NDF时码，则取名义FPS的模
             else:
                 pass
+            if minus_flag == False:
+                pass
+            else:
+                frame_index = -frame_index
             self.__precise_time = Fraction(frame_index / self.__fps)  # 时间戳=帧号/帧率
         elif timecode_type == 'srt':  # srt字幕
             if SRT_REGEX.match(timecode_value):  # 判断输入是否符合SRT类型
                 pass
             else:
                 logging.log(40, 'Timecode.__init__.srt: Timecode type DONOT match input value! Check input.')
                 raise DFTTTimecodeTypeError
@@ -114,15 +118,18 @@
             logging.log(20,
                         'Timecode.__init__.srt: SRT timecode framerate ' + str(self.__fps) + ', DF=' + str(
                             self.__drop_frame) + " assigned")
             hh = temp_timecode_list[0]
             mm = temp_timecode_list[1]
             ss = temp_timecode_list[2]
             sub_sec = temp_timecode_list[3]  # 取毫秒
-            self.__precise_time = Fraction(hh * 3600 + mm * 60 + ss + sub_sec / 1000)
+            if minus_flag == False:
+                self.__precise_time = (Fraction(hh * 3600 + mm * 60 + ss + sub_sec / 1000))
+            else:
+                self.__precise_time = -(Fraction(hh * 3600 + mm * 60 + ss + sub_sec / 1000))
             if self.__strict == True:  # strict逻辑 对于非帧相关值（时间戳） 直接取模
                 self.__precise_time = self.__precise_time % 86400
             else:
                 pass
         elif timecode_type == 'dlp':  # cinecanvas字幕
             if DLP_REGEX.match(timecode_value):
                 pass
@@ -136,15 +143,18 @@
                         'Timecode.__init__.dlp: DLP timecode framerate ' + str(self.__fps) + ', DF=' + str(
                             self.__drop_frame) + " assigned")
             hh = temp_timecode_list[0]
             mm = temp_timecode_list[1]
             ss = temp_timecode_list[2]
             sub_sec = temp_timecode_list[3]  # 取子帧戳 dlp每秒共250个子帧 即4ms一个
             # 详见https://interop-docs.cinepedia.com/Reference_Documents/CineCanvas(tm)_RevC.pdf 第17页 “TimeIn”部分
-            self.__precise_time = Fraction(hh * 3600 + mm * 60 + ss + sub_sec / 250)
+            if minus_flag == False:
+                self.__precise_time = Fraction(hh * 3600 + mm * 60 + ss + sub_sec / 250)
+            else:
+                self.__precise_time = -Fraction(hh * 3600 + mm * 60 + ss + sub_sec / 250)
             if self.__strict == True:  # strict逻辑 对于非帧相关值（时间戳） 直接取模
                 self.__precise_time = self.__precise_time % 86400
             else:
                 pass
         elif timecode_type == 'ffmpeg':  # ffmpeg时间
             if FFMPEG_REGEX.match(timecode_value):
                 pass
@@ -153,28 +163,35 @@
                 raise DFTTTimecodeTypeError
             self.__type = timecode_type
             temp_timecode_list = [int(x) if x else 0 for x in FFMPEG_REGEX.match(timecode_value).groups()]
             hh = temp_timecode_list[0]
             mm = temp_timecode_list[1]
             ss = temp_timecode_list[2]
             sub_sec = temp_timecode_list[3]
-            self.__precise_time = Fraction(hh * 3600 + mm * 60 + ss + float('0.{}'.format(sub_sec)))
+            if minus_flag == False:
+                self.__precise_time = Fraction(hh * 3600 + mm * 60 + ss + float('0.{}'.format(sub_sec)))
+            else:
+                self.__precise_time = -Fraction(hh * 3600 + mm * 60 + ss + float('0.{}'.format(sub_sec)))
             if self.__strict == True:  # strict逻辑 对于非帧相关值（时间戳） 直接取模
                 self.__precise_time = self.__precise_time % 86400
             else:
                 pass
         elif timecode_type == 'fcpx':  # fcpx xml时间戳
             if FCPX_REGEX.match(timecode_value):
                 pass
             else:
                 logging.log(40, 'Timecode.__init__.fcpx: Timecode type DONOT match input value! Check input.')
                 raise DFTTTimecodeTypeError
             self.__type = timecode_type
             temp_timecode_list = [int(x) if x else 0 for x in FCPX_REGEX.match(timecode_value).groups()]
-            self.__precise_time = Fraction(temp_timecode_list[0], temp_timecode_list[1])
+            print(temp_timecode_list[0])
+            if minus_flag == False:
+                self.__precise_time = Fraction(temp_timecode_list[0], temp_timecode_list[1])
+            else:
+                self.__precise_time = -Fraction(temp_timecode_list[0], temp_timecode_list[1])
             if self.__strict == True:  # strict逻辑 对于非帧相关值（时间戳） 直接取模
                 self.__precise_time = self.__precise_time % 86400
             else:
                 pass
         elif timecode_type == 'frame':  # 帧计数
             if FRAME_REGEX.match(timecode_value):
                 pass
@@ -200,15 +217,16 @@
             temp_timecode_value = TIME_REGEX.match(timecode_value).group(1)
             self.__precise_time = Fraction(temp_timecode_value)  # 内部时间戳直接等于输入值
             if self.__strict == True:  # strict逻辑 对于非帧相关值（时间戳） 直接取模
                 self.__precise_time = self.__precise_time % 86400
             else:
                 pass
         else:
-            logging.log(30, 'Timecode.__init__.str: Unknown Type, instancing default Timecode object.')
+            logging.log(30, 'Timecode.__init__.str: Unknown type or type DONOT match input value! Check input.')
+            raise DFTTTimecodeValueError
         instance_success_log = 'Timecode.__init__.str: Timecode instance, type=' + str(self.__type) + ', fps=' + str(
             self.__fps) + ', dropframe=' + str(self.__drop_frame) + ', strict=' + str(self.__strict)
         logging.log(10, instance_success_log)
 
     @InstanceMethodDispatch.register('__init__', Fraction)  # 输入为Fraction类分数，此时认为输入是时间戳，若不是，则会报错
     def _(self, timecode_value, timecode_type='time', fps=24.0, drop_frame=False, strict=True):
         if timecode_type in ('time', 'auto'):
@@ -228,18 +246,14 @@
         instance_success_log = 'Timecode.__init__.Fraction: Timecode instance, type=' + str(
             self.__type) + ', fps=' + str(
             self.__fps) + ', dropframe=' + str(self.__drop_frame) + ', strict=' + str(self.__strict)
         logging.log(10, instance_success_log)
 
     @InstanceMethodDispatch.register('__init__', int)
     def _(self, timecode_value, timecode_type='frame', fps=24.0, drop_frame=False, strict=True):
-        if timecode_value < 0:
-            minus_flag = True
-        else:
-            minus_flag = False
         if timecode_type in ('frame', 'auto'):
             self.__type = 'frame'
             self.__fps = fps
             self.__nominal_fps = ceil(fps)
             self.__drop_frame = drop_frame
             self.__strict = strict
             temp_frame_index = timecode_value
@@ -343,15 +357,19 @@
 
     @property
     def is_strict(self):
         return self.__strict
 
     @property
     def framecount(self):
-        return self._convert_to_output_frame()
+        return int(self._convert_to_output_frame())
+
+    @property
+    def timestamp(self):
+        return float(self._convert_to_output_time())
 
     def _convert_to_output_smpte(self, output_part=0):
         minus_flag = False
         frame_index = round(self.__precise_time * self.__fps)  # 从内部时间戳计算得帧计数
         if frame_index < 0:  # 负值时，打上flag，并翻转负号
             minus_flag = True
             frame_index = -frame_index
@@ -485,19 +503,18 @@
             return '{:03d}'.format(output_sub_sec)
 
     def _convert_to_output_fcpx(self, output_part=0):
         if output_part == 0:
             pass
         else:
             logging.log(30, '_convert_to_output_fcpx: This timecode type has only one part.')
-        return '{sign}{numerator}{denominator}s'.format(sign='' if self.__precise_time >= 0 else '-',
-                                                        numerator=self.__precise_time.numerator,
-                                                        denominator='' if float(
-                                                            self.__precise_time).is_integer() else '/{}'.format(
-                                                            self.__precise_time.denominator))
+        return '{numerator}{denominator}s'.format(numerator=self.__precise_time.numerator,
+                                                  denominator='' if float(
+                                                      self.__precise_time).is_integer() else '/{}'.format(
+                                                      self.__precise_time.denominator))
 
     def _convert_to_output_frame(self, output_part=0):
         if output_part == 0:
             pass
         else:
             logging.log(30, 'Timecode._convert_to_output_frame: This timecode type has only one part.')
         return str(round(self.__precise_time * self.__fps))
@@ -506,16 +523,19 @@
         if output_part == 0:
             pass
         else:
             logging.log(30, 'Timecode._convert_to_output_time: This timecode type has only one part.')
         output_time = round(float(self.__precise_time), 5)
         return str(output_time)
 
-    def timecode_output(self, dest_type='smpte', output_part=0):
-        func = getattr(self, '_convert_to_output_{}'.format(dest_type))
+    def timecode_output(self, dest_type='auto', output_part=0):
+        if dest_type == 'auto':
+            func = getattr(self, '_convert_to_output_{}'.format(self.__type))
+        else:
+            func = getattr(self, '_convert_to_output_{}'.format(dest_type))
         if func:
             return func(output_part)
         else:
             logging.log(30, 'Timecode.timecode_output: CANNOT find such destination type, will return SMPTE type')
             func = getattr(self, '_convert_to_output_smpte', None)
             return func(output_part)
 
@@ -544,20 +564,22 @@
     def set_strict(self, strict=True):
         if strict == self.__strict:
             pass
         else:
             temp_timecode_object = DfttTimecode(self.__precise_time, 'time', self.__fps, self.__drop_frame,
                                                 strict)
             self.__precise_time = temp_timecode_object.__precise_time
+            self.__strict = strict
         return self
 
     def __repr__(self):
-        return '<DfttTimecode>({}{}, {}{}, {}{:.02f} {})'.format('Time Stamp:', self.timecode_output('time'),
-                                                                 'Type:', self.__type, 'FPS:', float(self.__fps),
-                                                                 'DF' if self.__drop_frame == True else 'NDF')
+        return '<DfttTimecode>({}{}, {}{}, {}{:.02f} {}, {})'.format('Timecode:', self.timecode_output(self.__type),
+                                                                     'Type:', self.__type, 'FPS:', float(self.__fps),
+                                                                     'DF' if self.__drop_frame == True else 'NDF',
+                                                                     'Strict' if self.__strict == True else 'Non-Strict')
 
     def __add__(self, other):  # 运算符重载，加号，加int则认为是帧，加float则认为是时间
         temp_sum = self.__precise_time
         if isinstance(other, DfttTimecode):
             if self.__fps == other.__fps and self.__drop_frame == other.__drop_frame:
                 temp_sum = self.__precise_time + other.__precise_time
             else:  # 帧率不同不允许相加，返回前者的值
@@ -567,15 +589,17 @@
             temp_sum = self.__precise_time + (other / self.__fps)
         elif isinstance(other, float):  # 时间
             temp_sum = self.__precise_time + other
         elif isinstance(other, Fraction):  # 时间
             temp_sum = self.__precise_time + other
         else:
             logging.log(30, 'Timecode.__add__: Undefined addition, will return the former Timecode object.')
-        return DfttTimecode(temp_sum, 'time', self.__fps, self.__drop_frame, self.__strict)
+        temp_object = DfttTimecode(temp_sum, 'time', self.__fps, self.__drop_frame, self.__strict)
+        temp_object.set_type(self.type, rounding=False)
+        return temp_object
 
     def __radd__(self, other):  # 加法交换律
         return self.__add__(other)
 
     def __sub__(self, other):  # 运算符重载，减法，同理，int是帧，float是时间
         diff = self.__precise_time
         if isinstance(other, DfttTimecode):
@@ -589,61 +613,68 @@
             diff = self.__precise_time - other / self.__fps
         elif isinstance(other, float):  # 时间
             diff = self.__precise_time - other
         elif isinstance(other, Fraction):  # 时间
             diff = self.__precise_time - other
         else:
             logging.log(30, 'Timecode.__sub__: Undefined subtraction, will return the former Timecode object.')
-        return DfttTimecode(diff, 'time', self.__fps, self.__drop_frame, self.__strict)
+        temp_object = DfttTimecode(diff, 'time', self.__fps, self.__drop_frame, self.__strict)
+        temp_object.set_type(self.type, rounding=False)
+        return temp_object
 
     def __rsub__(self, other):  # 运算符重载，减法，同理，int是帧，float是时间
         diff = self.__precise_time
         if isinstance(other, int):  # 帧
             diff = other / self.__fps - self.__precise_time
         elif isinstance(other, float):  # 秒
             diff = other - self.__precise_time
         elif isinstance(other, Fraction):  # 时间
             diff = other - self.__precise_time
         else:
             logging.log(30, 'Timecode.__rsub__: Undefined subtraction, will return the latter Timecode object.')
-        return DfttTimecode(diff, 'time', self.__fps, self.__drop_frame, self.__strict)
+        temp_object = DfttTimecode(diff, 'time', self.__fps, self.__drop_frame, self.__strict)
+        temp_object.set_type(self.type, rounding=False)
+        return temp_object
 
     def __mul__(self, other):  # 运算符重载，乘法，int和float都是倍数
         prod = self.__precise_time
         if isinstance(other, DfttTimecode):
             logging.log(30,
                         'Timecode.__mul__: Timecode CANNOT multiply with another Timecode, will return the former Timecode object.')
         elif isinstance(other, int):
             prod = self.__precise_time * other
         elif isinstance(other, float):
             prod = self.__precise_time * other
         elif isinstance(other, Fraction):
             prod = self.__precise_time * other
         else:
             logging.log(30, 'Timecode.__mul__: Undefined multiplication, will return the former Timecode object.')
-        return DfttTimecode(prod, 'time', self.__fps, self.__drop_frame, self.__strict)
+        temp_object = DfttTimecode(prod, 'time', self.__fps, self.__drop_frame, self.__strict)
+        temp_object.set_type(self.type, rounding=False)
+        return temp_object
 
     def __rmul__(self, other):  # 乘法交换律
         return self.__mul__(other)
 
     def __truediv__(self, other):
         quo_time = self.__precise_time  # quo_time是商（时间戳）
         if isinstance(other, DfttTimecode):
             logging.log(30,
                         'Timecode.__truediv__: Timecode CANNOT be devided by another Timecode, will return the former Timecode object.')
         elif isinstance(other, int):  # timecode与数相除，得到结果是timecode
             quo_time = self.__precise_time / other
-            return DfttTimecode(quo_time, 'time', self.__fps, self.__drop_frame, self.__strict)
         elif isinstance(other, float):  # timecode与数相除，得到结果是timecode
             quo_time = self.__precise_time / other
         elif isinstance(other, Fraction):  # timecode与数相除，得到结果是timecode
             quo_time = self.__precise_time / other
         else:
             logging.log(30, 'Timecode.__truediv__: Undefined division, will return the former Timecode object.')
-        return DfttTimecode(quo_time, 'time', self.__fps, self.__drop_frame, self.__strict)
+        temp_object = DfttTimecode(quo_time, 'time', self.__fps, self.__drop_frame, self.__strict)
+        temp_object.set_type(self.type, rounding=False)
+        return temp_object
 
     def __rtruediv__(self, other):
         if isinstance(other, int) or isinstance(other, float) or isinstance(other, Fraction):
             logging.log(30,
                         'Timecode.__rtruediv__: Number CANNOT be devided by a Timecode, will return the Timecode object.')
         else:
             logging.log(30, 'Timecode.__rtruediv__: Undefined division, will return the latter Timecode object.')
@@ -714,8 +745,10 @@
         elif isinstance(other, Fraction):
             return round(self.__precise_time, 5) >= round(other, 5)
         else:
             logging.log(30, 'CANNOT compare with such data type, will return FALSE')
             return False
 
     def __neg__(self):  # 取负操作 返回时间戳取负的Timecode对象（strict规则照常应用 例如01:00:00:00 strict的对象 取负后为23:00:00:00）
-        return DfttTimecode(-self.__precise_time, self.__type, self.__fps, self.__drop_frame, self.__strict)
+        temp_object = DfttTimecode(-self.__precise_time, 'time', self.__fps, self.__drop_frame, self.__strict)
+        temp_object.set_type(self.type, rounding=False)
+        return temp_object
```

### Comparing `dftt_timecode-0.0.8/dftt_timecode/dispatch.py` & `dftt_timecode-0.0.9/dftt_timecode/dispatch.py`

 * *Files identical despite different names*

### Comparing `dftt_timecode-0.0.8/dftt_timecode/pattern.py` & `dftt_timecode-0.0.9/dftt_timecode/pattern.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # SMPTE全匹配 即SMPTE NDF与SMPTE DF的并集
 SRT_REGEX = re.compile(r'^(?:-)?(?:(?:(?:(\d\d{1}):){1}([0-5]?\d):){1}([0-5]?\d),){1}(\d\d\d){1}$')
 # SRT 形如01:23:45,678或-01:23:45,678
 FFMPEG_REGEX = re.compile(r'^(?:-)?(?:(?:(?:(\d\d{1}):){1}([0-5]?\d):){1}([0-5]?\d)\.){1}(\d?\d+){1}$')
 # FFMPEG 形如01:23:45.67或-01:23:45.67
 DLP_REGEX = re.compile(r'^(?:-)?(?:(?:(?:(\d\d{1}):){1}([0-5]?\d):){1}([0-5]?\d):){1}([0-2][0-4]\d{1}){1}$')
 # DLP 形如01:23:45:102或-01:23:45:102（末三位取值范围是0-249）
-FCPX_REGEX = re.compile(r'^(?:-)?(\d+)[/]?(\d+)?s$')
+FCPX_REGEX = re.compile(r'^(?:-)?(\d+)[/](\d+)?s$')
 # FCPX 形如1/24s或-1/24s s可有可无
 FRAME_REGEX = re.compile(r'^(-?\d+?)f?$')
 # 帧号 形如1234f或-1234f f可有可无
 TIME_REGEX = re.compile(r'^(-?\d+?(\.{1})\d+?|-?\d+?)s?$')
 # 时间戳 形如1234s或-1234.5s s可有可无
```

### Comparing `dftt_timecode-0.0.8/setup.py` & `dftt_timecode-0.0.9/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r",encoding='UTF-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="dftt_timecode",
-    version="0.0.8",
+    version="0.0.9",
     author="You Ziyuan",
     author_email="hikaridragon0216@gmail.com",
     description="Timecode library for film and TV industry, supports HFR and a bunch of cool features",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/OwenYou/dftt_timecode",
     packages=setuptools.find_packages(),
```

