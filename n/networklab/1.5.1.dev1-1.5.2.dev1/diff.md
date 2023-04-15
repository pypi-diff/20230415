# Comparing `tmp/networklab-1.5.1.dev1.tar.gz` & `tmp/networklab-1.5.2.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "networklab-1.5.1.dev1.tar", last modified: Wed Mar 29 16:28:22 2023, max compression
+gzip compressed data, was "networklab-1.5.2.dev1.tar", last modified: Sat Apr 15 09:01:42 2023, max compression
```

## Comparing `networklab-1.5.1.dev1.tar` & `networklab-1.5.2.dev1.tar`

### file list

```diff
@@ -1,578 +1,606 @@
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-03-29 16:28:22.105179 networklab-1.5.1.dev1/
--rw-r--r--   0 pipi       (501) staff       (20)     1153 2022-05-02 06:40:29.000000 networklab-1.5.1.dev1/LICENSE.md
--rw-r--r--   0 pipi       (501) staff       (20)      254 2021-12-28 08:07:36.000000 networklab-1.5.1.dev1/MANIFEST.in
--rw-r--r--   0 pipi       (501) staff       (20)     4081 2023-03-29 16:28:22.105002 networklab-1.5.1.dev1/PKG-INFO
--rw-r--r--   0 pipi       (501) staff       (20)     3367 2023-01-28 06:30:20.000000 networklab-1.5.1.dev1/README.md
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-03-29 16:28:21.942568 networklab-1.5.1.dev1/netsim/
--rwxr--r--   0 pipi       (501) staff       (20)       51 2023-03-29 16:27:48.000000 networklab-1.5.1.dev1/netsim/__init__.py
--rw-r--r--   0 pipi       (501) staff       (20)    13342 2022-11-23 16:13:46.000000 networklab-1.5.1.dev1/netsim/addressing.py
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-03-29 16:28:21.943884 networklab-1.5.1.dev1/netsim/ansible/
--rwxr-xr-x   0 pipi       (501) staff       (20)      900 2022-12-18 17:58:58.000000 networklab-1.5.1.dev1/netsim/ansible/collect-configs.ansible
--rwxr-xr-x   0 pipi       (501) staff       (20)     1404 2022-12-18 17:58:58.000000 networklab-1.5.1.dev1/netsim/ansible/config.ansible
--rwxr-xr-x   0 pipi       (501) staff       (20)     1269 2023-01-12 13:38:07.000000 networklab-1.5.1.dev1/netsim/ansible/create-config.ansible
--rwxr--r--   0 pipi       (501) staff       (20)      295 2022-10-25 08:11:07.000000 networklab-1.5.1.dev1/netsim/ansible/display-neighbors.ansible
--rwxr-xr-x   0 pipi       (501) staff       (20)     3424 2023-01-25 10:08:09.000000 networklab-1.5.1.dev1/netsim/ansible/initial-config.ansible
--rw-r--r--   0 pipi       (501) staff       (20)      401 2022-12-22 15:59:29.000000 networklab-1.5.1.dev1/netsim/ansible/missing.yml
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-03-29 16:28:21.944598 networklab-1.5.1.dev1/netsim/ansible/tasks/
--rw-r--r--   0 pipi       (501) staff       (20)      684 2023-01-12 13:38:07.000000 networklab-1.5.1.dev1/netsim/ansible/tasks/create-config.yml
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-03-29 16:28:21.948825 networklab-1.5.1.dev1/netsim/ansible/tasks/deploy-config/
--rw-r--r--   0 pipi       (501) staff       (20)      333 2022-05-02 05:23:35.000000 networklab-1.5.1.dev1/netsim/ansible/tasks/deploy-config/arcos.yml
--rw-r--r--   0 pipi       (501) staff       (20)      157 2022-11-10 07:29:53.000000 networklab-1.5.1.dev1/netsim/ansible/tasks/deploy-config/asa.yml
--rw-r--r--   0 pipi       (501) staff       (20)      717 2022-05-02 05:23:46.000000 networklab-1.5.1.dev1/netsim/ansible/tasks/deploy-config/cumulus.yml
--rw-r--r--   0 pipi       (501) staff       (20)      841 2022-10-19 17:10:38.000000 networklab-1.5.1.dev1/netsim/ansible/tasks/deploy-config/cumulus_nvue.yml
--rw-r--r--   0 pipi       (501) staff       (20)      376 2022-04-17 16:31:22.000000 networklab-1.5.1.dev1/netsim/ansible/tasks/deploy-config/dellos10.yml
--rw-r--r--   0 pipi       (501) staff       (20)      159 2023-01-12 13:38:07.000000 networklab-1.5.1.dev1/netsim/ansible/tasks/deploy-config/eos.yml
--rw-r--r--   0 pipi       (501) staff       (20)      525 2022-05-02 05:23:58.000000 networklab-1.5.1.dev1/netsim/ansible/tasks/deploy-config/frr.yml
--rw-r--r--   0 pipi       (501) staff       (20)      159 2022-12-19 08:16:52.000000 networklab-1.5.1.dev1/netsim/ansible/tasks/deploy-config/ios.yml
--rw-r--r--   0 pipi       (501) staff       (20)      163 2023-01-12 13:38:07.000000 networklab-1.5.1.dev1/netsim/ansible/tasks/deploy-config/iosxr.yml
--rw-r--r--   0 pipi       (501) staff       (20)      204 2022-12-18 17:58:58.000000 networklab-1.5.1.dev1/netsim/ansible/tasks/deploy-config/junos.yml
--rw-r--r--   0 pipi       (501) staff       (20)      278 2022-12-22 08:33:55.000000 networklab-1.5.1.dev1/netsim/ansible/tasks/deploy-config/linux.yml
--rw-r--r--   0 pipi       (501) staff       (20)      140 2022-03-20 08:56:05.000000 networklab-1.5.1.dev1/netsim/ansible/tasks/deploy-config/none.yml
--rw-r--r--   0 pipi       (501) staff       (20)      161 2022-05-02 06:40:29.000000 networklab-1.5.1.dev1/netsim/ansible/tasks/deploy-config/nxos.yml
--rw-r--r--   0 pipi       (501) staff       (20)      777 2022-05-02 05:37:23.000000 networklab-1.5.1.dev1/netsim/ansible/tasks/deploy-config/routeros.yml
--rw-r--r--   0 pipi       (501) staff       (20)      240 2022-10-19 17:10:38.000000 networklab-1.5.1.dev1/netsim/ansible/tasks/deploy-config/routeros7.yml
--rw-r--r--   0 pipi       (501) staff       (20)     3328 2023-03-06 07:47:06.000000 networklab-1.5.1.dev1/netsim/ansible/tasks/deploy-config/srlinux.yml
--rw-r--r--   0 pipi       (501) staff       (20)     4799 2023-01-28 06:30:20.000000 networklab-1.5.1.dev1/netsim/ansible/tasks/deploy-config/sros.yml
--rw-r--r--   0 pipi       (501) staff       (20)      551 2022-12-18 17:58:58.000000 networklab-1.5.1.dev1/netsim/ansible/tasks/deploy-config/vyos.yml
--rw-r--r--   0 pipi       (501) staff       (20)     1937 2023-01-12 13:38:07.000000 networklab-1.5.1.dev1/netsim/ansible/tasks/deploy-custom-config.yml
--rw-r--r--   0 pipi       (501) staff       (20)     2142 2023-01-25 10:08:09.000000 networklab-1.5.1.dev1/netsim/ansible/tasks/deploy-module.yml
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-03-29 16:28:21.955356 networklab-1.5.1.dev1/netsim/ansible/tasks/fetch-config/
--rw-r--r--   0 pipi       (501) staff       (20)      160 2021-07-09 15:23:10.000000 networklab-1.5.1.dev1/netsim/ansible/tasks/fetch-config/arcos.yml
--rw-r--r--   0 pipi       (501) staff       (20)      110 2022-11-10 07:29:53.000000 networklab-1.5.1.dev1/netsim/ansible/tasks/fetch-config/asa.yml
--rw-r--r--   0 pipi       (501) staff       (20)      254 2022-03-07 15:39:35.000000 networklab-1.5.1.dev1/netsim/ansible/tasks/fetch-config/cumulus.yml
--rw-r--r--   0 pipi       (501) staff       (20)      308 2022-03-07 15:39:45.000000 networklab-1.5.1.dev1/netsim/ansible/tasks/fetch-config/cumulus_nvue.yml
--rw-r--r--   0 pipi       (501) staff       (20)      115 2022-04-17 16:31:22.000000 networklab-1.5.1.dev1/netsim/ansible/tasks/fetch-config/dellos10.yml
--rw-r--r--   0 pipi       (501) staff       (20)      112 2022-03-07 15:40:03.000000 networklab-1.5.1.dev1/netsim/ansible/tasks/fetch-config/eos.yml
--rw-r--r--   0 pipi       (501) staff       (20)      346 2021-12-11 08:49:40.000000 networklab-1.5.1.dev1/netsim/ansible/tasks/fetch-config/fortinet.fortios.fortios.yml
--rw-r--r--   0 pipi       (501) staff       (20)      110 2022-12-19 08:45:45.000000 networklab-1.5.1.dev1/netsim/ansible/tasks/fetch-config/ios.yml
--rw-r--r--   0 pipi       (501) staff       (20)      107 2023-01-12 13:38:07.000000 networklab-1.5.1.dev1/netsim/ansible/tasks/fetch-config/iosxr.yml
--rw-r--r--   0 pipi       (501) staff       (20)      124 2021-07-09 15:23:10.000000 networklab-1.5.1.dev1/netsim/ansible/tasks/fetch-config/junos.yml
--rw-r--r--   0 pipi       (501) staff       (20)      113 2021-07-09 15:23:10.000000 networklab-1.5.1.dev1/netsim/ansible/tasks/fetch-config/nxos.yml
--rw-r--r--   0 pipi       (501) staff       (20)      195 2021-11-27 09:09:57.000000 networklab-1.5.1.dev1/netsim/ansible/tasks/fetch-config/routeros.yml
--rw-r--r--   0 pipi       (501) staff       (20)      195 2022-10-19 17:10:38.000000 networklab-1.5.1.dev1/netsim/ansible/tasks/fetch-config/routeros7.yml
--rw-r--r--   0 pipi       (501) staff       (20)      721 2022-03-07 17:07:35.000000 networklab-1.5.1.dev1/netsim/ansible/tasks/fetch-config/srlinux.yml
--rw-r--r--   0 pipi       (501) staff       (20)      469 2022-03-07 17:07:35.000000 networklab-1.5.1.dev1/netsim/ansible/tasks/fetch-config/sros.yml
--rw-r--r--   0 pipi       (501) staff       (20)      190 2021-11-27 09:09:57.000000 networklab-1.5.1.dev1/netsim/ansible/tasks/fetch-config/vyos.yml
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-03-29 16:28:21.959492 networklab-1.5.1.dev1/netsim/ansible/tasks/fortinet.fortios.fortios/
--rw-r--r--   0 pipi       (501) staff       (20)     2645 2022-01-20 07:34:11.000000 networklab-1.5.1.dev1/netsim/ansible/tasks/fortinet.fortios.fortios/initial.yml
--rw-r--r--   0 pipi       (501) staff       (20)     2494 2022-10-19 17:10:38.000000 networklab-1.5.1.dev1/netsim/ansible/tasks/fortinet.fortios.fortios/ospf.yml
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-03-29 16:28:21.959727 networklab-1.5.1.dev1/netsim/ansible/tasks/iosxr/
--rw-r--r--   0 pipi       (501) staff       (20)      900 2023-01-12 13:38:07.000000 networklab-1.5.1.dev1/netsim/ansible/tasks/iosxr/initial.yml
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-03-29 16:28:21.959970 networklab-1.5.1.dev1/netsim/ansible/tasks/linux/
--rw-r--r--   0 pipi       (501) staff       (20)     1504 2023-01-12 13:38:07.000000 networklab-1.5.1.dev1/netsim/ansible/tasks/linux/initial-clab.yml
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-03-29 16:28:21.960257 networklab-1.5.1.dev1/netsim/ansible/tasks/nxos/
--rw-r--r--   0 pipi       (501) staff       (20)      291 2022-12-05 12:30:42.000000 networklab-1.5.1.dev1/netsim/ansible/tasks/nxos/initial.yml
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-03-29 16:28:21.960962 networklab-1.5.1.dev1/netsim/ansible/tasks/readiness-check/
--rw-r--r--   0 pipi       (501) staff       (20)      491 2023-01-12 13:38:07.000000 networklab-1.5.1.dev1/netsim/ansible/tasks/readiness-check/dellos10.yml
--rw-r--r--   0 pipi       (501) staff       (20)      125 2023-01-12 13:38:07.000000 networklab-1.5.1.dev1/netsim/ansible/tasks/readiness-check/eos-clab.yml
--rw-r--r--   0 pipi       (501) staff       (20)      378 2023-01-12 13:38:07.000000 networklab-1.5.1.dev1/netsim/ansible/tasks/readiness-check/routeros7.yml
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-03-29 16:28:21.961280 networklab-1.5.1.dev1/netsim/ansible/tasks/vmx/
--rw-r--r--   0 pipi       (501) staff       (20)     1707 2022-12-22 09:02:46.000000 networklab-1.5.1.dev1/netsim/ansible/tasks/vmx/initial.yml
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-03-29 16:28:21.961539 networklab-1.5.1.dev1/netsim/ansible/templates/
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-03-29 16:28:21.963534 networklab-1.5.1.dev1/netsim/ansible/templates/bfd/
--rw-r--r--   0 pipi       (501) staff       (20)      700 2022-12-11 11:47:34.000000 networklab-1.5.1.dev1/netsim/ansible/templates/bfd/eos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      599 2022-01-09 08:37:35.000000 networklab-1.5.1.dev1/netsim/ansible/templates/bfd/ios.j2
--rw-r--r--   0 pipi       (501) staff       (20)        0 2022-01-09 08:37:35.000000 networklab-1.5.1.dev1/netsim/ansible/templates/bfd/none.j2
--rw-r--r--   0 pipi       (501) staff       (20)      834 2022-01-09 08:37:35.000000 networklab-1.5.1.dev1/netsim/ansible/templates/bfd/nxos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      611 2022-01-09 08:37:35.000000 networklab-1.5.1.dev1/netsim/ansible/templates/bfd/srlinux.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1268 2022-11-04 10:28:02.000000 networklab-1.5.1.dev1/netsim/ansible/templates/bfd/sros.j2
--rw-r--r--   0 pipi       (501) staff       (20)      486 2022-08-27 11:27:47.000000 networklab-1.5.1.dev1/netsim/ansible/templates/bfd/vyos.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-03-29 16:28:21.974533 networklab-1.5.1.dev1/netsim/ansible/templates/bgp/
--rw-r--r--   0 pipi       (501) staff       (20)      888 2022-11-10 07:29:53.000000 networklab-1.5.1.dev1/netsim/ansible/templates/bgp/asa.j2
--rw-r--r--   0 pipi       (501) staff       (20)      778 2022-11-10 07:29:53.000000 networklab-1.5.1.dev1/netsim/ansible/templates/bgp/asa.macro.j2
--rw-r--r--   0 pipi       (501) staff       (20)       74 2022-10-19 17:10:38.000000 networklab-1.5.1.dev1/netsim/ansible/templates/bgp/cumulus.j2
--rw-r--r--   0 pipi       (501) staff       (20)     3040 2022-10-19 17:10:38.000000 networklab-1.5.1.dev1/netsim/ansible/templates/bgp/cumulus_nvue.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1257 2022-10-19 17:10:38.000000 networklab-1.5.1.dev1/netsim/ansible/templates/bgp/dellos10.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2010 2022-10-19 17:10:38.000000 networklab-1.5.1.dev1/netsim/ansible/templates/bgp/dellos10.macro.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1755 2022-12-11 16:40:37.000000 networklab-1.5.1.dev1/netsim/ansible/templates/bgp/eos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      911 2022-10-19 17:10:38.000000 networklab-1.5.1.dev1/netsim/ansible/templates/bgp/eos.macro.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2621 2022-10-19 17:10:38.000000 networklab-1.5.1.dev1/netsim/ansible/templates/bgp/frr.bgp-config.j2
--rw-r--r--   0 pipi       (501) staff       (20)       66 2022-10-19 17:10:38.000000 networklab-1.5.1.dev1/netsim/ansible/templates/bgp/frr.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1369 2023-02-07 15:05:29.000000 networklab-1.5.1.dev1/netsim/ansible/templates/bgp/ios.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1539 2022-12-21 09:06:32.000000 networklab-1.5.1.dev1/netsim/ansible/templates/bgp/ios.macro.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1830 2023-01-12 13:38:07.000000 networklab-1.5.1.dev1/netsim/ansible/templates/bgp/iosxr.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2308 2022-05-02 06:40:29.000000 networklab-1.5.1.dev1/netsim/ansible/templates/bgp/junos.j2
--rw-r--r--   0 pipi       (501) staff       (20)        0 2021-12-28 08:07:36.000000 networklab-1.5.1.dev1/netsim/ansible/templates/bgp/none.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1696 2022-09-01 07:44:05.000000 networklab-1.5.1.dev1/netsim/ansible/templates/bgp/nxos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1045 2022-05-02 06:40:29.000000 networklab-1.5.1.dev1/netsim/ansible/templates/bgp/routeros.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1109 2022-04-16 08:35:35.000000 networklab-1.5.1.dev1/netsim/ansible/templates/bgp/routeros.macro.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1075 2022-10-19 17:10:38.000000 networklab-1.5.1.dev1/netsim/ansible/templates/bgp/routeros7.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1401 2022-10-19 17:10:38.000000 networklab-1.5.1.dev1/netsim/ansible/templates/bgp/routeros7.macro.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2924 2022-05-02 06:40:29.000000 networklab-1.5.1.dev1/netsim/ansible/templates/bgp/srlinux.cli.j2
--rw-r--r--   0 pipi       (501) staff       (20)      316 2022-12-18 17:58:58.000000 networklab-1.5.1.dev1/netsim/ansible/templates/bgp/srlinux.j2
--rw-r--r--   0 pipi       (501) staff       (20)     7934 2022-12-18 17:58:58.000000 networklab-1.5.1.dev1/netsim/ansible/templates/bgp/srlinux.macro.j2
--rw-r--r--   0 pipi       (501) staff       (20)     3252 2022-11-04 10:28:02.000000 networklab-1.5.1.dev1/netsim/ansible/templates/bgp/sros.gnmi.macro.j2
--rw-r--r--   0 pipi       (501) staff       (20)      534 2022-10-25 08:00:46.000000 networklab-1.5.1.dev1/netsim/ansible/templates/bgp/sros.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2873 2022-05-02 06:40:29.000000 networklab-1.5.1.dev1/netsim/ansible/templates/bgp/sros.md-cli.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2086 2022-01-30 15:43:37.000000 networklab-1.5.1.dev1/netsim/ansible/templates/bgp/sros.openconfig.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1492 2022-10-19 17:10:38.000000 networklab-1.5.1.dev1/netsim/ansible/templates/bgp/vyos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1323 2022-10-19 17:10:38.000000 networklab-1.5.1.dev1/netsim/ansible/templates/bgp/vyos.macro.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-03-29 16:28:21.974974 networklab-1.5.1.dev1/netsim/ansible/templates/eigrp/
--rw-r--r--   0 pipi       (501) staff       (20)     1234 2023-02-07 15:05:29.000000 networklab-1.5.1.dev1/netsim/ansible/templates/eigrp/ios.j2
--rw-r--r--   0 pipi       (501) staff       (20)      862 2022-02-14 14:03:36.000000 networklab-1.5.1.dev1/netsim/ansible/templates/eigrp/nxos.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-03-29 16:28:21.977554 networklab-1.5.1.dev1/netsim/ansible/templates/evpn/
--rw-r--r--   0 pipi       (501) staff       (20)     1143 2022-11-04 10:28:02.000000 networklab-1.5.1.dev1/netsim/ansible/templates/evpn/cumulus.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1621 2022-11-04 10:28:02.000000 networklab-1.5.1.dev1/netsim/ansible/templates/evpn/dellos10.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1423 2022-12-15 16:40:50.000000 networklab-1.5.1.dev1/netsim/ansible/templates/evpn/eos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1580 2022-10-19 17:10:38.000000 networklab-1.5.1.dev1/netsim/ansible/templates/evpn/frr.evpn-config.j2
--rw-r--r--   0 pipi       (501) staff       (20)       35 2022-10-19 17:10:38.000000 networklab-1.5.1.dev1/netsim/ansible/templates/evpn/frr.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1677 2023-01-30 13:30:53.000000 networklab-1.5.1.dev1/netsim/ansible/templates/evpn/nxos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1708 2022-12-18 17:58:58.000000 networklab-1.5.1.dev1/netsim/ansible/templates/evpn/srlinux.j2
--rw-r--r--   0 pipi       (501) staff       (20)      405 2022-10-19 17:10:38.000000 networklab-1.5.1.dev1/netsim/ansible/templates/evpn/sros.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2883 2022-09-25 16:03:22.000000 networklab-1.5.1.dev1/netsim/ansible/templates/evpn/vyos.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-03-29 16:28:21.980189 networklab-1.5.1.dev1/netsim/ansible/templates/gateway/
--rw-r--r--   0 pipi       (501) staff       (20)     1244 2022-11-04 10:28:02.000000 networklab-1.5.1.dev1/netsim/ansible/templates/gateway/cumulus.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1162 2022-11-17 08:20:15.000000 networklab-1.5.1.dev1/netsim/ansible/templates/gateway/dellos10.j2
--rw-r--r--   0 pipi       (501) staff       (20)      951 2022-11-04 10:28:02.000000 networklab-1.5.1.dev1/netsim/ansible/templates/gateway/eos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      739 2022-12-14 07:49:49.000000 networklab-1.5.1.dev1/netsim/ansible/templates/gateway/ios.j2
--rw-r--r--   0 pipi       (501) staff       (20)      727 2022-11-04 10:28:02.000000 networklab-1.5.1.dev1/netsim/ansible/templates/gateway/nxos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      613 2022-11-04 10:28:02.000000 networklab-1.5.1.dev1/netsim/ansible/templates/gateway/srlinux.j2
--rw-r--r--   0 pipi       (501) staff       (20)      953 2023-01-28 06:30:20.000000 networklab-1.5.1.dev1/netsim/ansible/templates/gateway/sros.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1006 2022-11-17 08:20:15.000000 networklab-1.5.1.dev1/netsim/ansible/templates/gateway/vyos.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-03-29 16:28:21.990443 networklab-1.5.1.dev1/netsim/ansible/templates/initial/
--rw-r--r--   0 pipi       (501) staff       (20)      836 2022-01-05 16:01:35.000000 networklab-1.5.1.dev1/netsim/ansible/templates/initial/arcos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1122 2022-11-10 07:29:53.000000 networklab-1.5.1.dev1/netsim/ansible/templates/initial/asa.j2
--rw-r--r--   0 pipi       (501) staff       (20)       44 2022-12-18 17:58:58.000000 networklab-1.5.1.dev1/netsim/ansible/templates/initial/csr.vlan.j2
--rw-r--r--   0 pipi       (501) staff       (20)     5271 2023-03-28 17:02:16.000000 networklab-1.5.1.dev1/netsim/ansible/templates/initial/cumulus.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1342 2022-10-22 08:18:07.000000 networklab-1.5.1.dev1/netsim/ansible/templates/initial/cumulus_nvue.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1643 2022-10-19 17:10:38.000000 networklab-1.5.1.dev1/netsim/ansible/templates/initial/dellos10.j2
--rw-r--r--   0 pipi       (501) staff       (20)      537 2022-08-27 11:27:47.000000 networklab-1.5.1.dev1/netsim/ansible/templates/initial/dellos10.vrf.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2201 2022-11-04 10:28:02.000000 networklab-1.5.1.dev1/netsim/ansible/templates/initial/eos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      261 2022-08-27 11:27:47.000000 networklab-1.5.1.dev1/netsim/ansible/templates/initial/eos.vrf.j2
--rw-r--r--   0 pipi       (501) staff       (20)     3075 2023-01-12 13:38:07.000000 networklab-1.5.1.dev1/netsim/ansible/templates/initial/frr.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2371 2022-12-18 17:58:58.000000 networklab-1.5.1.dev1/netsim/ansible/templates/initial/ios.j2
--rw-r--r--   0 pipi       (501) staff       (20)      157 2022-12-14 07:50:27.000000 networklab-1.5.1.dev1/netsim/ansible/templates/initial/ios.vlan.j2
--rw-r--r--   0 pipi       (501) staff       (20)      378 2022-09-11 07:46:54.000000 networklab-1.5.1.dev1/netsim/ansible/templates/initial/ios.vrf.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1717 2023-01-12 13:38:07.000000 networklab-1.5.1.dev1/netsim/ansible/templates/initial/iosxr.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2118 2023-01-28 06:30:20.000000 networklab-1.5.1.dev1/netsim/ansible/templates/initial/junos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1524 2022-12-19 09:40:05.000000 networklab-1.5.1.dev1/netsim/ansible/templates/initial/junos.vlan.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1607 2022-12-19 09:40:05.000000 networklab-1.5.1.dev1/netsim/ansible/templates/initial/junos.vrf.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-03-29 16:28:21.991150 networklab-1.5.1.dev1/netsim/ansible/templates/initial/linux/
--rw-r--r--   0 pipi       (501) staff       (20)      906 2022-12-22 08:29:57.000000 networklab-1.5.1.dev1/netsim/ansible/templates/initial/linux/hosts.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2918 2022-12-22 09:39:24.000000 networklab-1.5.1.dev1/netsim/ansible/templates/initial/linux/ubuntu.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1933 2023-01-12 13:38:07.000000 networklab-1.5.1.dev1/netsim/ansible/templates/initial/linux/vanilla.j2
--rw-r--r--   0 pipi       (501) staff       (20)      283 2023-01-12 13:38:07.000000 networklab-1.5.1.dev1/netsim/ansible/templates/initial/linux-clab.j2
--rw-r--r--   0 pipi       (501) staff       (20)      434 2023-01-12 13:38:07.000000 networklab-1.5.1.dev1/netsim/ansible/templates/initial/linux.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1937 2023-01-30 13:30:53.000000 networklab-1.5.1.dev1/netsim/ansible/templates/initial/nxos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      393 2022-08-27 11:27:47.000000 networklab-1.5.1.dev1/netsim/ansible/templates/initial/nxos.vrf.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1413 2022-06-20 08:57:47.000000 networklab-1.5.1.dev1/netsim/ansible/templates/initial/routeros.j2
--rw-r--r--   0 pipi       (501) staff       (20)      546 2022-06-20 08:57:47.000000 networklab-1.5.1.dev1/netsim/ansible/templates/initial/routeros.vlan.j2
--rw-r--r--   0 pipi       (501) staff       (20)      498 2022-08-18 15:16:48.000000 networklab-1.5.1.dev1/netsim/ansible/templates/initial/routeros.vrf.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1571 2022-10-19 17:10:38.000000 networklab-1.5.1.dev1/netsim/ansible/templates/initial/routeros7.j2
--rw-r--r--   0 pipi       (501) staff       (20)      611 2022-10-19 17:10:38.000000 networklab-1.5.1.dev1/netsim/ansible/templates/initial/routeros7.vlan.j2
--rw-r--r--   0 pipi       (501) staff       (20)      352 2022-10-19 17:10:38.000000 networklab-1.5.1.dev1/netsim/ansible/templates/initial/routeros7.vrf.j2
--rw-r--r--   0 pipi       (501) staff       (20)      968 2022-01-05 16:01:35.000000 networklab-1.5.1.dev1/netsim/ansible/templates/initial/srlinux.cli.j2
--rw-r--r--   0 pipi       (501) staff       (20)     3431 2022-10-19 17:10:38.000000 networklab-1.5.1.dev1/netsim/ansible/templates/initial/srlinux.j2
--rw-r--r--   0 pipi       (501) staff       (20)     4711 2023-03-29 16:02:34.000000 networklab-1.5.1.dev1/netsim/ansible/templates/initial/sros.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1434 2022-01-05 16:01:35.000000 networklab-1.5.1.dev1/netsim/ansible/templates/initial/sros.md-cli.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2622 2022-01-06 16:04:54.000000 networklab-1.5.1.dev1/netsim/ansible/templates/initial/sros.openconfig.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2782 2022-11-10 07:29:53.000000 networklab-1.5.1.dev1/netsim/ansible/templates/initial/vyos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      250 2022-06-20 08:57:47.000000 networklab-1.5.1.dev1/netsim/ansible/templates/initial/vyos.vlan.j2
--rw-r--r--   0 pipi       (501) staff       (20)      101 2022-08-18 15:17:06.000000 networklab-1.5.1.dev1/netsim/ansible/templates/initial/vyos.vrf.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-03-29 16:28:21.994815 networklab-1.5.1.dev1/netsim/ansible/templates/isis/
--rw-r--r--   0 pipi       (501) staff       (20)      887 2022-11-10 07:29:53.000000 networklab-1.5.1.dev1/netsim/ansible/templates/isis/asa.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1241 2022-02-14 14:03:36.000000 networklab-1.5.1.dev1/netsim/ansible/templates/isis/eos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1149 2022-02-14 14:03:36.000000 networklab-1.5.1.dev1/netsim/ansible/templates/isis/frr.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1505 2022-12-20 08:16:04.000000 networklab-1.5.1.dev1/netsim/ansible/templates/isis/ios.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1168 2023-01-12 13:38:07.000000 networklab-1.5.1.dev1/netsim/ansible/templates/isis/iosxr.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2225 2022-12-19 09:40:05.000000 networklab-1.5.1.dev1/netsim/ansible/templates/isis/junos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1701 2022-02-14 14:03:36.000000 networklab-1.5.1.dev1/netsim/ansible/templates/isis/nxos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2086 2022-11-23 16:08:58.000000 networklab-1.5.1.dev1/netsim/ansible/templates/isis/srlinux.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1426 2022-11-04 10:28:02.000000 networklab-1.5.1.dev1/netsim/ansible/templates/isis/sros.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1550 2022-01-06 06:47:23.000000 networklab-1.5.1.dev1/netsim/ansible/templates/isis/sros.openconfig.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1262 2022-08-27 11:27:47.000000 networklab-1.5.1.dev1/netsim/ansible/templates/isis/vyos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      136 2021-12-06 08:23:27.000000 networklab-1.5.1.dev1/netsim/ansible/templates/missing.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-03-29 16:28:22.007034 networklab-1.5.1.dev1/netsim/ansible/templates/mpls/
--rw-r--r--   0 pipi       (501) staff       (20)      670 2022-08-27 11:27:47.000000 networklab-1.5.1.dev1/netsim/ansible/templates/mpls/eos.6pe.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1089 2022-04-01 07:43:22.000000 networklab-1.5.1.dev1/netsim/ansible/templates/mpls/eos.bgp-lu.j2
--rw-r--r--   0 pipi       (501) staff       (20)      289 2022-08-27 11:27:47.000000 networklab-1.5.1.dev1/netsim/ansible/templates/mpls/eos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      410 2022-04-01 07:43:22.000000 networklab-1.5.1.dev1/netsim/ansible/templates/mpls/eos.ldp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      413 2022-04-01 07:43:22.000000 networklab-1.5.1.dev1/netsim/ansible/templates/mpls/eos.mplsvpn.j2
--rw-r--r--   0 pipi       (501) staff       (20)      195 2023-01-12 13:38:07.000000 networklab-1.5.1.dev1/netsim/ansible/templates/mpls/frr.frr-config.j2
--rw-r--r--   0 pipi       (501) staff       (20)      272 2023-01-12 13:38:07.000000 networklab-1.5.1.dev1/netsim/ansible/templates/mpls/frr.j2
--rw-r--r--   0 pipi       (501) staff       (20)      472 2023-01-12 13:38:07.000000 networklab-1.5.1.dev1/netsim/ansible/templates/mpls/frr.ldp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      327 2023-01-12 13:38:07.000000 networklab-1.5.1.dev1/netsim/ansible/templates/mpls/frr.mplsvpn.j2
--rw-r--r--   0 pipi       (501) staff       (20)      208 2022-08-27 11:27:47.000000 networklab-1.5.1.dev1/netsim/ansible/templates/mpls/ios.6pe.j2
--rw-r--r--   0 pipi       (501) staff       (20)      611 2022-08-11 09:57:08.000000 networklab-1.5.1.dev1/netsim/ansible/templates/mpls/ios.bgp-lu.j2
--rw-r--r--   0 pipi       (501) staff       (20)      302 2022-08-27 11:27:47.000000 networklab-1.5.1.dev1/netsim/ansible/templates/mpls/ios.j2
--rw-r--r--   0 pipi       (501) staff       (20)      257 2022-04-01 07:43:22.000000 networklab-1.5.1.dev1/netsim/ansible/templates/mpls/ios.ldp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      326 2022-04-01 07:43:22.000000 networklab-1.5.1.dev1/netsim/ansible/templates/mpls/ios.mplsvpn.j2
--rw-r--r--   0 pipi       (501) staff       (20)      328 2022-12-19 09:40:05.000000 networklab-1.5.1.dev1/netsim/ansible/templates/mpls/junos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      542 2022-12-19 09:40:05.000000 networklab-1.5.1.dev1/netsim/ansible/templates/mpls/junos.ldp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      656 2022-12-19 09:40:05.000000 networklab-1.5.1.dev1/netsim/ansible/templates/mpls/junos.mplsvpn.j2
--rw-r--r--   0 pipi       (501) staff       (20)      151 2022-04-06 16:02:55.000000 networklab-1.5.1.dev1/netsim/ansible/templates/mpls/routeros.j2
--rw-r--r--   0 pipi       (501) staff       (20)      383 2022-04-06 16:02:55.000000 networklab-1.5.1.dev1/netsim/ansible/templates/mpls/routeros.ldp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      412 2022-04-06 16:02:55.000000 networklab-1.5.1.dev1/netsim/ansible/templates/mpls/routeros.mplsvpn.j2
--rw-r--r--   0 pipi       (501) staff       (20)      198 2022-10-19 17:10:38.000000 networklab-1.5.1.dev1/netsim/ansible/templates/mpls/routeros7.j2
--rw-r--r--   0 pipi       (501) staff       (20)      382 2022-10-19 17:10:38.000000 networklab-1.5.1.dev1/netsim/ansible/templates/mpls/routeros7.ldp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      408 2022-10-19 17:10:38.000000 networklab-1.5.1.dev1/netsim/ansible/templates/mpls/routeros7.mplsvpn.j2
--rw-r--r--   0 pipi       (501) staff       (20)      272 2022-11-04 10:28:02.000000 networklab-1.5.1.dev1/netsim/ansible/templates/mpls/sros.j2
--rw-r--r--   0 pipi       (501) staff       (20)      732 2022-11-04 10:28:02.000000 networklab-1.5.1.dev1/netsim/ansible/templates/mpls/sros.ldp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      432 2022-04-17 16:31:22.000000 networklab-1.5.1.dev1/netsim/ansible/templates/mpls/vyos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      462 2023-01-12 13:38:07.000000 networklab-1.5.1.dev1/netsim/ansible/templates/mpls/vyos.ldp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      668 2022-04-17 16:31:22.000000 networklab-1.5.1.dev1/netsim/ansible/templates/mpls/vyos.mplsvpn.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-03-29 16:28:22.018751 networklab-1.5.1.dev1/netsim/ansible/templates/ospf/
--rw-r--r--   0 pipi       (501) staff       (20)      488 2022-01-06 08:25:20.000000 networklab-1.5.1.dev1/netsim/ansible/templates/ospf/arcos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      199 2022-10-19 17:10:38.000000 networklab-1.5.1.dev1/netsim/ansible/templates/ospf/cumulus.j2
--rw-r--r--   0 pipi       (501) staff       (20)      778 2022-10-19 17:10:38.000000 networklab-1.5.1.dev1/netsim/ansible/templates/ospf/cumulus.ospfv2.j2
--rw-r--r--   0 pipi       (501) staff       (20)      791 2022-10-19 17:10:38.000000 networklab-1.5.1.dev1/netsim/ansible/templates/ospf/cumulus.ospfv3.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1228 2022-10-19 17:10:38.000000 networklab-1.5.1.dev1/netsim/ansible/templates/ospf/cumulus_nvue.j2
--rw-r--r--   0 pipi       (501) staff       (20)      200 2022-04-17 16:31:22.000000 networklab-1.5.1.dev1/netsim/ansible/templates/ospf/dellos10.j2
--rw-r--r--   0 pipi       (501) staff       (20)      838 2022-04-17 16:31:22.000000 networklab-1.5.1.dev1/netsim/ansible/templates/ospf/dellos10.ospfv2.j2
--rw-r--r--   0 pipi       (501) staff       (20)      834 2022-04-17 16:31:22.000000 networklab-1.5.1.dev1/netsim/ansible/templates/ospf/dellos10.ospfv3.j2
--rw-r--r--   0 pipi       (501) staff       (20)      190 2022-03-06 19:16:46.000000 networklab-1.5.1.dev1/netsim/ansible/templates/ospf/eos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1032 2022-02-14 14:03:36.000000 networklab-1.5.1.dev1/netsim/ansible/templates/ospf/eos.ospfv2.j2
--rw-r--r--   0 pipi       (501) staff       (20)      967 2022-09-04 08:58:45.000000 networklab-1.5.1.dev1/netsim/ansible/templates/ospf/eos.ospfv3.j2
--rw-r--r--   0 pipi       (501) staff       (20)      222 2022-10-19 17:10:38.000000 networklab-1.5.1.dev1/netsim/ansible/templates/ospf/frr.j2
--rw-r--r--   0 pipi       (501) staff       (20)      737 2023-01-12 13:38:07.000000 networklab-1.5.1.dev1/netsim/ansible/templates/ospf/frr.ospfv2.j2
--rw-r--r--   0 pipi       (501) staff       (20)      713 2022-12-20 07:49:03.000000 networklab-1.5.1.dev1/netsim/ansible/templates/ospf/frr.ospfv3.j2
--rw-r--r--   0 pipi       (501) staff       (20)      190 2022-03-06 19:16:05.000000 networklab-1.5.1.dev1/netsim/ansible/templates/ospf/ios.j2
--rw-r--r--   0 pipi       (501) staff       (20)      897 2022-02-14 14:03:36.000000 networklab-1.5.1.dev1/netsim/ansible/templates/ospf/ios.ospfv2.j2
--rw-r--r--   0 pipi       (501) staff       (20)      871 2022-02-14 14:03:36.000000 networklab-1.5.1.dev1/netsim/ansible/templates/ospf/ios.ospfv3.j2
--rw-r--r--   0 pipi       (501) staff       (20)      194 2023-01-12 13:38:07.000000 networklab-1.5.1.dev1/netsim/ansible/templates/ospf/iosxr.j2
--rw-r--r--   0 pipi       (501) staff       (20)      948 2023-01-12 13:38:07.000000 networklab-1.5.1.dev1/netsim/ansible/templates/ospf/iosxr.ospfv2.j2
--rw-r--r--   0 pipi       (501) staff       (20)      936 2023-01-12 13:38:07.000000 networklab-1.5.1.dev1/netsim/ansible/templates/ospf/iosxr.ospfv3.j2
--rw-r--r--   0 pipi       (501) staff       (20)      430 2022-12-19 09:40:05.000000 networklab-1.5.1.dev1/netsim/ansible/templates/ospf/junos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1082 2022-12-19 09:40:05.000000 networklab-1.5.1.dev1/netsim/ansible/templates/ospf/junos.ospfv2.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1084 2022-12-19 09:40:05.000000 networklab-1.5.1.dev1/netsim/ansible/templates/ospf/junos.ospfv3.j2
--rw-r--r--   0 pipi       (501) staff       (20)        0 2021-12-28 08:07:36.000000 networklab-1.5.1.dev1/netsim/ansible/templates/ospf/none.j2
--rw-r--r--   0 pipi       (501) staff       (20)      152 2022-10-19 17:10:38.000000 networklab-1.5.1.dev1/netsim/ansible/templates/ospf/nxos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      987 2022-10-19 17:10:38.000000 networklab-1.5.1.dev1/netsim/ansible/templates/ospf/nxos.ospfv2.j2
--rw-r--r--   0 pipi       (501) staff       (20)      995 2022-10-19 17:10:38.000000 networklab-1.5.1.dev1/netsim/ansible/templates/ospf/nxos.ospfv3.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2141 2022-04-06 16:02:55.000000 networklab-1.5.1.dev1/netsim/ansible/templates/ospf/routeros.j2
--rw-r--r--   0 pipi       (501) staff       (20)      478 2022-10-19 17:10:38.000000 networklab-1.5.1.dev1/netsim/ansible/templates/ospf/routeros7.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1983 2022-10-19 17:10:38.000000 networklab-1.5.1.dev1/netsim/ansible/templates/ospf/routeros7.ospf-include.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1145 2022-01-05 16:01:35.000000 networklab-1.5.1.dev1/netsim/ansible/templates/ospf/srlinux.cli.j2
--rw-r--r--   0 pipi       (501) staff       (20)      304 2022-08-27 11:27:47.000000 networklab-1.5.1.dev1/netsim/ansible/templates/ospf/srlinux.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1763 2022-12-07 08:01:39.000000 networklab-1.5.1.dev1/netsim/ansible/templates/ospf/srlinux.macro.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1513 2023-03-29 08:59:57.000000 networklab-1.5.1.dev1/netsim/ansible/templates/ospf/sros.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1038 2022-01-21 21:00:25.000000 networklab-1.5.1.dev1/netsim/ansible/templates/ospf/sros.md-cli.j2
--rw-r--r--   0 pipi       (501) staff       (20)      618 2021-12-28 08:07:36.000000 networklab-1.5.1.dev1/netsim/ansible/templates/ospf/sros.openconfig.j2
--rw-r--r--   0 pipi       (501) staff       (20)      385 2022-03-09 10:04:56.000000 networklab-1.5.1.dev1/netsim/ansible/templates/ospf/vyos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      957 2022-08-27 11:27:47.000000 networklab-1.5.1.dev1/netsim/ansible/templates/ospf/vyos.ospfv2.j2
--rw-r--r--   0 pipi       (501) staff       (20)      869 2022-08-27 11:27:47.000000 networklab-1.5.1.dev1/netsim/ansible/templates/ospf/vyos.ospfv3.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-03-29 16:28:22.022354 networklab-1.5.1.dev1/netsim/ansible/templates/sr/
--rw-r--r--   0 pipi       (501) staff       (20)      245 2021-07-09 15:23:10.000000 networklab-1.5.1.dev1/netsim/ansible/templates/sr/eos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      270 2021-07-09 15:23:10.000000 networklab-1.5.1.dev1/netsim/ansible/templates/sr/ios.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1127 2023-01-12 13:45:42.000000 networklab-1.5.1.dev1/netsim/ansible/templates/sr/junos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2286 2023-01-04 17:29:57.000000 networklab-1.5.1.dev1/netsim/ansible/templates/sr/srlinux.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1237 2023-01-04 17:30:40.000000 networklab-1.5.1.dev1/netsim/ansible/templates/sr/sros.j2
--rw-r--r--   0 pipi       (501) staff       (20)      945 2021-12-28 08:07:36.000000 networklab-1.5.1.dev1/netsim/ansible/templates/sr/sros.openconfig.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-03-29 16:28:22.022673 networklab-1.5.1.dev1/netsim/ansible/templates/srv6/
--rw-r--r--   0 pipi       (501) staff       (20)     4092 2022-10-19 17:10:38.000000 networklab-1.5.1.dev1/netsim/ansible/templates/srv6/sros.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-03-29 16:28:22.026132 networklab-1.5.1.dev1/netsim/ansible/templates/vlan/
--rw-r--r--   0 pipi       (501) staff       (20)     1186 2022-12-18 14:12:35.000000 networklab-1.5.1.dev1/netsim/ansible/templates/vlan/csr.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1730 2022-12-18 14:12:35.000000 networklab-1.5.1.dev1/netsim/ansible/templates/vlan/cumulus.j2
--rw-r--r--   0 pipi       (501) staff       (20)      949 2022-11-17 08:20:15.000000 networklab-1.5.1.dev1/netsim/ansible/templates/vlan/dellos10.j2
--rw-r--r--   0 pipi       (501) staff       (20)      757 2022-12-15 11:32:15.000000 networklab-1.5.1.dev1/netsim/ansible/templates/vlan/eos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1212 2022-10-19 17:10:38.000000 networklab-1.5.1.dev1/netsim/ansible/templates/vlan/frr.j2
--rw-r--r--   0 pipi       (501) staff       (20)      457 2022-12-14 07:49:35.000000 networklab-1.5.1.dev1/netsim/ansible/templates/vlan/ios.j2
--rw-r--r--   0 pipi       (501) staff       (20)      776 2022-08-27 11:27:47.000000 networklab-1.5.1.dev1/netsim/ansible/templates/vlan/nxos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      432 2022-06-20 08:57:47.000000 networklab-1.5.1.dev1/netsim/ansible/templates/vlan/routeros.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1115 2022-10-19 17:10:38.000000 networklab-1.5.1.dev1/netsim/ansible/templates/vlan/routeros7.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2756 2022-10-19 17:10:38.000000 networklab-1.5.1.dev1/netsim/ansible/templates/vlan/srlinux.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1909 2023-03-29 16:02:34.000000 networklab-1.5.1.dev1/netsim/ansible/templates/vlan/sros.j2
--rw-r--r--   0 pipi       (501) staff       (20)      815 2022-12-19 09:40:05.000000 networklab-1.5.1.dev1/netsim/ansible/templates/vlan/vmx.j2
--rw-r--r--   0 pipi       (501) staff       (20)       25 2022-12-19 09:40:05.000000 networklab-1.5.1.dev1/netsim/ansible/templates/vlan/vsrx.j2
--rw-r--r--   0 pipi       (501) staff       (20)      771 2022-06-20 08:57:47.000000 networklab-1.5.1.dev1/netsim/ansible/templates/vlan/vyos.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-03-29 16:28:22.036935 networklab-1.5.1.dev1/netsim/ansible/templates/vrf/
--rw-r--r--   0 pipi       (501) staff       (20)      492 2022-10-19 17:10:38.000000 networklab-1.5.1.dev1/netsim/ansible/templates/vrf/cumulus.j2
--rw-r--r--   0 pipi       (501) staff       (20)      106 2022-04-17 16:31:22.000000 networklab-1.5.1.dev1/netsim/ansible/templates/vrf/cumulus_nvue.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2010 2022-10-19 17:10:38.000000 networklab-1.5.1.dev1/netsim/ansible/templates/vrf/dellos10.bgp-macro.j2
--rw-r--r--   0 pipi       (501) staff       (20)      690 2022-08-27 11:27:47.000000 networklab-1.5.1.dev1/netsim/ansible/templates/vrf/dellos10.bgp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      182 2022-09-10 16:16:52.000000 networklab-1.5.1.dev1/netsim/ansible/templates/vrf/dellos10.j2
--rw-r--r--   0 pipi       (501) staff       (20)      888 2022-09-10 16:21:58.000000 networklab-1.5.1.dev1/netsim/ansible/templates/vrf/dellos10.ospfv2-vrf.j2
--rw-r--r--   0 pipi       (501) staff       (20)      911 2022-10-19 17:10:38.000000 networklab-1.5.1.dev1/netsim/ansible/templates/vrf/eos.bgp-macro.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1189 2022-10-19 17:10:38.000000 networklab-1.5.1.dev1/netsim/ansible/templates/vrf/eos.bgp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      172 2022-09-11 07:35:29.000000 networklab-1.5.1.dev1/netsim/ansible/templates/vrf/eos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1027 2022-05-02 06:40:29.000000 networklab-1.5.1.dev1/netsim/ansible/templates/vrf/eos.ospfv2-vrf.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1679 2023-01-12 13:38:07.000000 networklab-1.5.1.dev1/netsim/ansible/templates/vrf/frr.bgp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      412 2022-10-24 12:44:53.000000 networklab-1.5.1.dev1/netsim/ansible/templates/vrf/frr.frr-config.j2
--rw-r--r--   0 pipi       (501) staff       (20)      524 2023-01-12 13:38:07.000000 networklab-1.5.1.dev1/netsim/ansible/templates/vrf/frr.j2
--rw-r--r--   0 pipi       (501) staff       (20)      762 2023-01-12 13:38:07.000000 networklab-1.5.1.dev1/netsim/ansible/templates/vrf/frr.ospfv2-vrf.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1539 2022-12-21 09:06:32.000000 networklab-1.5.1.dev1/netsim/ansible/templates/vrf/ios.bgp-macro.j2
--rw-r--r--   0 pipi       (501) staff       (20)      716 2022-10-19 17:10:38.000000 networklab-1.5.1.dev1/netsim/ansible/templates/vrf/ios.bgp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      172 2022-09-10 16:23:03.000000 networklab-1.5.1.dev1/netsim/ansible/templates/vrf/ios.j2
--rw-r--r--   0 pipi       (501) staff       (20)      880 2022-10-24 08:27:03.000000 networklab-1.5.1.dev1/netsim/ansible/templates/vrf/ios.ospfv2-vrf.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2169 2022-12-19 09:40:05.000000 networklab-1.5.1.dev1/netsim/ansible/templates/vrf/junos.bgp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      693 2022-12-19 09:40:05.000000 networklab-1.5.1.dev1/netsim/ansible/templates/vrf/junos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1169 2022-12-19 09:40:05.000000 networklab-1.5.1.dev1/netsim/ansible/templates/vrf/junos.ospfv2-vrf.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1423 2022-08-27 11:27:47.000000 networklab-1.5.1.dev1/netsim/ansible/templates/vrf/nxos.bgp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      173 2022-08-27 11:27:47.000000 networklab-1.5.1.dev1/netsim/ansible/templates/vrf/nxos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      989 2022-08-27 11:27:47.000000 networklab-1.5.1.dev1/netsim/ansible/templates/vrf/nxos.ospfv2-vrf.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1109 2022-04-16 08:35:35.000000 networklab-1.5.1.dev1/netsim/ansible/templates/vrf/routeros.bgp-macro.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1540 2022-08-18 15:19:05.000000 networklab-1.5.1.dev1/netsim/ansible/templates/vrf/routeros.bgp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      182 2022-04-06 16:02:55.000000 networklab-1.5.1.dev1/netsim/ansible/templates/vrf/routeros.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1721 2022-05-01 16:20:27.000000 networklab-1.5.1.dev1/netsim/ansible/templates/vrf/routeros.ospfv2-vrf.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1401 2022-10-19 17:10:38.000000 networklab-1.5.1.dev1/netsim/ansible/templates/vrf/routeros7.bgp-macro.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1095 2022-10-19 17:10:38.000000 networklab-1.5.1.dev1/netsim/ansible/templates/vrf/routeros7.bgp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      185 2022-10-19 17:10:38.000000 networklab-1.5.1.dev1/netsim/ansible/templates/vrf/routeros7.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1983 2022-10-19 17:10:38.000000 networklab-1.5.1.dev1/netsim/ansible/templates/vrf/routeros7.ospf-include.j2
--rw-r--r--   0 pipi       (501) staff       (20)      463 2022-10-19 17:10:38.000000 networklab-1.5.1.dev1/netsim/ansible/templates/vrf/routeros7.ospfv2-vrf.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1276 2022-10-19 17:10:38.000000 networklab-1.5.1.dev1/netsim/ansible/templates/vrf/srlinux.j2
--rw-r--r--   0 pipi       (501) staff       (20)      464 2022-10-19 17:10:38.000000 networklab-1.5.1.dev1/netsim/ansible/templates/vrf/sros.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1323 2022-10-19 17:10:38.000000 networklab-1.5.1.dev1/netsim/ansible/templates/vrf/vyos.bgp-macro.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1272 2022-12-07 14:41:22.000000 networklab-1.5.1.dev1/netsim/ansible/templates/vrf/vyos.bgp.j2
--rw-r--r--   0 pipi       (501) staff       (20)      535 2022-04-17 16:31:22.000000 networklab-1.5.1.dev1/netsim/ansible/templates/vrf/vyos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1037 2022-04-17 16:31:22.000000 networklab-1.5.1.dev1/netsim/ansible/templates/vrf/vyos.ospfv2-vrf.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-03-29 16:28:22.039032 networklab-1.5.1.dev1/netsim/ansible/templates/vxlan/
--rw-r--r--   0 pipi       (501) staff       (20)      570 2022-12-18 14:12:35.000000 networklab-1.5.1.dev1/netsim/ansible/templates/vxlan/csr.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1011 2022-12-15 13:56:36.000000 networklab-1.5.1.dev1/netsim/ansible/templates/vxlan/cumulus.j2
--rw-r--r--   0 pipi       (501) staff       (20)      420 2022-09-16 11:40:01.000000 networklab-1.5.1.dev1/netsim/ansible/templates/vxlan/dellos10.j2
--rw-r--r--   0 pipi       (501) staff       (20)      381 2022-12-15 14:02:16.000000 networklab-1.5.1.dev1/netsim/ansible/templates/vxlan/eos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1651 2022-10-19 17:10:38.000000 networklab-1.5.1.dev1/netsim/ansible/templates/vxlan/frr.j2
--rw-r--r--   0 pipi       (501) staff       (20)      662 2022-12-15 14:02:29.000000 networklab-1.5.1.dev1/netsim/ansible/templates/vxlan/nxos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2219 2022-11-04 10:28:02.000000 networklab-1.5.1.dev1/netsim/ansible/templates/vxlan/srlinux.j2
--rw-r--r--   0 pipi       (501) staff       (20)     2579 2022-11-04 10:28:02.000000 networklab-1.5.1.dev1/netsim/ansible/templates/vxlan/sros.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1315 2022-09-16 11:40:09.000000 networklab-1.5.1.dev1/netsim/ansible/templates/vxlan/vyos.j2
--rw-r--r--   0 pipi       (501) staff       (20)      740 2022-11-04 10:28:02.000000 networklab-1.5.1.dev1/netsim/api.py
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-03-29 16:28:22.041366 networklab-1.5.1.dev1/netsim/augment/
--rw-r--r--   0 pipi       (501) staff       (20)      205 2023-01-28 06:30:20.000000 networklab-1.5.1.dev1/netsim/augment/__init__.py
--rw-r--r--   0 pipi       (501) staff       (20)     2803 2023-01-28 06:30:20.000000 networklab-1.5.1.dev1/netsim/augment/config.py
--rw-r--r--   0 pipi       (501) staff       (20)     3328 2023-03-27 09:52:30.000000 networklab-1.5.1.dev1/netsim/augment/devices.py
--rw-r--r--   0 pipi       (501) staff       (20)    16957 2023-03-26 10:09:05.000000 networklab-1.5.1.dev1/netsim/augment/groups.py
--rw-r--r--   0 pipi       (501) staff       (20)    39639 2023-03-27 16:51:17.000000 networklab-1.5.1.dev1/netsim/augment/links.py
--rw-r--r--   0 pipi       (501) staff       (20)     3088 2023-03-27 09:52:30.000000 networklab-1.5.1.dev1/netsim/augment/main.py
--rw-r--r--   0 pipi       (501) staff       (20)    12316 2023-03-26 10:09:05.000000 networklab-1.5.1.dev1/netsim/augment/nodes.py
--rw-r--r--   0 pipi       (501) staff       (20)     2833 2023-01-28 06:30:20.000000 networklab-1.5.1.dev1/netsim/augment/plugin.py
--rw-r--r--   0 pipi       (501) staff       (20)     5710 2023-01-28 06:30:20.000000 networklab-1.5.1.dev1/netsim/augment/topology.py
--rw-r--r--   0 pipi       (501) staff       (20)     1152 2023-01-28 06:30:20.000000 networklab-1.5.1.dev1/netsim/callback.py
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-03-29 16:28:22.046914 networklab-1.5.1.dev1/netsim/cli/
--rwxr-xr-x   0 pipi       (501) staff       (20)     8522 2023-03-29 09:00:02.000000 networklab-1.5.1.dev1/netsim/cli/__init__.py
--rw-r--r--   0 pipi       (501) staff       (20)      319 2022-08-23 07:24:58.000000 networklab-1.5.1.dev1/netsim/cli/alias.txt
--rw-r--r--   0 pipi       (501) staff       (20)     1758 2022-03-20 09:00:36.000000 networklab-1.5.1.dev1/netsim/cli/ansible.py
--rw-r--r--   0 pipi       (501) staff       (20)     4192 2022-12-11 09:34:30.000000 networklab-1.5.1.dev1/netsim/cli/clab.py
--rw-r--r--   0 pipi       (501) staff       (20)     2680 2022-03-20 09:12:02.000000 networklab-1.5.1.dev1/netsim/cli/collect.py
--rw-r--r--   0 pipi       (501) staff       (20)     1392 2022-03-07 15:33:10.000000 networklab-1.5.1.dev1/netsim/cli/config.py
--rw-r--r--   0 pipi       (501) staff       (20)     3684 2022-12-14 06:39:46.000000 networklab-1.5.1.dev1/netsim/cli/connect.py
--rw-r--r--   0 pipi       (501) staff       (20)     2966 2022-11-04 10:28:02.000000 networklab-1.5.1.dev1/netsim/cli/create.py
--rw-r--r--   0 pipi       (501) staff       (20)     5275 2023-03-29 09:00:02.000000 networklab-1.5.1.dev1/netsim/cli/down.py
--rw-r--r--   0 pipi       (501) staff       (20)       63 2023-03-06 07:47:06.000000 networklab-1.5.1.dev1/netsim/cli/empty.yml
--rw-r--r--   0 pipi       (501) staff       (20)     3362 2023-01-28 06:30:20.000000 networklab-1.5.1.dev1/netsim/cli/external_commands.py
--rw-r--r--   0 pipi       (501) staff       (20)     3181 2023-03-29 09:00:02.000000 networklab-1.5.1.dev1/netsim/cli/initial.py
--rw-r--r--   0 pipi       (501) staff       (20)     2038 2021-12-28 08:07:36.000000 networklab-1.5.1.dev1/netsim/cli/install.py
--rw-r--r--   0 pipi       (501) staff       (20)     9143 2023-03-29 09:10:21.000000 networklab-1.5.1.dev1/netsim/cli/libvirt.py
--rw-r--r--   0 pipi       (501) staff       (20)     1332 2023-01-15 15:54:21.000000 networklab-1.5.1.dev1/netsim/cli/read.py
--rw-r--r--   0 pipi       (501) staff       (20)     1408 2022-05-02 06:40:29.000000 networklab-1.5.1.dev1/netsim/cli/restart.py
--rw-r--r--   0 pipi       (501) staff       (20)     4428 2023-03-06 07:47:06.000000 networklab-1.5.1.dev1/netsim/cli/show.py
--rw-r--r--   0 pipi       (501) staff       (20)     4785 2023-03-29 09:00:02.000000 networklab-1.5.1.dev1/netsim/cli/status.py
--rw-r--r--   0 pipi       (501) staff       (20)     3453 2023-01-28 06:30:20.000000 networklab-1.5.1.dev1/netsim/cli/test.py
--rw-r--r--   0 pipi       (501) staff       (20)     9366 2023-03-29 09:00:02.000000 networklab-1.5.1.dev1/netsim/cli/up.py
--rw-r--r--   0 pipi       (501) staff       (20)      417 2021-06-25 12:25:32.000000 networklab-1.5.1.dev1/netsim/cli/usage.py
--rw-r--r--   0 pipi       (501) staff       (20)     1937 2022-08-27 11:27:47.000000 networklab-1.5.1.dev1/netsim/cli/usage.txt
--rw-r--r--   0 pipi       (501) staff       (20)      180 2022-08-27 11:27:47.000000 networklab-1.5.1.dev1/netsim/cli/version.py
--rw-r--r--   0 pipi       (501) staff       (20)     3322 2023-01-28 06:30:20.000000 networklab-1.5.1.dev1/netsim/common.py
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-03-29 16:28:22.048011 networklab-1.5.1.dev1/netsim/data/
--rw-r--r--   0 pipi       (501) staff       (20)     5148 2023-01-25 18:53:29.000000 networklab-1.5.1.dev1/netsim/data/__init__.py
--rw-r--r--   0 pipi       (501) staff       (20)     1097 2022-11-04 10:28:02.000000 networklab-1.5.1.dev1/netsim/data/global_vars.py
--rw-r--r--   0 pipi       (501) staff       (20)    20668 2023-03-26 10:09:05.000000 networklab-1.5.1.dev1/netsim/data/types.py
--rw-r--r--   0 pipi       (501) staff       (20)    19276 2023-03-26 10:09:05.000000 networklab-1.5.1.dev1/netsim/data/validate.py
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-03-29 16:28:22.049421 networklab-1.5.1.dev1/netsim/defaults/
--rw-r--r--   0 pipi       (501) staff       (20)      294 2023-01-28 06:30:20.000000 networklab-1.5.1.dev1/netsim/defaults/addressing.yml
--rw-r--r--   0 pipi       (501) staff       (20)     2282 2023-03-26 10:09:05.000000 networklab-1.5.1.dev1/netsim/defaults/attributes.yml
--rw-r--r--   0 pipi       (501) staff       (20)      112 2023-01-28 06:30:20.000000 networklab-1.5.1.dev1/netsim/defaults/automation.yml
--rw-r--r--   0 pipi       (501) staff       (20)      378 2023-01-28 06:30:20.000000 networklab-1.5.1.dev1/netsim/defaults/hints.yml
--rw-r--r--   0 pipi       (501) staff       (20)      363 2023-01-28 06:30:20.000000 networklab-1.5.1.dev1/netsim/defaults/multilab.yml
--rw-r--r--   0 pipi       (501) staff       (20)       86 2023-01-28 06:30:20.000000 networklab-1.5.1.dev1/netsim/defaults/ports.yml
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-03-29 16:28:22.059099 networklab-1.5.1.dev1/netsim/devices/
--rw-r--r--   0 pipi       (501) staff       (20)     1844 2023-01-28 06:30:20.000000 networklab-1.5.1.dev1/netsim/devices/__init__.py
--rw-r--r--   0 pipi       (501) staff       (20)      996 2023-01-28 06:30:20.000000 networklab-1.5.1.dev1/netsim/devices/asav.py
--rw-r--r--   0 pipi       (501) staff       (20)      798 2023-03-26 10:09:05.000000 networklab-1.5.1.dev1/netsim/devices/asav.yml
--rw-r--r--   0 pipi       (501) staff       (20)     1184 2023-01-28 06:30:20.000000 networklab-1.5.1.dev1/netsim/devices/csr.yml
--rw-r--r--   0 pipi       (501) staff       (20)     1049 2023-01-28 06:30:20.000000 networklab-1.5.1.dev1/netsim/devices/cumulus.yml
--rw-r--r--   0 pipi       (501) staff       (20)      748 2023-01-28 06:30:20.000000 networklab-1.5.1.dev1/netsim/devices/cumulus_nvue.yml
--rw-r--r--   0 pipi       (501) staff       (20)     1152 2023-01-28 06:30:20.000000 networklab-1.5.1.dev1/netsim/devices/dellos10.yml
--rw-r--r--   0 pipi       (501) staff       (20)     2273 2023-01-28 06:30:20.000000 networklab-1.5.1.dev1/netsim/devices/eos.py
--rw-r--r--   0 pipi       (501) staff       (20)     1554 2023-02-12 08:44:04.000000 networklab-1.5.1.dev1/netsim/devices/eos.yml
--rw-r--r--   0 pipi       (501) staff       (20)      502 2023-01-28 06:30:20.000000 networklab-1.5.1.dev1/netsim/devices/fortios.yml
--rw-r--r--   0 pipi       (501) staff       (20)      927 2023-01-28 06:30:20.000000 networklab-1.5.1.dev1/netsim/devices/frr.yml
--rw-r--r--   0 pipi       (501) staff       (20)      854 2023-01-28 06:30:20.000000 networklab-1.5.1.dev1/netsim/devices/iosv.py
--rw-r--r--   0 pipi       (501) staff       (20)     1372 2023-01-28 06:30:20.000000 networklab-1.5.1.dev1/netsim/devices/iosv.yml
--rw-r--r--   0 pipi       (501) staff       (20)      949 2023-01-28 06:30:20.000000 networklab-1.5.1.dev1/netsim/devices/iosxr.yml
--rw-r--r--   0 pipi       (501) staff       (20)     2346 2023-01-28 06:30:20.000000 networklab-1.5.1.dev1/netsim/devices/junos.py
--rw-r--r--   0 pipi       (501) staff       (20)      705 2023-01-28 06:30:20.000000 networklab-1.5.1.dev1/netsim/devices/linux.yml
--rw-r--r--   0 pipi       (501) staff       (20)     1109 2023-01-28 06:30:20.000000 networklab-1.5.1.dev1/netsim/devices/none.yml
--rw-r--r--   0 pipi       (501) staff       (20)      858 2023-01-28 06:30:20.000000 networklab-1.5.1.dev1/netsim/devices/nxos.yml
--rw-r--r--   0 pipi       (501) staff       (20)      507 2023-01-28 06:30:20.000000 networklab-1.5.1.dev1/netsim/devices/routeros.yml
--rw-r--r--   0 pipi       (501) staff       (20)      910 2023-01-28 06:30:20.000000 networklab-1.5.1.dev1/netsim/devices/routeros7.yml
--rw-r--r--   0 pipi       (501) staff       (20)     1311 2023-01-28 06:30:20.000000 networklab-1.5.1.dev1/netsim/devices/srlinux.yml
--rw-r--r--   0 pipi       (501) staff       (20)     1634 2023-01-28 06:30:20.000000 networklab-1.5.1.dev1/netsim/devices/sros.yml
--rw-r--r--   0 pipi       (501) staff       (20)     2346 2023-01-28 06:30:20.000000 networklab-1.5.1.dev1/netsim/devices/vmx.py
--rw-r--r--   0 pipi       (501) staff       (20)      827 2023-01-28 06:30:20.000000 networklab-1.5.1.dev1/netsim/devices/vmx.yml
--rw-r--r--   0 pipi       (501) staff       (20)     2346 2023-01-28 06:30:20.000000 networklab-1.5.1.dev1/netsim/devices/vsrx.py
--rw-r--r--   0 pipi       (501) staff       (20)     1098 2023-01-28 06:30:20.000000 networklab-1.5.1.dev1/netsim/devices/vsrx.yml
--rw-r--r--   0 pipi       (501) staff       (20)     1008 2023-01-28 06:30:20.000000 networklab-1.5.1.dev1/netsim/devices/vyos.yml
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-03-29 16:28:21.938709 networklab-1.5.1.dev1/netsim/extra/
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-03-29 16:28:22.059291 networklab-1.5.1.dev1/netsim/extra/__pycache__/
--rw-r--r--   0 pipi       (501) staff       (20)     2215 2022-09-04 16:06:08.000000 networklab-1.5.1.dev1/netsim/extra/__pycache__/ebgp-local_as.cpython-39.pyc
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-03-29 16:28:22.062377 networklab-1.5.1.dev1/netsim/extra/ebgp.utils/
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-03-29 16:28:22.062556 networklab-1.5.1.dev1/netsim/extra/ebgp.utils/__pycache__/
--rw-r--r--   0 pipi       (501) staff       (20)     2171 2023-02-02 15:17:54.000000 networklab-1.5.1.dev1/netsim/extra/ebgp.utils/__pycache__/plugin.cpython-310.pyc
--rw-r--r--   0 pipi       (501) staff       (20)      681 2022-12-22 16:28:14.000000 networklab-1.5.1.dev1/netsim/extra/ebgp.utils/default-originate.yml
--rw-r--r--   0 pipi       (501) staff       (20)     1198 2022-08-27 11:27:47.000000 networklab-1.5.1.dev1/netsim/extra/ebgp.utils/eos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1528 2022-08-27 11:27:47.000000 networklab-1.5.1.dev1/netsim/extra/ebgp.utils/ios.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1891 2022-12-19 09:40:05.000000 networklab-1.5.1.dev1/netsim/extra/ebgp.utils/junos.j2
--rw-r--r--   0 pipi       (501) staff       (20)     4428 2023-01-28 06:30:20.000000 networklab-1.5.1.dev1/netsim/extra/ebgp.utils/plugin.py
--rw-r--r--   0 pipi       (501) staff       (20)     2924 2022-10-19 17:10:38.000000 networklab-1.5.1.dev1/netsim/extra/ebgp.utils/routeros7.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1695 2022-10-19 17:10:38.000000 networklab-1.5.1.dev1/netsim/extra/ebgp.utils/srlinux.j2
--rw-r--r--   0 pipi       (501) staff       (20)      263 2022-08-21 12:51:31.000000 networklab-1.5.1.dev1/netsim/extra/ebgp.utils/topology.yml
--rw-r--r--   0 pipi       (501) staff       (20)     2877 2022-08-27 11:27:47.000000 networklab-1.5.1.dev1/netsim/extra/ebgp.utils/vyos.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-03-29 16:28:22.062825 networklab-1.5.1.dev1/netsim/extra/multilab/
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-03-29 16:28:22.063157 networklab-1.5.1.dev1/netsim/extra/multilab/__pycache__/
--rw-r--r--   0 pipi       (501) staff       (20)     1787 2023-01-30 16:32:51.000000 networklab-1.5.1.dev1/netsim/extra/multilab/__pycache__/plugin.cpython-310.pyc
--rw-r--r--   0 pipi       (501) staff       (20)     3051 2023-02-07 15:05:29.000000 networklab-1.5.1.dev1/netsim/extra/multilab/plugin.py
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-03-29 16:28:22.063446 networklab-1.5.1.dev1/netsim/extra/none/
--rw-r--r--   0 pipi       (501) staff       (20)        0 2021-12-28 08:07:36.000000 networklab-1.5.1.dev1/netsim/extra/none/none.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-03-29 16:28:22.064057 networklab-1.5.1.dev1/netsim/extra/proxy-arp/
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-03-29 16:28:22.064596 networklab-1.5.1.dev1/netsim/extra/proxy-arp/__pycache__/
--rw-r--r--   0 pipi       (501) staff       (20)     1098 2023-02-02 15:17:59.000000 networklab-1.5.1.dev1/netsim/extra/proxy-arp/__pycache__/plugin.cpython-310.pyc
--rw-r--r--   0 pipi       (501) staff       (20)      934 2022-10-24 08:42:48.000000 networklab-1.5.1.dev1/netsim/extra/proxy-arp/__pycache__/plugin.cpython-39.pyc
--rw-r--r--   0 pipi       (501) staff       (20)      890 2023-01-28 06:30:20.000000 networklab-1.5.1.dev1/netsim/extra/proxy-arp/plugin.py
--rw-r--r--   0 pipi       (501) staff       (20)      717 2022-11-04 10:28:02.000000 networklab-1.5.1.dev1/netsim/extra/proxy-arp/srlinux.j2
--rw-r--r--   0 pipi       (501) staff       (20)      682 2022-11-04 10:28:02.000000 networklab-1.5.1.dev1/netsim/extra/proxy-arp/sros.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-03-29 16:28:22.066212 networklab-1.5.1.dev1/netsim/install/
--rwxr--r--   0 pipi       (501) staff       (20)     2162 2023-03-13 11:11:29.000000 networklab-1.5.1.dev1/netsim/install/ansible.sh
--rwxr-xr-x   0 pipi       (501) staff       (20)     3484 2022-11-04 10:28:02.000000 networklab-1.5.1.dev1/netsim/install/containerlab.sh
--rwxr-xr-x   0 pipi       (501) staff       (20)      745 2023-01-13 19:14:18.000000 networklab-1.5.1.dev1/netsim/install/grpc.sh
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-03-29 16:28:22.069126 networklab-1.5.1.dev1/netsim/install/libvirt/
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-03-29 16:28:22.069375 networklab-1.5.1.dev1/netsim/install/libvirt/asav/
--rw-r--r--   0 pipi       (501) staff       (20)      972 2023-03-26 10:09:05.000000 networklab-1.5.1.dev1/netsim/install/libvirt/asav/day0-config
--rw-r--r--   0 pipi       (501) staff       (20)      369 2023-03-26 10:09:05.000000 networklab-1.5.1.dev1/netsim/install/libvirt/asav.txt
--rw-r--r--   0 pipi       (501) staff       (20)     1219 2022-12-11 18:08:47.000000 networklab-1.5.1.dev1/netsim/install/libvirt/csr.txt
--rw-r--r--   0 pipi       (501) staff       (20)     1493 2022-04-17 16:31:22.000000 networklab-1.5.1.dev1/netsim/install/libvirt/dellos10.txt
--rw-r--r--   0 pipi       (501) staff       (20)     2214 2022-03-09 10:04:56.000000 networklab-1.5.1.dev1/netsim/install/libvirt/eos.txt
--rw-r--r--   0 pipi       (501) staff       (20)     1531 2022-10-19 17:10:38.000000 networklab-1.5.1.dev1/netsim/install/libvirt/eos.xml.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1665 2022-10-19 17:10:38.000000 networklab-1.5.1.dev1/netsim/install/libvirt/iosv.txt
--rw-r--r--   0 pipi       (501) staff       (20)     2911 2022-10-19 17:10:38.000000 networklab-1.5.1.dev1/netsim/install/libvirt/iosv.xml.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-03-29 16:28:22.069594 networklab-1.5.1.dev1/netsim/install/libvirt/iosxr/
--rw-r--r--   0 pipi       (501) staff       (20)      360 2022-12-21 10:32:36.000000 networklab-1.5.1.dev1/netsim/install/libvirt/iosxr/iosxr_config.txt
--rw-r--r--   0 pipi       (501) staff       (20)     1044 2023-01-12 13:38:07.000000 networklab-1.5.1.dev1/netsim/install/libvirt/iosxr.txt
--rw-r--r--   0 pipi       (501) staff       (20)     1524 2022-01-28 18:41:01.000000 networklab-1.5.1.dev1/netsim/install/libvirt/nxos.txt
--rw-r--r--   0 pipi       (501) staff       (20)     1523 2022-09-25 07:16:04.000000 networklab-1.5.1.dev1/netsim/install/libvirt/nxos.xml.j2
--rw-r--r--   0 pipi       (501) staff       (20)      940 2022-10-19 17:10:38.000000 networklab-1.5.1.dev1/netsim/install/libvirt/routeros7.txt
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-03-29 16:28:22.069846 networklab-1.5.1.dev1/netsim/install/libvirt/vsrx/
--rw-r--r--   0 pipi       (501) staff       (20)     2243 2022-03-09 10:04:56.000000 networklab-1.5.1.dev1/netsim/install/libvirt/vsrx/juniper.conf
--rw-r--r--   0 pipi       (501) staff       (20)      540 2022-03-09 10:04:56.000000 networklab-1.5.1.dev1/netsim/install/libvirt/vsrx.txt
--rwxr-xr-x   0 pipi       (501) staff       (20)     3179 2023-01-12 13:45:42.000000 networklab-1.5.1.dev1/netsim/install/libvirt.sh
--rwxr-xr-x   0 pipi       (501) staff       (20)     1881 2022-11-04 10:28:02.000000 networklab-1.5.1.dev1/netsim/install/ubuntu.sh
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-03-29 16:28:22.078066 networklab-1.5.1.dev1/netsim/modules/
--rw-r--r--   0 pipi       (501) staff       (20)    21902 2023-01-28 06:30:20.000000 networklab-1.5.1.dev1/netsim/modules/__init__.py
--rw-r--r--   0 pipi       (501) staff       (20)     6194 2023-03-26 10:09:05.000000 networklab-1.5.1.dev1/netsim/modules/_dataplane.py
--rw-r--r--   0 pipi       (501) staff       (20)    10483 2023-01-14 11:38:47.000000 networklab-1.5.1.dev1/netsim/modules/_routing.py
--rw-r--r--   0 pipi       (501) staff       (20)     3923 2023-01-14 09:41:51.000000 networklab-1.5.1.dev1/netsim/modules/bfd.py
--rw-r--r--   0 pipi       (501) staff       (20)      693 2023-01-28 06:30:20.000000 networklab-1.5.1.dev1/netsim/modules/bfd.yml
--rw-r--r--   0 pipi       (501) staff       (20)    20279 2023-03-20 10:56:19.000000 networklab-1.5.1.dev1/netsim/modules/bgp.py
--rw-r--r--   0 pipi       (501) staff       (20)     1461 2023-03-20 10:39:39.000000 networklab-1.5.1.dev1/netsim/modules/bgp.yml
--rw-r--r--   0 pipi       (501) staff       (20)      496 2023-01-12 16:03:44.000000 networklab-1.5.1.dev1/netsim/modules/eigrp.py
--rw-r--r--   0 pipi       (501) staff       (20)      324 2023-01-28 06:30:20.000000 networklab-1.5.1.dev1/netsim/modules/eigrp.yml
--rw-r--r--   0 pipi       (501) staff       (20)    17812 2022-11-13 15:34:41.000000 networklab-1.5.1.dev1/netsim/modules/evpn.py
--rw-r--r--   0 pipi       (501) staff       (20)      883 2023-01-28 06:30:20.000000 networklab-1.5.1.dev1/netsim/modules/evpn.yml
--rw-r--r--   0 pipi       (501) staff       (20)     6795 2023-03-26 10:09:05.000000 networklab-1.5.1.dev1/netsim/modules/gateway.py
--rw-r--r--   0 pipi       (501) staff       (20)      951 2023-01-28 06:30:20.000000 networklab-1.5.1.dev1/netsim/modules/gateway.yml
--rw-r--r--   0 pipi       (501) staff       (20)     2579 2023-01-12 13:38:07.000000 networklab-1.5.1.dev1/netsim/modules/isis.py
--rw-r--r--   0 pipi       (501) staff       (20)      906 2023-01-28 06:30:20.000000 networklab-1.5.1.dev1/netsim/modules/isis.yml
--rw-r--r--   0 pipi       (501) staff       (20)     7057 2023-01-28 06:30:20.000000 networklab-1.5.1.dev1/netsim/modules/mpls.py
--rw-r--r--   0 pipi       (501) staff       (20)      870 2023-01-28 06:30:20.000000 networklab-1.5.1.dev1/netsim/modules/mpls.yml
--rw-r--r--   0 pipi       (501) staff       (20)     3036 2023-01-14 10:57:46.000000 networklab-1.5.1.dev1/netsim/modules/ospf.py
--rw-r--r--   0 pipi       (501) staff       (20)     1024 2023-01-28 06:30:20.000000 networklab-1.5.1.dev1/netsim/modules/ospf.yml
--rw-r--r--   0 pipi       (501) staff       (20)      152 2023-01-28 06:30:20.000000 networklab-1.5.1.dev1/netsim/modules/sr.py
--rw-r--r--   0 pipi       (501) staff       (20)      390 2023-01-28 06:30:20.000000 networklab-1.5.1.dev1/netsim/modules/sr.yml
--rw-r--r--   0 pipi       (501) staff       (20)      910 2023-01-14 09:55:20.000000 networklab-1.5.1.dev1/netsim/modules/srv6.py
--rw-r--r--   0 pipi       (501) staff       (20)      420 2023-01-28 06:30:20.000000 networklab-1.5.1.dev1/netsim/modules/srv6.yml
--rw-r--r--   0 pipi       (501) staff       (20)    58915 2023-03-26 10:09:05.000000 networklab-1.5.1.dev1/netsim/modules/vlan.py
--rw-r--r--   0 pipi       (501) staff       (20)     1013 2023-03-26 10:09:05.000000 networklab-1.5.1.dev1/netsim/modules/vlan.yml
--rw-r--r--   0 pipi       (501) staff       (20)    20566 2023-03-26 10:09:05.000000 networklab-1.5.1.dev1/netsim/modules/vrf.py
--rw-r--r--   0 pipi       (501) staff       (20)      422 2023-03-26 10:09:05.000000 networklab-1.5.1.dev1/netsim/modules/vrf.yml
--rw-r--r--   0 pipi       (501) staff       (20)     9079 2022-12-11 09:34:30.000000 networklab-1.5.1.dev1/netsim/modules/vxlan.py
--rw-r--r--   0 pipi       (501) staff       (20)      555 2023-03-26 10:09:05.000000 networklab-1.5.1.dev1/netsim/modules/vxlan.yml
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-03-29 16:28:22.081468 networklab-1.5.1.dev1/netsim/outputs/
--rw-r--r--   0 pipi       (501) staff       (20)     2301 2023-03-29 09:00:02.000000 networklab-1.5.1.dev1/netsim/outputs/__init__.py
--rw-r--r--   0 pipi       (501) staff       (20)     7081 2023-03-29 09:00:02.000000 networklab-1.5.1.dev1/netsim/outputs/ansible.py
--rw-r--r--   0 pipi       (501) staff       (20)     1745 2022-01-21 21:02:25.000000 networklab-1.5.1.dev1/netsim/outputs/common.py
--rw-r--r--   0 pipi       (501) staff       (20)     9596 2023-03-26 10:09:05.000000 networklab-1.5.1.dev1/netsim/outputs/d2.py
--rw-r--r--   0 pipi       (501) staff       (20)      468 2023-03-26 10:09:05.000000 networklab-1.5.1.dev1/netsim/outputs/d2.yml
--rw-r--r--   0 pipi       (501) staff       (20)     2739 2023-03-29 09:00:02.000000 networklab-1.5.1.dev1/netsim/outputs/devices.py
--rw-r--r--   0 pipi       (501) staff       (20)     1268 2022-11-04 10:28:02.000000 networklab-1.5.1.dev1/netsim/outputs/format.py
--rw-r--r--   0 pipi       (501) staff       (20)     7581 2022-11-04 10:28:02.000000 networklab-1.5.1.dev1/netsim/outputs/graph.py
--rw-r--r--   0 pipi       (501) staff       (20)      218 2023-03-26 10:09:05.000000 networklab-1.5.1.dev1/netsim/outputs/graph.yml
--rw-r--r--   0 pipi       (501) staff       (20)     5504 2022-11-04 10:28:02.000000 networklab-1.5.1.dev1/netsim/outputs/graphite.py
--rw-r--r--   0 pipi       (501) staff       (20)      278 2021-08-22 05:50:16.000000 networklab-1.5.1.dev1/netsim/outputs/json.py
--rw-r--r--   0 pipi       (501) staff       (20)      228 2021-12-18 16:49:49.000000 networklab-1.5.1.dev1/netsim/outputs/none.py
--rw-r--r--   0 pipi       (501) staff       (20)     1838 2023-03-29 09:00:02.000000 networklab-1.5.1.dev1/netsim/outputs/provider.py
--rw-r--r--   0 pipi       (501) staff       (20)     1711 2023-03-29 09:00:02.000000 networklab-1.5.1.dev1/netsim/outputs/yaml.py
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-03-29 16:28:22.087988 networklab-1.5.1.dev1/netsim/providers/
--rw-r--r--   0 pipi       (501) staff       (20)     7882 2023-01-28 06:30:20.000000 networklab-1.5.1.dev1/netsim/providers/__init__.py
--rw-r--r--   0 pipi       (501) staff       (20)     3733 2023-01-28 06:30:20.000000 networklab-1.5.1.dev1/netsim/providers/clab.py
--rw-r--r--   0 pipi       (501) staff       (20)      517 2023-03-29 09:00:02.000000 networklab-1.5.1.dev1/netsim/providers/clab.yml
--rw-r--r--   0 pipi       (501) staff       (20)      836 2022-12-24 16:57:23.000000 networklab-1.5.1.dev1/netsim/providers/external.py
--rw-r--r--   0 pipi       (501) staff       (20)      157 2023-01-28 06:30:20.000000 networklab-1.5.1.dev1/netsim/providers/external.yml
--rw-r--r--   0 pipi       (501) staff       (20)    11317 2023-03-27 16:36:19.000000 networklab-1.5.1.dev1/netsim/providers/libvirt.py
--rw-r--r--   0 pipi       (501) staff       (20)      481 2023-03-29 09:00:02.000000 networklab-1.5.1.dev1/netsim/providers/libvirt.yml
--rw-r--r--   0 pipi       (501) staff       (20)      210 2022-12-24 16:57:30.000000 networklab-1.5.1.dev1/netsim/providers/virtualbox.py
--rw-r--r--   0 pipi       (501) staff       (20)      320 2023-01-28 06:30:20.000000 networklab-1.5.1.dev1/netsim/providers/virtualbox.yml
--rw-r--r--   0 pipi       (501) staff       (20)     7937 2023-03-12 06:53:58.000000 networklab-1.5.1.dev1/netsim/read_topology.py
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-03-29 16:28:22.088169 networklab-1.5.1.dev1/netsim/templates/
--rw-r--r--   0 pipi       (501) staff       (20)      469 2022-05-26 14:27:51.000000 networklab-1.5.1.dev1/netsim/templates/ansible.cfg.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-03-29 16:28:21.939895 networklab-1.5.1.dev1/netsim/templates/provider/
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-03-29 16:28:22.088471 networklab-1.5.1.dev1/netsim/templates/provider/clab/
--rw-r--r--   0 pipi       (501) staff       (20)     3077 2023-01-28 06:30:20.000000 networklab-1.5.1.dev1/netsim/templates/provider/clab/clab.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-03-29 16:28:22.088649 networklab-1.5.1.dev1/netsim/templates/provider/clab/frr/
--rw-r--r--   0 pipi       (501) staff       (20)     2935 2023-01-12 13:38:07.000000 networklab-1.5.1.dev1/netsim/templates/provider/clab/frr/daemons.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-03-29 16:28:22.088925 networklab-1.5.1.dev1/netsim/templates/provider/clab/linux/
--rw-r--r--   0 pipi       (501) staff       (20)      604 2023-01-12 13:45:42.000000 networklab-1.5.1.dev1/netsim/templates/provider/clab/linux/hosts.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-03-29 16:28:22.089176 networklab-1.5.1.dev1/netsim/templates/provider/external/
--rw-r--r--   0 pipi       (501) staff       (20)     1318 2022-12-18 14:12:35.000000 networklab-1.5.1.dev1/netsim/templates/provider/external/external.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-03-29 16:28:22.099430 networklab-1.5.1.dev1/netsim/templates/provider/libvirt/
--rw-r--r--   0 pipi       (501) staff       (20)      541 2023-01-28 06:30:20.000000 networklab-1.5.1.dev1/netsim/templates/provider/libvirt/Vagrantfile.j2
--rw-r--r--   0 pipi       (501) staff       (20)      332 2022-01-25 17:29:43.000000 networklab-1.5.1.dev1/netsim/templates/provider/libvirt/arcos-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      427 2022-11-10 07:29:53.000000 networklab-1.5.1.dev1/netsim/templates/provider/libvirt/asav-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      445 2022-12-11 17:33:57.000000 networklab-1.5.1.dev1/netsim/templates/provider/libvirt/csr-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      190 2022-01-25 17:59:15.000000 networklab-1.5.1.dev1/netsim/templates/provider/libvirt/cumulus-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1177 2023-01-28 06:30:20.000000 networklab-1.5.1.dev1/netsim/templates/provider/libvirt/cumulus_nvue-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1297 2023-03-06 07:47:06.000000 networklab-1.5.1.dev1/netsim/templates/provider/libvirt/define-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      438 2022-04-17 16:31:22.000000 networklab-1.5.1.dev1/netsim/templates/provider/libvirt/dellos10-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      355 2022-01-25 17:30:38.000000 networklab-1.5.1.dev1/netsim/templates/provider/libvirt/eos-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      258 2022-01-25 17:30:42.000000 networklab-1.5.1.dev1/netsim/templates/provider/libvirt/fortios-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      380 2022-12-11 10:03:46.000000 networklab-1.5.1.dev1/netsim/templates/provider/libvirt/iosv-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1835 2023-01-12 13:38:07.000000 networklab-1.5.1.dev1/netsim/templates/provider/libvirt/iosxr-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      486 2023-01-28 06:30:20.000000 networklab-1.5.1.dev1/netsim/templates/provider/libvirt/libvirt-bridge.j2
--rw-r--r--   0 pipi       (501) staff       (20)      668 2023-01-28 06:30:20.000000 networklab-1.5.1.dev1/netsim/templates/provider/libvirt/libvirt-tunnel.j2
--rw-r--r--   0 pipi       (501) staff       (20)      190 2022-01-25 17:30:59.000000 networklab-1.5.1.dev1/netsim/templates/provider/libvirt/linux-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)       52 2021-12-28 08:07:36.000000 networklab-1.5.1.dev1/netsim/templates/provider/libvirt/none-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      814 2022-12-12 17:43:45.000000 networklab-1.5.1.dev1/netsim/templates/provider/libvirt/nxos-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      309 2022-01-25 17:31:10.000000 networklab-1.5.1.dev1/netsim/templates/provider/libvirt/routeros-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      347 2022-10-19 17:10:38.000000 networklab-1.5.1.dev1/netsim/templates/provider/libvirt/routeros7-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)     1283 2023-01-28 07:18:50.000000 networklab-1.5.1.dev1/netsim/templates/provider/libvirt/vagrant-libvirt.xml
--rw-r--r--   0 pipi       (501) staff       (20)      740 2023-01-28 06:30:20.000000 networklab-1.5.1.dev1/netsim/templates/provider/libvirt/vsrx-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      223 2022-01-25 17:31:29.000000 networklab-1.5.1.dev1/netsim/templates/provider/libvirt/vyos-domain.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-03-29 16:28:22.101643 networklab-1.5.1.dev1/netsim/templates/provider/virtualbox/
--rw-r--r--   0 pipi       (501) staff       (20)      782 2022-05-02 06:40:29.000000 networklab-1.5.1.dev1/netsim/templates/provider/virtualbox/Vagrantfile.j2
--rw-r--r--   0 pipi       (501) staff       (20)      274 2022-01-25 17:34:51.000000 networklab-1.5.1.dev1/netsim/templates/provider/virtualbox/arcos-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      192 2022-09-05 16:28:24.000000 networklab-1.5.1.dev1/netsim/templates/provider/virtualbox/cumulus-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      108 2022-01-25 17:35:32.000000 networklab-1.5.1.dev1/netsim/templates/provider/virtualbox/eos-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      191 2022-01-25 17:35:37.000000 networklab-1.5.1.dev1/netsim/templates/provider/virtualbox/linux-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      321 2022-01-25 17:36:47.000000 networklab-1.5.1.dev1/netsim/templates/provider/virtualbox/nxos-domain.j2
--rw-r--r--   0 pipi       (501) staff       (20)      217 2021-04-11 18:37:32.000000 networklab-1.5.1.dev1/netsim/templates/provider/virtualbox/virtualbox-network.j2
--rw-r--r--   0 pipi       (501) staff       (20)      323 2021-04-11 18:37:32.000000 networklab-1.5.1.dev1/netsim/templates/provider/virtualbox/virtualbox-ports.j2
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-03-29 16:28:22.102428 networklab-1.5.1.dev1/netsim/templates/tests/
--rw-r--r--   0 pipi       (501) staff       (20)      255 2022-12-11 17:33:46.000000 networklab-1.5.1.dev1/netsim/templates/tests/clab.yml
--rw-r--r--   0 pipi       (501) staff       (20)      181 2022-12-11 09:54:53.000000 networklab-1.5.1.dev1/netsim/templates/tests/libvirt.yml
--rw-r--r--   0 pipi       (501) staff       (20)      185 2022-12-11 09:54:58.000000 networklab-1.5.1.dev1/netsim/templates/tests/virtualbox.yml
--rw-r--r--   0 pipi       (501) staff       (20)      496 2023-03-26 10:09:05.000000 networklab-1.5.1.dev1/netsim/topology-defaults.yml
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-03-29 16:28:22.103383 networklab-1.5.1.dev1/netsim/utils/
--rw-r--r--   0 pipi       (501) staff       (20)       78 2023-01-28 06:30:20.000000 networklab-1.5.1.dev1/netsim/utils/__init__.py
--rw-r--r--   0 pipi       (501) staff       (20)     4068 2023-01-28 06:30:20.000000 networklab-1.5.1.dev1/netsim/utils/log.py
--rw-r--r--   0 pipi       (501) staff       (20)     3248 2023-03-29 09:00:02.000000 networklab-1.5.1.dev1/netsim/utils/status.py
--rw-r--r--   0 pipi       (501) staff       (20)     1277 2023-03-29 09:00:24.000000 networklab-1.5.1.dev1/netsim/utils/strings.py
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-03-29 16:28:22.104298 networklab-1.5.1.dev1/networklab.egg-info/
--rw-r--r--   0 pipi       (501) staff       (20)     4081 2023-03-29 16:28:21.000000 networklab-1.5.1.dev1/networklab.egg-info/PKG-INFO
--rw-r--r--   0 pipi       (501) staff       (20)    19297 2023-03-29 16:28:21.000000 networklab-1.5.1.dev1/networklab.egg-info/SOURCES.txt
--rw-r--r--   0 pipi       (501) staff       (20)        1 2023-03-29 16:28:21.000000 networklab-1.5.1.dev1/networklab.egg-info/dependency_links.txt
--rw-r--r--   0 pipi       (501) staff       (20)       51 2023-03-29 16:28:21.000000 networklab-1.5.1.dev1/networklab.egg-info/entry_points.txt
--rw-r--r--   0 pipi       (501) staff       (20)      122 2023-03-29 16:28:21.000000 networklab-1.5.1.dev1/networklab.egg-info/requires.txt
--rw-r--r--   0 pipi       (501) staff       (20)        7 2023-03-29 16:28:21.000000 networklab-1.5.1.dev1/networklab.egg-info/top_level.txt
--rw-r--r--   0 pipi       (501) staff       (20)      183 2023-03-29 09:00:02.000000 networklab-1.5.1.dev1/requirements.txt
--rw-r--r--   0 pipi       (501) staff       (20)       38 2023-03-29 16:28:22.105401 networklab-1.5.1.dev1/setup.cfg
--rw-r--r--   0 pipi       (501) staff       (20)     1477 2022-11-25 15:02:55.000000 networklab-1.5.1.dev1/setup.py
-drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-03-29 16:28:22.104446 networklab-1.5.1.dev1/tests/
--rwxr-xr-x   0 pipi       (501) staff       (20)     3462 2023-01-28 06:30:20.000000 networklab-1.5.1.dev1/tests/test_transformation.py
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.355123 networklab-1.5.2.dev1/
+-rw-r--r--   0 pipi       (501) staff       (20)     1153 2022-05-02 06:40:29.000000 networklab-1.5.2.dev1/LICENSE.md
+-rw-r--r--   0 pipi       (501) staff       (20)      254 2021-12-28 08:07:36.000000 networklab-1.5.2.dev1/MANIFEST.in
+-rw-r--r--   0 pipi       (501) staff       (20)     4081 2023-04-15 09:01:42.354911 networklab-1.5.2.dev1/PKG-INFO
+-rw-r--r--   0 pipi       (501) staff       (20)     3367 2023-04-02 11:32:00.000000 networklab-1.5.2.dev1/README.md
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.190458 networklab-1.5.2.dev1/netsim/
+-rwxr-xr-x   0 pipi       (501) staff       (20)       51 2023-04-15 09:01:29.000000 networklab-1.5.2.dev1/netsim/__init__.py
+-rw-r--r--   0 pipi       (501) staff       (20)    13342 2022-11-23 16:13:46.000000 networklab-1.5.2.dev1/netsim/addressing.py
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.191990 networklab-1.5.2.dev1/netsim/ansible/
+-rwxr-xr-x   0 pipi       (501) staff       (20)      900 2022-12-18 17:58:58.000000 networklab-1.5.2.dev1/netsim/ansible/collect-configs.ansible
+-rwxr-xr-x   0 pipi       (501) staff       (20)     2714 2023-04-08 06:22:10.000000 networklab-1.5.2.dev1/netsim/ansible/config.ansible
+-rwxr-xr-x   0 pipi       (501) staff       (20)     1269 2023-01-12 13:38:07.000000 networklab-1.5.2.dev1/netsim/ansible/create-config.ansible
+-rwxr--r--   0 pipi       (501) staff       (20)      295 2022-10-25 08:11:07.000000 networklab-1.5.2.dev1/netsim/ansible/display-neighbors.ansible
+-rwxr-xr-x   0 pipi       (501) staff       (20)     3424 2023-01-25 10:08:09.000000 networklab-1.5.2.dev1/netsim/ansible/initial-config.ansible
+-rw-r--r--   0 pipi       (501) staff       (20)      401 2022-12-22 15:59:29.000000 networklab-1.5.2.dev1/netsim/ansible/missing.yml
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.192720 networklab-1.5.2.dev1/netsim/ansible/tasks/
+-rw-r--r--   0 pipi       (501) staff       (20)      684 2023-01-12 13:38:07.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/create-config.yml
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.197240 networklab-1.5.2.dev1/netsim/ansible/tasks/deploy-config/
+-rw-r--r--   0 pipi       (501) staff       (20)      333 2022-05-02 05:23:35.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/deploy-config/arcos.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      592 2023-04-11 06:23:16.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/deploy-config/arubacx.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      157 2022-11-10 07:29:53.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/deploy-config/asa.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      717 2022-05-02 05:23:46.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/deploy-config/cumulus.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      841 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/deploy-config/cumulus_nvue.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      376 2022-04-17 16:31:22.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/deploy-config/dellos10.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      159 2023-01-12 13:38:07.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/deploy-config/eos.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      525 2022-05-02 05:23:58.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/deploy-config/frr.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      159 2022-12-19 08:16:52.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/deploy-config/ios.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      163 2023-01-12 13:38:07.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/deploy-config/iosxr.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      204 2022-12-18 17:58:58.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/deploy-config/junos.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      593 2023-04-07 18:34:46.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/deploy-config/linux-clab.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      278 2022-12-22 08:33:55.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/deploy-config/linux.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      140 2022-03-20 08:56:05.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/deploy-config/none.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      161 2022-05-02 06:40:29.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/deploy-config/nxos.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      777 2022-05-02 05:37:23.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/deploy-config/routeros.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      240 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/deploy-config/routeros7.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     3328 2023-03-06 07:47:06.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/deploy-config/srlinux.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     4846 2023-04-11 06:23:20.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/deploy-config/sros.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      551 2022-12-18 17:58:58.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/deploy-config/vyos.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     3084 2023-04-11 06:23:20.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/deploy-custom-config.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     2142 2023-01-25 10:08:09.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/deploy-module.yml
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.204485 networklab-1.5.2.dev1/netsim/ansible/tasks/fetch-config/
+-rw-r--r--   0 pipi       (501) staff       (20)      160 2021-07-09 15:23:10.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/fetch-config/arcos.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      110 2022-11-10 07:29:53.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/fetch-config/asa.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      254 2022-03-07 15:39:35.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/fetch-config/cumulus.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      308 2022-03-07 15:39:45.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/fetch-config/cumulus_nvue.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      115 2022-04-17 16:31:22.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/fetch-config/dellos10.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      112 2022-03-07 15:40:03.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/fetch-config/eos.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      346 2021-12-11 08:49:40.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/fetch-config/fortinet.fortios.fortios.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      110 2022-12-19 08:45:45.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/fetch-config/ios.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      107 2023-01-12 13:38:07.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/fetch-config/iosxr.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      124 2021-07-09 15:23:10.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/fetch-config/junos.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      113 2021-07-09 15:23:10.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/fetch-config/nxos.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      195 2021-11-27 09:09:57.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/fetch-config/routeros.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      195 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/fetch-config/routeros7.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      721 2022-03-07 17:07:35.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/fetch-config/srlinux.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      469 2022-03-07 17:07:35.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/fetch-config/sros.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      190 2021-11-27 09:09:57.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/fetch-config/vyos.yml
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.204971 networklab-1.5.2.dev1/netsim/ansible/tasks/fortinet.fortios.fortios/
+-rw-r--r--   0 pipi       (501) staff       (20)     2645 2022-01-20 07:34:11.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/fortinet.fortios.fortios/initial.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     2494 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/fortinet.fortios.fortios/ospf.yml
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.205182 networklab-1.5.2.dev1/netsim/ansible/tasks/iosxr/
+-rw-r--r--   0 pipi       (501) staff       (20)      900 2023-01-12 13:38:07.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/iosxr/initial.yml
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.205457 networklab-1.5.2.dev1/netsim/ansible/tasks/linux/
+-rw-r--r--   0 pipi       (501) staff       (20)     1504 2023-01-12 13:38:07.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/linux/initial-clab.yml
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.205691 networklab-1.5.2.dev1/netsim/ansible/tasks/nxos/
+-rw-r--r--   0 pipi       (501) staff       (20)      291 2022-12-05 12:30:42.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/nxos/initial.yml
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.206299 networklab-1.5.2.dev1/netsim/ansible/tasks/readiness-check/
+-rw-r--r--   0 pipi       (501) staff       (20)      491 2023-01-12 13:38:07.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/readiness-check/dellos10.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      125 2023-01-12 13:38:07.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/readiness-check/eos-clab.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      378 2023-01-12 13:38:07.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/readiness-check/routeros7.yml
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.206473 networklab-1.5.2.dev1/netsim/ansible/tasks/vmx/
+-rw-r--r--   0 pipi       (501) staff       (20)     1707 2022-12-22 09:02:46.000000 networklab-1.5.2.dev1/netsim/ansible/tasks/vmx/initial.yml
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.206699 networklab-1.5.2.dev1/netsim/ansible/templates/
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.208437 networklab-1.5.2.dev1/netsim/ansible/templates/bfd/
+-rw-r--r--   0 pipi       (501) staff       (20)      618 2023-04-11 06:23:16.000000 networklab-1.5.2.dev1/netsim/ansible/templates/bfd/arubacx.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      700 2022-12-11 11:47:34.000000 networklab-1.5.2.dev1/netsim/ansible/templates/bfd/eos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      599 2022-01-09 08:37:35.000000 networklab-1.5.2.dev1/netsim/ansible/templates/bfd/ios.j2
+-rw-r--r--   0 pipi       (501) staff       (20)        0 2022-01-09 08:37:35.000000 networklab-1.5.2.dev1/netsim/ansible/templates/bfd/none.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      834 2022-01-09 08:37:35.000000 networklab-1.5.2.dev1/netsim/ansible/templates/bfd/nxos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      611 2022-01-09 08:37:35.000000 networklab-1.5.2.dev1/netsim/ansible/templates/bfd/srlinux.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1268 2022-11-04 10:28:02.000000 networklab-1.5.2.dev1/netsim/ansible/templates/bfd/sros.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      486 2022-08-27 11:27:47.000000 networklab-1.5.2.dev1/netsim/ansible/templates/bfd/vyos.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.215119 networklab-1.5.2.dev1/netsim/ansible/templates/bgp/
+-rw-r--r--   0 pipi       (501) staff       (20)     1363 2023-04-11 06:23:16.000000 networklab-1.5.2.dev1/netsim/ansible/templates/bgp/arubacx.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1381 2023-04-11 06:23:16.000000 networklab-1.5.2.dev1/netsim/ansible/templates/bgp/arubacx.macro.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      888 2022-11-10 07:29:53.000000 networklab-1.5.2.dev1/netsim/ansible/templates/bgp/asa.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      778 2022-11-10 07:29:53.000000 networklab-1.5.2.dev1/netsim/ansible/templates/bgp/asa.macro.j2
+-rw-r--r--   0 pipi       (501) staff       (20)       74 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/bgp/cumulus.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     3040 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/bgp/cumulus_nvue.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1257 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/bgp/dellos10.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     2010 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/bgp/dellos10.macro.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1755 2022-12-11 16:40:37.000000 networklab-1.5.2.dev1/netsim/ansible/templates/bgp/eos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      911 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/bgp/eos.macro.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     2621 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/bgp/frr.bgp-config.j2
+-rw-r--r--   0 pipi       (501) staff       (20)       66 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/bgp/frr.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1369 2023-02-07 15:05:29.000000 networklab-1.5.2.dev1/netsim/ansible/templates/bgp/ios.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1539 2022-12-21 09:06:32.000000 networklab-1.5.2.dev1/netsim/ansible/templates/bgp/ios.macro.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1830 2023-01-12 13:38:07.000000 networklab-1.5.2.dev1/netsim/ansible/templates/bgp/iosxr.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     2308 2022-05-02 06:40:29.000000 networklab-1.5.2.dev1/netsim/ansible/templates/bgp/junos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)        0 2021-12-28 08:07:36.000000 networklab-1.5.2.dev1/netsim/ansible/templates/bgp/none.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1696 2022-09-01 07:44:05.000000 networklab-1.5.2.dev1/netsim/ansible/templates/bgp/nxos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1045 2022-05-02 06:40:29.000000 networklab-1.5.2.dev1/netsim/ansible/templates/bgp/routeros.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1109 2022-04-16 08:35:35.000000 networklab-1.5.2.dev1/netsim/ansible/templates/bgp/routeros.macro.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1075 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/bgp/routeros7.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1401 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/bgp/routeros7.macro.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     2924 2022-05-02 06:40:29.000000 networklab-1.5.2.dev1/netsim/ansible/templates/bgp/srlinux.cli.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      316 2022-12-18 17:58:58.000000 networklab-1.5.2.dev1/netsim/ansible/templates/bgp/srlinux.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     7934 2022-12-18 17:58:58.000000 networklab-1.5.2.dev1/netsim/ansible/templates/bgp/srlinux.macro.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     3252 2022-11-04 10:28:02.000000 networklab-1.5.2.dev1/netsim/ansible/templates/bgp/sros.gnmi.macro.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      534 2022-10-25 08:00:46.000000 networklab-1.5.2.dev1/netsim/ansible/templates/bgp/sros.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     2873 2022-05-02 06:40:29.000000 networklab-1.5.2.dev1/netsim/ansible/templates/bgp/sros.md-cli.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     2086 2022-01-30 15:43:37.000000 networklab-1.5.2.dev1/netsim/ansible/templates/bgp/sros.openconfig.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1492 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/bgp/vyos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1323 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/bgp/vyos.macro.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.215519 networklab-1.5.2.dev1/netsim/ansible/templates/eigrp/
+-rw-r--r--   0 pipi       (501) staff       (20)     1234 2023-02-07 15:05:29.000000 networklab-1.5.2.dev1/netsim/ansible/templates/eigrp/ios.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      862 2022-02-14 14:03:36.000000 networklab-1.5.2.dev1/netsim/ansible/templates/eigrp/nxos.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.217728 networklab-1.5.2.dev1/netsim/ansible/templates/evpn/
+-rw-r--r--   0 pipi       (501) staff       (20)      903 2023-04-11 06:23:16.000000 networklab-1.5.2.dev1/netsim/ansible/templates/evpn/arubacx.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1143 2022-11-04 10:28:02.000000 networklab-1.5.2.dev1/netsim/ansible/templates/evpn/cumulus.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1621 2022-11-04 10:28:02.000000 networklab-1.5.2.dev1/netsim/ansible/templates/evpn/dellos10.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1423 2022-12-15 16:40:50.000000 networklab-1.5.2.dev1/netsim/ansible/templates/evpn/eos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1580 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/evpn/frr.evpn-config.j2
+-rw-r--r--   0 pipi       (501) staff       (20)       35 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/evpn/frr.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1677 2023-01-30 13:30:53.000000 networklab-1.5.2.dev1/netsim/ansible/templates/evpn/nxos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1708 2022-12-18 17:58:58.000000 networklab-1.5.2.dev1/netsim/ansible/templates/evpn/srlinux.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      405 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/evpn/sros.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     2883 2022-09-25 16:03:22.000000 networklab-1.5.2.dev1/netsim/ansible/templates/evpn/vyos.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.219761 networklab-1.5.2.dev1/netsim/ansible/templates/gateway/
+-rw-r--r--   0 pipi       (501) staff       (20)     1346 2023-04-11 06:23:16.000000 networklab-1.5.2.dev1/netsim/ansible/templates/gateway/arubacx.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1244 2022-11-04 10:28:02.000000 networklab-1.5.2.dev1/netsim/ansible/templates/gateway/cumulus.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1162 2022-11-17 08:20:15.000000 networklab-1.5.2.dev1/netsim/ansible/templates/gateway/dellos10.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      951 2022-11-04 10:28:02.000000 networklab-1.5.2.dev1/netsim/ansible/templates/gateway/eos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      739 2022-12-14 07:49:49.000000 networklab-1.5.2.dev1/netsim/ansible/templates/gateway/ios.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      727 2022-11-04 10:28:02.000000 networklab-1.5.2.dev1/netsim/ansible/templates/gateway/nxos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      613 2022-11-04 10:28:02.000000 networklab-1.5.2.dev1/netsim/ansible/templates/gateway/srlinux.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      953 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/ansible/templates/gateway/sros.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1006 2022-11-17 08:20:15.000000 networklab-1.5.2.dev1/netsim/ansible/templates/gateway/vyos.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.228224 networklab-1.5.2.dev1/netsim/ansible/templates/initial/
+-rw-r--r--   0 pipi       (501) staff       (20)      836 2022-01-05 16:01:35.000000 networklab-1.5.2.dev1/netsim/ansible/templates/initial/arcos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1200 2023-04-11 06:23:16.000000 networklab-1.5.2.dev1/netsim/ansible/templates/initial/arubacx.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      480 2023-04-11 06:23:16.000000 networklab-1.5.2.dev1/netsim/ansible/templates/initial/arubacx.vlan.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      466 2023-04-11 06:23:16.000000 networklab-1.5.2.dev1/netsim/ansible/templates/initial/arubacx.vrf.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1122 2022-11-10 07:29:53.000000 networklab-1.5.2.dev1/netsim/ansible/templates/initial/asa.j2
+-rw-r--r--   0 pipi       (501) staff       (20)       44 2022-12-18 17:58:58.000000 networklab-1.5.2.dev1/netsim/ansible/templates/initial/csr.vlan.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     5271 2023-04-02 11:32:00.000000 networklab-1.5.2.dev1/netsim/ansible/templates/initial/cumulus.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1342 2022-10-22 08:18:07.000000 networklab-1.5.2.dev1/netsim/ansible/templates/initial/cumulus_nvue.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1643 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/initial/dellos10.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      537 2022-08-27 11:27:47.000000 networklab-1.5.2.dev1/netsim/ansible/templates/initial/dellos10.vrf.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     2201 2022-11-04 10:28:02.000000 networklab-1.5.2.dev1/netsim/ansible/templates/initial/eos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      261 2022-08-27 11:27:47.000000 networklab-1.5.2.dev1/netsim/ansible/templates/initial/eos.vrf.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     3075 2023-01-12 13:38:07.000000 networklab-1.5.2.dev1/netsim/ansible/templates/initial/frr.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     2371 2022-12-18 17:58:58.000000 networklab-1.5.2.dev1/netsim/ansible/templates/initial/ios.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      157 2022-12-14 07:50:27.000000 networklab-1.5.2.dev1/netsim/ansible/templates/initial/ios.vlan.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      378 2022-09-11 07:46:54.000000 networklab-1.5.2.dev1/netsim/ansible/templates/initial/ios.vrf.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1717 2023-01-12 13:38:07.000000 networklab-1.5.2.dev1/netsim/ansible/templates/initial/iosxr.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     2118 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/ansible/templates/initial/junos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1524 2022-12-19 09:40:05.000000 networklab-1.5.2.dev1/netsim/ansible/templates/initial/junos.vlan.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1607 2022-12-19 09:40:05.000000 networklab-1.5.2.dev1/netsim/ansible/templates/initial/junos.vrf.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.229012 networklab-1.5.2.dev1/netsim/ansible/templates/initial/linux/
+-rw-r--r--   0 pipi       (501) staff       (20)      906 2022-12-22 08:29:57.000000 networklab-1.5.2.dev1/netsim/ansible/templates/initial/linux/hosts.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     2918 2022-12-22 09:39:24.000000 networklab-1.5.2.dev1/netsim/ansible/templates/initial/linux/ubuntu.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1933 2023-01-12 13:38:07.000000 networklab-1.5.2.dev1/netsim/ansible/templates/initial/linux/vanilla.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      283 2023-01-12 13:38:07.000000 networklab-1.5.2.dev1/netsim/ansible/templates/initial/linux-clab.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      434 2023-01-12 13:38:07.000000 networklab-1.5.2.dev1/netsim/ansible/templates/initial/linux.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1937 2023-01-30 13:30:53.000000 networklab-1.5.2.dev1/netsim/ansible/templates/initial/nxos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      393 2022-08-27 11:27:47.000000 networklab-1.5.2.dev1/netsim/ansible/templates/initial/nxos.vrf.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1413 2022-06-20 08:57:47.000000 networklab-1.5.2.dev1/netsim/ansible/templates/initial/routeros.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      546 2022-06-20 08:57:47.000000 networklab-1.5.2.dev1/netsim/ansible/templates/initial/routeros.vlan.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      498 2022-08-18 15:16:48.000000 networklab-1.5.2.dev1/netsim/ansible/templates/initial/routeros.vrf.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1571 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/initial/routeros7.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      611 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/initial/routeros7.vlan.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      352 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/initial/routeros7.vrf.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      968 2022-01-05 16:01:35.000000 networklab-1.5.2.dev1/netsim/ansible/templates/initial/srlinux.cli.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     3431 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/initial/srlinux.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     4711 2023-04-02 11:32:00.000000 networklab-1.5.2.dev1/netsim/ansible/templates/initial/sros.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1434 2022-01-05 16:01:35.000000 networklab-1.5.2.dev1/netsim/ansible/templates/initial/sros.md-cli.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     2622 2022-01-06 16:04:54.000000 networklab-1.5.2.dev1/netsim/ansible/templates/initial/sros.openconfig.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     2782 2022-11-10 07:29:53.000000 networklab-1.5.2.dev1/netsim/ansible/templates/initial/vyos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      250 2022-06-20 08:57:47.000000 networklab-1.5.2.dev1/netsim/ansible/templates/initial/vyos.vlan.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      101 2022-08-18 15:17:06.000000 networklab-1.5.2.dev1/netsim/ansible/templates/initial/vyos.vrf.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.231501 networklab-1.5.2.dev1/netsim/ansible/templates/isis/
+-rw-r--r--   0 pipi       (501) staff       (20)      887 2022-11-10 07:29:53.000000 networklab-1.5.2.dev1/netsim/ansible/templates/isis/asa.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1241 2022-02-14 14:03:36.000000 networklab-1.5.2.dev1/netsim/ansible/templates/isis/eos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1149 2022-02-14 14:03:36.000000 networklab-1.5.2.dev1/netsim/ansible/templates/isis/frr.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1505 2022-12-20 08:16:04.000000 networklab-1.5.2.dev1/netsim/ansible/templates/isis/ios.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1168 2023-01-12 13:38:07.000000 networklab-1.5.2.dev1/netsim/ansible/templates/isis/iosxr.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     2225 2022-12-19 09:40:05.000000 networklab-1.5.2.dev1/netsim/ansible/templates/isis/junos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1701 2022-02-14 14:03:36.000000 networklab-1.5.2.dev1/netsim/ansible/templates/isis/nxos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     2086 2022-11-23 16:08:58.000000 networklab-1.5.2.dev1/netsim/ansible/templates/isis/srlinux.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1426 2022-11-04 10:28:02.000000 networklab-1.5.2.dev1/netsim/ansible/templates/isis/sros.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1550 2022-01-06 06:47:23.000000 networklab-1.5.2.dev1/netsim/ansible/templates/isis/sros.openconfig.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1262 2022-08-27 11:27:47.000000 networklab-1.5.2.dev1/netsim/ansible/templates/isis/vyos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      136 2021-12-06 08:23:27.000000 networklab-1.5.2.dev1/netsim/ansible/templates/missing.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.242141 networklab-1.5.2.dev1/netsim/ansible/templates/mpls/
+-rw-r--r--   0 pipi       (501) staff       (20)      149 2023-04-11 06:23:16.000000 networklab-1.5.2.dev1/netsim/ansible/templates/mpls/arubacx.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      203 2023-04-11 06:23:16.000000 networklab-1.5.2.dev1/netsim/ansible/templates/mpls/arubacx.ldp.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      333 2023-04-11 06:23:16.000000 networklab-1.5.2.dev1/netsim/ansible/templates/mpls/arubacx.mplsvpn.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      670 2022-08-27 11:27:47.000000 networklab-1.5.2.dev1/netsim/ansible/templates/mpls/eos.6pe.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1089 2022-04-01 07:43:22.000000 networklab-1.5.2.dev1/netsim/ansible/templates/mpls/eos.bgp-lu.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      289 2022-08-27 11:27:47.000000 networklab-1.5.2.dev1/netsim/ansible/templates/mpls/eos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      410 2022-04-01 07:43:22.000000 networklab-1.5.2.dev1/netsim/ansible/templates/mpls/eos.ldp.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      413 2022-04-01 07:43:22.000000 networklab-1.5.2.dev1/netsim/ansible/templates/mpls/eos.mplsvpn.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      195 2023-01-12 13:38:07.000000 networklab-1.5.2.dev1/netsim/ansible/templates/mpls/frr.frr-config.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      272 2023-01-12 13:38:07.000000 networklab-1.5.2.dev1/netsim/ansible/templates/mpls/frr.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      472 2023-01-12 13:38:07.000000 networklab-1.5.2.dev1/netsim/ansible/templates/mpls/frr.ldp.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      327 2023-01-12 13:38:07.000000 networklab-1.5.2.dev1/netsim/ansible/templates/mpls/frr.mplsvpn.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      208 2022-08-27 11:27:47.000000 networklab-1.5.2.dev1/netsim/ansible/templates/mpls/ios.6pe.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      611 2022-08-11 09:57:08.000000 networklab-1.5.2.dev1/netsim/ansible/templates/mpls/ios.bgp-lu.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      302 2022-08-27 11:27:47.000000 networklab-1.5.2.dev1/netsim/ansible/templates/mpls/ios.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      257 2022-04-01 07:43:22.000000 networklab-1.5.2.dev1/netsim/ansible/templates/mpls/ios.ldp.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      326 2022-04-01 07:43:22.000000 networklab-1.5.2.dev1/netsim/ansible/templates/mpls/ios.mplsvpn.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      328 2022-12-19 09:40:05.000000 networklab-1.5.2.dev1/netsim/ansible/templates/mpls/junos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      542 2022-12-19 09:40:05.000000 networklab-1.5.2.dev1/netsim/ansible/templates/mpls/junos.ldp.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      656 2022-12-19 09:40:05.000000 networklab-1.5.2.dev1/netsim/ansible/templates/mpls/junos.mplsvpn.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      151 2022-04-06 16:02:55.000000 networklab-1.5.2.dev1/netsim/ansible/templates/mpls/routeros.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      383 2022-04-06 16:02:55.000000 networklab-1.5.2.dev1/netsim/ansible/templates/mpls/routeros.ldp.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      412 2022-04-06 16:02:55.000000 networklab-1.5.2.dev1/netsim/ansible/templates/mpls/routeros.mplsvpn.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      198 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/mpls/routeros7.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      382 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/mpls/routeros7.ldp.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      408 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/mpls/routeros7.mplsvpn.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      272 2022-11-04 10:28:02.000000 networklab-1.5.2.dev1/netsim/ansible/templates/mpls/sros.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      732 2022-11-04 10:28:02.000000 networklab-1.5.2.dev1/netsim/ansible/templates/mpls/sros.ldp.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      432 2022-04-17 16:31:22.000000 networklab-1.5.2.dev1/netsim/ansible/templates/mpls/vyos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      462 2023-01-12 13:38:07.000000 networklab-1.5.2.dev1/netsim/ansible/templates/mpls/vyos.ldp.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      668 2022-04-17 16:31:22.000000 networklab-1.5.2.dev1/netsim/ansible/templates/mpls/vyos.mplsvpn.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.251456 networklab-1.5.2.dev1/netsim/ansible/templates/ospf/
+-rw-r--r--   0 pipi       (501) staff       (20)      488 2022-01-06 08:25:20.000000 networklab-1.5.2.dev1/netsim/ansible/templates/ospf/arcos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      198 2023-04-11 06:23:16.000000 networklab-1.5.2.dev1/netsim/ansible/templates/ospf/arubacx.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1040 2023-04-11 06:23:16.000000 networklab-1.5.2.dev1/netsim/ansible/templates/ospf/arubacx.ospfv2.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1061 2023-04-11 06:23:16.000000 networklab-1.5.2.dev1/netsim/ansible/templates/ospf/arubacx.ospfv3.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      199 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/ospf/cumulus.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      778 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/ospf/cumulus.ospfv2.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      791 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/ospf/cumulus.ospfv3.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1228 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/ospf/cumulus_nvue.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      200 2022-04-17 16:31:22.000000 networklab-1.5.2.dev1/netsim/ansible/templates/ospf/dellos10.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      838 2022-04-17 16:31:22.000000 networklab-1.5.2.dev1/netsim/ansible/templates/ospf/dellos10.ospfv2.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      834 2022-04-17 16:31:22.000000 networklab-1.5.2.dev1/netsim/ansible/templates/ospf/dellos10.ospfv3.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      190 2022-03-06 19:16:46.000000 networklab-1.5.2.dev1/netsim/ansible/templates/ospf/eos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1032 2022-02-14 14:03:36.000000 networklab-1.5.2.dev1/netsim/ansible/templates/ospf/eos.ospfv2.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      967 2022-09-04 08:58:45.000000 networklab-1.5.2.dev1/netsim/ansible/templates/ospf/eos.ospfv3.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      222 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/ospf/frr.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      737 2023-01-12 13:38:07.000000 networklab-1.5.2.dev1/netsim/ansible/templates/ospf/frr.ospfv2.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      713 2022-12-20 07:49:03.000000 networklab-1.5.2.dev1/netsim/ansible/templates/ospf/frr.ospfv3.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      190 2022-03-06 19:16:05.000000 networklab-1.5.2.dev1/netsim/ansible/templates/ospf/ios.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      897 2022-02-14 14:03:36.000000 networklab-1.5.2.dev1/netsim/ansible/templates/ospf/ios.ospfv2.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      871 2022-02-14 14:03:36.000000 networklab-1.5.2.dev1/netsim/ansible/templates/ospf/ios.ospfv3.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      194 2023-01-12 13:38:07.000000 networklab-1.5.2.dev1/netsim/ansible/templates/ospf/iosxr.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      948 2023-01-12 13:38:07.000000 networklab-1.5.2.dev1/netsim/ansible/templates/ospf/iosxr.ospfv2.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      936 2023-01-12 13:38:07.000000 networklab-1.5.2.dev1/netsim/ansible/templates/ospf/iosxr.ospfv3.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      430 2022-12-19 09:40:05.000000 networklab-1.5.2.dev1/netsim/ansible/templates/ospf/junos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1082 2022-12-19 09:40:05.000000 networklab-1.5.2.dev1/netsim/ansible/templates/ospf/junos.ospfv2.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1084 2022-12-19 09:40:05.000000 networklab-1.5.2.dev1/netsim/ansible/templates/ospf/junos.ospfv3.j2
+-rw-r--r--   0 pipi       (501) staff       (20)        0 2021-12-28 08:07:36.000000 networklab-1.5.2.dev1/netsim/ansible/templates/ospf/none.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      152 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/ospf/nxos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      987 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/ospf/nxos.ospfv2.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      995 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/ospf/nxos.ospfv3.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     2141 2022-04-06 16:02:55.000000 networklab-1.5.2.dev1/netsim/ansible/templates/ospf/routeros.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      478 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/ospf/routeros7.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1983 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/ospf/routeros7.ospf-include.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1145 2022-01-05 16:01:35.000000 networklab-1.5.2.dev1/netsim/ansible/templates/ospf/srlinux.cli.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      304 2022-08-27 11:27:47.000000 networklab-1.5.2.dev1/netsim/ansible/templates/ospf/srlinux.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1801 2023-04-11 06:23:20.000000 networklab-1.5.2.dev1/netsim/ansible/templates/ospf/srlinux.macro.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1653 2023-04-11 06:23:20.000000 networklab-1.5.2.dev1/netsim/ansible/templates/ospf/sros.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1038 2022-01-21 21:00:25.000000 networklab-1.5.2.dev1/netsim/ansible/templates/ospf/sros.md-cli.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      618 2021-12-28 08:07:36.000000 networklab-1.5.2.dev1/netsim/ansible/templates/ospf/sros.openconfig.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      385 2022-03-09 10:04:56.000000 networklab-1.5.2.dev1/netsim/ansible/templates/ospf/vyos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      957 2022-08-27 11:27:47.000000 networklab-1.5.2.dev1/netsim/ansible/templates/ospf/vyos.ospfv2.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      869 2022-08-27 11:27:47.000000 networklab-1.5.2.dev1/netsim/ansible/templates/ospf/vyos.ospfv3.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.252895 networklab-1.5.2.dev1/netsim/ansible/templates/sr/
+-rw-r--r--   0 pipi       (501) staff       (20)      245 2021-07-09 15:23:10.000000 networklab-1.5.2.dev1/netsim/ansible/templates/sr/eos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      270 2021-07-09 15:23:10.000000 networklab-1.5.2.dev1/netsim/ansible/templates/sr/ios.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1127 2023-01-12 13:45:42.000000 networklab-1.5.2.dev1/netsim/ansible/templates/sr/junos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     2286 2023-01-04 17:29:57.000000 networklab-1.5.2.dev1/netsim/ansible/templates/sr/srlinux.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1237 2023-01-04 17:30:40.000000 networklab-1.5.2.dev1/netsim/ansible/templates/sr/sros.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      945 2021-12-28 08:07:36.000000 networklab-1.5.2.dev1/netsim/ansible/templates/sr/sros.openconfig.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.253197 networklab-1.5.2.dev1/netsim/ansible/templates/srv6/
+-rw-r--r--   0 pipi       (501) staff       (20)     4092 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/srv6/sros.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.256696 networklab-1.5.2.dev1/netsim/ansible/templates/vlan/
+-rw-r--r--   0 pipi       (501) staff       (20)      561 2023-04-11 06:23:16.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vlan/arubacx.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1186 2022-12-18 14:12:35.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vlan/csr.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1730 2022-12-18 14:12:35.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vlan/cumulus.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      949 2022-11-17 08:20:15.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vlan/dellos10.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      757 2022-12-15 11:32:15.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vlan/eos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1212 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vlan/frr.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      457 2022-12-14 07:49:35.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vlan/ios.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      776 2022-08-27 11:27:47.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vlan/nxos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      432 2022-06-20 08:57:47.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vlan/routeros.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1115 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vlan/routeros7.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     2756 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vlan/srlinux.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1909 2023-04-02 11:32:00.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vlan/sros.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      815 2022-12-19 09:40:05.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vlan/vmx.j2
+-rw-r--r--   0 pipi       (501) staff       (20)       25 2022-12-19 09:40:05.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vlan/vsrx.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      771 2022-06-20 08:57:47.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vlan/vyos.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.274088 networklab-1.5.2.dev1/netsim/ansible/templates/vrf/
+-rw-r--r--   0 pipi       (501) staff       (20)     1381 2023-04-11 06:23:16.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vrf/arubacx.bgp-macro.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      920 2023-04-11 06:23:16.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vrf/arubacx.bgp.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      180 2023-04-11 06:23:16.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vrf/arubacx.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1068 2023-04-11 06:23:16.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vrf/arubacx.ospfv2-vrf.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      492 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vrf/cumulus.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      106 2022-04-17 16:31:22.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vrf/cumulus_nvue.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     2010 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vrf/dellos10.bgp-macro.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      690 2022-08-27 11:27:47.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vrf/dellos10.bgp.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      182 2022-09-10 16:16:52.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vrf/dellos10.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      888 2022-09-10 16:21:58.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vrf/dellos10.ospfv2-vrf.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      911 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vrf/eos.bgp-macro.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1189 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vrf/eos.bgp.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      172 2022-09-11 07:35:29.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vrf/eos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1027 2022-05-02 06:40:29.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vrf/eos.ospfv2-vrf.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1679 2023-01-12 13:38:07.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vrf/frr.bgp.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      412 2022-10-24 12:44:53.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vrf/frr.frr-config.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      524 2023-01-12 13:38:07.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vrf/frr.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      762 2023-01-12 13:38:07.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vrf/frr.ospfv2-vrf.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1539 2022-12-21 09:06:32.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vrf/ios.bgp-macro.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      716 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vrf/ios.bgp.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      172 2022-09-10 16:23:03.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vrf/ios.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      880 2022-10-24 08:27:03.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vrf/ios.ospfv2-vrf.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     2169 2022-12-19 09:40:05.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vrf/junos.bgp.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      693 2022-12-19 09:40:05.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vrf/junos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1169 2022-12-19 09:40:05.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vrf/junos.ospfv2-vrf.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1423 2022-08-27 11:27:47.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vrf/nxos.bgp.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      173 2022-08-27 11:27:47.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vrf/nxos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      989 2022-08-27 11:27:47.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vrf/nxos.ospfv2-vrf.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1109 2022-04-16 08:35:35.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vrf/routeros.bgp-macro.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1540 2022-08-18 15:19:05.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vrf/routeros.bgp.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      182 2022-04-06 16:02:55.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vrf/routeros.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1721 2022-05-01 16:20:27.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vrf/routeros.ospfv2-vrf.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1401 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vrf/routeros7.bgp-macro.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1095 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vrf/routeros7.bgp.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      185 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vrf/routeros7.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1983 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vrf/routeros7.ospf-include.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      463 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vrf/routeros7.ospfv2-vrf.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1336 2023-04-11 06:23:20.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vrf/srlinux.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      807 2023-04-11 06:23:20.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vrf/sros.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1323 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vrf/vyos.bgp-macro.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1272 2022-12-07 14:41:22.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vrf/vyos.bgp.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      535 2022-04-17 16:31:22.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vrf/vyos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1037 2022-04-17 16:31:22.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vrf/vyos.ospfv2-vrf.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.276942 networklab-1.5.2.dev1/netsim/ansible/templates/vxlan/
+-rw-r--r--   0 pipi       (501) staff       (20)      423 2023-04-11 06:23:16.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vxlan/arubacx.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      570 2022-12-18 14:12:35.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vxlan/csr.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1011 2022-12-15 13:56:36.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vxlan/cumulus.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      420 2022-09-16 11:40:01.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vxlan/dellos10.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      381 2022-12-15 14:02:16.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vxlan/eos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1651 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vxlan/frr.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      662 2022-12-15 14:02:29.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vxlan/nxos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     2219 2022-11-04 10:28:02.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vxlan/srlinux.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     2579 2022-11-04 10:28:02.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vxlan/sros.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1315 2022-09-16 11:40:09.000000 networklab-1.5.2.dev1/netsim/ansible/templates/vxlan/vyos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      740 2022-11-04 10:28:02.000000 networklab-1.5.2.dev1/netsim/api.py
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.280663 networklab-1.5.2.dev1/netsim/augment/
+-rw-r--r--   0 pipi       (501) staff       (20)      230 2023-04-08 17:21:52.000000 networklab-1.5.2.dev1/netsim/augment/__init__.py
+-rw-r--r--   0 pipi       (501) staff       (20)     6449 2023-04-10 10:09:55.000000 networklab-1.5.2.dev1/netsim/augment/components.py
+-rw-r--r--   0 pipi       (501) staff       (20)     2803 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/augment/config.py
+-rw-r--r--   0 pipi       (501) staff       (20)     3328 2023-04-02 11:32:00.000000 networklab-1.5.2.dev1/netsim/augment/devices.py
+-rw-r--r--   0 pipi       (501) staff       (20)    17286 2023-04-08 17:21:52.000000 networklab-1.5.2.dev1/netsim/augment/groups.py
+-rw-r--r--   0 pipi       (501) staff       (20)    39765 2023-04-08 17:21:52.000000 networklab-1.5.2.dev1/netsim/augment/links.py
+-rw-r--r--   0 pipi       (501) staff       (20)     3138 2023-04-10 10:09:55.000000 networklab-1.5.2.dev1/netsim/augment/main.py
+-rw-r--r--   0 pipi       (501) staff       (20)    12464 2023-04-13 14:55:11.000000 networklab-1.5.2.dev1/netsim/augment/nodes.py
+-rw-r--r--   0 pipi       (501) staff       (20)     2866 2023-04-13 14:06:49.000000 networklab-1.5.2.dev1/netsim/augment/plugin.py
+-rw-r--r--   0 pipi       (501) staff       (20)     5710 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/augment/topology.py
+-rw-r--r--   0 pipi       (501) staff       (20)     1152 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/callback.py
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.295676 networklab-1.5.2.dev1/netsim/cli/
+-rwxr-xr-x   0 pipi       (501) staff       (20)     8522 2023-04-10 10:10:02.000000 networklab-1.5.2.dev1/netsim/cli/__init__.py
+-rw-r--r--   0 pipi       (501) staff       (20)      319 2022-08-23 07:24:58.000000 networklab-1.5.2.dev1/netsim/cli/alias.txt
+-rw-r--r--   0 pipi       (501) staff       (20)     1758 2022-03-20 09:00:36.000000 networklab-1.5.2.dev1/netsim/cli/ansible.py
+-rw-r--r--   0 pipi       (501) staff       (20)     4192 2022-12-11 09:34:30.000000 networklab-1.5.2.dev1/netsim/cli/clab.py
+-rw-r--r--   0 pipi       (501) staff       (20)     2680 2022-03-20 09:12:02.000000 networklab-1.5.2.dev1/netsim/cli/collect.py
+-rw-r--r--   0 pipi       (501) staff       (20)     1392 2022-03-07 15:33:10.000000 networklab-1.5.2.dev1/netsim/cli/config.py
+-rw-r--r--   0 pipi       (501) staff       (20)     3684 2022-12-14 06:39:46.000000 networklab-1.5.2.dev1/netsim/cli/connect.py
+-rw-r--r--   0 pipi       (501) staff       (20)     2966 2022-11-04 10:28:02.000000 networklab-1.5.2.dev1/netsim/cli/create.py
+-rw-r--r--   0 pipi       (501) staff       (20)     5295 2023-04-13 15:09:55.000000 networklab-1.5.2.dev1/netsim/cli/down.py
+-rw-r--r--   0 pipi       (501) staff       (20)       63 2023-03-06 07:47:06.000000 networklab-1.5.2.dev1/netsim/cli/empty.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     3362 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/cli/external_commands.py
+-rw-r--r--   0 pipi       (501) staff       (20)     3181 2023-04-02 11:32:00.000000 networklab-1.5.2.dev1/netsim/cli/initial.py
+-rw-r--r--   0 pipi       (501) staff       (20)     2038 2021-12-28 08:07:36.000000 networklab-1.5.2.dev1/netsim/cli/install.py
+-rw-r--r--   0 pipi       (501) staff       (20)     9143 2023-04-02 11:32:00.000000 networklab-1.5.2.dev1/netsim/cli/libvirt.py
+-rw-r--r--   0 pipi       (501) staff       (20)     1332 2023-04-10 10:10:02.000000 networklab-1.5.2.dev1/netsim/cli/read.py
+-rw-r--r--   0 pipi       (501) staff       (20)     1408 2022-05-02 06:40:29.000000 networklab-1.5.2.dev1/netsim/cli/restart.py
+-rw-r--r--   0 pipi       (501) staff       (20)     4428 2023-03-06 07:47:06.000000 networklab-1.5.2.dev1/netsim/cli/show.py
+-rw-r--r--   0 pipi       (501) staff       (20)     4785 2023-04-02 11:32:00.000000 networklab-1.5.2.dev1/netsim/cli/status.py
+-rw-r--r--   0 pipi       (501) staff       (20)     3453 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/cli/test.py
+-rw-r--r--   0 pipi       (501) staff       (20)     9366 2023-04-02 11:32:00.000000 networklab-1.5.2.dev1/netsim/cli/up.py
+-rw-r--r--   0 pipi       (501) staff       (20)      417 2021-06-25 12:25:32.000000 networklab-1.5.2.dev1/netsim/cli/usage.py
+-rw-r--r--   0 pipi       (501) staff       (20)     1937 2022-08-27 11:27:47.000000 networklab-1.5.2.dev1/netsim/cli/usage.txt
+-rw-r--r--   0 pipi       (501) staff       (20)      180 2022-08-27 11:27:47.000000 networklab-1.5.2.dev1/netsim/cli/version.py
+-rw-r--r--   0 pipi       (501) staff       (20)     1488 2023-04-13 14:06:49.000000 networklab-1.5.2.dev1/netsim/common.py
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.297070 networklab-1.5.2.dev1/netsim/data/
+-rw-r--r--   0 pipi       (501) staff       (20)     5148 2023-04-10 13:06:35.000000 networklab-1.5.2.dev1/netsim/data/__init__.py
+-rw-r--r--   0 pipi       (501) staff       (20)     1097 2022-11-04 10:28:02.000000 networklab-1.5.2.dev1/netsim/data/global_vars.py
+-rw-r--r--   0 pipi       (501) staff       (20)    20668 2023-04-02 11:32:00.000000 networklab-1.5.2.dev1/netsim/data/types.py
+-rw-r--r--   0 pipi       (501) staff       (20)    19276 2023-04-02 11:32:00.000000 networklab-1.5.2.dev1/netsim/data/validate.py
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.298529 networklab-1.5.2.dev1/netsim/defaults/
+-rw-r--r--   0 pipi       (501) staff       (20)      294 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/defaults/addressing.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     2282 2023-04-02 11:32:00.000000 networklab-1.5.2.dev1/netsim/defaults/attributes.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      112 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/defaults/automation.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      378 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/defaults/hints.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      363 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/defaults/multilab.yml
+-rw-r--r--   0 pipi       (501) staff       (20)       86 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/defaults/ports.yml
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.309720 networklab-1.5.2.dev1/netsim/devices/
+-rw-r--r--   0 pipi       (501) staff       (20)     1844 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/devices/__init__.py
+-rw-r--r--   0 pipi       (501) staff       (20)      886 2023-04-11 06:23:16.000000 networklab-1.5.2.dev1/netsim/devices/arubacx.py
+-rw-r--r--   0 pipi       (501) staff       (20)     1128 2023-04-11 06:23:16.000000 networklab-1.5.2.dev1/netsim/devices/arubacx.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      996 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/devices/asav.py
+-rw-r--r--   0 pipi       (501) staff       (20)      798 2023-04-02 11:32:00.000000 networklab-1.5.2.dev1/netsim/devices/asav.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     1184 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/devices/csr.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     1049 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/devices/cumulus.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      748 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/devices/cumulus_nvue.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     1152 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/devices/dellos10.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     2273 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/devices/eos.py
+-rw-r--r--   0 pipi       (501) staff       (20)     1554 2023-02-12 08:44:04.000000 networklab-1.5.2.dev1/netsim/devices/eos.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      502 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/devices/fortios.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      927 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/devices/frr.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      854 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/devices/iosv.py
+-rw-r--r--   0 pipi       (501) staff       (20)     1372 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/devices/iosv.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      949 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/devices/iosxr.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     2346 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/devices/junos.py
+-rw-r--r--   0 pipi       (501) staff       (20)      705 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/devices/linux.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     1109 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/devices/none.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      858 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/devices/nxos.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      507 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/devices/routeros.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      910 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/devices/routeros7.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     1311 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/devices/srlinux.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     1634 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/devices/sros.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     2346 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/devices/vmx.py
+-rw-r--r--   0 pipi       (501) staff       (20)      827 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/devices/vmx.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     2346 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/devices/vsrx.py
+-rw-r--r--   0 pipi       (501) staff       (20)     1098 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/devices/vsrx.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     1008 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/devices/vyos.yml
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.186664 networklab-1.5.2.dev1/netsim/extra/
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.309915 networklab-1.5.2.dev1/netsim/extra/__pycache__/
+-rw-r--r--   0 pipi       (501) staff       (20)     2215 2022-09-04 16:06:08.000000 networklab-1.5.2.dev1/netsim/extra/__pycache__/ebgp-local_as.cpython-39.pyc
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.312621 networklab-1.5.2.dev1/netsim/extra/ebgp.utils/
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.312811 networklab-1.5.2.dev1/netsim/extra/ebgp.utils/__pycache__/
+-rw-r--r--   0 pipi       (501) staff       (20)     2171 2023-02-02 15:17:54.000000 networklab-1.5.2.dev1/netsim/extra/ebgp.utils/__pycache__/plugin.cpython-310.pyc
+-rw-r--r--   0 pipi       (501) staff       (20)      681 2022-12-22 16:28:14.000000 networklab-1.5.2.dev1/netsim/extra/ebgp.utils/default-originate.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     1198 2022-08-27 11:27:47.000000 networklab-1.5.2.dev1/netsim/extra/ebgp.utils/eos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1528 2022-08-27 11:27:47.000000 networklab-1.5.2.dev1/netsim/extra/ebgp.utils/ios.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1891 2022-12-19 09:40:05.000000 networklab-1.5.2.dev1/netsim/extra/ebgp.utils/junos.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     4428 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/extra/ebgp.utils/plugin.py
+-rw-r--r--   0 pipi       (501) staff       (20)     2924 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/extra/ebgp.utils/routeros7.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1695 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/extra/ebgp.utils/srlinux.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      263 2022-08-21 12:51:31.000000 networklab-1.5.2.dev1/netsim/extra/ebgp.utils/topology.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     2877 2022-08-27 11:27:47.000000 networklab-1.5.2.dev1/netsim/extra/ebgp.utils/vyos.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.313104 networklab-1.5.2.dev1/netsim/extra/multilab/
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.313364 networklab-1.5.2.dev1/netsim/extra/multilab/__pycache__/
+-rw-r--r--   0 pipi       (501) staff       (20)     1787 2023-01-30 16:32:51.000000 networklab-1.5.2.dev1/netsim/extra/multilab/__pycache__/plugin.cpython-310.pyc
+-rw-r--r--   0 pipi       (501) staff       (20)     3051 2023-02-07 15:05:29.000000 networklab-1.5.2.dev1/netsim/extra/multilab/plugin.py
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.313614 networklab-1.5.2.dev1/netsim/extra/none/
+-rw-r--r--   0 pipi       (501) staff       (20)        0 2021-12-28 08:07:36.000000 networklab-1.5.2.dev1/netsim/extra/none/none.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.314216 networklab-1.5.2.dev1/netsim/extra/proxy-arp/
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.314782 networklab-1.5.2.dev1/netsim/extra/proxy-arp/__pycache__/
+-rw-r--r--   0 pipi       (501) staff       (20)     1098 2023-02-02 15:17:59.000000 networklab-1.5.2.dev1/netsim/extra/proxy-arp/__pycache__/plugin.cpython-310.pyc
+-rw-r--r--   0 pipi       (501) staff       (20)      934 2022-10-24 08:42:48.000000 networklab-1.5.2.dev1/netsim/extra/proxy-arp/__pycache__/plugin.cpython-39.pyc
+-rw-r--r--   0 pipi       (501) staff       (20)      890 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/extra/proxy-arp/plugin.py
+-rw-r--r--   0 pipi       (501) staff       (20)      717 2022-11-04 10:28:02.000000 networklab-1.5.2.dev1/netsim/extra/proxy-arp/srlinux.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      682 2022-11-04 10:28:02.000000 networklab-1.5.2.dev1/netsim/extra/proxy-arp/sros.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.316152 networklab-1.5.2.dev1/netsim/install/
+-rwxr--r--   0 pipi       (501) staff       (20)     2162 2023-03-13 11:11:29.000000 networklab-1.5.2.dev1/netsim/install/ansible.sh
+-rwxr-xr-x   0 pipi       (501) staff       (20)     3484 2022-11-04 10:28:02.000000 networklab-1.5.2.dev1/netsim/install/containerlab.sh
+-rwxr-xr-x   0 pipi       (501) staff       (20)      745 2023-01-13 19:14:18.000000 networklab-1.5.2.dev1/netsim/install/grpc.sh
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.319478 networklab-1.5.2.dev1/netsim/install/libvirt/
+-rw-r--r--   0 pipi       (501) staff       (20)     1183 2023-04-11 06:23:16.000000 networklab-1.5.2.dev1/netsim/install/libvirt/arubacx.txt
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.319741 networklab-1.5.2.dev1/netsim/install/libvirt/asav/
+-rw-r--r--   0 pipi       (501) staff       (20)      972 2023-04-02 11:32:00.000000 networklab-1.5.2.dev1/netsim/install/libvirt/asav/day0-config
+-rw-r--r--   0 pipi       (501) staff       (20)      369 2023-04-02 11:32:00.000000 networklab-1.5.2.dev1/netsim/install/libvirt/asav.txt
+-rw-r--r--   0 pipi       (501) staff       (20)     1219 2022-12-11 18:08:47.000000 networklab-1.5.2.dev1/netsim/install/libvirt/csr.txt
+-rw-r--r--   0 pipi       (501) staff       (20)     1493 2022-04-17 16:31:22.000000 networklab-1.5.2.dev1/netsim/install/libvirt/dellos10.txt
+-rw-r--r--   0 pipi       (501) staff       (20)     2214 2022-03-09 10:04:56.000000 networklab-1.5.2.dev1/netsim/install/libvirt/eos.txt
+-rw-r--r--   0 pipi       (501) staff       (20)     1531 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/install/libvirt/eos.xml.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1665 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/install/libvirt/iosv.txt
+-rw-r--r--   0 pipi       (501) staff       (20)     2911 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/install/libvirt/iosv.xml.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.319959 networklab-1.5.2.dev1/netsim/install/libvirt/iosxr/
+-rw-r--r--   0 pipi       (501) staff       (20)      360 2022-12-21 10:32:36.000000 networklab-1.5.2.dev1/netsim/install/libvirt/iosxr/iosxr_config.txt
+-rw-r--r--   0 pipi       (501) staff       (20)     1044 2023-01-12 13:38:07.000000 networklab-1.5.2.dev1/netsim/install/libvirt/iosxr.txt
+-rw-r--r--   0 pipi       (501) staff       (20)     1524 2022-01-28 18:41:01.000000 networklab-1.5.2.dev1/netsim/install/libvirt/nxos.txt
+-rw-r--r--   0 pipi       (501) staff       (20)     1523 2022-09-25 07:16:04.000000 networklab-1.5.2.dev1/netsim/install/libvirt/nxos.xml.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      940 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/install/libvirt/routeros7.txt
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.320289 networklab-1.5.2.dev1/netsim/install/libvirt/vsrx/
+-rw-r--r--   0 pipi       (501) staff       (20)     2243 2022-03-09 10:04:56.000000 networklab-1.5.2.dev1/netsim/install/libvirt/vsrx/juniper.conf
+-rw-r--r--   0 pipi       (501) staff       (20)      540 2022-03-09 10:04:56.000000 networklab-1.5.2.dev1/netsim/install/libvirt/vsrx.txt
+-rwxr-xr-x   0 pipi       (501) staff       (20)     3179 2023-01-12 13:45:42.000000 networklab-1.5.2.dev1/netsim/install/libvirt.sh
+-rwxr-xr-x   0 pipi       (501) staff       (20)     1881 2022-11-04 10:28:02.000000 networklab-1.5.2.dev1/netsim/install/ubuntu.sh
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.328574 networklab-1.5.2.dev1/netsim/modules/
+-rw-r--r--   0 pipi       (501) staff       (20)    21902 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/modules/__init__.py
+-rw-r--r--   0 pipi       (501) staff       (20)     6194 2023-04-02 11:32:00.000000 networklab-1.5.2.dev1/netsim/modules/_dataplane.py
+-rw-r--r--   0 pipi       (501) staff       (20)    10483 2023-01-14 11:38:47.000000 networklab-1.5.2.dev1/netsim/modules/_routing.py
+-rw-r--r--   0 pipi       (501) staff       (20)     3923 2023-01-14 09:41:51.000000 networklab-1.5.2.dev1/netsim/modules/bfd.py
+-rw-r--r--   0 pipi       (501) staff       (20)      702 2023-04-11 06:23:16.000000 networklab-1.5.2.dev1/netsim/modules/bfd.yml
+-rw-r--r--   0 pipi       (501) staff       (20)    20279 2023-03-20 10:56:19.000000 networklab-1.5.2.dev1/netsim/modules/bgp.py
+-rw-r--r--   0 pipi       (501) staff       (20)     1470 2023-04-11 06:23:16.000000 networklab-1.5.2.dev1/netsim/modules/bgp.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      496 2023-01-12 16:03:44.000000 networklab-1.5.2.dev1/netsim/modules/eigrp.py
+-rw-r--r--   0 pipi       (501) staff       (20)      324 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/modules/eigrp.yml
+-rw-r--r--   0 pipi       (501) staff       (20)    17812 2022-11-13 15:34:41.000000 networklab-1.5.2.dev1/netsim/modules/evpn.py
+-rw-r--r--   0 pipi       (501) staff       (20)      892 2023-04-11 06:23:16.000000 networklab-1.5.2.dev1/netsim/modules/evpn.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     6795 2023-04-02 11:32:00.000000 networklab-1.5.2.dev1/netsim/modules/gateway.py
+-rw-r--r--   0 pipi       (501) staff       (20)      960 2023-04-11 06:23:16.000000 networklab-1.5.2.dev1/netsim/modules/gateway.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     2579 2023-01-12 13:38:07.000000 networklab-1.5.2.dev1/netsim/modules/isis.py
+-rw-r--r--   0 pipi       (501) staff       (20)      906 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/modules/isis.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     7057 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/modules/mpls.py
+-rw-r--r--   0 pipi       (501) staff       (20)      879 2023-04-11 06:23:16.000000 networklab-1.5.2.dev1/netsim/modules/mpls.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     3036 2023-01-14 10:57:46.000000 networklab-1.5.2.dev1/netsim/modules/ospf.py
+-rw-r--r--   0 pipi       (501) staff       (20)     1033 2023-04-11 06:23:16.000000 networklab-1.5.2.dev1/netsim/modules/ospf.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      152 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/modules/sr.py
+-rw-r--r--   0 pipi       (501) staff       (20)      390 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/modules/sr.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      910 2023-01-14 09:55:20.000000 networklab-1.5.2.dev1/netsim/modules/srv6.py
+-rw-r--r--   0 pipi       (501) staff       (20)      420 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/modules/srv6.yml
+-rw-r--r--   0 pipi       (501) staff       (20)    58915 2023-04-02 11:32:00.000000 networklab-1.5.2.dev1/netsim/modules/vlan.py
+-rw-r--r--   0 pipi       (501) staff       (20)     1022 2023-04-11 06:23:16.000000 networklab-1.5.2.dev1/netsim/modules/vlan.yml
+-rw-r--r--   0 pipi       (501) staff       (20)    20566 2023-04-02 11:32:00.000000 networklab-1.5.2.dev1/netsim/modules/vrf.py
+-rw-r--r--   0 pipi       (501) staff       (20)      431 2023-04-11 06:23:16.000000 networklab-1.5.2.dev1/netsim/modules/vrf.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     9079 2022-12-11 09:34:30.000000 networklab-1.5.2.dev1/netsim/modules/vxlan.py
+-rw-r--r--   0 pipi       (501) staff       (20)      564 2023-04-11 06:23:16.000000 networklab-1.5.2.dev1/netsim/modules/vxlan.yml
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.334088 networklab-1.5.2.dev1/netsim/outputs/
+-rw-r--r--   0 pipi       (501) staff       (20)     2277 2023-04-02 11:32:00.000000 networklab-1.5.2.dev1/netsim/outputs/__init__.py
+-rw-r--r--   0 pipi       (501) staff       (20)     7081 2023-04-02 11:32:00.000000 networklab-1.5.2.dev1/netsim/outputs/ansible.py
+-rw-r--r--   0 pipi       (501) staff       (20)     1745 2022-01-21 21:02:25.000000 networklab-1.5.2.dev1/netsim/outputs/common.py
+-rw-r--r--   0 pipi       (501) staff       (20)     9596 2023-04-02 11:32:00.000000 networklab-1.5.2.dev1/netsim/outputs/d2.py
+-rw-r--r--   0 pipi       (501) staff       (20)      468 2023-04-02 11:32:00.000000 networklab-1.5.2.dev1/netsim/outputs/d2.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     2739 2023-04-02 11:32:00.000000 networklab-1.5.2.dev1/netsim/outputs/devices.py
+-rw-r--r--   0 pipi       (501) staff       (20)     1268 2022-11-04 10:28:02.000000 networklab-1.5.2.dev1/netsim/outputs/format.py
+-rw-r--r--   0 pipi       (501) staff       (20)     7581 2022-11-04 10:28:02.000000 networklab-1.5.2.dev1/netsim/outputs/graph.py
+-rw-r--r--   0 pipi       (501) staff       (20)      218 2023-04-02 11:32:00.000000 networklab-1.5.2.dev1/netsim/outputs/graph.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     5504 2022-11-04 10:28:02.000000 networklab-1.5.2.dev1/netsim/outputs/graphite.py
+-rw-r--r--   0 pipi       (501) staff       (20)      278 2021-08-22 05:50:16.000000 networklab-1.5.2.dev1/netsim/outputs/json.py
+-rw-r--r--   0 pipi       (501) staff       (20)      228 2021-12-18 16:49:49.000000 networklab-1.5.2.dev1/netsim/outputs/none.py
+-rw-r--r--   0 pipi       (501) staff       (20)     1838 2023-04-02 11:32:00.000000 networklab-1.5.2.dev1/netsim/outputs/provider.py
+-rw-r--r--   0 pipi       (501) staff       (20)     1711 2023-04-02 11:32:00.000000 networklab-1.5.2.dev1/netsim/outputs/yaml.py
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.340730 networklab-1.5.2.dev1/netsim/providers/
+-rw-r--r--   0 pipi       (501) staff       (20)     7882 2023-04-11 06:23:16.000000 networklab-1.5.2.dev1/netsim/providers/__init__.py
+-rw-r--r--   0 pipi       (501) staff       (20)     3733 2023-04-11 06:23:16.000000 networklab-1.5.2.dev1/netsim/providers/clab.py
+-rw-r--r--   0 pipi       (501) staff       (20)      517 2023-04-02 11:32:00.000000 networklab-1.5.2.dev1/netsim/providers/clab.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      836 2022-12-24 16:57:23.000000 networklab-1.5.2.dev1/netsim/providers/external.py
+-rw-r--r--   0 pipi       (501) staff       (20)      157 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/providers/external.yml
+-rw-r--r--   0 pipi       (501) staff       (20)    11317 2023-04-02 11:32:00.000000 networklab-1.5.2.dev1/netsim/providers/libvirt.py
+-rw-r--r--   0 pipi       (501) staff       (20)      481 2023-04-02 11:32:00.000000 networklab-1.5.2.dev1/netsim/providers/libvirt.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      210 2022-12-24 16:57:30.000000 networklab-1.5.2.dev1/netsim/providers/virtualbox.py
+-rw-r--r--   0 pipi       (501) staff       (20)      320 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/providers/virtualbox.yml
+-rw-r--r--   0 pipi       (501) staff       (20)     7937 2023-04-10 09:56:31.000000 networklab-1.5.2.dev1/netsim/read_topology.py
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.340903 networklab-1.5.2.dev1/netsim/templates/
+-rw-r--r--   0 pipi       (501) staff       (20)      469 2022-05-26 14:27:51.000000 networklab-1.5.2.dev1/netsim/templates/ansible.cfg.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.187894 networklab-1.5.2.dev1/netsim/templates/provider/
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.341175 networklab-1.5.2.dev1/netsim/templates/provider/clab/
+-rw-r--r--   0 pipi       (501) staff       (20)     3077 2023-04-11 06:23:16.000000 networklab-1.5.2.dev1/netsim/templates/provider/clab/clab.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.341380 networklab-1.5.2.dev1/netsim/templates/provider/clab/frr/
+-rw-r--r--   0 pipi       (501) staff       (20)     2935 2023-01-12 13:38:07.000000 networklab-1.5.2.dev1/netsim/templates/provider/clab/frr/daemons.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.341706 networklab-1.5.2.dev1/netsim/templates/provider/clab/linux/
+-rw-r--r--   0 pipi       (501) staff       (20)      604 2023-01-12 13:45:42.000000 networklab-1.5.2.dev1/netsim/templates/provider/clab/linux/hosts.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.342041 networklab-1.5.2.dev1/netsim/templates/provider/external/
+-rw-r--r--   0 pipi       (501) staff       (20)     1318 2022-12-18 14:12:35.000000 networklab-1.5.2.dev1/netsim/templates/provider/external/external.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.349287 networklab-1.5.2.dev1/netsim/templates/provider/libvirt/
+-rw-r--r--   0 pipi       (501) staff       (20)      541 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/templates/provider/libvirt/Vagrantfile.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      332 2022-01-25 17:29:43.000000 networklab-1.5.2.dev1/netsim/templates/provider/libvirt/arcos-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      410 2023-04-11 06:23:16.000000 networklab-1.5.2.dev1/netsim/templates/provider/libvirt/arubacx-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      427 2022-11-10 07:29:53.000000 networklab-1.5.2.dev1/netsim/templates/provider/libvirt/asav-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      445 2022-12-11 17:33:57.000000 networklab-1.5.2.dev1/netsim/templates/provider/libvirt/csr-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      190 2022-01-25 17:59:15.000000 networklab-1.5.2.dev1/netsim/templates/provider/libvirt/cumulus-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1177 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/templates/provider/libvirt/cumulus_nvue-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1297 2023-03-06 07:47:06.000000 networklab-1.5.2.dev1/netsim/templates/provider/libvirt/define-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      438 2022-04-17 16:31:22.000000 networklab-1.5.2.dev1/netsim/templates/provider/libvirt/dellos10-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      355 2022-01-25 17:30:38.000000 networklab-1.5.2.dev1/netsim/templates/provider/libvirt/eos-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      258 2022-01-25 17:30:42.000000 networklab-1.5.2.dev1/netsim/templates/provider/libvirt/fortios-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      380 2022-12-11 10:03:46.000000 networklab-1.5.2.dev1/netsim/templates/provider/libvirt/iosv-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1835 2023-01-12 13:38:07.000000 networklab-1.5.2.dev1/netsim/templates/provider/libvirt/iosxr-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      486 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/templates/provider/libvirt/libvirt-bridge.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      668 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/templates/provider/libvirt/libvirt-tunnel.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      190 2022-01-25 17:30:59.000000 networklab-1.5.2.dev1/netsim/templates/provider/libvirt/linux-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)       52 2021-12-28 08:07:36.000000 networklab-1.5.2.dev1/netsim/templates/provider/libvirt/none-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      814 2022-12-12 17:43:45.000000 networklab-1.5.2.dev1/netsim/templates/provider/libvirt/nxos-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      309 2022-01-25 17:31:10.000000 networklab-1.5.2.dev1/netsim/templates/provider/libvirt/routeros-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      347 2022-10-19 17:10:38.000000 networklab-1.5.2.dev1/netsim/templates/provider/libvirt/routeros7-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)     1283 2023-01-28 07:18:50.000000 networklab-1.5.2.dev1/netsim/templates/provider/libvirt/vagrant-libvirt.xml
+-rw-r--r--   0 pipi       (501) staff       (20)      740 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/templates/provider/libvirt/vsrx-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      223 2022-01-25 17:31:29.000000 networklab-1.5.2.dev1/netsim/templates/provider/libvirt/vyos-domain.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.351375 networklab-1.5.2.dev1/netsim/templates/provider/virtualbox/
+-rw-r--r--   0 pipi       (501) staff       (20)      782 2022-05-02 06:40:29.000000 networklab-1.5.2.dev1/netsim/templates/provider/virtualbox/Vagrantfile.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      274 2022-01-25 17:34:51.000000 networklab-1.5.2.dev1/netsim/templates/provider/virtualbox/arcos-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      192 2022-09-05 16:28:24.000000 networklab-1.5.2.dev1/netsim/templates/provider/virtualbox/cumulus-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      108 2022-01-25 17:35:32.000000 networklab-1.5.2.dev1/netsim/templates/provider/virtualbox/eos-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      191 2022-01-25 17:35:37.000000 networklab-1.5.2.dev1/netsim/templates/provider/virtualbox/linux-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      321 2022-01-25 17:36:47.000000 networklab-1.5.2.dev1/netsim/templates/provider/virtualbox/nxos-domain.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      217 2021-04-11 18:37:32.000000 networklab-1.5.2.dev1/netsim/templates/provider/virtualbox/virtualbox-network.j2
+-rw-r--r--   0 pipi       (501) staff       (20)      323 2021-04-11 18:37:32.000000 networklab-1.5.2.dev1/netsim/templates/provider/virtualbox/virtualbox-ports.j2
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.352201 networklab-1.5.2.dev1/netsim/templates/tests/
+-rw-r--r--   0 pipi       (501) staff       (20)      255 2022-12-11 17:33:46.000000 networklab-1.5.2.dev1/netsim/templates/tests/clab.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      181 2022-12-11 09:54:53.000000 networklab-1.5.2.dev1/netsim/templates/tests/libvirt.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      185 2022-12-11 09:54:58.000000 networklab-1.5.2.dev1/netsim/templates/tests/virtualbox.yml
+-rw-r--r--   0 pipi       (501) staff       (20)      496 2023-04-02 11:32:00.000000 networklab-1.5.2.dev1/netsim/topology-defaults.yml
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.353490 networklab-1.5.2.dev1/netsim/utils/
+-rw-r--r--   0 pipi       (501) staff       (20)       78 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/utils/__init__.py
+-rw-r--r--   0 pipi       (501) staff       (20)     4068 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/netsim/utils/log.py
+-rw-r--r--   0 pipi       (501) staff       (20)     3248 2023-04-02 11:32:00.000000 networklab-1.5.2.dev1/netsim/utils/status.py
+-rw-r--r--   0 pipi       (501) staff       (20)     1277 2023-04-02 11:32:00.000000 networklab-1.5.2.dev1/netsim/utils/strings.py
+-rw-r--r--   0 pipi       (501) staff       (20)     4906 2023-04-13 14:06:49.000000 networklab-1.5.2.dev1/netsim/utils/templates.py
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.354484 networklab-1.5.2.dev1/networklab.egg-info/
+-rw-r--r--   0 pipi       (501) staff       (20)     4081 2023-04-15 09:01:42.000000 networklab-1.5.2.dev1/networklab.egg-info/PKG-INFO
+-rw-r--r--   0 pipi       (501) staff       (20)    20481 2023-04-15 09:01:42.000000 networklab-1.5.2.dev1/networklab.egg-info/SOURCES.txt
+-rw-r--r--   0 pipi       (501) staff       (20)        1 2023-04-15 09:01:42.000000 networklab-1.5.2.dev1/networklab.egg-info/dependency_links.txt
+-rw-r--r--   0 pipi       (501) staff       (20)       51 2023-04-15 09:01:42.000000 networklab-1.5.2.dev1/networklab.egg-info/entry_points.txt
+-rw-r--r--   0 pipi       (501) staff       (20)      122 2023-04-15 09:01:42.000000 networklab-1.5.2.dev1/networklab.egg-info/requires.txt
+-rw-r--r--   0 pipi       (501) staff       (20)        7 2023-04-15 09:01:42.000000 networklab-1.5.2.dev1/networklab.egg-info/top_level.txt
+-rw-r--r--   0 pipi       (501) staff       (20)      183 2023-04-02 11:32:00.000000 networklab-1.5.2.dev1/requirements.txt
+-rw-r--r--   0 pipi       (501) staff       (20)       38 2023-04-15 09:01:42.355170 networklab-1.5.2.dev1/setup.cfg
+-rw-r--r--   0 pipi       (501) staff       (20)     1477 2022-11-25 15:02:55.000000 networklab-1.5.2.dev1/setup.py
+drwxr-xr-x   0 pipi       (501) staff       (20)        0 2023-04-15 09:01:42.354616 networklab-1.5.2.dev1/tests/
+-rwxr-xr-x   0 pipi       (501) staff       (20)     3462 2023-01-28 06:30:20.000000 networklab-1.5.2.dev1/tests/test_transformation.py
```

### Comparing `networklab-1.5.1.dev1/LICENSE.md` & `networklab-1.5.2.dev1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/PKG-INFO` & `networklab-1.5.2.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: networklab
-Version: 1.5.1.dev1
+Version: 1.5.2.dev1
 Summary: CLI-based Virtual Networking Lab Abstraction Layer
 Home-page: https://github.com/ipspace/netlab
 Author: Ivan Pepelnjak
 Author-email: ip@ipspace.net
 Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -30,15 +30,15 @@
 
 Instead of wasting time creating lab topology in a GUI and configuring boring details, you'll start with a lab preconfigured according to your specifications.
 
 Interested? [Read the documentation](https://netsim-tools.readthedocs.io/) and [installation guidelines](https://netsim-tools.readthedocs.io/en/latest/install.html).
 
 ## Releases
 
-The latest release is [release 1.5.0](https://github.com/ipspace/netlab/releases/tag/release_1.5.0). We redesigned topology validation in release 1.5.0, resulting in potentially breaking changes. If you're a long-time _netlab_ user, please read the [release notes](https://netsim-tools.readthedocs.io/en/latest/release.html) first.
+The latest release is [release 1.5.1](https://github.com/ipspace/netlab/releases/tag/release_1.5.1). We redesigned topology validation in release 1.5.0, resulting in potentially breaking changes. If you're a long-time _netlab_ user, please read the [release notes](https://netsim-tools.readthedocs.io/en/latest/release.html) first.
 
 The latest release before the changes made in release 1.5.0 is [release 1.4.3](https://github.com/ipspace/netlab/releases/tag/release_1.4.3).
 
 ## An overview of tools:
 
 **netlab up**
 : Uses **netlab create** to create configuration files, starts the virtual lab, and uses **netlab initial** to deploy device configurations. [More details](https://netsim-tools.readthedocs.io/en/latest/netlab/up.html)
```

### Comparing `networklab-1.5.1.dev1/README.md` & `networklab-1.5.2.dev1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 Instead of wasting time creating lab topology in a GUI and configuring boring details, you'll start with a lab preconfigured according to your specifications.
 
 Interested? [Read the documentation](https://netsim-tools.readthedocs.io/) and [installation guidelines](https://netsim-tools.readthedocs.io/en/latest/install.html).
 
 ## Releases
 
-The latest release is [release 1.5.0](https://github.com/ipspace/netlab/releases/tag/release_1.5.0). We redesigned topology validation in release 1.5.0, resulting in potentially breaking changes. If you're a long-time _netlab_ user, please read the [release notes](https://netsim-tools.readthedocs.io/en/latest/release.html) first.
+The latest release is [release 1.5.1](https://github.com/ipspace/netlab/releases/tag/release_1.5.1). We redesigned topology validation in release 1.5.0, resulting in potentially breaking changes. If you're a long-time _netlab_ user, please read the [release notes](https://netsim-tools.readthedocs.io/en/latest/release.html) first.
 
 The latest release before the changes made in release 1.5.0 is [release 1.4.3](https://github.com/ipspace/netlab/releases/tag/release_1.4.3).
 
 ## An overview of tools:
 
 **netlab up**
 : Uses **netlab create** to create configuration files, starts the virtual lab, and uses **netlab initial** to deploy device configurations. [More details](https://netsim-tools.readthedocs.io/en/latest/netlab/up.html)
```

### Comparing `networklab-1.5.1.dev1/netsim/addressing.py` & `networklab-1.5.2.dev1/netsim/addressing.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/collect-configs.ansible` & `networklab-1.5.2.dev1/netsim/ansible/collect-configs.ansible`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/create-config.ansible` & `networklab-1.5.2.dev1/netsim/ansible/create-config.ansible`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/initial-config.ansible` & `networklab-1.5.2.dev1/netsim/ansible/initial-config.ansible`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/tasks/create-config.yml` & `networklab-1.5.2.dev1/netsim/ansible/tasks/create-config.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/tasks/deploy-config/cumulus.yml` & `networklab-1.5.2.dev1/netsim/ansible/tasks/deploy-config/cumulus.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/tasks/deploy-config/cumulus_nvue.yml` & `networklab-1.5.2.dev1/netsim/ansible/tasks/deploy-config/cumulus_nvue.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/tasks/deploy-config/frr.yml` & `networklab-1.5.2.dev1/netsim/ansible/tasks/deploy-config/frr.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/tasks/deploy-config/routeros.yml` & `networklab-1.5.2.dev1/netsim/ansible/tasks/deploy-config/routeros.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/tasks/deploy-config/srlinux.yml` & `networklab-1.5.2.dev1/netsim/ansible/tasks/deploy-config/srlinux.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/tasks/deploy-config/sros.yml` & `networklab-1.5.2.dev1/netsim/ansible/tasks/deploy-config/sros.yml`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,16 @@
   set_fact:
     sros_provisioning_model: "sros" # Default: without '.gnmi'
 
 - name: Select provisioning template netsim_action={{ netsim_action }}
   set_fact:
     template_to_use: "{{ config_template|replace('sros.j2',sros_provisioning_model+'.j2') }}"
 
-- local_action:
+- name: Process template {{ template_to_use }}
+  local_action:
     module: template
     src: "{{ template_to_use }}"
     dest: "{{ tempfile_1.path }}"
 
 - block:
   - name: Show generated config from {{template_to_use}} based on {{tempfile_1.path}}
     debug: msg="{{ cfg }}" verbosity=1
```

### Comparing `networklab-1.5.1.dev1/netsim/ansible/tasks/deploy-config/vyos.yml` & `networklab-1.5.2.dev1/netsim/ansible/tasks/deploy-config/vyos.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/tasks/deploy-custom-config.yml` & `networklab-1.5.2.dev1/netsim/ansible/tasks/deploy-custom-config.yml`

 * *Files 14% similar despite different names*

```diff
@@ -6,38 +6,51 @@
   tags: [ always ]
   vars:
     params:
       paths:
       - "{{ lookup('env','PWD') }}"
       - "../../extra"
       files:
+      - "{{ custom_config + '/' + inventory_hostname + '.' + netlab_device_type + '-' + netlab_provider + '.j2' }}"
+      - "{{ custom_config + '/' + inventory_hostname + '.' + netlab_device_type + '.j2' }}"
+      - "{{ custom_config + '/' + inventory_hostname + '.j2' }}"
       - "{{ custom_config + '/' + netlab_device_type + '-' + netlab_provider + '.j2' }}"
       - "{{ custom_config + '/' + netlab_device_type + '.j2' }}"
-      - "{{ custom_config + '.' + netlab_device_type + '.j2' }}"
       - "{{ custom_config + '/' + ansible_network_os + '-' + netlab_provider + '.j2' }}"
       - "{{ custom_config + '/' + ansible_network_os + '.j2' }}"
+      - "{{ custom_config + '.' + inventory_hostname + '.' + netlab_device_type + '.j2' }}"
+      - "{{ custom_config + '.' + inventory_hostname + '.' + ansible_network_os + '.j2' }}"
+      - "{{ custom_config + '.' + inventory_hostname + '.j2' }}"
+      - "{{ custom_config + '.' + netlab_device_type + '.j2' }}"
       - "{{ custom_config + '.' + ansible_network_os + '.j2' }}"
       - "{{ custom_config }}"
       - "{{ custom_config + '.j2' }}"
 
 - fail: msg="Cannot find configuration template {{ custom_config }} for device {{ inventory_hostname }}"
   when: config_template == ''
   tags: [ always ]
 
-- debug:
+- name: "Process template {{ config_template }} for {{ inventory_hostname }}"
+  debug:
     msg: |
       {{ config_template }} configuration for {{ inventory_hostname }}
       =========================================
       {{ lookup('template',config_template) }}
     verbosity: 1
   tags: [ test,custom ]
 
 - include_tasks: "{{ item }}"
   tags: [ custom ]
   with_first_found:
+  - "{{ lookup('env','PWD') }}/{{ custom_config }}/deploy-{{ inventory_hostname }}.yml"
+  - "{{ lookup('env','PWD') }}/{{ custom_config }}/deploy.{{ netlab_device_type }}-{{ netlab_provider }}.yml"
+  - "{{ lookup('env','PWD') }}/{{ custom_config }}/deploy.{{ netlab_device_type }}.yml"
+  - "{{ lookup('env','PWD') }}/{{ custom_config }}/deploy.{{ ansible_network_os }}-{{ netlab_provider }}.yml"
+  - "{{ lookup('env','PWD') }}/{{ custom_config }}/deploy.{{ ansible_network_os }}.yml"
+  - "{{ lookup('env','PWD') }}/{{ custom_config }}/deploy.yml"
   - "../../extra/{{ custom_config }}/deploy.{{ netlab_device_type }}-{{ netlab_provider }}.yml"
   - "../../extra/{{ custom_config }}/deploy.{{ netlab_device_type }}.yml"
   - "deploy-config/{{netlab_device_type}}-{{ netlab_provider }}.yml"
   - "deploy-config/{{netlab_device_type}}.yml"
   - "../../extra/{{ custom_config }}/deploy.{{ ansible_network_os }}-{{ netlab_provider }}.yml"
   - "../../extra/{{ custom_config }}/deploy.{{ ansible_network_os }}.yml"
   - "deploy-config/{{ansible_network_os}}-{{ netlab_provider }}.yml"
```

### Comparing `networklab-1.5.1.dev1/netsim/ansible/tasks/deploy-module.yml` & `networklab-1.5.2.dev1/netsim/ansible/tasks/deploy-module.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/tasks/fetch-config/srlinux.yml` & `networklab-1.5.2.dev1/netsim/ansible/tasks/fetch-config/srlinux.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/tasks/fortinet.fortios.fortios/initial.yml` & `networklab-1.5.2.dev1/netsim/ansible/tasks/fortinet.fortios.fortios/initial.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/tasks/fortinet.fortios.fortios/ospf.yml` & `networklab-1.5.2.dev1/netsim/ansible/tasks/fortinet.fortios.fortios/ospf.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/tasks/iosxr/initial.yml` & `networklab-1.5.2.dev1/netsim/ansible/tasks/iosxr/initial.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/tasks/linux/initial-clab.yml` & `networklab-1.5.2.dev1/netsim/ansible/tasks/linux/initial-clab.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/tasks/vmx/initial.yml` & `networklab-1.5.2.dev1/netsim/ansible/tasks/vmx/initial.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/bfd/eos.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/bfd/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/bfd/ios.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/bfd/ios.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/bfd/nxos.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/bfd/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/bfd/srlinux.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/bfd/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/bfd/sros.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/bfd/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/bgp/asa.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/bgp/asa.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/bgp/asa.macro.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/bgp/asa.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/bgp/cumulus_nvue.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/bgp/cumulus_nvue.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/bgp/dellos10.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/bgp/dellos10.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/bgp/dellos10.macro.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/bgp/dellos10.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/bgp/eos.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/bgp/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/bgp/eos.macro.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/bgp/eos.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/bgp/frr.bgp-config.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/bgp/frr.bgp-config.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/bgp/ios.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/bgp/ios.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/bgp/ios.macro.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/bgp/ios.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/bgp/iosxr.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/bgp/iosxr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/bgp/junos.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/bgp/junos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/bgp/nxos.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/bgp/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/bgp/routeros.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/bgp/routeros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/bgp/routeros.macro.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/bgp/routeros.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/bgp/routeros7.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/bgp/routeros7.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/bgp/routeros7.macro.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/bgp/routeros7.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/bgp/srlinux.cli.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/bgp/srlinux.cli.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/bgp/srlinux.macro.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/bgp/srlinux.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/bgp/sros.gnmi.macro.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/bgp/sros.gnmi.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/bgp/sros.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/bgp/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/bgp/sros.md-cli.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/bgp/sros.md-cli.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/bgp/sros.openconfig.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/bgp/sros.openconfig.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/bgp/vyos.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/bgp/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/bgp/vyos.macro.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/bgp/vyos.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/eigrp/ios.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/eigrp/ios.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/eigrp/nxos.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/eigrp/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/evpn/cumulus.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/evpn/cumulus.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/evpn/dellos10.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/evpn/dellos10.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/evpn/eos.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/evpn/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/evpn/frr.evpn-config.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/evpn/frr.evpn-config.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/evpn/nxos.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/evpn/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/evpn/srlinux.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/evpn/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/evpn/vyos.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/evpn/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/gateway/cumulus.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/gateway/cumulus.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/gateway/dellos10.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/gateway/dellos10.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/gateway/eos.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/gateway/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/gateway/ios.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/gateway/ios.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/gateway/nxos.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/gateway/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/gateway/srlinux.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/gateway/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/gateway/sros.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/gateway/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/gateway/vyos.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/gateway/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/initial/arcos.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/initial/arcos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/initial/asa.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/initial/asa.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/initial/cumulus.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/initial/cumulus.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/initial/cumulus_nvue.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/initial/cumulus_nvue.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/initial/dellos10.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/initial/dellos10.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/initial/dellos10.vrf.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/initial/dellos10.vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/initial/eos.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/initial/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/initial/frr.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/initial/frr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/initial/ios.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/initial/ios.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/initial/iosxr.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/initial/iosxr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/initial/junos.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/initial/junos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/initial/junos.vlan.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/initial/junos.vlan.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/initial/junos.vrf.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/initial/junos.vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/initial/linux/hosts.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/initial/linux/hosts.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/initial/linux/ubuntu.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/initial/linux/ubuntu.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/initial/linux/vanilla.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/initial/linux/vanilla.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/initial/nxos.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/initial/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/initial/routeros.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/initial/routeros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/initial/routeros.vlan.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/initial/routeros.vlan.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/initial/routeros7.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/initial/routeros7.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/initial/routeros7.vlan.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/initial/routeros7.vlan.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/initial/srlinux.cli.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/initial/srlinux.cli.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/initial/srlinux.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/initial/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/initial/sros.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/initial/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/initial/sros.md-cli.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/initial/sros.md-cli.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/initial/sros.openconfig.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/initial/sros.openconfig.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/initial/vyos.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/initial/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/isis/asa.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/isis/asa.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/isis/eos.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/isis/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/isis/frr.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/isis/frr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/isis/ios.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/isis/ios.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/isis/iosxr.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/isis/iosxr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/isis/junos.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/isis/junos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/isis/nxos.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/isis/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/isis/srlinux.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/isis/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/isis/sros.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/isis/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/isis/sros.openconfig.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/isis/sros.openconfig.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/isis/vyos.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/isis/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/mpls/eos.6pe.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/mpls/eos.6pe.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/mpls/eos.bgp-lu.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/mpls/eos.bgp-lu.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/mpls/ios.bgp-lu.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/mpls/ios.bgp-lu.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/mpls/junos.ldp.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/mpls/junos.ldp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/mpls/junos.mplsvpn.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/mpls/junos.mplsvpn.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/mpls/sros.ldp.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/mpls/sros.ldp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/mpls/vyos.mplsvpn.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/mpls/vyos.mplsvpn.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/ospf/cumulus.ospfv2.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/ospf/cumulus.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/ospf/cumulus.ospfv3.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/ospf/cumulus.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/ospf/cumulus_nvue.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/ospf/cumulus_nvue.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/ospf/dellos10.ospfv2.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/ospf/dellos10.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/ospf/dellos10.ospfv3.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/ospf/dellos10.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/ospf/eos.ospfv2.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/ospf/eos.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/ospf/eos.ospfv3.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/ospf/eos.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/ospf/frr.ospfv2.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/ospf/frr.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/ospf/frr.ospfv3.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/ospf/frr.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/ospf/ios.ospfv2.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/ospf/ios.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/ospf/ios.ospfv3.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/ospf/ios.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/ospf/iosxr.ospfv2.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/ospf/iosxr.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/ospf/iosxr.ospfv3.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/ospf/iosxr.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/ospf/junos.ospfv2.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/ospf/junos.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/ospf/junos.ospfv3.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/ospf/junos.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/ospf/nxos.ospfv2.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/ospf/nxos.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/ospf/nxos.ospfv3.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/ospf/nxos.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/ospf/routeros.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/ospf/routeros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/ospf/routeros7.ospf-include.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/ospf/routeros7.ospf-include.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/ospf/srlinux.cli.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/ospf/srlinux.cli.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/ospf/srlinux.macro.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/ospf/srlinux.macro.j2`

 * *Files 8% similar despite different names*

```diff
@@ -28,15 +28,17 @@
 {%      set if_index = if_name_index[1] if if_name_index|length > 1 else l.ifindex if l.type=='stub' else '0' %}
 {%      if 'ospf' not in l %}
        # OSPF not configured on external interface {{ if_name }}
 {%      else %}
        - area-id: {{ l.ospf.area }}
          interface:
          - interface-name: {{ if_name }}.{{ if_index }}
-           passive: {{ ospf.passive | default(False) }}
+{%         if l.ospf.passive | default(False) %}
+           passive: True
+{%         endif %}
 {%         if l.ospf.network_type|default("") in ["broadcast","point-to-point"] %}
            interface-type: "{{ l.ospf.network_type }}"
 {%         endif %}
            failure-detection:
             enable-bfd: {{ l.ospf.bfd|default(False) }}
 {%         if l.ospf.cost is defined %}
            metric: {{ l.ospf.cost }}
```

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/ospf/sros.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/ospf/sros.j2`

 * *Files 9% similar despite different names*

```diff
@@ -1,44 +1,46 @@
 {% from "templates/initial/sros.j2" import if_name, declare_router with context %}
-{% set pid = ospf.process|default(0) %}
 
-{% macro ospf_config(af) %}
+{% macro ospf_config(af,ospf,vrf_interfaces,include_system) %}
+{% set pid = ospf.process|default(0) %}
 {% set ospfv = 'ospf3' if af=='ipv6' else 'ospf' %}
 
 {% macro ospf_interface(l) %}
 {{ declare_router(l,sub_path="/"+ospfv+"[ospf-instance="+pid|string + "]") }}
   val:
 {% if ospf.reference_bandwidth is defined %}
    reference-bandwidth: {{ ospf.reference_bandwidth * 1000 }} # in kbps
 {% endif %}
    admin-state: enable
    area:
    - area-id: "{{ l.ospf.area }}"
      interface:
      - interface-name: "{{ if_name(l.ifname) }}"
-       passive: {{ l.ospf.passive }}
+{% if l.ospf.passive|default(False) %}
+       passive: True
+{% endif %}
 {%  if l.ospf.bfd|default(False) %}
        bfd-liveness: { }
 {%  endif %}
        # mtu: 1500 # SRL defaults to 1500, now supporting global mtu settings
 {# TODO: Add support for multi-area adjacencies and 'secondary' interface-type #}
 {%  if l.ospf.network_type|default("") in ["broadcast","non-broadcast","point-to-point"] %}
        interface-type: "{{ l.ospf.network_type }}"
 {%  endif %}
 {%  if l.ospf.cost is defined %}
        metric: {{ l.ospf.cost }}
 {%  endif %}
 {% endmacro %}
 
 {% set system_if = { 'ifname': "system", 'ospf': { 'passive': True, 'area': ospf.area }, af: True } %}
-{% for l in interfaces|default([])+([system_if] if af in loopback else []) if 'ospf' in l and af in l %}
+{% for l in vrf_interfaces+([system_if] if include_system else []) if 'ospf' in l and af in l %}
 {{ ospf_interface(l)}}
 {% endfor %}
 {% endmacro %}
 
 updates:
-{% if ospf.af.ipv4 is defined %}
-{{ ospf_config('ipv4') }}
+{% if ospf.af.ipv4|default(False) %}
+{{ ospf_config('ipv4',ospf,interfaces,'ipv4' in loopback) }}
 {% endif %}
-{% if ospf.af.ipv6 is defined %}
-{{ ospf_config('ipv6') }}
+{% if ospf.af.ipv6|default(False) %}
+{{ ospf_config('ipv6',ospf,interfaces,'ipv6' in loopback) }}
 {% endif %}
```

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/ospf/sros.md-cli.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/ospf/sros.md-cli.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/ospf/sros.openconfig.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/ospf/sros.openconfig.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/ospf/vyos.ospfv2.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/ospf/vyos.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/ospf/vyos.ospfv3.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/ospf/vyos.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/sr/junos.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/sr/junos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/sr/srlinux.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/sr/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/sr/sros.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/sr/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/sr/sros.openconfig.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/sr/sros.openconfig.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/srv6/sros.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/srv6/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/vlan/csr.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vlan/csr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/vlan/cumulus.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vlan/cumulus.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/vlan/dellos10.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vlan/dellos10.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/vlan/eos.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vlan/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/vlan/frr.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vlan/frr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/vlan/nxos.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vlan/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/vlan/routeros7.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vlan/routeros7.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/vlan/srlinux.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vlan/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/vlan/sros.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vlan/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/vlan/vmx.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vlan/vmx.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/vlan/vyos.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vlan/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/vrf/dellos10.bgp-macro.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vrf/dellos10.bgp-macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/vrf/dellos10.bgp.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vrf/dellos10.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/vrf/dellos10.ospfv2-vrf.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vrf/dellos10.ospfv2-vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/vrf/eos.bgp-macro.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vrf/eos.bgp-macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/vrf/eos.bgp.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vrf/eos.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/vrf/eos.ospfv2-vrf.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vrf/eos.ospfv2-vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/vrf/frr.bgp.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vrf/frr.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/vrf/frr.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vrf/frr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/vrf/frr.ospfv2-vrf.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vrf/frr.ospfv2-vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/vrf/ios.bgp-macro.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vrf/ios.bgp-macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/vrf/ios.bgp.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vrf/ios.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/vrf/ios.ospfv2-vrf.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vrf/ios.ospfv2-vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/vrf/junos.bgp.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vrf/junos.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/vrf/junos.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vrf/junos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/vrf/junos.ospfv2-vrf.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vrf/junos.ospfv2-vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/vrf/nxos.bgp.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vrf/nxos.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/vrf/nxos.ospfv2-vrf.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vrf/nxos.ospfv2-vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/vrf/routeros.bgp-macro.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vrf/routeros.bgp-macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/vrf/routeros.bgp.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vrf/routeros.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/vrf/routeros.ospfv2-vrf.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vrf/routeros.ospfv2-vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/vrf/routeros7.bgp-macro.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vrf/routeros7.bgp-macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/vrf/routeros7.bgp.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vrf/routeros7.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/vrf/routeros7.ospf-include.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vrf/routeros7.ospf-include.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/vrf/srlinux.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vrf/srlinux.j2`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,19 @@
 {% for vname,vdata in vrfs.items() %}
 
 - path: network-instance[name={{vname}}]
   val:
    type: ip-vrf
 
 {% if 'ospf' in vdata %}
-{{ ospf_config(0,'ipv4' if vdata.af.ipv4|default(0) else 'ipv6',vname,vdata.ospf,vdata.ospf.interfaces)}}
+{%  for af in ['ipv4','ipv6'] %}
+{%   if af in vdata.af and vdata.af[af] %}
+{{ ospf_config(0,af,vname,vdata.ospf,vdata.ospf.interfaces)}}
+{%   endif %}
+{%  endfor %}
 {% endif %}
 
 {# Create an AS path set for this VRF, if vrf.as is set #}
 {% if vdata.as is defined %}
 - path: routing-policy/as-path-set[name={{vname}}]
   val:
    expression: "{{ vdata.as }}"
```

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/vrf/vyos.bgp-macro.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vrf/vyos.bgp-macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/vrf/vyos.bgp.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vrf/vyos.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/vrf/vyos.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vrf/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/vrf/vyos.ospfv2-vrf.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vrf/vyos.ospfv2-vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/vxlan/csr.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vxlan/csr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/vxlan/cumulus.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vxlan/cumulus.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/vxlan/frr.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vxlan/frr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/vxlan/nxos.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vxlan/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/vxlan/srlinux.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vxlan/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/vxlan/sros.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vxlan/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/ansible/templates/vxlan/vyos.j2` & `networklab-1.5.2.dev1/netsim/ansible/templates/vxlan/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/api.py` & `networklab-1.5.2.dev1/netsim/api.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/augment/config.py` & `networklab-1.5.2.dev1/netsim/augment/config.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/augment/devices.py` & `networklab-1.5.2.dev1/netsim/augment/devices.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/augment/groups.py` & `networklab-1.5.2.dev1/netsim/augment/groups.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 from box import Box
 
 from .. import common
 from .. import data
 from .. import modules
 from ..modules import bgp
+from ..data import get_box
 from ..data.validate import validate_attributes
 from ..data.types import must_be_dict,must_be_list,must_be_string,must_be_id
 from . import nodes
 
 '''
 Return members of the specified group. Recurse through child groups if needed
 '''
@@ -236,14 +237,15 @@
         if common.debug_active('groups'):
           print(f'... adding module {gdata.module} to {name}. Node modules now {ndata.module}')
 
 '''
 Copy node data from group into group members
 '''
 def copy_group_node_data(topology: Box,pfx: str) -> None:
+  topo_modules = topology.get('module',[])                            # Get list of default list of modules
   for grp in reverse_topsort(topology):
     if not grp.startswith(pfx):                                       # Skip groups that don't match the current prefix (ex: BGP autogroups)
       continue
     gdata = topology.groups[grp]
     if not 'node_data' in gdata:                                      # No group data, skip
       continue
 
@@ -252,15 +254,21 @@
       print(f'copy node data {grp}: {gdata.node_data}')
     for name in g_members:                                            # Iterate over group members
       if not name in topology.nodes:                                  # Member is not a node, skip it
         continue
 
       if common.debug_active('groups'):
         print(f'... merging node data with {name}')
-      topology.nodes[name] = gdata.node_data + topology.nodes[name]
+      merge_data=Box(gdata.node_data)
+      if 'module' in topology.nodes[name]:
+        for m in topo_modules:
+          if not m in topology.nodes[name].module:
+            merge_data.pop(m,None)
+
+      topology.nodes[name] = merge_data + topology.nodes[name]
 
 '''
 Export node_data from groups to topology
 
 Used to create module-specific data structures in pre_transform hook before the
 node data is populated from groups.node_data
```

### Comparing `networklab-1.5.1.dev1/netsim/augment/links.py` & `networklab-1.5.2.dev1/netsim/augment/links.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,15 +90,19 @@
     link_data = data.get_box({ '_linkname' : linkname })              # ... create stub link data structure
     link_data.interfaces = adjust_interface_list(l,link_data,nodes)   # ... and adjust interface list
     return link_data
 
   if isinstance(l,str):                                       # String, split into a list of nodes
     link_intf = []
     for n in l.split('-'):                # ... split it into a list of nodes
-      if n in nodes:                      # If the node name is valid
+      valid_node = n in nodes
+      if not valid_node:
+        valid_node = len([ x for x in nodes if n.startswith(x) ]) > 0
+
+      if valid_node:                      # If the node name is valid
         link_intf.append({ 'node': n })   # ... append it to the list of interfaces
       else:
         common.error(
           f'Link string {l} in {linkname} refers to an unknown node {n}',
           common.IncorrectValue,
           'links')
     return data.get_box({
```

### Comparing `networklab-1.5.1.dev1/netsim/augment/main.py` & `networklab-1.5.2.dev1/netsim/augment/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,16 @@
   global_vars.init(topology)
   augment.config.attributes(topology)
   augment.topology.check_required_elements(topology)
   topology.nodes = augment.nodes.create_node_dict(topology.nodes)
   if 'links' in topology:
     augment.links.links_init(topology)
 
+  augment.components.expand_components(topology)
+
   augment.devices.augment_device_settings(topology)
   augment.plugin.init(topology)                                         # Initialize plugins very early on in case they modify extra attributes
   augment.plugin.execute('init',topology)
   common.exit_on_error()
 
   augment.topology.extend_attribute_list(topology.defaults)             # Attributes have to be extended before group init
   augment.topology.extend_module_attribute_list(topology)               # ... or we won't recognize node attributes in groups
```

### Comparing `networklab-1.5.1.dev1/netsim/augment/nodes.py` & `networklab-1.5.2.dev1/netsim/augment/nodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 from .. import addressing
 from .. import providers
 from . import devices
 from ..data.validate import validate_attributes
 from ..data.types import must_be_int,must_be_string,must_be_id
 from ..modules._dataplane import extend_id_set,is_id_used,set_id_counter,get_next_id
 
+MAX_NODE_ID: typing.Final[int] = 250
+
 """
 Reserve a node ID, for example for gateway ID, return True if successful, False if duplicate
 """
 def reserve_id(n_id: int) -> bool:
   if is_id_used('node_id',n_id):
     return False
 
@@ -223,14 +225,18 @@
 Validate provider setting used in a node
 """
 
 def validate_node_provider(n: Box, topology: Box) -> bool:
   if not 'provider' in n:
     return True
 
+  if n.provider == topology.get('provider',None):
+    n.pop('provider',None)
+    return True
+
   if not n.provider in topology.defaults.providers:
     common.error(
       f'Invalid provider {n.provider} specified in node {n.name}',
       common.IncorrectValue,
       'nodes')
     return False
 
@@ -309,24 +315,24 @@
 * set node ID
 * set loopback address(es)
 * copy device data from defaults
 * set management IP and MAC addresses
 '''
 def transform(topology: Box, defaults: Box, pools: Box) -> None:
   for name,n in topology.nodes.items():
-    if not must_be_int(n,'id',f'nodes.{name}',module='nodes',min_value=1,max_value=250):
+    if not must_be_int(n,'id',f'nodes.{name}',module='nodes',min_value=1,max_value=MAX_NODE_ID):
       continue
     if not reserve_id(n.id):
       common.error(
         f'Duplicate static node ID {n.id} on node {n.name}',
         common.IncorrectValue,
         'nodes')
 
   common.exit_on_error()
-  set_id_counter('node_id',1,250)
+  set_id_counter('node_id',1,MAX_NODE_ID)
   for name,n in topology.nodes.items():
     if not 'id' in n:
       n.id = get_next_id('node_id')
 
     if not n.name: # pragma: no cover (name should have been checked way before)
       common.fatal(f"Internal error: node does not have a name {n}",'nodes')
       return
```

### Comparing `networklab-1.5.1.dev1/netsim/augment/plugin.py` & `networklab-1.5.2.dev1/netsim/augment/plugin.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import sys
 import typing
 import importlib
 import importlib.util
 
 from box import Box
 from .. import common
+from ..utils.templates import get_moddir
 from .. import data
 
 def load_plugin_from_path(path: str, plugin: str) -> typing.Optional[object]:
   module_path = path+'/'+plugin
   if not os.path.exists(module_path):
     if os.path.exists(module_path+'.py'):
       module_path = module_path+'.py'
@@ -58,15 +59,15 @@
 
   if not 'plugin' in topology:
     return
 
   topology.Plugin = []
   for pname in topology.plugin:
     plugin = None
-    search_path = ('.',common.netsim_package_path+'/extra')
+    search_path = ('.',str(get_moddir() / 'extra'))
     for path in search_path:
       if not plugin:
         plugin = load_plugin_from_path(path,pname)
     if plugin:
       topology.Plugin.append(plugin)
     else:
       common.error(f"Cannot find plugin {pname} in {search_path}",common.IncorrectValue,'plugin')
```

### Comparing `networklab-1.5.1.dev1/netsim/augment/topology.py` & `networklab-1.5.2.dev1/netsim/augment/topology.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/callback.py` & `networklab-1.5.2.dev1/netsim/callback.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/cli/__init__.py` & `networklab-1.5.2.dev1/netsim/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/cli/ansible.py` & `networklab-1.5.2.dev1/netsim/cli/ansible.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/cli/clab.py` & `networklab-1.5.2.dev1/netsim/cli/clab.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/cli/collect.py` & `networklab-1.5.2.dev1/netsim/cli/collect.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/cli/config.py` & `networklab-1.5.2.dev1/netsim/cli/config.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/cli/connect.py` & `networklab-1.5.2.dev1/netsim/cli/connect.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/cli/create.py` & `networklab-1.5.2.dev1/netsim/cli/create.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/cli/down.py` & `networklab-1.5.2.dev1/netsim/cli/down.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,26 +8,24 @@
 import argparse
 import typing
 import textwrap
 import os
 import sys
 from box import Box
 
-from . import topology_parse_args, load_snapshot_or_topology, external_commands,fs_cleanup
-from . import lab_status_change, lab_status_update,get_lab_id
-from .. import read_topology,augment,common
-from .. import providers
+from . import external_commands
+from . import lab_status_change,get_lab_id,fs_cleanup
+from .. import read_topology,common,providers
 from ..utils import status,strings
 from .up import provider_probes
 #
 # CLI parser for 'netlab down' command
 #
 def down_parse(args: typing.List[str]) -> argparse.Namespace:
   parser = argparse.ArgumentParser(
-    parents=[ topology_parse_args() ],
     prog="netlab down",
     description='Destroy the virtual lab')
 
   parser.add_argument(
     '-v','--verbose',
     dest='verbose',
     action='count',
@@ -35,23 +33,26 @@
     help='Verbose logging (where applicable)')
   parser.add_argument(
     '--cleanup',
     dest='cleanup',
     action='store_true',
     help='Remove all configuration files created by netlab create')
   parser.add_argument(
+    '--force',
+    dest='force',
+    action='store_true',
+    help='Force shutdown or cleanup (use at your own risk)')
+  parser.add_argument(
     '--snapshot',
     dest='snapshot',
     action='store',
     nargs='?',
+    default='netlab.snapshot.yml',
     const='netlab.snapshot.yml',
     help='Transformed topology snapshot file')
-  parser.add_argument(
-    dest='topology', action='store', nargs='?',
-    help='Topology file (default: topology.yml)')
 
   return parser.parse_args(args)
 
 def down_cleanup(topology: Box, verbose: bool = False) -> None:
   p_provider = topology.provider
   cleanup_list = topology.defaults.providers[p_provider].cleanup or []
 
@@ -109,46 +110,53 @@
 
   status.change_status(
     topology,
     callback = lambda s,t: s.pop(lab_id,None))
 
 def run(cli_args: typing.List[str]) -> None:
   args = down_parse(cli_args)
-  topology = load_snapshot_or_topology(args)
-
-  if args.topology:
-    print(f"Reading lab topology from {args.topology}")
-  else:
-    if not os.path.isfile(args.snapshot):
-      print(f"The topology snapshot file {args.snapshot} does not exist.\n"+
-            "Looks like no lab was started from this directory")
-      sys.exit(1)
-
-    print(f"Reading transformed lab topology from snapshot file {args.snapshot}")
+  if not os.path.isfile(args.snapshot):
+    print(f"The topology snapshot file {args.snapshot} does not exist.\n"+
+          "Looks like no lab was started from this directory")
+    sys.exit(1)
 
+  print(f"Reading transformed lab topology from snapshot file {args.snapshot}")
+  topology = read_topology.read_yaml(filename=args.snapshot)
   if topology is None:
     common.fatal('... could not read the lab topology, aborting')
     return
 
   mismatch = lab_dir_mismatch(topology)
 
   lab_status_change(topology,f'lab shutdown requested{" in conflicting directory" if mismatch else ""}')
-  provider_probes(topology)
+  try:
+    provider_probes(topology)
+  except:
+    if not args.force:
+      return
 
   p_provider = topology.provider
   p_module = providers._Provider.load(p_provider,topology.defaults.providers[p_provider])
   providers.mark_providers(topology)
   p_module.call('pre_output_transform',topology)
 
   for s_provider in topology[p_provider].providers:
     lab_status_change(topology,f'stopping {s_provider} provider')
-    stop_provider_lab(topology,p_provider,s_provider)
+    try:
+      stop_provider_lab(topology,p_provider,s_provider)
+    except:
+      if not args.force:
+        return
     print()
 
-  stop_provider_lab(topology,p_provider)
+  try:
+    stop_provider_lab(topology,p_provider)
+  except:
+    if not args.force:
+      return
 
   if args.cleanup:
     external_commands.print_step(3,"Cleanup configuration files",spacing = True)
     down_cleanup(topology,True)
 
   if not mismatch:
     remove_lab_status(topology)
```

### Comparing `networklab-1.5.1.dev1/netsim/cli/external_commands.py` & `networklab-1.5.2.dev1/netsim/cli/external_commands.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/cli/initial.py` & `networklab-1.5.2.dev1/netsim/cli/initial.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/cli/install.py` & `networklab-1.5.2.dev1/netsim/cli/install.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/cli/libvirt.py` & `networklab-1.5.2.dev1/netsim/cli/libvirt.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/cli/read.py` & `networklab-1.5.2.dev1/netsim/cli/read.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/cli/restart.py` & `networklab-1.5.2.dev1/netsim/cli/restart.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/cli/show.py` & `networklab-1.5.2.dev1/netsim/cli/show.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/cli/status.py` & `networklab-1.5.2.dev1/netsim/cli/status.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/cli/test.py` & `networklab-1.5.2.dev1/netsim/cli/test.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/cli/up.py` & `networklab-1.5.2.dev1/netsim/cli/up.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/cli/usage.txt` & `networklab-1.5.2.dev1/netsim/cli/usage.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/data/__init__.py` & `networklab-1.5.2.dev1/netsim/data/__init__.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/data/global_vars.py` & `networklab-1.5.2.dev1/netsim/data/global_vars.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/data/types.py` & `networklab-1.5.2.dev1/netsim/data/types.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/data/validate.py` & `networklab-1.5.2.dev1/netsim/data/validate.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/defaults/attributes.yml` & `networklab-1.5.2.dev1/netsim/defaults/attributes.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/devices/__init__.py` & `networklab-1.5.2.dev1/netsim/devices/__init__.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/devices/asav.py` & `networklab-1.5.2.dev1/netsim/devices/asav.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/devices/asav.yml` & `networklab-1.5.2.dev1/netsim/devices/asav.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/devices/csr.yml` & `networklab-1.5.2.dev1/netsim/devices/csr.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/devices/cumulus.yml` & `networklab-1.5.2.dev1/netsim/devices/cumulus.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/devices/cumulus_nvue.yml` & `networklab-1.5.2.dev1/netsim/devices/cumulus_nvue.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/devices/dellos10.yml` & `networklab-1.5.2.dev1/netsim/devices/dellos10.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/devices/eos.py` & `networklab-1.5.2.dev1/netsim/devices/eos.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/devices/eos.yml` & `networklab-1.5.2.dev1/netsim/devices/eos.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/devices/frr.yml` & `networklab-1.5.2.dev1/netsim/devices/frr.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/devices/iosv.py` & `networklab-1.5.2.dev1/netsim/devices/iosv.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/devices/iosv.yml` & `networklab-1.5.2.dev1/netsim/devices/iosv.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/devices/iosxr.yml` & `networklab-1.5.2.dev1/netsim/devices/iosxr.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/devices/junos.py` & `networklab-1.5.2.dev1/netsim/devices/junos.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/devices/linux.yml` & `networklab-1.5.2.dev1/netsim/devices/linux.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/devices/none.yml` & `networklab-1.5.2.dev1/netsim/devices/none.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/devices/nxos.yml` & `networklab-1.5.2.dev1/netsim/devices/nxos.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/devices/routeros7.yml` & `networklab-1.5.2.dev1/netsim/devices/routeros7.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/devices/srlinux.yml` & `networklab-1.5.2.dev1/netsim/devices/srlinux.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/devices/sros.yml` & `networklab-1.5.2.dev1/netsim/devices/sros.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/devices/vmx.py` & `networklab-1.5.2.dev1/netsim/devices/vmx.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/devices/vmx.yml` & `networklab-1.5.2.dev1/netsim/devices/vmx.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/devices/vsrx.py` & `networklab-1.5.2.dev1/netsim/devices/vsrx.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/devices/vsrx.yml` & `networklab-1.5.2.dev1/netsim/devices/vsrx.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/devices/vyos.yml` & `networklab-1.5.2.dev1/netsim/devices/vyos.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/extra/__pycache__/ebgp-local_as.cpython-39.pyc` & `networklab-1.5.2.dev1/netsim/extra/__pycache__/ebgp-local_as.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/extra/ebgp.utils/__pycache__/plugin.cpython-310.pyc` & `networklab-1.5.2.dev1/netsim/extra/ebgp.utils/__pycache__/plugin.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/extra/ebgp.utils/default-originate.yml` & `networklab-1.5.2.dev1/netsim/extra/ebgp.utils/default-originate.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/extra/ebgp.utils/eos.j2` & `networklab-1.5.2.dev1/netsim/extra/ebgp.utils/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/extra/ebgp.utils/ios.j2` & `networklab-1.5.2.dev1/netsim/extra/ebgp.utils/ios.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/extra/ebgp.utils/junos.j2` & `networklab-1.5.2.dev1/netsim/extra/ebgp.utils/junos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/extra/ebgp.utils/plugin.py` & `networklab-1.5.2.dev1/netsim/extra/ebgp.utils/plugin.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/extra/ebgp.utils/routeros7.j2` & `networklab-1.5.2.dev1/netsim/extra/ebgp.utils/routeros7.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/extra/ebgp.utils/srlinux.j2` & `networklab-1.5.2.dev1/netsim/extra/ebgp.utils/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/extra/ebgp.utils/vyos.j2` & `networklab-1.5.2.dev1/netsim/extra/ebgp.utils/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/extra/multilab/__pycache__/plugin.cpython-310.pyc` & `networklab-1.5.2.dev1/netsim/extra/multilab/__pycache__/plugin.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/extra/multilab/plugin.py` & `networklab-1.5.2.dev1/netsim/extra/multilab/plugin.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/extra/proxy-arp/__pycache__/plugin.cpython-310.pyc` & `networklab-1.5.2.dev1/netsim/extra/proxy-arp/__pycache__/plugin.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/extra/proxy-arp/__pycache__/plugin.cpython-39.pyc` & `networklab-1.5.2.dev1/netsim/extra/proxy-arp/__pycache__/plugin.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/extra/proxy-arp/plugin.py` & `networklab-1.5.2.dev1/netsim/extra/proxy-arp/plugin.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/extra/proxy-arp/srlinux.j2` & `networklab-1.5.2.dev1/netsim/extra/proxy-arp/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/extra/proxy-arp/sros.j2` & `networklab-1.5.2.dev1/netsim/extra/proxy-arp/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/install/ansible.sh` & `networklab-1.5.2.dev1/netsim/install/ansible.sh`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/install/containerlab.sh` & `networklab-1.5.2.dev1/netsim/install/containerlab.sh`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/install/grpc.sh` & `networklab-1.5.2.dev1/netsim/install/grpc.sh`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/install/libvirt/asav/day0-config` & `networklab-1.5.2.dev1/netsim/install/libvirt/asav/day0-config`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/install/libvirt/csr.txt` & `networklab-1.5.2.dev1/netsim/install/libvirt/csr.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/install/libvirt/dellos10.txt` & `networklab-1.5.2.dev1/netsim/install/libvirt/dellos10.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/install/libvirt/eos.txt` & `networklab-1.5.2.dev1/netsim/install/libvirt/eos.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/install/libvirt/eos.xml.j2` & `networklab-1.5.2.dev1/netsim/install/libvirt/eos.xml.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/install/libvirt/iosv.txt` & `networklab-1.5.2.dev1/netsim/install/libvirt/iosv.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/install/libvirt/iosv.xml.j2` & `networklab-1.5.2.dev1/netsim/install/libvirt/iosv.xml.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/install/libvirt/iosxr.txt` & `networklab-1.5.2.dev1/netsim/install/libvirt/iosxr.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/install/libvirt/nxos.txt` & `networklab-1.5.2.dev1/netsim/install/libvirt/nxos.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/install/libvirt/nxos.xml.j2` & `networklab-1.5.2.dev1/netsim/install/libvirt/nxos.xml.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/install/libvirt/routeros7.txt` & `networklab-1.5.2.dev1/netsim/install/libvirt/routeros7.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/install/libvirt/vsrx/juniper.conf` & `networklab-1.5.2.dev1/netsim/install/libvirt/vsrx/juniper.conf`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/install/libvirt/vsrx.txt` & `networklab-1.5.2.dev1/netsim/install/libvirt/vsrx.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/install/libvirt.sh` & `networklab-1.5.2.dev1/netsim/install/libvirt.sh`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/install/ubuntu.sh` & `networklab-1.5.2.dev1/netsim/install/ubuntu.sh`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/modules/__init__.py` & `networklab-1.5.2.dev1/netsim/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/modules/_dataplane.py` & `networklab-1.5.2.dev1/netsim/modules/_dataplane.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/modules/_routing.py` & `networklab-1.5.2.dev1/netsim/modules/_routing.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/modules/bfd.py` & `networklab-1.5.2.dev1/netsim/modules/bfd.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/modules/bfd.yml` & `networklab-1.5.2.dev1/netsim/modules/bfd.yml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # BFD (RFC 5880) default settings and attributes
 #
-supported_on: [ srlinux, sros, iosv, csr, nxos, eos, vyos, none ]
+supported_on: [ srlinux, sros, iosv, csr, nxos, eos, vyos, arubacx, none ]
 min_echo_rx: 0      # Echo function, 0=disabled by default
 multiplier: 3       # Detection time multiplier, number of packets lost before down
 attributes:
   global:
     min_tx: { type: int, min_value: 1 }
     min_rx: { type: int, min_value: 1 }
     min_echo_rx: { type: int, min_value: 0 }
```

### Comparing `networklab-1.5.1.dev1/netsim/modules/bgp.py` & `networklab-1.5.2.dev1/netsim/modules/bgp.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/modules/bgp.yml` & `networklab-1.5.2.dev1/netsim/modules/bgp.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # BGP default settings and attributes
 #
 supported_on: [ cumulus, cumulus_nvue, eos, frr, csr, iosv, nxos, asav, vsrx, vyos, routeros,
-  srlinux, sros, none, dellos10, routeros7, vmx, iosxr, none ]
+  srlinux, sros, none, dellos10, routeros7, vmx, iosxr, arubacx, none ]
 ebgp_role: external
 advertise_roles: [ stub ]
 advertise_loopback: True
 community:
   ibgp: [ standard, extended ]
   ebgp: [ standard ]
 no_propagate: [ ebgp_role, advertise_roles, rr_list, as_list ]
```

### Comparing `networklab-1.5.1.dev1/netsim/modules/evpn.py` & `networklab-1.5.2.dev1/netsim/modules/evpn.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/modules/evpn.yml` & `networklab-1.5.2.dev1/netsim/modules/evpn.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # EVPN default settings and attributes
 requires: [ bgp ]
-supported_on: [ sros, srlinux, frr, eos, vyos, dellos10, cumulus, nxos, none ]
+supported_on: [ sros, srlinux, frr, eos, vyos, dellos10, cumulus, nxos, arubacx, none ]
 no_propagate: [ start_transit_vni, transport, vlan_bundle_service, as ]
 transform_after: [ vlan, vxlan, vrf ]
 config_after: [ vlan, vxlan, vrf ]
 session: [ ibgp ]
 start_transit_vni: 200000
 attributes:
   global:
```

### Comparing `networklab-1.5.1.dev1/netsim/modules/gateway.py` & `networklab-1.5.2.dev1/netsim/modules/gateway.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/modules/gateway.yml` & `networklab-1.5.2.dev1/netsim/modules/gateway.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Gateway (FHRP) default settings and attributes
 #
-supported_on: [ none, eos, cumulus, iosv, csr, nxos, sros, srlinux, vyos, dellos10 ]
+supported_on: [ none, eos, cumulus, iosv, csr, nxos, sros, srlinux, vyos, dellos10, arubacx ]
 transform_after: [ vlan, vrf, ospf, isis, eigrp ]
 config_after: [ vlan,vrf ]
 id: -2
 protocol: anycast
 anycast:
   mac: 0200.cafe.00ff
   unicast: True
```

### Comparing `networklab-1.5.1.dev1/netsim/modules/isis.py` & `networklab-1.5.2.dev1/netsim/modules/isis.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/modules/isis.yml` & `networklab-1.5.2.dev1/netsim/modules/isis.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/modules/mpls.py` & `networklab-1.5.2.dev1/netsim/modules/mpls.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/modules/mpls.yml` & `networklab-1.5.2.dev1/netsim/modules/mpls.yml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MPLS (LDP, BGP LU, L3VPN, 6PE) default settings and attributes
 #
-supported_on: [ eos, iosv, csr, routeros, vyos, routeros7, sros, vmx, vsrx, frr, none ]
+supported_on: [ eos, iosv, csr, routeros, vyos, routeros7, sros, vmx, vsrx, frr, none, arubacx ]
 config_after: [ vlan, ospf, isis, bgp ]
 transform_after: [ vlan, bgp ]
 ldp: True
 attributes:
   global:
     ldp:
       _alt_types: [ bool ]
```

### Comparing `networklab-1.5.1.dev1/netsim/modules/ospf.py` & `networklab-1.5.2.dev1/netsim/modules/ospf.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/modules/ospf.yml` & `networklab-1.5.2.dev1/netsim/modules/ospf.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # OSPFv2/OSPFv3 default settings and attributes
 #
 area: 0.0.0.0
 supported_on: [
   arcos, cumulus, cumulus_nvue, eos, fortios, frr, csr, iosv, nxos, vsrx, vyos, routeros,
-  srlinux, sros, dellos10, routeros7, vmx, iosxr, none ]
+  srlinux, sros, dellos10, routeros7, vmx, iosxr, arubacx, none ]
 transform_after: [ vlan,vrf ]
 config_after: [ vlan ]
 attributes:
   global:
     af:
       _list_to_dict: True
       _alt_types: [ NoneType ]
```

### Comparing `networklab-1.5.1.dev1/netsim/modules/srv6.py` & `networklab-1.5.2.dev1/netsim/modules/srv6.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/modules/vlan.py` & `networklab-1.5.2.dev1/netsim/modules/vlan.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/modules/vlan.yml` & `networklab-1.5.2.dev1/netsim/modules/vlan.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # VLAN default settings and attributes
 #
-supported_on: [ eos, iosv, csr, vyos, dellos10, srlinux, none, routeros, nxos, frr, cumulus, sros, routeros7, vmx, vsrx, none ]
+supported_on: [ eos, iosv, csr, vyos, dellos10, srlinux, none, routeros, nxos, frr, cumulus, sros, routeros7, vmx, vsrx, arubacx, none ]
 no_propagate: [ start_vlan_id, mode ]
 start_vlan_id: 1000
 mode: irb
 attributes:
   global:
     mode: { type: str, valid_values: [ bridge, irb, route] }
   node:
```

### Comparing `networklab-1.5.1.dev1/netsim/modules/vrf.py` & `networklab-1.5.2.dev1/netsim/modules/vrf.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/modules/vxlan.py` & `networklab-1.5.2.dev1/netsim/modules/vxlan.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/modules/vxlan.yml` & `networklab-1.5.2.dev1/netsim/modules/vxlan.yml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # VXLAN default settings and attributes
 #
-supported_on: [ eos, nxos, vyos, csr, dellos10, srlinux, frr, cumulus, sros, none ]
+supported_on: [ eos, nxos, vyos, csr, dellos10, srlinux, frr, cumulus, sros, arubacx, none ]
 requires: [ vlan ]
 config_after: [ vrf ] # For platforms that suppport L3 VXLAN, vrfs must be created first
 transform_after: [ vlan, vrf ]
 domain: global
 flooding: static
 start_vni: 100000
 attributes:
```

### Comparing `networklab-1.5.1.dev1/netsim/outputs/__init__.py` & `networklab-1.5.2.dev1/netsim/outputs/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,16 +10,15 @@
 import os
 import typing
 import re
 
 # Related modules
 from box import Box
 
-from .. import common
-from ..utils import status
+from ..utils import status,log
 from ..callback import Callback
 
 '''
 check_writeable -- check if the current directory is writeable (does not have netlab.lock file)
 
 Print an error message explaining what to do next and exit with a fatal error if the directory is locked
 '''
@@ -32,15 +31,15 @@
 
 Please use 'netlab status' to check the status of labs running on this machine, or
 'netlab down' to shut down the other lab running in this directory.
 
 If you are sure that no other lab is running in this directory, you can remove
 the netlab.lock file manually and retry.
 ''')
-    common.fatal('Cannot create configuration files in a locked directory')
+    log.fatal('Cannot create configuration files in a locked directory')
 
 class _TopologyOutput(Callback):
   def __init__(self, output: str, data: Box) -> None:
     self.settings = data
 
     output_parts = output.split('=')
 
@@ -70,8 +69,8 @@
 
     if self.settings:
       return self.settings.filename
 
     return None
 
   def write(self, topology: Box) -> None:
-    common.fatal('someone called the "write" method of TopologyOutput abstract class')
+    log.fatal('someone called the "write" method of TopologyOutput abstract class')
```

### Comparing `networklab-1.5.1.dev1/netsim/outputs/ansible.py` & `networklab-1.5.2.dev1/netsim/outputs/ansible.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/outputs/common.py` & `networklab-1.5.2.dev1/netsim/outputs/common.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/outputs/d2.py` & `networklab-1.5.2.dev1/netsim/outputs/d2.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/outputs/devices.py` & `networklab-1.5.2.dev1/netsim/outputs/devices.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/outputs/format.py` & `networklab-1.5.2.dev1/netsim/outputs/format.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/outputs/graph.py` & `networklab-1.5.2.dev1/netsim/outputs/graph.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/outputs/graphite.py` & `networklab-1.5.2.dev1/netsim/outputs/graphite.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/outputs/provider.py` & `networklab-1.5.2.dev1/netsim/outputs/provider.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/outputs/yaml.py` & `networklab-1.5.2.dev1/netsim/outputs/yaml.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/providers/__init__.py` & `networklab-1.5.2.dev1/netsim/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/providers/clab.py` & `networklab-1.5.2.dev1/netsim/providers/clab.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/providers/clab.yml` & `networklab-1.5.2.dev1/netsim/providers/clab.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/providers/external.py` & `networklab-1.5.2.dev1/netsim/providers/external.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/providers/libvirt.py` & `networklab-1.5.2.dev1/netsim/providers/libvirt.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/read_topology.py` & `networklab-1.5.2.dev1/netsim/read_topology.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/templates/provider/clab/clab.j2` & `networklab-1.5.2.dev1/netsim/templates/provider/clab/clab.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/templates/provider/clab/frr/daemons.j2` & `networklab-1.5.2.dev1/netsim/templates/provider/clab/frr/daemons.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/templates/provider/clab/linux/hosts.j2` & `networklab-1.5.2.dev1/netsim/templates/provider/clab/linux/hosts.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/templates/provider/external/external.j2` & `networklab-1.5.2.dev1/netsim/templates/provider/external/external.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/templates/provider/libvirt/Vagrantfile.j2` & `networklab-1.5.2.dev1/netsim/templates/provider/libvirt/Vagrantfile.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/templates/provider/libvirt/cumulus_nvue-domain.j2` & `networklab-1.5.2.dev1/netsim/templates/provider/libvirt/cumulus_nvue-domain.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/templates/provider/libvirt/define-domain.j2` & `networklab-1.5.2.dev1/netsim/templates/provider/libvirt/define-domain.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/templates/provider/libvirt/iosxr-domain.j2` & `networklab-1.5.2.dev1/netsim/templates/provider/libvirt/iosxr-domain.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/templates/provider/libvirt/libvirt-tunnel.j2` & `networklab-1.5.2.dev1/netsim/templates/provider/libvirt/libvirt-tunnel.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/templates/provider/libvirt/nxos-domain.j2` & `networklab-1.5.2.dev1/netsim/templates/provider/libvirt/nxos-domain.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/templates/provider/libvirt/vagrant-libvirt.xml` & `networklab-1.5.2.dev1/netsim/templates/provider/libvirt/vagrant-libvirt.xml`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/templates/provider/libvirt/vsrx-domain.j2` & `networklab-1.5.2.dev1/netsim/templates/provider/libvirt/vsrx-domain.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/templates/provider/virtualbox/Vagrantfile.j2` & `networklab-1.5.2.dev1/netsim/templates/provider/virtualbox/Vagrantfile.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/utils/log.py` & `networklab-1.5.2.dev1/netsim/utils/log.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/utils/status.py` & `networklab-1.5.2.dev1/netsim/utils/status.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/netsim/utils/strings.py` & `networklab-1.5.2.dev1/netsim/utils/strings.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/networklab.egg-info/PKG-INFO` & `networklab-1.5.2.dev1/networklab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: networklab
-Version: 1.5.1.dev1
+Version: 1.5.2.dev1
 Summary: CLI-based Virtual Networking Lab Abstraction Layer
 Home-page: https://github.com/ipspace/netlab
 Author: Ivan Pepelnjak
 Author-email: ip@ipspace.net
 Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -30,15 +30,15 @@
 
 Instead of wasting time creating lab topology in a GUI and configuring boring details, you'll start with a lab preconfigured according to your specifications.
 
 Interested? [Read the documentation](https://netsim-tools.readthedocs.io/) and [installation guidelines](https://netsim-tools.readthedocs.io/en/latest/install.html).
 
 ## Releases
 
-The latest release is [release 1.5.0](https://github.com/ipspace/netlab/releases/tag/release_1.5.0). We redesigned topology validation in release 1.5.0, resulting in potentially breaking changes. If you're a long-time _netlab_ user, please read the [release notes](https://netsim-tools.readthedocs.io/en/latest/release.html) first.
+The latest release is [release 1.5.1](https://github.com/ipspace/netlab/releases/tag/release_1.5.1). We redesigned topology validation in release 1.5.0, resulting in potentially breaking changes. If you're a long-time _netlab_ user, please read the [release notes](https://netsim-tools.readthedocs.io/en/latest/release.html) first.
 
 The latest release before the changes made in release 1.5.0 is [release 1.4.3](https://github.com/ipspace/netlab/releases/tag/release_1.4.3).
 
 ## An overview of tools:
 
 **netlab up**
 : Uses **netlab create** to create configuration files, starts the virtual lab, and uses **netlab initial** to deploy device configurations. [More details](https://netsim-tools.readthedocs.io/en/latest/netlab/up.html)
```

### Comparing `networklab-1.5.1.dev1/networklab.egg-info/SOURCES.txt` & `networklab-1.5.2.dev1/networklab.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -16,23 +16,25 @@
 netsim/ansible/display-neighbors.ansible
 netsim/ansible/initial-config.ansible
 netsim/ansible/missing.yml
 netsim/ansible/tasks/create-config.yml
 netsim/ansible/tasks/deploy-custom-config.yml
 netsim/ansible/tasks/deploy-module.yml
 netsim/ansible/tasks/deploy-config/arcos.yml
+netsim/ansible/tasks/deploy-config/arubacx.yml
 netsim/ansible/tasks/deploy-config/asa.yml
 netsim/ansible/tasks/deploy-config/cumulus.yml
 netsim/ansible/tasks/deploy-config/cumulus_nvue.yml
 netsim/ansible/tasks/deploy-config/dellos10.yml
 netsim/ansible/tasks/deploy-config/eos.yml
 netsim/ansible/tasks/deploy-config/frr.yml
 netsim/ansible/tasks/deploy-config/ios.yml
 netsim/ansible/tasks/deploy-config/iosxr.yml
 netsim/ansible/tasks/deploy-config/junos.yml
+netsim/ansible/tasks/deploy-config/linux-clab.yml
 netsim/ansible/tasks/deploy-config/linux.yml
 netsim/ansible/tasks/deploy-config/none.yml
 netsim/ansible/tasks/deploy-config/nxos.yml
 netsim/ansible/tasks/deploy-config/routeros.yml
 netsim/ansible/tasks/deploy-config/routeros7.yml
 netsim/ansible/tasks/deploy-config/srlinux.yml
 netsim/ansible/tasks/deploy-config/sros.yml
@@ -59,21 +61,24 @@
 netsim/ansible/tasks/linux/initial-clab.yml
 netsim/ansible/tasks/nxos/initial.yml
 netsim/ansible/tasks/readiness-check/dellos10.yml
 netsim/ansible/tasks/readiness-check/eos-clab.yml
 netsim/ansible/tasks/readiness-check/routeros7.yml
 netsim/ansible/tasks/vmx/initial.yml
 netsim/ansible/templates/missing.j2
+netsim/ansible/templates/bfd/arubacx.j2
 netsim/ansible/templates/bfd/eos.j2
 netsim/ansible/templates/bfd/ios.j2
 netsim/ansible/templates/bfd/none.j2
 netsim/ansible/templates/bfd/nxos.j2
 netsim/ansible/templates/bfd/srlinux.j2
 netsim/ansible/templates/bfd/sros.j2
 netsim/ansible/templates/bfd/vyos.j2
+netsim/ansible/templates/bgp/arubacx.j2
+netsim/ansible/templates/bgp/arubacx.macro.j2
 netsim/ansible/templates/bgp/asa.j2
 netsim/ansible/templates/bgp/asa.macro.j2
 netsim/ansible/templates/bgp/cumulus.j2
 netsim/ansible/templates/bgp/cumulus_nvue.j2
 netsim/ansible/templates/bgp/dellos10.j2
 netsim/ansible/templates/bgp/dellos10.macro.j2
 netsim/ansible/templates/bgp/eos.j2
@@ -97,32 +102,37 @@
 netsim/ansible/templates/bgp/sros.j2
 netsim/ansible/templates/bgp/sros.md-cli.j2
 netsim/ansible/templates/bgp/sros.openconfig.j2
 netsim/ansible/templates/bgp/vyos.j2
 netsim/ansible/templates/bgp/vyos.macro.j2
 netsim/ansible/templates/eigrp/ios.j2
 netsim/ansible/templates/eigrp/nxos.j2
+netsim/ansible/templates/evpn/arubacx.j2
 netsim/ansible/templates/evpn/cumulus.j2
 netsim/ansible/templates/evpn/dellos10.j2
 netsim/ansible/templates/evpn/eos.j2
 netsim/ansible/templates/evpn/frr.evpn-config.j2
 netsim/ansible/templates/evpn/frr.j2
 netsim/ansible/templates/evpn/nxos.j2
 netsim/ansible/templates/evpn/srlinux.j2
 netsim/ansible/templates/evpn/sros.j2
 netsim/ansible/templates/evpn/vyos.j2
+netsim/ansible/templates/gateway/arubacx.j2
 netsim/ansible/templates/gateway/cumulus.j2
 netsim/ansible/templates/gateway/dellos10.j2
 netsim/ansible/templates/gateway/eos.j2
 netsim/ansible/templates/gateway/ios.j2
 netsim/ansible/templates/gateway/nxos.j2
 netsim/ansible/templates/gateway/srlinux.j2
 netsim/ansible/templates/gateway/sros.j2
 netsim/ansible/templates/gateway/vyos.j2
 netsim/ansible/templates/initial/arcos.j2
+netsim/ansible/templates/initial/arubacx.j2
+netsim/ansible/templates/initial/arubacx.vlan.j2
+netsim/ansible/templates/initial/arubacx.vrf.j2
 netsim/ansible/templates/initial/asa.j2
 netsim/ansible/templates/initial/csr.vlan.j2
 netsim/ansible/templates/initial/cumulus.j2
 netsim/ansible/templates/initial/cumulus_nvue.j2
 netsim/ansible/templates/initial/dellos10.j2
 netsim/ansible/templates/initial/dellos10.vrf.j2
 netsim/ansible/templates/initial/eos.j2
@@ -163,14 +173,17 @@
 netsim/ansible/templates/isis/iosxr.j2
 netsim/ansible/templates/isis/junos.j2
 netsim/ansible/templates/isis/nxos.j2
 netsim/ansible/templates/isis/srlinux.j2
 netsim/ansible/templates/isis/sros.j2
 netsim/ansible/templates/isis/sros.openconfig.j2
 netsim/ansible/templates/isis/vyos.j2
+netsim/ansible/templates/mpls/arubacx.j2
+netsim/ansible/templates/mpls/arubacx.ldp.j2
+netsim/ansible/templates/mpls/arubacx.mplsvpn.j2
 netsim/ansible/templates/mpls/eos.6pe.j2
 netsim/ansible/templates/mpls/eos.bgp-lu.j2
 netsim/ansible/templates/mpls/eos.j2
 netsim/ansible/templates/mpls/eos.ldp.j2
 netsim/ansible/templates/mpls/eos.mplsvpn.j2
 netsim/ansible/templates/mpls/frr.frr-config.j2
 netsim/ansible/templates/mpls/frr.j2
@@ -192,14 +205,17 @@
 netsim/ansible/templates/mpls/routeros7.mplsvpn.j2
 netsim/ansible/templates/mpls/sros.j2
 netsim/ansible/templates/mpls/sros.ldp.j2
 netsim/ansible/templates/mpls/vyos.j2
 netsim/ansible/templates/mpls/vyos.ldp.j2
 netsim/ansible/templates/mpls/vyos.mplsvpn.j2
 netsim/ansible/templates/ospf/arcos.j2
+netsim/ansible/templates/ospf/arubacx.j2
+netsim/ansible/templates/ospf/arubacx.ospfv2.j2
+netsim/ansible/templates/ospf/arubacx.ospfv3.j2
 netsim/ansible/templates/ospf/cumulus.j2
 netsim/ansible/templates/ospf/cumulus.ospfv2.j2
 netsim/ansible/templates/ospf/cumulus.ospfv3.j2
 netsim/ansible/templates/ospf/cumulus_nvue.j2
 netsim/ansible/templates/ospf/dellos10.j2
 netsim/ansible/templates/ospf/dellos10.ospfv2.j2
 netsim/ansible/templates/ospf/dellos10.ospfv3.j2
@@ -237,28 +253,33 @@
 netsim/ansible/templates/sr/eos.j2
 netsim/ansible/templates/sr/ios.j2
 netsim/ansible/templates/sr/junos.j2
 netsim/ansible/templates/sr/srlinux.j2
 netsim/ansible/templates/sr/sros.j2
 netsim/ansible/templates/sr/sros.openconfig.j2
 netsim/ansible/templates/srv6/sros.j2
+netsim/ansible/templates/vlan/arubacx.j2
 netsim/ansible/templates/vlan/csr.j2
 netsim/ansible/templates/vlan/cumulus.j2
 netsim/ansible/templates/vlan/dellos10.j2
 netsim/ansible/templates/vlan/eos.j2
 netsim/ansible/templates/vlan/frr.j2
 netsim/ansible/templates/vlan/ios.j2
 netsim/ansible/templates/vlan/nxos.j2
 netsim/ansible/templates/vlan/routeros.j2
 netsim/ansible/templates/vlan/routeros7.j2
 netsim/ansible/templates/vlan/srlinux.j2
 netsim/ansible/templates/vlan/sros.j2
 netsim/ansible/templates/vlan/vmx.j2
 netsim/ansible/templates/vlan/vsrx.j2
 netsim/ansible/templates/vlan/vyos.j2
+netsim/ansible/templates/vrf/arubacx.bgp-macro.j2
+netsim/ansible/templates/vrf/arubacx.bgp.j2
+netsim/ansible/templates/vrf/arubacx.j2
+netsim/ansible/templates/vrf/arubacx.ospfv2-vrf.j2
 netsim/ansible/templates/vrf/cumulus.j2
 netsim/ansible/templates/vrf/cumulus_nvue.j2
 netsim/ansible/templates/vrf/dellos10.bgp-macro.j2
 netsim/ansible/templates/vrf/dellos10.bgp.j2
 netsim/ansible/templates/vrf/dellos10.j2
 netsim/ansible/templates/vrf/dellos10.ospfv2-vrf.j2
 netsim/ansible/templates/vrf/eos.bgp-macro.j2
@@ -290,24 +311,26 @@
 netsim/ansible/templates/vrf/routeros7.ospfv2-vrf.j2
 netsim/ansible/templates/vrf/srlinux.j2
 netsim/ansible/templates/vrf/sros.j2
 netsim/ansible/templates/vrf/vyos.bgp-macro.j2
 netsim/ansible/templates/vrf/vyos.bgp.j2
 netsim/ansible/templates/vrf/vyos.j2
 netsim/ansible/templates/vrf/vyos.ospfv2-vrf.j2
+netsim/ansible/templates/vxlan/arubacx.j2
 netsim/ansible/templates/vxlan/csr.j2
 netsim/ansible/templates/vxlan/cumulus.j2
 netsim/ansible/templates/vxlan/dellos10.j2
 netsim/ansible/templates/vxlan/eos.j2
 netsim/ansible/templates/vxlan/frr.j2
 netsim/ansible/templates/vxlan/nxos.j2
 netsim/ansible/templates/vxlan/srlinux.j2
 netsim/ansible/templates/vxlan/sros.j2
 netsim/ansible/templates/vxlan/vyos.j2
 netsim/augment/__init__.py
+netsim/augment/components.py
 netsim/augment/config.py
 netsim/augment/devices.py
 netsim/augment/groups.py
 netsim/augment/links.py
 netsim/augment/main.py
 netsim/augment/nodes.py
 netsim/augment/plugin.py
@@ -342,14 +365,16 @@
 netsim/defaults/addressing.yml
 netsim/defaults/attributes.yml
 netsim/defaults/automation.yml
 netsim/defaults/hints.yml
 netsim/defaults/multilab.yml
 netsim/defaults/ports.yml
 netsim/devices/__init__.py
+netsim/devices/arubacx.py
+netsim/devices/arubacx.yml
 netsim/devices/asav.py
 netsim/devices/asav.yml
 netsim/devices/csr.yml
 netsim/devices/cumulus.yml
 netsim/devices/cumulus_nvue.yml
 netsim/devices/dellos10.yml
 netsim/devices/eos.py
@@ -392,14 +417,15 @@
 netsim/extra/proxy-arp/__pycache__/plugin.cpython-310.pyc
 netsim/extra/proxy-arp/__pycache__/plugin.cpython-39.pyc
 netsim/install/ansible.sh
 netsim/install/containerlab.sh
 netsim/install/grpc.sh
 netsim/install/libvirt.sh
 netsim/install/ubuntu.sh
+netsim/install/libvirt/arubacx.txt
 netsim/install/libvirt/asav.txt
 netsim/install/libvirt/csr.txt
 netsim/install/libvirt/dellos10.txt
 netsim/install/libvirt/eos.txt
 netsim/install/libvirt/eos.xml.j2
 netsim/install/libvirt/iosv.txt
 netsim/install/libvirt/iosv.xml.j2
@@ -466,14 +492,15 @@
 netsim/templates/ansible.cfg.j2
 netsim/templates/provider/clab/clab.j2
 netsim/templates/provider/clab/frr/daemons.j2
 netsim/templates/provider/clab/linux/hosts.j2
 netsim/templates/provider/external/external.j2
 netsim/templates/provider/libvirt/Vagrantfile.j2
 netsim/templates/provider/libvirt/arcos-domain.j2
+netsim/templates/provider/libvirt/arubacx-domain.j2
 netsim/templates/provider/libvirt/asav-domain.j2
 netsim/templates/provider/libvirt/csr-domain.j2
 netsim/templates/provider/libvirt/cumulus-domain.j2
 netsim/templates/provider/libvirt/cumulus_nvue-domain.j2
 netsim/templates/provider/libvirt/define-domain.j2
 netsim/templates/provider/libvirt/dellos10-domain.j2
 netsim/templates/provider/libvirt/eos-domain.j2
@@ -501,14 +528,15 @@
 netsim/templates/tests/clab.yml
 netsim/templates/tests/libvirt.yml
 netsim/templates/tests/virtualbox.yml
 netsim/utils/__init__.py
 netsim/utils/log.py
 netsim/utils/status.py
 netsim/utils/strings.py
+netsim/utils/templates.py
 networklab.egg-info/PKG-INFO
 networklab.egg-info/SOURCES.txt
 networklab.egg-info/dependency_links.txt
 networklab.egg-info/entry_points.txt
 networklab.egg-info/requires.txt
 networklab.egg-info/top_level.txt
 tests/test_transformation.py
```

### Comparing `networklab-1.5.1.dev1/setup.py` & `networklab-1.5.2.dev1/setup.py`

 * *Files identical despite different names*

### Comparing `networklab-1.5.1.dev1/tests/test_transformation.py` & `networklab-1.5.2.dev1/tests/test_transformation.py`

 * *Files identical despite different names*

