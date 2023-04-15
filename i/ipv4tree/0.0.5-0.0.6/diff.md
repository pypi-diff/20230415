# Comparing `tmp/ipv4tree-0.0.5.tar.gz` & `tmp/ipv4tree-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipv4tree-0.0.5.tar", last modified: Wed Apr  5 06:40:45 2023, max compression
+gzip compressed data, was "ipv4tree-0.0.6.tar", last modified: Sat Apr 15 09:52:10 2023, max compression
```

## Comparing `ipv4tree-0.0.5.tar` & `ipv4tree-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxrwxr-x   0 dvolkow   (1000) dvolkow   (1000)        0 2023-04-05 06:40:45.118315 ipv4tree-0.0.5/
--rw-rw-r--   0 dvolkow   (1000) dvolkow   (1000)    35149 2023-04-05 06:34:33.000000 ipv4tree-0.0.5/LICENSE
--rw-rw-r--   0 dvolkow   (1000) dvolkow   (1000)        0 2023-04-05 06:34:33.000000 ipv4tree-0.0.5/MANIFEST.in
--rw-rw-r--   0 dvolkow   (1000) dvolkow   (1000)      259 2023-04-05 06:40:45.118315 ipv4tree-0.0.5/PKG-INFO
--rw-rw-r--   0 dvolkow   (1000) dvolkow   (1000)     2253 2023-04-05 06:39:47.000000 ipv4tree-0.0.5/README.md
-drwxrwxr-x   0 dvolkow   (1000) dvolkow   (1000)        0 2023-04-05 06:40:45.118315 ipv4tree-0.0.5/ipv4tree/
--rw-rw-r--   0 dvolkow   (1000) dvolkow   (1000)       41 2023-04-05 06:39:47.000000 ipv4tree-0.0.5/ipv4tree/__init__.py
--rw-rw-r--   0 dvolkow   (1000) dvolkow   (1000)    12603 2023-04-05 06:39:47.000000 ipv4tree-0.0.5/ipv4tree/ipv4tree.py
-drwxrwxr-x   0 dvolkow   (1000) dvolkow   (1000)        0 2023-04-05 06:40:45.118315 ipv4tree-0.0.5/ipv4tree.egg-info/
--rw-rw-r--   0 dvolkow   (1000) dvolkow   (1000)      259 2023-04-05 06:40:45.000000 ipv4tree-0.0.5/ipv4tree.egg-info/PKG-INFO
--rw-rw-r--   0 dvolkow   (1000) dvolkow   (1000)      239 2023-04-05 06:40:45.000000 ipv4tree-0.0.5/ipv4tree.egg-info/SOURCES.txt
--rw-rw-r--   0 dvolkow   (1000) dvolkow   (1000)        1 2023-04-05 06:40:45.000000 ipv4tree-0.0.5/ipv4tree.egg-info/dependency_links.txt
--rw-rw-r--   0 dvolkow   (1000) dvolkow   (1000)       10 2023-04-05 06:40:45.000000 ipv4tree-0.0.5/ipv4tree.egg-info/requires.txt
--rw-rw-r--   0 dvolkow   (1000) dvolkow   (1000)        9 2023-04-05 06:40:45.000000 ipv4tree-0.0.5/ipv4tree.egg-info/top_level.txt
--rw-rw-r--   0 dvolkow   (1000) dvolkow   (1000)       38 2023-04-05 06:40:45.118315 ipv4tree-0.0.5/setup.cfg
--rw-rw-r--   0 dvolkow   (1000) dvolkow   (1000)      447 2023-04-05 06:34:33.000000 ipv4tree-0.0.5/setup.py
+drwxrwxr-x   0 dvolkow   (1000) dvolkow   (1000)        0 2023-04-15 09:52:10.634602 ipv4tree-0.0.6/
+-rw-rw-r--   0 dvolkow   (1000) dvolkow   (1000)    35149 2023-04-05 06:34:33.000000 ipv4tree-0.0.6/LICENSE
+-rw-rw-r--   0 dvolkow   (1000) dvolkow   (1000)        0 2023-04-05 06:34:33.000000 ipv4tree-0.0.6/MANIFEST.in
+-rw-rw-r--   0 dvolkow   (1000) dvolkow   (1000)      259 2023-04-15 09:52:10.634602 ipv4tree-0.0.6/PKG-INFO
+-rw-rw-r--   0 dvolkow   (1000) dvolkow   (1000)     5344 2023-04-15 09:51:17.000000 ipv4tree-0.0.6/README.md
+drwxrwxr-x   0 dvolkow   (1000) dvolkow   (1000)        0 2023-04-15 09:52:10.634602 ipv4tree-0.0.6/ipv4tree/
+-rw-rw-r--   0 dvolkow   (1000) dvolkow   (1000)       69 2023-04-15 08:33:57.000000 ipv4tree-0.0.6/ipv4tree/__init__.py
+-rw-rw-r--   0 dvolkow   (1000) dvolkow   (1000)    16870 2023-04-15 09:42:17.000000 ipv4tree-0.0.6/ipv4tree/ipv4tree.py
+-rw-rw-r--   0 dvolkow   (1000) dvolkow   (1000)     1395 2023-04-15 08:46:50.000000 ipv4tree-0.0.6/ipv4tree/multiprocessing.py
+-rw-rw-r--   0 dvolkow   (1000) dvolkow   (1000)     1043 2023-04-14 17:06:56.000000 ipv4tree-0.0.6/ipv4tree/utils.py
+drwxrwxr-x   0 dvolkow   (1000) dvolkow   (1000)        0 2023-04-15 09:52:10.634602 ipv4tree-0.0.6/ipv4tree.egg-info/
+-rw-rw-r--   0 dvolkow   (1000) dvolkow   (1000)      259 2023-04-15 09:52:10.000000 ipv4tree-0.0.6/ipv4tree.egg-info/PKG-INFO
+-rw-rw-r--   0 dvolkow   (1000) dvolkow   (1000)      285 2023-04-15 09:52:10.000000 ipv4tree-0.0.6/ipv4tree.egg-info/SOURCES.txt
+-rw-rw-r--   0 dvolkow   (1000) dvolkow   (1000)        1 2023-04-15 09:52:10.000000 ipv4tree-0.0.6/ipv4tree.egg-info/dependency_links.txt
+-rw-rw-r--   0 dvolkow   (1000) dvolkow   (1000)       10 2023-04-15 09:52:10.000000 ipv4tree-0.0.6/ipv4tree.egg-info/requires.txt
+-rw-rw-r--   0 dvolkow   (1000) dvolkow   (1000)        9 2023-04-15 09:52:10.000000 ipv4tree-0.0.6/ipv4tree.egg-info/top_level.txt
+-rw-rw-r--   0 dvolkow   (1000) dvolkow   (1000)       38 2023-04-15 09:52:10.634602 ipv4tree-0.0.6/setup.cfg
+-rw-rw-r--   0 dvolkow   (1000) dvolkow   (1000)      447 2023-04-05 06:34:33.000000 ipv4tree-0.0.6/setup.py
```

### Comparing `ipv4tree-0.0.5/LICENSE` & `ipv4tree-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ipv4tree-0.0.5/ipv4tree/ipv4tree.py` & `ipv4tree-0.0.6/ipv4tree/ipv4tree.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from collections.abc import Collection, Iterable
 from ipaddress import IPv4Address, IPv4Network
 from typing import Union, Optional, Dict
+from ipv4tree.utils import _get_binary_path_from_ipv4_addr
 
 
 class IPv4TreeNode(Iterable):
     """
     Unit for IPv4Tree structure.
     """
 
@@ -135,14 +136,21 @@
                             prefixlen=prev.prefixlen + 1,
                             size=size,
                             parent=prev,
                             **kwargs)
         self._nodes += 1
         return node
 
+    def __add__(self, other: 'IPv4Tree'):
+        for node in other:
+            if node.islast:
+                self.insert(str(node))
+
+        return self
+
     def delete(self, ip: Union[str, int, IPv4Address, IPv4Network]) -> None:
         """
         Delete IPv4 address or network from tree
         :param ip: IPv4 address or network
         """
         net = IPv4Network(ip)
         if not self.intree(ip):
@@ -156,18 +164,18 @@
             prev = node
             node = prev.child(n)
             inv_key = '1' if n == '0' else '0'
             inv_node = prev.child(inv_key)
             if prev.islast and not in_last:
                 in_last = True
 
-            if node == None:
+            if node is None:
                 node = self._insert_node(prev, n, 0)
 
-            if inv_node == None:
+            if inv_node is None:
                 inv_node = self._insert_node(prev, inv_key, 0)
                 inv_node._islast = in_last
 
             prev._islast = False
             if node.prefixlen == net.prefixlen:
                 break
 
@@ -183,17 +191,17 @@
         """
         Check address in tree.
 
         :param ip: IPv4 address or network
         :return: True if address or network exist in tree
         """
         ip = IPv4Network(ip)
-        intree = ip in self
-        if intree:
+        if ip in self:
             return True
+
         node = self._root
         for n in _get_binary_path_from_ipv4_addr(ip):
             prev = node
             node = prev.child(n)
             if node is None:
                 return False
             if node.islast or node.prefixlen == ip.prefixlen:
@@ -214,24 +222,66 @@
             node = prev.child(n)
             if node is None:
                 return None
             if node.islast or node.prefixlen == ip.prefixlen:
                 break
         return node
 
+    def insert_node(self, new_node: IPv4TreeNode) -> None:
+        """
+        Insert IPv4 address or network in IPv4Tree structure.
+
+        :param ip: IPv4 address or network
+        :param kwargs: custom parameters for your nodes.
+        """
+        ip = IPv4Network(str(new_node))
+        if ip in self:
+            return
+
+        size = new_node.size
+        node = self._root
+        self._root.update(-1, size)
+        was_insert = False
+        for n in _get_binary_path_from_ipv4_addr(ip):
+            prev = node
+            node = prev.child(n)
+            if node is None:
+                node = self._insert_node(prev, n, size)
+                was_insert = True
+            else:
+                node.update(node.prefixlen, size)
+
+            if node.prefixlen == ip.prefixlen:
+                new_node._parent = prev
+                node = new_node
+                break
+
+        prev.new_child(n, new_node)
+        if not was_insert:
+            if node.prefixlen != ip.prefixlen:
+                # is supernet
+                excess = size
+            else:
+                excess = node.size - size
+            while node is not None:
+                node.update(-1, -excess)
+                node = node.parent
+        else:
+            # new node in last level
+            self._nodes_map[ip] = node
+
     def insert(self, ip: Union[str, int, IPv4Address, IPv4Network], **kwargs) -> None:
         """
         Insert IPv4 address or network in IPv4Tree structure.
 
         :param ip: IPv4 address or network
         :param kwargs: custom parameters for your nodes.
         """
         ip = IPv4Network(ip)
-        intree = ip in self
-        if intree:
+        if ip in self:
             return
 
         size = ip.num_addresses
         node = self._root
         self._root.update(-1, size)
         was_insert = False
         for n in _get_binary_path_from_ipv4_addr(ip):
@@ -261,14 +311,81 @@
             while node is not None:
                 node.update(-1, -excess)
                 node = node.parent
         else:
             # new node in last level
             self._nodes_map[ip] = node
 
+    def fake_insert(self, ip: Union[str, int, IPv4Address, IPv4Network], **kwargs) -> None:
+        """
+        Fake insert IPv4 address or network in IPv4Tree structure (path created for multiprocessing usage).
+
+        :param ip: IPv4 address or network
+        :param kwargs: custom parameters for your nodes.
+        """
+        ip = IPv4Network(ip)
+        size = ip.num_addresses
+        node = self._root
+        self._root.update(-1, size)
+        was_insert = False
+        for n in _get_binary_path_from_ipv4_addr(ip):
+            prev = node
+            node = prev.child(n)
+            if node is None:
+                node = self._insert_node(prev, n, size, **kwargs)
+                was_insert = True
+
+            if node.prefixlen == ip.prefixlen:
+                # try insert for supernetwork?
+                break
+
+        if not was_insert:
+            if node.prefixlen != ip.prefixlen:
+                # is supernet
+                excess = size
+            else:
+                excess = node.size - size
+            while node is not None:
+                node.update(-1, -excess)
+                node = node.parent
+
+    def fast_insert(self, ip: Union[str, int, IPv4Address, IPv4Network], **kwargs) -> None:
+        """
+        Insert IPv4 address or network in IPv4Tree structure.
+        ATTENTION! Has no updates for size!
+
+        :param ip: IPv4 address or network
+        :param kwargs: custom parameters for your nodes.
+        """
+        ip = IPv4Network(ip)
+        if ip in self:
+            return
+
+        node = self._root
+        was_insert = False
+        for n in _get_binary_path_from_ipv4_addr(ip):
+            prev = node
+            node = prev.child(n)
+            if node is None:
+                node = self._insert_node(prev, n, **kwargs)
+                was_insert = True
+
+            if node.islast:
+                # try insert for subnetwork of exist in tree
+                break
+
+            if node.prefixlen == ip.prefixlen:
+                # try insert for supernetwork?
+                break
+
+        node._islast = True
+        if was_insert:
+            # new node in last level
+            self._nodes_map[ip] = node
+
     def __contains__(self, ipv4: Union[str, int, IPv4Address, IPv4Network]) -> bool:
         return IPv4Network(ipv4) in self._nodes_map.keys()
 
     def __iter__(self) -> Iterable:
         return iter(self._root)
 
     def __len__(self) -> int:
@@ -305,30 +422,24 @@
         last_nodes = 0
         for node in self:
             prefixlen = str(node.prefixlen)
             if prefixlen not in prefixlens.keys():
                 prefixlens[prefixlen] = 1
             else:
                 prefixlens[prefixlen] += 1
+
             if node.islast:
                 last_nodes += 1
+
         return str(prefixlens) + "\nTotal nodes: {}\nSize: {}" \
                                  "\nLast nodes: {}".format(self._nodes,
                                                            self._root.size,
                                                            last_nodes)
 
 
-def _get_binary_path_from_ipv4_addr(ipv4: Union[IPv4Address, IPv4Network]):
-    if isinstance(ipv4, IPv4Network):
-        return "{0:032b}".format(int(ipv4.network_address))
-    if isinstance(ipv4, IPv4Address):
-        return "{0:032b}".format(int(ipv4))
-    raise TypeError("bad type {}".format(type(ipv4)))
-
-
 class CIDRTree(IPv4Tree):
     """
     The prefix tree special for CIDR matching based on IPv4TRee.
 
     Insert: ignore already existed node for insert in tree.
     Supernet: search all last nodes and return node with largest prefixlen.
     """
@@ -338,16 +449,15 @@
         Insert IPv4 address or network in IPv4Tree structure.
         IMPORTANT! Insert are ignore exists networks in path!
 
         :param ip: IPv4 address or network
         :param kwargs: custom parameters for your nodes.
         """
         ip = IPv4Network(ip)
-        intree = ip in self
-        if intree:
+        if ip in self:
             return
 
         size = ip.num_addresses
         node = self._root
         self._root.update(-1, size)
         was_insert = False
         for n in _get_binary_path_from_ipv4_addr(ip):
@@ -373,14 +483,44 @@
             while node is not None:
                 node.update(-1, -excess)
                 node = node.parent
         else:
             # new node in last level
             self._nodes_map[ip] = node
 
+    def fast_insert(self, ip: Union[str, int, IPv4Address, IPv4Network], **kwargs) -> None:
+        """
+        Insert IPv4 address or network in IPv4Tree structure.
+        ATTENTION! Has no updates for size!
+
+        :param ip: IPv4 address or network
+        :param kwargs: custom parameters for your nodes.
+        """
+        ip = IPv4Network(ip)
+        if ip in self:
+            return
+
+        node = self._root
+        was_insert = False
+        for n in _get_binary_path_from_ipv4_addr(ip):
+            prev = node
+            node = prev.child(n)
+            if node is None:
+                node = self._insert_node(prev, n, **kwargs)
+                was_insert = True
+
+            if node.prefixlen == ip.prefixlen:
+                # try insert for supernetwork?
+                break
+
+        node._islast = True
+        if was_insert:
+            # new node in last level
+            self._nodes_map[ip] = node
+
     def supernet(self, ip: Union[str, IPv4Address, IPv4Network]) -> Optional[IPv4TreeNode]:
         """
         Return supernet for custom IPv4 address from IPv4Tree structure.
         IMPORTANT! Return subnet in tree with largest prefixlen!
 
         :param ip: IPv4 Address, string or IPv4Address type
         :return: IPv4TreeNode or None if not exist in tree
@@ -390,14 +530,16 @@
 
         last_nodes = []
         for n in _get_binary_path_from_ipv4_addr(ip):
             prev = node
             node = prev.child(n)
             if node is None:
                 break
+
             if node.islast:
                 last_nodes.append(node)
+
             if node.prefixlen == ip.prefixlen:
                 last_nodes.append(node)
                 break
 
         return last_nodes[-1] if last_nodes else None
```

