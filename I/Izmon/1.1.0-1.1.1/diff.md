# Comparing `tmp/Izmon-1.1.0.tar.gz` & `tmp/Izmon-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Izmon-1.1.0.tar", last modified: Tue Apr 11 10:22:16 2023, max compression
+gzip compressed data, was "Izmon-1.1.1.tar", last modified: Sat Apr 15 08:28:32 2023, max compression
```

## Comparing `Izmon-1.1.0.tar` & `Izmon-1.1.1.tar`

### file list

```diff
@@ -1,50 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 10:22:16.000000 Izmon-1.1.0/
-drwxrwxrwx   0        0        0        0 2023-04-11 10:22:16.000000 Izmon-1.1.0/Izmon/
-drwxrwxrwx   0        0        0        0 2023-04-11 10:22:16.000000 Izmon-1.1.0/Izmon/Class/
-drwxrwxrwx   0        0        0        0 2023-04-11 10:22:16.000000 Izmon-1.1.0/Izmon/Class/Basic/
--rw-rw-rw-   0        0        0      738 2023-03-27 00:35:52.000000 Izmon-1.1.0/Izmon/Class/Basic/Common_Function.py
--rw-rw-rw-   0        0        0      860 2023-03-27 00:34:28.000000 Izmon-1.1.0/Izmon/Class/Basic/Common_Variable.py
--rw-rw-rw-   0        0        0     8849 2023-03-30 01:10:32.000000 Izmon-1.1.0/Izmon/Class/Basic/Settings.py
--rw-rw-rw-   0        0        0       14 2023-03-06 02:43:12.000000 Izmon-1.1.0/Izmon/Class/Basic/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-11 10:22:16.000000 Izmon-1.1.0/Izmon/Class/Battle/
--rw-rw-rw-   0        0        0     3733 2023-03-10 00:50:08.000000 Izmon-1.1.0/Izmon/Class/Battle/Battle.py
--rw-rw-rw-   0        0        0     2696 2023-03-27 01:57:28.000000 Izmon-1.1.0/Izmon/Class/Battle/Battle_Caluculate.py
--rw-rw-rw-   0        0        0     2638 2023-03-05 23:44:30.000000 Izmon-1.1.0/Izmon/Class/Battle/Battle_Other.py
--rw-rw-rw-   0        0        0     2628 2023-03-06 04:02:18.000000 Izmon-1.1.0/Izmon/Class/Battle/Battle_Set.py
--rw-rw-rw-   0        0        0       15 2023-03-06 02:43:30.000000 Izmon-1.1.0/Izmon/Class/Battle/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-11 10:22:16.000000 Izmon-1.1.0/Izmon/Class/CloudSave/
--rw-rw-rw-   0        0        0      791 2023-03-29 11:33:42.000000 Izmon-1.1.0/Izmon/Class/CloudSave/Common.py
--rw-rw-rw-   0        0        0     1194 2023-04-02 04:40:40.000000 Izmon-1.1.0/Izmon/Class/CloudSave/Download.py
--rw-rw-rw-   0        0        0     1263 2023-04-02 04:40:08.000000 Izmon-1.1.0/Izmon/Class/CloudSave/Upload.py
--rw-rw-rw-   0        0        0       18 2023-04-11 10:17:56.000000 Izmon-1.1.0/Izmon/Class/CloudSave/__init__.py
--rw-rw-rw-   0        0        0     1355 2023-03-06 10:15:46.000000 Izmon-1.1.0/Izmon/Class/Dictionary.py
-drwxrwxrwx   0        0        0        0 2023-04-11 10:22:16.000000 Izmon-1.1.0/Izmon/Class/Events/
--rw-rw-rw-   0        0        0      313 2023-03-05 08:36:34.000000 Izmon-1.1.0/Izmon/Class/Events/Events_Latest.py
--rw-rw-rw-   0        0        0        0 2023-03-01 05:47:34.000000 Izmon-1.1.0/Izmon/Class/Events/Events_Passed.py
--rw-rw-rw-   0        0        0       15 2023-03-06 02:43:42.000000 Izmon-1.1.0/Izmon/Class/Events/__init__.py
--rw-rw-rw-   0        0        0     4778 2023-03-27 02:18:00.000000 Izmon-1.1.0/Izmon/Class/Gym.py
-drwxrwxrwx   0        0        0        0 2023-04-11 10:22:16.000000 Izmon-1.1.0/Izmon/Class/Save_Code/
--rw-rw-rw-   0        0        0     1601 2023-03-27 03:08:20.000000 Izmon-1.1.0/Izmon/Class/Save_Code/Decode.py
--rw-rw-rw-   0        0        0     1177 2023-03-09 04:41:52.000000 Izmon-1.1.0/Izmon/Class/Save_Code/Encode.py
--rw-rw-rw-   0        0        0       18 2023-03-06 02:43:56.000000 Izmon-1.1.0/Izmon/Class/Save_Code/__init__.py
--rw-rw-rw-   0        0        0     2153 2023-03-27 03:13:26.000000 Izmon-1.1.0/Izmon/Class/Set.py
-drwxrwxrwx   0        0        0        0 2023-04-11 10:22:16.000000 Izmon-1.1.0/Izmon/Class/Start_End/
--rw-rw-rw-   0        0        0     1779 2023-04-01 02:50:02.000000 Izmon-1.1.0/Izmon/Class/Start_End/End.py
--rw-rw-rw-   0        0        0     4895 2023-04-01 23:28:28.000000 Izmon-1.1.0/Izmon/Class/Start_End/Start.py
--rw-rw-rw-   0        0        0       18 2023-03-06 02:44:10.000000 Izmon-1.1.0/Izmon/Class/Start_End/__init__.py
--rw-rw-rw-   0        0        0       64 2023-03-06 09:47:24.000000 Izmon-1.1.0/Izmon/Class/__init__.py
--rw-rw-rw-   0        0        0      281 2023-03-30 01:10:42.000000 Izmon-1.1.0/Izmon/Class/setup.py
--rw-rw-rw-   0        0        0     1506 2023-04-11 10:21:52.000000 Izmon-1.1.0/Izmon/Main.py
--rw-rw-rw-   0        0        0       64 2023-03-06 10:08:06.000000 Izmon-1.1.0/Izmon/__init__.py
--rw-rw-rw-   0        0        0      295 2023-03-30 01:10:38.000000 Izmon-1.1.0/Izmon/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-11 10:22:16.000000 Izmon-1.1.0/Izmon.egg-info/
--rw-rw-rw-   0        0        0      980 2023-04-11 10:22:16.000000 Izmon-1.1.0/Izmon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1059 2023-04-11 10:22:16.000000 Izmon-1.1.0/Izmon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 10:22:16.000000 Izmon-1.1.0/Izmon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-11 10:22:16.000000 Izmon-1.1.0/Izmon.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-11 10:22:16.000000 Izmon-1.1.0/Izmon.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      634 2023-03-02 11:44:52.000000 Izmon-1.1.0/LICENSE.txt
--rw-rw-rw-   0        0        0      980 2023-04-11 10:22:18.000000 Izmon-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      492 2023-03-06 05:47:12.000000 Izmon-1.1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-04-11 10:22:18.000000 Izmon-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      743 2023-04-11 10:05:32.000000 Izmon-1.1.0/setup.py
+drwxr-xr-x   0 yohei      (504) staff       (20)        0 2023-04-15 08:28:32.361338 Izmon-1.1.1/
+drwxr-xr-x   0 yohei      (504) staff       (20)        0 2023-04-15 08:28:32.268688 Izmon-1.1.1/Izmon/
+drwxr-xr-x   0 yohei      (504) staff       (20)        0 2023-04-15 08:28:32.283595 Izmon-1.1.1/Izmon/Class/
+drwxr-xr-x   0 yohei      (504) staff       (20)        0 2023-04-15 08:28:32.293218 Izmon-1.1.1/Izmon/Class/Basic/
+-rwxrwxrwx   0 yohei      (504) staff       (20)      738 2023-03-27 00:35:52.000000 Izmon-1.1.1/Izmon/Class/Basic/Common_Function.py
+-rwxrwxrwx   0 yohei      (504) staff       (20)      859 2023-04-14 12:09:48.000000 Izmon-1.1.1/Izmon/Class/Basic/Common_Variable.py
+-rwxrwxrwx   0 yohei      (504) staff       (20)     8906 2023-04-14 12:19:57.000000 Izmon-1.1.1/Izmon/Class/Basic/Settings.py
+-rwxrwxrwx   0 yohei      (504) staff       (20)       14 2023-03-06 02:43:12.000000 Izmon-1.1.1/Izmon/Class/Basic/__init__.py
+drwxr-xr-x   0 yohei      (504) staff       (20)        0 2023-04-15 08:28:32.326196 Izmon-1.1.1/Izmon/Class/Battle/
+-rwxrwxrwx   0 yohei      (504) staff       (20)     3733 2023-03-10 00:50:08.000000 Izmon-1.1.1/Izmon/Class/Battle/Battle.py
+-rwxrwxrwx   0 yohei      (504) staff       (20)     2696 2023-03-27 01:57:28.000000 Izmon-1.1.1/Izmon/Class/Battle/Battle_Caluculate.py
+-rwxrwxrwx   0 yohei      (504) staff       (20)     2638 2023-03-05 23:44:30.000000 Izmon-1.1.1/Izmon/Class/Battle/Battle_Other.py
+-rwxrwxrwx   0 yohei      (504) staff       (20)     2628 2023-03-06 04:02:18.000000 Izmon-1.1.1/Izmon/Class/Battle/Battle_Set.py
+-rwxrwxrwx   0 yohei      (504) staff       (20)       15 2023-03-06 02:43:30.000000 Izmon-1.1.1/Izmon/Class/Battle/__init__.py
+-rwxrwxrwx   0 yohei      (504) staff       (20)     1355 2023-03-06 10:15:46.000000 Izmon-1.1.1/Izmon/Class/Dictionary.py
+drwxr-xr-x   0 yohei      (504) staff       (20)        0 2023-04-15 08:28:32.336728 Izmon-1.1.1/Izmon/Class/Events/
+-rwxrwxrwx   0 yohei      (504) staff       (20)      313 2023-03-05 08:36:34.000000 Izmon-1.1.1/Izmon/Class/Events/Events_Latest.py
+-rwxrwxrwx   0 yohei      (504) staff       (20)        0 2023-03-01 05:47:34.000000 Izmon-1.1.1/Izmon/Class/Events/Events_Passed.py
+-rwxrwxrwx   0 yohei      (504) staff       (20)       15 2023-03-06 02:43:42.000000 Izmon-1.1.1/Izmon/Class/Events/__init__.py
+-rwxrwxrwx   0 yohei      (504) staff       (20)     4778 2023-04-12 11:12:48.000000 Izmon-1.1.1/Izmon/Class/Gym.py
+drwxr-xr-x   0 yohei      (504) staff       (20)        0 2023-04-15 08:28:32.347166 Izmon-1.1.1/Izmon/Class/Save_Code/
+-rwxrwxrwx   0 yohei      (504) staff       (20)     1601 2023-03-27 03:08:20.000000 Izmon-1.1.1/Izmon/Class/Save_Code/Decode.py
+-rwxrwxrwx   0 yohei      (504) staff       (20)     1177 2023-03-09 04:41:52.000000 Izmon-1.1.1/Izmon/Class/Save_Code/Encode.py
+-rwxrwxrwx   0 yohei      (504) staff       (20)       18 2023-03-06 02:43:56.000000 Izmon-1.1.1/Izmon/Class/Save_Code/__init__.py
+-rwxrwxrwx   0 yohei      (504) staff       (20)     2153 2023-03-27 03:13:26.000000 Izmon-1.1.1/Izmon/Class/Set.py
+drwxr-xr-x   0 yohei      (504) staff       (20)        0 2023-04-15 08:28:32.354548 Izmon-1.1.1/Izmon/Class/Start_End/
+-rwxrwxrwx   0 yohei      (504) staff       (20)     2135 2023-04-14 12:27:14.000000 Izmon-1.1.1/Izmon/Class/Start_End/End.py
+-rwxrwxrwx   0 yohei      (504) staff       (20)     5275 2023-04-14 12:25:52.000000 Izmon-1.1.1/Izmon/Class/Start_End/Start.py
+-rwxrwxrwx   0 yohei      (504) staff       (20)       18 2023-03-06 02:44:10.000000 Izmon-1.1.1/Izmon/Class/Start_End/__init__.py
+-rwxrwxrwx   0 yohei      (504) staff       (20)       64 2023-03-06 09:47:24.000000 Izmon-1.1.1/Izmon/Class/__init__.py
+-rwxrwxrwx   0 yohei      (504) staff       (20)      281 2023-03-30 01:10:43.000000 Izmon-1.1.1/Izmon/Class/setup.py
+-rwxrwxrwx   0 yohei      (504) staff       (20)     1513 2023-04-14 12:01:37.000000 Izmon-1.1.1/Izmon/Main.py
+-rwxrwxrwx   0 yohei      (504) staff       (20)       64 2023-03-06 10:08:06.000000 Izmon-1.1.1/Izmon/__init__.py
+-rwxrwxrwx   0 yohei      (504) staff       (20)      280 2023-04-14 11:24:09.000000 Izmon-1.1.1/Izmon/setup.py
+drwxr-xr-x   0 yohei      (504) staff       (20)        0 2023-04-15 08:28:32.273651 Izmon-1.1.1/Izmon.egg-info/
+-rw-r--r--   0 yohei      (504) staff       (20)     1024 2023-04-15 08:28:32.000000 Izmon-1.1.1/Izmon.egg-info/PKG-INFO
+-rw-r--r--   0 yohei      (504) staff       (20)      899 2023-04-15 08:28:32.000000 Izmon-1.1.1/Izmon.egg-info/SOURCES.txt
+-rw-r--r--   0 yohei      (504) staff       (20)        1 2023-04-15 08:28:32.000000 Izmon-1.1.1/Izmon.egg-info/dependency_links.txt
+-rw-r--r--   0 yohei      (504) staff       (20)        6 2023-04-15 08:28:32.000000 Izmon-1.1.1/Izmon.egg-info/top_level.txt
+-rwxrwxrwx   0 yohei      (504) staff       (20)      634 2023-03-02 11:44:52.000000 Izmon-1.1.1/LICENSE.txt
+-rw-r--r--   0 yohei      (504) staff       (20)     1024 2023-04-15 08:28:32.360697 Izmon-1.1.1/PKG-INFO
+-rwxrwxrwx   0 yohei      (504) staff       (20)      492 2023-03-06 05:47:12.000000 Izmon-1.1.1/README.md
+-rw-r--r--   0 yohei      (504) staff       (20)       38 2023-04-15 08:28:32.361567 Izmon-1.1.1/setup.cfg
+-rwxrwxrwx   0 yohei      (504) staff       (20)      877 2023-04-14 11:23:57.000000 Izmon-1.1.1/setup.py
```

### Comparing `Izmon-1.1.0/Izmon/Class/Basic/Common_Function.py` & `Izmon-1.1.1/Izmon/Class/Basic/Common_Function.py`

 * *Files identical despite different names*

### Comparing `Izmon-1.1.0/Izmon/Class/Basic/Common_Variable.py` & `Izmon-1.1.1/Izmon/Class/Basic/Common_Variable.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -25,8 +25,8 @@
 	
 	player_name = ""
 
 	badges = [0, 0, 0, 0, 0, 0]
 
 	num_killed = 0
 
-	show_length = 4
+	show_length = 4
```

### Comparing `Izmon-1.1.0/Izmon/Class/Basic/Settings.py` & `Izmon-1.1.1/Izmon/Class/Basic/Settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 	・PARTY_NUM
 	・LEVELUP_NUM (桁数)
 	・CODE_FELLOW_LEN
 	以上の 4 定数の " いずれか " を変更する際はコード と メジャーバージョンの変更が必要
 	'''
 
 	#バージョン
-	VERSION = '1.1.0'
+	VERSION = '1.1.1'
 	
 	#イズモンの数
 	IZ_NUM = 80
 
 	#イズモン設定一覧
 	IZUMON_SETTING = [[1 , "サーファー", 0, 162, 80, 115, 153, 111, 0.4, 0], [2 , "キョーリュー", 0, 166, 154, 115, 120, 120, 0.2, 0],
 					[3 , "ササントラ", 1, 167, 125, 110, 145, 110, 0.2, 0], [4 , "トラパルト", 2, 163, 140, 95, 120, 95, 0.2, 0],
@@ -132,7 +132,10 @@
 	IZMON_P_LEN = 95
 
 	#データの保存の際の桁数
 	CODE_CAP = 100
 
 	#10進数に仲間のデータを変換した時の桁数
 	CODE_FELLOW_LEN = 31
+
+	#クラウドセーブ再試行時の間隔
+	RETRY = 15
```

### Comparing `Izmon-1.1.0/Izmon/Class/Battle/Battle.py` & `Izmon-1.1.1/Izmon/Class/Battle/Battle.py`

 * *Files identical despite different names*

### Comparing `Izmon-1.1.0/Izmon/Class/Battle/Battle_Caluculate.py` & `Izmon-1.1.1/Izmon/Class/Battle/Battle_Caluculate.py`

 * *Files identical despite different names*

### Comparing `Izmon-1.1.0/Izmon/Class/Battle/Battle_Other.py` & `Izmon-1.1.1/Izmon/Class/Battle/Battle_Other.py`

 * *Files identical despite different names*

### Comparing `Izmon-1.1.0/Izmon/Class/Battle/Battle_Set.py` & `Izmon-1.1.1/Izmon/Class/Battle/Battle_Set.py`

 * *Files identical despite different names*

### Comparing `Izmon-1.1.0/Izmon/Class/Dictionary.py` & `Izmon-1.1.1/Izmon/Class/Dictionary.py`

 * *Files identical despite different names*

### Comparing `Izmon-1.1.0/Izmon/Class/Gym.py` & `Izmon-1.1.1/Izmon/Class/Gym.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 		action = self.co_f.typing(f"どのジムリーダーと戦うのじゃ？( {str(leadar_len)} でやめる)", 1, leadar_len)
 		if action == leadar_len:
 			self.co_f.show("やめるのじゃな")
 			return
 		leadar = self.st.GYM_DEFAULT[action]
 		gym_num = len(leadar)
 		for i in range(gym_num):
-			self.hp_me[i] = self.st.IZUMON_SETTING[self.co_f.party[i]][3]
+			self.hp_me[i] = self.st.IZUMON_SETTING[self.co_v.party[i]][3]
 		for i in range(gym_num):
 			
 			res = self.bat.battle(leadar[i] - 1, 1)
 			if res == 0:
 				self.co_f.show("またチャレンジするんじゃぞ")
 				break
 			elif res == 1 and i != gym_num:
```

### Comparing `Izmon-1.1.0/Izmon/Class/Save_Code/Decode.py` & `Izmon-1.1.1/Izmon/Class/Save_Code/Decode.py`

 * *Files identical despite different names*

### Comparing `Izmon-1.1.0/Izmon/Class/Save_Code/Encode.py` & `Izmon-1.1.1/Izmon/Class/Save_Code/Encode.py`

 * *Files identical despite different names*

### Comparing `Izmon-1.1.0/Izmon/Class/Set.py` & `Izmon-1.1.1/Izmon/Class/Set.py`

 * *Files identical despite different names*

### Comparing `Izmon-1.1.0/Izmon/Class/Start_End/End.py` & `Izmon-1.1.1/Izmon/Class/Start_End/End.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 class End:
 	from ..Basic.Common_Function import Common_Function as co_f
 	from ..Basic.Common_Variable import Common_Variable as co_v
 	from ..Basic.Settings import Settings as st
+	import datetime as dt
+	import time
 	
 	def main(self): #データをセーブする		
 		ty = self.co_f.typing("データをセーブしますか？ 0:する 1:しない", 1, 2)
 		print("~" * self.st.SEPALATE_LEN)
 		if ty == 0:
 			self.save()
 		else:
@@ -16,31 +18,42 @@
 		print("=" * self.st.SEPALATE_LEN)
 		return
 	
 	def save(self):
 		from ..Save_Code.Encode import Encode
 		from ..CloudSave.Upload import Upload as u
 		code = Encode.encode()
+		rem = 0
 		ty = self.co_f.typing("クラウドセーブを利用しますか？(事前登録が必要です) 0:利用する 1:利用しない", 1, 2)
 		print("~注意事項~")
 		print("データは上書きされます。上書きしたくない場合は新たにアカウントを作成してください。")
 		if ty == 0:
 			while True:
-				print("~" * self.st.SEPALATE_LEN)
+				if self.co_v.retry != 0:
+					rem = rem - self.dt.datetime.now()
+					rem = int(rem.total_seconds() + 0.5)
+				else:
+					rem = 0
 				u_name = self.co_f.typing("ユーザー名", 0)
 				pas = self.co_f.typing("パスワード", 0)
 				print("~" * self.st.SEPALATE_LEN)
+
+				self.time.sleep(rem) #待機時間
+				if rem != 0:
+						print(f"再試行されるまで{rem}秒お待ちください。")
 				res = u.upload(u_name, pas, code)
+				
 				if res[0]:
 					print("正常に保存されました。")
 					break
 				else:
 					print(res[1])
 					ty = self.co_f.typing("再試行しますか？ 0:する 1:しない(コードは表示されます)", 1, 2)
 					print("~" * self.st.SEPALATE_LEN)
 					if ty == 0:
-						continue
+						now = self.dt.datetime.now()
+						rem = now + self.dt.timedelta(seconds=self.st.RETRY)
 					else:
 						print("-" * self.st.SEPALATE_LEN)
 						print("プレイヤー名と共に保管してください。")
 						print(f"コード: {code}")
 						print(f"プレイヤー名: {self.co_v.player_name}")
```

### Comparing `Izmon-1.1.0/Izmon/Class/Start_End/Start.py` & `Izmon-1.1.1/Izmon/Class/Start_End/Start.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 class Start:
 	from ..Basic.Common_Function import Common_Function as co_f
 	from ..Basic.Common_Variable import Common_Variable as co_v
 	from ..Basic.Settings import Settings as st
 	from ..Battle.Battle_Caluculate import Battle_Caluculate
 	from ..Gym import Gym
+	import datetime as dt
+	import time
 
 	gym = Gym(); bat_cal = Battle_Caluculate
 	
 	MSG_SELECT = ["イズットモンスターの世界へ ようこそ！ わしの名前は オーキ二 みんなからは イズモン はかせと 慕われておるよ ",
 	"イズットモンスター………イズモン この 世界には イズットモンスターと 呼ばれる いきもの達が いたる所に 住んでいる! ",
 	"人は イズモンたちと 仲良く遊んだり 一緒に戦ったり………… 助け合いながら 暮らしているのじゃ ",
 	"しかし わしらは イズモンの全てを 知っている 訳ではない イズモンの 秘密は まだまだ いっぱい ある！ ",
@@ -19,29 +21,40 @@
 	" ! 準備は いいかな？ いよいよ これから きみの 物語が 始まる！ ",
 	"楽しいことも 苦しいことも いっぱい きみを 待っているだろう！ 夢と 冒険と！ ",
 	"イズットモンスターの 世界へ！ レッツ ゴー"]
 
 	def set_up(self): #開始する
 		from ..Save_Code.Decode import Decode
 		from ..CloudSave.Download import Download as d
+		rem = 0
 		print("イズットモンスター(Ver", self.st.VERSION, ")")
 		ty = self.co_f.typing("0:はじめから 1:続きから", 1, 2)
 		self.co_f.show("=" * self.st.SEPALATE_LEN, 0)
 		if ty == 0:
 			self.select_izmon()
 		else:
 				ty = self.co_f.typing("クラウドからロードしますか？ 0:する 1:しない", 1, 2)
 				if ty == 0:
 					while True:
 						print("~" * self.st.SEPALATE_LEN)
+						if rem != 0:
+							rem = rem - self.dt.datetime.now()
+							rem = int(rem.total_seconds() + 0.5)
+						else:
+							rem = 0
+						print(rem)
 						u_name = self.co_f.typing("ユーザー名", 0)
 						pas = self.co_f.typing("パスワード", 0)
 						print("~" * self.st.SEPALATE_LEN)
-						status = d.download(u_name, pas)
-						res = status[0]; code = status[1]; name = status[2]
+
+						if rem != 0:
+							print(f"再試行されるまで{rem}秒お待ちください。")
+						self.time.sleep(rem) #待機時間
+
+						res, code, name = d.download(u_name, pas)
 						if res:
 							print("正常にダウンロードされました。")
 							self.co_v.player_name = name
 							res = Decode.decode(code)
 							if res == 1:
 								print("~" * self.st.SEPALATE_LEN)
 								print("無効なコードじゃ。不正はダメじゃぞ")
@@ -52,14 +65,16 @@
 								break
 						else:
 							print(code)
 							print("~" * self.st.SEPALATE_LEN)
 							ty = self.co_f.typing("再試行しますか？ 0:する 1:しない(手動でロードできます)", 1, 2)
 							print("~" * self.st.SEPALATE_LEN)
 							if ty == 0:
+								now = self.dt.datetime.now()
+								rem = now + self.dt.timedelta(seconds=self.st.RETRY)
 								continue
 							else:
 								self.manual()
 				else:
 					self.manual()
 					
 	def select_izmon(self): #開始時のイズモンを選択
```

### Comparing `Izmon-1.1.0/Izmon/Main.py` & `Izmon-1.1.1/Izmon/Main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 def main():
-	# from Class.Basic.Common_Function import Common_Function as co_f
-	# from Class.Gym import Gym
-	# from Class.Dictionary import Dictionary as dic
-	# from Class.Events.Events_Latest import Events_Latest as ev
-	# from Class.Start_End.Start import Start
-	# from Class.Start_End.End import End
-	# from Class.Set import Set
-	# from Class.Battle.Battle_Set import Battle_Set as bat_s
-	# from Class.Battle.Battle import Battle as ba
-	from Izmon.Class.Basic.Common_Function import Common_Function as co_f
-	from Izmon.Class.Gym import Gym
-	from Izmon.Class.Dictionary import Dictionary as dic
-	from Izmon.Class.Events.Events_Latest import Events_Latest as ev
-	from Izmon.Class.Start_End.Start import Start
-	from Izmon.Class.Start_End.End import End
-	from Izmon.Class.Set import Set
-	from Izmon.Class.Battle.Battle_Set import Battle_Set as bat_s
-	from Izmon.Class.Battle.Battle import Battle as ba
+	from Class.Basic.Common_Function import Common_Function as co_f
+	from Class.Gym import Gym
+	from Class.Dictionary import Dictionary as dic
+	from Class.Events.Events_Latest import Events_Latest as ev
+	from Class.Start_End.Start import Start
+	from Class.Start_End.End import End
+	from Class.Set import Set
+	from Class.Battle.Battle_Set import Battle_Set as bat_s
+	from Class.Battle.Battle import Battle as ba
+	# from Izmon.Class.Basic.Common_Function import Common_Function as co_f
+	# from Izmon.Class.Gym import Gym
+	# from Izmon.Class.Dictionary import Dictionary as dic
+	# from Izmon.Class.Events.Events_Latest import Events_Latest as ev
+	# from Izmon.Class.Start_End.Start import Start
+	# from Izmon.Class.Start_End.End import End
+	# from Izmon.Class.Set import Set
+	# from Izmon.Class.Battle.Battle_Set import Battle_Set as bat_s
+	# from Izmon.Class.Battle.Battle import Battle as ba
 	gym = Gym(); start = Start(); end = End(); set = Set()
 	start.set_up()
 	while True:
 		action = co_f.typing("どうしますか? 0:バトルする 1:ジムに行く 2:イズモン辞典 3:イベント 4:設定 5:やめる", 1, 6)
 		if action == 0:
 			enemy = bat_s.select_ene()
 			ba.battle(enemy, 0)
@@ -34,8 +34,9 @@
 			set.main()
 		elif action ==5:
 			action = co_f.typing("本当にやめますか? 0:やめる 1:続ける", 1, 2)
 			if action == 0:
 				break
 			else:
 				continue
-	end.main()
+	end.main()
+main()
```

### Comparing `Izmon-1.1.0/Izmon.egg-info/PKG-INFO` & `Izmon-1.1.1/Izmon.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,30 @@
-Metadata-Version: 2.1
-Name: Izmon
-Version: 1.1.0
-Summary: You can play Izmon with this libraly.
-Home-page: https://github.com/akita0724
-Author: Yohei Akita, nabe, miso
-Author-email: akita.yohei0724@gmail.com
-License: GPLv2
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-This software is released under the GPL, see LICENSE.
-
-To play izmon, you need to take 3 steps below.
-
-1. install this library
-2. import this library( from Izmon import Main )
-3. run script( Main.main() )
-
-To get more information about Izmon or learn about the specification of Izmon or contact us,
-please look at the official reference ↓ (all of them are written in Japanese).
-https://docs.google.com/spreadsheets/d/1bX43X_iltZBGkd1p2V-UCpBOe-Mpj0kI1CqSpalVTo4/
-
-2023/03/02 akita nabe miso
+Metadata-Version: 2.1
+Name: Izmon
+Version: 1.1.1
+Summary: You can play Izmon with this libraly.
+Home-page: https://github.com/akita0724
+Author: Yohei Akita, nabe, miso
+Author-email: akita.yohei0724@gmail.com
+License: GPL v2.0
+Keywords: Izmon
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
+Classifier: Operating System :: OS Independent
+Requires: requests
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+This software is released under the GPL, see LICENSE.
+
+To play izmon, you need to take 3 steps below.
+
+1. install this library
+2. import this library( from Izmon import Main )
+3. run script( Main.main() )
+
+To get more information about Izmon or learn about the specification of Izmon or contact us,
+please look at the official reference ↓ (all of them are written in Japanese).
+https://docs.google.com/spreadsheets/d/1bX43X_iltZBGkd1p2V-UCpBOe-Mpj0kI1CqSpalVTo4/
+
+2023/03/02 akita nabe miso
```

### Comparing `Izmon-1.1.0/Izmon.egg-info/SOURCES.txt` & `Izmon-1.1.1/Izmon.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 setup.py
 Izmon/Main.py
 Izmon/__init__.py
 Izmon/setup.py
 Izmon.egg-info/PKG-INFO
 Izmon.egg-info/SOURCES.txt
 Izmon.egg-info/dependency_links.txt
-Izmon.egg-info/requires.txt
 Izmon.egg-info/top_level.txt
 Izmon/Class/Dictionary.py
 Izmon/Class/Gym.py
 Izmon/Class/Set.py
 Izmon/Class/__init__.py
 Izmon/Class/setup.py
 Izmon/Class/Basic/Common_Function.py
@@ -19,18 +18,14 @@
 Izmon/Class/Basic/Settings.py
 Izmon/Class/Basic/__init__.py
 Izmon/Class/Battle/Battle.py
 Izmon/Class/Battle/Battle_Caluculate.py
 Izmon/Class/Battle/Battle_Other.py
 Izmon/Class/Battle/Battle_Set.py
 Izmon/Class/Battle/__init__.py
-Izmon/Class/CloudSave/Common.py
-Izmon/Class/CloudSave/Download.py
-Izmon/Class/CloudSave/Upload.py
-Izmon/Class/CloudSave/__init__.py
 Izmon/Class/Events/Events_Latest.py
 Izmon/Class/Events/Events_Passed.py
 Izmon/Class/Events/__init__.py
 Izmon/Class/Save_Code/Decode.py
 Izmon/Class/Save_Code/Encode.py
 Izmon/Class/Save_Code/__init__.py
 Izmon/Class/Start_End/End.py
```

### Comparing `Izmon-1.1.0/LICENSE.txt` & `Izmon-1.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Izmon-1.1.0/PKG-INFO` & `Izmon-1.1.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,30 @@
-Metadata-Version: 2.1
-Name: Izmon
-Version: 1.1.0
-Summary: You can play Izmon with this libraly.
-Home-page: https://github.com/akita0724
-Author: Yohei Akita, nabe, miso
-Author-email: akita.yohei0724@gmail.com
-License: GPLv2
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-This software is released under the GPL, see LICENSE.
-
-To play izmon, you need to take 3 steps below.
-
-1. install this library
-2. import this library( from Izmon import Main )
-3. run script( Main.main() )
-
-To get more information about Izmon or learn about the specification of Izmon or contact us,
-please look at the official reference ↓ (all of them are written in Japanese).
-https://docs.google.com/spreadsheets/d/1bX43X_iltZBGkd1p2V-UCpBOe-Mpj0kI1CqSpalVTo4/
-
-2023/03/02 akita nabe miso
+Metadata-Version: 2.1
+Name: Izmon
+Version: 1.1.1
+Summary: You can play Izmon with this libraly.
+Home-page: https://github.com/akita0724
+Author: Yohei Akita, nabe, miso
+Author-email: akita.yohei0724@gmail.com
+License: GPL v2.0
+Keywords: Izmon
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
+Classifier: Operating System :: OS Independent
+Requires: requests
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+This software is released under the GPL, see LICENSE.
+
+To play izmon, you need to take 3 steps below.
+
+1. install this library
+2. import this library( from Izmon import Main )
+3. run script( Main.main() )
+
+To get more information about Izmon or learn about the specification of Izmon or contact us,
+please look at the official reference ↓ (all of them are written in Japanese).
+https://docs.google.com/spreadsheets/d/1bX43X_iltZBGkd1p2V-UCpBOe-Mpj0kI1CqSpalVTo4/
+
+2023/03/02 akita nabe miso
```

