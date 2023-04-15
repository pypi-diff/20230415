# Comparing `tmp/trest-1.3.0.tar.gz` & `tmp/trest-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trest-1.3.0.tar", last modified: Tue Mar 28 15:33:51 2023, max compression
+gzip compressed data, was "trest-1.4.0.tar", last modified: Sat Apr 15 17:38:52 2023, max compression
```

## Comparing `trest-1.3.0.tar` & `trest-1.4.0.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-03-28 15:33:51.017027 trest-1.3.0/
--rw-rw-rw-   0        0        0    11558 2022-09-22 06:54:22.000000 trest-1.3.0/LICENSE.md
--rw-rw-rw-   0        0        0    14640 2023-03-28 15:33:51.016025 trest-1.3.0/PKG-INFO
--rw-rw-rw-   0        0        0      944 2023-01-03 12:16:50.000000 trest-1.3.0/README.md
--rw-rw-rw-   0        0        0      757 2023-03-28 15:28:33.000000 trest-1.3.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-28 15:33:51.017027 trest-1.3.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-03-28 15:33:50.934027 trest-1.3.0/src/
-drwxrwxrwx   0        0        0        0 2023-03-28 15:33:50.953025 trest-1.3.0/src/trest/
--rw-rw-rw-   0        0        0        0 2022-10-13 12:00:14.000000 trest-1.3.0/src/trest/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-28 15:33:50.995026 trest-1.3.0/src/trest/configuration/
--rw-rw-rw-   0        0        0        0 2023-01-03 09:01:35.000000 trest-1.3.0/src/trest/configuration/__init__.py
--rw-rw-rw-   0        0        0      153 2023-01-03 11:39:21.000000 trest-1.3.0/src/trest/configuration/config.py
--rw-rw-rw-   0        0        0     1578 2023-03-28 15:28:33.000000 trest-1.3.0/src/trest/curl_converter.py
--rw-rw-rw-   0        0        0     5963 2023-03-28 15:28:33.000000 trest-1.3.0/src/trest/rest_request.py
--rw-rw-rw-   0        0        0     4157 2023-03-28 15:28:33.000000 trest-1.3.0/src/trest/rest_response.py
-drwxrwxrwx   0        0        0        0 2023-03-28 15:33:50.999024 trest-1.3.0/src/trest/utils/
--rw-rw-rw-   0        0        0      158 2023-03-28 15:28:33.000000 trest-1.3.0/src/trest/utils/__init__.py
--rw-rw-rw-   0        0        0     1511 2023-03-28 15:28:33.000000 trest-1.3.0/src/trest/utils/logging_utils.py
-drwxrwxrwx   0        0        0        0 2023-03-28 15:33:50.989027 trest-1.3.0/src/trest.egg-info/
--rw-rw-rw-   0        0        0    14640 2023-03-28 15:33:50.000000 trest-1.3.0/src/trest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      558 2023-03-28 15:33:50.000000 trest-1.3.0/src/trest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-28 15:33:50.000000 trest-1.3.0/src/trest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-03-28 15:33:50.000000 trest-1.3.0/src/trest.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-03-28 15:33:50.000000 trest-1.3.0/src/trest.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-28 15:33:51.013026 trest-1.3.0/tests/
--rw-rw-rw-   0        0        0     1005 2022-10-17 11:15:31.000000 trest-1.3.0/tests/test_basic.py
--rw-rw-rw-   0        0        0     1105 2023-03-28 15:28:33.000000 trest-1.3.0/tests/test_config.py
--rw-rw-rw-   0        0        0     1845 2023-03-28 15:28:33.000000 trest-1.3.0/tests/test_curl_converter.py
--rw-rw-rw-   0        0        0     1255 2023-03-28 15:28:33.000000 trest-1.3.0/tests/test_rest_request.py
--rw-rw-rw-   0        0        0     1394 2023-03-28 15:28:33.000000 trest-1.3.0/tests/test_rest_response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:38:52.858239 trest-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-15 17:38:41.000000 trest-1.4.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    14393 2023-04-15 17:38:52.858239 trest-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-04-15 17:38:41.000000 trest-1.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-04-15 17:38:41.000000 trest-1.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 17:38:52.858239 trest-1.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:38:52.858239 trest-1.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:38:52.858239 trest-1.4.0/src/trest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 17:38:41.000000 trest-1.4.0/src/trest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:38:52.858239 trest-1.4.0/src/trest/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 17:38:41.000000 trest-1.4.0/src/trest/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-15 17:38:41.000000 trest-1.4.0/src/trest/configuration/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-04-15 17:38:41.000000 trest-1.4.0/src/trest/curl_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-04-15 17:38:41.000000 trest-1.4.0/src/trest/object_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6283 2023-04-15 17:38:41.000000 trest-1.4.0/src/trest/rest_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-04-15 17:38:41.000000 trest-1.4.0/src/trest/rest_response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:38:52.858239 trest-1.4.0/src/trest/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-15 17:38:41.000000 trest-1.4.0/src/trest/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-04-15 17:38:41.000000 trest-1.4.0/src/trest/utils/logging_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:38:52.858239 trest-1.4.0/src/trest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14393 2023-04-15 17:38:52.000000 trest-1.4.0/src/trest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-15 17:38:52.000000 trest-1.4.0/src/trest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 17:38:52.000000 trest-1.4.0/src/trest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-15 17:38:52.000000 trest-1.4.0/src/trest.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-15 17:38:52.000000 trest-1.4.0/src/trest.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 17:38:52.858239 trest-1.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-04-15 17:38:41.000000 trest-1.4.0/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-04-15 17:38:41.000000 trest-1.4.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-04-15 17:38:41.000000 trest-1.4.0/tests/test_curl_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-04-15 17:38:41.000000 trest-1.4.0/tests/test_rest_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-04-15 17:38:41.000000 trest-1.4.0/tests/test_rest_response.py
```

### Comparing `trest-1.3.0/LICENSE.md` & `trest-1.4.0/LICENSE.md`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright [yyyy] [name of copyright owner]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [yyyy] [name of copyright owner]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `trest-1.3.0/PKG-INFO` & `trest-1.4.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,247 +1,247 @@
-Metadata-Version: 2.1
-Name: trest
-Version: 1.3.0
-Summary: Basic REST client with extended logging
-Author-email: l0kifs <l0kifs91@gmail.com>
-License:                                  Apache License
-                                   Version 2.0, January 2004
-                                http://www.apache.org/licenses/
-        
-           TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-        
-           1. Definitions.
-        
-              "License" shall mean the terms and conditions for use, reproduction,
-              and distribution as defined by Sections 1 through 9 of this document.
-        
-              "Licensor" shall mean the copyright owner or entity authorized by
-              the copyright owner that is granting the License.
-        
-              "Legal Entity" shall mean the union of the acting entity and all
-              other entities that control, are controlled by, or are under common
-              control with that entity. For the purposes of this definition,
-              "control" means (i) the power, direct or indirect, to cause the
-              direction or management of such entity, whether by contract or
-              otherwise, or (ii) ownership of fifty percent (50%) or more of the
-              outstanding shares, or (iii) beneficial ownership of such entity.
-        
-              "You" (or "Your") shall mean an individual or Legal Entity
-              exercising permissions granted by this License.
-        
-              "Source" form shall mean the preferred form for making modifications,
-              including but not limited to software source code, documentation
-              source, and configuration files.
-        
-              "Object" form shall mean any form resulting from mechanical
-              transformation or translation of a Source form, including but
-              not limited to compiled object code, generated documentation,
-              and conversions to other media types.
-        
-              "Work" shall mean the work of authorship, whether in Source or
-              Object form, made available under the License, as indicated by a
-              copyright notice that is included in or attached to the work
-              (an example is provided in the Appendix below).
-        
-              "Derivative Works" shall mean any work, whether in Source or Object
-              form, that is based on (or derived from) the Work and for which the
-              editorial revisions, annotations, elaborations, or other modifications
-              represent, as a whole, an original work of authorship. For the purposes
-              of this License, Derivative Works shall not include works that remain
-              separable from, or merely link (or bind by name) to the interfaces of,
-              the Work and Derivative Works thereof.
-        
-              "Contribution" shall mean any work of authorship, including
-              the original version of the Work and any modifications or additions
-              to that Work or Derivative Works thereof, that is intentionally
-              submitted to Licensor for inclusion in the Work by the copyright owner
-              or by an individual or Legal Entity authorized to submit on behalf of
-              the copyright owner. For the purposes of this definition, "submitted"
-              means any form of electronic, verbal, or written communication sent
-              to the Licensor or its representatives, including but not limited to
-              communication on electronic mailing lists, source code control systems,
-              and issue tracking systems that are managed by, or on behalf of, the
-              Licensor for the purpose of discussing and improving the Work, but
-              excluding communication that is conspicuously marked or otherwise
-              designated in writing by the copyright owner as "Not a Contribution."
-        
-              "Contributor" shall mean Licensor and any individual or Legal Entity
-              on behalf of whom a Contribution has been received by Licensor and
-              subsequently incorporated within the Work.
-        
-           2. Grant of Copyright License. Subject to the terms and conditions of
-              this License, each Contributor hereby grants to You a perpetual,
-              worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-              copyright license to reproduce, prepare Derivative Works of,
-              publicly display, publicly perform, sublicense, and distribute the
-              Work and such Derivative Works in Source or Object form.
-        
-           3. Grant of Patent License. Subject to the terms and conditions of
-              this License, each Contributor hereby grants to You a perpetual,
-              worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-              (except as stated in this section) patent license to make, have made,
-              use, offer to sell, sell, import, and otherwise transfer the Work,
-              where such license applies only to those patent claims licensable
-              by such Contributor that are necessarily infringed by their
-              Contribution(s) alone or by combination of their Contribution(s)
-              with the Work to which such Contribution(s) was submitted. If You
-              institute patent litigation against any entity (including a
-              cross-claim or counterclaim in a lawsuit) alleging that the Work
-              or a Contribution incorporated within the Work constitutes direct
-              or contributory patent infringement, then any patent licenses
-              granted to You under this License for that Work shall terminate
-              as of the date such litigation is filed.
-        
-           4. Redistribution. You may reproduce and distribute copies of the
-              Work or Derivative Works thereof in any medium, with or without
-              modifications, and in Source or Object form, provided that You
-              meet the following conditions:
-        
-              (a) You must give any other recipients of the Work or
-                  Derivative Works a copy of this License; and
-        
-              (b) You must cause any modified files to carry prominent notices
-                  stating that You changed the files; and
-        
-              (c) You must retain, in the Source form of any Derivative Works
-                  that You distribute, all copyright, patent, trademark, and
-                  attribution notices from the Source form of the Work,
-                  excluding those notices that do not pertain to any part of
-                  the Derivative Works; and
-        
-              (d) If the Work includes a "NOTICE" text file as part of its
-                  distribution, then any Derivative Works that You distribute must
-                  include a readable copy of the attribution notices contained
-                  within such NOTICE file, excluding those notices that do not
-                  pertain to any part of the Derivative Works, in at least one
-                  of the following places: within a NOTICE text file distributed
-                  as part of the Derivative Works; within the Source form or
-                  documentation, if provided along with the Derivative Works; or,
-                  within a display generated by the Derivative Works, if and
-                  wherever such third-party notices normally appear. The contents
-                  of the NOTICE file are for informational purposes only and
-                  do not modify the License. You may add Your own attribution
-                  notices within Derivative Works that You distribute, alongside
-                  or as an addendum to the NOTICE text from the Work, provided
-                  that such additional attribution notices cannot be construed
-                  as modifying the License.
-        
-              You may add Your own copyright statement to Your modifications and
-              may provide additional or different license terms and conditions
-              for use, reproduction, or distribution of Your modifications, or
-              for any such Derivative Works as a whole, provided Your use,
-              reproduction, and distribution of the Work otherwise complies with
-              the conditions stated in this License.
-        
-           5. Submission of Contributions. Unless You explicitly state otherwise,
-              any Contribution intentionally submitted for inclusion in the Work
-              by You to the Licensor shall be under the terms and conditions of
-              this License, without any additional terms or conditions.
-              Notwithstanding the above, nothing herein shall supersede or modify
-              the terms of any separate license agreement you may have executed
-              with Licensor regarding such Contributions.
-        
-           6. Trademarks. This License does not grant permission to use the trade
-              names, trademarks, service marks, or product names of the Licensor,
-              except as required for reasonable and customary use in describing the
-              origin of the Work and reproducing the content of the NOTICE file.
-        
-           7. Disclaimer of Warranty. Unless required by applicable law or
-              agreed to in writing, Licensor provides the Work (and each
-              Contributor provides its Contributions) on an "AS IS" BASIS,
-              WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-              implied, including, without limitation, any warranties or conditions
-              of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-              PARTICULAR PURPOSE. You are solely responsible for determining the
-              appropriateness of using or redistributing the Work and assume any
-              risks associated with Your exercise of permissions under this License.
-        
-           8. Limitation of Liability. In no event and under no legal theory,
-              whether in tort (including negligence), contract, or otherwise,
-              unless required by applicable law (such as deliberate and grossly
-              negligent acts) or agreed to in writing, shall any Contributor be
-              liable to You for damages, including any direct, indirect, special,
-              incidental, or consequential damages of any character arising as a
-              result of this License or out of the use or inability to use the
-              Work (including but not limited to damages for loss of goodwill,
-              work stoppage, computer failure or malfunction, or any and all
-              other commercial damages or losses), even if such Contributor
-              has been advised of the possibility of such damages.
-        
-           9. Accepting Warranty or Additional Liability. While redistributing
-              the Work or Derivative Works thereof, You may choose to offer,
-              and charge a fee for, acceptance of support, warranty, indemnity,
-              or other liability obligations and/or rights consistent with this
-              License. However, in accepting such obligations, You may act only
-              on Your own behalf and on Your sole responsibility, not on behalf
-              of any other Contributor, and only if You agree to indemnify,
-              defend, and hold each Contributor harmless for any liability
-              incurred by, or claims asserted against, such Contributor by reason
-              of your accepting any such warranty or additional liability.
-        
-           END OF TERMS AND CONDITIONS
-        
-           APPENDIX: How to apply the Apache License to your work.
-        
-              To apply the Apache License to your work, attach the following
-              boilerplate notice, with the fields enclosed by brackets "[]"
-              replaced with your own identifying information. (Don't include
-              the brackets!)  The text should be enclosed in the appropriate
-              comment syntax for the file format. We also recommend that a
-              file or class name and description of purpose be included on the
-              same "printed page" as the copyright notice for easier
-              identification within third-party archives.
-        
-           Copyright [yyyy] [name of copyright owner]
-        
-           Licensed under the Apache License, Version 2.0 (the "License");
-           you may not use this file except in compliance with the License.
-           You may obtain a copy of the License at
-        
-               http://www.apache.org/licenses/LICENSE-2.0
-        
-           Unless required by applicable law or agreed to in writing, software
-           distributed under the License is distributed on an "AS IS" BASIS,
-           WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-           See the License for the specific language governing permissions and
-           limitations under the License.
-        
-Project-URL: Homepage, https://github.com/l0kifs/trest_client
-Keywords: rest,client,allure,logging
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE.md
-
-# TREST client
-
-## Description
-Basic REST client with extended logging.
-
-## Features
-- Every request provide allure report step with all request and response data.  
-Report data organised in a way convenient for testing API and repeating issues in Postman.
-- Dataclass objects provided by `jto` library can be used as request body.  
-Useful for project organization.
-- Client configuration using `Config` module.
-  - Print full request and response data to stdout. Useful for fast debugging.
-  - Provide oneline representation of request and response. Useful for mor accurate logging.
-
-## Examples
-
-Basic usage:
-```python
-from trest.rest_request import RESTRequest
-
-request = RESTRequest(method='GET', url='https://api.ipify.org')
-response = request.send()
-```
-Client configuration:
-```python
-from trest.configuration.config import Config
-
-Config.one_line_response = True
-Config.print_response_to_std_out = True
-```
+Metadata-Version: 2.1
+Name: trest
+Version: 1.4.0
+Summary: Basic REST client with extended logging
+Author-email: l0kifs <l0kifs91@gmail.com>
+License:                                  Apache License
+                                   Version 2.0, January 2004
+                                http://www.apache.org/licenses/
+        
+           TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+        
+           1. Definitions.
+        
+              "License" shall mean the terms and conditions for use, reproduction,
+              and distribution as defined by Sections 1 through 9 of this document.
+        
+              "Licensor" shall mean the copyright owner or entity authorized by
+              the copyright owner that is granting the License.
+        
+              "Legal Entity" shall mean the union of the acting entity and all
+              other entities that control, are controlled by, or are under common
+              control with that entity. For the purposes of this definition,
+              "control" means (i) the power, direct or indirect, to cause the
+              direction or management of such entity, whether by contract or
+              otherwise, or (ii) ownership of fifty percent (50%) or more of the
+              outstanding shares, or (iii) beneficial ownership of such entity.
+        
+              "You" (or "Your") shall mean an individual or Legal Entity
+              exercising permissions granted by this License.
+        
+              "Source" form shall mean the preferred form for making modifications,
+              including but not limited to software source code, documentation
+              source, and configuration files.
+        
+              "Object" form shall mean any form resulting from mechanical
+              transformation or translation of a Source form, including but
+              not limited to compiled object code, generated documentation,
+              and conversions to other media types.
+        
+              "Work" shall mean the work of authorship, whether in Source or
+              Object form, made available under the License, as indicated by a
+              copyright notice that is included in or attached to the work
+              (an example is provided in the Appendix below).
+        
+              "Derivative Works" shall mean any work, whether in Source or Object
+              form, that is based on (or derived from) the Work and for which the
+              editorial revisions, annotations, elaborations, or other modifications
+              represent, as a whole, an original work of authorship. For the purposes
+              of this License, Derivative Works shall not include works that remain
+              separable from, or merely link (or bind by name) to the interfaces of,
+              the Work and Derivative Works thereof.
+        
+              "Contribution" shall mean any work of authorship, including
+              the original version of the Work and any modifications or additions
+              to that Work or Derivative Works thereof, that is intentionally
+              submitted to Licensor for inclusion in the Work by the copyright owner
+              or by an individual or Legal Entity authorized to submit on behalf of
+              the copyright owner. For the purposes of this definition, "submitted"
+              means any form of electronic, verbal, or written communication sent
+              to the Licensor or its representatives, including but not limited to
+              communication on electronic mailing lists, source code control systems,
+              and issue tracking systems that are managed by, or on behalf of, the
+              Licensor for the purpose of discussing and improving the Work, but
+              excluding communication that is conspicuously marked or otherwise
+              designated in writing by the copyright owner as "Not a Contribution."
+        
+              "Contributor" shall mean Licensor and any individual or Legal Entity
+              on behalf of whom a Contribution has been received by Licensor and
+              subsequently incorporated within the Work.
+        
+           2. Grant of Copyright License. Subject to the terms and conditions of
+              this License, each Contributor hereby grants to You a perpetual,
+              worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+              copyright license to reproduce, prepare Derivative Works of,
+              publicly display, publicly perform, sublicense, and distribute the
+              Work and such Derivative Works in Source or Object form.
+        
+           3. Grant of Patent License. Subject to the terms and conditions of
+              this License, each Contributor hereby grants to You a perpetual,
+              worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+              (except as stated in this section) patent license to make, have made,
+              use, offer to sell, sell, import, and otherwise transfer the Work,
+              where such license applies only to those patent claims licensable
+              by such Contributor that are necessarily infringed by their
+              Contribution(s) alone or by combination of their Contribution(s)
+              with the Work to which such Contribution(s) was submitted. If You
+              institute patent litigation against any entity (including a
+              cross-claim or counterclaim in a lawsuit) alleging that the Work
+              or a Contribution incorporated within the Work constitutes direct
+              or contributory patent infringement, then any patent licenses
+              granted to You under this License for that Work shall terminate
+              as of the date such litigation is filed.
+        
+           4. Redistribution. You may reproduce and distribute copies of the
+              Work or Derivative Works thereof in any medium, with or without
+              modifications, and in Source or Object form, provided that You
+              meet the following conditions:
+        
+              (a) You must give any other recipients of the Work or
+                  Derivative Works a copy of this License; and
+        
+              (b) You must cause any modified files to carry prominent notices
+                  stating that You changed the files; and
+        
+              (c) You must retain, in the Source form of any Derivative Works
+                  that You distribute, all copyright, patent, trademark, and
+                  attribution notices from the Source form of the Work,
+                  excluding those notices that do not pertain to any part of
+                  the Derivative Works; and
+        
+              (d) If the Work includes a "NOTICE" text file as part of its
+                  distribution, then any Derivative Works that You distribute must
+                  include a readable copy of the attribution notices contained
+                  within such NOTICE file, excluding those notices that do not
+                  pertain to any part of the Derivative Works, in at least one
+                  of the following places: within a NOTICE text file distributed
+                  as part of the Derivative Works; within the Source form or
+                  documentation, if provided along with the Derivative Works; or,
+                  within a display generated by the Derivative Works, if and
+                  wherever such third-party notices normally appear. The contents
+                  of the NOTICE file are for informational purposes only and
+                  do not modify the License. You may add Your own attribution
+                  notices within Derivative Works that You distribute, alongside
+                  or as an addendum to the NOTICE text from the Work, provided
+                  that such additional attribution notices cannot be construed
+                  as modifying the License.
+        
+              You may add Your own copyright statement to Your modifications and
+              may provide additional or different license terms and conditions
+              for use, reproduction, or distribution of Your modifications, or
+              for any such Derivative Works as a whole, provided Your use,
+              reproduction, and distribution of the Work otherwise complies with
+              the conditions stated in this License.
+        
+           5. Submission of Contributions. Unless You explicitly state otherwise,
+              any Contribution intentionally submitted for inclusion in the Work
+              by You to the Licensor shall be under the terms and conditions of
+              this License, without any additional terms or conditions.
+              Notwithstanding the above, nothing herein shall supersede or modify
+              the terms of any separate license agreement you may have executed
+              with Licensor regarding such Contributions.
+        
+           6. Trademarks. This License does not grant permission to use the trade
+              names, trademarks, service marks, or product names of the Licensor,
+              except as required for reasonable and customary use in describing the
+              origin of the Work and reproducing the content of the NOTICE file.
+        
+           7. Disclaimer of Warranty. Unless required by applicable law or
+              agreed to in writing, Licensor provides the Work (and each
+              Contributor provides its Contributions) on an "AS IS" BASIS,
+              WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+              implied, including, without limitation, any warranties or conditions
+              of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+              PARTICULAR PURPOSE. You are solely responsible for determining the
+              appropriateness of using or redistributing the Work and assume any
+              risks associated with Your exercise of permissions under this License.
+        
+           8. Limitation of Liability. In no event and under no legal theory,
+              whether in tort (including negligence), contract, or otherwise,
+              unless required by applicable law (such as deliberate and grossly
+              negligent acts) or agreed to in writing, shall any Contributor be
+              liable to You for damages, including any direct, indirect, special,
+              incidental, or consequential damages of any character arising as a
+              result of this License or out of the use or inability to use the
+              Work (including but not limited to damages for loss of goodwill,
+              work stoppage, computer failure or malfunction, or any and all
+              other commercial damages or losses), even if such Contributor
+              has been advised of the possibility of such damages.
+        
+           9. Accepting Warranty or Additional Liability. While redistributing
+              the Work or Derivative Works thereof, You may choose to offer,
+              and charge a fee for, acceptance of support, warranty, indemnity,
+              or other liability obligations and/or rights consistent with this
+              License. However, in accepting such obligations, You may act only
+              on Your own behalf and on Your sole responsibility, not on behalf
+              of any other Contributor, and only if You agree to indemnify,
+              defend, and hold each Contributor harmless for any liability
+              incurred by, or claims asserted against, such Contributor by reason
+              of your accepting any such warranty or additional liability.
+        
+           END OF TERMS AND CONDITIONS
+        
+           APPENDIX: How to apply the Apache License to your work.
+        
+              To apply the Apache License to your work, attach the following
+              boilerplate notice, with the fields enclosed by brackets "[]"
+              replaced with your own identifying information. (Don't include
+              the brackets!)  The text should be enclosed in the appropriate
+              comment syntax for the file format. We also recommend that a
+              file or class name and description of purpose be included on the
+              same "printed page" as the copyright notice for easier
+              identification within third-party archives.
+        
+           Copyright [yyyy] [name of copyright owner]
+        
+           Licensed under the Apache License, Version 2.0 (the "License");
+           you may not use this file except in compliance with the License.
+           You may obtain a copy of the License at
+        
+               http://www.apache.org/licenses/LICENSE-2.0
+        
+           Unless required by applicable law or agreed to in writing, software
+           distributed under the License is distributed on an "AS IS" BASIS,
+           WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+           See the License for the specific language governing permissions and
+           limitations under the License.
+        
+Project-URL: Homepage, https://github.com/l0kifs/trest_client
+Keywords: rest,client,allure,logging
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE.md
+
+# TREST client
+
+## Description
+Basic REST client with extended logging.
+
+## Features
+- Every request provide allure report step with all request and response data.  
+Report data organised in a way convenient for testing API and repeating issues in Postman.
+- Dataclass objects provided by `jto` library can be used as request body.  
+Useful for project organization.
+- Client configuration using `Config` module.
+  - Print full request and response data to stdout. Useful for fast debugging.
+  - Provide oneline representation of request and response. Useful for mor accurate logging.
+
+## Examples
+
+Basic usage:
+```python
+from trest.rest_request import RESTRequest
+
+request = RESTRequest(method='GET', url='https://api.ipify.org')
+response = request.send()
+```
+Client configuration:
+```python
+from trest.configuration.config import Config
+
+Config.one_line_response = True
+Config.print_response_to_std_out = True
+```
```

### Comparing `trest-1.3.0/README.md` & `trest-1.4.0/README.md`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-# TREST client
-
-## Description
-Basic REST client with extended logging.
-
-## Features
-- Every request provide allure report step with all request and response data.  
-Report data organised in a way convenient for testing API and repeating issues in Postman.
-- Dataclass objects provided by `jto` library can be used as request body.  
-Useful for project organization.
-- Client configuration using `Config` module.
-  - Print full request and response data to stdout. Useful for fast debugging.
-  - Provide oneline representation of request and response. Useful for mor accurate logging.
-
-## Examples
-
-Basic usage:
-```python
-from trest.rest_request import RESTRequest
-
-request = RESTRequest(method='GET', url='https://api.ipify.org')
-response = request.send()
-```
-Client configuration:
-```python
-from trest.configuration.config import Config
-
-Config.one_line_response = True
-Config.print_response_to_std_out = True
+# TREST client
+
+## Description
+Basic REST client with extended logging.
+
+## Features
+- Every request provide allure report step with all request and response data.  
+Report data organised in a way convenient for testing API and repeating issues in Postman.
+- Dataclass objects provided by `jto` library can be used as request body.  
+Useful for project organization.
+- Client configuration using `Config` module.
+  - Print full request and response data to stdout. Useful for fast debugging.
+  - Provide oneline representation of request and response. Useful for mor accurate logging.
+
+## Examples
+
+Basic usage:
+```python
+from trest.rest_request import RESTRequest
+
+request = RESTRequest(method='GET', url='https://api.ipify.org')
+response = request.send()
+```
+Client configuration:
+```python
+from trest.configuration.config import Config
+
+Config.one_line_response = True
+Config.print_response_to_std_out = True
 ```
```

### Comparing `trest-1.3.0/src/trest/curl_converter.py` & `trest-1.4.0/src/trest/curl_converter.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,43 +1,62 @@
-import inspect
-import logging
-from typing import Dict, List, Union
-
-
-class CurlConverter:
-    _log = logging.getLogger(__name__)
-
-    @classmethod
-    def to_curl(cls, method: str,
-                url: str,
-                params: Dict[str, Union[str, List[str]]] = None,
-                headers: Dict[str, str] = None,
-                data: str = None) -> str:
-        """
-        Generates Curl string representation
-        :param method: http method
-        :param url: url
-        :param params: dictionary of url parameters
-        :param headers: dict of headers
-        :param data: data string
-        :return: curl string representation
-        """
-        cls._log.debug(f'function "{inspect.currentframe().f_code.co_name}" '
-                       f'called with args "{inspect.getargvalues(inspect.currentframe()).locals}"')
-
-        curl_cmd = f'curl -X {method}'
-        if headers is not None:
-            headers = ' '.join(f'-H "{key}: {value}"' for key, value in headers.items())
-            curl_cmd += f' {headers}'
-        if data is not None:
-            curl_cmd += f' -d \'{data}\''
-        if params is not None:
-            params_list = []
-            for key, value in params.items():
-                if type(value) == list:
-                    for item in value:
-                        params_list.append(f'{key}={item}')
-                else:
-                    params_list.append(f'{key}={value}')
-            url = f'{url}?'+'&'.join(params_list)
-        curl_cmd += f' {url}'
-        return curl_cmd
+import inspect
+import logging
+from typing import Dict, List, Union
+
+from trest.object_converter import ObjectConverter
+
+
+class CurlConverter:
+    _log = logging.getLogger(__name__)
+
+    @classmethod
+    def to_curl(cls, method: str,
+                url: str,
+                params: Dict[str, Union[str, List[str]]] = None,
+                headers: Dict[str, str] = None,
+                data: str = None,
+                multiline: bool = False) -> str:
+        """
+        Generates Curl string representation
+        :param method: http method
+        :param url: url
+        :param params: dictionary of url parameters
+        :param headers: dict of headers
+        :param data: data string
+        :param multiline: if True, returns curl string in multiline format
+        :return: curl string representation
+        """
+        cls._log.debug(f'function "{inspect.currentframe().f_code.co_name}" '
+                       f'called with args "{inspect.getargvalues(inspect.currentframe()).locals}"')
+        if multiline:
+            curl_cmd = f'curl -X {method}'
+        else:
+            curl_cmd = f'curl -X {method}'
+
+        if headers is not None:
+            if multiline:
+                headers = ' \\\n'.join(f'-H "{key}: {value}"' for key, value in headers.items())
+                curl_cmd += f' \\\n{headers}'
+            else:
+                headers = ' '.join(f'-H "{key}: {value}"' for key, value in headers.items())
+                curl_cmd += f' {headers}'
+
+        if data is not None:
+            if multiline:
+                curl_cmd += f' \\\n-d \'{ObjectConverter.to_string(data, indent=4)}\''
+            else:
+                curl_cmd += f' -d \'{data}\''
+
+        if params is not None:
+            params_list = []
+            for key, value in params.items():
+                if type(value) == list:
+                    for item in value:
+                        params_list.append(f'{key}={item}')
+                else:
+                    params_list.append(f'{key}={value}')
+            url = f'{url}?'+'&'.join(params_list)
+        if multiline:
+            curl_cmd += f' \\\n{url}'
+        else:
+            curl_cmd += f' {url}'
+        return curl_cmd
```

### Comparing `trest-1.3.0/src/trest/rest_response.py` & `trest-1.4.0/src/trest/rest_response.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,97 +1,97 @@
-import inspect
-import json
-import logging
-from typing import Dict
-
-from trest.utils import is_json_string
-
-
-class RESTResponse(object):
-    _log = logging.getLogger(__name__)
-
-    def __init__(self, url: str,
-                 method: str,
-                 path: str,
-                 request_headers: Dict[str, str],
-                 request_body: str,
-                 status_code: int,
-                 reason: str,
-                 response_headers: Dict[str, str],
-                 response_body: str,
-                 elapsed_time: str):
-        self._log.debug(f'function "{inspect.currentframe().f_code.co_name}" '
-                        f'called with args "{inspect.getargvalues(inspect.currentframe()).locals}"')
-
-        self.url = url
-        self.method = method
-        self.path = path
-        self.request_headers = request_headers
-        self.request_body = request_body
-
-        self.status_code = status_code
-        self.reason = reason
-        self.response_headers = response_headers
-        self.response_body = response_body
-        self.elapsed_time = elapsed_time
-
-    def get_response_body_json(self):
-        self._log.debug(f'function "{inspect.currentframe().f_code.co_name}" '
-                        f'called with args "{inspect.getargvalues(inspect.currentframe()).locals}"')
-        if not is_json_string(self.response_body):
-            raise TypeError(f'Response body {self.response_body} is not json')
-        return json.loads(self.response_body)
-
-    def get_request_json_repr(self):
-        self._log.debug(f'function "{inspect.currentframe().f_code.co_name}" '
-                        f'called with args "{inspect.getargvalues(inspect.currentframe()).locals}"')
-        json_response = {
-            'status_code': self.status_code,
-            'reason': self.reason,
-            'headers': self.response_headers,
-            'elapsed_time': self.elapsed_time,
-            'body': self.response_body if not is_json_string(self.response_body) else json.loads(
-                self.response_body)
-        }
-        json_request = {
-            'url': self.url,
-            'method': self.method,
-            'path': self.path,
-            'headers': self.request_headers,
-            'body': self.request_body if not is_json_string(self.request_body) else json.loads(
-                self.request_body),
-            'response': json_response
-        }
-        return json_request
-
-    def get_string_repr(self, one_line: bool = False) -> str:
-        self._log.debug(f'function "{inspect.currentframe().f_code.co_name}" '
-                        f'called with args "{inspect.getargvalues(inspect.currentframe()).locals}"')
-        result_string = f'{self.status_code} {self.reason} {self.elapsed_time}'
-
-        if self.response_headers:
-            if one_line:
-                result_string = result_string + ', Headers: '
-                headers = []
-                for key, value in self.response_headers.items():
-                    headers.append(f"{key}: {value}")
-                result_string = result_string + ', '.join(headers)
-            else:
-                result_string = result_string + '\n\nHeaders:\n'
-                headers = []
-                for key, value in self.response_headers.items():
-                    headers.append(f"{key}: {value}")
-                result_string = result_string + '\n'.join(headers)
-
-        if self.response_body:
-            if one_line:
-                result_string = result_string + ', Content: '
-                body_string = self.response_body if not is_json_string(self.response_body) else json.dumps(
-                    json.loads(self.response_body))
-                result_string = result_string + body_string
-            else:
-                result_string = result_string + '\n\nContent:\n'
-                body_string = self.response_body if not is_json_string(self.response_body) else json.dumps(
-                    json.loads(self.response_body), indent=4)
-                result_string = result_string + body_string
-
-        return result_string
+import inspect
+import json
+import logging
+from typing import Dict
+
+from trest.utils import is_json_string
+
+
+class RESTResponse(object):
+    _log = logging.getLogger(__name__)
+
+    def __init__(self, url: str,
+                 method: str,
+                 path: str,
+                 request_headers: Dict[str, str],
+                 request_body: str,
+                 status_code: int,
+                 reason: str,
+                 response_headers: Dict[str, str],
+                 response_body: str,
+                 elapsed_time: str):
+        self._log.debug(f'function "{inspect.currentframe().f_code.co_name}" '
+                        f'called with args "{inspect.getargvalues(inspect.currentframe()).locals}"')
+
+        self.url = url
+        self.method = method
+        self.path = path
+        self.request_headers = request_headers
+        self.request_body = request_body
+
+        self.status_code = status_code
+        self.reason = reason
+        self.response_headers = response_headers
+        self.response_body = response_body
+        self.elapsed_time = elapsed_time
+
+    def get_response_body_json(self):
+        self._log.debug(f'function "{inspect.currentframe().f_code.co_name}" '
+                        f'called with args "{inspect.getargvalues(inspect.currentframe()).locals}"')
+        if not is_json_string(self.response_body):
+            raise TypeError(f'Response body {self.response_body} is not json')
+        return json.loads(self.response_body)
+
+    def get_request_json_repr(self):
+        self._log.debug(f'function "{inspect.currentframe().f_code.co_name}" '
+                        f'called with args "{inspect.getargvalues(inspect.currentframe()).locals}"')
+        json_response = {
+            'status_code': self.status_code,
+            'reason': self.reason,
+            'headers': self.response_headers,
+            'elapsed_time': self.elapsed_time,
+            'body': self.response_body if not is_json_string(self.response_body) else json.loads(
+                self.response_body)
+        }
+        json_request = {
+            'url': self.url,
+            'method': self.method,
+            'path': self.path,
+            'headers': self.request_headers,
+            'body': self.request_body if not is_json_string(self.request_body) else json.loads(
+                self.request_body),
+            'response': json_response
+        }
+        return json_request
+
+    def get_string_repr(self, one_line: bool = False) -> str:
+        self._log.debug(f'function "{inspect.currentframe().f_code.co_name}" '
+                        f'called with args "{inspect.getargvalues(inspect.currentframe()).locals}"')
+        result_string = f'{self.status_code} {self.reason} {self.elapsed_time}'
+
+        if self.response_headers:
+            if one_line:
+                result_string = result_string + ', Headers: '
+                headers = []
+                for key, value in self.response_headers.items():
+                    headers.append(f"{key}: {value}")
+                result_string = result_string + ', '.join(headers)
+            else:
+                result_string = result_string + '\n\nHeaders:\n'
+                headers = []
+                for key, value in self.response_headers.items():
+                    headers.append(f"{key}: {value}")
+                result_string = result_string + '\n'.join(headers)
+
+        if self.response_body:
+            if one_line:
+                result_string = result_string + ', Content: '
+                body_string = self.response_body if not is_json_string(self.response_body) else json.dumps(
+                    json.loads(self.response_body))
+                result_string = result_string + body_string
+            else:
+                result_string = result_string + '\n\nContent:\n'
+                body_string = self.response_body if not is_json_string(self.response_body) else json.dumps(
+                    json.loads(self.response_body), indent=4)
+                result_string = result_string + body_string
+
+        return result_string
```

### Comparing `trest-1.3.0/src/trest/utils/logging_utils.py` & `trest-1.4.0/src/trest/utils/logging_utils.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-import functools
-import inspect
-import logging
-
-
-def log(logger: logging.Logger = None):
-    def decorator(func):
-        @functools.wraps(func)
-        def wrapper(*args, **kwargs):
-            func_logger = logger if logger is not None else logging.getLogger(func.__name__)
-
-            try:
-                args_names = inspect.signature(func).parameters.keys()
-                args_dict = dict(zip(args_names, args))
-                args_repr = [f"{k}={v}" for k, v in args_dict.items()]
-                kwargs_repr = [f"{k}={v}" for k, v in kwargs.items()]
-                signature = ", ".join(args_repr + kwargs_repr)
-                func_logger.debug(f"function {func.__name__} called with args {signature}")
-            except:
-                func_logger.debug(f"function {func.__name__} called")
-
-            try:
-                result = func(*args, **kwargs)
-                return result
-            except Exception as e:
-                func_logger.exception(f"Exception raised in {func.__name__}", exc_info=True)
-                raise e
-
-        wrapper.__name__ = func.__name__
-        wrapper.__doc__ = func.__doc__
-        wrapper.__module__ = func.__module__
-        wrapper.__qualname__ = func.__qualname__
-
-        return wrapper
-    return decorator
-
-
-# logging.basicConfig(level=logging.DEBUG, format='%(asctime)s - %(name)s - %(levelname)s - %(lineno)d - %(message)s')
-# @log()
-# def my_func(qwer):
-#     print("hello world")
-# my_func("qqq")
+import functools
+import inspect
+import logging
+
+
+def log(logger: logging.Logger = None):
+    def decorator(func):
+        @functools.wraps(func)
+        def wrapper(*args, **kwargs):
+            func_logger = logger if logger is not None else logging.getLogger(func.__name__)
+
+            try:
+                args_names = inspect.signature(func).parameters.keys()
+                args_dict = dict(zip(args_names, args))
+                args_repr = [f"{k}={v}" for k, v in args_dict.items()]
+                kwargs_repr = [f"{k}={v}" for k, v in kwargs.items()]
+                signature = ", ".join(args_repr + kwargs_repr)
+                func_logger.debug(f"function {func.__name__} called with args {signature}")
+            except:
+                func_logger.debug(f"function {func.__name__} called")
+
+            try:
+                result = func(*args, **kwargs)
+                return result
+            except Exception as e:
+                func_logger.exception(f"Exception raised in {func.__name__}", exc_info=True)
+                raise e
+
+        wrapper.__name__ = func.__name__
+        wrapper.__doc__ = func.__doc__
+        wrapper.__module__ = func.__module__
+        wrapper.__qualname__ = func.__qualname__
+
+        return wrapper
+    return decorator
+
+
+# logging.basicConfig(level=logging.DEBUG, format='%(asctime)s - %(name)s - %(levelname)s - %(lineno)d - %(message)s')
+# @log()
+# def my_func(qwer):
+#     print("hello world")
+# my_func("qqq")
```

### Comparing `trest-1.3.0/src/trest.egg-info/PKG-INFO` & `trest-1.4.0/src/trest.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,247 +1,247 @@
-Metadata-Version: 2.1
-Name: trest
-Version: 1.3.0
-Summary: Basic REST client with extended logging
-Author-email: l0kifs <l0kifs91@gmail.com>
-License:                                  Apache License
-                                   Version 2.0, January 2004
-                                http://www.apache.org/licenses/
-        
-           TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-        
-           1. Definitions.
-        
-              "License" shall mean the terms and conditions for use, reproduction,
-              and distribution as defined by Sections 1 through 9 of this document.
-        
-              "Licensor" shall mean the copyright owner or entity authorized by
-              the copyright owner that is granting the License.
-        
-              "Legal Entity" shall mean the union of the acting entity and all
-              other entities that control, are controlled by, or are under common
-              control with that entity. For the purposes of this definition,
-              "control" means (i) the power, direct or indirect, to cause the
-              direction or management of such entity, whether by contract or
-              otherwise, or (ii) ownership of fifty percent (50%) or more of the
-              outstanding shares, or (iii) beneficial ownership of such entity.
-        
-              "You" (or "Your") shall mean an individual or Legal Entity
-              exercising permissions granted by this License.
-        
-              "Source" form shall mean the preferred form for making modifications,
-              including but not limited to software source code, documentation
-              source, and configuration files.
-        
-              "Object" form shall mean any form resulting from mechanical
-              transformation or translation of a Source form, including but
-              not limited to compiled object code, generated documentation,
-              and conversions to other media types.
-        
-              "Work" shall mean the work of authorship, whether in Source or
-              Object form, made available under the License, as indicated by a
-              copyright notice that is included in or attached to the work
-              (an example is provided in the Appendix below).
-        
-              "Derivative Works" shall mean any work, whether in Source or Object
-              form, that is based on (or derived from) the Work and for which the
-              editorial revisions, annotations, elaborations, or other modifications
-              represent, as a whole, an original work of authorship. For the purposes
-              of this License, Derivative Works shall not include works that remain
-              separable from, or merely link (or bind by name) to the interfaces of,
-              the Work and Derivative Works thereof.
-        
-              "Contribution" shall mean any work of authorship, including
-              the original version of the Work and any modifications or additions
-              to that Work or Derivative Works thereof, that is intentionally
-              submitted to Licensor for inclusion in the Work by the copyright owner
-              or by an individual or Legal Entity authorized to submit on behalf of
-              the copyright owner. For the purposes of this definition, "submitted"
-              means any form of electronic, verbal, or written communication sent
-              to the Licensor or its representatives, including but not limited to
-              communication on electronic mailing lists, source code control systems,
-              and issue tracking systems that are managed by, or on behalf of, the
-              Licensor for the purpose of discussing and improving the Work, but
-              excluding communication that is conspicuously marked or otherwise
-              designated in writing by the copyright owner as "Not a Contribution."
-        
-              "Contributor" shall mean Licensor and any individual or Legal Entity
-              on behalf of whom a Contribution has been received by Licensor and
-              subsequently incorporated within the Work.
-        
-           2. Grant of Copyright License. Subject to the terms and conditions of
-              this License, each Contributor hereby grants to You a perpetual,
-              worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-              copyright license to reproduce, prepare Derivative Works of,
-              publicly display, publicly perform, sublicense, and distribute the
-              Work and such Derivative Works in Source or Object form.
-        
-           3. Grant of Patent License. Subject to the terms and conditions of
-              this License, each Contributor hereby grants to You a perpetual,
-              worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-              (except as stated in this section) patent license to make, have made,
-              use, offer to sell, sell, import, and otherwise transfer the Work,
-              where such license applies only to those patent claims licensable
-              by such Contributor that are necessarily infringed by their
-              Contribution(s) alone or by combination of their Contribution(s)
-              with the Work to which such Contribution(s) was submitted. If You
-              institute patent litigation against any entity (including a
-              cross-claim or counterclaim in a lawsuit) alleging that the Work
-              or a Contribution incorporated within the Work constitutes direct
-              or contributory patent infringement, then any patent licenses
-              granted to You under this License for that Work shall terminate
-              as of the date such litigation is filed.
-        
-           4. Redistribution. You may reproduce and distribute copies of the
-              Work or Derivative Works thereof in any medium, with or without
-              modifications, and in Source or Object form, provided that You
-              meet the following conditions:
-        
-              (a) You must give any other recipients of the Work or
-                  Derivative Works a copy of this License; and
-        
-              (b) You must cause any modified files to carry prominent notices
-                  stating that You changed the files; and
-        
-              (c) You must retain, in the Source form of any Derivative Works
-                  that You distribute, all copyright, patent, trademark, and
-                  attribution notices from the Source form of the Work,
-                  excluding those notices that do not pertain to any part of
-                  the Derivative Works; and
-        
-              (d) If the Work includes a "NOTICE" text file as part of its
-                  distribution, then any Derivative Works that You distribute must
-                  include a readable copy of the attribution notices contained
-                  within such NOTICE file, excluding those notices that do not
-                  pertain to any part of the Derivative Works, in at least one
-                  of the following places: within a NOTICE text file distributed
-                  as part of the Derivative Works; within the Source form or
-                  documentation, if provided along with the Derivative Works; or,
-                  within a display generated by the Derivative Works, if and
-                  wherever such third-party notices normally appear. The contents
-                  of the NOTICE file are for informational purposes only and
-                  do not modify the License. You may add Your own attribution
-                  notices within Derivative Works that You distribute, alongside
-                  or as an addendum to the NOTICE text from the Work, provided
-                  that such additional attribution notices cannot be construed
-                  as modifying the License.
-        
-              You may add Your own copyright statement to Your modifications and
-              may provide additional or different license terms and conditions
-              for use, reproduction, or distribution of Your modifications, or
-              for any such Derivative Works as a whole, provided Your use,
-              reproduction, and distribution of the Work otherwise complies with
-              the conditions stated in this License.
-        
-           5. Submission of Contributions. Unless You explicitly state otherwise,
-              any Contribution intentionally submitted for inclusion in the Work
-              by You to the Licensor shall be under the terms and conditions of
-              this License, without any additional terms or conditions.
-              Notwithstanding the above, nothing herein shall supersede or modify
-              the terms of any separate license agreement you may have executed
-              with Licensor regarding such Contributions.
-        
-           6. Trademarks. This License does not grant permission to use the trade
-              names, trademarks, service marks, or product names of the Licensor,
-              except as required for reasonable and customary use in describing the
-              origin of the Work and reproducing the content of the NOTICE file.
-        
-           7. Disclaimer of Warranty. Unless required by applicable law or
-              agreed to in writing, Licensor provides the Work (and each
-              Contributor provides its Contributions) on an "AS IS" BASIS,
-              WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-              implied, including, without limitation, any warranties or conditions
-              of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-              PARTICULAR PURPOSE. You are solely responsible for determining the
-              appropriateness of using or redistributing the Work and assume any
-              risks associated with Your exercise of permissions under this License.
-        
-           8. Limitation of Liability. In no event and under no legal theory,
-              whether in tort (including negligence), contract, or otherwise,
-              unless required by applicable law (such as deliberate and grossly
-              negligent acts) or agreed to in writing, shall any Contributor be
-              liable to You for damages, including any direct, indirect, special,
-              incidental, or consequential damages of any character arising as a
-              result of this License or out of the use or inability to use the
-              Work (including but not limited to damages for loss of goodwill,
-              work stoppage, computer failure or malfunction, or any and all
-              other commercial damages or losses), even if such Contributor
-              has been advised of the possibility of such damages.
-        
-           9. Accepting Warranty or Additional Liability. While redistributing
-              the Work or Derivative Works thereof, You may choose to offer,
-              and charge a fee for, acceptance of support, warranty, indemnity,
-              or other liability obligations and/or rights consistent with this
-              License. However, in accepting such obligations, You may act only
-              on Your own behalf and on Your sole responsibility, not on behalf
-              of any other Contributor, and only if You agree to indemnify,
-              defend, and hold each Contributor harmless for any liability
-              incurred by, or claims asserted against, such Contributor by reason
-              of your accepting any such warranty or additional liability.
-        
-           END OF TERMS AND CONDITIONS
-        
-           APPENDIX: How to apply the Apache License to your work.
-        
-              To apply the Apache License to your work, attach the following
-              boilerplate notice, with the fields enclosed by brackets "[]"
-              replaced with your own identifying information. (Don't include
-              the brackets!)  The text should be enclosed in the appropriate
-              comment syntax for the file format. We also recommend that a
-              file or class name and description of purpose be included on the
-              same "printed page" as the copyright notice for easier
-              identification within third-party archives.
-        
-           Copyright [yyyy] [name of copyright owner]
-        
-           Licensed under the Apache License, Version 2.0 (the "License");
-           you may not use this file except in compliance with the License.
-           You may obtain a copy of the License at
-        
-               http://www.apache.org/licenses/LICENSE-2.0
-        
-           Unless required by applicable law or agreed to in writing, software
-           distributed under the License is distributed on an "AS IS" BASIS,
-           WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-           See the License for the specific language governing permissions and
-           limitations under the License.
-        
-Project-URL: Homepage, https://github.com/l0kifs/trest_client
-Keywords: rest,client,allure,logging
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE.md
-
-# TREST client
-
-## Description
-Basic REST client with extended logging.
-
-## Features
-- Every request provide allure report step with all request and response data.  
-Report data organised in a way convenient for testing API and repeating issues in Postman.
-- Dataclass objects provided by `jto` library can be used as request body.  
-Useful for project organization.
-- Client configuration using `Config` module.
-  - Print full request and response data to stdout. Useful for fast debugging.
-  - Provide oneline representation of request and response. Useful for mor accurate logging.
-
-## Examples
-
-Basic usage:
-```python
-from trest.rest_request import RESTRequest
-
-request = RESTRequest(method='GET', url='https://api.ipify.org')
-response = request.send()
-```
-Client configuration:
-```python
-from trest.configuration.config import Config
-
-Config.one_line_response = True
-Config.print_response_to_std_out = True
-```
+Metadata-Version: 2.1
+Name: trest
+Version: 1.4.0
+Summary: Basic REST client with extended logging
+Author-email: l0kifs <l0kifs91@gmail.com>
+License:                                  Apache License
+                                   Version 2.0, January 2004
+                                http://www.apache.org/licenses/
+        
+           TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+        
+           1. Definitions.
+        
+              "License" shall mean the terms and conditions for use, reproduction,
+              and distribution as defined by Sections 1 through 9 of this document.
+        
+              "Licensor" shall mean the copyright owner or entity authorized by
+              the copyright owner that is granting the License.
+        
+              "Legal Entity" shall mean the union of the acting entity and all
+              other entities that control, are controlled by, or are under common
+              control with that entity. For the purposes of this definition,
+              "control" means (i) the power, direct or indirect, to cause the
+              direction or management of such entity, whether by contract or
+              otherwise, or (ii) ownership of fifty percent (50%) or more of the
+              outstanding shares, or (iii) beneficial ownership of such entity.
+        
+              "You" (or "Your") shall mean an individual or Legal Entity
+              exercising permissions granted by this License.
+        
+              "Source" form shall mean the preferred form for making modifications,
+              including but not limited to software source code, documentation
+              source, and configuration files.
+        
+              "Object" form shall mean any form resulting from mechanical
+              transformation or translation of a Source form, including but
+              not limited to compiled object code, generated documentation,
+              and conversions to other media types.
+        
+              "Work" shall mean the work of authorship, whether in Source or
+              Object form, made available under the License, as indicated by a
+              copyright notice that is included in or attached to the work
+              (an example is provided in the Appendix below).
+        
+              "Derivative Works" shall mean any work, whether in Source or Object
+              form, that is based on (or derived from) the Work and for which the
+              editorial revisions, annotations, elaborations, or other modifications
+              represent, as a whole, an original work of authorship. For the purposes
+              of this License, Derivative Works shall not include works that remain
+              separable from, or merely link (or bind by name) to the interfaces of,
+              the Work and Derivative Works thereof.
+        
+              "Contribution" shall mean any work of authorship, including
+              the original version of the Work and any modifications or additions
+              to that Work or Derivative Works thereof, that is intentionally
+              submitted to Licensor for inclusion in the Work by the copyright owner
+              or by an individual or Legal Entity authorized to submit on behalf of
+              the copyright owner. For the purposes of this definition, "submitted"
+              means any form of electronic, verbal, or written communication sent
+              to the Licensor or its representatives, including but not limited to
+              communication on electronic mailing lists, source code control systems,
+              and issue tracking systems that are managed by, or on behalf of, the
+              Licensor for the purpose of discussing and improving the Work, but
+              excluding communication that is conspicuously marked or otherwise
+              designated in writing by the copyright owner as "Not a Contribution."
+        
+              "Contributor" shall mean Licensor and any individual or Legal Entity
+              on behalf of whom a Contribution has been received by Licensor and
+              subsequently incorporated within the Work.
+        
+           2. Grant of Copyright License. Subject to the terms and conditions of
+              this License, each Contributor hereby grants to You a perpetual,
+              worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+              copyright license to reproduce, prepare Derivative Works of,
+              publicly display, publicly perform, sublicense, and distribute the
+              Work and such Derivative Works in Source or Object form.
+        
+           3. Grant of Patent License. Subject to the terms and conditions of
+              this License, each Contributor hereby grants to You a perpetual,
+              worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+              (except as stated in this section) patent license to make, have made,
+              use, offer to sell, sell, import, and otherwise transfer the Work,
+              where such license applies only to those patent claims licensable
+              by such Contributor that are necessarily infringed by their
+              Contribution(s) alone or by combination of their Contribution(s)
+              with the Work to which such Contribution(s) was submitted. If You
+              institute patent litigation against any entity (including a
+              cross-claim or counterclaim in a lawsuit) alleging that the Work
+              or a Contribution incorporated within the Work constitutes direct
+              or contributory patent infringement, then any patent licenses
+              granted to You under this License for that Work shall terminate
+              as of the date such litigation is filed.
+        
+           4. Redistribution. You may reproduce and distribute copies of the
+              Work or Derivative Works thereof in any medium, with or without
+              modifications, and in Source or Object form, provided that You
+              meet the following conditions:
+        
+              (a) You must give any other recipients of the Work or
+                  Derivative Works a copy of this License; and
+        
+              (b) You must cause any modified files to carry prominent notices
+                  stating that You changed the files; and
+        
+              (c) You must retain, in the Source form of any Derivative Works
+                  that You distribute, all copyright, patent, trademark, and
+                  attribution notices from the Source form of the Work,
+                  excluding those notices that do not pertain to any part of
+                  the Derivative Works; and
+        
+              (d) If the Work includes a "NOTICE" text file as part of its
+                  distribution, then any Derivative Works that You distribute must
+                  include a readable copy of the attribution notices contained
+                  within such NOTICE file, excluding those notices that do not
+                  pertain to any part of the Derivative Works, in at least one
+                  of the following places: within a NOTICE text file distributed
+                  as part of the Derivative Works; within the Source form or
+                  documentation, if provided along with the Derivative Works; or,
+                  within a display generated by the Derivative Works, if and
+                  wherever such third-party notices normally appear. The contents
+                  of the NOTICE file are for informational purposes only and
+                  do not modify the License. You may add Your own attribution
+                  notices within Derivative Works that You distribute, alongside
+                  or as an addendum to the NOTICE text from the Work, provided
+                  that such additional attribution notices cannot be construed
+                  as modifying the License.
+        
+              You may add Your own copyright statement to Your modifications and
+              may provide additional or different license terms and conditions
+              for use, reproduction, or distribution of Your modifications, or
+              for any such Derivative Works as a whole, provided Your use,
+              reproduction, and distribution of the Work otherwise complies with
+              the conditions stated in this License.
+        
+           5. Submission of Contributions. Unless You explicitly state otherwise,
+              any Contribution intentionally submitted for inclusion in the Work
+              by You to the Licensor shall be under the terms and conditions of
+              this License, without any additional terms or conditions.
+              Notwithstanding the above, nothing herein shall supersede or modify
+              the terms of any separate license agreement you may have executed
+              with Licensor regarding such Contributions.
+        
+           6. Trademarks. This License does not grant permission to use the trade
+              names, trademarks, service marks, or product names of the Licensor,
+              except as required for reasonable and customary use in describing the
+              origin of the Work and reproducing the content of the NOTICE file.
+        
+           7. Disclaimer of Warranty. Unless required by applicable law or
+              agreed to in writing, Licensor provides the Work (and each
+              Contributor provides its Contributions) on an "AS IS" BASIS,
+              WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+              implied, including, without limitation, any warranties or conditions
+              of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+              PARTICULAR PURPOSE. You are solely responsible for determining the
+              appropriateness of using or redistributing the Work and assume any
+              risks associated with Your exercise of permissions under this License.
+        
+           8. Limitation of Liability. In no event and under no legal theory,
+              whether in tort (including negligence), contract, or otherwise,
+              unless required by applicable law (such as deliberate and grossly
+              negligent acts) or agreed to in writing, shall any Contributor be
+              liable to You for damages, including any direct, indirect, special,
+              incidental, or consequential damages of any character arising as a
+              result of this License or out of the use or inability to use the
+              Work (including but not limited to damages for loss of goodwill,
+              work stoppage, computer failure or malfunction, or any and all
+              other commercial damages or losses), even if such Contributor
+              has been advised of the possibility of such damages.
+        
+           9. Accepting Warranty or Additional Liability. While redistributing
+              the Work or Derivative Works thereof, You may choose to offer,
+              and charge a fee for, acceptance of support, warranty, indemnity,
+              or other liability obligations and/or rights consistent with this
+              License. However, in accepting such obligations, You may act only
+              on Your own behalf and on Your sole responsibility, not on behalf
+              of any other Contributor, and only if You agree to indemnify,
+              defend, and hold each Contributor harmless for any liability
+              incurred by, or claims asserted against, such Contributor by reason
+              of your accepting any such warranty or additional liability.
+        
+           END OF TERMS AND CONDITIONS
+        
+           APPENDIX: How to apply the Apache License to your work.
+        
+              To apply the Apache License to your work, attach the following
+              boilerplate notice, with the fields enclosed by brackets "[]"
+              replaced with your own identifying information. (Don't include
+              the brackets!)  The text should be enclosed in the appropriate
+              comment syntax for the file format. We also recommend that a
+              file or class name and description of purpose be included on the
+              same "printed page" as the copyright notice for easier
+              identification within third-party archives.
+        
+           Copyright [yyyy] [name of copyright owner]
+        
+           Licensed under the Apache License, Version 2.0 (the "License");
+           you may not use this file except in compliance with the License.
+           You may obtain a copy of the License at
+        
+               http://www.apache.org/licenses/LICENSE-2.0
+        
+           Unless required by applicable law or agreed to in writing, software
+           distributed under the License is distributed on an "AS IS" BASIS,
+           WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+           See the License for the specific language governing permissions and
+           limitations under the License.
+        
+Project-URL: Homepage, https://github.com/l0kifs/trest_client
+Keywords: rest,client,allure,logging
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE.md
+
+# TREST client
+
+## Description
+Basic REST client with extended logging.
+
+## Features
+- Every request provide allure report step with all request and response data.  
+Report data organised in a way convenient for testing API and repeating issues in Postman.
+- Dataclass objects provided by `jto` library can be used as request body.  
+Useful for project organization.
+- Client configuration using `Config` module.
+  - Print full request and response data to stdout. Useful for fast debugging.
+  - Provide oneline representation of request and response. Useful for mor accurate logging.
+
+## Examples
+
+Basic usage:
+```python
+from trest.rest_request import RESTRequest
+
+request = RESTRequest(method='GET', url='https://api.ipify.org')
+response = request.send()
+```
+Client configuration:
+```python
+from trest.configuration.config import Config
+
+Config.one_line_response = True
+Config.print_response_to_std_out = True
+```
```

### Comparing `trest-1.3.0/src/trest.egg-info/SOURCES.txt` & `trest-1.4.0/src/trest.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE.md
 README.md
 pyproject.toml
 src/trest/__init__.py
 src/trest/curl_converter.py
+src/trest/object_converter.py
 src/trest/rest_request.py
 src/trest/rest_response.py
 src/trest.egg-info/PKG-INFO
 src/trest.egg-info/SOURCES.txt
 src/trest.egg-info/dependency_links.txt
 src/trest.egg-info/requires.txt
 src/trest.egg-info/top_level.txt
```

### Comparing `trest-1.3.0/tests/test_curl_converter.py` & `trest-1.4.0/tests/test_curl_converter.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-from trest.curl_converter import CurlConverter
-
-
-def test_curl_get():
-    curl_str = CurlConverter.to_curl('GET', 'https://www.example.com')
-    assert curl_str == 'curl -X GET https://www.example.com'
-
-
-def test_curl_post_json():
-    curl_str = CurlConverter.to_curl(method='POST', url='https://www.example.com',
-                                     headers={'Content-Type': 'application/json'},
-                                     data='{"key1": "value1", "key2": "value2"}')
-    assert curl_str == 'curl -X POST -H "Content-Type: application/json" ' \
-                       '-d \'{"key1": "value1", "key2": "value2"}\' ' \
-                       'https://www.example.com'
-
-
-def test_simple_params():
-    curl_str = CurlConverter.to_curl(method='POST', url='https://www.example.com',
-                                     params={'p1': 'v1', 'p2': 'v2'},
-                                     headers={'Content-Type': 'application/json'},
-                                     data='{"key1": "value1", "key2": "value2"}')
-    assert curl_str == 'curl -X POST -H "Content-Type: application/json" ' \
-                       '-d \'{"key1": "value1", "key2": "value2"}\' ' \
-                       'https://www.example.com?p1=v1&p2=v2'
-
-
-def test_list_param():
-    curl_str = CurlConverter.to_curl(method='POST', url='https://www.example.com',
-                                     params={'p1': 'v1', 'p2[]': ['111', '222']},
-                                     headers={'Content-Type': 'application/json'},
-                                     data='{"key1": "value1", "key2": "value2"}')
-    assert curl_str == 'curl -X POST -H "Content-Type: application/json" ' \
-                       '-d \'{"key1": "value1", "key2": "value2"}\' ' \
-                       'https://www.example.com?p1=v1&p2[]=111&p2[]=222'
+from trest.curl_converter import CurlConverter
+
+
+def test_curl_get():
+    curl_str = CurlConverter.to_curl('GET', 'https://www.example.com')
+    assert curl_str == 'curl -X GET https://www.example.com'
+
+
+def test_curl_post_json():
+    curl_str = CurlConverter.to_curl(method='POST', url='https://www.example.com',
+                                     headers={'Content-Type': 'application/json'},
+                                     data='{"key1": "value1", "key2": "value2"}')
+    assert curl_str == 'curl -X POST -H "Content-Type: application/json" ' \
+                       '-d \'{"key1": "value1", "key2": "value2"}\' ' \
+                       'https://www.example.com'
+
+
+def test_simple_params():
+    curl_str = CurlConverter.to_curl(method='POST', url='https://www.example.com',
+                                     params={'p1': 'v1', 'p2': 'v2'},
+                                     headers={'Content-Type': 'application/json'},
+                                     data='{"key1": "value1", "key2": "value2"}')
+    assert curl_str == 'curl -X POST -H "Content-Type: application/json" ' \
+                       '-d \'{"key1": "value1", "key2": "value2"}\' ' \
+                       'https://www.example.com?p1=v1&p2=v2'
+
+
+def test_list_param():
+    curl_str = CurlConverter.to_curl(method='POST', url='https://www.example.com',
+                                     params={'p1': 'v1', 'p2[]': ['111', '222']},
+                                     headers={'Content-Type': 'application/json'},
+                                     data='{"key1": "value1", "key2": "value2"}')
+    assert curl_str == 'curl -X POST -H "Content-Type: application/json" ' \
+                       '-d \'{"key1": "value1", "key2": "value2"}\' ' \
+                       'https://www.example.com?p1=v1&p2[]=111&p2[]=222'
```

### Comparing `trest-1.3.0/tests/test_rest_request.py` & `trest-1.4.0/tests/test_rest_request.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-from trest.rest_request import RESTRequest
-
-
-def test_get_curl_string():
-    request = RESTRequest(method='POST', url='https://api.ipify.org',
-                          params={'param1': 'one', 'param2': 'two'},
-                          headers={'header1': 'one', 'header2': 'four'},
-                          body={'body1': 'one', 'body2': 'two'})
-
-    expected = 'curl -X POST -H "header1: one" -H "header2: four" ' \
-               '-d \'{"body1": "one", "body2": "two"}\' ' \
-               'https://api.ipify.org?param1=one&param2=two'
-    assert request.get_curl_string() == expected
-
-
-# def test_get_curl_string_one_line():
-#     request = RESTRequest(method='POST', url='https://api.ipify.org',
-#                           params={'param1': 'one', 'param2': 'two'},
-#                           headers={'header1': 'one', 'header2': 'four'},
-#                           body={'body1': 'one', 'body2': 'two'})
-#
-#     expected = "curl --location --request POST https://api.ipify.org?param1=one&param2=two " \
-#                "--header 'header1: one' --header 'header2: four' " \
-#                "--data-raw '{\"body1\": \"one\", \"body2\": \"two\"}'"
-#     assert request.get_curl_string(one_line=True) == expected
-
-
-
+from trest.rest_request import RESTRequest
+
+
+def test_get_curl_string():
+    request = RESTRequest(method='POST', url='https://api.ipify.org',
+                          params={'param1': 'one', 'param2': 'two'},
+                          headers={'header1': 'one', 'header2': 'four'},
+                          body={'body1': 'one', 'body2': 'two'})
+
+    expected = 'curl -X POST -H "header1: one" -H "header2: four" ' \
+               '-d \'{"body1": "one", "body2": "two"}\' ' \
+               'https://api.ipify.org?param1=one&param2=two'
+    assert request.get_curl_string() == expected
+
+
+# def test_get_curl_string_one_line():
+#     request = RESTRequest(method='POST', url='https://api.ipify.org',
+#                           params={'param1': 'one', 'param2': 'two'},
+#                           headers={'header1': 'one', 'header2': 'four'},
+#                           body={'body1': 'one', 'body2': 'two'})
+#
+#     expected = "curl --location --request POST https://api.ipify.org?param1=one&param2=two " \
+#                "--header 'header1: one' --header 'header2: four' " \
+#                "--data-raw '{\"body1\": \"one\", \"body2\": \"two\"}'"
+#     assert request.get_curl_string(one_line=True) == expected
+
+
+
```

### Comparing `trest-1.3.0/tests/test_rest_response.py` & `trest-1.4.0/tests/test_rest_response.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-from trest.rest_response import RESTResponse
-
-
-def test_get_string_repr():
-    response = RESTResponse(url='https://api.ipify.org', method='GET', path='/foo',
-                            request_headers={'header1': 'value1', 'header2': 'value2'},
-                            request_body='{"body1":"value1"}', status_code=200,
-                            reason='ok', response_headers={'header1': 'value1', 'header2': 'value2'},
-                            response_body='{"body1":"value1"}', elapsed_time='0.123')
-
-    expected = '200 ok 0.123\n\nHeaders:\nheader1: value1\nheader2: value2\n\n' \
-               'Content:\n{\n    "body1": "value1"\n}'
-    assert response.get_string_repr() == expected
-
-
-def test_get_string_repr_one_line():
-    response = RESTResponse(url='https://api.ipify.org', method='GET', path='/foo',
-                            request_headers={'header1': 'value1', 'header2': 'value2'},
-                            request_body='{"body1":"value1"}', status_code=200,
-                            reason='ok', response_headers={'header1': 'value1', 'header2': 'value2'},
-                            response_body='{"body1":"value1"}', elapsed_time='0.123')
-
-    expected = '200 ok 0.123, Headers: header1: value1, header2: value2, ' \
-               'Content: {"body1": "value1"}'
-    assert response.get_string_repr(one_line=True) == expected
+from trest.rest_response import RESTResponse
+
+
+def test_get_string_repr():
+    response = RESTResponse(url='https://api.ipify.org', method='GET', path='/foo',
+                            request_headers={'header1': 'value1', 'header2': 'value2'},
+                            request_body='{"body1":"value1"}', status_code=200,
+                            reason='ok', response_headers={'header1': 'value1', 'header2': 'value2'},
+                            response_body='{"body1":"value1"}', elapsed_time='0.123')
+
+    expected = '200 ok 0.123\n\nHeaders:\nheader1: value1\nheader2: value2\n\n' \
+               'Content:\n{\n    "body1": "value1"\n}'
+    assert response.get_string_repr() == expected
+
+
+def test_get_string_repr_one_line():
+    response = RESTResponse(url='https://api.ipify.org', method='GET', path='/foo',
+                            request_headers={'header1': 'value1', 'header2': 'value2'},
+                            request_body='{"body1":"value1"}', status_code=200,
+                            reason='ok', response_headers={'header1': 'value1', 'header2': 'value2'},
+                            response_body='{"body1":"value1"}', elapsed_time='0.123')
+
+    expected = '200 ok 0.123, Headers: header1: value1, header2: value2, ' \
+               'Content: {"body1": "value1"}'
+    assert response.get_string_repr(one_line=True) == expected
```

