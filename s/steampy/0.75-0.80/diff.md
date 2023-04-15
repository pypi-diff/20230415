# Comparing `tmp/steampy-0.75.tar.gz` & `tmp/steampy-0.80.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "steampy-0.75.tar", last modified: Mon Oct 18 08:04:52 2021, max compression
+gzip compressed data, was "steampy-0.80.tar", last modified: Sat Apr 15 09:44:38 2023, max compression
```

## Comparing `steampy-0.75.tar` & `steampy-0.80.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-18 08:04:52.435626 steampy-0.75/
--rw-r--r--   0 runner    (1001) docker     (121)     1093 2021-10-18 08:04:40.000000 steampy-0.75/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)      347 2021-10-18 08:04:52.435626 steampy-0.75/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    24744 2021-10-18 08:04:40.000000 steampy-0.75/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-18 08:04:52.431626 steampy-0.75/examples/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-18 08:04:40.000000 steampy-0.75/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      997 2021-10-18 08:04:40.000000 steampy-0.75/examples/chat_bot.py
--rw-r--r--   0 runner    (1001) docker     (121)      478 2021-10-18 08:04:40.000000 steampy-0.75/examples/desktop_authenticator.py
--rw-r--r--   0 runner    (1001) docker     (121)     1522 2021-10-18 08:04:40.000000 steampy-0.75/examples/storehouse.py
--rw-r--r--   0 runner    (1001) docker     (121)       79 2021-10-18 08:04:52.435626 steampy-0.75/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      671 2021-10-18 08:04:40.000000 steampy-0.75/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-18 08:04:52.431626 steampy-0.75/steampy/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-18 08:04:40.000000 steampy-0.75/steampy/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3789 2021-10-18 08:04:40.000000 steampy-0.75/steampy/chat.py
--rw-r--r--   0 runner    (1001) docker     (121)    15505 2021-10-18 08:04:40.000000 steampy-0.75/steampy/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     5365 2021-10-18 08:04:40.000000 steampy-0.75/steampy/confirmation.py
--rw-r--r--   0 runner    (1001) docker     (121)      323 2021-10-18 08:04:40.000000 steampy-0.75/steampy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1707 2021-10-18 08:04:40.000000 steampy-0.75/steampy/guard.py
--rw-r--r--   0 runner    (1001) docker     (121)     4756 2021-10-18 08:04:40.000000 steampy-0.75/steampy/login.py
--rw-r--r--   0 runner    (1001) docker     (121)     9608 2021-10-18 08:04:40.000000 steampy-0.75/steampy/market.py
--rw-r--r--   0 runner    (1001) docker     (121)     1778 2021-10-18 08:04:40.000000 steampy-0.75/steampy/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     7402 2021-10-18 08:04:40.000000 steampy-0.75/steampy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-18 08:04:52.431626 steampy-0.75/steampy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      347 2021-10-18 08:04:52.000000 steampy-0.75/steampy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      575 2021-10-18 08:04:52.000000 steampy-0.75/steampy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-18 08:04:52.000000 steampy-0.75/steampy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       28 2021-10-18 08:04:52.000000 steampy-0.75/steampy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       22 2021-10-18 08:04:52.000000 steampy-0.75/steampy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-18 08:04:52.435626 steampy-0.75/test/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-18 08:04:40.000000 steampy-0.75/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7938 2021-10-18 08:04:40.000000 steampy-0.75/test/test_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     1004 2021-10-18 08:04:40.000000 steampy-0.75/test/test_guard.py
--rw-r--r--   0 runner    (1001) docker     (121)     3952 2021-10-18 08:04:40.000000 steampy-0.75/test/test_market.py
--rw-r--r--   0 runner    (1001) docker     (121)     2370 2021-10-18 08:04:40.000000 steampy-0.75/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 09:44:38.742903 steampy-0.80/
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-04-15 09:44:30.000000 steampy-0.80/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-15 09:44:38.742903 steampy-0.80/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    26923 2023-04-15 09:44:30.000000 steampy-0.80/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 09:44:38.742903 steampy-0.80/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 09:44:30.000000 steampy-0.80/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-15 09:44:30.000000 steampy-0.80/examples/chat_bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-15 09:44:30.000000 steampy-0.80/examples/desktop_authenticator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-04-15 09:44:30.000000 steampy-0.80/examples/storehouse.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-15 09:44:38.742903 steampy-0.80/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-04-15 09:44:30.000000 steampy-0.80/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 09:44:38.742903 steampy-0.80/steampy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 09:44:30.000000 steampy-0.80/steampy/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3789 2023-04-15 09:44:30.000000 steampy-0.80/steampy/chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15505 2023-04-15 09:44:30.000000 steampy-0.80/steampy/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-04-15 09:44:30.000000 steampy-0.80/steampy/confirmation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-15 09:44:30.000000 steampy-0.80/steampy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-04-15 09:44:30.000000 steampy-0.80/steampy/guard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-04-15 09:44:30.000000 steampy-0.80/steampy/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9608 2023-04-15 09:44:30.000000 steampy-0.80/steampy/market.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-04-15 09:44:30.000000 steampy-0.80/steampy/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7402 2023-04-15 09:44:30.000000 steampy-0.80/steampy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 09:44:38.742903 steampy-0.80/steampy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-15 09:44:38.000000 steampy-0.80/steampy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-15 09:44:38.000000 steampy-0.80/steampy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 09:44:38.000000 steampy-0.80/steampy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-15 09:44:38.000000 steampy-0.80/steampy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-15 09:44:38.000000 steampy-0.80/steampy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 09:44:38.742903 steampy-0.80/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 09:44:30.000000 steampy-0.80/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7938 2023-04-15 09:44:30.000000 steampy-0.80/test/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-04-15 09:44:30.000000 steampy-0.80/test/test_guard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-04-15 09:44:30.000000 steampy-0.80/test/test_market.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-04-15 09:44:30.000000 steampy-0.80/test/test_utils.py
```

### Comparing `steampy-0.75/LICENSE.txt` & `steampy-0.80/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `steampy-0.75/README.md` & `steampy-0.80/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Steam Trade Offers Client for Python
 =======
 
 [![PayPal Donate Button](https://img.shields.io/badge/donate-paypal-orange.svg)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=XC8BMJ8QRD9ZY "Donate to this project via PayPal")
-[![Bitcoin Donate Button](https://img.shields.io/badge/donate-bitcoin-orange.svg)](https://blockchain.info/payment_request?address=3FCe4D73J7tJ1zH2Q8NM3xnEeLsevvX3jR&message=Development+of+steampy&amount_local=12&currency=USD&nosavecurrency=true "Donate to this project via Bitcoin")
+
+Donate bitcoin: 3KrB6B5YRQuSEEZ5EVMAQeGa3SLCFZ76T7
 
 `steampy` is a library for Python, inspired by node-steam-tradeoffers, node-steam and other libraries for Node.js.
 It was designed as a simple lightweight library, combining features of many steam libraries from Node.js into a single python module.
 `steampy` is capable of logging into steam, fetching trade offers and handling them in simple manner, using steam user credentials
 and SteamGuard file(no need to extract and pass sessionID and webCookie).
 `steampy` is developed with Python 3 using type hints and many other features its supported for Windows, Linux and MacOs.
 
@@ -386,15 +387,15 @@
 ==============
 
 **fetch_price(item_hash_name: str, game: GameOptions, currency: str = Currency.USD) -> dict**
 
 Some games are predefined in `GameOptions` class, such as `GameOptions.DOTA2`, `GameOptions.CS` and `GameOptions.TF2,
 but `GameOptions` object can be constructed with custom parameters.
 
-Currencies are defined in Currency class, currently `Currency.USD`, `Currency.GBP`, `Currency.EURO`, `Currency.CHF`
+Currencies are defined in Currency class, [currently](https://github.com/bukson/steampy#currencies)
 
 Default currency is USD
 
 May rise `TooManyRequests` exception if used more than 20 times in 60 seconds.
 
 ```python
 steam_client = SteamClient(self.credentials.api_key)
@@ -498,14 +499,67 @@
 ```python
 steam_client = SteamClient(self.credentials.api_key)
 steam_client.login('MY_USERNAME', 'MY_PASSWORD', 'PATH_TO_STEAMGUARD_FILE')
 buy_order_id = "some_buy_order_id"
 response = steam_client.market.cancel_buy_order(buy_order_id)
 ```
 
+Currencies
+----------
+
+| Currency class | Description                 |
+| ---            | ---                         |
+| Currency.USD   | United States Dollar        |
+| Currency.GBP   | United Kingdom Pound        |
+| Currency.EURO  | European Union Euro         |
+| Currency.CHF   | Swiss Francs                |
+| Currency.RUB   | Russian Rouble              |
+| Currency.PLN   | Polish Złoty                |
+| Currency.BRL   | Brazilian Reals             |
+| Currency.JPY   | Japanese Yen                |
+| Currency.NOK   | Norwegian Krone             |
+| Currency.IDR   | Indonesian Rupiah           |
+| Currency.MYR   | Malaysian Ringgit           |
+| Currency.PHP   | Philippine Peso             |
+| Currency.SGD   | Singapore Dollar            |
+| Currency.THB   | Thai Baht                   |
+| Currency.VND   | Vietnamese Dong             |
+| Currency.KRW   | South Korean Won            |
+| Currency.TRY   | Turkish Lira                |
+| Currency.UAH   | Ukrainian Hryvnia           |
+| Currency.MXN   | Mexican Peso                |
+| Currency.CAD   | Canadian Dollars            |
+| Currency.AUD   | Australian Dollars          |
+| Currency.NZD   | New Zealand Dollar          |
+| Currency.CNY   | Chinese Renminbi (yuan)     |
+| Currency.INR   | Indian Rupee                |
+| Currency.CLP   | Chilean Peso                |
+| Currency.PEN   | Peruvian Sol                |
+| Currency.COP   | Colombian Peso              |
+| Currency.ZAR   | South African Rand          |
+| Currency.HKD   | Hong Kong Dollar            |
+| Currency.TWD   | New Taiwan Dollar           |
+| Currency.SAR   | Saudi Riyal                 |
+| Currency.AED   | United Arab Emirates Dirham |
+| Currency.SEK   | Swedish Krona               |
+| Currency.ARS   | Argentine Peso              |
+| Currency.ILS   | Israeli New Shekel          |
+| Currency.BYN   | Belarusian Ruble            |
+| Currency.KZT   | Kazakhstani Tenge           |
+| Currency.KWD   | Kuwaiti Dinar               |
+| Currency.QAR   | Qatari Riyal                |
+| Currency.CRC   | Costa Rican Colón           |
+| Currency.UYU   | Uruguayan Peso              |
+| Currency.BGN   | Bulgarian Lev               |
+| Currency.HRK   | Croatian Kuna               |
+| Currency.CZK   | Czech Koruna                |
+| Currency.DKK   | Danish Krone                |
+| Currency.HUF   | Hungarian Forint            |
+| Currency.RON   | Romanian Leu                |
+
 guard module functions
 ======================
 
 **load_steam_guard(steam_guard: str) -> dict**
 
 If `steam_guard` is file name then load and parse it, else just parse `steam_guard` as json string.
```

### Comparing `steampy-0.75/examples/chat_bot.py` & `steampy-0.80/examples/chat_bot.py`

 * *Files identical despite different names*

### Comparing `steampy-0.75/examples/storehouse.py` & `steampy-0.80/examples/storehouse.py`

 * *Files identical despite different names*

### Comparing `steampy-0.75/setup.py` & `steampy-0.80/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 import sys
 
 if not sys.version_info[0] == 3 and sys.version_info[1] < 5:
     sys.exit('Python < 3.5 is not supported')
 
-version = '0.75'
+version = '0.80'
 
 setup(
     name='steampy',
     packages=['steampy', 'test', 'examples', ],
     version=version,
     description='A Steam lib for trade automation',
     author='Michał Bukowski',
```

### Comparing `steampy-0.75/steampy/chat.py` & `steampy-0.80/steampy/chat.py`

 * *Files identical despite different names*

### Comparing `steampy-0.75/steampy/client.py` & `steampy-0.80/steampy/client.py`

 * *Files identical despite different names*

### Comparing `steampy-0.75/steampy/confirmation.py` & `steampy-0.80/steampy/confirmation.py`

 * *Files identical despite different names*

### Comparing `steampy-0.75/steampy/guard.py` & `steampy-0.80/steampy/guard.py`

 * *Files identical despite different names*

### Comparing `steampy-0.75/steampy/login.py` & `steampy-0.80/steampy/login.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         return self.session
 
     def _send_login_request(self) -> requests.Response:
         rsa_params = self._fetch_rsa_params()
         encrypted_password = self._encrypt_password(rsa_params)
         rsa_timestamp = rsa_params['rsa_timestamp']
         request_data = self._prepare_login_request_data(encrypted_password, rsa_timestamp)
-        return self.session.post(SteamUrl.STORE_URL + '/login/dologin', data=request_data)
+        return self.session.post(SteamUrl.COMMUNITY_URL + '/login/dologin', data=request_data)
 
     def set_sessionid_cookies(self):
         sessionid = self.session.cookies.get_dict()['sessionid']
         community_domain = SteamUrl.COMMUNITY_URL[8:]
         store_domain = SteamUrl.STORE_URL[8:]
         community_cookie = self._create_session_id_cookie(sessionid, community_domain)
         store_cookie = self._create_session_id_cookie(sessionid, store_domain)
@@ -45,15 +45,15 @@
     def _create_session_id_cookie(sessionid: str, domain: str) -> dict:
         return {"name": "sessionid",
                 "value": sessionid,
                 "domain": domain}
 
     def _fetch_rsa_params(self, current_number_of_repetitions: int = 0) -> dict:
         maximal_number_of_repetitions = 5
-        key_response = self.session.post(SteamUrl.STORE_URL + '/login/getrsakey/',
+        key_response = self.session.post(SteamUrl.COMMUNITY_URL + '/login/getrsakey/',
                                          data={'username': self.username}).json()
         try:
             rsa_mod = int(key_response['publickey_mod'], 16)
             rsa_exp = int(key_response['publickey_exp'], 16)
             rsa_timestamp = key_response['timestamp']
             return {'rsa_key': rsa.PublicKey(rsa_mod, rsa_exp),
                     'rsa_timestamp': rsa_timestamp}
```

### Comparing `steampy-0.75/steampy/market.py` & `steampy-0.80/steampy/market.py`

 * *Files identical despite different names*

### Comparing `steampy-0.75/steampy/utils.py` & `steampy-0.80/steampy/utils.py`

 * *Files identical despite different names*

### Comparing `steampy-0.75/steampy.egg-info/SOURCES.txt` & `steampy-0.80/steampy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `steampy-0.75/test/test_client.py` & `steampy-0.80/test/test_client.py`

 * *Files identical despite different names*

### Comparing `steampy-0.75/test/test_guard.py` & `steampy-0.80/test/test_guard.py`

 * *Files identical despite different names*

### Comparing `steampy-0.75/test/test_market.py` & `steampy-0.80/test/test_market.py`

 * *Files identical despite different names*

### Comparing `steampy-0.75/test/test_utils.py` & `steampy-0.80/test/test_utils.py`

 * *Files identical despite different names*

