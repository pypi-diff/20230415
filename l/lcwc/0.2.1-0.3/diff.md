# Comparing `tmp/lcwc-0.2.1.tar.gz` & `tmp/lcwc-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lcwc-0.2.1.tar", last modified: Fri Apr  7 11:30:50 2023, max compression
+gzip compressed data, was "lcwc-0.3.tar", last modified: Sat Apr 15 17:57:44 2023, max compression
```

## Comparing `lcwc-0.2.1.tar` & `lcwc-0.3.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-07 11:30:50.654747 lcwc-0.2.1/
--rw-rw-rw-   0        0        0     1058 2023-01-16 14:14:04.000000 lcwc-0.2.1/LICENSE
--rw-rw-rw-   0        0        0     1832 2023-04-07 11:30:50.653749 lcwc-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     1176 2023-04-07 11:27:35.000000 lcwc-0.2.1/README.md
--rw-rw-rw-   0        0        0      791 2023-04-07 11:30:39.000000 lcwc-0.2.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-07 11:30:50.654747 lcwc-0.2.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-07 11:30:50.632747 lcwc-0.2.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-07 11:30:50.646748 lcwc-0.2.1/src/lcwc/
--rw-rw-rw-   0        0        0      172 2023-02-04 13:19:54.000000 lcwc-0.2.1/src/lcwc/__init__.py
--rw-rw-rw-   0        0        0      324 2023-01-28 13:09:14.000000 lcwc-0.2.1/src/lcwc/category.py
--rw-rw-rw-   0        0        0      825 2023-03-19 12:44:01.000000 lcwc-0.2.1/src/lcwc/client.py
--rw-rw-rw-   0        0        0     5710 2023-04-07 11:28:33.000000 lcwc-0.2.1/src/lcwc/feedclient.py
--rw-rw-rw-   0        0        0     2315 2023-02-25 16:34:29.000000 lcwc-0.2.1/src/lcwc/incident.py
--rw-rw-rw-   0        0        0      602 2023-02-13 11:08:18.000000 lcwc-0.2.1/src/lcwc/incidentlist.py
--rw-rw-rw-   0        0        0     3260 2023-04-07 11:30:01.000000 lcwc-0.2.1/src/lcwc/webclient.py
-drwxrwxrwx   0        0        0        0 2023-04-07 11:30:50.652748 lcwc-0.2.1/src/lcwc.egg-info/
--rw-rw-rw-   0        0        0     1832 2023-04-07 11:30:50.000000 lcwc-0.2.1/src/lcwc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      343 2023-04-07 11:30:50.000000 lcwc-0.2.1/src/lcwc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-07 11:30:50.000000 lcwc-0.2.1/src/lcwc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-04-07 11:30:50.000000 lcwc-0.2.1/src/lcwc.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-07 11:30:50.000000 lcwc-0.2.1/src/lcwc.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-15 17:57:44.448328 lcwc-0.3/
+-rw-rw-rw-   0        0        0     1058 2023-01-16 14:14:04.000000 lcwc-0.3/LICENSE
+-rw-rw-rw-   0        0        0     1764 2023-04-15 17:57:44.447328 lcwc-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1110 2023-04-15 17:56:28.000000 lcwc-0.3/README.md
+-rw-rw-rw-   0        0        0      789 2023-04-15 17:49:50.000000 lcwc-0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-15 17:57:44.448328 lcwc-0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-15 17:57:44.424328 lcwc-0.3/src/
+drwxrwxrwx   0        0        0        0 2023-04-15 17:57:44.439326 lcwc-0.3/src/lcwc/
+-rw-rw-rw-   0        0        0      172 2023-02-04 13:19:54.000000 lcwc-0.3/src/lcwc/__init__.py
+-rw-rw-rw-   0        0        0      324 2023-01-28 13:09:14.000000 lcwc-0.3/src/lcwc/category.py
+-rw-rw-rw-   0        0        0      915 2023-04-08 10:55:17.000000 lcwc-0.3/src/lcwc/client.py
+-rw-rw-rw-   0        0        0     6124 2023-04-15 17:55:42.000000 lcwc-0.3/src/lcwc/feedclient.py
+-rw-rw-rw-   0        0        0     2314 2023-04-15 17:45:56.000000 lcwc-0.3/src/lcwc/incident.py
+-rw-rw-rw-   0        0        0     3609 2023-04-15 17:56:04.000000 lcwc-0.3/src/lcwc/webclient.py
+drwxrwxrwx   0        0        0        0 2023-04-15 17:57:44.446327 lcwc-0.3/src/lcwc.egg-info/
+-rw-rw-rw-   0        0        0     1764 2023-04-15 17:57:44.000000 lcwc-0.3/src/lcwc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      318 2023-04-15 17:57:44.000000 lcwc-0.3/src/lcwc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 17:57:44.000000 lcwc-0.3/src/lcwc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-04-15 17:57:44.000000 lcwc-0.3/src/lcwc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-15 17:57:44.000000 lcwc-0.3/src/lcwc.egg-info/top_level.txt
```

### Comparing `lcwc-0.2.1/LICENSE` & `lcwc-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lcwc-0.2.1/PKG-INFO` & `lcwc-0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lcwc
-Version: 0.2.1
+Version: 0.3
 Summary: Python library for fetching the Lancaster County-Wide Communications live incident list.
 Author-email: Nate Shoffner <nate.shoffner@gmail.com>
 Project-URL: Homepage, https://github.com/NateShoffner/python-lcwc
 Project-URL: Bug Tracker, https://github.com/NateShoffner/python-lcwc/issues
 Keywords: lcwc,lancaster,police,fire,ems,dispatch,911,incident
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -13,36 +13,33 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # python-lcwc
 
 python-lcwc is a Python library for the [LCWC](https://www.lcwc911.us/live-incident-list) incident feed.
 
-Not affiliated or endorsed by LCWC.
-
 The library features both a web scraper and a RSS feed parser. The web scraper client is more reliable due to the RSS feed not categorizing incidents so we have to attempt to extrapolate the category from the incident description/units assigned. Functionally, it should be mostly accurate but edge cases may pop up. Addtionally, the feed parser offers a GUID. This is a unique identifier for each incident. The web client does not offer this.
 
 ## Installation
 
     pip install lcwc
 
 ## Example
 
 ```python
 
 import aiohttp
-from lcwc import webclient
+from lcwc import feedclient
 
-client = webclient.IncidentWebClient()
+client = feedclient.IncidentFeedClient()
 
 async with aiohttp.ClientSession() as session:
-    incidents = client.fetch_and_parse(session)
+    incidents = await client.fetch_and_parse(session)
 
     for incident in incidents:
-        print(f'Date: {incident.date}')
-        print(f'Description: {incident.description}')
+        print(f'{incident.date} - {incident.description}')
 ```
 
 ## TODO
 
 - [ ] Identify potential duplicate incidents reported under multiple categories (e.g. "Fire" and "Traffic" for vehicle fire)
 - [ ] Backing store and event emitter
```

### Comparing `lcwc-0.2.1/README.md` & `lcwc-0.3/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,30 @@
 # python-lcwc
 
 python-lcwc is a Python library for the [LCWC](https://www.lcwc911.us/live-incident-list) incident feed.
 
-Not affiliated or endorsed by LCWC.
-
 The library features both a web scraper and a RSS feed parser. The web scraper client is more reliable due to the RSS feed not categorizing incidents so we have to attempt to extrapolate the category from the incident description/units assigned. Functionally, it should be mostly accurate but edge cases may pop up. Addtionally, the feed parser offers a GUID. This is a unique identifier for each incident. The web client does not offer this.
 
 ## Installation
 
     pip install lcwc
 
 ## Example
 
 ```python
 
 import aiohttp
-from lcwc import webclient
+from lcwc import feedclient
 
-client = webclient.IncidentWebClient()
+client = feedclient.IncidentFeedClient()
 
 async with aiohttp.ClientSession() as session:
-    incidents = client.fetch_and_parse(session)
+    incidents = await client.fetch_and_parse(session)
 
     for incident in incidents:
-        print(f'Date: {incident.date}')
-        print(f'Description: {incident.description}')
+        print(f'{incident.date} - {incident.description}')
 ```
 
 ## TODO
 
 - [ ] Identify potential duplicate incidents reported under multiple categories (e.g. "Fire" and "Traffic" for vehicle fire)
 - [ ] Backing store and event emitter
```

### Comparing `lcwc-0.2.1/pyproject.toml` & `lcwc-0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "lcwc"
-version = "0.2.1"
+version = "0.3"
 authors = [
   { name="Nate Shoffner", email="nate.shoffner@gmail.com" },
 ]
 description = "Python library for fetching the Lancaster County-Wide Communications live incident list."
 keywords = ["lcwc", "lancaster", "police", "fire", "ems", "dispatch", "911", "incident"]
 readme = "README.md"
 requires-python = ">=3.9"
```

### Comparing `lcwc-0.2.1/src/lcwc/client.py` & `lcwc-0.3/src/lcwc/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,8 +18,9 @@
     @abstractmethod
     def parse(self, contents: bytes) -> list[Incident]:
         """ Parses the contents of the page and returns a list of incidents """
         pass
 
     @abstractmethod
     def fetch_and_parse(self, session: aiohttp.ClientSession, timeout: int) -> list[Incident]:
+        """ Fetches the page and parses the contents and returns a list of incidents """
         pass
```

### Comparing `lcwc-0.2.1/src/lcwc/feedclient.py` & `lcwc-0.3/src/lcwc/feedclient.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,45 +39,35 @@
     """ The URL of the live incident feed """
 
     FIRE_UNIT_NAMES = ['BRUSH', 'CHIEF', 'DEPUTY', 'DUTY OFFICER', 'ENGINE', 'FIRE POLICE', 'RESCUE', 'SQUAD', 'TRUCK', 'UTV']
     MEDICAL_UNIT_NAMES = ['AMB', 'EMS', 'INT', 'MEDIC', 'QRS']
 
     LOCATION_NAMES = ['ALY', 'AVE', 'CIR', 'CT', 'DR', 'LN', 'PL', 'PIKE', 'RAMP', 'RD', 'ROUTE', 'ST']
 
+    MEDICAL_DESCRIPTION_KEYWORDS = ['MEDICAL']
+    FIRE_DESCRIPTION_KEYWORDS = ['FIRE']
+    TRAFFIC_DESCRIPTION_KEYWORDS = ['TRAFFIC']
+
     def __init__(self):
         super().__init__()
 
-    async def get_incidents(self, session: aiohttp.ClientSession = None) -> list[FeedIncident]:
-        """ Gets the live incident feed and returns a list of incidents
-
-        :return: A list of incidents
-        :rtype: list[Incident]
-
-        :param session: An optional aiohttp session to use
-        """
-
-        if session is None:
-            session = aiohttp.ClientSession()
-        async with aiohttp.ClientSession() as session:    
-            contents = await self.fetch(session)
-            return self.parse(contents)
-
     async def fetch(self, session: aiohttp.ClientSession, timeout: int = 10) -> bytes:
         """ Gets the live incident feed and returns the xml as bytes
 
+        :param session: The aiohttp session to use
+        :param timeout: The timeout in seconds
         :return: The xml of the live incident feed
         :rtype: bytes
         """
         async with session:
             html = await super().fetch(session, timeout)
             return html
 
     def parse(self, contents: bytes) -> list[FeedIncident]:
-        """
-        Parses the live incident feed and returns a list of incidents
+        """ Parses the live incident feed and returns a list of incidents
 
         :param contents: The xml of the live incident feed
         :return: A list of incidents
         :rtype: list[Incident]
         """
         incidents = []
 
@@ -117,28 +107,46 @@
             description = entry.title
             cat = self.__determine_category(description, units)
             incidents.append(FeedIncident(cat, date, description, township, intersection, units, guid))
 
         return incidents
 
     async def fetch_and_parse(self, session: aiohttp.ClientSession, timeout: int = 10) -> list[FeedIncident]:
+        """ Gets the live incident feed and returns a list of incidents
+
+        :param session: The aiohttp session to use
+        :param timeout: The timeout for the request
+        :return: A list of incidents
+        :rtype: list[Incident]
+        """
         result = await self.fetch(session, timeout)
         active_incidents = self.parse(result)
         return active_incidents
 
     def __determine_category(self, description: str, units: list[str]) -> IncidentCategory:
-        """ Determines the category of an incident based on the description and units assigned """
+        """ Determines the category of an incident based on the description and units assigned 
+        
+        :param description: The description of the incident
+        :param units: The units assigned to the incident
+        :return: The category of the incident
+        :rtype: IncidentCategory
+        """
 
         # check for unit matches 
         for unit in units:
             if any(k in unit for k in self.FIRE_UNIT_NAMES):
                 return IncidentCategory.FIRE
             elif any(k in unit for k in self.MEDICAL_UNIT_NAMES):
                 return IncidentCategory.MEDICAL
 
-        # traffic incidents tend to not have units assigned
+        # perform a basic description check
+        if any(k in description for k in self.MEDICAL_DESCRIPTION_KEYWORDS):
+            return IncidentCategory.MEDICAL
+        if any(k in description for k in self.FIRE_DESCRIPTION_KEYWORDS):
+            return IncidentCategory.FIRE
+
+        # extra note regarding traffic incidents: they tend to not have units assigned
         # unless there is an accompanying fire or medical incident for the same call
-        traffic_title_keywords = ['TRAFFIC', 'VEHICLE']
-        if len(units) == 0 and any(k in description for k in traffic_title_keywords):
+        if any(k in description for k in self.TRAFFIC_DESCRIPTION_KEYWORDS):
             return IncidentCategory.TRAFFIC
 
         return IncidentCategory.UNKNOWN
```

### Comparing `lcwc-0.2.1/src/lcwc/incident.py` & `lcwc-0.3/src/lcwc/incident.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     def __init__(self, category: IncidentCategory, date: datetime, description: str, township: str, intersection: str, units: list[str] = []) -> None:
         """Constructor.
 
         :param IncidentCategory category: The category of the incident
         
         :param datetime date: The date and time of the incident in local time (EST)
 
-        :param str description: The description of thew incident
+        :param str description: The description of the incident
 
         :param str township: The location of the incident location
 
         :param str intersection: The intersection of the incident location
 
         :param list[str] units: A list of units responding to the incident
         """
```

### Comparing `lcwc-0.2.1/src/lcwc/webclient.py` & `lcwc-0.3/src/lcwc/webclient.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,24 +19,25 @@
 
     def __init__(self):
         super().__init__()
 
     async def fetch(self, session: aiohttp.ClientSession, timeout: int = 10) -> bytes:
         """ Gets the live incident page and returns the html as bytes
 
+        :param session: The aiohttp session to use
+        :param timeout: The timeout in seconds
         :return: The html of the live incident page
         :rtype: bytes
         """
         async with session:
             html = await super().fetch(session, timeout)
             return html
 
     def parse(self, page_html: bytes) -> list[Incident]:
-        """
-        Parses the live incident page and returns a list of incidents
+        """ Parses the live incident page and returns a list of incidents
 
         :param page_html: The html of the live incident page
         :return: A list of incidents
         :rtype: list[Incident]
         """
 
         incidents = []
@@ -80,10 +81,17 @@
     
                 incident = Incident(category, date, description, township, intersection, units)
                 incidents.append(incident)
 
         return incidents
 
     async def fetch_and_parse(self, session: aiohttp.ClientSession, timeout: int = 10) -> list[Incident]:
+        """ Gets the live incident page and returns a list of incidents
+
+        :param session: The aiohttp session to use
+        :param timeout: The timeout in seconds
+        :return: A list of incidents
+        :rtype: list[Incident]
+        """
         result = await self.fetch(session)
         active_incidents = self.parse(result)
         return active_incidents
```

### Comparing `lcwc-0.2.1/src/lcwc.egg-info/PKG-INFO` & `lcwc-0.3/src/lcwc.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lcwc
-Version: 0.2.1
+Version: 0.3
 Summary: Python library for fetching the Lancaster County-Wide Communications live incident list.
 Author-email: Nate Shoffner <nate.shoffner@gmail.com>
 Project-URL: Homepage, https://github.com/NateShoffner/python-lcwc
 Project-URL: Bug Tracker, https://github.com/NateShoffner/python-lcwc/issues
 Keywords: lcwc,lancaster,police,fire,ems,dispatch,911,incident
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -13,36 +13,33 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # python-lcwc
 
 python-lcwc is a Python library for the [LCWC](https://www.lcwc911.us/live-incident-list) incident feed.
 
-Not affiliated or endorsed by LCWC.
-
 The library features both a web scraper and a RSS feed parser. The web scraper client is more reliable due to the RSS feed not categorizing incidents so we have to attempt to extrapolate the category from the incident description/units assigned. Functionally, it should be mostly accurate but edge cases may pop up. Addtionally, the feed parser offers a GUID. This is a unique identifier for each incident. The web client does not offer this.
 
 ## Installation
 
     pip install lcwc
 
 ## Example
 
 ```python
 
 import aiohttp
-from lcwc import webclient
+from lcwc import feedclient
 
-client = webclient.IncidentWebClient()
+client = feedclient.IncidentFeedClient()
 
 async with aiohttp.ClientSession() as session:
-    incidents = client.fetch_and_parse(session)
+    incidents = await client.fetch_and_parse(session)
 
     for incident in incidents:
-        print(f'Date: {incident.date}')
-        print(f'Description: {incident.description}')
+        print(f'{incident.date} - {incident.description}')
 ```
 
 ## TODO
 
 - [ ] Identify potential duplicate incidents reported under multiple categories (e.g. "Fire" and "Traffic" for vehicle fire)
 - [ ] Backing store and event emitter
```

