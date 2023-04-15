# Comparing `tmp/discord-ext-pager-1.0.0.tar.gz` & `tmp/discord-ext-pager-1.0.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discord-ext-pager-1.0.0.tar", last modified: Fri Apr 14 15:04:21 2023, max compression
+gzip compressed data, was "discord-ext-pager-1.0.0.post1.tar", last modified: Sat Apr 15 14:38:44 2023, max compression
```

## Comparing `discord-ext-pager-1.0.0.tar` & `discord-ext-pager-1.0.0.post1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 15:04:21.425590 discord-ext-pager-1.0.0/
--rw-rw-rw-   0        0        0    17097 2023-04-14 12:58:35.000000 discord-ext-pager-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     5483 2023-04-14 15:04:21.424490 discord-ext-pager-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     4538 2023-04-14 15:03:08.000000 discord-ext-pager-1.0.0/README.md
--rw-rw-rw-   0        0        0     1125 2023-04-14 14:03:46.000000 discord-ext-pager-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-14 15:04:21.425590 discord-ext-pager-1.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-14 15:04:21.395377 discord-ext-pager-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-04-14 15:04:21.393917 discord-ext-pager-1.0.0/src/discord/
-drwxrwxrwx   0        0        0        0 2023-04-14 15:04:21.393917 discord-ext-pager-1.0.0/src/discord/ext/
-drwxrwxrwx   0        0        0        0 2023-04-14 15:04:21.399776 discord-ext-pager-1.0.0/src/discord/ext/pager/
--rw-rw-rw-   0        0        0    16115 2023-04-14 14:34:18.000000 discord-ext-pager-1.0.0/src/discord/ext/pager/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-14 15:04:21.423491 discord-ext-pager-1.0.0/src/discord_ext_pager.egg-info/
--rw-rw-rw-   0        0        0     5483 2023-04-14 15:04:21.000000 discord-ext-pager-1.0.0/src/discord_ext_pager.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      290 2023-04-14 15:04:21.000000 discord-ext-pager-1.0.0/src/discord_ext_pager.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 15:04:21.000000 discord-ext-pager-1.0.0/src/discord_ext_pager.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-04-14 15:04:21.000000 discord-ext-pager-1.0.0/src/discord_ext_pager.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-14 15:04:21.000000 discord-ext-pager-1.0.0/src/discord_ext_pager.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 14:38:44.722700 discord-ext-pager-1.0.0.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-04-15 14:38:30.000000 discord-ext-pager-1.0.0.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5838 2023-04-15 14:38:44.722700 discord-ext-pager-1.0.0.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-04-15 14:38:30.000000 discord-ext-pager-1.0.0.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-15 14:38:30.000000 discord-ext-pager-1.0.0.post1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 14:38:44.722700 discord-ext-pager-1.0.0.post1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 14:38:44.722700 discord-ext-pager-1.0.0.post1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 14:38:44.722700 discord-ext-pager-1.0.0.post1/src/discord/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 14:38:44.722700 discord-ext-pager-1.0.0.post1/src/discord/ext/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 14:38:44.722700 discord-ext-pager-1.0.0.post1/src/discord/ext/pager/
+-rw-r--r--   0 runner    (1001) docker     (123)    15626 2023-04-15 14:38:30.000000 discord-ext-pager-1.0.0.post1/src/discord/ext/pager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 14:38:44.722700 discord-ext-pager-1.0.0.post1/src/discord_ext_pager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5838 2023-04-15 14:38:44.000000 discord-ext-pager-1.0.0.post1/src/discord_ext_pager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-15 14:38:44.000000 discord-ext-pager-1.0.0.post1/src/discord_ext_pager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 14:38:44.000000 discord-ext-pager-1.0.0.post1/src/discord_ext_pager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-15 14:38:44.000000 discord-ext-pager-1.0.0.post1/src/discord_ext_pager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-15 14:38:44.000000 discord-ext-pager-1.0.0.post1/src/discord_ext_pager.egg-info/top_level.txt
```

### Comparing `discord-ext-pager-1.0.0/LICENSE` & `discord-ext-pager-1.0.0.post1/LICENSE`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,373 +1,373 @@
-Mozilla Public License Version 2.0
-==================================
-
-1. Definitions
---------------
-
-1.1. "Contributor"
-    means each individual or legal entity that creates, contributes to
-    the creation of, or owns Covered Software.
-
-1.2. "Contributor Version"
-    means the combination of the Contributions of others (if any) used
-    by a Contributor and that particular Contributor's Contribution.
-
-1.3. "Contribution"
-    means Covered Software of a particular Contributor.
-
-1.4. "Covered Software"
-    means Source Code Form to which the initial Contributor has attached
-    the notice in Exhibit A, the Executable Form of such Source Code
-    Form, and Modifications of such Source Code Form, in each case
-    including portions thereof.
-
-1.5. "Incompatible With Secondary Licenses"
-    means
-
-    (a) that the initial Contributor has attached the notice described
-        in Exhibit B to the Covered Software; or
-
-    (b) that the Covered Software was made available under the terms of
-        version 1.1 or earlier of the License, but not also under the
-        terms of a Secondary License.
-
-1.6. "Executable Form"
-    means any form of the work other than Source Code Form.
-
-1.7. "Larger Work"
-    means a work that combines Covered Software with other material, in
-    a separate file or files, that is not Covered Software.
-
-1.8. "License"
-    means this document.
-
-1.9. "Licensable"
-    means having the right to grant, to the maximum extent possible,
-    whether at the time of the initial grant or subsequently, any and
-    all of the rights conveyed by this License.
-
-1.10. "Modifications"
-    means any of the following:
-
-    (a) any file in Source Code Form that results from an addition to,
-        deletion from, or modification of the contents of Covered
-        Software; or
-
-    (b) any new file in Source Code Form that contains any Covered
-        Software.
-
-1.11. "Patent Claims" of a Contributor
-    means any patent claim(s), including without limitation, method,
-    process, and apparatus claims, in any patent Licensable by such
-    Contributor that would be infringed, but for the grant of the
-    License, by the making, using, selling, offering for sale, having
-    made, import, or transfer of either its Contributions or its
-    Contributor Version.
-
-1.12. "Secondary License"
-    means either the GNU General Public License, Version 2.0, the GNU
-    Lesser General Public License, Version 2.1, the GNU Affero General
-    Public License, Version 3.0, or any later versions of those
-    licenses.
-
-1.13. "Source Code Form"
-    means the form of the work preferred for making modifications.
-
-1.14. "You" (or "Your")
-    means an individual or a legal entity exercising rights under this
-    License. For legal entities, "You" includes any entity that
-    controls, is controlled by, or is under common control with You. For
-    purposes of this definition, "control" means (a) the power, direct
-    or indirect, to cause the direction or management of such entity,
-    whether by contract or otherwise, or (b) ownership of more than
-    fifty percent (50%) of the outstanding shares or beneficial
-    ownership of such entity.
-
-2. License Grants and Conditions
---------------------------------
-
-2.1. Grants
-
-Each Contributor hereby grants You a world-wide, royalty-free,
-non-exclusive license:
-
-(a) under intellectual property rights (other than patent or trademark)
-    Licensable by such Contributor to use, reproduce, make available,
-    modify, display, perform, distribute, and otherwise exploit its
-    Contributions, either on an unmodified basis, with Modifications, or
-    as part of a Larger Work; and
-
-(b) under Patent Claims of such Contributor to make, use, sell, offer
-    for sale, have made, import, and otherwise transfer either its
-    Contributions or its Contributor Version.
-
-2.2. Effective Date
-
-The licenses granted in Section 2.1 with respect to any Contribution
-become effective for each Contribution on the date the Contributor first
-distributes such Contribution.
-
-2.3. Limitations on Grant Scope
-
-The licenses granted in this Section 2 are the only rights granted under
-this License. No additional rights or licenses will be implied from the
-distribution or licensing of Covered Software under this License.
-Notwithstanding Section 2.1(b) above, no patent license is granted by a
-Contributor:
-
-(a) for any code that a Contributor has removed from Covered Software;
-    or
-
-(b) for infringements caused by: (i) Your and any other third party's
-    modifications of Covered Software, or (ii) the combination of its
-    Contributions with other software (except as part of its Contributor
-    Version); or
-
-(c) under Patent Claims infringed by Covered Software in the absence of
-    its Contributions.
-
-This License does not grant any rights in the trademarks, service marks,
-or logos of any Contributor (except as may be necessary to comply with
-the notice requirements in Section 3.4).
-
-2.4. Subsequent Licenses
-
-No Contributor makes additional grants as a result of Your choice to
-distribute the Covered Software under a subsequent version of this
-License (see Section 10.2) or under the terms of a Secondary License (if
-permitted under the terms of Section 3.3).
-
-2.5. Representation
-
-Each Contributor represents that the Contributor believes its
-Contributions are its original creation(s) or it has sufficient rights
-to grant the rights to its Contributions conveyed by this License.
-
-2.6. Fair Use
-
-This License is not intended to limit any rights You have under
-applicable copyright doctrines of fair use, fair dealing, or other
-equivalents.
-
-2.7. Conditions
-
-Sections 3.1, 3.2, 3.3, and 3.4 are conditions of the licenses granted
-in Section 2.1.
-
-3. Responsibilities
--------------------
-
-3.1. Distribution of Source Form
-
-All distribution of Covered Software in Source Code Form, including any
-Modifications that You create or to which You contribute, must be under
-the terms of this License. You must inform recipients that the Source
-Code Form of the Covered Software is governed by the terms of this
-License, and how they can obtain a copy of this License. You may not
-attempt to alter or restrict the recipients' rights in the Source Code
-Form.
-
-3.2. Distribution of Executable Form
-
-If You distribute Covered Software in Executable Form then:
-
-(a) such Covered Software must also be made available in Source Code
-    Form, as described in Section 3.1, and You must inform recipients of
-    the Executable Form how they can obtain a copy of such Source Code
-    Form by reasonable means in a timely manner, at a charge no more
-    than the cost of distribution to the recipient; and
-
-(b) You may distribute such Executable Form under the terms of this
-    License, or sublicense it under different terms, provided that the
-    license for the Executable Form does not attempt to limit or alter
-    the recipients' rights in the Source Code Form under this License.
-
-3.3. Distribution of a Larger Work
-
-You may create and distribute a Larger Work under terms of Your choice,
-provided that You also comply with the requirements of this License for
-the Covered Software. If the Larger Work is a combination of Covered
-Software with a work governed by one or more Secondary Licenses, and the
-Covered Software is not Incompatible With Secondary Licenses, this
-License permits You to additionally distribute such Covered Software
-under the terms of such Secondary License(s), so that the recipient of
-the Larger Work may, at their option, further distribute the Covered
-Software under the terms of either this License or such Secondary
-License(s).
-
-3.4. Notices
-
-You may not remove or alter the substance of any license notices
-(including copyright notices, patent notices, disclaimers of warranty,
-or limitations of liability) contained within the Source Code Form of
-the Covered Software, except that You may alter any license notices to
-the extent required to remedy known factual inaccuracies.
-
-3.5. Application of Additional Terms
-
-You may choose to offer, and to charge a fee for, warranty, support,
-indemnity or liability obligations to one or more recipients of Covered
-Software. However, You may do so only on Your own behalf, and not on
-behalf of any Contributor. You must make it absolutely clear that any
-such warranty, support, indemnity, or liability obligation is offered by
-You alone, and You hereby agree to indemnify every Contributor for any
-liability incurred by such Contributor as a result of warranty, support,
-indemnity or liability terms You offer. You may include additional
-disclaimers of warranty and limitations of liability specific to any
-jurisdiction.
-
-4. Inability to Comply Due to Statute or Regulation
----------------------------------------------------
-
-If it is impossible for You to comply with any of the terms of this
-License with respect to some or all of the Covered Software due to
-statute, judicial order, or regulation then You must: (a) comply with
-the terms of this License to the maximum extent possible; and (b)
-describe the limitations and the code they affect. Such description must
-be placed in a text file included with all distributions of the Covered
-Software under this License. Except to the extent prohibited by statute
-or regulation, such description must be sufficiently detailed for a
-recipient of ordinary skill to be able to understand it.
-
-5. Termination
---------------
-
-5.1. The rights granted under this License will terminate automatically
-if You fail to comply with any of its terms. However, if You become
-compliant, then the rights granted under this License from a particular
-Contributor are reinstated (a) provisionally, unless and until such
-Contributor explicitly and finally terminates Your grants, and (b) on an
-ongoing basis, if such Contributor fails to notify You of the
-non-compliance by some reasonable means prior to 60 days after You have
-come back into compliance. Moreover, Your grants from a particular
-Contributor are reinstated on an ongoing basis if such Contributor
-notifies You of the non-compliance by some reasonable means, this is the
-first time You have received notice of non-compliance with this License
-from such Contributor, and You become compliant prior to 30 days after
-Your receipt of the notice.
-
-5.2. If You initiate litigation against any entity by asserting a patent
-infringement claim (excluding declaratory judgment actions,
-counter-claims, and cross-claims) alleging that a Contributor Version
-directly or indirectly infringes any patent, then the rights granted to
-You by any and all Contributors for the Covered Software under Section
-2.1 of this License shall terminate.
-
-5.3. In the event of termination under Sections 5.1 or 5.2 above, all
-end user license agreements (excluding distributors and resellers) which
-have been validly granted by You or Your distributors under this License
-prior to termination shall survive termination.
-
-************************************************************************
-*                                                                      *
-*  6. Disclaimer of Warranty                                           *
-*  -------------------------                                           *
-*                                                                      *
-*  Covered Software is provided under this License on an "as is"       *
-*  basis, without warranty of any kind, either expressed, implied, or  *
-*  statutory, including, without limitation, warranties that the       *
-*  Covered Software is free of defects, merchantable, fit for a        *
-*  particular purpose or non-infringing. The entire risk as to the     *
-*  quality and performance of the Covered Software is with You.        *
-*  Should any Covered Software prove defective in any respect, You     *
-*  (not any Contributor) assume the cost of any necessary servicing,   *
-*  repair, or correction. This disclaimer of warranty constitutes an   *
-*  essential part of this License. No use of any Covered Software is   *
-*  authorized under this License except under this disclaimer.         *
-*                                                                      *
-************************************************************************
-
-************************************************************************
-*                                                                      *
-*  7. Limitation of Liability                                          *
-*  --------------------------                                          *
-*                                                                      *
-*  Under no circumstances and under no legal theory, whether tort      *
-*  (including negligence), contract, or otherwise, shall any           *
-*  Contributor, or anyone who distributes Covered Software as          *
-*  permitted above, be liable to You for any direct, indirect,         *
-*  special, incidental, or consequential damages of any character      *
-*  including, without limitation, damages for lost profits, loss of    *
-*  goodwill, work stoppage, computer failure or malfunction, or any    *
-*  and all other commercial damages or losses, even if such party      *
-*  shall have been informed of the possibility of such damages. This   *
-*  limitation of liability shall not apply to liability for death or   *
-*  personal injury resulting from such party's negligence to the       *
-*  extent applicable law prohibits such limitation. Some               *
-*  jurisdictions do not allow the exclusion or limitation of           *
-*  incidental or consequential damages, so this exclusion and          *
-*  limitation may not apply to You.                                    *
-*                                                                      *
-************************************************************************
-
-8. Litigation
--------------
-
-Any litigation relating to this License may be brought only in the
-courts of a jurisdiction where the defendant maintains its principal
-place of business and such litigation shall be governed by laws of that
-jurisdiction, without reference to its conflict-of-law provisions.
-Nothing in this Section shall prevent a party's ability to bring
-cross-claims or counter-claims.
-
-9. Miscellaneous
-----------------
-
-This License represents the complete agreement concerning the subject
-matter hereof. If any provision of this License is held to be
-unenforceable, such provision shall be reformed only to the extent
-necessary to make it enforceable. Any law or regulation which provides
-that the language of a contract shall be construed against the drafter
-shall not be used to construe this License against a Contributor.
-
-10. Versions of the License
----------------------------
-
-10.1. New Versions
-
-Mozilla Foundation is the license steward. Except as provided in Section
-10.3, no one other than the license steward has the right to modify or
-publish new versions of this License. Each version will be given a
-distinguishing version number.
-
-10.2. Effect of New Versions
-
-You may distribute the Covered Software under the terms of the version
-of the License under which You originally received the Covered Software,
-or under the terms of any subsequent version published by the license
-steward.
-
-10.3. Modified Versions
-
-If you create software not governed by this License, and you want to
-create a new license for such software, you may create and use a
-modified version of this License if you rename the license and remove
-any references to the name of the license steward (except to note that
-such modified license differs from this License).
-
-10.4. Distributing Source Code Form that is Incompatible With Secondary
-Licenses
-
-If You choose to distribute Source Code Form that is Incompatible With
-Secondary Licenses under the terms of this version of the License, the
-notice described in Exhibit B of this License must be attached.
-
-Exhibit A - Source Code Form License Notice
--------------------------------------------
-
-  This Source Code Form is subject to the terms of the Mozilla Public
-  License, v. 2.0. If a copy of the MPL was not distributed with this
-  file, You can obtain one at http://mozilla.org/MPL/2.0/.
-
-If it is not possible or desirable to put the notice in a particular
-file, then You may include the notice in a location (such as a LICENSE
-file in a relevant directory) where a recipient would be likely to look
-for such a notice.
-
-You may add additional accurate notices of copyright ownership.
-
-Exhibit B - "Incompatible With Secondary Licenses" Notice
----------------------------------------------------------
-
-  This Source Code Form is "Incompatible With Secondary Licenses", as
+Mozilla Public License Version 2.0
+==================================
+
+1. Definitions
+--------------
+
+1.1. "Contributor"
+    means each individual or legal entity that creates, contributes to
+    the creation of, or owns Covered Software.
+
+1.2. "Contributor Version"
+    means the combination of the Contributions of others (if any) used
+    by a Contributor and that particular Contributor's Contribution.
+
+1.3. "Contribution"
+    means Covered Software of a particular Contributor.
+
+1.4. "Covered Software"
+    means Source Code Form to which the initial Contributor has attached
+    the notice in Exhibit A, the Executable Form of such Source Code
+    Form, and Modifications of such Source Code Form, in each case
+    including portions thereof.
+
+1.5. "Incompatible With Secondary Licenses"
+    means
+
+    (a) that the initial Contributor has attached the notice described
+        in Exhibit B to the Covered Software; or
+
+    (b) that the Covered Software was made available under the terms of
+        version 1.1 or earlier of the License, but not also under the
+        terms of a Secondary License.
+
+1.6. "Executable Form"
+    means any form of the work other than Source Code Form.
+
+1.7. "Larger Work"
+    means a work that combines Covered Software with other material, in
+    a separate file or files, that is not Covered Software.
+
+1.8. "License"
+    means this document.
+
+1.9. "Licensable"
+    means having the right to grant, to the maximum extent possible,
+    whether at the time of the initial grant or subsequently, any and
+    all of the rights conveyed by this License.
+
+1.10. "Modifications"
+    means any of the following:
+
+    (a) any file in Source Code Form that results from an addition to,
+        deletion from, or modification of the contents of Covered
+        Software; or
+
+    (b) any new file in Source Code Form that contains any Covered
+        Software.
+
+1.11. "Patent Claims" of a Contributor
+    means any patent claim(s), including without limitation, method,
+    process, and apparatus claims, in any patent Licensable by such
+    Contributor that would be infringed, but for the grant of the
+    License, by the making, using, selling, offering for sale, having
+    made, import, or transfer of either its Contributions or its
+    Contributor Version.
+
+1.12. "Secondary License"
+    means either the GNU General Public License, Version 2.0, the GNU
+    Lesser General Public License, Version 2.1, the GNU Affero General
+    Public License, Version 3.0, or any later versions of those
+    licenses.
+
+1.13. "Source Code Form"
+    means the form of the work preferred for making modifications.
+
+1.14. "You" (or "Your")
+    means an individual or a legal entity exercising rights under this
+    License. For legal entities, "You" includes any entity that
+    controls, is controlled by, or is under common control with You. For
+    purposes of this definition, "control" means (a) the power, direct
+    or indirect, to cause the direction or management of such entity,
+    whether by contract or otherwise, or (b) ownership of more than
+    fifty percent (50%) of the outstanding shares or beneficial
+    ownership of such entity.
+
+2. License Grants and Conditions
+--------------------------------
+
+2.1. Grants
+
+Each Contributor hereby grants You a world-wide, royalty-free,
+non-exclusive license:
+
+(a) under intellectual property rights (other than patent or trademark)
+    Licensable by such Contributor to use, reproduce, make available,
+    modify, display, perform, distribute, and otherwise exploit its
+    Contributions, either on an unmodified basis, with Modifications, or
+    as part of a Larger Work; and
+
+(b) under Patent Claims of such Contributor to make, use, sell, offer
+    for sale, have made, import, and otherwise transfer either its
+    Contributions or its Contributor Version.
+
+2.2. Effective Date
+
+The licenses granted in Section 2.1 with respect to any Contribution
+become effective for each Contribution on the date the Contributor first
+distributes such Contribution.
+
+2.3. Limitations on Grant Scope
+
+The licenses granted in this Section 2 are the only rights granted under
+this License. No additional rights or licenses will be implied from the
+distribution or licensing of Covered Software under this License.
+Notwithstanding Section 2.1(b) above, no patent license is granted by a
+Contributor:
+
+(a) for any code that a Contributor has removed from Covered Software;
+    or
+
+(b) for infringements caused by: (i) Your and any other third party's
+    modifications of Covered Software, or (ii) the combination of its
+    Contributions with other software (except as part of its Contributor
+    Version); or
+
+(c) under Patent Claims infringed by Covered Software in the absence of
+    its Contributions.
+
+This License does not grant any rights in the trademarks, service marks,
+or logos of any Contributor (except as may be necessary to comply with
+the notice requirements in Section 3.4).
+
+2.4. Subsequent Licenses
+
+No Contributor makes additional grants as a result of Your choice to
+distribute the Covered Software under a subsequent version of this
+License (see Section 10.2) or under the terms of a Secondary License (if
+permitted under the terms of Section 3.3).
+
+2.5. Representation
+
+Each Contributor represents that the Contributor believes its
+Contributions are its original creation(s) or it has sufficient rights
+to grant the rights to its Contributions conveyed by this License.
+
+2.6. Fair Use
+
+This License is not intended to limit any rights You have under
+applicable copyright doctrines of fair use, fair dealing, or other
+equivalents.
+
+2.7. Conditions
+
+Sections 3.1, 3.2, 3.3, and 3.4 are conditions of the licenses granted
+in Section 2.1.
+
+3. Responsibilities
+-------------------
+
+3.1. Distribution of Source Form
+
+All distribution of Covered Software in Source Code Form, including any
+Modifications that You create or to which You contribute, must be under
+the terms of this License. You must inform recipients that the Source
+Code Form of the Covered Software is governed by the terms of this
+License, and how they can obtain a copy of this License. You may not
+attempt to alter or restrict the recipients' rights in the Source Code
+Form.
+
+3.2. Distribution of Executable Form
+
+If You distribute Covered Software in Executable Form then:
+
+(a) such Covered Software must also be made available in Source Code
+    Form, as described in Section 3.1, and You must inform recipients of
+    the Executable Form how they can obtain a copy of such Source Code
+    Form by reasonable means in a timely manner, at a charge no more
+    than the cost of distribution to the recipient; and
+
+(b) You may distribute such Executable Form under the terms of this
+    License, or sublicense it under different terms, provided that the
+    license for the Executable Form does not attempt to limit or alter
+    the recipients' rights in the Source Code Form under this License.
+
+3.3. Distribution of a Larger Work
+
+You may create and distribute a Larger Work under terms of Your choice,
+provided that You also comply with the requirements of this License for
+the Covered Software. If the Larger Work is a combination of Covered
+Software with a work governed by one or more Secondary Licenses, and the
+Covered Software is not Incompatible With Secondary Licenses, this
+License permits You to additionally distribute such Covered Software
+under the terms of such Secondary License(s), so that the recipient of
+the Larger Work may, at their option, further distribute the Covered
+Software under the terms of either this License or such Secondary
+License(s).
+
+3.4. Notices
+
+You may not remove or alter the substance of any license notices
+(including copyright notices, patent notices, disclaimers of warranty,
+or limitations of liability) contained within the Source Code Form of
+the Covered Software, except that You may alter any license notices to
+the extent required to remedy known factual inaccuracies.
+
+3.5. Application of Additional Terms
+
+You may choose to offer, and to charge a fee for, warranty, support,
+indemnity or liability obligations to one or more recipients of Covered
+Software. However, You may do so only on Your own behalf, and not on
+behalf of any Contributor. You must make it absolutely clear that any
+such warranty, support, indemnity, or liability obligation is offered by
+You alone, and You hereby agree to indemnify every Contributor for any
+liability incurred by such Contributor as a result of warranty, support,
+indemnity or liability terms You offer. You may include additional
+disclaimers of warranty and limitations of liability specific to any
+jurisdiction.
+
+4. Inability to Comply Due to Statute or Regulation
+---------------------------------------------------
+
+If it is impossible for You to comply with any of the terms of this
+License with respect to some or all of the Covered Software due to
+statute, judicial order, or regulation then You must: (a) comply with
+the terms of this License to the maximum extent possible; and (b)
+describe the limitations and the code they affect. Such description must
+be placed in a text file included with all distributions of the Covered
+Software under this License. Except to the extent prohibited by statute
+or regulation, such description must be sufficiently detailed for a
+recipient of ordinary skill to be able to understand it.
+
+5. Termination
+--------------
+
+5.1. The rights granted under this License will terminate automatically
+if You fail to comply with any of its terms. However, if You become
+compliant, then the rights granted under this License from a particular
+Contributor are reinstated (a) provisionally, unless and until such
+Contributor explicitly and finally terminates Your grants, and (b) on an
+ongoing basis, if such Contributor fails to notify You of the
+non-compliance by some reasonable means prior to 60 days after You have
+come back into compliance. Moreover, Your grants from a particular
+Contributor are reinstated on an ongoing basis if such Contributor
+notifies You of the non-compliance by some reasonable means, this is the
+first time You have received notice of non-compliance with this License
+from such Contributor, and You become compliant prior to 30 days after
+Your receipt of the notice.
+
+5.2. If You initiate litigation against any entity by asserting a patent
+infringement claim (excluding declaratory judgment actions,
+counter-claims, and cross-claims) alleging that a Contributor Version
+directly or indirectly infringes any patent, then the rights granted to
+You by any and all Contributors for the Covered Software under Section
+2.1 of this License shall terminate.
+
+5.3. In the event of termination under Sections 5.1 or 5.2 above, all
+end user license agreements (excluding distributors and resellers) which
+have been validly granted by You or Your distributors under this License
+prior to termination shall survive termination.
+
+************************************************************************
+*                                                                      *
+*  6. Disclaimer of Warranty                                           *
+*  -------------------------                                           *
+*                                                                      *
+*  Covered Software is provided under this License on an "as is"       *
+*  basis, without warranty of any kind, either expressed, implied, or  *
+*  statutory, including, without limitation, warranties that the       *
+*  Covered Software is free of defects, merchantable, fit for a        *
+*  particular purpose or non-infringing. The entire risk as to the     *
+*  quality and performance of the Covered Software is with You.        *
+*  Should any Covered Software prove defective in any respect, You     *
+*  (not any Contributor) assume the cost of any necessary servicing,   *
+*  repair, or correction. This disclaimer of warranty constitutes an   *
+*  essential part of this License. No use of any Covered Software is   *
+*  authorized under this License except under this disclaimer.         *
+*                                                                      *
+************************************************************************
+
+************************************************************************
+*                                                                      *
+*  7. Limitation of Liability                                          *
+*  --------------------------                                          *
+*                                                                      *
+*  Under no circumstances and under no legal theory, whether tort      *
+*  (including negligence), contract, or otherwise, shall any           *
+*  Contributor, or anyone who distributes Covered Software as          *
+*  permitted above, be liable to You for any direct, indirect,         *
+*  special, incidental, or consequential damages of any character      *
+*  including, without limitation, damages for lost profits, loss of    *
+*  goodwill, work stoppage, computer failure or malfunction, or any    *
+*  and all other commercial damages or losses, even if such party      *
+*  shall have been informed of the possibility of such damages. This   *
+*  limitation of liability shall not apply to liability for death or   *
+*  personal injury resulting from such party's negligence to the       *
+*  extent applicable law prohibits such limitation. Some               *
+*  jurisdictions do not allow the exclusion or limitation of           *
+*  incidental or consequential damages, so this exclusion and          *
+*  limitation may not apply to You.                                    *
+*                                                                      *
+************************************************************************
+
+8. Litigation
+-------------
+
+Any litigation relating to this License may be brought only in the
+courts of a jurisdiction where the defendant maintains its principal
+place of business and such litigation shall be governed by laws of that
+jurisdiction, without reference to its conflict-of-law provisions.
+Nothing in this Section shall prevent a party's ability to bring
+cross-claims or counter-claims.
+
+9. Miscellaneous
+----------------
+
+This License represents the complete agreement concerning the subject
+matter hereof. If any provision of this License is held to be
+unenforceable, such provision shall be reformed only to the extent
+necessary to make it enforceable. Any law or regulation which provides
+that the language of a contract shall be construed against the drafter
+shall not be used to construe this License against a Contributor.
+
+10. Versions of the License
+---------------------------
+
+10.1. New Versions
+
+Mozilla Foundation is the license steward. Except as provided in Section
+10.3, no one other than the license steward has the right to modify or
+publish new versions of this License. Each version will be given a
+distinguishing version number.
+
+10.2. Effect of New Versions
+
+You may distribute the Covered Software under the terms of the version
+of the License under which You originally received the Covered Software,
+or under the terms of any subsequent version published by the license
+steward.
+
+10.3. Modified Versions
+
+If you create software not governed by this License, and you want to
+create a new license for such software, you may create and use a
+modified version of this License if you rename the license and remove
+any references to the name of the license steward (except to note that
+such modified license differs from this License).
+
+10.4. Distributing Source Code Form that is Incompatible With Secondary
+Licenses
+
+If You choose to distribute Source Code Form that is Incompatible With
+Secondary Licenses under the terms of this version of the License, the
+notice described in Exhibit B of this License must be attached.
+
+Exhibit A - Source Code Form License Notice
+-------------------------------------------
+
+  This Source Code Form is subject to the terms of the Mozilla Public
+  License, v. 2.0. If a copy of the MPL was not distributed with this
+  file, You can obtain one at http://mozilla.org/MPL/2.0/.
+
+If it is not possible or desirable to put the notice in a particular
+file, then You may include the notice in a location (such as a LICENSE
+file in a relevant directory) where a recipient would be likely to look
+for such a notice.
+
+You may add additional accurate notices of copyright ownership.
+
+Exhibit B - "Incompatible With Secondary Licenses" Notice
+---------------------------------------------------------
+
+  This Source Code Form is "Incompatible With Secondary Licenses", as
   defined by the Mozilla Public License, v. 2.0.
```

### Comparing `discord-ext-pager-1.0.0/PKG-INFO` & `discord-ext-pager-1.0.0.post1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,132 +1,140 @@
-Metadata-Version: 2.1
-Name: discord-ext-pager
-Version: 1.0.0
-Summary: A view-based paginator library for discord.py 2.0
-Author: thegamecracks
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Framework :: AsyncIO
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved
-Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Software Development
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Typing :: Typed
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# discord-ext-pager
-
-A simple view-based paginator library for discord.py 2.0.
-
-## Installation
-
-This package is available on pip as `discord-ext-pager`.
-If you have Git, you may also choose to install the latest version
-using `pip install git+https://github.com/thegamecracks/discord-ext-pager`.
-
-## Basic Usage
-
-Prior users of Danny's [`discord-ext-menus`] will find some familiarity
-in this library. Provided are the following classes:
-
-- PaginatorView:
-  The view class that manages the paginator.
-- PageSource:
-  The base class for sources the paginator view can accept.
-- ListPageSource:
-  The base class for formatting a list of items.
-- AsyncIteratorPageSource:
-  The base class for formatting an asynchronous iterator of items.
-- PageOption:
-  A subclass of `discord.SelectOption` that also stores a `PageSource` instance.
-  Used for the navigation select menu.
-- TimeoutAction:
-  An enum for customizing PaginatorView's timeout behaviour.
-
-The `PaginatorView` can be instantiated and used by itself, but page formatting
-is handled by subclassing one of the `PageSource` base classes.
-
-```py
-from typing import Any, List
-from discord.ext.pager import ListPageSource, PaginatorView
-
-class EmbedListPageSource(ListPageSource[Any, None, PaginatorView]):
-    """Takes a list of items and formats it in an embed."""
-
-    def format_page(self, view: PaginatorView, page: List[Any]):
-        index = self.current_index * self.page_size
-        description = "\n".join(
-            f"{i}. {x}"
-            for i, x in enumerate(page, start=index + 1)
-        )
-        return discord.Embed(description=description)
-
-# Anywhere a channel or interaction is available:
-fruits = ["🍎 Apple", "🍊 Orange", "🍋 Lemon"]
-source = EmbedListPageSource(fruits, page_size=2)
-view = PaginatorView(sources=source, timeout=180)
-await view.start(interaction)
-```
-
-If the navigation select menu is desired, the `get_page_options()` method
-should be overridden to return a list of `PageOption` objects for the user
-to select from:
-
-```py
-from typing import List
-from discord.ext.pager import ListPageSource, PageOption, PaginatorView, PageSource
-
-class MessageSource(PageSource[str, None, PaginatorView]):
-    """A single page for displaying a string."""
-
-    def __init__(self, message: str, *, current_index: int = 0):
-        super().__init__(current_index=current_index)
-        self.message = message
-
-    def get_page(self, index: int):
-        return self.message
-
-    def format_page(self, view: PaginatorView, page: str):
-        # If we don't specify both content and embed, either will
-        # persist as the user clicks between options
-        return {"content": page, "embed": None}
-
-class MessageNavigator(ListPageSource[MessageSource, MessageSource, PaginatorView]):
-    """A list of messages for the user to select from."""
-
-    def get_page_options(self, view: PaginatorView, page: List[MessageSource]):
-        return [PageOption(source=source, label=source.message) for source in page]
-
-    def format_page(self, view: PaginatorView, page: List[MessageSource]):
-        description = "\n".join(source.message for source in page)
-        embed = discord.Embed(description=description)
-        return {"content": None, "embed": embed}
-
-hands = "👈👉👆👇🫵🤞🫰🤘🤙🤛🤜✊👊👋👏🙌"
-source = MessageNavigator([MessageSource(s) for s in hands], page_size=5)
-view = PaginatorView(sources=source)
-await view.start(ctx)
-```
-
-When an option is selected, the `PageSource` contained within that option
-is appended to `PaginatorView.sources`, causing that source to be displayed.
-Another button is automatically provided for users to back out to the last
-page source. This can be manually triggered by passing a list of page sources
-to the `PaginatorView(sources=)` argument.
-
-[`discord-ext-menus`]: https://github.com/Rapptz/discord-ext-menus
-
-## Examples
-
-Click on each example to see the source code:
-
-[![Tag leaderboard](https://github.com/thegamecracks/discord-ext-pager/blob/main/docs/images/thegamebot_tags.png?raw=true)](https://github.com/thegamecracks/thegamebot/blob/04d9909877685acd24654a911b1853e2143fc316/bot/cogs/tags/__init__.py#L123-L162)
-
-[![Help command](https://github.com/thegamecracks/discord-ext-pager/blob/main/docs/images/thegamebot_help.png?raw=true)](https://github.com/thegamecracks/thegamebot/blob/04d9909877685acd24654a911b1853e2143fc316/bot/cogs/helpcommand.py#L26-L249)
+Metadata-Version: 2.1
+Name: discord-ext-pager
+Version: 1.0.0.post1
+Summary: A view-based paginator library for discord.py 2.0
+Author: thegamecracks
+Keywords: discord,discord.py,paginator,view
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Framework :: AsyncIO
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved
+Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Typing :: Typed
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# discord-ext-pager
+
+[![PyPI](https://img.shields.io/pypi/v/discord-ext-pager?label=View%20on%20pypi&style=flat-square)](https://pypi.org/project/discord-ext-pager/)
+
+A simple view-based paginator library for discord.py 2.0.
+
+## Installation
+
+[discord-ext-pager] is available on PyPI, and as such can be installed using pip.
+
+[discord-ext-pager]: https://pypi.org/project/discord-ext-pager/
+
+## Usage
+
+Users of Danny's [discord-ext-menus] will find some familiarity
+in this library. Provided are the following classes:
+
+- PaginatorView:
+  The view class that manages pagination and navigation.
+- PageSource:
+  The base class for sources the paginator view can accept.
+- ListPageSource:
+  The base class for formatting a list of items.
+- AsyncIteratorPageSource:
+  The base class for formatting an asynchronous iterator of items.
+- PageOption:
+  A subclass of `discord.SelectOption` used for presenting navigation options.
+- TimeoutAction:
+  An enum for customizing PaginatorView's timeout behaviour.
+
+[discord-ext-menus]: https://github.com/Rapptz/discord-ext-menus
+
+The `PaginatorView` can be instantiated and used by itself, but page formatting
+is handled by subclassing one of the `PageSource` base classes.
+
+```py
+from typing import Any, List
+from discord.ext.pager import ListPageSource, PaginatorView
+
+class EmbedListPageSource(ListPageSource[Any, None, PaginatorView]):
+    #                                   ^^^^^^^^^^^^^^^^^^^^^^^^^^
+    #            These type parameters denote the page item type,
+    #            source type for page options (demonstrated later),
+    #            and view type. Only needed for static typing.
+    """Takes a list of items and formats it in an embed."""
+
+    def format_page(self, view: PaginatorView, page: List[Any]):
+        index = self.current_index * self.page_size
+        description = "\n".join(
+            f"{i}. {x}"
+            for i, x in enumerate(page, start=index + 1)
+        )
+        return discord.Embed(description=description)
+
+# Anywhere a channel or interaction is available:
+fruits = ["🍎 Apple", "🍊 Orange", "🍋 Lemon"]
+source = EmbedListPageSource(fruits, page_size=2)
+view = PaginatorView(sources=source, timeout=180)
+await view.start(interaction)
+```
+
+If the navigation select menu is desired, the `get_page_options()` method
+should be overridden to return a list of `PageOption` objects for the user
+to select from:
+
+```py
+from typing import List
+from discord.ext.pager import ListPageSource, PageOption, PageSource, PaginatorView
+
+class MessageSource(PageSource[str, None, PaginatorView]):
+    """A single page for displaying a string."""
+
+    def __init__(self, message: str, *, current_index: int = 0):
+        super().__init__(current_index=current_index)
+        self.message = message
+
+    def get_page(self, index: int):
+        return self.message
+
+    def format_page(self, view: PaginatorView, page: str):
+        # If we don't specify both content and embed, either will
+        # persist as the user clicks between options
+        return {"content": page, "embed": None}
+
+class MessageNavigator(ListPageSource[MessageSource, MessageSource, PaginatorView]):
+    """A list of messages for the user to select from."""
+
+    def get_page_options(self, view: PaginatorView, page: List[MessageSource]):
+        # PageOption() takes the same arguments as discord.SelectOption,
+        # except that source= is also required
+        return [PageOption(source=source, label=source.message) for source in page]
+
+    def format_page(self, view: PaginatorView, page: List[MessageSource]):
+        description = "\n".join(source.message for source in page)
+        embed = discord.Embed(description=description)
+        return {"content": None, "embed": embed}
+
+hands = "👈👉👆👇🫵🤞🫰🤘🤙🤛🤜✊👊👋👏🙌"
+source = MessageNavigator([MessageSource(s) for s in hands], page_size=5)
+view = PaginatorView(sources=source)
+await view.start(ctx)
+```
+
+When an option is selected, the `PageSource` contained within that option
+is appended to `PaginatorView.sources`, causing that source to be displayed.
+Another button is automatically provided for users to back out to the last
+page source. This can be manually triggered by passing a list of page sources
+to the `PaginatorView(sources=)` argument.
+
+## Examples
+
+Click on an example below to see its source code:
+
+[![Tag leaderboard](https://github.com/thegamecracks/discord-ext-pager/blob/main/docs/images/thegamebot_tags.png?raw=true)](https://github.com/thegamecracks/thegamebot/blob/04d9909877685acd24654a911b1853e2143fc316/bot/cogs/tags/__init__.py#L123-L162)
+
+[![Help command](https://github.com/thegamecracks/discord-ext-pager/blob/main/docs/images/thegamebot_help.png?raw=true)](https://github.com/thegamecracks/thegamebot/blob/04d9909877685acd24654a911b1853e2143fc316/bot/cogs/helpcommand.py#L26-L249)
```

### Comparing `discord-ext-pager-1.0.0/README.md` & `discord-ext-pager-1.0.0.post1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,109 +1,116 @@
-# discord-ext-pager
-
-A simple view-based paginator library for discord.py 2.0.
-
-## Installation
-
-This package is available on pip as `discord-ext-pager`.
-If you have Git, you may also choose to install the latest version
-using `pip install git+https://github.com/thegamecracks/discord-ext-pager`.
-
-## Basic Usage
-
-Prior users of Danny's [`discord-ext-menus`] will find some familiarity
-in this library. Provided are the following classes:
-
-- PaginatorView:
-  The view class that manages the paginator.
-- PageSource:
-  The base class for sources the paginator view can accept.
-- ListPageSource:
-  The base class for formatting a list of items.
-- AsyncIteratorPageSource:
-  The base class for formatting an asynchronous iterator of items.
-- PageOption:
-  A subclass of `discord.SelectOption` that also stores a `PageSource` instance.
-  Used for the navigation select menu.
-- TimeoutAction:
-  An enum for customizing PaginatorView's timeout behaviour.
-
-The `PaginatorView` can be instantiated and used by itself, but page formatting
-is handled by subclassing one of the `PageSource` base classes.
-
-```py
-from typing import Any, List
-from discord.ext.pager import ListPageSource, PaginatorView
-
-class EmbedListPageSource(ListPageSource[Any, None, PaginatorView]):
-    """Takes a list of items and formats it in an embed."""
-
-    def format_page(self, view: PaginatorView, page: List[Any]):
-        index = self.current_index * self.page_size
-        description = "\n".join(
-            f"{i}. {x}"
-            for i, x in enumerate(page, start=index + 1)
-        )
-        return discord.Embed(description=description)
-
-# Anywhere a channel or interaction is available:
-fruits = ["🍎 Apple", "🍊 Orange", "🍋 Lemon"]
-source = EmbedListPageSource(fruits, page_size=2)
-view = PaginatorView(sources=source, timeout=180)
-await view.start(interaction)
-```
-
-If the navigation select menu is desired, the `get_page_options()` method
-should be overridden to return a list of `PageOption` objects for the user
-to select from:
-
-```py
-from typing import List
-from discord.ext.pager import ListPageSource, PageOption, PaginatorView, PageSource
-
-class MessageSource(PageSource[str, None, PaginatorView]):
-    """A single page for displaying a string."""
-
-    def __init__(self, message: str, *, current_index: int = 0):
-        super().__init__(current_index=current_index)
-        self.message = message
-
-    def get_page(self, index: int):
-        return self.message
-
-    def format_page(self, view: PaginatorView, page: str):
-        # If we don't specify both content and embed, either will
-        # persist as the user clicks between options
-        return {"content": page, "embed": None}
-
-class MessageNavigator(ListPageSource[MessageSource, MessageSource, PaginatorView]):
-    """A list of messages for the user to select from."""
-
-    def get_page_options(self, view: PaginatorView, page: List[MessageSource]):
-        return [PageOption(source=source, label=source.message) for source in page]
-
-    def format_page(self, view: PaginatorView, page: List[MessageSource]):
-        description = "\n".join(source.message for source in page)
-        embed = discord.Embed(description=description)
-        return {"content": None, "embed": embed}
-
-hands = "👈👉👆👇🫵🤞🫰🤘🤙🤛🤜✊👊👋👏🙌"
-source = MessageNavigator([MessageSource(s) for s in hands], page_size=5)
-view = PaginatorView(sources=source)
-await view.start(ctx)
-```
-
-When an option is selected, the `PageSource` contained within that option
-is appended to `PaginatorView.sources`, causing that source to be displayed.
-Another button is automatically provided for users to back out to the last
-page source. This can be manually triggered by passing a list of page sources
-to the `PaginatorView(sources=)` argument.
-
-[`discord-ext-menus`]: https://github.com/Rapptz/discord-ext-menus
-
-## Examples
-
-Click on each example to see the source code:
-
-[![Tag leaderboard](https://github.com/thegamecracks/discord-ext-pager/blob/main/docs/images/thegamebot_tags.png?raw=true)](https://github.com/thegamecracks/thegamebot/blob/04d9909877685acd24654a911b1853e2143fc316/bot/cogs/tags/__init__.py#L123-L162)
-
-[![Help command](https://github.com/thegamecracks/discord-ext-pager/blob/main/docs/images/thegamebot_help.png?raw=true)](https://github.com/thegamecracks/thegamebot/blob/04d9909877685acd24654a911b1853e2143fc316/bot/cogs/helpcommand.py#L26-L249)
+# discord-ext-pager
+
+[![PyPI](https://img.shields.io/pypi/v/discord-ext-pager?label=View%20on%20pypi&style=flat-square)](https://pypi.org/project/discord-ext-pager/)
+
+A simple view-based paginator library for discord.py 2.0.
+
+## Installation
+
+[discord-ext-pager] is available on PyPI, and as such can be installed using pip.
+
+[discord-ext-pager]: https://pypi.org/project/discord-ext-pager/
+
+## Usage
+
+Users of Danny's [discord-ext-menus] will find some familiarity
+in this library. Provided are the following classes:
+
+- PaginatorView:
+  The view class that manages pagination and navigation.
+- PageSource:
+  The base class for sources the paginator view can accept.
+- ListPageSource:
+  The base class for formatting a list of items.
+- AsyncIteratorPageSource:
+  The base class for formatting an asynchronous iterator of items.
+- PageOption:
+  A subclass of `discord.SelectOption` used for presenting navigation options.
+- TimeoutAction:
+  An enum for customizing PaginatorView's timeout behaviour.
+
+[discord-ext-menus]: https://github.com/Rapptz/discord-ext-menus
+
+The `PaginatorView` can be instantiated and used by itself, but page formatting
+is handled by subclassing one of the `PageSource` base classes.
+
+```py
+from typing import Any, List
+from discord.ext.pager import ListPageSource, PaginatorView
+
+class EmbedListPageSource(ListPageSource[Any, None, PaginatorView]):
+    #                                   ^^^^^^^^^^^^^^^^^^^^^^^^^^
+    #            These type parameters denote the page item type,
+    #            source type for page options (demonstrated later),
+    #            and view type. Only needed for static typing.
+    """Takes a list of items and formats it in an embed."""
+
+    def format_page(self, view: PaginatorView, page: List[Any]):
+        index = self.current_index * self.page_size
+        description = "\n".join(
+            f"{i}. {x}"
+            for i, x in enumerate(page, start=index + 1)
+        )
+        return discord.Embed(description=description)
+
+# Anywhere a channel or interaction is available:
+fruits = ["🍎 Apple", "🍊 Orange", "🍋 Lemon"]
+source = EmbedListPageSource(fruits, page_size=2)
+view = PaginatorView(sources=source, timeout=180)
+await view.start(interaction)
+```
+
+If the navigation select menu is desired, the `get_page_options()` method
+should be overridden to return a list of `PageOption` objects for the user
+to select from:
+
+```py
+from typing import List
+from discord.ext.pager import ListPageSource, PageOption, PageSource, PaginatorView
+
+class MessageSource(PageSource[str, None, PaginatorView]):
+    """A single page for displaying a string."""
+
+    def __init__(self, message: str, *, current_index: int = 0):
+        super().__init__(current_index=current_index)
+        self.message = message
+
+    def get_page(self, index: int):
+        return self.message
+
+    def format_page(self, view: PaginatorView, page: str):
+        # If we don't specify both content and embed, either will
+        # persist as the user clicks between options
+        return {"content": page, "embed": None}
+
+class MessageNavigator(ListPageSource[MessageSource, MessageSource, PaginatorView]):
+    """A list of messages for the user to select from."""
+
+    def get_page_options(self, view: PaginatorView, page: List[MessageSource]):
+        # PageOption() takes the same arguments as discord.SelectOption,
+        # except that source= is also required
+        return [PageOption(source=source, label=source.message) for source in page]
+
+    def format_page(self, view: PaginatorView, page: List[MessageSource]):
+        description = "\n".join(source.message for source in page)
+        embed = discord.Embed(description=description)
+        return {"content": None, "embed": embed}
+
+hands = "👈👉👆👇🫵🤞🫰🤘🤙🤛🤜✊👊👋👏🙌"
+source = MessageNavigator([MessageSource(s) for s in hands], page_size=5)
+view = PaginatorView(sources=source)
+await view.start(ctx)
+```
+
+When an option is selected, the `PageSource` contained within that option
+is appended to `PaginatorView.sources`, causing that source to be displayed.
+Another button is automatically provided for users to back out to the last
+page source. This can be manually triggered by passing a list of page sources
+to the `PaginatorView(sources=)` argument.
+
+## Examples
+
+Click on an example below to see its source code:
+
+[![Tag leaderboard](https://github.com/thegamecracks/discord-ext-pager/blob/main/docs/images/thegamebot_tags.png?raw=true)](https://github.com/thegamecracks/thegamebot/blob/04d9909877685acd24654a911b1853e2143fc316/bot/cogs/tags/__init__.py#L123-L162)
+
+[![Help command](https://github.com/thegamecracks/discord-ext-pager/blob/main/docs/images/thegamebot_help.png?raw=true)](https://github.com/thegamecracks/thegamebot/blob/04d9909877685acd24654a911b1853e2143fc316/bot/cogs/helpcommand.py#L26-L249)
```

### Comparing `discord-ext-pager-1.0.0/src/discord/ext/pager/__init__.py` & `discord-ext-pager-1.0.0.post1/src/discord/ext/pager/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,495 +1,495 @@
-#  Copyright (C) 2023 thegamecracks
-#  This Source Code Form is subject to the terms of the Mozilla Public
-#  License, v. 2.0. If a copy of the MPL was not distributed with this
-#  file, You can obtain one at http://mozilla.org/MPL/2.0/.
-import functools
-import math
-from abc import ABC, abstractmethod
-from enum import Enum, auto
-from typing import (
-    Any,
-    AsyncIterator,
-    Collection,
-    Coroutine,
-    Dict,
-    Generic,
-    Iterable,
-    List,
-    Optional,
-    Sequence,
-    Tuple,
-    TypedDict,
-    TypeVar,
-    Union,
-    cast,
-)
-
-import discord
-from typing_extensions import TypeAlias
-
-__version__ = "1.0.0"
-
-__all__ = (
-    "PageOption",
-    "PageSource",
-    "ListPageSource",
-    "AsyncIteratorPageSource",
-    "TimeoutAction",
-    "PaginatorView",
-)
-
-E = TypeVar("E")
-T = TypeVar("T")
-S_co = TypeVar("S_co", bound="PageSource", covariant=True)
-V_contra = TypeVar("V_contra", bound="PaginatorView", contravariant=True)
-FP: TypeAlias = "Union[_PageParams, str, discord.Embed]"
-PO: TypeAlias = "Sequence[PageOption[S_co]]"
-
-
-class _PageParams(TypedDict, total=False):
-    content: str
-    embed: discord.Embed
-
-
-class PageOption(discord.SelectOption, Generic[S_co]):
-    """A select option that can store a nested page
-    through the added `source=` kwarg.
-    """
-
-    def __init__(self, *args, source: S_co, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.source = source
-
-
-class PageSource(ABC, Generic[T, S_co, V_contra]):
-    """The base page source class."""
-
-    def __init__(self, *, current_index: int = 0):
-        self.current_index = current_index
-
-    @abstractmethod
-    def get_page(self, index: int) -> Union[T, Coroutine[None, None, T]]:
-        """Returns a page based on the given index.
-
-        This method may be asynchronous.
-
-        """
-
-    @property
-    def max_pages(self) -> int:
-        """The max number of pages the page source can return.
-
-        Can return 0 to disable the view entirely.
-
-        """
-        return 1
-
-    def get_page_options(
-        self,
-        view: V_contra,
-        page: T,
-    ) -> Union[PO, Coroutine[None, None, PO]]:
-        """Returns a list of page options for the user to select.
-
-        This method may be asynchronous.
-
-        """
-        return []
-
-    @abstractmethod
-    def format_page(
-        self,
-        view: V_contra,
-        page: T,
-    ) -> Union[FP, Coroutine[None, None, FP]]:
-        """Returns a dictionary presenting the items in the page.
-
-        This method may be asynchronous.
-
-        """
-
-
-class ListPageSource(
-    PageSource[List[E], S_co, V_contra],
-    ABC,
-    Generic[E, S_co, V_contra],
-):
-    """Paginates a list of elements."""
-
-    def __init__(self, items: List[E], *args, page_size: int, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.items = items
-        self.page_size = page_size
-
-    def get_page(self, index: int) -> List[E]:
-        start = index * self.page_size
-        return self.items[start : start + self.page_size]
-
-    @functools.cached_property
-    def max_pages(self) -> int:
-        pages, remainder = divmod(len(self.items), self.page_size)
-        return pages + bool(remainder)
-
-
-class AsyncIteratorPageSource(
-    PageSource[List[E], S_co, V_contra],
-    ABC,
-    Generic[E, S_co, V_contra],
-):
-    """Paginates an async iterator."""
-
-    def __init__(self, iterator: AsyncIterator[E], *args, page_size: int, **kwargs):
-        super().__init__(*args, **kwargs)
-        self._cache: list[E] = []
-        self._iterator = iterator
-        self._max_index = 0
-        self._exhausted = False
-        self.page_size = page_size
-
-    async def get_page(self, index: int) -> List[E]:
-        start = index * self.page_size
-        end = start + self.page_size
-        if self._exhausted:
-            return self._cache[start:end]
-
-        # Get enough items to have at least one extra page
-        # so paginator knows if next/last buttons should turn off
-        required = end + self.page_size - len(self._cache)
-        if required > 0:
-            new_items = []
-            max_index = index + 1
-            for i in range(required):
-                try:
-                    new_items.append(await self._iterator.__anext__())
-                except StopAsyncIteration:
-                    max_index = math.ceil((len(self._cache) + i) / self.page_size)
-                    self._exhausted = True
-                    break
-            self._cache.extend(new_items)
-            self._max_index = max_index
-
-        return self._cache[start:end]
-
-    @property
-    def max_pages(self) -> int:
-        return self._max_index + (not self._exhausted)
-
-
-class TimeoutAction(Enum):
-    """Specifies what action should be taken when the view times out."""
-
-    NONE = auto()
-    """On timeout, no action will occur on the message."""
-    DISABLE = auto()
-    """On timeout, all components will be disabled."""
-    CLEAR = auto()
-    """On timeout, all components will be removed from the message."""
-    DELETE = auto()
-    """On timeout, the message will be deleted."""
-
-
-class PaginatorView(discord.ui.View, Generic[T, S_co, V_contra]):
-    """A view that handles pagination and recursive levels of pages.
-
-    To use this view, pass a PageSource or list of PageSources
-    (the last one will be displayed first) to the `sources=` kwarg,
-    then begin the paginator using `await view.start(channel)`.
-
-    If adding the view to another message is desired,
-    `view.message` must be manually set for it to be accessible.
-    The initial page is not rendered until the user interacts
-    with the paginator or is explicitly done with `await view.show_page()`.
-
-    `interaction_check` by default will return True if `allowed_users`
-    is None, or the interaction user is one of the allowed users.
-    This may be extended to include an interaction response, or use
-    different behavior entirely.
-
-    Parameters
-    ----------
-    :param sources: The current stack of page sources.
-    :param allowed_users: A collection of user IDs that are allowed
-        to interact with this paginator. If None, any user can interact.
-    :param timeout_action:
-        The action to do when the view times out. This may not have any
-        effect if a subclass overrides the `on_timeout()` method.
-
-    """
-
-    def __init__(
-        self,
-        *args,
-        sources: Union[
-            Iterable[PageSource[T, S_co, V_contra]],
-            PageSource[T, S_co, V_contra],
-        ],
-        allowed_users: Optional[Collection[int]] = None,
-        timeout_action: TimeoutAction = TimeoutAction.CLEAR,
-        **kwargs,
-    ):
-        super().__init__(*args, **kwargs)
-        if isinstance(sources, PageSource):
-            sources = [sources]
-        else:
-            self.sources = list(sources)
-            if len(self.sources) == 0:
-                raise ValueError("must provide at least one page source")
-        self.allowed_users = allowed_users
-        self.timeout_action = timeout_action
-
-        self.message: Optional[discord.Message] = None
-        self.page: _PageParams = {}
-        self.options: Sequence[PageOption[S_co]] = []
-        self.option_sources: dict[str, PageSource] = {}
-
-    @property
-    def current_source(self) -> PageSource[T, S_co, V_contra]:
-        return self.sources[-1]
-
-    @property
-    def current_index(self) -> int:
-        return self.current_source.current_index
-
-    @current_index.setter
-    def current_index(self, index: int):
-        self.current_source.current_index = index
-
-    @property
-    def can_navigate(self) -> bool:
-        return len(self.options) > 0
-
-    @property
-    def can_paginate(self) -> bool:
-        return self.current_source.max_pages > 1
-
-    @property
-    def can_go_back(self) -> bool:
-        return len(self.sources) > 1
-
-    @functools.cached_property
-    def _pagination_buttons(self) -> Tuple[discord.ui.Button, ...]:
-        return self.first_page, self.prev_page, self.next_page, self.last_page
-
-    async def show_page(self, index: int) -> None:
-        self.current_index = index
-        maybe_coro = discord.utils.maybe_coroutine
-
-        page = await maybe_coro(self.current_source.get_page, index)
-        params = await maybe_coro(self.current_source.format_page, self, page)  # type: ignore
-        if isinstance(params, str):
-            params = {"content": params}
-        elif isinstance(params, discord.Embed):
-            params = {"embed": params}
-        elif not isinstance(params, dict):
-            raise TypeError("format_page() must return a dict, str, or Embed")
-        self.page = cast(_PageParams, params)
-
-        options: Sequence[PageOption[S_co]] = await maybe_coro(
-            self.current_source.get_page_options, self, page  # type: ignore
-        )
-        option_sources = {}
-        for i, option in enumerate(options):
-            option.value = str(i)
-            option_sources[option.value] = option.source
-        self.options = options
-        self.option_sources = option_sources
-
-        self._refresh_components()
-
-    async def start(
-        self,
-        channel: Union[discord.abc.Messageable, discord.Interaction],
-        ephemeral: bool = True,
-    ) -> None:
-        await self.show_page(self.current_source.current_index)
-        if isinstance(channel, discord.Interaction):
-            kwargs = self._get_message_kwargs(initial_response=True)
-
-            if channel.response.is_done():
-                self.message = await channel.followup.send(
-                    ephemeral=ephemeral,
-                    wait=True,
-                    **kwargs,
-                )
-            else:
-                await channel.response.send_message(ephemeral=ephemeral, **kwargs)
-                self.message = await channel.original_response()
-        else:
-            self.message = await channel.send(**self._get_message_kwargs())
-
-    async def interaction_check(self, interaction: discord.Interaction) -> bool:
-        if self.allowed_users is not None:
-            return interaction.user.id in self.allowed_users
-        return True
-
-    async def on_timeout(self) -> None:
-        action = self.timeout_action
-        if self.message is None or action is TimeoutAction.NONE:
-            return
-
-        if action is TimeoutAction.CLEAR:
-            await self.message.edit(view=None)
-        elif action is TimeoutAction.DELETE:
-            await self.message.delete()
-        elif action is TimeoutAction.DISABLE:
-            for item in self.children:
-                if hasattr(item, "disabled"):
-                    item.disabled = True  # type: ignore
-
-            await self.message.edit(view=self)
-        else:
-            raise TypeError(f"unknown timeout action: {action!r}")
-
-    def _get_message_kwargs(self, *, initial_response: bool = False) -> Dict[str, Any]:
-        # initial_response indicates if we can use view=None, necessary as
-        # InteractionResponse.send_message() does not accept view=None
-        kwargs = dict(self.page)
-        max_pages = self.current_source.max_pages
-        can_interact = self.can_navigate or self.can_paginate or self.can_go_back
-
-        if max_pages > 0 and can_interact:
-            kwargs["view"] = self
-        else:
-            self.stop()
-            if not initial_response:
-                kwargs["view"] = None
-
-        return kwargs
-
-    async def _respond(self, interaction: discord.Interaction) -> None:
-        await interaction.response.edit_message(**self._get_message_kwargs())
-
-    # noinspection PyUnresolvedReferences
-    def _refresh_components(self) -> None:
-        """Update the state of each component in this view according to
-        the current source and page.
-
-        The pagination and back/stop buttons will be organized one of four ways:
-
-        1. No pagination, no previous source::
-            STOP
-        2. No pagination, previous source::
-            BACK STOP
-        3. Pagination, no previous source::
-            FIRST PREV NEXT LAST STOP
-        4. Pagination, previous source::
-            FIRST PREV NEXT LAST STOP
-            BACK
-
-        This applies the same when navigation is enabled.
-
-        """
-        self.clear_items()
-
-        # Navigation (select menu)
-        if self.can_navigate:
-            self.add_item(self.navigate)
-            self.navigate.options = list(self.options)
-
-        # Pagination (left/right)
-        if self.can_paginate:
-            for button in self._pagination_buttons:
-                self.add_item(button)
-
-        on_first_page = self.current_index == 0
-        on_last_page = self.current_index + 1 >= self.current_source.max_pages
-        self.first_page.disabled = on_first_page
-        self.prev_page.disabled = on_first_page
-        self.next_page.disabled = on_last_page
-        self.last_page.disabled = on_last_page
-
-        # Back and stop buttons
-        if self.can_go_back:
-            self.back_button.row = 1 + self.can_paginate
-            self.add_item(self.back_button)
-        self.add_item(self.stop_button)
-
-    @discord.ui.select(options=[], placeholder="Navigate...", row=0)
-    async def navigate(
-        self,
-        interaction: discord.Interaction,
-        select: discord.ui.Select,
-    ) -> None:
-        source = self.option_sources[select.values[0]]
-        self.sources.append(source)
-        await self.show_page(self.current_index)
-        await self._respond(interaction)
-
-    @discord.ui.button(
-        emoji="\N{BLACK LEFT-POINTING DOUBLE TRIANGLE WITH VERTICAL BAR}",
-        style=discord.ButtonStyle.blurple,
-        row=1,
-    )
-    async def first_page(
-        self,
-        interaction: discord.Interaction,
-        button: discord.ui.Button,
-    ) -> None:
-        await self.show_page(0)
-        await self._respond(interaction)
-
-    @discord.ui.button(
-        emoji="\N{BLACK LEFT-POINTING TRIANGLE}",
-        style=discord.ButtonStyle.blurple,
-        row=1,
-    )
-    async def prev_page(
-        self,
-        interaction: discord.Interaction,
-        button: discord.ui.Button,
-    ) -> None:
-        await self.show_page(self.current_index - 1)
-        await self._respond(interaction)
-
-    @discord.ui.button(
-        emoji="\N{BLACK RIGHT-POINTING TRIANGLE}",
-        style=discord.ButtonStyle.blurple,
-        row=1,
-    )
-    async def next_page(
-        self,
-        interaction: discord.Interaction,
-        button: discord.ui.Button,
-    ) -> None:
-        await self.show_page(self.current_index + 1)
-        await self._respond(interaction)
-
-    @discord.ui.button(
-        emoji="\N{BLACK RIGHT-POINTING DOUBLE TRIANGLE WITH VERTICAL BAR}",
-        style=discord.ButtonStyle.blurple,
-        row=1,
-    )
-    async def last_page(
-        self,
-        interaction: discord.Interaction,
-        button: discord.ui.Button,
-    ) -> None:
-        await self.show_page(self.current_source.max_pages - 1)
-        await self._respond(interaction)
-
-    @discord.ui.button(
-        emoji="\N{THUMBS UP SIGN}",
-        style=discord.ButtonStyle.success,
-        row=1,
-    )
-    async def stop_button(
-        self,
-        interaction: discord.Interaction,
-        button: discord.ui.Button,
-    ) -> None:
-        self.stop()
-        await interaction.message.delete()  # type: ignore  # message is not None
-
-    @discord.ui.button(
-        emoji="\N{LEFTWARDS ARROW WITH HOOK}",
-        style=discord.ButtonStyle.blurple,
-        row=2,
-    )
-    async def back_button(
-        self,
-        interaction: discord.Interaction,
-        button: discord.ui.Button,
-    ) -> None:
-        self.sources.pop()
-        await self.show_page(self.current_index)
-        await self._respond(interaction)
+#  Copyright (C) 2023 thegamecracks
+#  This Source Code Form is subject to the terms of the Mozilla Public
+#  License, v. 2.0. If a copy of the MPL was not distributed with this
+#  file, You can obtain one at http://mozilla.org/MPL/2.0/.
+import functools
+import math
+from abc import ABC, abstractmethod
+from enum import Enum, auto
+from typing import (
+    Any,
+    AsyncIterator,
+    Collection,
+    Coroutine,
+    Dict,
+    Generic,
+    Iterable,
+    List,
+    Optional,
+    Sequence,
+    Tuple,
+    TypedDict,
+    TypeVar,
+    Union,
+    cast,
+)
+
+import discord
+from typing_extensions import TypeAlias
+
+__version__ = "1.0.0.post1"
+
+__all__ = (
+    "PageOption",
+    "PageSource",
+    "ListPageSource",
+    "AsyncIteratorPageSource",
+    "TimeoutAction",
+    "PaginatorView",
+)
+
+E = TypeVar("E")
+T = TypeVar("T")
+S_co = TypeVar("S_co", bound="PageSource", covariant=True)
+V_contra = TypeVar("V_contra", bound="PaginatorView", contravariant=True)
+FP: TypeAlias = "Union[_PageParams, str, discord.Embed]"
+PO: TypeAlias = "Sequence[PageOption[S_co]]"
+
+
+class _PageParams(TypedDict, total=False):
+    content: str
+    embed: discord.Embed
+
+
+class PageOption(discord.SelectOption, Generic[S_co]):
+    """A select option that can store a nested page
+    through the added `source=` kwarg.
+    """
+
+    def __init__(self, *args, source: S_co, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.source = source
+
+
+class PageSource(ABC, Generic[T, S_co, V_contra]):
+    """The base page source class."""
+
+    def __init__(self, *, current_index: int = 0):
+        self.current_index = current_index
+
+    @abstractmethod
+    def get_page(self, index: int) -> Union[T, Coroutine[None, None, T]]:
+        """Returns a page based on the given index.
+
+        This method may be asynchronous.
+
+        """
+
+    @property
+    def max_pages(self) -> int:
+        """The max number of pages the page source can return.
+
+        Can return 0 to disable the view entirely.
+
+        """
+        return 1
+
+    def get_page_options(
+        self,
+        view: V_contra,
+        page: T,
+    ) -> Union[PO, Coroutine[None, None, PO]]:
+        """Returns a list of page options for the user to select.
+
+        This method may be asynchronous.
+
+        """
+        return []
+
+    @abstractmethod
+    def format_page(
+        self,
+        view: V_contra,
+        page: T,
+    ) -> Union[FP, Coroutine[None, None, FP]]:
+        """Returns a dictionary presenting the items in the page.
+
+        This method may be asynchronous.
+
+        """
+
+
+class ListPageSource(
+    PageSource[List[E], S_co, V_contra],
+    ABC,
+    Generic[E, S_co, V_contra],
+):
+    """Paginates a list of elements."""
+
+    def __init__(self, items: List[E], *args, page_size: int, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.items = items
+        self.page_size = page_size
+
+    def get_page(self, index: int) -> List[E]:
+        start = index * self.page_size
+        return self.items[start : start + self.page_size]
+
+    @functools.cached_property
+    def max_pages(self) -> int:
+        pages, remainder = divmod(len(self.items), self.page_size)
+        return pages + bool(remainder)
+
+
+class AsyncIteratorPageSource(
+    PageSource[List[E], S_co, V_contra],
+    ABC,
+    Generic[E, S_co, V_contra],
+):
+    """Paginates an async iterator."""
+
+    def __init__(self, iterator: AsyncIterator[E], *args, page_size: int, **kwargs):
+        super().__init__(*args, **kwargs)
+        self._cache: list[E] = []
+        self._iterator = iterator
+        self._max_index = 0
+        self._exhausted = False
+        self.page_size = page_size
+
+    async def get_page(self, index: int) -> List[E]:
+        start = index * self.page_size
+        end = start + self.page_size
+        if self._exhausted:
+            return self._cache[start:end]
+
+        # Get enough items to have at least one extra page
+        # so paginator knows if next/last buttons should turn off
+        required = end + self.page_size - len(self._cache)
+        if required > 0:
+            new_items = []
+            max_index = index + 1
+            for i in range(required):
+                try:
+                    new_items.append(await self._iterator.__anext__())
+                except StopAsyncIteration:
+                    max_index = math.ceil((len(self._cache) + i) / self.page_size)
+                    self._exhausted = True
+                    break
+            self._cache.extend(new_items)
+            self._max_index = max_index
+
+        return self._cache[start:end]
+
+    @property
+    def max_pages(self) -> int:
+        return self._max_index + (not self._exhausted)
+
+
+class TimeoutAction(Enum):
+    """Specifies what action should be taken when the view times out."""
+
+    NONE = auto()
+    """On timeout, no action will occur on the message."""
+    DISABLE = auto()
+    """On timeout, all components will be disabled."""
+    CLEAR = auto()
+    """On timeout, all components will be removed from the message."""
+    DELETE = auto()
+    """On timeout, the message will be deleted."""
+
+
+class PaginatorView(discord.ui.View, Generic[T, S_co, V_contra]):
+    """A view that handles pagination and recursive levels of pages.
+
+    To use this view, pass a PageSource or list of PageSources
+    (the last one will be displayed first) to the `sources=` kwarg,
+    then begin the paginator using `await view.start(channel)`.
+
+    If adding the view to another message is desired,
+    `view.message` must be manually set for it to be accessible.
+    The initial page is not rendered until the user interacts
+    with the paginator or is explicitly done with `await view.show_page()`.
+
+    `interaction_check` by default will return True if `allowed_users`
+    is None, or the interaction user is one of the allowed users.
+    This may be extended to include an interaction response, or use
+    different behavior entirely.
+
+    Parameters
+    ----------
+    :param sources: The current stack of page sources.
+    :param allowed_users: A collection of user IDs that are allowed
+        to interact with this paginator. If None, any user can interact.
+    :param timeout_action:
+        The action to do when the view times out. This may not have any
+        effect if a subclass overrides the `on_timeout()` method.
+
+    """
+
+    def __init__(
+        self,
+        *args,
+        sources: Union[
+            Iterable[PageSource[T, S_co, V_contra]],
+            PageSource[T, S_co, V_contra],
+        ],
+        allowed_users: Optional[Collection[int]] = None,
+        timeout_action: TimeoutAction = TimeoutAction.CLEAR,
+        **kwargs,
+    ):
+        super().__init__(*args, **kwargs)
+        if isinstance(sources, PageSource):
+            sources = [sources]
+        else:
+            self.sources = list(sources)
+            if len(self.sources) == 0:
+                raise ValueError("must provide at least one page source")
+        self.allowed_users = allowed_users
+        self.timeout_action = timeout_action
+
+        self.message: Optional[discord.Message] = None
+        self.page: _PageParams = {}
+        self.options: Sequence[PageOption[S_co]] = []
+        self.option_sources: dict[str, PageSource] = {}
+
+    @property
+    def current_source(self) -> PageSource[T, S_co, V_contra]:
+        return self.sources[-1]
+
+    @property
+    def current_index(self) -> int:
+        return self.current_source.current_index
+
+    @current_index.setter
+    def current_index(self, index: int):
+        self.current_source.current_index = index
+
+    @property
+    def can_navigate(self) -> bool:
+        return len(self.options) > 0
+
+    @property
+    def can_paginate(self) -> bool:
+        return self.current_source.max_pages > 1
+
+    @property
+    def can_go_back(self) -> bool:
+        return len(self.sources) > 1
+
+    @functools.cached_property
+    def _pagination_buttons(self) -> Tuple[discord.ui.Button, ...]:
+        return self.first_page, self.prev_page, self.next_page, self.last_page
+
+    async def show_page(self, index: int) -> None:
+        self.current_index = index
+        maybe_coro = discord.utils.maybe_coroutine
+
+        page = await maybe_coro(self.current_source.get_page, index)
+        params = await maybe_coro(self.current_source.format_page, self, page)  # type: ignore
+        if isinstance(params, str):
+            params = {"content": params}
+        elif isinstance(params, discord.Embed):
+            params = {"embed": params}
+        elif not isinstance(params, dict):
+            raise TypeError("format_page() must return a dict, str, or Embed")
+        self.page = cast(_PageParams, params)
+
+        options: Sequence[PageOption[S_co]] = await maybe_coro(
+            self.current_source.get_page_options, self, page  # type: ignore
+        )
+        option_sources = {}
+        for i, option in enumerate(options):
+            option.value = str(i)
+            option_sources[option.value] = option.source
+        self.options = options
+        self.option_sources = option_sources
+
+        self._refresh_components()
+
+    async def start(
+        self,
+        channel: Union[discord.abc.Messageable, discord.Interaction],
+        ephemeral: bool = True,
+    ) -> None:
+        await self.show_page(self.current_source.current_index)
+        if isinstance(channel, discord.Interaction):
+            kwargs = self._get_message_kwargs(initial_response=True)
+
+            if channel.response.is_done():
+                self.message = await channel.followup.send(
+                    ephemeral=ephemeral,
+                    wait=True,
+                    **kwargs,
+                )
+            else:
+                await channel.response.send_message(ephemeral=ephemeral, **kwargs)
+                self.message = await channel.original_response()
+        else:
+            self.message = await channel.send(**self._get_message_kwargs())
+
+    async def interaction_check(self, interaction: discord.Interaction) -> bool:
+        if self.allowed_users is not None:
+            return interaction.user.id in self.allowed_users
+        return True
+
+    async def on_timeout(self) -> None:
+        action = self.timeout_action
+        if self.message is None or action is TimeoutAction.NONE:
+            return
+
+        if action is TimeoutAction.CLEAR:
+            await self.message.edit(view=None)
+        elif action is TimeoutAction.DELETE:
+            await self.message.delete()
+        elif action is TimeoutAction.DISABLE:
+            for item in self.children:
+                if hasattr(item, "disabled"):
+                    item.disabled = True  # type: ignore
+
+            await self.message.edit(view=self)
+        else:
+            raise TypeError(f"unknown timeout action: {action!r}")
+
+    def _get_message_kwargs(self, *, initial_response: bool = False) -> Dict[str, Any]:
+        # initial_response indicates if we can use view=None, necessary as
+        # InteractionResponse.send_message() does not accept view=None
+        kwargs = dict(self.page)
+        max_pages = self.current_source.max_pages
+        can_interact = self.can_navigate or self.can_paginate or self.can_go_back
+
+        if max_pages > 0 and can_interact:
+            kwargs["view"] = self
+        else:
+            self.stop()
+            if not initial_response:
+                kwargs["view"] = None
+
+        return kwargs
+
+    async def _respond(self, interaction: discord.Interaction) -> None:
+        await interaction.response.edit_message(**self._get_message_kwargs())
+
+    # noinspection PyUnresolvedReferences
+    def _refresh_components(self) -> None:
+        """Update the state of each component in this view according to
+        the current source and page.
+
+        The pagination and back/stop buttons will be organized one of four ways:
+
+        1. No pagination, no previous source::
+            STOP
+        2. No pagination, previous source::
+            BACK STOP
+        3. Pagination, no previous source::
+            FIRST PREV NEXT LAST STOP
+        4. Pagination, previous source::
+            FIRST PREV NEXT LAST STOP
+            BACK
+
+        This applies the same when navigation is enabled.
+
+        """
+        self.clear_items()
+
+        # Navigation (select menu)
+        if self.can_navigate:
+            self.add_item(self.navigate)
+            self.navigate.options = list(self.options)
+
+        # Pagination (left/right)
+        if self.can_paginate:
+            for button in self._pagination_buttons:
+                self.add_item(button)
+
+        on_first_page = self.current_index == 0
+        on_last_page = self.current_index + 1 >= self.current_source.max_pages
+        self.first_page.disabled = on_first_page
+        self.prev_page.disabled = on_first_page
+        self.next_page.disabled = on_last_page
+        self.last_page.disabled = on_last_page
+
+        # Back and stop buttons
+        if self.can_go_back:
+            self.back_button.row = 1 + self.can_paginate
+            self.add_item(self.back_button)
+        self.add_item(self.stop_button)
+
+    @discord.ui.select(options=[], placeholder="Navigate...", row=0)
+    async def navigate(
+        self,
+        interaction: discord.Interaction,
+        select: discord.ui.Select,
+    ) -> None:
+        source = self.option_sources[select.values[0]]
+        self.sources.append(source)
+        await self.show_page(self.current_index)
+        await self._respond(interaction)
+
+    @discord.ui.button(
+        emoji="\N{BLACK LEFT-POINTING DOUBLE TRIANGLE WITH VERTICAL BAR}",
+        style=discord.ButtonStyle.blurple,
+        row=1,
+    )
+    async def first_page(
+        self,
+        interaction: discord.Interaction,
+        button: discord.ui.Button,
+    ) -> None:
+        await self.show_page(0)
+        await self._respond(interaction)
+
+    @discord.ui.button(
+        emoji="\N{BLACK LEFT-POINTING TRIANGLE}",
+        style=discord.ButtonStyle.blurple,
+        row=1,
+    )
+    async def prev_page(
+        self,
+        interaction: discord.Interaction,
+        button: discord.ui.Button,
+    ) -> None:
+        await self.show_page(self.current_index - 1)
+        await self._respond(interaction)
+
+    @discord.ui.button(
+        emoji="\N{BLACK RIGHT-POINTING TRIANGLE}",
+        style=discord.ButtonStyle.blurple,
+        row=1,
+    )
+    async def next_page(
+        self,
+        interaction: discord.Interaction,
+        button: discord.ui.Button,
+    ) -> None:
+        await self.show_page(self.current_index + 1)
+        await self._respond(interaction)
+
+    @discord.ui.button(
+        emoji="\N{BLACK RIGHT-POINTING DOUBLE TRIANGLE WITH VERTICAL BAR}",
+        style=discord.ButtonStyle.blurple,
+        row=1,
+    )
+    async def last_page(
+        self,
+        interaction: discord.Interaction,
+        button: discord.ui.Button,
+    ) -> None:
+        await self.show_page(self.current_source.max_pages - 1)
+        await self._respond(interaction)
+
+    @discord.ui.button(
+        emoji="\N{THUMBS UP SIGN}",
+        style=discord.ButtonStyle.success,
+        row=1,
+    )
+    async def stop_button(
+        self,
+        interaction: discord.Interaction,
+        button: discord.ui.Button,
+    ) -> None:
+        self.stop()
+        await interaction.message.delete()  # type: ignore  # message is not None
+
+    @discord.ui.button(
+        emoji="\N{LEFTWARDS ARROW WITH HOOK}",
+        style=discord.ButtonStyle.blurple,
+        row=2,
+    )
+    async def back_button(
+        self,
+        interaction: discord.Interaction,
+        button: discord.ui.Button,
+    ) -> None:
+        self.sources.pop()
+        await self.show_page(self.current_index)
+        await self._respond(interaction)
```

### Comparing `discord-ext-pager-1.0.0/src/discord_ext_pager.egg-info/PKG-INFO` & `discord-ext-pager-1.0.0.post1/src/discord_ext_pager.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,132 +1,140 @@
-Metadata-Version: 2.1
-Name: discord-ext-pager
-Version: 1.0.0
-Summary: A view-based paginator library for discord.py 2.0
-Author: thegamecracks
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Framework :: AsyncIO
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved
-Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Software Development
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Typing :: Typed
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# discord-ext-pager
-
-A simple view-based paginator library for discord.py 2.0.
-
-## Installation
-
-This package is available on pip as `discord-ext-pager`.
-If you have Git, you may also choose to install the latest version
-using `pip install git+https://github.com/thegamecracks/discord-ext-pager`.
-
-## Basic Usage
-
-Prior users of Danny's [`discord-ext-menus`] will find some familiarity
-in this library. Provided are the following classes:
-
-- PaginatorView:
-  The view class that manages the paginator.
-- PageSource:
-  The base class for sources the paginator view can accept.
-- ListPageSource:
-  The base class for formatting a list of items.
-- AsyncIteratorPageSource:
-  The base class for formatting an asynchronous iterator of items.
-- PageOption:
-  A subclass of `discord.SelectOption` that also stores a `PageSource` instance.
-  Used for the navigation select menu.
-- TimeoutAction:
-  An enum for customizing PaginatorView's timeout behaviour.
-
-The `PaginatorView` can be instantiated and used by itself, but page formatting
-is handled by subclassing one of the `PageSource` base classes.
-
-```py
-from typing import Any, List
-from discord.ext.pager import ListPageSource, PaginatorView
-
-class EmbedListPageSource(ListPageSource[Any, None, PaginatorView]):
-    """Takes a list of items and formats it in an embed."""
-
-    def format_page(self, view: PaginatorView, page: List[Any]):
-        index = self.current_index * self.page_size
-        description = "\n".join(
-            f"{i}. {x}"
-            for i, x in enumerate(page, start=index + 1)
-        )
-        return discord.Embed(description=description)
-
-# Anywhere a channel or interaction is available:
-fruits = ["🍎 Apple", "🍊 Orange", "🍋 Lemon"]
-source = EmbedListPageSource(fruits, page_size=2)
-view = PaginatorView(sources=source, timeout=180)
-await view.start(interaction)
-```
-
-If the navigation select menu is desired, the `get_page_options()` method
-should be overridden to return a list of `PageOption` objects for the user
-to select from:
-
-```py
-from typing import List
-from discord.ext.pager import ListPageSource, PageOption, PaginatorView, PageSource
-
-class MessageSource(PageSource[str, None, PaginatorView]):
-    """A single page for displaying a string."""
-
-    def __init__(self, message: str, *, current_index: int = 0):
-        super().__init__(current_index=current_index)
-        self.message = message
-
-    def get_page(self, index: int):
-        return self.message
-
-    def format_page(self, view: PaginatorView, page: str):
-        # If we don't specify both content and embed, either will
-        # persist as the user clicks between options
-        return {"content": page, "embed": None}
-
-class MessageNavigator(ListPageSource[MessageSource, MessageSource, PaginatorView]):
-    """A list of messages for the user to select from."""
-
-    def get_page_options(self, view: PaginatorView, page: List[MessageSource]):
-        return [PageOption(source=source, label=source.message) for source in page]
-
-    def format_page(self, view: PaginatorView, page: List[MessageSource]):
-        description = "\n".join(source.message for source in page)
-        embed = discord.Embed(description=description)
-        return {"content": None, "embed": embed}
-
-hands = "👈👉👆👇🫵🤞🫰🤘🤙🤛🤜✊👊👋👏🙌"
-source = MessageNavigator([MessageSource(s) for s in hands], page_size=5)
-view = PaginatorView(sources=source)
-await view.start(ctx)
-```
-
-When an option is selected, the `PageSource` contained within that option
-is appended to `PaginatorView.sources`, causing that source to be displayed.
-Another button is automatically provided for users to back out to the last
-page source. This can be manually triggered by passing a list of page sources
-to the `PaginatorView(sources=)` argument.
-
-[`discord-ext-menus`]: https://github.com/Rapptz/discord-ext-menus
-
-## Examples
-
-Click on each example to see the source code:
-
-[![Tag leaderboard](https://github.com/thegamecracks/discord-ext-pager/blob/main/docs/images/thegamebot_tags.png?raw=true)](https://github.com/thegamecracks/thegamebot/blob/04d9909877685acd24654a911b1853e2143fc316/bot/cogs/tags/__init__.py#L123-L162)
-
-[![Help command](https://github.com/thegamecracks/discord-ext-pager/blob/main/docs/images/thegamebot_help.png?raw=true)](https://github.com/thegamecracks/thegamebot/blob/04d9909877685acd24654a911b1853e2143fc316/bot/cogs/helpcommand.py#L26-L249)
+Metadata-Version: 2.1
+Name: discord-ext-pager
+Version: 1.0.0.post1
+Summary: A view-based paginator library for discord.py 2.0
+Author: thegamecracks
+Keywords: discord,discord.py,paginator,view
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Framework :: AsyncIO
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved
+Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Typing :: Typed
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# discord-ext-pager
+
+[![PyPI](https://img.shields.io/pypi/v/discord-ext-pager?label=View%20on%20pypi&style=flat-square)](https://pypi.org/project/discord-ext-pager/)
+
+A simple view-based paginator library for discord.py 2.0.
+
+## Installation
+
+[discord-ext-pager] is available on PyPI, and as such can be installed using pip.
+
+[discord-ext-pager]: https://pypi.org/project/discord-ext-pager/
+
+## Usage
+
+Users of Danny's [discord-ext-menus] will find some familiarity
+in this library. Provided are the following classes:
+
+- PaginatorView:
+  The view class that manages pagination and navigation.
+- PageSource:
+  The base class for sources the paginator view can accept.
+- ListPageSource:
+  The base class for formatting a list of items.
+- AsyncIteratorPageSource:
+  The base class for formatting an asynchronous iterator of items.
+- PageOption:
+  A subclass of `discord.SelectOption` used for presenting navigation options.
+- TimeoutAction:
+  An enum for customizing PaginatorView's timeout behaviour.
+
+[discord-ext-menus]: https://github.com/Rapptz/discord-ext-menus
+
+The `PaginatorView` can be instantiated and used by itself, but page formatting
+is handled by subclassing one of the `PageSource` base classes.
+
+```py
+from typing import Any, List
+from discord.ext.pager import ListPageSource, PaginatorView
+
+class EmbedListPageSource(ListPageSource[Any, None, PaginatorView]):
+    #                                   ^^^^^^^^^^^^^^^^^^^^^^^^^^
+    #            These type parameters denote the page item type,
+    #            source type for page options (demonstrated later),
+    #            and view type. Only needed for static typing.
+    """Takes a list of items and formats it in an embed."""
+
+    def format_page(self, view: PaginatorView, page: List[Any]):
+        index = self.current_index * self.page_size
+        description = "\n".join(
+            f"{i}. {x}"
+            for i, x in enumerate(page, start=index + 1)
+        )
+        return discord.Embed(description=description)
+
+# Anywhere a channel or interaction is available:
+fruits = ["🍎 Apple", "🍊 Orange", "🍋 Lemon"]
+source = EmbedListPageSource(fruits, page_size=2)
+view = PaginatorView(sources=source, timeout=180)
+await view.start(interaction)
+```
+
+If the navigation select menu is desired, the `get_page_options()` method
+should be overridden to return a list of `PageOption` objects for the user
+to select from:
+
+```py
+from typing import List
+from discord.ext.pager import ListPageSource, PageOption, PageSource, PaginatorView
+
+class MessageSource(PageSource[str, None, PaginatorView]):
+    """A single page for displaying a string."""
+
+    def __init__(self, message: str, *, current_index: int = 0):
+        super().__init__(current_index=current_index)
+        self.message = message
+
+    def get_page(self, index: int):
+        return self.message
+
+    def format_page(self, view: PaginatorView, page: str):
+        # If we don't specify both content and embed, either will
+        # persist as the user clicks between options
+        return {"content": page, "embed": None}
+
+class MessageNavigator(ListPageSource[MessageSource, MessageSource, PaginatorView]):
+    """A list of messages for the user to select from."""
+
+    def get_page_options(self, view: PaginatorView, page: List[MessageSource]):
+        # PageOption() takes the same arguments as discord.SelectOption,
+        # except that source= is also required
+        return [PageOption(source=source, label=source.message) for source in page]
+
+    def format_page(self, view: PaginatorView, page: List[MessageSource]):
+        description = "\n".join(source.message for source in page)
+        embed = discord.Embed(description=description)
+        return {"content": None, "embed": embed}
+
+hands = "👈👉👆👇🫵🤞🫰🤘🤙🤛🤜✊👊👋👏🙌"
+source = MessageNavigator([MessageSource(s) for s in hands], page_size=5)
+view = PaginatorView(sources=source)
+await view.start(ctx)
+```
+
+When an option is selected, the `PageSource` contained within that option
+is appended to `PaginatorView.sources`, causing that source to be displayed.
+Another button is automatically provided for users to back out to the last
+page source. This can be manually triggered by passing a list of page sources
+to the `PaginatorView(sources=)` argument.
+
+## Examples
+
+Click on an example below to see its source code:
+
+[![Tag leaderboard](https://github.com/thegamecracks/discord-ext-pager/blob/main/docs/images/thegamebot_tags.png?raw=true)](https://github.com/thegamecracks/thegamebot/blob/04d9909877685acd24654a911b1853e2143fc316/bot/cogs/tags/__init__.py#L123-L162)
+
+[![Help command](https://github.com/thegamecracks/discord-ext-pager/blob/main/docs/images/thegamebot_help.png?raw=true)](https://github.com/thegamecracks/thegamebot/blob/04d9909877685acd24654a911b1853e2143fc316/bot/cogs/helpcommand.py#L26-L249)
```

