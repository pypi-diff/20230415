# Comparing `tmp/projectZ.py-1.1.6.7.tar.gz` & `tmp/projectZ.py-1.1.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "projectZ.py-1.1.6.7.tar", last modified: Thu Apr 13 17:38:51 2023, max compression
+gzip compressed data, was "projectZ.py-1.1.6.8.tar", last modified: Sat Apr 15 19:43:34 2023, max compression
```

## Comparing `projectZ.py-1.1.6.7.tar` & `projectZ.py-1.1.6.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 17:38:51.877354 projectZ.py-1.1.6.7/
--rw-rw-rw-   0        0        0     2779 2023-04-13 17:38:51.878355 projectZ.py-1.1.6.7/PKG-INFO
--rw-rw-rw-   0        0        0     1777 2023-03-16 22:32:28.000000 projectZ.py-1.1.6.7/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 17:38:51.833728 projectZ.py-1.1.6.7/projectZ/
--rw-rw-rw-   0        0        0      748 2023-04-13 17:36:05.000000 projectZ.py-1.1.6.7/projectZ/__init__.py
--rw-rw-rw-   0        0        0    32362 2023-04-13 17:24:01.000000 projectZ.py-1.1.6.7/projectZ/async_client.py
--rw-rw-rw-   0        0        0     8713 2023-04-01 11:49:21.000000 projectZ.py-1.1.6.7/projectZ/async_socket.py
--rw-rw-rw-   0        0        0    28645 2023-04-13 17:30:53.000000 projectZ.py-1.1.6.7/projectZ/client.py
--rw-rw-rw-   0        0        0     9048 2023-04-10 10:03:57.000000 projectZ.py-1.1.6.7/projectZ/socket.py
-drwxrwxrwx   0        0        0        0 2023-04-13 17:38:51.876354 projectZ.py-1.1.6.7/projectZ/utils/
--rw-rw-rw-   0        0        0        0 2023-02-06 18:57:12.000000 projectZ.py-1.1.6.7/projectZ/utils/__init__.py
--rw-rw-rw-   0        0        0     1724 2023-04-01 11:47:12.000000 projectZ.py-1.1.6.7/projectZ/utils/exceptions.py
--rw-rw-rw-   0        0        0     2674 2023-03-17 11:05:21.000000 projectZ.py-1.1.6.7/projectZ/utils/generator.py
--rw-rw-rw-   0        0        0      985 2023-02-18 18:34:23.000000 projectZ.py-1.1.6.7/projectZ/utils/headers.py
--rw-rw-rw-   0        0        0    21006 2023-03-25 23:39:28.000000 projectZ.py-1.1.6.7/projectZ/utils/objects.py
-drwxrwxrwx   0        0        0        0 2023-04-13 17:38:51.861721 projectZ.py-1.1.6.7/projectZ.py.egg-info/
--rw-rw-rw-   0        0        0     2779 2023-04-13 17:38:50.000000 projectZ.py-1.1.6.7/projectZ.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      447 2023-04-13 17:38:51.000000 projectZ.py-1.1.6.7/projectZ.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 17:38:50.000000 projectZ.py-1.1.6.7/projectZ.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-04-13 17:38:50.000000 projectZ.py-1.1.6.7/projectZ.py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-13 17:38:50.000000 projectZ.py-1.1.6.7/projectZ.py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-13 17:38:51.879355 projectZ.py-1.1.6.7/setup.cfg
--rw-rw-rw-   0        0        0      857 2023-04-13 17:37:26.000000 projectZ.py-1.1.6.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-15 19:43:34.222315 projectZ.py-1.1.6.8/
+-rw-rw-rw-   0        0        0     2779 2023-04-15 19:43:34.222315 projectZ.py-1.1.6.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1777 2023-03-16 22:32:28.000000 projectZ.py-1.1.6.8/README.md
+drwxrwxrwx   0        0        0        0 2023-04-15 19:43:34.176293 projectZ.py-1.1.6.8/projectZ/
+-rw-rw-rw-   0        0        0      748 2023-04-15 19:42:30.000000 projectZ.py-1.1.6.8/projectZ/__init__.py
+-rw-rw-rw-   0        0        0    33557 2023-04-15 19:35:52.000000 projectZ.py-1.1.6.8/projectZ/async_client.py
+-rw-rw-rw-   0        0        0     8713 2023-04-01 11:49:21.000000 projectZ.py-1.1.6.8/projectZ/async_socket.py
+-rw-rw-rw-   0        0        0    29598 2023-04-15 19:41:18.000000 projectZ.py-1.1.6.8/projectZ/client.py
+-rw-rw-rw-   0        0        0     9048 2023-04-10 10:03:57.000000 projectZ.py-1.1.6.8/projectZ/socket.py
+drwxrwxrwx   0        0        0        0 2023-04-15 19:43:34.220302 projectZ.py-1.1.6.8/projectZ/utils/
+-rw-rw-rw-   0        0        0        0 2023-02-06 18:57:12.000000 projectZ.py-1.1.6.8/projectZ/utils/__init__.py
+-rw-rw-rw-   0        0        0     1869 2023-04-15 17:53:33.000000 projectZ.py-1.1.6.8/projectZ/utils/exceptions.py
+-rw-rw-rw-   0        0        0     2674 2023-03-17 11:05:21.000000 projectZ.py-1.1.6.8/projectZ/utils/generator.py
+-rw-rw-rw-   0        0        0      985 2023-02-18 18:34:23.000000 projectZ.py-1.1.6.8/projectZ/utils/headers.py
+-rw-rw-rw-   0        0        0    21942 2023-04-15 13:31:51.000000 projectZ.py-1.1.6.8/projectZ/utils/objects.py
+drwxrwxrwx   0        0        0        0 2023-04-15 19:43:34.205298 projectZ.py-1.1.6.8/projectZ.py.egg-info/
+-rw-rw-rw-   0        0        0     2779 2023-04-15 19:43:32.000000 projectZ.py-1.1.6.8/projectZ.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      447 2023-04-15 19:43:33.000000 projectZ.py-1.1.6.8/projectZ.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 19:43:32.000000 projectZ.py-1.1.6.8/projectZ.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-04-15 19:43:32.000000 projectZ.py-1.1.6.8/projectZ.py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-15 19:43:32.000000 projectZ.py-1.1.6.8/projectZ.py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-15 19:43:34.224310 projectZ.py-1.1.6.8/setup.cfg
+-rw-rw-rw-   0        0        0      857 2023-04-15 19:42:03.000000 projectZ.py-1.1.6.8/setup.py
```

### Comparing `projectZ.py-1.1.6.7/PKG-INFO` & `projectZ.py-1.1.6.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: projectZ.py
-Version: 1.1.6.7
+Version: 1.1.6.8
 Summary: Library for creating projectZ bots and scripts.
 Home-page: https://github.com/xXxCLOTIxXx/projectZ.py
 Author: Xsarz
 Author-email: xsarzy@gmail.com
 License: MIT
 Download-URL: https://github.com/xXxCLOTIxXx/projectZ.py/archive/refs/heads/main.zip
 Description: <table align="center">
```

### Comparing `projectZ.py-1.1.6.7/README.md` & `projectZ.py-1.1.6.8/README.md`

 * *Files identical despite different names*

### Comparing `projectZ.py-1.1.6.7/projectZ/__init__.py` & `projectZ.py-1.1.6.8/projectZ/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,14 +14,14 @@
 from json import loads
 from requests import get
 
 __title__ = 'projectZ.py'
 __author__ = 'Xsarz'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2023 Xsarz'
-__version__ = '1.1.6.7'
+__version__ = '1.1.6.8'
 
 
 __newest__ = loads(get("https://pypi.org/pypi/projectZ.py/json").text)["info"]["version"]
 if __version__ != __newest__:
 	s('cls || clear')
 	print(f'\033[38;5;214m{__title__} made by {__author__}\nPlease update the library. Your version: {__version__}  A new version:{__newest__}\033[0m')
```

### Comparing `projectZ.py-1.1.6.7/projectZ/async_client.py` & `projectZ.py-1.1.6.8/projectZ/async_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,21 +11,22 @@
 from io import BytesIO
 from aiofiles.threadpool.binary import AsyncBufferedReader
 from typing import Union, Optional
 
 gen = Generator()
 
 class AsyncClient(AsyncSocket, AsyncCallBacks):
-	def __init__(self, deviceId: str = None, socket_debug: bool = False, language: str = "en-US", country_code: str = "en", time_zone: int = 180):
+	def __init__(self, deviceId: str = None, socket_debug: bool = False, run_socket: bool = True, language: str = "en-US", country_code: str = "en", time_zone: int = 180):
 		self.api = 'https://api.projz.com'
 		self.deviceId = deviceId if deviceId else gen.deviceId()
 		self.profile = objects.User()
 		self.language = language
 		self.country_code = country_code
 		self.time_zone = time_zone
+		self.run_socket = run_socket
 
 		self.session = ClientSession()
 
 		AsyncSocket.__init__(self, headers=self.parse_headers, debug=socket_debug)
 		AsyncCallBacks.__init__(self)
 
 
@@ -81,33 +82,35 @@
 		})
 		endpoint = '/v1/auth/login'
 
 		async with self.session.post(f"{self.api}{endpoint}", headers=self.parse_headers(endpoint=endpoint, data=data), data=data) as response:
 			if response.status != 200: return exceptions.CheckException(await response.text())
 			else:
 				self.profile = objects.User(loads(await response.text()))
-				await self.connect()
+				if self.run_socket:await self.connect()
 				return self.profile
 
 
 	async def logout(self):
 		endpoint = '/v1/auth/logout'
 		async with self.session.post(f"{self.api}{endpoint}", headers=self.parse_headers(endpoint=endpoint)) as response:
 			if response.status != 200: return exceptions.CheckException(await response.text())
 			else:
 				self.profile = objects.User()
-				await self.disconnect()
+				if self.run_socket:await self.disconnect()
 				return response.status
 
 	async def Online(self):
+		if not self.run_socket:return
 		if self.online_loop_active: return
 		self.online_loop_active = create_task(self.online_loop())
 		return self.online_loop_active
 
 	async def Offline(self):
+		if not self.run_socket:return
 		if self.online_loop_active:
 			self.online_loop_active.cancel()
 			self.online_loop_active = None
 		return self.online_loop_active
 
 
 	async def join_chat(self, chatId: int):
@@ -170,14 +173,15 @@
 
 		endpoint = f'/v1/chat/joined-threads?start={start}&size={size}&type={type}'
 		async with self.session.get(f"{self.api}{endpoint}", headers=self.parse_headers(endpoint=endpoint)) as response:
 			return exceptions.CheckException(await response.text()) if response.status != 200 else  objects.Thread(loads(await response.text()))
 
 
 	async def send_message(self, chatId: int, message: str = None, file: AsyncBufferedReader = None, fileType: str = None, file_duration: int = None, message_type: int = 1, replyTo: int = None, pollId: int = None, diceId: int = None): 
+		if not self.run_socket:return
 		data = {
 			"threadId": chatId,
 			"uid": self.profile.uid,
 			"seqId": randint(0, maxsize),
 			"extensions": {}
 		}
 		if message:
@@ -351,41 +355,39 @@
 		async with self.session.post(f"{self.api}{endpoint}", headers=self.parse_headers(endpoint=endpoint)) as response:
 			return exceptions.CheckException(await response.text()) if response.status != 200 else response.status
 
 
 	async def check_in(self):
 		endpoint = f"/v1/users/check-in"
 		async with self.session.post(f"{self.api}{endpoint}", headers=self.parse_headers(endpoint=endpoint)) as response:
-			response = exceptions.CheckException(await response.text()) if response.status != 200 else loads(await response.text())
-		orderId = response.get("orderId", None)
-
-		await self.claim_transfer_orders(orderId=orderId)
+			response = exceptions.CheckException(await response.text()) if response.status != 200 else objects.OrderInfo(loads(await response.text()))
+		await self.claim_transfer_orders(orderId=response.orderId)
 
 		return response
 
 	async def claim_transfer_orders(self, orderId: int):
 
 		endpoint = f"/biz/v3/transfer-orders/{orderId}/claim"
 		async with self.session.post(f"{self.api}{endpoint}", headers=self.parse_headers(endpoint=endpoint)) as response:
-			return exceptions.CheckException(await response.text()) if response.status != 200 else response.status
+			return exceptions.CheckException(await response.text()) if response.status != 200 else loads(await response.text())#response.status
 
 
 	async def claim_gift_boxes(self, orderId: int):
 		endpoint = f"/v1/gift-boxes/{orderId}/claim"
 		async with self.session.post(f"{self.api}{endpoint}", headers=self.parse_headers(endpoint=endpoint)) as response:
 			return exceptions.CheckException(await response.text()) if response.status != 200 else response.status
 
 
 	async def get_transfer_order_info(self, orderId: int):
 
 		endpoint = f"/biz/v1/transfer-orders/{orderId}"
 		async with self.session.post(f"{self.api}{endpoint}", headers=self.parse_headers(endpoint=endpoint)) as response:
 			return exceptions.CheckException(await response.text()) if response.status != 200 else loads(await response.text())
 
-	async def send_coins(self, wallet_password: int, userId: int, amount: int, title: str = "Всего Наилучшего!"):
+	async def send_coins(self, wallet_password: int, userId: int, amount: int, title: str = "All the best!"):
 
 		data = dumps({
 			"toObjectId": userId,
 			"amount": f"{amount}000000000000000000",
 			"paymentPassword": str(wallet_password),
 			"toObjectType": 4,
 			"currencyType": 100,
@@ -726,8 +728,28 @@
 			"votedCount": 1,
 			"votedDate": 0,
 			"createdTime": 0,
 			"lastVoteTime": 0
 		})
 		endpoint = "/v1/qivotes"
 		async with self.session.post(f"{self.api}{endpoint}", headers=self.parse_headers(endpoint=endpoint, data=data), data=data) as response:
-			return exceptions.CheckException(await response.text()) if response.status != 200 else loads(await response.text())
+			return exceptions.CheckException(await response.text()) if response.status != 200 else loads(await response.text())
+
+
+	async def get_user_tasks(self):
+
+		endpoint = f"/v2/user-tasks"
+		async with self.session.get(f"{self.api}{endpoint}", headers=self.parse_headers(endpoint=endpoint)) as response:
+			return exceptions.CheckException(await response.text()) if response.status != 200 else loads(await response.text())
+
+
+	async def get_my_gifts(self, size: int = 60):
+		endpoint = f"/biz/v2/transfer-orders?size={size}"
+		async with self.session.get(f"{self.api}{endpoint}", headers=self.parse_headers(endpoint=endpoint)) as response:
+			return exceptions.CheckException(await response.text()) if response.status != 200 else objects.Gifts(loads(await response.text()))
+
+
+	async def gift_withdrawn(self, orderId):
+
+		endpoint = f"/biz/v1/gift-boxes/{orderId}/withdrawn"
+		async with self.session.post(f"{self.api}{endpoint}", headers=self.parse_headers(endpoint=endpoint)) as response:
+			return exceptions.CheckException(await response.text()) if response.status != 200 else loads(await response.text())
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `projectZ.py-1.1.6.7/projectZ/async_socket.py` & `projectZ.py-1.1.6.8/projectZ/async_socket.py`

 * *Files identical despite different names*

### Comparing `projectZ.py-1.1.6.7/projectZ/client.py` & `projectZ.py-1.1.6.8/projectZ/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -548,18 +548,16 @@
 		response = self.session.post(f"{self.api}{endpoint}", headers=self.parse_headers(endpoint=endpoint), proxies=self.proxies)
 		return exceptions.CheckException(response.text) if response.status_code != 200 else response.status_code
 
 
 	def check_in(self):
 		endpoint = f"/v1/users/check-in"
 		response = self.session.post(f"{self.api}{endpoint}", headers=self.parse_headers(endpoint=endpoint), proxies=self.proxies)
-		response = exceptions.CheckException(response.text) if response.status_code != 200 else loads(response.text)
-		orderId = response.get("orderId", None)
-		self.claim_transfer_orders(orderId=orderId)
-
+		response = exceptions.CheckException(response.text) if response.status_code != 200 else objects.OrderInfo(loads(response.text))
+		self.claim_transfer_orders(orderId=response.orderId)
 		return response
 
 	def claim_transfer_orders(self, orderId: int):
 
 		endpoint = f"/biz/v3/transfer-orders/{orderId}/claim"
 		response = self.session.post(f"{self.api}{endpoint}", headers=self.parse_headers(endpoint=endpoint), proxies=self.proxies)
 		return exceptions.CheckException(response.text) if response.status_code != 200 else response.status_code
@@ -648,7 +646,25 @@
 			"votedDate": 0,
 			"createdTime": 0,
 			"lastVoteTime": 0
 		})
 		endpoint = "/v1/qivotes"
 		response = self.session.post(f"{self.api}{endpoint}", headers=self.parse_headers(endpoint=endpoint, data=data), data=data, proxies=self.proxies)
 		return exceptions.CheckException(response.text) if response.status_code != 200 else loads(response.text)
+
+
+	def get_user_tasks(self):
+
+		endpoint = f"/v2/user-tasks"
+		response = self.session.get(f"{self.api}{endpoint}", headers=self.parse_headers(endpoint=endpoint), proxies=self.proxies)
+		return exceptions.CheckException(response.text) if response.status_code != 200 else loads(response.text)
+
+	def get_my_gifts(self, size: int = 60):
+		endpoint = f"/biz/v2/transfer-orders?size={size}"
+		response = self.session.get(f"{self.api}{endpoint}", headers=self.parse_headers(endpoint=endpoint), proxies=self.proxies)
+		return exceptions.CheckException(response.text) if response.status_code != 200 else objects.Gifts(loads(response.text))
+
+	def gift_withdrawn(self, orderId):
+
+		endpoint = f"/biz/v1/gift-boxes/{orderId}/withdrawn"
+		response = self.session.post(f"{self.api}{endpoint}", headers=self.parse_headers(endpoint=endpoint), proxies=self.proxies)
+		return exceptions.CheckException(response.text) if response.status != 200 else loads(response.text)
```

### Comparing `projectZ.py-1.1.6.7/projectZ/socket.py` & `projectZ.py-1.1.6.8/projectZ/socket.py`

 * *Files identical despite different names*

### Comparing `projectZ.py-1.1.6.7/projectZ/utils/exceptions.py` & `projectZ.py-1.1.6.8/projectZ/utils/exceptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -49,23 +49,29 @@
 
 
 class TooManyRequests(Exception):
 	def __init__(*args, **kwargs):
 		Exception.__init__(*args, **kwargs)
 
 
+class WalletNotActivated(Exception):
+	def __init__(*args, **kwargs):
+		Exception.__init__(*args, **kwargs)
+
+
 errors = {
 	2009: EmailNotRegistered,
 	2022: InvalidEmail,
 	4604: InvalidLink,
 	2010: IncorrectPassword,
 	2038: AlreadyRegistered,
 	6107: TooManyRequests,
 	7008: BadMedia,
-	1000004: NoWalletError
+	1000004: NoWalletError,
+	1000108: WalletNotActivated
 }
 
 def CheckException(data):
 	try:
 		data = loads(data)
 		code = data["apiCode"]
 	except:
```

### Comparing `projectZ.py-1.1.6.7/projectZ/utils/generator.py` & `projectZ.py-1.1.6.8/projectZ/utils/generator.py`

 * *Files identical despite different names*

### Comparing `projectZ.py-1.1.6.7/projectZ/utils/headers.py` & `projectZ.py-1.1.6.8/projectZ/utils/headers.py`

 * *Files identical despite different names*

### Comparing `projectZ.py-1.1.6.7/projectZ/utils/objects.py` & `projectZ.py-1.1.6.8/projectZ/utils/objects.py`

 * *Files 2% similar despite different names*

```diff
@@ -243,64 +243,65 @@
 		self.json = data
 		self.userId = self.json.get('uid', None)
 		self.activateStatus = self.json.get('activateStatus', None)
 		self.status = self.json.get('status', None)
 		self.createdTime = self.json.get('createdTime', None)
 		self.walletExtension = self.json.get('walletExtension', {})
 		self.unreadTransferOrderCount = self.json.get('unreadTransferOrderCount', None)
-		self.latestTransferOrder = self.LatestTransfer(self.json.get('latestTransferOrder', {}))
+		self.latestTransferOrder = LatestTransfer(self.json.get('latestTransferOrder', {}))
 		self.regularAccount = self.Account(self.json.get('regularAccount', {}))
 		self.storeAccount = self.Account(self.json.get('storeAccount', {}))
 
-	class LatestTransfer:
+	class Account:
 		def __init__(self, data: dict = {}):
 			self.json = data
+			self.accountId = self.json.get('accountId', None)
+			self.accountType = self.json.get('accountType', None)
+			self.status = self.json.get('status', None)
+			self.createdTime = self.json.get('createdTime', None)
+			self.ownerId = self.json.get('ownerId', None)
+			self.ownerType = self.json.get('ownerType', None)
+			self.currencyList = self.json.get('currencyList', None)
 
-			extensions = self.json.get('extensions', {})
 
-			self.orderId = self.json.get('orderId', None)
-			self.orderType = self.json.get('orderType', None)
-			self.currencyType = self.json.get('currencyType', None)
-			self.orderStatus = self.json.get('orderStatus', None)
-			self.fromUid = self.json.get('fromUid', None)
-			self.toUid = self.json.get('toUid', None)
-			self.amount = self.json.get('amount', None)
-			self.duration = self.json.get('duration', None)
-			self.minClaimedTime = self.json.get('minClaimedTime', None)
-			self.createdTime = self.json.get('createdTime', None)
-			self.returnTime = self.json.get('returnTime', None)
-			self.giftBoxId = extensions.get('status', None)
-			self.expiredTime = self.json.get('expiredTime', None)
-			self.currency = self.Currency(self.json.get('currency', {}))
 
 
-		class Currency:
-			def __init__(self, data: dict = {}):
-				self.json = data
-				self.name = self.json.get('name', None)
-				self.symbol = self.json.get('symbol', None)
-				self.icon = Media(self.json.get('icon', {}))
-				self.decimals = self.json.get('decimals', None)
-				self.currencyType = self.json.get('currencyType', None)
-				self.amount = self.json.get('amount', None)
 
 
+class LatestTransfer:
+	def __init__(self, data: dict = {}):
+		self.json = data
 
+		extensions = self.json.get('extensions', {})
 
+		self.orderId = self.json.get('orderId', None)
+		self.orderType = self.json.get('orderType', None)
+		self.currencyType = self.json.get('currencyType', None)
+		self.orderStatus = self.json.get('orderStatus', None)
+		self.fromUid = self.json.get('fromUid', None)
+		self.toUid = self.json.get('toUid', None)
+		self.amount = self.json.get('amount', None)
+		self.duration = self.json.get('duration', None)
+		self.minClaimedTime = self.json.get('minClaimedTime', None)
+		self.createdTime = self.json.get('createdTime', None)
+		self.returnTime = self.json.get('returnTime', None)
+		self.giftBoxId = extensions.get('status', None)
+		self.expiredTime = self.json.get('expiredTime', None)
+		self.currency = self.Currency(self.json.get('currency', {}))
 
-	class Account:
+
+	class Currency:
 		def __init__(self, data: dict = {}):
 			self.json = data
-			self.accountId = self.json.get('accountId', None)
-			self.accountType = self.json.get('accountType', None)
-			self.status = self.json.get('status', None)
-			self.createdTime = self.json.get('createdTime', None)
-			self.ownerId = self.json.get('ownerId', None)
-			self.ownerType = self.json.get('ownerType', None)
-			self.currencyList = self.json.get('currencyList', None)
+			self.name = self.json.get('name', None)
+			self.symbol = self.json.get('symbol', None)
+			self.icon = Media(self.json.get('icon', {}))
+			self.decimals = self.json.get('decimals', None)
+			self.currencyType = self.json.get('currencyType', None)
+			self.amount = self.json.get('amount', None)
 
 
 
 
 class ChatInfo:
 	def __init__(self, data: dict = {}):
 		self.json = data
@@ -546,8 +547,36 @@
 		self.json = data
 
 		pagination = self.json.get("pagination", None)
 
 		self.nextPageToken = pagination.get("nextPageToken", None)
 		self.members = list()
 		for member in self.json.get("list", []):
-			self.members.append(UserProfile(member))
+			self.members.append(UserProfile(member))
+
+
+class OrderInfo:
+	def __init__(self, data: dict = {}):
+		self.json = data
+		self.logId = self.json.get("logId")
+		self.userId = self.json.get("uid")
+		self.checkInDate = self.json.get("checkInDate")
+		self.orderId = self.json.get("orderId")
+		self.continuousCheckInDays = self.json.get("continuousCheckInDays")
+		self.createdTime = self.json.get("createdTime")
+		self.checkInDateUnix = self.json.get("checkInDateUnix")
+		self.nextMultipleStr = self.json.get("nextMultipleStr")
+		self.needDays = self.json.get("needDays")
+		self.decimals = self.json.get("decimals")
+		self.currencyType = self.json.get("currencyType")
+		self.currency = self.json.get("currency", {})
+		self.amount = self.currency.get("amount")
+
+
+
+class Gifts:
+	def __init__(self, data: dict = {}):
+		self.json = data
+		self.pagination = self.json.get("pagination")
+		self.gifts = list()
+		for gift in self.json.get("list", []):
+			self.gifts.append(LatestTransfer(gift))
```

### Comparing `projectZ.py-1.1.6.7/projectZ.py.egg-info/PKG-INFO` & `projectZ.py-1.1.6.8/projectZ.py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: projectZ.py
-Version: 1.1.6.7
+Version: 1.1.6.8
 Summary: Library for creating projectZ bots and scripts.
 Home-page: https://github.com/xXxCLOTIxXx/projectZ.py
 Author: Xsarz
 Author-email: xsarzy@gmail.com
 License: MIT
 Download-URL: https://github.com/xXxCLOTIxXx/projectZ.py/archive/refs/heads/main.zip
 Description: <table align="center">
```

### Comparing `projectZ.py-1.1.6.7/setup.py` & `projectZ.py-1.1.6.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as file:
 	long_description = file.read()
 
 link = 'https://github.com/xXxCLOTIxXx/projectZ.py/archive/refs/heads/main.zip'
-ver = '1.1.6.7'
+ver = '1.1.6.8'
 
 setup(
 	name = "projectZ.py",
 	version = ver,
 	url = "https://github.com/xXxCLOTIxXx/projectZ.py",
 	download_url = link,
 	license = "MIT",
```

