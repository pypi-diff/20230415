# Comparing `tmp/ttp_templates-0.3.4.tar.gz` & `tmp/ttp_templates-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ttp_templates-0.3.4.tar", max compression
+gzip compressed data, was "ttp_templates-0.3.5.tar", max compression
```

## Comparing `ttp_templates-0.3.4.tar` & `ttp_templates-0.3.5.tar`

### file list

```diff
@@ -1,67 +1,66 @@
--rw-r--r--   0        0        0     1071 2022-10-02 22:26:24.991502 ttp_templates-0.3.4/LICENSE
--rw-r--r--   0        0        0     3043 2023-03-27 09:36:31.817565 ttp_templates-0.3.4/pyproject.toml
--rw-r--r--   0        0        0    10972 2023-02-11 07:30:30.237497 ttp_templates-0.3.4/README.md
--rw-r--r--   0        0        0      123 2022-10-02 11:25:39.636968 ttp_templates-0.3.4/ttp_templates/__init__.py
--rw-r--r--   0        0        0      947 2022-10-02 22:37:25.532040 ttp_templates-0.3.4/ttp_templates/misc/N2G/cli_ip_data/a10.txt
--rw-r--r--   0        0        0     1101 2022-10-02 22:24:43.783367 ttp_templates-0.3.4/ttp_templates/misc/N2G/cli_ip_data/arista_eos.txt
--rw-r--r--   0        0        0     1283 2022-10-02 22:15:31.723463 ttp_templates-0.3.4/ttp_templates/misc/N2G/cli_ip_data/cisco_ios.txt
--rw-r--r--   0        0        0     1435 2022-10-02 22:09:41.086703 ttp_templates-0.3.4/ttp_templates/misc/N2G/cli_ip_data/cisco_nxos.txt
--rw-r--r--   0        0        0     1187 2022-10-02 22:19:24.578132 ttp_templates-0.3.4/ttp_templates/misc/N2G/cli_ip_data/cisco_xr.txt
--rw-r--r--   0        0        0     1228 2022-10-26 10:19:23.871810 ttp_templates-0.3.4/ttp_templates/misc/N2G/cli_ip_data/fortinet.txt
--rw-r--r--   0        0        0     1698 2022-10-26 10:19:35.064779 ttp_templates-0.3.4/ttp_templates/misc/N2G/cli_ip_data/huawei.txt
--rw-r--r--   0        0        0     3836 2022-10-02 12:29:05.629635 ttp_templates-0.3.4/ttp_templates/misc/N2G/cli_ip_data/readme.md
--rw-r--r--   0        0        0      379 2022-10-02 12:36:46.512026 ttp_templates-0.3.4/ttp_templates/misc/N2G/cli_isis_data/cisco_xr.txt
--rw-r--r--   0        0        0      315 2022-10-02 12:22:33.964512 ttp_templates-0.3.4/ttp_templates/misc/N2G/cli_isis_data/juniper.txt
--rw-r--r--   0        0        0      278 2022-10-02 12:12:56.783095 ttp_templates-0.3.4/ttp_templates/misc/N2G/cli_isis_data/readme.md
--rw-r--r--   0        0        0     3355 2022-10-02 12:32:05.654105 ttp_templates-0.3.4/ttp_templates/misc/N2G/cli_l2_data/cisco_ios.txt
--rw-r--r--   0        0        0     4007 2022-10-02 12:28:15.517930 ttp_templates-0.3.4/ttp_templates/misc/N2G/cli_l2_data/cisco_nxos.txt
--rw-r--r--   0        0        0     4813 2023-02-11 07:26:16.452597 ttp_templates-0.3.4/ttp_templates/misc/N2G/cli_l2_data/cisco_xr.txt
--rw-r--r--   0        0        0     3279 2022-10-02 12:32:51.413154 ttp_templates-0.3.4/ttp_templates/misc/N2G/cli_l2_data/huawei.txt
--rw-r--r--   0        0        0     3441 2022-10-02 12:31:29.981707 ttp_templates-0.3.4/ttp_templates/misc/N2G/cli_l2_data/juniper.txt
--rw-r--r--   0        0        0     6463 2022-10-02 12:16:02.938205 ttp_templates-0.3.4/ttp_templates/misc/N2G/cli_l2_data/readme.md
--rw-r--r--   0        0        0      561 2022-10-02 22:14:29.533821 ttp_templates-0.3.4/ttp_templates/misc/N2G/cli_ospf_data/cisco_ios.txt
--rw-r--r--   0        0        0      543 2022-10-02 22:12:32.166703 ttp_templates-0.3.4/ttp_templates/misc/N2G/cli_ospf_data/cisco_xr.txt
--rw-r--r--   0        0        0      328 2022-10-02 12:25:33.299732 ttp_templates-0.3.4/ttp_templates/misc/N2G/cli_ospf_data/huawei.txt
--rw-r--r--   0        0        0      263 2022-10-02 12:07:58.730648 ttp_templates-0.3.4/ttp_templates/misc/N2G/cli_ospf_data/readme.md
--rw-r--r--   0        0        0    11292 2023-03-27 09:28:11.040004 ttp_templates-0.3.4/ttp_templates/misc/Netbox/parse_arista_eos_config.txt
--rw-r--r--   0        0        0    18035 2023-03-27 09:35:20.790059 ttp_templates-0.3.4/ttp_templates/misc/Netbox/parse_cisco_xr_config.txt
--rw-r--r--   0        0        0    18394 2023-03-27 09:28:42.425193 ttp_templates-0.3.4/ttp_templates/misc/Netbox/parse_juniper_junos_config.txt
--rw-r--r--   0        0        0     1048 2022-10-02 22:28:21.715610 ttp_templates-0.3.4/ttp_templates/misc/Netmiko/cisco.ios.arp.txt
--rw-r--r--   0        0        0      573 2022-10-02 22:16:07.387371 ttp_templates-0.3.4/ttp_templates/misc/Netmiko/cisco.ios.cfg.bgp.txt
--rw-r--r--   0        0        0      269 2022-10-02 12:10:34.279564 ttp_templates-0.3.4/ttp_templates/misc/Netmiko/cisco.ios.cfg.interface.txt
--rw-r--r--   0        0        0     2508 2022-10-02 12:40:07.025191 ttp_templates-0.3.4/ttp_templates/misc/Netmiko/cisco.ios.cfg.ip.txt
--rw-r--r--   0        0        0      732 2022-10-02 22:29:33.869669 ttp_templates-0.3.4/ttp_templates/misc/Netmiko/cisco.ios.cfg.nat.static.txt
--rw-r--r--   0        0        0     1080 2022-10-02 22:25:48.921262 ttp_templates-0.3.4/ttp_templates/misc/Netmiko/cisco.iosxr.arp.txt
--rw-r--r--   0        0        0      237 2022-10-02 11:58:59.101208 ttp_templates-0.3.4/ttp_templates/misc/Netmiko/cisco.iosxr.cfg.interface.txt
--rw-r--r--   0        0        0     8068 2022-10-02 12:11:23.639834 ttp_templates-0.3.4/ttp_templates/misc/Netmiko/cisco.iosxr.cfg.ip.txt
--rw-r--r--   0        0        0      268 2022-10-02 12:10:19.166871 ttp_templates-0.3.4/ttp_templates/misc/Netmiko/huawei.vrp.cfg.interface.txt
--rw-r--r--   0        0        0     2318 2022-10-02 12:42:37.022824 ttp_templates-0.3.4/ttp_templates/misc/Netmiko/huawei.vrp.cfg.ip.txt
--rw-r--r--   0        0        0     2192 2022-10-02 21:48:54.840003 ttp_templates-0.3.4/ttp_templates/misc/ttp_templates_tests/cisco_ios_interfaces_cfg_per_ip.txt
--rw-r--r--   0        0        0      349 2022-10-02 12:30:37.129957 ttp_templates-0.3.4/ttp_templates/misc/ttp_templates_tests/netmiko_cisco_ios_interfaces.txt
--rw-r--r--   0        0        0      143 2022-10-02 11:29:02.448065 ttp_templates-0.3.4/ttp_templates/platform/arista_eos_show_hostname.txt
--rw-r--r--   0        0        0     1450 2022-10-02 22:09:04.273086 ttp_templates-0.3.4/ttp_templates/platform/cisco_ios_show_ip_arp.txt
--rw-r--r--   0        0        0     1617 2022-10-02 22:03:59.134611 ttp_templates-0.3.4/ttp_templates/platform/cisco_ios_show_ip_ospf_database_external.txt
--rw-r--r--   0        0        0     3119 2022-10-02 12:33:59.693245 ttp_templates-0.3.4/ttp_templates/platform/cisco_ios_show_ip_ospf_database_router.txt
--rw-r--r--   0        0        0     1526 2022-10-02 22:06:11.736590 ttp_templates-0.3.4/ttp_templates/platform/cisco_ios_show_ip_ospf_database_summary.txt
--rw-r--r--   0        0        0      648 2023-02-11 07:30:30.238493 ttp_templates-0.3.4/ttp_templates/platform/cisco_ios_show_isdn_status.txt
--rw-r--r--   0        0        0     4028 2022-10-02 12:28:09.353017 ttp_templates-0.3.4/ttp_templates/platform/cisco_ios_show_running_config_pipe_include_source_static.txt
--rw-r--r--   0        0        0      821 2022-10-02 22:35:43.065988 ttp_templates-0.3.4/ttp_templates/platform/cisco_ios_show_running_config_pipe_section_interface.txt
--rw-r--r--   0        0        0    10221 2022-10-02 12:06:52.103499 ttp_templates-0.3.4/ttp_templates/platform/cisco_ios_show_running_configuration_pipe_section_bgp.txt
--rw-r--r--   0        0        0      277 2022-10-02 12:12:24.982829 ttp_templates-0.3.4/ttp_templates/platform/cisco_xr_show_arp_vrf_all.txt
--rw-r--r--   0        0        0     3991 2022-10-02 12:28:18.389718 ttp_templates-0.3.4/ttp_templates/platform/cisco_xr_show_isis_database_verbose.txt
--rw-r--r--   0        0        0     2446 2022-10-02 12:40:55.762894 ttp_templates-0.3.4/ttp_templates/platform/cisco_xr_show_ospf_database_external.txt
--rw-r--r--   0        0        0     4772 2022-10-02 12:23:40.700422 ttp_templates-0.3.4/ttp_templates/platform/cisco_xr_show_ospf_database_router.txt
--rw-r--r--   0        0        0     2892 2022-10-02 12:35:46.603046 ttp_templates-0.3.4/ttp_templates/platform/cisco_xr_show_ospf_database_summary.txt
--rw-r--r--   0        0        0      631 2022-10-02 22:21:36.202852 ttp_templates-0.3.4/ttp_templates/platform/cisco_xr_show_running_config_interface.txt
--rw-r--r--   0        0        0      637 2022-10-02 22:22:05.335008 ttp_templates-0.3.4/ttp_templates/platform/huawei_display_current_configuration_interface.txt
--rw-r--r--   0        0        0     2459 2022-10-02 12:40:38.695782 ttp_templates-0.3.4/ttp_templates/platform/huawei_display_ospf_lsdb_router.txt
--rw-r--r--   0        0        0     4777 2022-10-02 12:23:37.635990 ttp_templates-0.3.4/ttp_templates/platform/juniper_show_isis_database_verbose_pipe_no_more.txt
--rw-r--r--   0        0        0      258 2022-10-02 12:05:49.151916 ttp_templates-0.3.4/ttp_templates/platform/test_platform_show_run_pipe_sec_interface.txt
--rw-r--r--   0        0        0     5457 2022-10-02 12:19:49.987503 ttp_templates-0.3.4/ttp_templates/ttp_templates.py
--rw-r--r--   0        0        0     3319 2022-10-02 12:32:22.339921 ttp_templates-0.3.4/ttp_templates/ttp_vars.py
--rw-r--r--   0        0        0     9598 2022-10-02 12:08:02.547047 ttp_templates-0.3.4/ttp_templates/yang/ietf-interfaces_cisco_ios.txt
--rw-r--r--   0        0        0     6846 2022-10-02 12:14:30.769683 ttp_templates-0.3.4/ttp_templates/yang/openconfig-lldp_cisco_ios.txt
--rw-r--r--   0        0        0     6686 2022-10-02 12:15:02.724690 ttp_templates-0.3.4/ttp_templates/yang/openconfig-lldp_cisco_nxos.txt
--rw-r--r--   0        0        0     6659 2022-10-02 12:15:19.863171 ttp_templates-0.3.4/ttp_templates/yang/openconfig-lldp_cisco_xr.txt
--rw-r--r--   0        0        0    12741 2023-03-27 09:36:52.978952 ttp_templates-0.3.4/setup.py
--rw-r--r--   0        0        0    12361 2023-03-27 09:36:52.978952 ttp_templates-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1071 2022-10-02 22:26:24.991502 ttp_templates-0.3.5/LICENSE
+-rw-r--r--   0        0        0     3042 2023-04-15 09:58:48.346483 ttp_templates-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0    10972 2023-02-11 07:30:30.237497 ttp_templates-0.3.5/README.md
+-rw-r--r--   0        0        0      123 2022-10-02 11:25:39.636968 ttp_templates-0.3.5/ttp_templates/__init__.py
+-rw-r--r--   0        0        0      947 2022-10-02 22:37:25.532040 ttp_templates-0.3.5/ttp_templates/misc/N2G/cli_ip_data/a10.txt
+-rw-r--r--   0        0        0     1101 2022-10-02 22:24:43.783367 ttp_templates-0.3.5/ttp_templates/misc/N2G/cli_ip_data/arista_eos.txt
+-rw-r--r--   0        0        0     1283 2022-10-02 22:15:31.723463 ttp_templates-0.3.5/ttp_templates/misc/N2G/cli_ip_data/cisco_ios.txt
+-rw-r--r--   0        0        0     1435 2022-10-02 22:09:41.086703 ttp_templates-0.3.5/ttp_templates/misc/N2G/cli_ip_data/cisco_nxos.txt
+-rw-r--r--   0        0        0     1187 2022-10-02 22:19:24.578132 ttp_templates-0.3.5/ttp_templates/misc/N2G/cli_ip_data/cisco_xr.txt
+-rw-r--r--   0        0        0     1228 2022-10-26 10:19:23.871810 ttp_templates-0.3.5/ttp_templates/misc/N2G/cli_ip_data/fortinet.txt
+-rw-r--r--   0        0        0     1698 2022-10-26 10:19:35.064779 ttp_templates-0.3.5/ttp_templates/misc/N2G/cli_ip_data/huawei.txt
+-rw-r--r--   0        0        0     3836 2022-10-02 12:29:05.629635 ttp_templates-0.3.5/ttp_templates/misc/N2G/cli_ip_data/readme.md
+-rw-r--r--   0        0        0      379 2022-10-02 12:36:46.512026 ttp_templates-0.3.5/ttp_templates/misc/N2G/cli_isis_data/cisco_xr.txt
+-rw-r--r--   0        0        0      315 2022-10-02 12:22:33.964512 ttp_templates-0.3.5/ttp_templates/misc/N2G/cli_isis_data/juniper.txt
+-rw-r--r--   0        0        0      278 2022-10-02 12:12:56.783095 ttp_templates-0.3.5/ttp_templates/misc/N2G/cli_isis_data/readme.md
+-rw-r--r--   0        0        0     3355 2022-10-02 12:32:05.654105 ttp_templates-0.3.5/ttp_templates/misc/N2G/cli_l2_data/cisco_ios.txt
+-rw-r--r--   0        0        0     4007 2022-10-02 12:28:15.517930 ttp_templates-0.3.5/ttp_templates/misc/N2G/cli_l2_data/cisco_nxos.txt
+-rw-r--r--   0        0        0     4813 2023-02-11 07:26:16.452597 ttp_templates-0.3.5/ttp_templates/misc/N2G/cli_l2_data/cisco_xr.txt
+-rw-r--r--   0        0        0     3279 2022-10-02 12:32:51.413154 ttp_templates-0.3.5/ttp_templates/misc/N2G/cli_l2_data/huawei.txt
+-rw-r--r--   0        0        0     3441 2022-10-02 12:31:29.981707 ttp_templates-0.3.5/ttp_templates/misc/N2G/cli_l2_data/juniper.txt
+-rw-r--r--   0        0        0     6463 2022-10-02 12:16:02.938205 ttp_templates-0.3.5/ttp_templates/misc/N2G/cli_l2_data/readme.md
+-rw-r--r--   0        0        0      561 2022-10-02 22:14:29.533821 ttp_templates-0.3.5/ttp_templates/misc/N2G/cli_ospf_data/cisco_ios.txt
+-rw-r--r--   0        0        0      543 2022-10-02 22:12:32.166703 ttp_templates-0.3.5/ttp_templates/misc/N2G/cli_ospf_data/cisco_xr.txt
+-rw-r--r--   0        0        0      328 2022-10-02 12:25:33.299732 ttp_templates-0.3.5/ttp_templates/misc/N2G/cli_ospf_data/huawei.txt
+-rw-r--r--   0        0        0      263 2022-10-02 12:07:58.730648 ttp_templates-0.3.5/ttp_templates/misc/N2G/cli_ospf_data/readme.md
+-rw-r--r--   0        0        0    11292 2023-03-27 09:28:11.040004 ttp_templates-0.3.5/ttp_templates/misc/Netbox/parse_arista_eos_config.txt
+-rw-r--r--   0        0        0    18124 2023-04-15 09:57:15.372704 ttp_templates-0.3.5/ttp_templates/misc/Netbox/parse_cisco_xr_config.txt
+-rw-r--r--   0        0        0    18448 2023-04-15 09:57:04.354679 ttp_templates-0.3.5/ttp_templates/misc/Netbox/parse_juniper_junos_config.txt
+-rw-r--r--   0        0        0     1048 2022-10-02 22:28:21.715610 ttp_templates-0.3.5/ttp_templates/misc/Netmiko/cisco.ios.arp.txt
+-rw-r--r--   0        0        0      573 2022-10-02 22:16:07.387371 ttp_templates-0.3.5/ttp_templates/misc/Netmiko/cisco.ios.cfg.bgp.txt
+-rw-r--r--   0        0        0      269 2022-10-02 12:10:34.279564 ttp_templates-0.3.5/ttp_templates/misc/Netmiko/cisco.ios.cfg.interface.txt
+-rw-r--r--   0        0        0     2508 2022-10-02 12:40:07.025191 ttp_templates-0.3.5/ttp_templates/misc/Netmiko/cisco.ios.cfg.ip.txt
+-rw-r--r--   0        0        0      732 2022-10-02 22:29:33.869669 ttp_templates-0.3.5/ttp_templates/misc/Netmiko/cisco.ios.cfg.nat.static.txt
+-rw-r--r--   0        0        0     1080 2022-10-02 22:25:48.921262 ttp_templates-0.3.5/ttp_templates/misc/Netmiko/cisco.iosxr.arp.txt
+-rw-r--r--   0        0        0      237 2022-10-02 11:58:59.101208 ttp_templates-0.3.5/ttp_templates/misc/Netmiko/cisco.iosxr.cfg.interface.txt
+-rw-r--r--   0        0        0     8068 2022-10-02 12:11:23.639834 ttp_templates-0.3.5/ttp_templates/misc/Netmiko/cisco.iosxr.cfg.ip.txt
+-rw-r--r--   0        0        0      268 2022-10-02 12:10:19.166871 ttp_templates-0.3.5/ttp_templates/misc/Netmiko/huawei.vrp.cfg.interface.txt
+-rw-r--r--   0        0        0     2318 2022-10-02 12:42:37.022824 ttp_templates-0.3.5/ttp_templates/misc/Netmiko/huawei.vrp.cfg.ip.txt
+-rw-r--r--   0        0        0     2192 2022-10-02 21:48:54.840003 ttp_templates-0.3.5/ttp_templates/misc/ttp_templates_tests/cisco_ios_interfaces_cfg_per_ip.txt
+-rw-r--r--   0        0        0      349 2022-10-02 12:30:37.129957 ttp_templates-0.3.5/ttp_templates/misc/ttp_templates_tests/netmiko_cisco_ios_interfaces.txt
+-rw-r--r--   0        0        0      143 2022-10-02 11:29:02.448065 ttp_templates-0.3.5/ttp_templates/platform/arista_eos_show_hostname.txt
+-rw-r--r--   0        0        0     1450 2022-10-02 22:09:04.273086 ttp_templates-0.3.5/ttp_templates/platform/cisco_ios_show_ip_arp.txt
+-rw-r--r--   0        0        0     1617 2022-10-02 22:03:59.134611 ttp_templates-0.3.5/ttp_templates/platform/cisco_ios_show_ip_ospf_database_external.txt
+-rw-r--r--   0        0        0     3119 2022-10-02 12:33:59.693245 ttp_templates-0.3.5/ttp_templates/platform/cisco_ios_show_ip_ospf_database_router.txt
+-rw-r--r--   0        0        0     1526 2022-10-02 22:06:11.736590 ttp_templates-0.3.5/ttp_templates/platform/cisco_ios_show_ip_ospf_database_summary.txt
+-rw-r--r--   0        0        0      648 2023-02-11 07:30:30.238493 ttp_templates-0.3.5/ttp_templates/platform/cisco_ios_show_isdn_status.txt
+-rw-r--r--   0        0        0     4028 2022-10-02 12:28:09.353017 ttp_templates-0.3.5/ttp_templates/platform/cisco_ios_show_running_config_pipe_include_source_static.txt
+-rw-r--r--   0        0        0      821 2022-10-02 22:35:43.065988 ttp_templates-0.3.5/ttp_templates/platform/cisco_ios_show_running_config_pipe_section_interface.txt
+-rw-r--r--   0        0        0    10221 2022-10-02 12:06:52.103499 ttp_templates-0.3.5/ttp_templates/platform/cisco_ios_show_running_configuration_pipe_section_bgp.txt
+-rw-r--r--   0        0        0      277 2022-10-02 12:12:24.982829 ttp_templates-0.3.5/ttp_templates/platform/cisco_xr_show_arp_vrf_all.txt
+-rw-r--r--   0        0        0     3991 2022-10-02 12:28:18.389718 ttp_templates-0.3.5/ttp_templates/platform/cisco_xr_show_isis_database_verbose.txt
+-rw-r--r--   0        0        0     2446 2022-10-02 12:40:55.762894 ttp_templates-0.3.5/ttp_templates/platform/cisco_xr_show_ospf_database_external.txt
+-rw-r--r--   0        0        0     4772 2022-10-02 12:23:40.700422 ttp_templates-0.3.5/ttp_templates/platform/cisco_xr_show_ospf_database_router.txt
+-rw-r--r--   0        0        0     2892 2022-10-02 12:35:46.603046 ttp_templates-0.3.5/ttp_templates/platform/cisco_xr_show_ospf_database_summary.txt
+-rw-r--r--   0        0        0      631 2022-10-02 22:21:36.202852 ttp_templates-0.3.5/ttp_templates/platform/cisco_xr_show_running_config_interface.txt
+-rw-r--r--   0        0        0      637 2022-10-02 22:22:05.335008 ttp_templates-0.3.5/ttp_templates/platform/huawei_display_current_configuration_interface.txt
+-rw-r--r--   0        0        0     2459 2022-10-02 12:40:38.695782 ttp_templates-0.3.5/ttp_templates/platform/huawei_display_ospf_lsdb_router.txt
+-rw-r--r--   0        0        0     4777 2022-10-02 12:23:37.635990 ttp_templates-0.3.5/ttp_templates/platform/juniper_show_isis_database_verbose_pipe_no_more.txt
+-rw-r--r--   0        0        0      258 2022-10-02 12:05:49.151916 ttp_templates-0.3.5/ttp_templates/platform/test_platform_show_run_pipe_sec_interface.txt
+-rw-r--r--   0        0        0     5457 2022-10-02 12:19:49.987503 ttp_templates-0.3.5/ttp_templates/ttp_templates.py
+-rw-r--r--   0        0        0     3319 2022-10-02 12:32:22.339921 ttp_templates-0.3.5/ttp_templates/ttp_vars.py
+-rw-r--r--   0        0        0     9598 2022-10-02 12:08:02.547047 ttp_templates-0.3.5/ttp_templates/yang/ietf-interfaces_cisco_ios.txt
+-rw-r--r--   0        0        0     6846 2022-10-02 12:14:30.769683 ttp_templates-0.3.5/ttp_templates/yang/openconfig-lldp_cisco_ios.txt
+-rw-r--r--   0        0        0     6686 2022-10-02 12:15:02.724690 ttp_templates-0.3.5/ttp_templates/yang/openconfig-lldp_cisco_nxos.txt
+-rw-r--r--   0        0        0     6659 2022-10-02 12:15:19.863171 ttp_templates-0.3.5/ttp_templates/yang/openconfig-lldp_cisco_xr.txt
+-rw-r--r--   0        0        0    12669 1970-01-01 00:00:00.000000 ttp_templates-0.3.5/PKG-INFO
```

### Comparing `ttp_templates-0.3.4/LICENSE` & `ttp_templates-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ttp_templates-0.3.4/pyproject.toml` & `ttp_templates-0.3.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ttp_templates"
-version = "0.3.4"
+version = "0.3.5"
 description = "Template Text Parser Templates collections"
 license = "MIT"
 include = [
     "platform/*.txt",
     "yang/*.txt",
     "misc/*/*.txt",
 ]
@@ -42,15 +42,15 @@
 [tool.poetry.dev-dependencies]
 bandit = { version = "1.7.*", markers = "python_version >= '3.7'" }
 black = { version = "22.3.*", markers = "python_version >= '3.7'" }
 flake8 = { version = "4.0.*", markers = "python_version >= '3.7'" }
 pre-commit = { version = "2.15.*", markers = "python_version >= '3.7'" }
 pyenchant = { version = "3.2.*", markers = "python_version >= '3.7'" }
 pylint = { version = "2.12.*", markers = "python_version >= '3.7'" }
-pytest = { version = "^7.1.*", markers = "python_version >= '3.7'" }
+pytest = { version = "7.1.*", markers = "python_version >= '3.7'" }
 cerberus = { version = "1.3.*", markers = "python_version >= '3.7'" }
 jinja2 = { version = "3.0.*", markers = "python_version >= '3.7'" }
 pyyaml = { version = "6.0", markers = "python_version >= '3.7'" }
 deepdiff = { version = "5.8.*", markers = "python_version >= '3.7'" }
 openpyxl = { version = "3.0.*", markers = "python_version >= '3.7'" }
 tabulate = { version = "0.8.*", markers = "python_version >= '3.7'" }
 yangson = { version = "1.4.*", markers = "python_version >= '3.7'" }
```

### Comparing `ttp_templates-0.3.4/README.md` & `ttp_templates-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `ttp_templates-0.3.4/ttp_templates/misc/N2G/cli_ip_data/a10.txt` & `ttp_templates-0.3.5/ttp_templates/misc/N2G/cli_ip_data/a10.txt`

 * *Files identical despite different names*

### Comparing `ttp_templates-0.3.4/ttp_templates/misc/N2G/cli_ip_data/arista_eos.txt` & `ttp_templates-0.3.5/ttp_templates/misc/N2G/cli_ip_data/arista_eos.txt`

 * *Files identical despite different names*

### Comparing `ttp_templates-0.3.4/ttp_templates/misc/N2G/cli_ip_data/cisco_ios.txt` & `ttp_templates-0.3.5/ttp_templates/misc/N2G/cli_ip_data/cisco_ios.txt`

 * *Files identical despite different names*

### Comparing `ttp_templates-0.3.4/ttp_templates/misc/N2G/cli_ip_data/cisco_nxos.txt` & `ttp_templates-0.3.5/ttp_templates/misc/N2G/cli_ip_data/cisco_nxos.txt`

 * *Files identical despite different names*

### Comparing `ttp_templates-0.3.4/ttp_templates/misc/N2G/cli_ip_data/cisco_xr.txt` & `ttp_templates-0.3.5/ttp_templates/misc/N2G/cli_ip_data/cisco_xr.txt`

 * *Files identical despite different names*

### Comparing `ttp_templates-0.3.4/ttp_templates/misc/N2G/cli_ip_data/fortinet.txt` & `ttp_templates-0.3.5/ttp_templates/misc/N2G/cli_ip_data/fortinet.txt`

 * *Files identical despite different names*

### Comparing `ttp_templates-0.3.4/ttp_templates/misc/N2G/cli_ip_data/huawei.txt` & `ttp_templates-0.3.5/ttp_templates/misc/N2G/cli_ip_data/huawei.txt`

 * *Files identical despite different names*

### Comparing `ttp_templates-0.3.4/ttp_templates/misc/N2G/cli_ip_data/readme.md` & `ttp_templates-0.3.5/ttp_templates/misc/N2G/cli_ip_data/readme.md`

 * *Files identical despite different names*

### Comparing `ttp_templates-0.3.4/ttp_templates/misc/N2G/cli_l2_data/cisco_ios.txt` & `ttp_templates-0.3.5/ttp_templates/misc/N2G/cli_l2_data/cisco_ios.txt`

 * *Files identical despite different names*

### Comparing `ttp_templates-0.3.4/ttp_templates/misc/N2G/cli_l2_data/cisco_nxos.txt` & `ttp_templates-0.3.5/ttp_templates/misc/N2G/cli_l2_data/cisco_nxos.txt`

 * *Files identical despite different names*

### Comparing `ttp_templates-0.3.4/ttp_templates/misc/N2G/cli_l2_data/cisco_xr.txt` & `ttp_templates-0.3.5/ttp_templates/misc/N2G/cli_l2_data/cisco_xr.txt`

 * *Files identical despite different names*

### Comparing `ttp_templates-0.3.4/ttp_templates/misc/N2G/cli_l2_data/huawei.txt` & `ttp_templates-0.3.5/ttp_templates/misc/N2G/cli_l2_data/huawei.txt`

 * *Files identical despite different names*

### Comparing `ttp_templates-0.3.4/ttp_templates/misc/N2G/cli_l2_data/juniper.txt` & `ttp_templates-0.3.5/ttp_templates/misc/N2G/cli_l2_data/juniper.txt`

 * *Files identical despite different names*

### Comparing `ttp_templates-0.3.4/ttp_templates/misc/N2G/cli_l2_data/readme.md` & `ttp_templates-0.3.5/ttp_templates/misc/N2G/cli_l2_data/readme.md`

 * *Files identical despite different names*

### Comparing `ttp_templates-0.3.4/ttp_templates/misc/N2G/cli_ospf_data/cisco_ios.txt` & `ttp_templates-0.3.5/ttp_templates/misc/N2G/cli_ospf_data/cisco_ios.txt`

 * *Files identical despite different names*

### Comparing `ttp_templates-0.3.4/ttp_templates/misc/N2G/cli_ospf_data/cisco_xr.txt` & `ttp_templates-0.3.5/ttp_templates/misc/N2G/cli_ospf_data/cisco_xr.txt`

 * *Files identical despite different names*

### Comparing `ttp_templates-0.3.4/ttp_templates/misc/Netbox/parse_arista_eos_config.txt` & `ttp_templates-0.3.5/ttp_templates/misc/Netbox/parse_arista_eos_config.txt`

 * *Files identical despite different names*

### Comparing `ttp_templates-0.3.4/ttp_templates/misc/Netbox/parse_cisco_xr_config.txt` & `ttp_templates-0.3.5/ttp_templates/misc/Netbox/parse_cisco_xr_config.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 <template name="netbox_data" results="per_template">
 <doc>
-Template to parse Arista EOS configuration and produce data structure
+Template to parse Cisco IOS-XR configuration and produce data structure
 that is easy to work with to import data into the Netbox.
 
 This template requires output of `show running-config` command.
 </doc>
 
 <input>
 commands = [
@@ -32,15 +32,15 @@
     return data
     
 def add_parent_interface(data):
     if "lag_id" in data:
         data["parent"] = "Bundle-Ether{}".format(data["lag_id"])
     elif "." in data["name"]:
         data["parent"] = data["name"].split(".")[0]
-    return data	
+    return data    
 </macro>
 
 ## ------------------------------------------------------------------------------------------
 ## Global Configuration facts
 ## ------------------------------------------------------------------------------------------
 <group name="facts**" method="table">
 hostname {{ hostname }}
@@ -163,14 +163,15 @@
 ## ------------------------------------------------------------------------------------------
 ## Interfaces configuration
 ## ------------------------------------------------------------------------------------------
 <group name="interfaces*" functions="contains('name') | macro('add_interface_type') | macro('add_parent_interface')">
 interface {{ name | _start_ }}
 interface {{ name | _start_ }} l2transport
 interface preconfigure {{ name | _start_ | let("preconfigure", True) }}
+interface preconfigure {{ name | _start_ | let("preconfigure", True) }} l2transport
  description {{ description | re(".*") | default("") }}
  mtu {{ mtu | to_int }}
  service-policy input {{ qos_policy_in }}
  service-policy output {{ qos_policy_out }}
  encapsulation dot1q {{ dot1q }}
  vrf {{ vrf }}
  bundle id {{ lag_id }} mode {{ lacp_mode }}
```

### Comparing `ttp_templates-0.3.4/ttp_templates/misc/Netbox/parse_juniper_junos_config.txt` & `ttp_templates-0.3.5/ttp_templates/misc/Netbox/parse_juniper_junos_config.txt`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,16 @@
 def postprocess(data):
     # transform vrf dict to list
     data["vrf"] = [{"name": k, **v} for k, v in data.get("vrf", {}).items()]
     
     # update interfaces with VRF reference
     for vrf in data["vrf"]:
         for interface in vrf.get("interfaces", []):
-            data["interfaces"][interface]["vrf"] = vrf["name"]
+            if data["interfaces"].get(interface):
+                data["interfaces"][interface]["vrf"] = vrf["name"]
             
     # transform interfaces dict to list
     data["interfaces"] = [
         {"name": k, **v} 
         for k, v in data["interfaces"].items()
     ]
```

### Comparing `ttp_templates-0.3.4/ttp_templates/misc/Netmiko/cisco.ios.arp.txt` & `ttp_templates-0.3.5/ttp_templates/misc/Netmiko/cisco.ios.arp.txt`

 * *Files identical despite different names*

### Comparing `ttp_templates-0.3.4/ttp_templates/misc/Netmiko/cisco.ios.cfg.bgp.txt` & `ttp_templates-0.3.5/ttp_templates/misc/Netmiko/cisco.ios.cfg.bgp.txt`

 * *Files identical despite different names*

### Comparing `ttp_templates-0.3.4/ttp_templates/misc/Netmiko/cisco.ios.cfg.ip.txt` & `ttp_templates-0.3.5/ttp_templates/misc/Netmiko/cisco.ios.cfg.ip.txt`

 * *Files identical despite different names*

### Comparing `ttp_templates-0.3.4/ttp_templates/misc/Netmiko/cisco.ios.cfg.nat.static.txt` & `ttp_templates-0.3.5/ttp_templates/misc/Netmiko/cisco.ios.cfg.nat.static.txt`

 * *Files identical despite different names*

### Comparing `ttp_templates-0.3.4/ttp_templates/misc/Netmiko/cisco.iosxr.arp.txt` & `ttp_templates-0.3.5/ttp_templates/misc/Netmiko/cisco.iosxr.arp.txt`

 * *Files identical despite different names*

### Comparing `ttp_templates-0.3.4/ttp_templates/misc/Netmiko/cisco.iosxr.cfg.ip.txt` & `ttp_templates-0.3.5/ttp_templates/misc/Netmiko/cisco.iosxr.cfg.ip.txt`

 * *Files identical despite different names*

### Comparing `ttp_templates-0.3.4/ttp_templates/misc/Netmiko/huawei.vrp.cfg.ip.txt` & `ttp_templates-0.3.5/ttp_templates/misc/Netmiko/huawei.vrp.cfg.ip.txt`

 * *Files identical despite different names*

### Comparing `ttp_templates-0.3.4/ttp_templates/misc/ttp_templates_tests/cisco_ios_interfaces_cfg_per_ip.txt` & `ttp_templates-0.3.5/ttp_templates/misc/ttp_templates_tests/cisco_ios_interfaces_cfg_per_ip.txt`

 * *Files identical despite different names*

### Comparing `ttp_templates-0.3.4/ttp_templates/platform/cisco_ios_show_ip_arp.txt` & `ttp_templates-0.3.5/ttp_templates/platform/cisco_ios_show_ip_arp.txt`

 * *Files identical despite different names*

### Comparing `ttp_templates-0.3.4/ttp_templates/platform/cisco_ios_show_ip_ospf_database_external.txt` & `ttp_templates-0.3.5/ttp_templates/platform/cisco_ios_show_ip_ospf_database_external.txt`

 * *Files identical despite different names*

### Comparing `ttp_templates-0.3.4/ttp_templates/platform/cisco_ios_show_ip_ospf_database_router.txt` & `ttp_templates-0.3.5/ttp_templates/platform/cisco_ios_show_ip_ospf_database_router.txt`

 * *Files identical despite different names*

### Comparing `ttp_templates-0.3.4/ttp_templates/platform/cisco_ios_show_ip_ospf_database_summary.txt` & `ttp_templates-0.3.5/ttp_templates/platform/cisco_ios_show_ip_ospf_database_summary.txt`

 * *Files identical despite different names*

### Comparing `ttp_templates-0.3.4/ttp_templates/platform/cisco_ios_show_isdn_status.txt` & `ttp_templates-0.3.5/ttp_templates/platform/cisco_ios_show_isdn_status.txt`

 * *Files identical despite different names*

### Comparing `ttp_templates-0.3.4/ttp_templates/platform/cisco_ios_show_running_config_pipe_include_source_static.txt` & `ttp_templates-0.3.5/ttp_templates/platform/cisco_ios_show_running_config_pipe_include_source_static.txt`

 * *Files identical despite different names*

### Comparing `ttp_templates-0.3.4/ttp_templates/platform/cisco_ios_show_running_config_pipe_section_interface.txt` & `ttp_templates-0.3.5/ttp_templates/platform/cisco_ios_show_running_config_pipe_section_interface.txt`

 * *Files identical despite different names*

### Comparing `ttp_templates-0.3.4/ttp_templates/platform/cisco_ios_show_running_configuration_pipe_section_bgp.txt` & `ttp_templates-0.3.5/ttp_templates/platform/cisco_ios_show_running_configuration_pipe_section_bgp.txt`

 * *Files identical despite different names*

### Comparing `ttp_templates-0.3.4/ttp_templates/platform/cisco_xr_show_isis_database_verbose.txt` & `ttp_templates-0.3.5/ttp_templates/platform/cisco_xr_show_isis_database_verbose.txt`

 * *Files identical despite different names*

### Comparing `ttp_templates-0.3.4/ttp_templates/platform/cisco_xr_show_ospf_database_external.txt` & `ttp_templates-0.3.5/ttp_templates/platform/cisco_xr_show_ospf_database_external.txt`

 * *Files identical despite different names*

### Comparing `ttp_templates-0.3.4/ttp_templates/platform/cisco_xr_show_ospf_database_router.txt` & `ttp_templates-0.3.5/ttp_templates/platform/cisco_xr_show_ospf_database_router.txt`

 * *Files identical despite different names*

### Comparing `ttp_templates-0.3.4/ttp_templates/platform/cisco_xr_show_ospf_database_summary.txt` & `ttp_templates-0.3.5/ttp_templates/platform/cisco_xr_show_ospf_database_summary.txt`

 * *Files identical despite different names*

### Comparing `ttp_templates-0.3.4/ttp_templates/platform/cisco_xr_show_running_config_interface.txt` & `ttp_templates-0.3.5/ttp_templates/platform/cisco_xr_show_running_config_interface.txt`

 * *Files identical despite different names*

### Comparing `ttp_templates-0.3.4/ttp_templates/platform/huawei_display_current_configuration_interface.txt` & `ttp_templates-0.3.5/ttp_templates/platform/huawei_display_current_configuration_interface.txt`

 * *Files identical despite different names*

### Comparing `ttp_templates-0.3.4/ttp_templates/platform/huawei_display_ospf_lsdb_router.txt` & `ttp_templates-0.3.5/ttp_templates/platform/huawei_display_ospf_lsdb_router.txt`

 * *Files identical despite different names*

### Comparing `ttp_templates-0.3.4/ttp_templates/platform/juniper_show_isis_database_verbose_pipe_no_more.txt` & `ttp_templates-0.3.5/ttp_templates/platform/juniper_show_isis_database_verbose_pipe_no_more.txt`

 * *Files identical despite different names*

### Comparing `ttp_templates-0.3.4/ttp_templates/ttp_templates.py` & `ttp_templates-0.3.5/ttp_templates/ttp_templates.py`

 * *Files identical despite different names*

### Comparing `ttp_templates-0.3.4/ttp_templates/ttp_vars.py` & `ttp_templates-0.3.5/ttp_templates/ttp_vars.py`

 * *Files identical despite different names*

### Comparing `ttp_templates-0.3.4/ttp_templates/yang/ietf-interfaces_cisco_ios.txt` & `ttp_templates-0.3.5/ttp_templates/yang/ietf-interfaces_cisco_ios.txt`

 * *Files identical despite different names*

### Comparing `ttp_templates-0.3.4/ttp_templates/yang/openconfig-lldp_cisco_ios.txt` & `ttp_templates-0.3.5/ttp_templates/yang/openconfig-lldp_cisco_ios.txt`

 * *Files identical despite different names*

### Comparing `ttp_templates-0.3.4/ttp_templates/yang/openconfig-lldp_cisco_nxos.txt` & `ttp_templates-0.3.5/ttp_templates/yang/openconfig-lldp_cisco_nxos.txt`

 * *Files identical despite different names*

### Comparing `ttp_templates-0.3.4/ttp_templates/yang/openconfig-lldp_cisco_xr.txt` & `ttp_templates-0.3.5/ttp_templates/yang/openconfig-lldp_cisco_xr.txt`

 * *Files identical despite different names*

### Comparing `ttp_templates-0.3.4/PKG-INFO` & `ttp_templates-0.3.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,42 @@
 Metadata-Version: 2.1
 Name: ttp-templates
-Version: 0.3.4
+Version: 0.3.5
 Summary: Template Text Parser Templates collections
 Home-page: https://github.com/dmulyalin/ttp_templates
 License: MIT
 Keywords: Parsing,TTP,regex
 Author: Denis Mulyalin
 Author-email: d.mulyalin@gmail.com
 Maintainer: Denis Mulyalin
 Maintainer-email: d.mulyalin@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Utilities
 Provides-Extra: docs
-Requires-Dist: mkdocs (==1.2.4); (python_version >= "3.7") and (extra == "docs")
-Requires-Dist: mkdocs-material (==7.2.2); (python_version >= "3.7") and (extra == "docs")
-Requires-Dist: mkdocs-material-extensions (==1.0.1); (python_version >= "3.7") and (extra == "docs")
-Requires-Dist: mkdocstrings[python] (>=0.18.0,<0.19.0); (python_version >= "3.7") and (extra == "docs")
-Requires-Dist: pygments (==2.11); (python_version >= "3.7") and (extra == "docs")
-Requires-Dist: pymdown-extensions (==9.3); (python_version >= "3.7") and (extra == "docs")
+Requires-Dist: mkdocs (==1.2.4) ; (python_version >= "3.7") and (extra == "docs")
+Requires-Dist: mkdocs-material (==7.2.2) ; (python_version >= "3.7") and (extra == "docs")
+Requires-Dist: mkdocs-material-extensions (==1.0.1) ; (python_version >= "3.7") and (extra == "docs")
+Requires-Dist: mkdocstrings[python] (>=0.18.0,<0.19.0) ; (python_version >= "3.7") and (extra == "docs")
+Requires-Dist: pygments (==2.11) ; (python_version >= "3.7") and (extra == "docs")
+Requires-Dist: pymdown-extensions (==9.3) ; (python_version >= "3.7") and (extra == "docs")
 Requires-Dist: ttp (>=0.6.0)
 Project-URL: Documentation, https://dmulyalin.github.io/ttp_templates/
 Project-URL: Repository, https://github.com/dmulyalin/ttp_templates
 Description-Content-Type: text/markdown
 
 [![Downloads](https://pepy.tech/badge/ttp_templates)](https://pepy.tech/project/ttp_templates)
 [![PyPI versions](https://img.shields.io/pypi/pyversions/ttp.svg)](https://pypi.python.org/pypi/ttp_templates/)
```

