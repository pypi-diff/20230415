# Comparing `tmp/ddqa-0.0.1.tar.gz` & `tmp/ddqa-0.1.0.tar.gz`

## Comparing `ddqa-0.0.1.tar` & `ddqa-0.1.0.tar`

### file list

```diff
@@ -1,1024 +1,111 @@
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 ddqa-0.0.1/.gitattributes
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 ddqa-0.0.1/.linkcheckerrc
--rw-r--r--   0        0        0     3192 2020-02-02 00:00:00.000000 ddqa-0.0.1/mkdocs.yml
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 ddqa-0.0.1/.github/dependabot.yml
--rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 ddqa-0.0.1/.github/workflows/build.yml
--rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 ddqa-0.0.1/.github/workflows/docs.yml
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 ddqa-0.0.1/.github/workflows/publish-docs.yml
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 ddqa-0.0.1/.github/workflows/test.yml
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/1029d87753feb69a
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/10373bc2dcc33db6
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/113f147c28e5068a
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/11427d1a344df241
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/117593f35b8dad72
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/1206e0cd494bb9a0
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/120b3b87b79ec6f4
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/1284f24ad366f6b1
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/12b91fce237b7dad
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/1328f38a9dae505c
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/133d6d6941b6c110
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/1369d1d4a2fa128c
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/13a7f397cde8dafc
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/13b00e48048133fe
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/13d3c165b6407de5
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/13e51d06e5c60916
--rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/1457430fda7b83ca
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/1489da15cfe57785
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/14e6bf91c9cc874b
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/15ebb27340a7d746
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/161a6b73b386fe6d
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/16adf796486a9c18
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/16b61e1438d4753c
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/16bc6b5309b82f4c
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/1731635225cf4e2b
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/1736db8819936b44
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/179d30666d859674
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/17b3a319fe6880d0
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/17f3f77f055bf8aa
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/180d6d66a31cb21
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/184e72bf94fbf0f7
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/185f2308cd0e2282
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/1865a3ab023568f9
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/188ff3ab0610e3fa
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/18cba55528275a2f
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/18d2ad3adab2111a
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/18d3a8b17c303c2b
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/19065c016fa870e0
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/191b9c9674e3fdfc
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/19501b2cb410981
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/19a227a22676940f
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/19c1444af4b29a7
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/19c6431ac2454384
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/1a75f79715004875
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/1a8922a5c5f2648a
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/1ab0686ba2a54fe0
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/1b7faba3056994ff
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/1bdbf3f62fdf84f7
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/1bff425a12f7ca81
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/1c2e0e0efff8f10
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/1c88d27ff0ea9682
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/1c9422ce88839089
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/1d324dfcc3545f23
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/1d7e0f80bb76a723
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/1dbff4c9ef6b2d58
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/1dfce5496d22a582
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/1e29ba3bd3b73bec
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/1e2a76e2eba1c472
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/1e91f4d485357889
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/1efac76dc25c5f64
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/1f0324c51af329ff
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/1f3b877f6c83f1e1
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/1f5fb8e250400fd7
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/1ffdf861d263f300
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/211d1d60b9859487
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/2180c2b1e31e87ed
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/218915227727a611
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/21a39b83f4e9ae06
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/21ad056728376e9f
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/2201a8feb7ca59c9
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/223e7bd83dbf000c
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/22ca5c611fd658f3
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/2366df546fae3f3f
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/236ffca4e716f4fa
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/237bbca6e63874ff
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/23f89ef6c0237832
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/245c581d4984a7a9
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/2468f386f32daa1d
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/247dae6198da2e58
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/24ccd941a0bb4bd5
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/25590c5b6177a409
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/25954b6c65416426
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/266295192a38703a
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/26ae945e0c037d98
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/26ba6d1bb3ef4505
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/27190ee6fe95f81e
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/2787a6f8e47efe84
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/27e5125eb54d3dd
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/287179b5a2d98ef3
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/28834f1daf529c9c
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/28dc17b46d43cde5
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/29221027f2ecd1d9
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/29273045af7c673c
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/29649f509c65079b
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/2a142155317913a4
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/2a9b91ae9fcb4d16
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/2ac8f0940d624c1a
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/2b6c689d7d940542
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/2b7b82d8208b6c5f
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/2ba3fcf65112d90a
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/2c6bc1bbefbe189f
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/2cd5f83bd60533c7
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/2cf168709a8ae76a
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/2d38e4b991f8c73
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/2d61328ede831075
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/2d8d7c8263c39ed2
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/2db417eb58195adb
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/2df0a456c6236db7
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/2e734f6c69c22c67
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/2e7b14bb35ecb641
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/2ea0aa913d15661a
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/2eec525fcfbf483f
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/2f089b4ecd332b80
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/2f0c8665485bd839
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/2f37d53e4fce4edf
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/2f5daaf8c7276710
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/3046fbee73101ba6
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/309eb5b0b062c521
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/30a757051bb87c41
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/30e68fcbfbcd388d
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/313f58a23d16dc56
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/31c239a79a150cc2
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/3207e7ea8f63887c
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/320f7a2c4483d170
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/326d13d0c26039b4
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/32dac69f42d22d43
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/33e1e9d1dc3d9d3
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/3466b6d5ddd5df2b
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/34687b099cad27a8
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/347d04d99847afe9
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/34a65c1f3b79df5b
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/3523f8d094edc73e
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/3657abae4673a791
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/36914b21fdf70c8d
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/369ed2d7a1a3f83a
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/3727d5f4d84155fb
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/37addcd0065b3a57
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/38da728ecd64f561
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/38f2b5804cbc8f3
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/390268ff8afd1a07
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/392aa3db698c231
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/39b913dde8dfebb0
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/3a3e21a4fffa6e2
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/3a5ec798cb4e26e6
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/3a9e9d4eb3f96325
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/3ac9959766fa7a20
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/3aca74fc9ea96deb
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/3b3f44227ea121de
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/3c0cdf4b6b60012c
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/3cfeb07ab7a582b7
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/3d0c3ad7bb589db8
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/3d201b0a2322367a
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/3ddbd03b8a50a8b2
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/3dfc1df6f2c304f1
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/3eb18ac5b70e9261
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/3eeb6d99c8953a0f
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/3eeca29e202930fb
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/3f1ae15aa3bd2b2e
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/3f43b58676d1664f
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/3f89abdce12374a8
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/3f95fda8bfa4a179
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/3fb9bf6090dc9158
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/401d96b09218d739
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/404ccb238b5e9d8b
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/40a45d6735f4b68c
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/40be32df8e7f334
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/41687d3e574fc67e
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/41794439a9611ebc
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/41c0d4ca8ba46cfe
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/41ddc42da5145862
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/424e0cbc746a66ae
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/428a00c1183a043
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/430bbefe2911326f
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/4366371e80079783
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/43730f0f9cd8d621
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/43877d87de7d97fb
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/43a8a86795d75cce
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/43e3a4177ec2d5db
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/4429fa20b5926b15
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/444f1f5e9fcbb337
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/46635d5329ff6c6
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/4684f15887a9e4e9
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/47177d5be0d5cf79
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/476ab4570cfdb409
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/4771f72255ab61b9
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/47b000a61c8945a
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/47e51158cf3988f6
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/47f996140e7d4b9f
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/4875a95f4c046ea6
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/48c25fd601b65da9
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/48efcf6833e51e57
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/491657159dcb22a5
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/4925405d013336a3
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/4a99979c03777c96
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/4ad37ffe4ba18253
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/4aed371a8aa05bef
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/4b24659322a4c3ba
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/4b2ea1c9eef860f7
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/4b6ee4eccb02d80a
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/4ba7a9d16f3e0975
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/4badfacf6d955ae0
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/4bb1015af0efa1b8
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/4c6343087ccc428a
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/4c7d4b84c6ab5e02
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/4dd62b9e28803e9e
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/4e509ef419e97e15
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/4ed1da3bbde3d39d
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/4f01edf05a1f1674
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/4fdd5e4aa6f8aed9
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/502250a457e31455
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/5022bf39ffc54558
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/5033eac691f9e1e3
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/5050126977cd1c5
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/507ee7850b43db8c
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/50bacf3510b25842
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/5102ead14c458377
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/517b989e10279ac6
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/52a89cc36fc3eaf0
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/52cec1b44d1f4fae
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/5337284f3b4a874
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/53a9b340c64b74
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/53c5a81a9a125f6
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/545bfc4b0100a055
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/54d19f9b12dfd7d4
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/55397a1bd540efa6
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/5567b27a2b510e07
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/56146d51b1386f7a
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/561daf4cb9b4a5eb
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/561ddc78426a3111
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/567288932bb94f1c
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/56cef349d4ea2e25
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/5700fb1f76cab5d8
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/57341afb9d34278c
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/57617c032953f63f
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/5775677a249ce5ff
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/5805b0986eedbcf4
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/5817efefdfa233c5
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/586a397d27fe79bd
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/58cf958f25a2288b
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/58e9c420c8cc55e
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/58ebb079374456f3
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/594341d418d22c40
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/59486d0c0195527e
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/5956c81ff9bf5843
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/59e9a44ba7a12380
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/59f582a151901112
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/5a0eb91ea66971d0
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/5a2303d90d1d33d7
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/5aa1c15152f21d69
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/5ac01a6e15ff8478
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/5c76063787444f7a
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/5c7c9c8da4ce8fc1
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/5c83b185456b3719
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/5d1a917eac921eb5
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/5d1de61e22ec72a
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/5d1fba4dd289871f
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/5d5bc73277fa02fb
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/5d76c0b602f336fe
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/5da340cb03d4bc9a
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/5dd59036b08f3483
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/5e36ca049112b4fe
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/5e41ada6349f3ca6
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/5f13814429146cf5
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/5f3a22cfd91b0ec9
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/5f802831a636066a
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/5fdd30f79b6bbd03
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/5fe0bffc53caa88d
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/5ff7f0e0e1d22af8
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/6026086e981d7a0f
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/60cf0fd980c226d2
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/60e999879f8dcb1
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/61c249217cd74cff
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/61c6fd3a471f4a06
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/623002241203c26b
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/6257b8a9182a0d2
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/62ab74165f7db054
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/62ae1aa6752cfe77
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/62c51c97baf05fdc
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/62c53d7c56e51e5a
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/62c672e20644f15b
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/62c8567a7296a72b
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/63b0cd917688cfdc
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/64265be764313a04
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/649c27656a975c4f
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/64b5dd366ceefc0d
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/6512836f769beffc
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/6588f30b5d1d856e
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/6622e0489d2c75aa
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/66de5a9959dfac08
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/679483fcfecfc02c
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/67c46eccb501a575
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/680b841dde35de21
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/6814c211e64a24a7
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/685788147a6ffe4b
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/6858ff4694691d18
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/6865b5f2c76add41
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/686edae0afe1ab13
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/68bfc86e93911d8a
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/68ed66e5f5493110
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/6939924ca3ec8a57
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/6951364d854c5eaa
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/695d5bc238cb4b4
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/6998415f81e36f49
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/69ec8d43b660dd46
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/6a0e053aea20fa2c
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/6a2042b68653590b
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/6afd3d2137282872
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/6b07ab729d3bc956
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/6bd04b5dd77a320f
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/6c297586d202f109
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/6c3bc8d8f1710c78
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/6c4c62c245e11547
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/6c7fc958c8938fdd
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/6cc23bedc5bb12e4
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/6d31e7794b73c35
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/6d40cd7bca279e16
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/6ddd42c150798f16
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/6e79f4e2fb7e62e2
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/6f1cad2503667165
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/6fb354465643bad2
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/71041f574a40917c
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/7109190ebdfabdac
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/71a1ff315399ba32
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/71c89d4e718206af
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/72332d480aac70ae
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/72fff96f04a5494e
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/733774167467b946
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/736bd13fb0b5699a
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/737588c0f715fe8c
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/73c3a5f624c35554
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/73fa0ba481238ee1
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/752d344fb41506c3
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/753259c9d81a6ace
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/755d3c3e336ce31
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/75841994be06f4d8
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/75e6c4f80382dfd4
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/76222df27542131a
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/76c32b2e908b2598
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/76c438afc7d5ca90
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/76c4d0a09e42fd17
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/76f225fbdb912ac0
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/77129650ce676d47
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/77a43462e48cc381
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/788654df64149c54
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/78d07d6c4e182161
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/78ed95a66c335914
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/791a2ad24eb1cda5
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/794f6cf92dbd9464
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/79625071b1aa68e1
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/7ad48657d7903f23
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/7adedcc6a26fa1cf
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/7af18ba888b8d8e6
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/7b35abc8de1afe51
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/7b523c29016e1d3b
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/7b93835cc8d63ce5
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/7bb6ad3ccde4cfa5
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/7be575df1216437e
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/7c30b2ef26c0621d
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/7c5bc17ad10bf34e
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/7c81d4fc4cf2ecc3
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/7c979ef93a40cb92
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/7d02cc2e2fa89687
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/7d0b8cbbe2859563
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/7d618b86ab7cbf46
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/7dad95f2f714d613
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/7de180de37ede5bd
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/7e1068a00ab8d89a
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/7e2ee3e31d918c21
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/7e342625a72c7bbb
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/7e63085161d20f09
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/7e7964e56b19ae4e
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/7ebc4d3992ff1007
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/7ef3833f171cf058
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/7f113015b5dc5255
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/7f601c24452496c9
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/7f898ec11a4ffc03
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/7f976df9a932883d
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/7fbd02d095bed02a
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/7fd686be86faf992
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/7fd6d67a3c17c1bf
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/7fdb4deb4be42fd
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/80348e3e1a1521e7
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/806cc7a976dbae77
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/808bc262b9313422
--rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/80e75c923ab5ecdb
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/812b0cddc67777b8
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/81311b4f2a2803c7
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/82172047f4f50b4
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/822250ac3f58061f
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/82b1783aa772d05d
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/82f9bdf565cead09
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/8329fdff4a814e94
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/83bd3de556909e3f
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/83d23c8830d5bb6e
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/83e5804b806a93f0
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/848c7ebc7561be3a
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/84e2688a1a24a7c0
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/84f52d5455442723
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/85a48fb0de0f33dc
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/85bba16ab34ede23
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/85e3af34e7e5997a
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/860c0615c24d61a4
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/86154a8122ed1889
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/861ef870e3d3c010
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/867c9f8ec99e901d
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/86a2815865c2926b
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/86e1923104f6531a
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/871ac4cd3ba887f7
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/87224888a1f5888
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/8730dc980f227534
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/8772ad5e62c849b8
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/8773df95f5fad110
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/87754ae15b13d585
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/87a2884d3d17e90d
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/87cd7633a7d2926
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/87d34a24c8bf0199
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/87f1d526b2e6a075
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/88927103a6a41931
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/88b869adb67962ba
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/894ad975626f566f
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/895c0d3c2937b3c9
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/8984e8b228a6d560
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/8a0f92620f7ce048
--rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/8a1512351c9e8f10
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/8ad53c5ebcb46e1e
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/8af763901d38b59a
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/8b273f31661ff1bc
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/8b2cbd7490928c33
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/8b55f3a25c6a0845
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/8b62a8b834cd6d70
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/8b70961732135e2d
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/8bea97e4ec1e0dc2
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/8c43e91097a5282a
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/8c8353e8887920bb
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/8ca2029fcdf7af36
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/8cb0a9bc2402dbe1
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/8cb71b11bed1e482
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/8d0543a618a5c8
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/8d2ecb685ec1c849
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/8d34039cb713ba48
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/8d71ac7643a5c6d4
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/8e18e0c9431ab589
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/8e4922e30eb05dc4
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/8e51121e8281c050
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/8eb87971b8bba1dd
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/8ef11f30a7fafcd6
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/8f342dfec8ee1700
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/8f44bb36ed1a2334
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/8f5bdb79cc4fc9d0
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/8f67c507f3fd049a
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/8fc33819786847e3
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/903fab6c2ec3b1b9
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/90433578d713ad5e
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/906fa32d23caf0b5
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/90ee21f13c49dd84
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/912d7f391ded0ed0
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/913abcc26e015800
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/9166cac753a0189d
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/918a0ba94cf55549
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/91dcca061920701
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/91ef348f2ff55a75
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/92514647a23e72e1
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/92a81931f41c719d
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/92c5ce7d3027d726
--rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/939d76ea40d18b03
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/93d76f78f34b59bf
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/9496fce63f3af335
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/949af70db17e71dd
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/94d4fd3525cc2d6
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/95192a8b82446905
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/95b2b9bf58e4b39d
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/95e8aade13a56ff2
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/960c31426918b84c
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/96130cbf7268ccf7
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/96131ae533d9661c
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/96218c3ea14e2484
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/96f1c60073c60ce6
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/9701399817288b5
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/97196bdcb0c2a308
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/972c333ce8fbfbf9
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/9805cf918bf34771
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/987249790d2171b1
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/987d3a341866cd3c
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/9896576d204e2bc3
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/98f29e6ae120180
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/99378d9ea0f1400b
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/9950b40828cbddc4
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/99940ae004391246
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/9a5ab5f55dafdf62
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/9a64d39865442c9
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/9ac31c2887e119c0
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/9ad544961783256d
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/9ae8fd9a96128eab
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/9af028685efc6f40
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/9b28dbd0854dc094
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/9bc0d90ac25f5ad1
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/9c4b50b70a8f568d
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/9c60329009619de4
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/9c6632fb65e50f76
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/9c873bcfaca7e2aa
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/9cb047f45596ce7a
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/9ce171fb86ed1e31
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/9d35e1915c2fdf0c
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/9d502be36994eb64
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/9d994c6f7246d9a7
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/9df3eaab0b4031a7
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/9e21e7741397e2a7
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/9e305a9b3eaa3958
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/9e8b08a9b661107c
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/9ebc27f3bd595143
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/9eed9a33f35ca54c
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/9ef8852da9807812
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/9f4d70c051034eb0
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/9f767739ef4066cc
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/9f7ec4c97b9e2645
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/a005e4afeac4a5cf
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/a07aed392da2c9f9
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/a07ca35e233e2600
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/a0c6d2059241e8b
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/a0ef892e8685877
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/a114c323377ae794
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/a13116c63c9c6187
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/a15651622836751c
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/a179da658be572c6
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/a17e191ec50ca070
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/a1cb41579910fb3c
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/a1f065f05b6fc45c
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/a1f16e7afad04eff
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/a224da8e066f14fc
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/a249521518b63c1
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/a262e10617cd7dd9
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/a2990702b35d4c6c
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/a2a25f936b1056c1
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/a33b798bc8cbab1c
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/a3f7f95e4dfe5412
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/a42e0eea43407e18
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/a4b29d316a626d8b
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/a4b9a4d8f01bb894
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/a4f124e3ee24c43a
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/a5024437b6f7ddd8
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/a53b88c07d095afb
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/a5675a24040a4180
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/a58e9b96ea251262
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/a5ffd3ce34c5fe33
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/a66a6ff42eeaae24
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/a69c07879edaf0ab
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/a712bd264b29522d
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/a724b32c8f1539ed
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/a7382e686df814f8
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/a763c8fde74e709b
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/a78d77c91a97e61b
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/a79463aa749d0c78
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/a7d591a2034beec9
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/a7d9b740ef1049b0
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/a8374b1bdac60813
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/a862f114e49490f5
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/a8cf7b40841d38e0
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/a8dd0377bb71b084
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/a8f1d2b40e2af2d
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/a96c5e29ffb89827
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/a982b74f9076d381
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/a98b0c2e91b941b0
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/a99db77f2a0939be
--rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/a9cfac07223df808
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/a9f5487cbc8d1572
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/a9f800497198c42b
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/a9f9af70b63ee3b1
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/aa31b384af487060
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/aaa8fce49c785adb
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/aae2de8f0b98e7e1
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/ab21780484f8e923
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/ab58c1a29f845321
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/ac2d078521169042
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/ac3e98cba712211e
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/ac9f1d0af8a12f6f
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/aca4c35f72a1bea6
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/ad1b1bacaa6fa54b
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/ad4ceebf4a083af5
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/adbe530919bb83c8
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/adc364c3c117ddb8
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/adec3e88f8a4a36
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/ae3e90b1bf901da3
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/ae40e142406f563c
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/ae7d990f7d0c70f
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/ae920c12de7cba3c
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/aef34db11f5c85e4
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/afea49db0bcfe8bf
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/b063d76bdac503f7
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/b08b21dc084ad711
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/b122574866dd0b45
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/b12d6fe401a6bfc1
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/b14325a31a79061d
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/b149005514edb45b
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/b17c81391ac1ae94
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/b1cd7f505f0f4f5f
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/b20a824fe8702d03
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/b240524a23a4c3e1
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/b27ed6e92464ee92
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/b294674382790c16
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/b2af5b21b75e0929
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/b2f11488894376a1
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/b32c2d46281fdaa8
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/b32cb5995e14c01a
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/b3cd83e0c32d8b70
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/b415d1d6ee14aad2
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/b4b29b824e1985df
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/b4b92f3d45f5fed
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/b50b01dd9b842e20
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/b58ef8916d45f14
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/b5909a4cfec00b67
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/b60aa8912277f286
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/b62aa9e97e2d409a
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/b65d3396156f98cb
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/b65e176b99ffe7e1
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/b66b6f857102bf0c
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/b6ac8e9c40520a40
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/b6b271f76addcd9
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/b6f1cbb52cb8310a
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/b70ac909b5f7c059
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/b715406779f810ad
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/b71cdee6fb53df29
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/b77e7bfc32e2459e
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/b79840a253e86c81
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/b7a94e4209ae12bb
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/b7f88a6d7ed5b892
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/b819b97186696869
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/b86c8a51807226af
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/b88de43c49b9721c
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/b8eb0d0ac0916e81
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/b96464de29dd22a4
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/b9c7de9dbfa7ddcb
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/ba13343e362fbcfc
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/ba589e51a85315cb
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/ba86d712c644e9da
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/baa048c0cb6b07e7
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/baba752afc051ad2
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/bb141f48565961df
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/bc5e8e7c060300d7
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/bc850aa9fc749874
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/bcbdd7f3c25540e0
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/bcc3d75a8519852a
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/bd72dbb36688c50d
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/be1bf775fa685dcb
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/be85d2cd47b6adbd
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/be8c9207429c6462
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/bede0878f1843a4
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/bf63bfbf7aabc8d0
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/bf63ccabbc916884
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/bfa3623d9a893800
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/bff4aec8ab026e14
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/c00887a8d121659e
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/c01c3165fcefa971
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/c04a38e7d5cea8c7
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/c07c8d8e525338d9
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/c0a88c023b6d9f56
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/c0eb5f283928b7d4
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/c1d8523e76d569f9
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/c2c26ce21aae0787
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/c30dce4e73e5b5b1
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/c3287a217ac864f8
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/c34625edb2b7eb
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/c39767e52957dea5
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/c3e00433d832e8c8
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/c4236e6f6a15a176
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/c47e385879c9fda7
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/c511a9b7270a02b3
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/c53c18394601ffc6
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/c64796230452243
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/c70b327b0fd76238
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/c7381efc483ca56
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/c745d35935d9e06
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/c79429e511d94722
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/c7973c123a5b85b0
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/c7d9ba4de659c61d
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/c7e256d0bf253e32
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/c7f8d6bde299a524
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/c813bb215ec3f5f5
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/c8af8fe37594f411
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/c8c37de6b1eb99d9
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/c8fdff0ea0a71bc8
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/c947484ae7e9fc42
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/c94f8006937cb41d
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/c967488ad3c98baf
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/ca0776a90f270a5c
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/ca0bf4c295de9c30
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/ca2ef05cea5ec6cd
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/ca34efa0c983bc2b
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/ca523b90891d7183
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/cacfcaf580f08c33
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/cadf08ddbd58f2bc
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/cb5a02d5536df67d
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/cbadbeaefc6eefdd
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/cc078b1db724fe6c
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/cc3eabbcf0ce048c
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/cc6f1c71d0e39213
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/cc867a72adcdb19
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/cca4cb0d46e949b3
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/cce3f903e562037f
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/cd2d23d26fd24395
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/cd3ad9c8e74138f3
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/cda89d175557a6b3
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/cdd708944850438
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/ce1161a02da2f5b1
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/ce5c81ab05d05aab
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/ce7d2a4a2e19a107
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/cedfd832f44e2051
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/cf291a3dc74291e4
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/d0385bb227b8ca5a
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/d064cbdcc6a8cbea
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/d0cfd3eda0bc8c5f
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/d0e9a2507295a9ba
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/d13a7296fa488f04
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/d14be06feeee3537
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/d208f937406b0cee
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/d2581dfe62ab60bf
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/d30036136d56a2fe
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/d3036e4d3aff5a15
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/d31594175fc8016f
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/d322db07cbbe20cb
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/d33fb6e0d7e1564c
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/d39632aab7b1a317
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/d3bc7e8fd8b92d0
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/d3bfcd34b8f155e3
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/d3d4f0563171e8b1
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/d425c2a663059cba
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/d427f97ea01ae293
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/d44a17cf607e96d9
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/d4519685a8b597ad
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/d4597249eb4ea3d5
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/d46df94d7f637b62
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/d4d66fa96050af1e
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/d5ac310d20e30cc6
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/d5f593c0675d43d
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/d68106b55925249a
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/d695fe834826aa11
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/d6a85d05bb2fe526
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/d6a949342405cb76
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/d6ae0bcf9b7a23a6
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/d6c6b8270f1c70de
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/d7364f16d06af9f8
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/d755d7cdab68b3ce
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/d80c7c3cf692986c
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/d86d9f269257b197
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/d8fc1d75fb83272
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/d917d9bd1c0b24a
--rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/d947f1e4a66b1bbf
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/d9b1483ad5a8ae6e
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/d9d1ac6c76c70f8e
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/d9d9b4d0564e125b
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/da7cb0cccc482f85
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/dab437dcb78e3074
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/db145ca3c1b673d6
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/db2c94a696ac6feb
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/db2fb600002683c4
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/db4d138a8f56bfdd
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/db7f9df6d34c8b68
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/dba6a7ba7076e786
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/dc05d3bf9b33f1ec
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/dc078c37d4cc1c9d
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/dc2618b4f6c9f605
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/dc483236155a8f0
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/dd6b0739feba3940
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/dd7ae84707dc45a8
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/ddd18a12a0a05c82
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/ddf7afd3542c7208
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/de1feecc7d15c9cd
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/deef703264fd5f39
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/defb57087b96f58b
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/df32047279300278
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/dff0f2c145e8cc6c
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/e09f80084172fad4
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/e0ec0ae5c91d615b
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/e0f110ead3071d66
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/e0f137b84f4d088b
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/e11758eb3803cf7e
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/e16cbf6b775cb84a
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/e17fd7c4b57dbf4f
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/e1cb6eb67afb1f40
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/e1edb0a9ce567202
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/e24382470968e6d1
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/e2632d65bd5e661b
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/e2935685a344e8f8
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/e354b9ef8339b77d
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/e3651748ccc51771
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/e37162d1bcb66197
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/e399746065cc818d
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/e3c21bc8fa99728b
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/e3c9f336c292a872
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/e3ee426cc5a942a0
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/e4a7c541627a46b4
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/e4c9acc3d8a8834c
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/e53631ae62978f3a
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/e53752cfa1c25b43
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/e558bddb3a435082
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/e56973fae9ab5fa4
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/e581d4df9163c98
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/e5ef2b0b99379ca1
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/e615d95e487ad20d
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/e699e2b298f72fd2
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/e74ce2e7a295dae9
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/e757c8e77f4179f8
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/e7690243598eb849
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/e77879a83227bae1
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/e7d3cdd0e495a810
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/e7e277320c964b0b
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/e80421723aa6c581
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/e80479a3d341ce17
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/e815c8fec51eacae
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/e86d198dae010b76
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/e87992850c354804
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/e8d641b764eb9955
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/e92cb34e0b6be858
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/e94a1a0424418aef
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/e9d2b58de83c56b5
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/ea53938047df63ea
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/eac31cc3f51b34c3
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/eb30950806c6e76b
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/eb455111ae611672
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/eb67fd5323a7bfa3
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/eb68eb567a5c9489
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/eb84d06e79b530c1
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/ebeaf2d910a2bf14
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/ec15b18cce7c7f93
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/ec432d593c8e080e
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/ec91f5bb75672781
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/ed2ad083fd7a464d
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/eda7689b56d5ca75
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/edad99584e243645
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/edff547eab75854f
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/ee142d7d44e3ca0f
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/ee62927e127af803
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/ee706825f5cb2471
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/ee83dfdc98fd31
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/ee86d6744943ee65
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/ee9ca0adf422e0fe
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/eeb98d77b2ddab4d
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/eec26bd67e882958
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/eecf1e1c013a68d3
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/eeff43067fddc7f8
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/ef703e8534d011ea
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/efab9fc01638867f
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/efb55b5010b2b4af
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/f0642e827f65a991
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/f066682feeb35af
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/f0d584f460b43a21
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/f0f4bd8876a2945c
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/f1936ccc8d9e7a24
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/f1ab41c745419b46
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/f214a7ef751ff93b
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/f2480c933c67bb5b
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/f24cf4f9b838fbe0
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/f2cb348bd66bb316
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/f2ce9d32630ae5d8
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/f31cff72f6f5610
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/f377626ff23f2d0d
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/f3bb6d485c9ca824
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/f3caccc869047be3
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/f3f5e8552d7c910c
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/f4b765908c06e80b
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/f4e266ff68e3cc3f
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/f5c4d27d21b73abf
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/f5f36642fa6eef91
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/f5f609b1c249b643
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/f5ff2787c9bb8668
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/f6394a4411be7eb0
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/f64f7fe355a6fcdb
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/f681e0692d7050f5
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/f697116f54fdc91d
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/f6a60f68c7df57cd
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/f6d55e42907566fe
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/f742b4c0dfa9da49
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/f75058cfb87b7bc0
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/f75db402fa9b6682
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/f803726bd37ffc59
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/f826bcbb252554b0
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/f8835087d3e668b0
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/f8ae247af44997b4
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/f908177871cbf802
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/f963a4801c8e6c21
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/f9f301b331ca704
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/fa1b0ed3130a24bb
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/fa4835115bbe7bf6
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/faa75f0938f6e629
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/fb26185ea423ac95
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/fb422b67919c3895
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/fbae13fa95cf583c
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/fbc1eaeb8ff35f42
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/fbd86b16e65f7303
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/fc0e0bcf9ce7a23f
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/fc128a2931d2248d
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/fc5477769c08a7b7
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/fcf4af13ee1e065
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/fcfe22afb8ae30d3
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/fd5255411ec5ae3
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/fdd06e548c28204a
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/fdd41663e4f20a53
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/fdedb9fdf4284318
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/fe1df057884166ba
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/fe29a04bf7dec162
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/fe5e1f26a8e8e612
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/fe746afdc102de8
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/fe7ec8ca7c77d8df
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/fe7f589cc82dfb18
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/fe99ec62263d0e7f
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/fee51681fb9e2528
--rw-r--r--   0        0        0    13041 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/fef5cf3f2d9c1da8
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/ff09a1e8f59497ac
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/ff1733d526881e8f
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/ff709a6b44dcd447
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/ffb6dc840996c0d1
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/ffc8a84c914d1869
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 ddqa-0.0.1/.ruff_cache/content/fffbdb408adee14e
--rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 ddqa-0.0.1/app/pyoxidizer.bzl
--rw-r--r--   0        0        0     3143 2020-02-02 00:00:00.000000 ddqa-0.0.1/docs/index.md
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 ddqa-0.0.1/docs/install.md
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 ddqa-0.0.1/docs/.snippets/abbrs.txt
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 ddqa-0.0.1/docs/.snippets/links.txt
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 ddqa-0.0.1/docs/assets/css/custom.css
--rw-r--r--   0        0        0    40436 2020-02-02 00:00:00.000000 ddqa-0.0.1/docs/assets/images/favicon.ico
--rw-r--r--   0        0        0     3934 2020-02-02 00:00:00.000000 ddqa-0.0.1/docs/assets/images/logo.svg
--rw-r--r--   0        0        0     3018 2020-02-02 00:00:00.000000 ddqa-0.0.1/docs/config/repo.md
--rw-r--r--   0        0        0     2294 2020-02-02 00:00:00.000000 ddqa-0.0.1/docs/config/user.md
--rw-r--r--   0        0        0   193753 2020-02-02 00:00:00.000000 ddqa-0.0.1/screenshots/config.PNG
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 ddqa-0.0.1/scripts/fix_requirements.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 ddqa-0.0.1/src/ddqa/__about__.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 ddqa-0.0.1/src/ddqa/__init__.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 ddqa-0.0.1/src/ddqa/__main__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ddqa-0.0.1/src/ddqa/py.typed
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.0.1/src/ddqa/app/__init__.py
--rw-r--r--   0        0        0     6973 2020-02-02 00:00:00.000000 ddqa-0.0.1/src/ddqa/app/core.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 ddqa-0.0.1/src/ddqa/app/style.py
--rw-r--r--   0        0        0     3095 2020-02-02 00:00:00.000000 ddqa-0.0.1/src/ddqa/cli/__init__.py
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 ddqa-0.0.1/src/ddqa/cli/config/__init__.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 ddqa-0.0.1/src/ddqa/cli/config/edit.py
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 ddqa-0.0.1/src/ddqa/cli/config/explore.py
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 ddqa-0.0.1/src/ddqa/cli/config/find.py
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 ddqa-0.0.1/src/ddqa/cli/config/restore.py
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 ddqa-0.0.1/src/ddqa/cli/config/show.py
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 ddqa-0.0.1/src/ddqa/cli/create/__init__.py
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 ddqa-0.0.1/src/ddqa/cli/status/__init__.py
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 ddqa-0.0.1/src/ddqa/cli/sync/__init__.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.0.1/src/ddqa/config/__init__.py
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 ddqa-0.0.1/src/ddqa/config/constants.py
--rw-r--r--   0        0        0     2566 2020-02-02 00:00:00.000000 ddqa-0.0.1/src/ddqa/config/core.py
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 ddqa-0.0.1/src/ddqa/config/file.py
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 ddqa-0.0.1/src/ddqa/config/utils.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.0.1/src/ddqa/data/__init__.py
--rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 ddqa-0.0.1/src/ddqa/data/logo.png
--rw-r--r--   0        0        0   345099 2020-02-02 00:00:00.000000 ddqa-0.0.1/src/ddqa/data/shame.png
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.0.1/src/ddqa/models/__init__.py
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 ddqa-0.0.1/src/ddqa/models/github.py
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 ddqa-0.0.1/src/ddqa/models/jira.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.0.1/src/ddqa/models/config/__init__.py
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 ddqa-0.0.1/src/ddqa/models/config/app.py
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 ddqa-0.0.1/src/ddqa/models/config/auth.py
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 ddqa-0.0.1/src/ddqa/models/config/repo.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 ddqa-0.0.1/src/ddqa/models/config/team.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.0.1/src/ddqa/screens/__init__.py
--rw-r--r--   0        0        0     7522 2020-02-02 00:00:00.000000 ddqa-0.0.1/src/ddqa/screens/configure.py
--rw-r--r--   0        0        0    14891 2020-02-02 00:00:00.000000 ddqa-0.0.1/src/ddqa/screens/create.py
--rw-r--r--   0        0        0    17398 2020-02-02 00:00:00.000000 ddqa-0.0.1/src/ddqa/screens/status.py
--rw-r--r--   0        0        0     4094 2020-02-02 00:00:00.000000 ddqa-0.0.1/src/ddqa/screens/sync.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 ddqa-0.0.1/src/ddqa/utils/__init__.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 ddqa-0.0.1/src/ddqa/utils/ci.py
--rw-r--r--   0        0        0    25498 2020-02-02 00:00:00.000000 ddqa-0.0.1/src/ddqa/utils/clipboard.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 ddqa-0.0.1/src/ddqa/utils/errors.py
--rw-r--r--   0        0        0     2562 2020-02-02 00:00:00.000000 ddqa-0.0.1/src/ddqa/utils/fs.py
--rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 ddqa-0.0.1/src/ddqa/utils/git.py
--rw-r--r--   0        0        0     9054 2020-02-02 00:00:00.000000 ddqa-0.0.1/src/ddqa/utils/github.py
--rw-r--r--   0        0        0    11019 2020-02-02 00:00:00.000000 ddqa-0.0.1/src/ddqa/utils/jira.py
--rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 ddqa-0.0.1/src/ddqa/utils/network.py
--rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 ddqa-0.0.1/src/ddqa/utils/structures.py
--rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 ddqa-0.0.1/src/ddqa/utils/time.py
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 ddqa-0.0.1/src/ddqa/utils/toml.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 ddqa-0.0.1/src/ddqa/utils/widgets.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.0.1/src/ddqa/widgets/__init__.py
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 ddqa-0.0.1/src/ddqa/widgets/input.py
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 ddqa-0.0.1/src/ddqa/widgets/layout.py
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 ddqa-0.0.1/src/ddqa/widgets/static.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 ddqa-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0     5132 2020-02-02 00:00:00.000000 ddqa-0.0.1/tests/conftest.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.0.1/tests/cli/__init__.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.0.1/tests/cli/config/__init__.py
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 ddqa-0.0.1/tests/cli/config/test_edit.py
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 ddqa-0.0.1/tests/cli/config/test_explore.py
--rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 ddqa-0.0.1/tests/cli/config/test_find.py
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 ddqa-0.0.1/tests/cli/config/test_restore.py
--rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 ddqa-0.0.1/tests/cli/config/test_show.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.0.1/tests/cli/create/__init__.py
--rw-r--r--   0        0        0     3575 2020-02-02 00:00:00.000000 ddqa-0.0.1/tests/cli/create/test_create.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.0.1/tests/cli/status/__init__.py
--rw-r--r--   0        0        0     3515 2020-02-02 00:00:00.000000 ddqa-0.0.1/tests/cli/status/test_status.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.0.1/tests/cli/sync/__init__.py
--rw-r--r--   0        0        0     3435 2020-02-02 00:00:00.000000 ddqa-0.0.1/tests/cli/sync/test_sync.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.0.1/tests/helpers/__init__.py
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 ddqa-0.0.1/tests/helpers/api.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.0.1/tests/screens/__init__.py
--rw-r--r--   0        0        0    23170 2020-02-02 00:00:00.000000 ddqa-0.0.1/tests/screens/test_configure.py
--rw-r--r--   0        0        0    34653 2020-02-02 00:00:00.000000 ddqa-0.0.1/tests/screens/test_create.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.0.1/tests/screens/test_status.py
--rw-r--r--   0        0        0     7905 2020-02-02 00:00:00.000000 ddqa-0.0.1/tests/screens/test_sync.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 ddqa-0.0.1/tests/utils/__init__.py
--rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 ddqa-0.0.1/tests/utils/test_fs.py
--rw-r--r--   0        0        0     2476 2020-02-02 00:00:00.000000 ddqa-0.0.1/tests/utils/test_git.py
--rw-r--r--   0        0        0    22414 2020-02-02 00:00:00.000000 ddqa-0.0.1/tests/utils/test_github.py
--rw-r--r--   0        0        0    28668 2020-02-02 00:00:00.000000 ddqa-0.0.1/tests/utils/test_jira.py
--rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 ddqa-0.0.1/tests/utils/test_structures.py
--rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 ddqa-0.0.1/tests/utils/test_time.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 ddqa-0.0.1/.gitignore
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 ddqa-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 ddqa-0.0.1/README.md
--rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 ddqa-0.0.1/hatch.toml
--rw-r--r--   0        0        0     3117 2020-02-02 00:00:00.000000 ddqa-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3720 2020-02-02 00:00:00.000000 ddqa-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 ddqa-0.1.0/.gitattributes
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 ddqa-0.1.0/.linkcheckerrc
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 ddqa-0.1.0/HISTORY.md
+-rw-r--r--   0        0        0     3192 2020-02-02 00:00:00.000000 ddqa-0.1.0/mkdocs.yml
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 ddqa-0.1.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     4336 2020-02-02 00:00:00.000000 ddqa-0.1.0/.github/workflows/build.yml
+-rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 ddqa-0.1.0/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 ddqa-0.1.0/.github/workflows/publish-docs.yml
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 ddqa-0.1.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 ddqa-0.1.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0     2548 2020-02-02 00:00:00.000000 ddqa-0.1.0/app/pyoxidizer.bzl
+-rw-r--r--   0        0        0     3143 2020-02-02 00:00:00.000000 ddqa-0.1.0/docs/index.md
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 ddqa-0.1.0/docs/install.md
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 ddqa-0.1.0/docs/.snippets/abbrs.txt
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 ddqa-0.1.0/docs/.snippets/links.txt
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 ddqa-0.1.0/docs/assets/css/custom.css
+-rw-r--r--   0        0        0    40436 2020-02-02 00:00:00.000000 ddqa-0.1.0/docs/assets/images/favicon.ico
+-rw-r--r--   0        0        0     3934 2020-02-02 00:00:00.000000 ddqa-0.1.0/docs/assets/images/logo.svg
+-rw-r--r--   0        0        0     3018 2020-02-02 00:00:00.000000 ddqa-0.1.0/docs/config/repo.md
+-rw-r--r--   0        0        0     2294 2020-02-02 00:00:00.000000 ddqa-0.1.0/docs/config/user.md
+-rw-r--r--   0        0        0   193753 2020-02-02 00:00:00.000000 ddqa-0.1.0/screenshots/config.PNG
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/__init__.py
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/__main__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/py.typed
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/app/__init__.py
+-rw-r--r--   0        0        0     6606 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/app/core.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/app/style.py
+-rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/cli/__init__.py
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/cli/config/__init__.py
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/cli/config/edit.py
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/cli/config/explore.py
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/cli/config/find.py
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/cli/config/restore.py
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/cli/config/show.py
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/cli/create/__init__.py
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/cli/status/__init__.py
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/cli/sync/__init__.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/config/__init__.py
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/config/constants.py
+-rw-r--r--   0        0        0     2566 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/config/core.py
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/config/file.py
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/config/utils.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/data/__init__.py
+-rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/data/logo.png
+-rw-r--r--   0        0        0   345099 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/data/shame.png
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/models/__init__.py
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/models/github.py
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/models/jira.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/models/config/__init__.py
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/models/config/app.py
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/models/config/auth.py
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/models/config/repo.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/models/config/team.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/screens/__init__.py
+-rw-r--r--   0        0        0     7782 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/screens/configure.py
+-rw-r--r--   0        0        0    15351 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/screens/create.py
+-rw-r--r--   0        0        0    17067 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/screens/status.py
+-rw-r--r--   0        0        0     4051 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/screens/sync.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/utils/__init__.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/utils/ci.py
+-rw-r--r--   0        0        0    25498 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/utils/clipboard.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/utils/errors.py
+-rw-r--r--   0        0        0     2562 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/utils/fs.py
+-rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/utils/git.py
+-rw-r--r--   0        0        0     9054 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/utils/github.py
+-rw-r--r--   0        0        0    11019 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/utils/jira.py
+-rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/utils/network.py
+-rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/utils/structures.py
+-rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/utils/time.py
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/utils/toml.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/utils/widgets.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/widgets/__init__.py
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/widgets/input.py
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/widgets/layout.py
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 ddqa-0.1.0/src/ddqa/widgets/static.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     5132 2020-02-02 00:00:00.000000 ddqa-0.1.0/tests/conftest.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.1.0/tests/cli/__init__.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.1.0/tests/cli/config/__init__.py
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 ddqa-0.1.0/tests/cli/config/test_edit.py
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 ddqa-0.1.0/tests/cli/config/test_explore.py
+-rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 ddqa-0.1.0/tests/cli/config/test_find.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 ddqa-0.1.0/tests/cli/config/test_restore.py
+-rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 ddqa-0.1.0/tests/cli/config/test_show.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.1.0/tests/cli/create/__init__.py
+-rw-r--r--   0        0        0     3575 2020-02-02 00:00:00.000000 ddqa-0.1.0/tests/cli/create/test_create.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.1.0/tests/cli/status/__init__.py
+-rw-r--r--   0        0        0     3515 2020-02-02 00:00:00.000000 ddqa-0.1.0/tests/cli/status/test_status.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.1.0/tests/cli/sync/__init__.py
+-rw-r--r--   0        0        0     3435 2020-02-02 00:00:00.000000 ddqa-0.1.0/tests/cli/sync/test_sync.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.1.0/tests/helpers/__init__.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 ddqa-0.1.0/tests/helpers/api.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.1.0/tests/screens/__init__.py
+-rw-r--r--   0        0        0    23170 2020-02-02 00:00:00.000000 ddqa-0.1.0/tests/screens/test_configure.py
+-rw-r--r--   0        0        0    34644 2020-02-02 00:00:00.000000 ddqa-0.1.0/tests/screens/test_create.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.1.0/tests/screens/test_status.py
+-rw-r--r--   0        0        0     7905 2020-02-02 00:00:00.000000 ddqa-0.1.0/tests/screens/test_sync.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 ddqa-0.1.0/tests/utils/__init__.py
+-rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 ddqa-0.1.0/tests/utils/test_fs.py
+-rw-r--r--   0        0        0     2476 2020-02-02 00:00:00.000000 ddqa-0.1.0/tests/utils/test_git.py
+-rw-r--r--   0        0        0    22414 2020-02-02 00:00:00.000000 ddqa-0.1.0/tests/utils/test_github.py
+-rw-r--r--   0        0        0    28668 2020-02-02 00:00:00.000000 ddqa-0.1.0/tests/utils/test_jira.py
+-rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 ddqa-0.1.0/tests/utils/test_structures.py
+-rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 ddqa-0.1.0/tests/utils/test_time.py
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 ddqa-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ddqa-0.1.0/LICENSE.txt
+-rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 ddqa-0.1.0/README.md
+-rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 ddqa-0.1.0/hatch.toml
+-rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 ddqa-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3712 2020-02-02 00:00:00.000000 ddqa-0.1.0/PKG-INFO
```

### Comparing `ddqa-0.0.1/mkdocs.yml` & `ddqa-0.1.0/mkdocs.yml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 site_name: Datadog QA
 site_description: Datadog's QA manager for releases of GitHub repositories
 site_author: Datadog
 site_url: https://datadoghq.dev/ddqa/
 repo_name: datadog/ddqa
 repo_url: https://github.com/DataDog/ddqa
 edit_uri: blob/master/docs
-copyright: 'Copyright &copy; Datadog, Inc. 2017-present'
+copyright: 'Copyright &copy; Datadog, Inc. 2023-present'
 
 docs_dir: docs
 site_dir: site
 theme:
   name: material
   language: en
   favicon: assets/images/favicon.ico
```

### Comparing `ddqa-0.0.1/.github/workflows/docs.yml` & `ddqa-0.1.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `ddqa-0.0.1/.github/workflows/publish-docs.yml` & `ddqa-0.1.0/.github/workflows/publish-docs.yml`

 * *Files identical despite different names*

### Comparing `ddqa-0.0.1/.github/workflows/test.yml` & `ddqa-0.1.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `ddqa-0.0.1/app/pyoxidizer.bzl` & `ddqa-0.1.0/app/pyoxidizer.bzl`

 * *Files 20% similar despite different names*

```diff
@@ -1,54 +1,64 @@
-# SPDX-FileCopyrightText: 2023-present Datadog, Inc. <dev@datadoghq.com>
-#
-# SPDX-License-Identifier: MIT
-def make_exe():
-    # https://gregoryszorc.com/docs/pyoxidizer/main/pyoxidizer_config_type_python_distribution.html#starlark_pyoxidizer.default_python_distribution
-    dist = default_python_distribution(python_version = "3.10", flavor="standalone")
-
-    # https://gregoryszorc.com/docs/pyoxidizer/main/pyoxidizer_config_type_python_packaging_policy.html#starlark_pyoxidizer.PythonPackagingPolicy
-    policy = dist.make_python_packaging_policy()
-    policy.resources_location = "in-memory"
-    policy.resources_location_fallback = "filesystem-relative:site-packages"
-
-    # https://gregoryszorc.com/docs/pyoxidizer/main/pyoxidizer_config_type_python_interpreter_config.html#starlark_pyoxidizer.PythonInterpreterConfig
-    python_config = dist.make_python_interpreter_config()
-    python_config.run_module = "ddqa"
-    python_config.sys_frozen = True
-
-    # https://gregoryszorc.com/docs/pyoxidizer/main/pyoxidizer_config_type_python_executable.html#starlark_pyoxidizer.PythonExecutable
-    exe = dist.to_python_executable(
-        name="ddqa",
-        packaging_policy=policy,
-        config=python_config,
-    )
-    exe.add_python_resources(exe.pip_download(["-r", "requirements.txt", "--no-deps"]))
-
-    return exe
-
-def make_embedded_resources(exe):
-    return exe.to_embedded_resources()
-
-def make_install(exe):
-    # https://gregoryszorc.com/docs/pyoxidizer/main/tugger_starlark_type_file_manifest.html#starlark_tugger.FileManifest
-    files = FileManifest()
-
-    # https://gregoryszorc.com/docs/pyoxidizer/main/pyoxidizer_config_tugger_extensions.html#filemanifest-add-python-resource
-    files.add_python_resource(".", exe)
-
-    return files
-
-def make_msi(exe):
-    # https://gregoryszorc.com/docs/pyoxidizer/main/tugger_starlark_type_wix_msi_builder.html#starlark_tugger.WiXMSIBuilder
-    return exe.to_wix_msi_builder(
-        "ddqa",
-        "Datadog QA",
-        "1.0",
-        "Datadog, Inc.",
-    )
-
-register_target("exe", make_exe)
-register_target("resources", make_embedded_resources, depends=["exe"], default_build_script=True)
-register_target("install", make_install, depends=["exe"], default=True)
-register_target("msi_installer", make_msi, depends=["exe"])
-
-resolve_targets()
+# SPDX-FileCopyrightText: 2023-present Datadog, Inc. <dev@datadoghq.com>
+#
+# SPDX-License-Identifier: MIT
+VERSION = VARS["version"]
+
+def make_exe():
+    # https://gregoryszorc.com/docs/pyoxidizer/main/pyoxidizer_config_type_python_distribution.html#starlark_pyoxidizer.default_python_distribution
+    dist = default_python_distribution(python_version = "3.10", flavor="standalone")
+
+    # https://gregoryszorc.com/docs/pyoxidizer/main/pyoxidizer_config_type_python_packaging_policy.html#starlark_pyoxidizer.PythonPackagingPolicy
+    policy = dist.make_python_packaging_policy()
+    policy.set_resource_handling_mode("files")
+    policy.resources_location = "filesystem-relative:lib"
+
+    # https://gregoryszorc.com/docs/pyoxidizer/main/pyoxidizer_config_type_python_interpreter_config.html#starlark_pyoxidizer.PythonInterpreterConfig
+    python_config = dist.make_python_interpreter_config()
+    python_config.module_search_paths = ["$ORIGIN/lib"]
+    python_config.run_module = "ddqa"
+    python_config.sys_frozen = True
+
+    # https://gregoryszorc.com/docs/pyoxidizer/main/pyoxidizer_config_type_python_executable.html#starlark_pyoxidizer.PythonExecutable
+    exe = dist.to_python_executable(
+        name="ddqa",
+        packaging_policy=policy,
+        config=python_config,
+    )
+    exe.add_python_resources(exe.pip_download(["ddqa==" + VERSION]))
+
+    return exe
+
+def make_embedded_resources(exe):
+    return exe.to_embedded_resources()
+
+def make_install(exe):
+    # https://gregoryszorc.com/docs/pyoxidizer/main/tugger_starlark_type_file_manifest.html#starlark_tugger.FileManifest
+    files = FileManifest()
+
+    # https://gregoryszorc.com/docs/pyoxidizer/main/pyoxidizer_config_tugger_extensions.html#filemanifest-add-python-resource
+    files.add_python_resource(".", exe)
+
+    return files
+
+def make_msi(exe):
+    version = VERSION.replace(".dev", ".")
+
+    # https://gregoryszorc.com/docs/pyoxidizer/main/tugger_starlark_type_wix_msi_builder.html#starlark_tugger.WiXMSIBuilder
+    msi = exe.to_wix_msi_builder(
+        "ddqa",
+        "Datadog QA",
+        version,
+        "Datadog, Inc.",
+    )
+    msi.msi_filename = "ddqa-" + version + "-x64.msi"
+    msi.help_url = "https://datadoghq.dev/ddqa/"
+    msi.license_path = CWD + "/../LICENSE.txt"
+
+    return msi
+
+register_target("exe", make_exe)
+register_target("resources", make_embedded_resources, depends=["exe"], default_build_script=True)
+register_target("install", make_install, depends=["exe"], default=True)
+register_target("msi", make_msi, depends=["exe"])
+
+resolve_targets()
```

### Comparing `ddqa-0.0.1/docs/index.md` & `ddqa-0.1.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `ddqa-0.0.1/docs/assets/css/custom.css` & `ddqa-0.1.0/docs/assets/css/custom.css`

 * *Files identical despite different names*

### Comparing `ddqa-0.0.1/docs/assets/images/favicon.ico` & `ddqa-0.1.0/docs/assets/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `ddqa-0.0.1/docs/assets/images/logo.svg` & `ddqa-0.1.0/docs/assets/images/logo.svg`

 * *Files identical despite different names*

### Comparing `ddqa-0.0.1/docs/config/repo.md` & `ddqa-0.1.0/docs/config/repo.md`

 * *Files identical despite different names*

### Comparing `ddqa-0.0.1/docs/config/user.md` & `ddqa-0.1.0/docs/config/user.md`

 * *Files identical despite different names*

### Comparing `ddqa-0.0.1/screenshots/config.PNG` & `ddqa-0.1.0/screenshots/config.PNG`

 * *Files identical despite different names*

### Comparing `ddqa-0.0.1/src/ddqa/app/core.py` & `ddqa-0.1.0/src/ddqa/app/core.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # SPDX-FileCopyrightText: 2023-present Datadog, Inc. <dev@datadoghq.com>
 #
 # SPDX-License-Identifier: MIT
 from __future__ import annotations
 
-import asyncio
 import os
 from functools import cached_property
 from typing import TYPE_CHECKING
 
 from rich.console import Console
 from textual.app import App
 
@@ -39,17 +38,14 @@
             emoji=False,
             highlight=False,
         )
         self.config_file = config_file
         self.__cache_dir = cache_dir
         self.__queued_screens: list[tuple[str, Screen]] = []
 
-        # Hold references to long-running background tasks
-        self.__background_tasks: list[asyncio.Task] = []
-
     @property
     def config(self) -> Config:
         return self.config_file.model
 
     @cached_property
     def repo(self) -> RepoConfig:
         return self.config.repos[self.config.app.repo]
@@ -133,20 +129,14 @@
         else:
             for name, _ in self.__queued_screens:
                 await self.push_screen(name)
 
     def select_screen(self, name: str, screen: Screen) -> None:
         self.__queued_screens.append((name, screen))
 
-    def run_in_background(self, coroutine) -> None:
-        self.__background_tasks.append(asyncio.create_task(coroutine))
-
-    async def wait_for_background_tasks(self) -> None:
-        await asyncio.gather(*self.__background_tasks)
-
     def print(self, *args, **kwargs) -> None:  # noqa: A003
         self.__console.print(*args, **kwargs)
 
     def needs_syncing(self) -> bool:
         return not self.github.load_global_config(self.repo.global_config_source) or not any(
             self.github.cache_dir_team_members.iterdir()
         )
```

### Comparing `ddqa-0.0.1/src/ddqa/cli/__init__.py` & `ddqa-0.1.0/src/ddqa/cli/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 import os
 import sys
 
 import click
 
-from ddqa.__about__ import __version__
+from ddqa._version import __version__
 from ddqa.cli.config import config
 from ddqa.cli.create import create
 from ddqa.cli.status import status
 from ddqa.cli.sync import sync
 from ddqa.config.constants import AppEnvVars, ConfigEnvVars
```

### Comparing `ddqa-0.0.1/src/ddqa/cli/config/__init__.py` & `ddqa-0.1.0/src/ddqa/cli/config/__init__.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.0.1/src/ddqa/cli/config/find.py` & `ddqa-0.1.0/src/ddqa/cli/config/find.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.0.1/src/ddqa/cli/config/show.py` & `ddqa-0.1.0/src/ddqa/cli/config/show.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.0.1/src/ddqa/cli/create/__init__.py` & `ddqa-0.1.0/src/ddqa/cli/create/__init__.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.0.1/src/ddqa/cli/status/__init__.py` & `ddqa-0.1.0/src/ddqa/cli/status/__init__.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.0.1/src/ddqa/config/core.py` & `ddqa-0.1.0/src/ddqa/config/core.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.0.1/src/ddqa/config/file.py` & `ddqa-0.1.0/src/ddqa/config/file.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.0.1/src/ddqa/data/logo.png` & `ddqa-0.1.0/src/ddqa/data/logo.png`

 * *Files identical despite different names*

### Comparing `ddqa-0.0.1/src/ddqa/data/shame.png` & `ddqa-0.1.0/src/ddqa/data/shame.png`

 * *Files identical despite different names*

### Comparing `ddqa-0.0.1/src/ddqa/models/github.py` & `ddqa-0.1.0/src/ddqa/models/github.py`

 * *Files 23% similar despite different names*

```diff
@@ -20,7 +20,13 @@
     id: str  # noqa: A003
     title: str
     url: str
     user: str = ''
     body: str = ''
     labels: list[PullRequestLabel] = []
     reviewers: list[PullRequestReviewer] = []
+
+    def short_display(self) -> str:
+        return f'#{self.id}' if self.id.isdigit() else self.id[:7]
+
+    def long_display(self) -> str:
+        return f'pull request #{self.id}' if self.id.isdigit() else f'commit {self.id[:7]}'
```

### Comparing `ddqa-0.0.1/src/ddqa/models/jira.py` & `ddqa-0.1.0/src/ddqa/models/jira.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.0.1/src/ddqa/models/config/repo.py` & `ddqa-0.1.0/src/ddqa/models/config/repo.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.0.1/src/ddqa/screens/configure.py` & `ddqa-0.1.0/src/ddqa/screens/configure.py`

 * *Files 7% similar despite different names*

```diff
@@ -155,36 +155,50 @@
             self.app.config.data.setdefault('jira', {})['token'] = value
         else:
             self.app.config.data.get('jira', {}).pop('token', None)
 
 
 class ConfigurationInput(Widget):
     DEFAULT_CSS = """
+    ConfigurationInput {
+        layout: grid;
+        grid-size: 1 3;
+        grid-rows: 6fr 4fr 1fr;
+    }
+
+    #input-box {
+        height: 100%;
+        width: 100%;
+        scrollbar-gutter: stable;
+    }
+
     ConfigurationInput > Button {
         border: none;
-        margin: 1;
         width: 100%;
+        height: auto;
     }
 
     ConfigurationInput > TextLog {
-        margin: 1;
-        padding-bottom: 2;
-        height: 1fr;
+        height: 100%;
+        scrollbar-gutter: stable;
     }
     """
 
     def compose(self) -> ComposeResult:
-        yield LabeledInput(Label('Repo name:'), RepoNameInput())
-        yield LabeledInput(Label('Repo path:'), RepoPathInput())
-        yield LabeledInput(Label('GitHub user:'), GitHubUserInput())
-        yield LabeledInput(Label('GitHub token:'), GitHubTokenInput())
-        yield LabeledInput(Label('Jira email:'), JiraEmailInput())
-        yield LabeledInput(Label('Jira token:'), JiraTokenInput())
-        yield Button('Save', variant='primary', disabled=True)
+        yield Container(
+            LabeledInput(Label('Repo name:'), RepoNameInput()),
+            LabeledInput(Label('Repo path:'), RepoPathInput()),
+            LabeledInput(Label('GitHub user:'), GitHubUserInput()),
+            LabeledInput(Label('GitHub token:'), GitHubTokenInput()),
+            LabeledInput(Label('Jira email:'), JiraEmailInput()),
+            LabeledInput(Label('Jira token:'), JiraTokenInput()),
+            id='input-box',
+        )
         yield TextLog()
+        yield Button('Save', variant='primary', disabled=True)
 
     async def on_button_pressed(self, _event: Button.Pressed) -> None:
         self.app.config_file.save()
 
         with suppress(AttributeError):
             del self.app.repo
         with suppress(AttributeError):
```

### Comparing `ddqa-0.0.1/src/ddqa/screens/create.py` & `ddqa-0.1.0/src/ddqa/screens/create.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,26 +5,27 @@
 
 import typing
 
 from rich.markdown import Markdown as RichMarkdown
 from rich.markup import escape
 from textual.app import ComposeResult
 from textual.binding import Binding
-from textual.containers import Container, Horizontal, Vertical
+from textual.containers import Container, HorizontalScroll, VerticalScroll
 from textual.screen import Screen
 from textual.widgets import Button, DataTable, Header, Label, Markdown, Switch
 
 from ddqa.utils.network import ResponsiveNetworkClient
 from ddqa.utils.widgets import switch_to_widget
 from ddqa.widgets.input import LabeledSwitch
 from ddqa.widgets.layout import LabeledBox
 from ddqa.widgets.static import Placeholder
 
 if typing.TYPE_CHECKING:
     from ddqa.models.config.repo import RepoConfig
+    from ddqa.models.config.team import TeamConfig
     from ddqa.models.github import TestCandidate
 
 
 class Candidate:
     def __init__(self, candidate: TestCandidate, repo_config: RepoConfig):
         self.data = candidate
 
@@ -41,14 +42,21 @@
 
     @property
     def status_indicator(self) -> str:
         return '✓' if self.assigned else ''
 
 
 class CandidateListing(DataTable):
+    DEFAULT_CSS = """
+    CandidateListing {
+        height: 1fr;
+        max-height: 1fr;
+    }
+    """
+
     def __init__(
         self, sidebar: CandidateSidebar, previous_ref: str, current_ref: str, labels: tuple[str, ...], *args, **kwargs
     ):
         super().__init__(*args, **kwargs)
 
         self.sidebar = sidebar
         self.previous_ref = previous_ref
@@ -66,15 +74,15 @@
 
         self.add_column('_', key='status')
         self.add_column('_', key='title')
         self.show_header = False
         self.cursor_type = 'row'
         self.focus()
 
-        self.call_after_refresh(lambda: self.app.run_in_background(self.__on_mount()))
+        self.run_worker(self.__on_mount())
 
     async def __on_mount(self) -> None:
         try:
             commits = self.app.git.get_mutually_exclusive_commits(self.previous_ref, self.current_ref)
         except Exception as e:
             self.app.print(f'Failed to get commits for {self.previous_ref}..{self.current_ref}: {e}')
             self.sidebar.label.update(' error ')
@@ -93,17 +101,16 @@
                 model = await self.app.github.get_candidate(client, commit)
                 if model.id.isdigit():
                     if model.id in processed_pr_numbers:
                         ignored += 1
                         continue
 
                     processed_pr_numbers.add(model.id)
-                    self.app.print(f'Processing pull request #{model.id}')
-                else:
-                    self.app.print(f'Processing commit {model.id[:7]}')
+
+                self.app.print(f'Processing {model.long_display()}')
 
                 index = i - ignored
                 candidate = Candidate(model, self.app.repo)
                 self.candidates[index] = candidate
 
                 shown_index = str(index + 1)
                 self.sidebar.label.update(f' {shown_index} / {total - ignored} ')
@@ -140,31 +147,25 @@
         self.focus()
         display_updated = False
 
         self.app.print(f'Candidates ready for creation: {total}')
         self.sidebar.status.update('Creating...')
         async with ResponsiveNetworkClient(self.sidebar.status) as client:
             for index, candidate in self.candidates.items():
-                if candidate.data.id.isdigit():
-                    self.app.print(f'Creating issue for pull request #{candidate.data.id}')
-                else:
-                    self.app.print(f'Creating issue for commit {candidate.data.id[:7]}')
+                self.app.print(f'Creating issue for {candidate.data.long_display()}')
 
                 assignments: dict[str, str] = {}
                 for team, assigned in candidate.assignments.items():
                     if not assigned:
                         continue
 
-                    team_members = await self.app.github.get_team_members(client, self.app.repo.teams[team].github_team)
-                    team_members.discard(candidate.data.user)
-                    for reviewer in candidate.data.reviewers:
-                        team_members.discard(reviewer.name)
-
-                    assignee = secrets.choice(sorted(team_members)) if team_members else ''
-                    assignments[team] = assignee
+                    potential_assignees = await self.__get_potential_assignees(
+                        client, candidate.data, self.app.repo.teams[team]
+                    )
+                    assignments[team] = secrets.choice(sorted(potential_assignees)) if potential_assignees else ''
 
                 try:
                     created_issues = await self.app.jira.create_issues(client, candidate.data, self.labels, assignments)
                 except Exception as e:
                     self.sidebar.status.update(escape(str(e)))
                     return
 
@@ -176,25 +177,46 @@
                     result.add_row(
                         team,
                         f'[link=https://github.com/{assignee}]{assignee}[/link]' if assignee else '',
                         f'[link={issue_url}]{issue_url.rpartition("/")[2]}[/link]',
                     )
 
                 await self.app.query_one(CandidateRendering).add_assignment_result(
-                    candidate.data.id, Horizontal(result, classes='assignment-result-box'), update=not display_updated
+                    candidate.data.id,
+                    HorizontalScroll(result, classes='assignment-result-box'),
+                    update=not display_updated,
                 )
                 self.update_cell(str(index), 'status', len(created_issues), update_width=True)
 
                 if not display_updated:
                     display_updated = True
 
         self.app.print('Finished creating issues')
         self.sidebar.status.update('Finished')
         self.sidebar.button.disabled = False
 
+    async def __get_potential_assignees(
+        self, client: ResponsiveNetworkClient, candidate: TestCandidate, team: TeamConfig
+    ) -> set:
+        team_members = await self.app.github.get_team_members(client, team.github_team)
+        if not team_members:
+            return team_members
+
+        team_members.discard(candidate.user)
+        team_members.difference_update(team.exclude_members)
+        if not team_members:
+            return {candidate.user}
+
+        team_member_reviewers = {reviewer.name for reviewer in candidate.reviewers if reviewer.name in team_members}
+        if len(team_member_reviewers) == len(team_members):
+            return team_member_reviewers
+
+        team_members -= team_member_reviewers
+        return team_members
+
 
 class CandidateSidebar(LabeledBox):
     DEFAULT_CSS = """
     #sidebar-status {
         height: auto;
         border-bottom: dashed #632CA6;
     }
@@ -251,15 +273,15 @@
         if str(self.button.label) == 'Create':
             self.button.disabled = True
             self.button.label = 'Exit'
 
             for widget in self.app.query_one('#candidate-assignments').children:
                 await widget.remove()
 
-            self.app.run_in_background(self.listing.create())
+            self.run_worker(self.listing.create())
         else:
             self.app.exit()
 
 
 class CandidateRendering(LabeledBox):
     DEFAULT_CSS = """
     #candidate-info {
@@ -289,24 +311,25 @@
 
     .assignment-result-box {
         align: center middle;
     }
 
     .assignment-result {
         width: auto;
+        max-height: 1fr;
     }
     """
 
     def __init__(self) -> None:
         self.__title = Label()
         self.__labels = Label()
         self.__body = Container(Placeholder(width_factor=2.5), id='candidate-body')
         self.__body_renderings: dict[str, Markdown] = {}
-        self.__candidate_assignments = Vertical(id='candidate-assignments')
-        self.__assignment_results: dict[str, Horizontal] = {}
+        self.__candidate_assignments = VerticalScroll(id='candidate-assignments')
+        self.__assignment_results: dict[str, HorizontalScroll] = {}
 
         super().__init__(
             '',
             Container(self.__title, self.__labels, id='candidate-info'),
             self.__body,
             self.__candidate_assignments,
         )
@@ -320,35 +343,31 @@
         return self.__body
 
     @property
     def labels(self) -> Label:
         return self.__labels
 
     @property
-    def candidate_assignments(self) -> Vertical:
+    def candidate_assignments(self) -> VerticalScroll:
         return self.__candidate_assignments
 
     async def on_mount(self) -> None:
         teams = list(self.app.repo.teams)
         width = 3
         for i in range(0, len(teams), width):
             await self.candidate_assignments.mount(
-                Horizontal(
+                HorizontalScroll(
                     *[LabeledSwitch(label=team, classes='assignment-box') for team in teams[i : i + width]],
                     classes='assignment-row',
                 )
             )
 
     async def render_candidate(self, candidate: Candidate):
         data = candidate.data
-        self.label.update(
-            f' [link={data.url}]PR {data.id}[/link] '
-            if data.id.isdigit()
-            else f' [link={data.url}]Commit {data.id[:7]}[/link] '
-        )
+        self.label.update(f' [link={data.url}]{data.short_display()}[/link] ')
         self.title.update(RichMarkdown(data.title))
         self.labels.update(' '.join(f'[black on #{label.color}]{label.name}[/]' for label in data.labels))
 
         if data.id in self.__body_renderings:
             body_rendering = self.__body_renderings[data.id]
         else:
             body_rendering = Markdown(data.body)
@@ -359,15 +378,17 @@
         if data.id in self.__assignment_results:
             await switch_to_widget(self.__assignment_results[data.id], self.candidate_assignments)
         else:
             self.candidate_assignments.scroll_home(animate=False)
             for widget in self.query(LabeledSwitch).results():
                 widget.switch.value = candidate.assignments[str(widget.label.render())]
 
-    async def add_assignment_result(self, candidate_id: str, table_box: Horizontal, *, update: bool = False) -> None:
+    async def add_assignment_result(
+        self, candidate_id: str, table_box: HorizontalScroll, *, update: bool = False
+    ) -> None:
         self.__assignment_results[candidate_id] = table_box
         if update:
             await switch_to_widget(table_box, self.candidate_assignments)
 
 
 class CreateScreen(Screen):
     BINDINGS = [
@@ -425,11 +446,11 @@
         await content.render_candidate(listing.candidates[event.cursor_row])
 
     async def on_switch_changed(self, event: Switch.Changed) -> None:
         listing = self.query_one(CandidateListing)
         sidebar = self.query_one(CandidateSidebar)
 
         candidate = listing.candidates[listing.cursor_row]
-        candidate.assignments[str(event.input.parent.label.render())] = event.value
+        candidate.assignments[str(event.switch.parent.label.render())] = event.value
 
         sidebar.update_assignment_status()
         listing.update_cell(str(listing.cursor_row), 'status', candidate.status_indicator)
```

### Comparing `ddqa-0.0.1/src/ddqa/screens/status.py` & `ddqa-0.1.0/src/ddqa/screens/status.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,23 +9,22 @@
 from decimal import Decimal
 from functools import cache, cached_property
 from typing import TYPE_CHECKING
 
 from textual import events
 from textual.app import ComposeResult
 from textual.binding import Binding
-from textual.containers import Container, Horizontal, Vertical
+from textual.containers import Container, HorizontalScroll, VerticalScroll
 from textual.coordinate import Coordinate
 from textual.screen import Screen
-from textual.widgets import Button, DataTable, Header, Input, Label, Switch
+from textual.widgets import Button, DataTable, Header, Input, Label, RadioButton, RadioSet
 from textual_autocomplete import AutoComplete, Dropdown, DropdownItem
 
 from ddqa.utils.network import ResponsiveNetworkClient
 from ddqa.utils.time import format_elapsed_time
-from ddqa.widgets.input import LabeledSwitch
 from ddqa.widgets.layout import LabeledBox
 
 if TYPE_CHECKING:
     from ddqa.models.jira import JiraIssue
 
 COMPLETION_PRECISION = Decimal('0.00')
 
@@ -116,32 +115,40 @@
 def get_timedelta(dt: datetime):
     return FormattedTimeDelta(dt - datetime.now(tz=dt.tzinfo))
 
 
 class StatusChanger(LabeledBox):
     DEFAULT_CSS = """
     #status-choices {
+        border: none;
+        width: 100%;
         height: 1fr;
+        margin-top: 1;
     }
 
     #status-submission {
         border: none;
         width: 100%;
     }
     """
 
     def __init__(self, statuses: list[str]) -> None:
-        self.__switches = {status: LabeledSwitch(label=status) for status in statuses}
+        self.__radio_buttons = {status: RadioButton(label=status) for status in statuses}
+        self.__radio_set = RadioSet(*self.__radio_buttons.values(), id='status-choices')
         self.__button = Button('Move', variant='primary', id='status-submission')
 
-        super().__init__(' Status ', Vertical(*self.__switches.values(), id='status-choices'), self.__button)
+        super().__init__(' Status ', self.__radio_set, self.__button)
+
+    @property
+    def radio_set(self) -> RadioSet:
+        return self.__radio_set
 
     @property
-    def switches(self) -> dict[str, LabeledSwitch]:
-        return self.__switches
+    def radio_buttons(self) -> dict[str, RadioButton]:
+        return self.__radio_buttons
 
     @property
     def button(self) -> Button:
         return self.__button
 
 
 class StatusTable(DataTable):
@@ -171,14 +178,15 @@
         width: auto;
     }
 
     Status StatusTable {
         width: auto;
         margin-top: 1;
         scrollbar-gutter: stable;
+        max-height: 1fr;
     }
     """
 
     def __init__(self, name: str):
         self.__name = name
         self.__table = StatusTable()
 
@@ -229,16 +237,16 @@
 
     def __init__(self, statuses: Iterable[Status]):
         self.__info = Label()
 
         super().__init__(
             '',
             Container(
-                Horizontal(self.__info, id='issue-info'),
-                Horizontal(*statuses, id='statuses-box'),
+                HorizontalScroll(self.__info, id='issue-info'),
+                HorizontalScroll(*statuses, id='statuses-box'),
                 id='issues-box',
             ),
         )
 
     @property
     def info(self) -> Label:
         return self.__info
@@ -258,28 +266,28 @@
     .issue-filter {
         height: 5;
     }
     """
 
     def __init__(self):
         self.__status = Label()
-        self.__options = Vertical()
+        self.__options = VerticalScroll()
 
         super().__init__(
             '',
             Container(self.__status, id='sidebar-status'),
             Container(self.__options, id='sidebar-options'),
         )
 
     @property
     def status(self) -> Label:
         return self.__status
 
     @property
-    def options(self) -> Vertical:
+    def options(self) -> VerticalScroll:
         return self.__options
 
 
 class StatusScreen(Screen):
     BINDINGS = [
         Binding('ctrl+c', 'quit', 'Quit', show=False, priority=True),
         Binding('tab', 'focus_next', 'Focus Next', show=False),
@@ -384,15 +392,15 @@
         yield Container(
             Container(OptionsSidebar(), id='screen-status-sidebar'),
             Container(Issues(self.statuses.values()), id='screen-status-rendering'),
             id='screen-status',
         )
 
     def on_mount(self) -> None:
-        self.call_after_refresh(lambda: self.app.run_in_background(self.__on_mount()))
+        self.run_worker(self.__on_mount())
 
     async def __on_mount(self) -> None:
         issues_found = False
 
         self.sidebar.status.update('Loading...')
         async with ResponsiveNetworkClient(self.sidebar.status) as client:
             async for issue in self.app.jira.search_issues(client, self.labels):
@@ -414,34 +422,34 @@
             self.sidebar.status.update('No issues found')
             return
 
         for status in self.statuses.values():
             status.sort_issues()
 
         await self.sidebar.options.mount(
-            Horizontal(LabeledBox(' Team ', FilterAutoComplete(self.team_filter)), classes='issue-filter')
+            HorizontalScroll(LabeledBox(' Team ', FilterAutoComplete(self.team_filter)), classes='issue-filter')
         )
         await self.sidebar.options.mount(
-            Horizontal(LabeledBox(' Member ', FilterAutoComplete(self.member_filter)), classes='issue-filter')
+            HorizontalScroll(LabeledBox(' Member ', FilterAutoComplete(self.member_filter)), classes='issue-filter')
         )
-        await self.sidebar.options.mount(Horizontal(self.status_changer))
+        await self.sidebar.options.mount(HorizontalScroll(self.status_changer))
 
         self.__update_completion_status()
         self.__refocus()
 
     async def on_auto_complete_selected(self, event: AutoComplete.Selected) -> None:
         choice = str(event.item.main)
         for widget in self.query(Input).results():
-            if widget is not event.sender.input:
+            if widget is not event._sender.input:
                 widget.value = ''
 
         for status in self.statuses.values():
             status.clear_issues()
 
-        for issue in event.sender.issue_filter.issues[choice].values():
+        for issue in event._sender.issue_filter.issues[choice].values():
             self.statuses[self.get_qa_status(issue)].add_issue(issue)
 
         for status in self.statuses.values():
             status.sort_issues()
 
         self.__update_completion_status()
         self.__refocus()
@@ -460,49 +468,37 @@
         for status in self.statuses.values():
             status.sort_issues()
 
         self.__update_completion_status()
         self.__refocus()
 
     async def on_data_table_row_highlighted(self, event: DataTable.RowHighlighted) -> None:
-        if not event.sender.show_cursor:
+        if not event.data_table.show_cursor:
             return
 
-        issue_key = event.sender.get_cell_at(Coordinate(event.cursor_row, 0))
+        issue_key = event.data_table.get_cell_at(Coordinate(event.cursor_row, 0))
         issue = self.cached_issues[issue_key]
         self.issues.label.update(f' [link={self.app.jira.construct_issue_url(issue.key)}]{issue.key}[/link] ')
         self.issues.info.update(issue.summary)
 
         current_status = self.get_qa_status(issue)
-        self.status_changer.switches[current_status].switch.value = True
-
-    async def on_switch_changed(self, event: Switch.Changed) -> None:
-        if not event.value:
-            if not any(labeled_switch.switch.value for labeled_switch in self.status_changer.switches.values()):
-                self.status_changer.button.disabled = True
-
-            return
-
-        for labeled_switch in self.status_changer.switches.values():
-            if labeled_switch.switch is not event.sender:
-                labeled_switch.switch.value = False
+        self.status_changer.radio_buttons[current_status].value = True
 
+    async def on_radio_set_changed(self, event: RadioSet.Changed) -> None:
         current_issue = self.cached_issues[str(self.issues.label.render()).strip()]
-        if current_issue.assignee is not None:
-            self.status_changer.button.disabled = current_issue.assignee.id != self.current_user_id
+        current_status = self.get_qa_status(current_issue)
+        self.status_changer.button.disabled = (
+            current_issue.assignee is None
+            or current_issue.assignee.id != self.current_user_id
+            or str(event.pressed.label) == current_status
+        )
 
     async def on_button_pressed(self, _event: Button.Pressed) -> None:
         old_issue = self.cached_issues[str(self.issues.label.render()).strip()]
-        for labeled_switch in self.status_changer.switches.values():
-            if labeled_switch.switch.value:
-                selected_status = str(labeled_switch.label.render())
-                break
-        else:  # no cov
-            message = 'No status selected'
-            raise ValueError(message)
+        selected_status = str(self.status_changer.radio_set.pressed_button.label)
 
         async with ResponsiveNetworkClient(self.sidebar.status) as client:
             new_issue = await self.app.jira.update_issue_status(
                 client, old_issue, self.app.qa_statuses[self.get_team(old_issue)][selected_status]
             )
 
         self.cached_issues[new_issue.key] = new_issue
@@ -522,28 +518,27 @@
         old_status.sort_issues()
 
         new_status = self.statuses[self.get_qa_status(new_issue)]
         new_status.add_issue(new_issue)
         new_status.sort_issues()
 
         new_status.table.cursor_coordinate = Coordinate(0, 0)
-        await new_status.table.post_message(
+        new_status.table.post_message(
             events.Click(
-                sender=self.app,
                 x=0,
                 y=0,
                 delta_x=0,
                 delta_y=0,
                 button=0,
                 shift=False,
                 meta=False,
                 ctrl=False,
             )
         )
-        self.status_changer.switches[str(new_status.name)].switch.value = True
+        self.status_changer.button.disabled = True
         self.__update_completion_status()
 
     def __get_status_label(self, labels: list[str]) -> str:
         for label in labels:
             if label in self.statuses:
                 return label
```

### Comparing `ddqa-0.0.1/src/ddqa/screens/sync.py` & `ddqa-0.1.0/src/ddqa/screens/sync.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,30 +23,30 @@
     InteractiveSidebar > TextLog {
         height: 8fr;
     }
 
     InteractiveSidebar > Button {
         border: none;
         width: 100%;
-        height: 1fr;
+        height: auto;
     }
     """
 
     def __init__(self, *args, manual_execution, **kwargs):
         super().__init__(*args, **kwargs)
 
         self.__manual_execution = manual_execution
 
     def compose(self) -> ComposeResult:
         yield Label()
         yield TextLog()
         yield Button('Exit' if self.__manual_execution else 'Continue', variant='primary', disabled=True)
 
     def on_mount(self) -> None:
-        self.call_after_refresh(lambda: self.app.run_in_background(self.__on_mount()))
+        self.run_worker(self.__on_mount())
 
     async def __on_mount(self) -> None:
         status = self.query_one(Label)
         text_log = self.query_one(TextLog)
         button = self.query_one(Button)
 
         async with ResponsiveNetworkClient(status) as client:
```

### Comparing `ddqa-0.0.1/src/ddqa/utils/clipboard.py` & `ddqa-0.1.0/src/ddqa/utils/clipboard.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.0.1/src/ddqa/utils/fs.py` & `ddqa-0.1.0/src/ddqa/utils/fs.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.0.1/src/ddqa/utils/git.py` & `ddqa-0.1.0/src/ddqa/utils/git.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.0.1/src/ddqa/utils/github.py` & `ddqa-0.1.0/src/ddqa/utils/github.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.0.1/src/ddqa/utils/jira.py` & `ddqa-0.1.0/src/ddqa/utils/jira.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.0.1/src/ddqa/utils/network.py` & `ddqa-0.1.0/src/ddqa/utils/network.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.0.1/src/ddqa/utils/structures.py` & `ddqa-0.1.0/src/ddqa/utils/structures.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.0.1/src/ddqa/utils/time.py` & `ddqa-0.1.0/src/ddqa/utils/time.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.0.1/src/ddqa/widgets/input.py` & `ddqa-0.1.0/src/ddqa/widgets/input.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # SPDX-FileCopyrightText: 2023-present Datadog, Inc. <dev@datadoghq.com>
 #
 # SPDX-License-Identifier: MIT
-from textual.containers import Horizontal
+from textual.containers import HorizontalScroll
 from textual.widgets import Label, Switch
 
 
-class LabeledInput(Horizontal):
+class LabeledInput(HorizontalScroll):
     DEFAULT_CSS = """
     LabeledInput {
         height: 3;
     }
 
     LabeledInput > Label {
         margin-top: 1;
@@ -19,15 +19,15 @@
 
     LabeledInput > Input {
         width: 5fr;
     }
     """
 
 
-class LabeledSwitch(Horizontal):
+class LabeledSwitch(HorizontalScroll):
     DEFAULT_CSS = """
     LabeledSwitch {
         height: auto;
         width: auto;
     }
 
     LabeledSwitch > Label {
```

### Comparing `ddqa-0.0.1/src/ddqa/widgets/layout.py` & `ddqa-0.1.0/src/ddqa/widgets/layout.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.0.1/src/ddqa/widgets/static.py` & `ddqa-0.1.0/src/ddqa/widgets/static.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.0.1/tests/conftest.py` & `ddqa-0.1.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.0.1/tests/cli/config/test_find.py` & `ddqa-0.1.0/tests/cli/config/test_find.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.0.1/tests/cli/config/test_restore.py` & `ddqa-0.1.0/tests/cli/config/test_restore.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.0.1/tests/cli/config/test_show.py` & `ddqa-0.1.0/tests/cli/config/test_show.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.0.1/tests/cli/create/test_create.py` & `ddqa-0.1.0/tests/cli/create/test_create.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.0.1/tests/cli/status/test_status.py` & `ddqa-0.1.0/tests/cli/status/test_status.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.0.1/tests/cli/sync/test_sync.py` & `ddqa-0.1.0/tests/cli/sync/test_sync.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.0.1/tests/helpers/api.py` & `ddqa-0.1.0/tests/helpers/api.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.0.1/tests/screens/test_configure.py` & `ddqa-0.1.0/tests/screens/test_configure.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.0.1/tests/screens/test_create.py` & `ddqa-0.1.0/tests/screens/test_create.py`

 * *Files 1% similar despite different names*

```diff
@@ -261,15 +261,15 @@
 
         sidebar = app.query_one(CandidateSidebar)
         table = sidebar.listing
 
         rendering = app.query_one(CandidateRendering)
         rendered_label = rendering.label.render()
         rendered_label_text = str(rendered_label)
-        assert rendered_label_text == ' PR 2 '
+        assert rendered_label_text == ' #2 '
         assert len(rendered_label.spans) == 1
         rendered_label_span = rendered_label.spans[0]
         assert rendered_label_span.start == 1
         assert rendered_label_span.end == len(rendered_label_text) - 1
         assert rendered_label_span.style == 'link https://github.com/org/repo/pull/2'
 
         rendered_title = rendering.title.render()
@@ -282,15 +282,15 @@
         rendered_body1 = [w for w in rendering.body.children if isinstance(w, Markdown)][0]
 
         table.cursor_coordinate = Coordinate(1, 0)
         await pilot.pause(helpers.ASYNC_WAIT)
 
         rendered_label = rendering.label.render()
         rendered_label_text = str(rendered_label)
-        assert rendered_label_text == ' Commit hash3 '
+        assert rendered_label_text == ' hash3 '
         assert len(rendered_label.spans) == 1
         rendered_label_span = rendered_label.spans[0]
         assert rendered_label_span.start == 1
         assert rendered_label_span.end == len(rendered_label_text) - 1
         assert rendered_label_span.style == 'link https://github.com/org/repo/commit/hash3'
 
         rendered_title = rendering.title.render()
@@ -708,15 +708,15 @@
                         },
                     ),
                 ),
             ],
         )
 
         async with app.run_test() as pilot:
-            await app.wait_for_background_tasks()
+            await app.workers.wait_for_complete()
             await pilot.pause(helpers.ASYNC_WAIT)
 
             sidebar = app.query_one(CandidateSidebar)
             table = sidebar.listing
             num_candidates = len(table.rows)
             assert num_candidates == 3
             assert table.get_row_at(0) == ['✓', 'title2']
@@ -750,15 +750,15 @@
                 True,
                 True,
                 True,
             ]
 
             app.set_focus(sidebar.button)
             await pilot.press('enter')
-            await app.wait_for_background_tasks()
+            await app.workers.wait_for_complete()
             await pilot.pause(helpers.ASYNC_WAIT)
 
             assert str(sidebar.status.render()) == 'Finished'
             assert str(sidebar.label.render()) == f' {num_candidates} / {num_candidates} '
             assert str(sidebar.button.label) == 'Exit'
 
             assert response_mock.call_args_list == [
```

### Comparing `ddqa-0.0.1/tests/screens/test_sync.py` & `ddqa-0.1.0/tests/screens/test_sync.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.0.1/tests/utils/test_fs.py` & `ddqa-0.1.0/tests/utils/test_fs.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.0.1/tests/utils/test_git.py` & `ddqa-0.1.0/tests/utils/test_git.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.0.1/tests/utils/test_github.py` & `ddqa-0.1.0/tests/utils/test_github.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.0.1/tests/utils/test_jira.py` & `ddqa-0.1.0/tests/utils/test_jira.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.0.1/tests/utils/test_structures.py` & `ddqa-0.1.0/tests/utils/test_structures.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.0.1/tests/utils/test_time.py` & `ddqa-0.1.0/tests/utils/test_time.py`

 * *Files identical despite different names*

### Comparing `ddqa-0.0.1/LICENSE.txt` & `ddqa-0.1.0/LICENSE.txt`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-MIT License
-
-Copyright (c) 2023-present Datadog, Inc. <dev@datadoghq.com>
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+MIT License
+
+Copyright (c) 2023-present Datadog, Inc. <dev@datadoghq.com>
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `ddqa-0.0.1/README.md` & `ddqa-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `ddqa-0.0.1/hatch.toml` & `ddqa-0.1.0/hatch.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [envs.default]
-python = "3.11"
+python = "3.10"
 dependencies = [
   "coverage[toml]>=6.5",
   "pytest",
   "pytest-asyncio",
   "pytest-mock",
 ]
 # pre-install-commands = [
@@ -79,15 +79,14 @@
   "validate",
 ]
 
 [envs.build]
 detached = true
 dependencies = [
   "pyoxidizer>=0.24.0",
-  "pip-tools>=6.12.3",
 ]
 
 [envs.build.env-vars]
 PIP_FIND_LINKS = "dist"
 
 [envs.build.scripts]
 _template = "pyoxidizer build --path app {args}"
@@ -97,13 +96,9 @@
 ]
 release = [
   "hatch build -t wheel",
   "_template install --release",
 ]
 msi = [
   "hatch build -t wheel",
-  "_template msi_installer --release",
-]
-setup = [
-  "pip-compile -o requirements.txt pyproject.toml",
-  "python scripts/fix_requirements.py",
+  "_template msi --release",
 ]
```

### Comparing `ddqa-0.0.1/pyproject.toml` & `ddqa-0.1.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [build-system]
-requires = ["hatchling"]
+requires = ["hatchling", "hatch-vcs"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ddqa"
 dynamic = ["version"]
 description = "Datadog's QA manager for releases of GitHub repositories"
 readme = "README.md"
@@ -29,28 +29,32 @@
 dependencies = [
   "click>=8.1.3",
   "httpx",
   "pillow",
   "platformdirs",
   "pydantic<2",
   "rich",
-  "textual>=0.11.1,<0.14.0",
-  "textual-autocomplete>=2.0.1b0",
+  "textual~=0.19.0",
+  "textual-autocomplete>=2.1.0b0",
   "tomli; python_version < '3.11'",
   "tomli-w",
 ]
 
 [project.urls]
 Source = "https://github.com/DataDog/ddqa"
 
 [project.scripts]
 ddqa = "ddqa.cli:main"
 
 [tool.hatch.version]
-path = "src/ddqa/__about__.py"
+source = "vcs"
+raw-options = { version_scheme = "python-simplified-semver", local_scheme = "no-local-version" }
+
+[tool.hatch.build.hooks.vcs]
+version-file = "src/ddqa/_version.py"
 
 [tool.black]
 target-version = ["py310"]
 line-length = 120
 skip-string-normalization = true
 extend-exclude = """
 src/ddqa/utils/clipboard.py
@@ -145,15 +149,15 @@
 "tests/**/*" = ["PLR2004", "S101", "TID252"]
 
 [tool.coverage.run]
 source_pkgs = ["ddqa", "tests"]
 branch = true
 parallel = true
 omit = [
-  "src/ddqa/__about__.py",
+  "src/ddqa/_version.py.py",
 ]
 
 [tool.coverage.paths]
 ddqa = ["src/ddqa", "*/ddqa/src/ddqa"]
 tests = ["tests", "*/ddqa/tests"]
 
 [tool.coverage.report]
```

### Comparing `ddqa-0.0.1/PKG-INFO` & `ddqa-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ddqa
-Version: 0.0.1
+Version: 0.1.0
 Summary: Datadog's QA manager for releases of GitHub repositories
 Project-URL: Source, https://github.com/DataDog/ddqa
 Author-email: "Datadog, Inc." <dev@datadoghq.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Keywords: datadog,qa,testing,tooling
 Classifier: Development Status :: 4 - Beta
@@ -16,16 +16,16 @@
 Requires-Python: >=3.10
 Requires-Dist: click>=8.1.3
 Requires-Dist: httpx
 Requires-Dist: pillow
 Requires-Dist: platformdirs
 Requires-Dist: pydantic<2
 Requires-Dist: rich
-Requires-Dist: textual-autocomplete>=2.0.1b0
-Requires-Dist: textual<0.14.0,>=0.11.1
+Requires-Dist: textual-autocomplete>=2.1.0b0
+Requires-Dist: textual~=0.19.0
 Requires-Dist: tomli-w
 Requires-Dist: tomli; python_version < '3.11'
 Description-Content-Type: text/markdown
 
 # Datadog QA
 
 | | |
```

